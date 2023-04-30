# Comparing `tmp/nonebot_plugin_og-0.1.0.tar.gz` & `tmp/nonebot_plugin_og-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_og-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_og-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_og-0.1.0.tar` & `nonebot_plugin_og-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-04-30 07:04:55.926537 nonebot_plugin_og-0.1.0/LICENSE
--rw-r--r--   0        0        0     1713 2023-04-30 07:04:55.926537 nonebot_plugin_og-0.1.0/README.md
--rw-r--r--   0        0        0      986 2023-04-30 07:04:55.926537 nonebot_plugin_og-0.1.0/nonebot_plugin_og/__init__.py
--rw-r--r--   0        0        0      768 2023-04-30 07:04:55.926537 nonebot_plugin_og-0.1.0/nonebot_plugin_og/utils.py
--rw-r--r--   0        0        0      452 2023-04-30 07:04:55.926537 nonebot_plugin_og-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 nonebot_plugin_og-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-30 08:00:49.030113 nonebot_plugin_og-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2072 2023-04-30 08:00:49.030113 nonebot_plugin_og-0.2.0/README.md
+-rw-r--r--   0        0        0      873 2023-04-30 08:00:49.030113 nonebot_plugin_og-0.2.0/nonebot_plugin_og/__init__.py
+-rw-r--r--   0        0        0      768 2023-04-30 08:00:49.030113 nonebot_plugin_og-0.2.0/nonebot_plugin_og/utils.py
+-rw-r--r--   0        0        0      973 2023-04-30 08:00:49.030113 nonebot_plugin_og-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 nonebot_plugin_og-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_og-0.1.0/LICENSE` & `nonebot_plugin_og-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_og-0.1.0/README.md` & `nonebot_plugin_og-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,130 @@
 00000000: 0a3c 6469 7620 616c 6967 6e3d 2263 656e  .<div align="cen
 00000010: 7465 7222 3e0a 0a23 204e 6f6e 6562 6f74  ter">..# Nonebot
 00000020: 2d70 6c75 6769 6e2d 6f67 0a0a 5fe2 9ca8  -plugin-og.._...
 00000030: 20e6 a380 e6b5 8be9 93be e68e a5e5 b9b6   ...............
 00000040: e794 9fe6 8890 e9a2 84e8 a788 e59b be20  ............... 
-00000050: e29c a85f 2020 0a0a 3c2f 6469 763e 0a0a  ..._  ..</div>..
-00000060: 2323 20f0 9f93 9620 e4bb 8be7 bb8d 0a0a  ## .... ........
-00000070: e6a3 80e6 b58b e993 bee6 8ea5 e5b9 b6e7  ................
-00000080: 949f e688 90e9 a284 e8a7 88e5 9bbe efbc  ................
-00000090: 8ce5 9fba e4ba 8e20 5b4f 7065 6e20 4772  ....... [Open Gr
-000000a0: 6170 685d 2868 7474 7073 3a2f 2f6f 6770  aph](https://ogp
-000000b0: 2e6d 652f 2920 e58d 8fe8 aeae 0a0a 2323  .me/) ........##
-000000c0: 20f0 9f92 bf20 e5ae 89e8 a385 0a0a 3c64   .... ........<d
-000000d0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-000000e0: 3ee4 bdbf e794 a820 6e62 2d63 6c69 20e5  >...... nb-cli .
-000000f0: ae89 e8a3 853c 2f73 756d 6d61 7279 3e0a  .....</summary>.
-00000100: e59c a820 6e6f 6e65 626f 7432 20e9 a1b9  ... nonebot2 ...
-00000110: e79b aee7 9a84 e6a0 b9e7 9bae e5bd 95e4  ................
-00000120: b88b e689 93e5 bc80 e591 bde4 bba4 e8a1  ................
-00000130: 8c2c 20e8 be93 e585 a5e4 bba5 e4b8 8be6  ., .............
-00000140: 8c87 e4bb a4e5 8db3 e58f afe5 ae89 e8a3  ................
-00000150: 850a 0a20 2020 206e 6220 706c 7567 696e  ...    nb plugin
-00000160: 2069 6e73 7461 6c6c 206e 6f6e 6562 6f74   install nonebot
-00000170: 2d70 6c75 6769 6e2d 6f67 0a0a 3c2f 6465  -plugin-og..</de
-00000180: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
-00000190: 3e0a 3c73 756d 6d61 7279 3ee4 bdbf e794  >.<summary>.....
-000001a0: a870 6970 e5ae 89e8 a385 3c2f 7375 6d6d  .pip......</summ
-000001b0: 6172 793e 0ae5 9ca8 206e 6f6e 6562 6f74  ary>.... nonebot
-000001c0: 3220 e9a1 b9e7 9bae e79a 84e6 8f92 e4bb  2 ..............
-000001d0: b6e7 9bae e5bd 95e4 b88b 2c20 e689 93e5  .........., ....
-000001e0: bc80 e591 bde4 bba4 e8a1 8c2c 20e8 be93  ..........., ...
-000001f0: e585 a5e4 bba5 e4b8 8be6 8c87 e4bb a4e5  ................
-00000200: 8db3 e58f afe5 ae89 e8a3 850a 0a20 2020  .............   
-00000210: 2070 6970 2069 716e 7374 616c 6c20 6e6f   pip iqnstall no
-00000220: 6e65 626f 742d 706c 7567 696e 2d6f 670a  nebot-plugin-og.
-00000230: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a e689  .</details>.....
-00000240: 93e5 bc80 206e 6f6e 6562 6f74 3220 e9a1  .... nonebot2 ..
-00000250: b9e7 9bae e6a0 b9e7 9bae e5bd 95e4 b88b  ................
-00000260: e79a 8420 6070 7970 726f 6a65 6374 2e74  ... `pyproject.t
-00000270: 6f6d 6c60 20e6 9687 e4bb b62c 20e5 9ca8  oml` ......, ...
-00000280: 2060 5b74 6f6f 6c2e 6e6f 6e65 626f 745d   `[tool.nonebot]
-00000290: 6020 e983 a8e5 8886 e8bf bde5 8aa0 e586  ` ..............
-000002a0: 99e5 85a5 0a0a 2020 2020 706c 7567 696e  ......    plugin
-000002b0: 7320 3d20 5b22 6e6f 6e65 626f 745f 706c  s = ["nonebot_pl
-000002c0: 7567 696e 5f6f 6722 5d0a 0a0a 2323 20f0  ugin_og"]...## .
-000002d0: 9f8e 8920 e4bd bfe7 94a8 0a0a e79b b4e6  ... ............
-000002e0: 8ea5 e58f 91e9 8081 e4bb bbe6 848f e993  ................
-000002f0: bee6 8ea5 efbc 8ce5 8faa e8a6 81e6 98af  ................
-00000300: e694 afe6 8c81 204f 7065 6e20 4772 6170  ...... Open Grap
-00000310: 6820 e58d 8fe8 aeae e79a 84e7 bd91 e7ab  h ..............
-00000320: 99ef bc8c e6ad a4e6 8f92 e4bb b6e9 83bd  ................
-00000330: e4bc 9ae8 87aa e58a a8e5 8f91 e980 81e9  ................
-00000340: a284 e8a7 88e5 9bbe e380 820a 0a23 2320  .............## 
-00000350: e9b8 a3e8 b0a2 0a0a 2a20 5b60 6e6f 6e65  ........* [`none
-00000360: 626f 742f 6e6f 656e 626f 7432 605d 2868  bot/noenbot2`](h
-00000370: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000380: 6d2f 6e6f 6e65 626f 742f 6e6f 6e65 626f  m/nonebot/nonebo
-00000390: 7432 29ef bc9a e8b7 a8e5 b9b3 e58f b050  t2)............P
-000003a0: 7974 686f 6ee5 bc82 e6ad a5e6 9cba e599  ython...........
-000003b0: a8e4 baba e6a1 86e6 9eb6 0a2a 205b 604d  ...........* [`M
-000003c0: 7273 3473 2f67 6f2d 6371 6874 7470 605d  rs4s/go-cqhttp`]
-000003d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000003e0: 636f 6d2f 4d72 7334 732f 676f 2d63 7168  com/Mrs4s/go-cqh
-000003f0: 7474 7029 efbc 9a63 7168 7474 70e7 9a84  ttp)...cqhttp...
-00000400: 676f 6c61 6e67 e5ae 9ee7 8eb0 efbc 8ce8  golang..........
-00000410: bdbb e987 8fe3 8081 e58e 9fe7 949f e8b7  ................
-00000420: a8e5 b9b3 e58f b02e 0a2a 205b 606b 6f69  .........* [`koi
-00000430: 7368 696a 732f 6b6f 6973 6869 2d70 6c75  shijs/koishi-plu
-00000440: 6769 6e2d 6f67 605d 2868 7474 7073 3a2f  gin-og`](https:/
-00000450: 2f67 6974 6875 622e 636f 6d2f 6b6f 6973  /github.com/kois
-00000460: 6869 6a73 2f6b 6f69 7368 692d 706c 7567  hijs/koishi-plug
-00000470: 696e 2d6f 6729 efbc 9ae6 9cac e9a1 b9e7  in-og)..........
-00000480: 9bae e79b b4e6 8ea5 e58f 82e8 8083 207e  .............. ~
-00000490: 7eef bc88 e79b b4e6 8ea5 e5bc 80e6 8a84  ~...............
-000004a0: 7e7e 0a0a 0a23 2320 e5bc 80e6 ba90 e8ae  ~~...## ........
-000004b0: b8e5 8faf e8af 810a 0ae4 bdbf e794 a820  ............... 
-000004c0: 5b4d 4954 5d28 2329 20e8 aeb8 e58f afe8  [MIT](#) .......
-000004d0: af81 e58f 91e5 b883 e380 820a 0a60 6060  .............```
-000004e0: 0a54 4845 2053 4f46 5457 4152 4520 4953  .THE SOFTWARE IS
-000004f0: 2050 524f 5649 4445 4420 2241 5320 4953   PROVIDED "AS IS
-00000500: 222c 2057 4954 484f 5554 2057 4152 5241  ", WITHOUT WARRA
-00000510: 4e54 5920 4f46 2041 4e59 204b 494e 442c  NTY OF ANY KIND,
-00000520: 2045 5850 5245 5353 204f 520a 494d 504c   EXPRESS OR.IMPL
-00000530: 4945 442c 2049 4e43 4c55 4449 4e47 2042  IED, INCLUDING B
-00000540: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
-00000550: 4f20 5448 4520 5741 5252 414e 5449 4553  O THE WARRANTIES
-00000560: 204f 4620 4d45 5243 4841 4e54 4142 494c   OF MERCHANTABIL
-00000570: 4954 592c 2046 4954 4e45 5353 0a46 4f52  ITY, FITNESS.FOR
-00000580: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
-00000590: 5250 4f53 4520 414e 4420 4e4f 4e49 4e46  RPOSE AND NONINF
-000005a0: 5249 4e47 454d 454e 542e 2049 4e20 4e4f  RINGEMENT. IN NO
-000005b0: 2045 5645 4e54 2053 4841 4c4c 2054 4845   EVENT SHALL THE
-000005c0: 2041 5554 484f 5253 204f 520a 434f 5059   AUTHORS OR.COPY
-000005d0: 5249 4748 5420 484f 4c44 4552 5320 4245  RIGHT HOLDERS BE
-000005e0: 204c 4941 424c 4520 464f 5220 414e 5920   LIABLE FOR ANY 
-000005f0: 434c 4149 4d2c 2044 414d 4147 4553 204f  CLAIM, DAMAGES O
-00000600: 5220 4f54 4845 5220 4c49 4142 494c 4954  R OTHER LIABILIT
-00000610: 592c 2057 4845 5448 4552 0a49 4e20 414e  Y, WHETHER.IN AN
-00000620: 2041 4354 494f 4e20 4f46 2043 4f4e 5452   ACTION OF CONTR
-00000630: 4143 542c 2054 4f52 5420 4f52 204f 5448  ACT, TORT OR OTH
-00000640: 4552 5749 5345 2c20 4152 4953 494e 4720  ERWISE, ARISING 
-00000650: 4652 4f4d 2c20 4f55 5420 4f46 204f 5220  FROM, OUT OF OR 
-00000660: 494e 0a43 4f4e 4e45 4354 494f 4e20 5749  IN.CONNECTION WI
-00000670: 5448 2054 4845 2053 4f46 5457 4152 4520  TH THE SOFTWARE 
-00000680: 4f52 2054 4845 2055 5345 204f 5220 4f54  OR THE USE OR OT
-00000690: 4845 5220 4445 414c 494e 4753 2049 4e20  HER DEALINGS IN 
-000006a0: 5448 4520 534f 4654 5741 5245 2e0a 6060  THE SOFTWARE..``
-000006b0: 60                                       `
+00000050: e29c a85f 2020 0a0a 3c61 2068 7265 663d  ..._  ..<a href=
+00000060: 222e 2f4c 4943 454e 5345 223e 0a20 2020  "./LICENSE">.   
+00000070: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000080: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000090: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+000000a0: 2f6d 7574 6532 332d 636f 6465 2f6e 6f6e  /mute23-code/non
+000000b0: 6562 6f74 5f70 6c75 6769 6e5f 6f67 2220  ebot_plugin_og" 
+000000c0: 616c 743d 226c 6963 656e 7365 223e 0a3c  alt="license">.<
+000000d0: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
+000000e0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
+000000f0: 2e6f 7267 2f70 7970 692f 6e6f 6e65 626f  .org/pypi/nonebo
+00000100: 745f 706c 7567 696e 5f6f 6722 3e0a 2020  t_plugin_og">.  
+00000110: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000120: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000130: 696f 2f70 7970 692f 762f 6e6f 6e65 626f  io/pypi/v/nonebo
+00000140: 745f 706c 7567 696e 5f6f 672e 7376 6722  t_plugin_og.svg"
+00000150: 2061 6c74 3d22 7079 7069 223e 0a3c 2f61   alt="pypi">.</a
+00000160: 3e0a 3c69 6d67 2073 7263 3d22 6874 7470  >.<img src="http
+00000170: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000180: 696f 2f62 6164 6765 2f70 7974 686f 6e2d  io/badge/python-
+00000190: 332e 382b 2d62 6c75 652e 7376 6722 2061  3.8+-blue.svg" a
+000001a0: 6c74 3d22 7079 7468 6f6e 223e 0a0a 0a3c  lt="python">...<
+000001b0: 2f64 6976 3e0a 0a20 2020 2023 2320 f09f  /div>..    ## ..
+000001c0: 9396 20e4 bb8b e7bb 8d0a 0a20 2020 20e6  .. ........    .
+000001d0: a380 e6b5 8be9 93be e68e a5e5 b9b6 e794  ................
+000001e0: 9fe6 8890 e9a2 84e8 a788 e59b beef bc8c  ................
+000001f0: e59f bae4 ba8e 205b 4f70 656e 2047 7261  ...... [Open Gra
+00000200: 7068 5d28 6874 7470 733a 2f2f 6f67 702e  ph](https://ogp.
+00000210: 6d65 2f29 20e5 8d8f e8ae ae0a 0a23 2320  me/) ........## 
+00000220: f09f 92bf 20e5 ae89 e8a3 850a 0a3c 6465  .... ........<de
+00000230: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
+00000240: e4bd bfe7 94a8 206e 622d 636c 6920 e5ae  ...... nb-cli ..
+00000250: 89e8 a385 3c2f 7375 6d6d 6172 793e 0ae5  ....</summary>..
+00000260: 9ca8 206e 6f6e 6562 6f74 3220 e9a1 b9e7  .. nonebot2 ....
+00000270: 9bae e79a 84e6 a0b9 e79b aee5 bd95 e4b8  ................
+00000280: 8be6 8993 e5bc 80e5 91bd e4bb a4e8 a18c  ................
+00000290: 2c20 e8be 93e5 85a5 e4bb a5e4 b88b e68c  , ..............
+000002a0: 87e4 bba4 e58d b3e5 8faf e5ae 89e8 a385  ................
+000002b0: 0a0a 2020 2020 6e62 2070 6c75 6769 6e20  ..    nb plugin 
+000002c0: 696e 7374 616c 6c20 6e6f 6e65 626f 742d  install nonebot-
+000002d0: 706c 7567 696e 2d6f 670a 0a3c 2f64 6574  plugin-og..</det
+000002e0: 6169 6c73 3e0a 0a3c 6465 7461 696c 733e  ails>..<details>
+000002f0: 0a3c 7375 6d6d 6172 793e e4bd bfe7 94a8  .<summary>......
+00000300: 7069 70e5 ae89 e8a3 853c 2f73 756d 6d61  pip......</summa
+00000310: 7279 3e0a e59c a820 6e6f 6e65 626f 7432  ry>.... nonebot2
+00000320: 20e9 a1b9 e79b aee7 9a84 e68f 92e4 bbb6   ...............
+00000330: e79b aee5 bd95 e4b8 8b2c 20e6 8993 e5bc  ........., .....
+00000340: 80e5 91bd e4bb a4e8 a18c 2c20 e8be 93e5  .........., ....
+00000350: 85a5 e4bb a5e4 b88b e68c 87e4 bba4 e58d  ................
+00000360: b3e5 8faf e5ae 89e8 a385 0a0a 2020 2020  ............    
+00000370: 7069 7020 6971 6e73 7461 6c6c 206e 6f6e  pip iqnstall non
+00000380: 6562 6f74 2d70 6c75 6769 6e2d 6f67 0a0a  ebot-plugin-og..
+00000390: 3c2f 6465 7461 696c 733e 0a0a 0ae6 8993  </details>......
+000003a0: e5bc 8020 6e6f 6e65 626f 7432 20e9 a1b9  ... nonebot2 ...
+000003b0: e79b aee6 a0b9 e79b aee5 bd95 e4b8 8be7  ................
+000003c0: 9a84 2060 7079 7072 6f6a 6563 742e 746f  .. `pyproject.to
+000003d0: 6d6c 6020 e696 87e4 bbb6 2c20 e59c a820  ml` ......, ... 
+000003e0: 605b 746f 6f6c 2e6e 6f6e 6562 6f74 5d60  `[tool.nonebot]`
+000003f0: 20e9 83a8 e588 86e8 bfbd e58a a0e5 8699   ...............
+00000400: e585 a50a 0a20 2020 2070 6c75 6769 6e73  .....    plugins
+00000410: 203d 205b 226e 6f6e 6562 6f74 5f70 6c75   = ["nonebot_plu
+00000420: 6769 6e5f 6f67 225d 0a0a 0a23 2320 f09f  gin_og"]...## ..
+00000430: 8e89 20e4 bdbf e794 a80a 0ae7 9bb4 e68e  .. .............
+00000440: a5e5 8f91 e980 81e4 bbbb e684 8fe9 93be  ................
+00000450: e68e a5ef bc8c e58f aae8 a681 e698 afe6  ................
+00000460: 94af e68c 8120 4f70 656e 2047 7261 7068  ..... Open Graph
+00000470: 20e5 8d8f e8ae aee7 9a84 e7bd 91e7 ab99   ...............
+00000480: efbc 8ce6 ada4 e68f 92e4 bbb6 e983 bde4  ................
+00000490: bc9a e887 aae5 8aa8 e58f 91e9 8081 e9a2  ................
+000004a0: 84e8 a788 e59b bee3 8082 0a0a 2323 20e9  ............## .
+000004b0: b8a3 e8b0 a20a 0a2a 205b 606e 6f6e 6562  .......* [`noneb
+000004c0: 6f74 2f6e 6f65 6e62 6f74 3260 5d28 6874  ot/noenbot2`](ht
+000004d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000004e0: 2f6e 6f6e 6562 6f74 2f6e 6f6e 6562 6f74  /nonebot/nonebot
+000004f0: 3229 efbc 9ae8 b7a8 e5b9 b3e5 8fb0 5079  2)............Py
+00000500: 7468 6f6e e5bc 82e6 ada5 e69c bae5 99a8  thon............
+00000510: e4ba bae6 a186 e69e b60a 2a20 5b60 4d72  ..........* [`Mr
+00000520: 7334 732f 676f 2d63 7168 7474 7060 5d28  s4s/go-cqhttp`](
+00000530: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000540: 6f6d 2f4d 7273 3473 2f67 6f2d 6371 6874  om/Mrs4s/go-cqht
+00000550: 7470 29ef bc9a 6371 6874 7470 e79a 8467  tp)...cqhttp...g
+00000560: 6f6c 616e 67e5 ae9e e78e b0ef bc8c e8bd  olang...........
+00000570: bbe9 878f e380 81e5 8e9f e794 9fe8 b7a8  ................
+00000580: e5b9 b3e5 8fb0 2e0a 2a20 5b60 6b6f 6973  ........* [`kois
+00000590: 6869 6a73 2f6b 6f69 7368 692d 706c 7567  hijs/koishi-plug
+000005a0: 696e 2d6f 6760 5d28 6874 7470 733a 2f2f  in-og`](https://
+000005b0: 6769 7468 7562 2e63 6f6d 2f6b 6f69 7368  github.com/koish
+000005c0: 696a 732f 6b6f 6973 6869 2d70 6c75 6769  ijs/koishi-plugi
+000005d0: 6e2d 6f67 29ef bc9a e69c ace9 a1b9 e79b  n-og)...........
+000005e0: aee7 9bb4 e68e a5e5 8f82 e880 8320 7e7e  ............. ~~
+000005f0: efbc 88e7 9bb4 e68e a5e5 bc80 e68a 847e  ...............~
+00000600: 7e0a 0a0a 2323 20e5 bc80 e6ba 90e8 aeb8  ~...## .........
+00000610: e58f afe8 af81 0a0a e4bd bfe7 94a8 205b  .............. [
+00000620: 4d49 545d 282e 2f4c 4943 454e 5345 2920  MIT](./LICENSE) 
+00000630: e8ae b8e5 8faf e8af 81e5 8f91 e5b8 83e3  ................
+00000640: 8082 0a0a 6060 600a 5448 4520 534f 4654  ....```.THE SOFT
+00000650: 5741 5245 2049 5320 5052 4f56 4944 4544  WARE IS PROVIDED
+00000660: 2022 4153 2049 5322 2c20 5749 5448 4f55   "AS IS", WITHOU
+00000670: 5420 5741 5252 414e 5459 204f 4620 414e  T WARRANTY OF AN
+00000680: 5920 4b49 4e44 2c20 4558 5052 4553 5320  Y KIND, EXPRESS 
+00000690: 4f52 0a49 4d50 4c49 4544 2c20 494e 434c  OR.IMPLIED, INCL
+000006a0: 5544 494e 4720 4255 5420 4e4f 5420 4c49  UDING BUT NOT LI
+000006b0: 4d49 5445 4420 544f 2054 4845 2057 4152  MITED TO THE WAR
+000006c0: 5241 4e54 4945 5320 4f46 204d 4552 4348  RANTIES OF MERCH
+000006d0: 414e 5441 4249 4c49 5459 2c20 4649 544e  ANTABILITY, FITN
+000006e0: 4553 530a 464f 5220 4120 5041 5254 4943  ESS.FOR A PARTIC
+000006f0: 554c 4152 2050 5552 504f 5345 2041 4e44  ULAR PURPOSE AND
+00000700: 204e 4f4e 494e 4652 494e 4745 4d45 4e54   NONINFRINGEMENT
+00000710: 2e20 494e 204e 4f20 4556 454e 5420 5348  . IN NO EVENT SH
+00000720: 414c 4c20 5448 4520 4155 5448 4f52 5320  ALL THE AUTHORS 
+00000730: 4f52 0a43 4f50 5952 4947 4854 2048 4f4c  OR.COPYRIGHT HOL
+00000740: 4445 5253 2042 4520 4c49 4142 4c45 2046  DERS BE LIABLE F
+00000750: 4f52 2041 4e59 2043 4c41 494d 2c20 4441  OR ANY CLAIM, DA
+00000760: 4d41 4745 5320 4f52 204f 5448 4552 204c  MAGES OR OTHER L
+00000770: 4941 4249 4c49 5459 2c20 5748 4554 4845  IABILITY, WHETHE
+00000780: 520a 494e 2041 4e20 4143 5449 4f4e 204f  R.IN AN ACTION O
+00000790: 4620 434f 4e54 5241 4354 2c20 544f 5254  F CONTRACT, TORT
+000007a0: 204f 5220 4f54 4845 5257 4953 452c 2041   OR OTHERWISE, A
+000007b0: 5249 5349 4e47 2046 524f 4d2c 204f 5554  RISING FROM, OUT
+000007c0: 204f 4620 4f52 2049 4e0a 434f 4e4e 4543   OF OR IN.CONNEC
+000007d0: 5449 4f4e 2057 4954 4820 5448 4520 534f  TION WITH THE SO
+000007e0: 4654 5741 5245 204f 5220 5448 4520 5553  FTWARE OR THE US
+000007f0: 4520 4f52 204f 5448 4552 2044 4541 4c49  E OR OTHER DEALI
+00000800: 4e47 5320 494e 2054 4845 2053 4f46 5457  NGS IN THE SOFTW
+00000810: 4152 452e 0a60 6060                      ARE..```
```

### Comparing `nonebot_plugin_og-0.1.0/nonebot_plugin_og/__init__.py` & `nonebot_plugin_og-0.2.0/nonebot_plugin_og/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from typing import Union
 from nonebot import on_message
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent
-from nonebot_plugin_guild_patch import Bot, GuildMessageEvent
 from .utils import get_og_info
 
 __plugin_meta__ = PluginMetadata(
     name="og",
     description="检测链接并发送网站简介及预览图",
     usage="无",
     extra={
         "Author": "mute. <mute231010@gmail.com>",
-        "version": "v0.1.0"
+        "version": "v0.2.0"
     },
 )
 
 
 get_og = on_message(priority=99)
 
 @get_og.handle()
-async def get_og(bot: Bot, event: Union[MessageEvent, GuildMessageEvent]):
+async def get_og(bot: Bot, event: MessageEvent):
     og_info = await get_og_info(event.message)
     if og_info:
         title = og_info.get('title', '未知标题')
         desc = og_info.get('description', '未提供描述信息')
         img = og_info.get('image', None)
         if img:
             msg = f'{img}\n{title}\n{desc}'
```

### Comparing `nonebot_plugin_og-0.1.0/nonebot_plugin_og/utils.py` & `nonebot_plugin_og-0.2.0/nonebot_plugin_og/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_og-0.1.0/PKG-INFO` & `nonebot_plugin_og-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 6e65  : 2.1.Name: none
 00000020: 626f 742d 706c 7567 696e 2d6f 670a 5665  bot-plugin-og.Ve
-00000030: 7273 696f 6e3a 2030 2e31 2e30 0a53 756d  rsion: 0.1.0.Sum
+00000030: 7273 696f 6e3a 2030 2e32 2e30 0a53 756d  rsion: 0.2.0.Sum
 00000040: 6d61 7279 3a20 e6a3 80e6 b58b e993 bee6  mary: ..........
 00000050: 8ea5 e5b9 b6e5 8f91 e980 81e7 bd91 e7ab  ................
 00000060: 99e7 ae80 e4bb 8be5 8f8a e9a2 84e8 a788  ................
 00000070: e59b be0a 4c69 6365 6e73 653a 204d 4954  ....License: MIT
 00000080: 0a41 7574 686f 723a 206d 7574 652e 0a41  .Author: mute..A
 00000090: 7574 686f 722d 656d 6169 6c3a 206d 7574  uthor-email: mut
 000000a0: 6532 3331 3031 3040 676d 6169 6c2e 636f  e231010@gmail.co
@@ -22,123 +22,142 @@
 00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
 00000160: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
 00000170: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
 00000180: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 00000190: 3a3a 2033 2e31 310a 5265 7175 6972 6573  :: 3.11.Requires
 000001a0: 2d44 6973 743a 2068 7474 7078 2028 3e3d  -Dist: httpx (>=
 000001b0: 302e 3234 2e30 2c3c 302e 3235 2e30 290a  0.24.0,<0.25.0).
-000001c0: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
-000001d0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6775  onebot-plugin-gu
-000001e0: 696c 642d 7061 7463 6820 283e 3d30 2e32  ild-patch (>=0.2
-000001f0: 2e33 2c3c 302e 332e 3029 0a52 6571 7569  .3,<0.3.0).Requi
-00000200: 7265 732d 4469 7374 3a20 7079 7175 6572  res-Dist: pyquer
-00000210: 7920 283e 3d32 2e30 2e30 2c3c 332e 302e  y (>=2.0.0,<3.0.
-00000220: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
-00000230: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000240: 742f 6d61 726b 646f 776e 0a0a 0a3c 6469  t/markdown...<di
-00000250: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00000260: 3e0a 0a23 204e 6f6e 6562 6f74 2d70 6c75  >..# Nonebot-plu
-00000270: 6769 6e2d 6f67 0a0a 5fe2 9ca8 20e6 a380  gin-og.._... ...
-00000280: e6b5 8be9 93be e68e a5e5 b9b6 e794 9fe6  ................
-00000290: 8890 e9a2 84e8 a788 e59b be20 e29c a85f  ........... ..._
-000002a0: 2020 0a0a 3c2f 6469 763e 0a0a 2323 20f0    ..</div>..## .
-000002b0: 9f93 9620 e4bb 8be7 bb8d 0a0a e6a3 80e6  ... ............
-000002c0: b58b e993 bee6 8ea5 e5b9 b6e7 949f e688  ................
-000002d0: 90e9 a284 e8a7 88e5 9bbe efbc 8ce5 9fba  ................
-000002e0: e4ba 8e20 5b4f 7065 6e20 4772 6170 685d  ... [Open Graph]
-000002f0: 2868 7474 7073 3a2f 2f6f 6770 2e6d 652f  (https://ogp.me/
-00000300: 2920 e58d 8fe8 aeae 0a0a 2323 20f0 9f92  ) ........## ...
-00000310: bf20 e5ae 89e8 a385 0a0a 3c64 6574 6169  . ........<detai
-00000320: 6c73 3e0a 3c73 756d 6d61 7279 3ee4 bdbf  ls>.<summary>...
-00000330: e794 a820 6e62 2d63 6c69 20e5 ae89 e8a3  ... nb-cli .....
-00000340: 853c 2f73 756d 6d61 7279 3e0a e59c a820  .</summary>.... 
-00000350: 6e6f 6e65 626f 7432 20e9 a1b9 e79b aee7  nonebot2 .......
-00000360: 9a84 e6a0 b9e7 9bae e5bd 95e4 b88b e689  ................
-00000370: 93e5 bc80 e591 bde4 bba4 e8a1 8c2c 20e8  ............., .
-00000380: be93 e585 a5e4 bba5 e4b8 8be6 8c87 e4bb  ................
-00000390: a4e5 8db3 e58f afe5 ae89 e8a3 850a 0a20  ............... 
-000003a0: 2020 206e 6220 706c 7567 696e 2069 6e73     nb plugin ins
-000003b0: 7461 6c6c 206e 6f6e 6562 6f74 2d70 6c75  tall nonebot-plu
-000003c0: 6769 6e2d 6f67 0a0a 3c2f 6465 7461 696c  gin-og..</detail
-000003d0: 733e 0a0a 3c64 6574 6169 6c73 3e0a 3c73  s>..<details>.<s
-000003e0: 756d 6d61 7279 3ee4 bdbf e794 a870 6970  ummary>......pip
-000003f0: e5ae 89e8 a385 3c2f 7375 6d6d 6172 793e  ......</summary>
-00000400: 0ae5 9ca8 206e 6f6e 6562 6f74 3220 e9a1  .... nonebot2 ..
-00000410: b9e7 9bae e79a 84e6 8f92 e4bb b6e7 9bae  ................
-00000420: e5bd 95e4 b88b 2c20 e689 93e5 bc80 e591  ......, ........
-00000430: bde4 bba4 e8a1 8c2c 20e8 be93 e585 a5e4  ......., .......
-00000440: bba5 e4b8 8be6 8c87 e4bb a4e5 8db3 e58f  ................
-00000450: afe5 ae89 e8a3 850a 0a20 2020 2070 6970  .........    pip
-00000460: 2069 716e 7374 616c 6c20 6e6f 6e65 626f   iqnstall nonebo
-00000470: 742d 706c 7567 696e 2d6f 670a 0a3c 2f64  t-plugin-og..</d
-00000480: 6574 6169 6c73 3e0a 0a0a e689 93e5 bc80  etails>.........
-00000490: 206e 6f6e 6562 6f74 3220 e9a1 b9e7 9bae   nonebot2 ......
-000004a0: e6a0 b9e7 9bae e5bd 95e4 b88b e79a 8420  ............... 
-000004b0: 6070 7970 726f 6a65 6374 2e74 6f6d 6c60  `pyproject.toml`
-000004c0: 20e6 9687 e4bb b62c 20e5 9ca8 2060 5b74   ......, ... `[t
-000004d0: 6f6f 6c2e 6e6f 6e65 626f 745d 6020 e983  ool.nonebot]` ..
-000004e0: a8e5 8886 e8bf bde5 8aa0 e586 99e5 85a5  ................
-000004f0: 0a0a 2020 2020 706c 7567 696e 7320 3d20  ..    plugins = 
-00000500: 5b22 6e6f 6e65 626f 745f 706c 7567 696e  ["nonebot_plugin
-00000510: 5f6f 6722 5d0a 0a0a 2323 20f0 9f8e 8920  _og"]...## .... 
-00000520: e4bd bfe7 94a8 0a0a e79b b4e6 8ea5 e58f  ................
-00000530: 91e9 8081 e4bb bbe6 848f e993 bee6 8ea5  ................
-00000540: efbc 8ce5 8faa e8a6 81e6 98af e694 afe6  ................
-00000550: 8c81 204f 7065 6e20 4772 6170 6820 e58d  .. Open Graph ..
-00000560: 8fe8 aeae e79a 84e7 bd91 e7ab 99ef bc8c  ................
-00000570: e6ad a4e6 8f92 e4bb b6e9 83bd e4bc 9ae8  ................
-00000580: 87aa e58a a8e5 8f91 e980 81e9 a284 e8a7  ................
-00000590: 88e5 9bbe e380 820a 0a23 2320 e9b8 a3e8  .........## ....
-000005a0: b0a2 0a0a 2a20 5b60 6e6f 6e65 626f 742f  ....* [`nonebot/
-000005b0: 6e6f 656e 626f 7432 605d 2868 7474 7073  noenbot2`](https
-000005c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e6f  ://github.com/no
-000005d0: 6e65 626f 742f 6e6f 6e65 626f 7432 29ef  nebot/nonebot2).
-000005e0: bc9a e8b7 a8e5 b9b3 e58f b050 7974 686f  ...........Pytho
-000005f0: 6ee5 bc82 e6ad a5e6 9cba e599 a8e4 baba  n...............
-00000600: e6a1 86e6 9eb6 0a2a 205b 604d 7273 3473  .......* [`Mrs4s
-00000610: 2f67 6f2d 6371 6874 7470 605d 2868 7474  /go-cqhttp`](htt
-00000620: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000630: 4d72 7334 732f 676f 2d63 7168 7474 7029  Mrs4s/go-cqhttp)
-00000640: efbc 9a63 7168 7474 70e7 9a84 676f 6c61  ...cqhttp...gola
-00000650: 6e67 e5ae 9ee7 8eb0 efbc 8ce8 bdbb e987  ng..............
-00000660: 8fe3 8081 e58e 9fe7 949f e8b7 a8e5 b9b3  ................
-00000670: e58f b02e 0a2a 205b 606b 6f69 7368 696a  .....* [`koishij
-00000680: 732f 6b6f 6973 6869 2d70 6c75 6769 6e2d  s/koishi-plugin-
-00000690: 6f67 605d 2868 7474 7073 3a2f 2f67 6974  og`](https://git
-000006a0: 6875 622e 636f 6d2f 6b6f 6973 6869 6a73  hub.com/koishijs
-000006b0: 2f6b 6f69 7368 692d 706c 7567 696e 2d6f  /koishi-plugin-o
-000006c0: 6729 efbc 9ae6 9cac e9a1 b9e7 9bae e79b  g)..............
-000006d0: b4e6 8ea5 e58f 82e8 8083 207e 7eef bc88  .......... ~~...
-000006e0: e79b b4e6 8ea5 e5bc 80e6 8a84 7e7e 0a0a  ............~~..
-000006f0: 0a23 2320 e5bc 80e6 ba90 e8ae b8e5 8faf  .## ............
-00000700: e8af 810a 0ae4 bdbf e794 a820 5b4d 4954  ........... [MIT
-00000710: 5d28 2329 20e8 aeb8 e58f afe8 af81 e58f  ](#) ...........
-00000720: 91e5 b883 e380 820a 0a60 6060 0a54 4845  .........```.THE
-00000730: 2053 4f46 5457 4152 4520 4953 2050 524f   SOFTWARE IS PRO
-00000740: 5649 4445 4420 2241 5320 4953 222c 2057  VIDED "AS IS", W
-00000750: 4954 484f 5554 2057 4152 5241 4e54 5920  ITHOUT WARRANTY 
-00000760: 4f46 2041 4e59 204b 494e 442c 2045 5850  OF ANY KIND, EXP
-00000770: 5245 5353 204f 520a 494d 504c 4945 442c  RESS OR.IMPLIED,
-00000780: 2049 4e43 4c55 4449 4e47 2042 5554 204e   INCLUDING BUT N
-00000790: 4f54 204c 494d 4954 4544 2054 4f20 5448  OT LIMITED TO TH
-000007a0: 4520 5741 5252 414e 5449 4553 204f 4620  E WARRANTIES OF 
-000007b0: 4d45 5243 4841 4e54 4142 494c 4954 592c  MERCHANTABILITY,
-000007c0: 2046 4954 4e45 5353 0a46 4f52 2041 2050   FITNESS.FOR A P
-000007d0: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
-000007e0: 4520 414e 4420 4e4f 4e49 4e46 5249 4e47  E AND NONINFRING
-000007f0: 454d 454e 542e 2049 4e20 4e4f 2045 5645  EMENT. IN NO EVE
-00000800: 4e54 2053 4841 4c4c 2054 4845 2041 5554  NT SHALL THE AUT
-00000810: 484f 5253 204f 520a 434f 5059 5249 4748  HORS OR.COPYRIGH
-00000820: 5420 484f 4c44 4552 5320 4245 204c 4941  T HOLDERS BE LIA
-00000830: 424c 4520 464f 5220 414e 5920 434c 4149  BLE FOR ANY CLAI
-00000840: 4d2c 2044 414d 4147 4553 204f 5220 4f54  M, DAMAGES OR OT
-00000850: 4845 5220 4c49 4142 494c 4954 592c 2057  HER LIABILITY, W
-00000860: 4845 5448 4552 0a49 4e20 414e 2041 4354  HETHER.IN AN ACT
-00000870: 494f 4e20 4f46 2043 4f4e 5452 4143 542c  ION OF CONTRACT,
-00000880: 2054 4f52 5420 4f52 204f 5448 4552 5749   TORT OR OTHERWI
-00000890: 5345 2c20 4152 4953 494e 4720 4652 4f4d  SE, ARISING FROM
-000008a0: 2c20 4f55 5420 4f46 204f 5220 494e 0a43  , OUT OF OR IN.C
-000008b0: 4f4e 4e45 4354 494f 4e20 5749 5448 2054  ONNECTION WITH T
-000008c0: 4845 2053 4f46 5457 4152 4520 4f52 2054  HE SOFTWARE OR T
-000008d0: 4845 2055 5345 204f 5220 4f54 4845 5220  HE USE OR OTHER 
-000008e0: 4445 414c 494e 4753 2049 4e20 5448 4520  DEALINGS IN THE 
-000008f0: 534f 4654 5741 5245 2e0a 6060 600a       SOFTWARE..```.
+000001c0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+000001d0: 7971 7565 7279 2028 3e3d 322e 302e 302c  yquery (>=2.0.0,
+000001e0: 3c33 2e30 2e30 290a 4465 7363 7269 7074  <3.0.0).Descript
+000001f0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+00000200: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+00000210: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000220: 6e74 6572 223e 0a0a 2320 4e6f 6e65 626f  nter">..# Nonebo
+00000230: 742d 706c 7567 696e 2d6f 670a 0a5f e29c  t-plugin-og.._..
+00000240: a820 e6a3 80e6 b58b e993 bee6 8ea5 e5b9  . ..............
+00000250: b6e7 949f e688 90e9 a284 e8a7 88e5 9bbe  ................
+00000260: 20e2 9ca8 5f20 200a 0a3c 6120 6872 6566   ..._  ..<a href
+00000270: 3d22 2e2f 4c49 4345 4e53 4522 3e0a 2020  ="./LICENSE">.  
+00000280: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000290: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000002a0: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+000002b0: 652f 6d75 7465 3233 2d63 6f64 652f 6e6f  e/mute23-code/no
+000002c0: 6e65 626f 745f 706c 7567 696e 5f6f 6722  nebot_plugin_og"
+000002d0: 2061 6c74 3d22 6c69 6365 6e73 6522 3e0a   alt="license">.
+000002e0: 3c2f 613e 0a3c 6120 6872 6566 3d22 6874  </a>.<a href="ht
+000002f0: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
+00000300: 6e2e 6f72 672f 7079 7069 2f6e 6f6e 6562  n.org/pypi/noneb
+00000310: 6f74 5f70 6c75 6769 6e5f 6f67 223e 0a20  ot_plugin_og">. 
+00000320: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000330: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000340: 2e69 6f2f 7079 7069 2f76 2f6e 6f6e 6562  .io/pypi/v/noneb
+00000350: 6f74 5f70 6c75 6769 6e5f 6f67 2e73 7667  ot_plugin_og.svg
+00000360: 2220 616c 743d 2270 7970 6922 3e0a 3c2f  " alt="pypi">.</
+00000370: 613e 0a3c 696d 6720 7372 633d 2268 7474  a>.<img src="htt
+00000380: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000390: 2e69 6f2f 6261 6467 652f 7079 7468 6f6e  .io/badge/python
+000003a0: 2d33 2e38 2b2d 626c 7565 2e73 7667 2220  -3.8+-blue.svg" 
+000003b0: 616c 743d 2270 7974 686f 6e22 3e0a 0a0a  alt="python">...
+000003c0: 3c2f 6469 763e 0a0a 2020 2020 2323 20f0  </div>..    ## .
+000003d0: 9f93 9620 e4bb 8be7 bb8d 0a0a 2020 2020  ... ........    
+000003e0: e6a3 80e6 b58b e993 bee6 8ea5 e5b9 b6e7  ................
+000003f0: 949f e688 90e9 a284 e8a7 88e5 9bbe efbc  ................
+00000400: 8ce5 9fba e4ba 8e20 5b4f 7065 6e20 4772  ....... [Open Gr
+00000410: 6170 685d 2868 7474 7073 3a2f 2f6f 6770  aph](https://ogp
+00000420: 2e6d 652f 2920 e58d 8fe8 aeae 0a0a 2323  .me/) ........##
+00000430: 20f0 9f92 bf20 e5ae 89e8 a385 0a0a 3c64   .... ........<d
+00000440: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00000450: 3ee4 bdbf e794 a820 6e62 2d63 6c69 20e5  >...... nb-cli .
+00000460: ae89 e8a3 853c 2f73 756d 6d61 7279 3e0a  .....</summary>.
+00000470: e59c a820 6e6f 6e65 626f 7432 20e9 a1b9  ... nonebot2 ...
+00000480: e79b aee7 9a84 e6a0 b9e7 9bae e5bd 95e4  ................
+00000490: b88b e689 93e5 bc80 e591 bde4 bba4 e8a1  ................
+000004a0: 8c2c 20e8 be93 e585 a5e4 bba5 e4b8 8be6  ., .............
+000004b0: 8c87 e4bb a4e5 8db3 e58f afe5 ae89 e8a3  ................
+000004c0: 850a 0a20 2020 206e 6220 706c 7567 696e  ...    nb plugin
+000004d0: 2069 6e73 7461 6c6c 206e 6f6e 6562 6f74   install nonebot
+000004e0: 2d70 6c75 6769 6e2d 6f67 0a0a 3c2f 6465  -plugin-og..</de
+000004f0: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
+00000500: 3e0a 3c73 756d 6d61 7279 3ee4 bdbf e794  >.<summary>.....
+00000510: a870 6970 e5ae 89e8 a385 3c2f 7375 6d6d  .pip......</summ
+00000520: 6172 793e 0ae5 9ca8 206e 6f6e 6562 6f74  ary>.... nonebot
+00000530: 3220 e9a1 b9e7 9bae e79a 84e6 8f92 e4bb  2 ..............
+00000540: b6e7 9bae e5bd 95e4 b88b 2c20 e689 93e5  .........., ....
+00000550: bc80 e591 bde4 bba4 e8a1 8c2c 20e8 be93  ..........., ...
+00000560: e585 a5e4 bba5 e4b8 8be6 8c87 e4bb a4e5  ................
+00000570: 8db3 e58f afe5 ae89 e8a3 850a 0a20 2020  .............   
+00000580: 2070 6970 2069 716e 7374 616c 6c20 6e6f   pip iqnstall no
+00000590: 6e65 626f 742d 706c 7567 696e 2d6f 670a  nebot-plugin-og.
+000005a0: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a e689  .</details>.....
+000005b0: 93e5 bc80 206e 6f6e 6562 6f74 3220 e9a1  .... nonebot2 ..
+000005c0: b9e7 9bae e6a0 b9e7 9bae e5bd 95e4 b88b  ................
+000005d0: e79a 8420 6070 7970 726f 6a65 6374 2e74  ... `pyproject.t
+000005e0: 6f6d 6c60 20e6 9687 e4bb b62c 20e5 9ca8  oml` ......, ...
+000005f0: 2060 5b74 6f6f 6c2e 6e6f 6e65 626f 745d   `[tool.nonebot]
+00000600: 6020 e983 a8e5 8886 e8bf bde5 8aa0 e586  ` ..............
+00000610: 99e5 85a5 0a0a 2020 2020 706c 7567 696e  ......    plugin
+00000620: 7320 3d20 5b22 6e6f 6e65 626f 745f 706c  s = ["nonebot_pl
+00000630: 7567 696e 5f6f 6722 5d0a 0a0a 2323 20f0  ugin_og"]...## .
+00000640: 9f8e 8920 e4bd bfe7 94a8 0a0a e79b b4e6  ... ............
+00000650: 8ea5 e58f 91e9 8081 e4bb bbe6 848f e993  ................
+00000660: bee6 8ea5 efbc 8ce5 8faa e8a6 81e6 98af  ................
+00000670: e694 afe6 8c81 204f 7065 6e20 4772 6170  ...... Open Grap
+00000680: 6820 e58d 8fe8 aeae e79a 84e7 bd91 e7ab  h ..............
+00000690: 99ef bc8c e6ad a4e6 8f92 e4bb b6e9 83bd  ................
+000006a0: e4bc 9ae8 87aa e58a a8e5 8f91 e980 81e9  ................
+000006b0: a284 e8a7 88e5 9bbe e380 820a 0a23 2320  .............## 
+000006c0: e9b8 a3e8 b0a2 0a0a 2a20 5b60 6e6f 6e65  ........* [`none
+000006d0: 626f 742f 6e6f 656e 626f 7432 605d 2868  bot/noenbot2`](h
+000006e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006f0: 6d2f 6e6f 6e65 626f 742f 6e6f 6e65 626f  m/nonebot/nonebo
+00000700: 7432 29ef bc9a e8b7 a8e5 b9b3 e58f b050  t2)............P
+00000710: 7974 686f 6ee5 bc82 e6ad a5e6 9cba e599  ython...........
+00000720: a8e4 baba e6a1 86e6 9eb6 0a2a 205b 604d  ...........* [`M
+00000730: 7273 3473 2f67 6f2d 6371 6874 7470 605d  rs4s/go-cqhttp`]
+00000740: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000750: 636f 6d2f 4d72 7334 732f 676f 2d63 7168  com/Mrs4s/go-cqh
+00000760: 7474 7029 efbc 9a63 7168 7474 70e7 9a84  ttp)...cqhttp...
+00000770: 676f 6c61 6e67 e5ae 9ee7 8eb0 efbc 8ce8  golang..........
+00000780: bdbb e987 8fe3 8081 e58e 9fe7 949f e8b7  ................
+00000790: a8e5 b9b3 e58f b02e 0a2a 205b 606b 6f69  .........* [`koi
+000007a0: 7368 696a 732f 6b6f 6973 6869 2d70 6c75  shijs/koishi-plu
+000007b0: 6769 6e2d 6f67 605d 2868 7474 7073 3a2f  gin-og`](https:/
+000007c0: 2f67 6974 6875 622e 636f 6d2f 6b6f 6973  /github.com/kois
+000007d0: 6869 6a73 2f6b 6f69 7368 692d 706c 7567  hijs/koishi-plug
+000007e0: 696e 2d6f 6729 efbc 9ae6 9cac e9a1 b9e7  in-og)..........
+000007f0: 9bae e79b b4e6 8ea5 e58f 82e8 8083 207e  .............. ~
+00000800: 7eef bc88 e79b b4e6 8ea5 e5bc 80e6 8a84  ~...............
+00000810: 7e7e 0a0a 0a23 2320 e5bc 80e6 ba90 e8ae  ~~...## ........
+00000820: b8e5 8faf e8af 810a 0ae4 bdbf e794 a820  ............... 
+00000830: 5b4d 4954 5d28 2e2f 4c49 4345 4e53 4529  [MIT](./LICENSE)
+00000840: 20e8 aeb8 e58f afe8 af81 e58f 91e5 b883   ...............
+00000850: e380 820a 0a60 6060 0a54 4845 2053 4f46  .....```.THE SOF
+00000860: 5457 4152 4520 4953 2050 524f 5649 4445  TWARE IS PROVIDE
+00000870: 4420 2241 5320 4953 222c 2057 4954 484f  D "AS IS", WITHO
+00000880: 5554 2057 4152 5241 4e54 5920 4f46 2041  UT WARRANTY OF A
+00000890: 4e59 204b 494e 442c 2045 5850 5245 5353  NY KIND, EXPRESS
+000008a0: 204f 520a 494d 504c 4945 442c 2049 4e43   OR.IMPLIED, INC
+000008b0: 4c55 4449 4e47 2042 5554 204e 4f54 204c  LUDING BUT NOT L
+000008c0: 494d 4954 4544 2054 4f20 5448 4520 5741  IMITED TO THE WA
+000008d0: 5252 414e 5449 4553 204f 4620 4d45 5243  RRANTIES OF MERC
+000008e0: 4841 4e54 4142 494c 4954 592c 2046 4954  HANTABILITY, FIT
+000008f0: 4e45 5353 0a46 4f52 2041 2050 4152 5449  NESS.FOR A PARTI
+00000900: 4355 4c41 5220 5055 5250 4f53 4520 414e  CULAR PURPOSE AN
+00000910: 4420 4e4f 4e49 4e46 5249 4e47 454d 454e  D NONINFRINGEMEN
+00000920: 542e 2049 4e20 4e4f 2045 5645 4e54 2053  T. IN NO EVENT S
+00000930: 4841 4c4c 2054 4845 2041 5554 484f 5253  HALL THE AUTHORS
+00000940: 204f 520a 434f 5059 5249 4748 5420 484f   OR.COPYRIGHT HO
+00000950: 4c44 4552 5320 4245 204c 4941 424c 4520  LDERS BE LIABLE 
+00000960: 464f 5220 414e 5920 434c 4149 4d2c 2044  FOR ANY CLAIM, D
+00000970: 414d 4147 4553 204f 5220 4f54 4845 5220  AMAGES OR OTHER 
+00000980: 4c49 4142 494c 4954 592c 2057 4845 5448  LIABILITY, WHETH
+00000990: 4552 0a49 4e20 414e 2041 4354 494f 4e20  ER.IN AN ACTION 
+000009a0: 4f46 2043 4f4e 5452 4143 542c 2054 4f52  OF CONTRACT, TOR
+000009b0: 5420 4f52 204f 5448 4552 5749 5345 2c20  T OR OTHERWISE, 
+000009c0: 4152 4953 494e 4720 4652 4f4d 2c20 4f55  ARISING FROM, OU
+000009d0: 5420 4f46 204f 5220 494e 0a43 4f4e 4e45  T OF OR IN.CONNE
+000009e0: 4354 494f 4e20 5749 5448 2054 4845 2053  CTION WITH THE S
+000009f0: 4f46 5457 4152 4520 4f52 2054 4845 2055  OFTWARE OR THE U
+00000a00: 5345 204f 5220 4f54 4845 5220 4445 414c  SE OR OTHER DEAL
+00000a10: 494e 4753 2049 4e20 5448 4520 534f 4654  INGS IN THE SOFT
+00000a20: 5741 5245 2e0a 6060 600a                 WARE..```.
```

