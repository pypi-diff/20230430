# Comparing `tmp/posuto-2023.4.0.tar.gz` & `tmp/posuto-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posuto-2023.4.0.tar", last modified: Mon Apr  3 07:04:09 2023, max compression
+gzip compressed data, was "posuto-2023.5.0.tar", last modified: Sun Apr 30 12:09:50 2023, max compression
```

## Comparing `posuto-2023.4.0.tar` & `posuto-2023.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-03 07:04:09.939770 posuto-2023.4.0/
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-03 07:04:09.876436 posuto-2023.4.0/.github/
--rw-r--r--   0 23        (1000) u23       (1000)       13 2020-12-07 10:56:39.000000 posuto-2023.4.0/.github/FUNDING.yml
--rw-r--r--   0 23        (1000) u23       (1000)     1872 2020-12-07 10:56:39.000000 posuto-2023.4.0/.gitignore
--rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-12-07 10:56:39.000000 posuto-2023.4.0/LICENSE
--rw-r--r--   0 23        (1000) u23       (1000)      142 2020-12-07 10:56:39.000000 posuto-2023.4.0/MANIFEST.in
--rw-r--r--   0 23        (1000) u23       (1000)      692 2021-02-26 11:37:41.000000 posuto-2023.4.0/Makefile
--rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-04-03 07:04:09.939770 posuto-2023.4.0/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)     5639 2023-01-31 11:52:04.000000 posuto-2023.4.0/README.md
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-03 07:04:09.876436 posuto-2023.4.0/examples/
--rw-r--r--   0 23        (1000) u23       (1000)      272 2020-12-07 10:56:39.000000 posuto-2023.4.0/examples/sample.py
--rw-r--r--   0 23        (1000) u23       (1000)   295014 2020-12-07 10:56:39.000000 posuto-2023.4.0/postcharacter.png
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-03 07:04:09.939770 posuto-2023.4.0/posuto/
--rw-r--r--   0 23        (1000) u23       (1000)       40 2022-12-01 14:35:27.000000 posuto-2023.4.0/posuto/__init__.py
--rw-r--r--   0 23        (1000) u23       (1000) 13101710 2023-04-03 06:53:22.000000 posuto-2023.4.0/posuto/officedata.json
--rw-r--r--   0 23        (1000) u23       (1000) 81149952 2023-04-03 06:53:23.000000 posuto-2023.4.0/posuto/postaldata.db
--rw-r--r--   0 23        (1000) u23       (1000)     2770 2022-12-01 14:35:27.000000 posuto-2023.4.0/posuto/posuto.py
--rw-r--r--   0 23        (1000) u23       (1000)    11156 2023-03-15 04:34:33.000000 posuto-2023.4.0/posuto/prep.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-03 07:04:09.939770 posuto-2023.4.0/posuto/tests/
--rw-r--r--   0 23        (1000) u23       (1000)     1756 2023-03-15 04:34:33.000000 posuto-2023.4.0/posuto/tests/test_basic.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-03 07:04:09.939770 posuto-2023.4.0/posuto.egg-info/
--rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-04-03 07:04:09.000000 posuto-2023.4.0/posuto.egg-info/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)      367 2023-04-03 07:04:09.000000 posuto-2023.4.0/posuto.egg-info/SOURCES.txt
--rw-r--r--   0 23        (1000) u23       (1000)        1 2023-04-03 07:04:09.000000 posuto-2023.4.0/posuto.egg-info/dependency_links.txt
--rw-r--r--   0 23        (1000) u23       (1000)        7 2023-04-03 07:04:09.000000 posuto-2023.4.0/posuto.egg-info/top_level.txt
--rw-r--r--   0 23        (1000) u23       (1000)      706 2023-04-03 07:04:09.939770 posuto-2023.4.0/setup.cfg
--rw-r--r--   0 23        (1000) u23       (1000)      471 2020-12-07 10:56:40.000000 posuto-2023.4.0/setup.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.280827 posuto-2023.5.0/
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.217493 posuto-2023.5.0/.github/
+-rw-r--r--   0 23        (1000) u23       (1000)       13 2020-12-07 10:56:39.000000 posuto-2023.5.0/.github/FUNDING.yml
+-rw-r--r--   0 23        (1000) u23       (1000)     1872 2020-12-07 10:56:39.000000 posuto-2023.5.0/.gitignore
+-rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-12-07 10:56:39.000000 posuto-2023.5.0/LICENSE
+-rw-r--r--   0 23        (1000) u23       (1000)      142 2020-12-07 10:56:39.000000 posuto-2023.5.0/MANIFEST.in
+-rw-r--r--   0 23        (1000) u23       (1000)      692 2021-02-26 11:37:41.000000 posuto-2023.5.0/Makefile
+-rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-04-30 12:09:50.280827 posuto-2023.5.0/PKG-INFO
+-rw-r--r--   0 23        (1000) u23       (1000)     5639 2023-01-31 11:52:04.000000 posuto-2023.5.0/README.md
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.217493 posuto-2023.5.0/examples/
+-rw-r--r--   0 23        (1000) u23       (1000)      272 2020-12-07 10:56:39.000000 posuto-2023.5.0/examples/sample.py
+-rw-r--r--   0 23        (1000) u23       (1000)   295014 2020-12-07 10:56:39.000000 posuto-2023.5.0/postcharacter.png
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.280827 posuto-2023.5.0/posuto/
+-rw-r--r--   0 23        (1000) u23       (1000)       40 2022-12-01 14:35:27.000000 posuto-2023.5.0/posuto/__init__.py
+-rw-r--r--   0 23        (1000) u23       (1000) 13104799 2023-04-30 11:44:00.000000 posuto-2023.5.0/posuto/officedata.json
+-rw-r--r--   0 23        (1000) u23       (1000) 81154048 2023-04-30 11:44:01.000000 posuto-2023.5.0/posuto/postaldata.db
+-rw-r--r--   0 23        (1000) u23       (1000)     2770 2022-12-01 14:35:27.000000 posuto-2023.5.0/posuto/posuto.py
+-rw-r--r--   0 23        (1000) u23       (1000)    11156 2023-03-15 04:34:33.000000 posuto-2023.5.0/posuto/prep.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.280827 posuto-2023.5.0/posuto/tests/
+-rw-r--r--   0 23        (1000) u23       (1000)     1756 2023-03-15 04:34:33.000000 posuto-2023.5.0/posuto/tests/test_basic.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-04-30 12:09:50.280827 posuto-2023.5.0/posuto.egg-info/
+-rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-04-30 12:09:49.000000 posuto-2023.5.0/posuto.egg-info/PKG-INFO
+-rw-r--r--   0 23        (1000) u23       (1000)      367 2023-04-30 12:09:49.000000 posuto-2023.5.0/posuto.egg-info/SOURCES.txt
+-rw-r--r--   0 23        (1000) u23       (1000)        1 2023-04-30 12:09:49.000000 posuto-2023.5.0/posuto.egg-info/dependency_links.txt
+-rw-r--r--   0 23        (1000) u23       (1000)        7 2023-04-30 12:09:49.000000 posuto-2023.5.0/posuto.egg-info/top_level.txt
+-rw-r--r--   0 23        (1000) u23       (1000)      706 2023-04-30 12:09:50.280827 posuto-2023.5.0/setup.cfg
+-rw-r--r--   0 23        (1000) u23       (1000)      471 2020-12-07 10:56:40.000000 posuto-2023.5.0/setup.py
```

### Comparing `posuto-2023.4.0/.gitignore` & `posuto-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `posuto-2023.4.0/LICENSE` & `posuto-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posuto-2023.4.0/Makefile` & `posuto-2023.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `posuto-2023.4.0/PKG-INFO` & `posuto-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `posuto-2023.4.0/README.md` & `posuto-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `posuto-2023.4.0/postcharacter.png` & `posuto-2023.5.0/postcharacter.png`

 * *Files identical despite different names*

### Comparing `posuto-2023.4.0/posuto/officedata.json` & `posuto-2023.5.0/posuto/officedata.json`

 * *Files 0% similar despite different names*

```diff
@@ -10843,15 +10843,15 @@
     "neighborhood": "永山三条",
     "banchi": "23丁目1番9番",
     "postal_code": "0798501",
     "old_code": "079  ",
     "post_office": "永山",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0798509": {
     "jis": "01204",
@@ -11033,15 +11033,15 @@
     "neighborhood": "永山七条",
     "banchi": "16丁目3番16号",
     "postal_code": "0798505",
     "old_code": "079  ",
     "post_office": "永山",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0798516": {
     "jis": "01204",
@@ -27763,83 +27763,64 @@
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0390195": {
     "jis": "02445",
-    "kana": "ナンブチヨウヤクバ ナンブブンチヨウシヤ",
-    "name": "南部町役場　南部分庁舎",
+    "kana": "ナンブシシヨ",
+    "name": "南部支所",
     "prefecture": "青森県",
     "city": "三戸郡南部町",
     "neighborhood": "大字沖田面",
     "banchi": "字沖中46",
     "postal_code": "0390195",
     "old_code": "03901",
     "post_office": "三戸",
     "type": "office",
     "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
-  "0390595": {
-    "jis": "02445",
-    "kana": "ナンブチヨウヤクバ ナガワブンチヨウシヤ",
-    "name": "南部町役場　名川分庁舎",
-    "prefecture": "青森県",
-    "city": "三戸郡南部町",
-    "neighborhood": "大字平",
-    "banchi": "字広場22",
-    "postal_code": "0390595",
-    "old_code": "03905",
-    "post_office": "上名久井",
-    "type": "office",
-    "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0390592": {
     "jis": "02445",
-    "kana": "ナンブチヨウヤクバ ホンチヨウシヤ",
-    "name": "南部町役場　本庁舎",
+    "kana": "ナンブチヨウヤクバ",
+    "name": "南部町役場",
     "prefecture": "青森県",
     "city": "三戸郡南部町",
     "neighborhood": "大字平",
     "banchi": "字広場28番地1",
     "postal_code": "0390592",
     "old_code": "03905",
     "post_office": "上名久井",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0390892": {
     "jis": "02445",
-    "kana": "ナンブチヨウヤクバ",
-    "name": "南部町役場",
+    "kana": "フクチシシヨ",
+    "name": "福地支所",
     "prefecture": "青森県",
     "city": "三戸郡南部町",
     "neighborhood": "大字苫米地",
     "banchi": "字下宿23-1",
     "postal_code": "0390892",
     "old_code": "03908",
     "post_office": "福地",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "0208584": {
     "jis": "03201",
@@ -37859,21 +37840,21 @@
   "9894592": {
     "jis": "04213",
     "kana": "クリハラシ セミネソウゴウシシヨ",
     "name": "栗原市　瀬峰総合支所",
     "prefecture": "宮城県",
     "city": "栗原市",
     "neighborhood": "瀬峰",
-    "banchi": "下藤沢118-1",
+    "banchi": "長者原37番地2",
     "postal_code": "9894592",
     "old_code": "98945",
     "post_office": "高清水",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9895392": {
     "jis": "04213",
@@ -47694,14 +47675,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "コオリヤマシ",
     "neighborhood_kana": "ハヤマ",
     "alternates": []
   },
+  "9638637": {
+    "jis": "07203",
+    "kana": "ニデツクプレシジヨン カブシキガイシヤ コオリヤマジギヨウシヨ",
+    "name": "ニデックプレシジョン　株式会社　郡山事業所",
+    "prefecture": "福島県",
+    "city": "郡山市",
+    "neighborhood": "富田町",
+    "banchi": "字諏訪内37(郡山郵便局私書箱第37号)",
+    "postal_code": "9638637",
+    "old_code": "963  ",
+    "post_office": "郡山",
+    "type": "box",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "フクシマケン",
+    "city_kana": "コオリヤマシ",
+    "neighborhood_kana": "トミタマチ",
+    "alternates": []
+  },
   "9638580": {
     "jis": "07203",
     "kana": "ニホンセイメイホケン ソウゴガイシヤ コオリヤマシシヤ",
     "name": "日本生命保険　相互会社　郡山支社",
     "prefecture": "福島県",
     "city": "郡山市",
     "neighborhood": "駅前",
@@ -48398,33 +48398,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "コオリヤマシ",
     "neighborhood_kana": "シミズダイ",
     "alternates": []
   },
-  "9638637": {
-    "jis": "07203",
-    "kana": "ニホンデンサンコパル カブシキガイシヤ コオリヤマギジユツカイハツセンタ-",
-    "name": "日本電産コパル　株式会社　郡山技術開発センター",
-    "prefecture": "福島県",
-    "city": "郡山市",
-    "neighborhood": "富田町",
-    "banchi": "字諏訪内37(郡山郵便局私書箱第37号)",
-    "postal_code": "9638637",
-    "old_code": "96391",
-    "post_office": "郡山",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "フクシマケン",
-    "city_kana": "コオリヤマシ",
-    "neighborhood_kana": "トミタマチ",
-    "alternates": []
-  },
   "9638794": {
     "jis": "07203",
     "kana": "コオリヤマテン ホウジンサ-ビスブ",
     "name": "郡山店　法人サービス部",
     "prefecture": "福島県",
     "city": "郡山市",
     "neighborhood": "清水台",
@@ -48590,26 +48571,26 @@
     "prefecture_kana": "フクシマケン",
     "city_kana": "イワキシ",
     "neighborhood_kana": "タイラ",
     "alternates": []
   },
   "9701192": {
     "jis": "07204",
-    "kana": "アルパイン カブシキガイシヤ イワキジギヨウシヨ",
-    "name": "アルパイン　株式会社　いわき事業所",
+    "kana": "アルプスアルパイン カブシキガイシヤ イワキカイハツセンタ-",
+    "name": "アルプスアルパイン　株式会社　いわき開発センター",
     "prefecture": "福島県",
     "city": "いわき市",
     "neighborhood": "好間工業団地",
     "banchi": "20-1",
     "postal_code": "9701192",
     "old_code": "97011",
     "post_office": "いわき",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "フクシマケン",
     "city_kana": "イワキシ",
     "neighborhood_kana": "ヨシマコウギョウダンチ",
     "alternates": []
   },
   "9701193": {
     "jis": "07204",
@@ -53106,15 +53087,15 @@
     "neighborhood": "安良川",
     "banchi": "字下ノ内363",
     "postal_code": "3188505",
     "old_code": "318  ",
     "post_office": "高萩",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "イバラキケン",
     "city_kana": "タカハギシ",
     "neighborhood_kana": "アラカワ",
     "alternates": []
   },
   "3191592": {
     "jis": "08215",
@@ -59920,25 +59901,25 @@
   },
   "3248551": {
     "jis": "09210",
     "kana": "オオタワラケンゼイジムシヨ",
     "name": "大田原県税事務所",
     "prefecture": "栃木県",
     "city": "大田原市",
-    "neighborhood": "中央",
-    "banchi": "1丁目9-9",
+    "neighborhood": "本町",
+    "banchi": "2丁目2828-4",
     "postal_code": "3248551",
     "old_code": "324  ",
     "post_office": "大田原",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トチギケン",
     "city_kana": "オオタワラシ",
-    "neighborhood_kana": "チュウオウ",
+    "neighborhood_kana": "ホンチョウ",
     "alternates": []
   },
   "3248641": {
     "jis": "09210",
     "kana": "オオタワラシヤクシヨ",
     "name": "大田原市役所",
     "prefecture": "栃木県",
@@ -59952,14 +59933,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トチギケン",
     "city_kana": "オオタワラシ",
     "neighborhood_kana": "ホンチョウ",
     "alternates": []
   },
+  "3248765": {
+    "jis": "09210",
+    "kana": "オオタワラドボクジムシヨ",
+    "name": "大田原土木事務所",
+    "prefecture": "栃木県",
+    "city": "大田原市",
+    "neighborhood": "本町",
+    "banchi": "2-2828-4",
+    "postal_code": "3248765",
+    "old_code": "324  ",
+    "post_office": "大田原",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トチギケン",
+    "city_kana": "オオタワラシ",
+    "neighborhood_kana": "ホンチョウ",
+    "alternates": []
+  },
   "3248625": {
     "jis": "09210",
     "kana": "カブシキガイシヤ トチギニコン",
     "name": "株式会社　栃木ニコン",
     "prefecture": "栃木県",
     "city": "大田原市",
     "neighborhood": "実取",
@@ -60067,50 +60067,50 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トチギケン",
     "city_kana": "オオタワラシ",
     "neighborhood_kana": "シモイシガミ",
     "alternates": []
   },
-  "3248686": {
+  "3248585": {
     "jis": "09210",
-    "kana": "ナスセキジユウジビヨウイン",
-    "name": "那須赤十字病院",
+    "kana": "トチギケンケンポクケンコウフクシセンタ-",
+    "name": "栃木県県北健康福祉センター",
     "prefecture": "栃木県",
     "city": "大田原市",
-    "neighborhood": "中田原",
-    "banchi": "1081番地4(大田原郵便局私書箱第15号)",
-    "postal_code": "3248686",
+    "neighborhood": "本町",
+    "banchi": "2丁目2828-4",
+    "postal_code": "3248585",
     "old_code": "324  ",
     "post_office": "大田原",
-    "type": "box",
+    "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トチギケン",
     "city_kana": "オオタワラシ",
-    "neighborhood_kana": "ナカダワラ",
+    "neighborhood_kana": "ホンチョウ",
     "alternates": []
   },
-  "3248585": {
+  "3248686": {
     "jis": "09210",
-    "kana": "ナスフクシジムシヨ",
-    "name": "那須福祉事務所",
+    "kana": "ナスセキジユウジビヨウイン",
+    "name": "那須赤十字病院",
     "prefecture": "栃木県",
     "city": "大田原市",
-    "neighborhood": "中央",
-    "banchi": "1丁目9-9",
-    "postal_code": "3248585",
+    "neighborhood": "中田原",
+    "banchi": "1081番地4(大田原郵便局私書箱第15号)",
+    "postal_code": "3248686",
     "old_code": "324  ",
     "post_office": "大田原",
-    "type": "office",
+    "type": "box",
     "multiple": false,
     "new": false,
     "prefecture_kana": "トチギケン",
     "city_kana": "オオタワラシ",
-    "neighborhood_kana": "チュウオウ",
+    "neighborhood_kana": "ナカダワラ",
     "alternates": []
   },
   "3248540": {
     "jis": "09210",
     "kana": "ニツポンネンキンキコウ オオタワラネンキンジムシヨ",
     "name": "日本年金機構　大田原年金事務所",
     "prefecture": "栃木県",
@@ -65273,14 +65273,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "グンマケン",
     "city_kana": "フジオカシ",
     "neighborhood_kana": "フジオカ",
     "alternates": []
   },
+  "3758507": {
+    "jis": "10209",
+    "kana": "ミサトコウギヨウ カブシキカイシヤ",
+    "name": "美里工業　株式会社",
+    "prefecture": "群馬県",
+    "city": "藤岡市",
+    "neighborhood": "藤岡",
+    "banchi": "1360",
+    "postal_code": "3758507",
+    "old_code": "375  ",
+    "post_office": "藤岡",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "グンマケン",
+    "city_kana": "フジオカシ",
+    "neighborhood_kana": "フジオカ",
+    "alternates": []
+  },
   "3758501": {
     "jis": "10209",
     "kana": "ミツビシエンピツ カブシキガイシヤ グンマコウジヨウ",
     "name": "三菱鉛筆　株式会社　群馬工場",
     "prefecture": "群馬県",
     "city": "藤岡市",
     "neighborhood": "立石",
@@ -78748,29 +78767,29 @@
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "3628577": {
     "jis": "11301",
-    "kana": "ダイニツポンインキカガクコウギヨウ カブシキガイシヤ サイタマコウジヨウ",
-    "name": "大日本インキ化学工業　株式会社　埼玉工場",
+    "kana": "デイ-アイシ- カブシキガイシヤ サイタマコウジヨウ",
+    "name": "ＤＩＣ　株式会社　埼玉工場",
     "prefecture": "埼玉県",
     "city": "北足立郡伊奈町",
-    "neighborhood": "大字小室",
+    "neighborhood": "小室",
     "banchi": "4472-1",
     "postal_code": "3628577",
     "old_code": "362  ",
     "post_office": "上尾",
     "type": "office",
     "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
+    "new": true,
+    "prefecture_kana": "サイタマケン",
+    "city_kana": "キタアダチグンイナマチ",
+    "neighborhood_kana": "コムロ",
     "alternates": []
   },
   "3548565": {
     "jis": "11324",
     "kana": "アスクル ロジ パ-ク シユトケン",
     "name": "ＡＳＫＵＬ　Ｌｏｇｉ　ＰＡＲＫ　首都圏",
     "prefecture": "埼玉県",
@@ -80508,15 +80527,15 @@
     "neighborhood": "青葉町",
     "banchi": "977-1青葉の森公園芸術文化ホール内",
     "postal_code": "2608661",
     "old_code": "260  ",
     "post_office": "千葉中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "チバシチュウオウク",
     "neighborhood_kana": "アオバチョウ",
     "alternates": []
   },
   "2608566": {
     "jis": "12101",
@@ -88508,15 +88527,15 @@
     "neighborhood": "五井南海岸",
     "banchi": "14",
     "postal_code": "2908567",
     "old_code": "290  ",
     "post_office": "市原",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "イチハラシ",
     "neighborhood_kana": "ゴイミナミカイガン",
     "alternates": []
   },
   "2908560": {
     "jis": "12219",
@@ -96533,15 +96552,15 @@
     "neighborhood": "丸の内",
     "banchi": "2-7-3",
     "postal_code": "1008335",
     "old_code": "100  ",
     "post_office": "銀座",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "マルノウチ",
     "alternates": []
   },
   "1008303": {
     "jis": "13101",
@@ -103639,15 +103658,15 @@
     "neighborhood": "九段南",
     "banchi": "一丁目6番5号",
     "postal_code": "1028513",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "クダンミナミ",
     "alternates": []
   },
   "1028181": {
     "jis": "13101",
@@ -104057,15 +104076,15 @@
     "neighborhood": "九段南",
     "banchi": "一丁目6番5号",
     "postal_code": "1028582",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "クダンミナミ",
     "alternates": []
   },
   "1028343": {
     "jis": "13101",
@@ -104076,15 +104095,15 @@
     "neighborhood": "九段南",
     "banchi": "一丁目6番5号",
     "postal_code": "1028343",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "クダンミナミ",
     "alternates": []
   },
   "1028583": {
     "jis": "13101",
@@ -104095,15 +104114,15 @@
     "neighborhood": "九段南",
     "banchi": "一丁目6番5号",
     "postal_code": "1028583",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "クダンミナミ",
     "alternates": []
   },
   "1028621": {
     "jis": "13101",
@@ -105342,25 +105361,25 @@
   },
   "1028532": {
     "jis": "13101",
     "kana": "ゼンコクドボクケンチク コクミンケンコウホケンクミアイ カントウジムシヨ",
     "name": "全国土木建築　国民健康保険組合　関東事務所",
     "prefecture": "東京都",
     "city": "千代田区",
-    "neighborhood": "麹町",
-    "banchi": "3丁目2麹町共同ビル",
+    "neighborhood": "平河町",
+    "banchi": "一丁目五番九号厚生会館",
     "postal_code": "1028532",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
-    "neighborhood_kana": "コウジマチ",
+    "neighborhood_kana": "ヒラカワチョウ",
     "alternates": []
   },
   "1028564": {
     "jis": "13101",
     "kana": "ゼンコクドボクケンチクコクミンケンコウホケンクミアイ",
     "name": "全国土木建築国民健康保険組合",
     "prefecture": "東京都",
@@ -109398,15 +109417,15 @@
     "neighborhood": "日本橋馬喰町",
     "banchi": "1-12-3",
     "postal_code": "1038366",
     "old_code": "103  ",
     "post_office": "日本橋",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ニホンバシバクロチョウ",
     "alternates": []
   },
   "1038501": {
     "jis": "13102",
@@ -109759,15 +109778,15 @@
     "neighborhood": "日本橋室町",
     "banchi": "二丁目1番1号",
     "postal_code": "1038338",
     "old_code": "103  ",
     "post_office": "日本橋",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ニホンバシムロマチ",
     "alternates": []
   },
   "1038566": {
     "jis": "13102",
@@ -114338,15 +114357,15 @@
     "neighborhood": "銀座",
     "banchi": "6-18-2野村不動産銀座ビル",
     "postal_code": "1048112",
     "old_code": "104  ",
     "post_office": "銀座",
     "type": "office",
     "multiple": true,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ギンザ",
     "alternates": []
   },
   "1048530": {
     "jis": "13102",
@@ -114509,15 +114528,15 @@
     "neighborhood": "明石町",
     "banchi": "8-1聖路加タワー1階・16階",
     "postal_code": "1048175",
     "old_code": "104  ",
     "post_office": "晴海",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "アカシチョウ",
     "alternates": []
   },
   "1048365": {
     "jis": "13102",
@@ -114870,15 +114889,15 @@
     "neighborhood": "八重洲",
     "banchi": "2丁目1番1号YANMARTOKYO10階",
     "postal_code": "1048481",
     "old_code": "104  ",
     "post_office": "晴海",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ヤエス",
     "alternates": []
   },
   "1048546": {
     "jis": "13102",
@@ -116016,33 +116035,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "ヒガシシンバシ",
     "alternates": []
   },
-  "1058688": {
-    "jis": "13103",
-    "kana": "カブシキガイシヤ シヨウセンミツイ",
-    "name": "株式会社　商船三井",
-    "prefecture": "東京都",
-    "city": "港区",
-    "neighborhood": "虎ノ門",
-    "banchi": "2丁目1-1(芝郵便局私書箱第5号)",
-    "postal_code": "1058688",
-    "old_code": "105  ",
-    "post_office": "芝",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "ミナトク",
-    "neighborhood_kana": "トラノモン",
-    "alternates": []
-  },
   "1058335": {
     "jis": "13103",
     "kana": "カブシキガイシヤ ジエイテイ-ビ-コミユニケ-シヨンデザイン",
     "name": "株式会社　ＪＴＢコミュニケーションデザイン",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "芝",
@@ -118355,14 +118355,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "ニシシンバシ",
     "alternates": []
   },
+  "1058467": {
+    "jis": "13103",
+    "kana": "ニホンコクドカイハツ (カ)",
+    "name": "日本国土開発　株式会社",
+    "prefecture": "東京都",
+    "city": "港区",
+    "neighborhood": "虎ノ門",
+    "banchi": "4丁目3-13ヒューリック神谷町ビル5F",
+    "postal_code": "1058467",
+    "old_code": "105  ",
+    "post_office": "芝",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "ミナトク",
+    "neighborhood_kana": "トラノモン",
+    "alternates": []
+  },
   "1058521": {
     "jis": "13103",
     "kana": "ニホンセキジユウジシヤ",
     "name": "日本赤十字社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "芝大門",
@@ -127974,28 +127993,47 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "シナノマチ",
     "alternates": []
   },
+  "1608313": {
+    "jis": "13104",
+    "kana": "ソンガイホケンジヤパン カブシキガイシヤ",
+    "name": "損害保険ジャパン　株式会社",
+    "prefecture": "東京都",
+    "city": "新宿区",
+    "neighborhood": "西新宿",
+    "banchi": "1-26-1",
+    "postal_code": "1608313",
+    "old_code": "160  ",
+    "post_office": "新宿",
+    "type": "office",
+    "multiple": true,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "シンジュクク",
+    "neighborhood_kana": "ニシシンジュク",
+    "alternates": []
+  },
   "1608338": {
     "jis": "13104",
-    "kana": "ソンガイホケンジヤパンニツポンコウア カブシキガイシヤ",
-    "name": "損害保険ジャパン日本興亜　株式会社",
+    "kana": "ソンガイホケンジヤパン カブシキガイシヤ",
+    "name": "損害保険ジャパン　株式会社",
     "prefecture": "東京都",
     "city": "新宿区",
     "neighborhood": "西新宿",
     "banchi": "1-26-1",
     "postal_code": "1608338",
     "old_code": "160  ",
     "post_office": "新宿",
     "type": "office",
-    "multiple": false,
-    "new": false,
+    "multiple": true,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ニシシンジュク",
     "alternates": []
   },
   "1638626": {
     "jis": "13104",
@@ -129418,33 +129456,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ナカオチアイ",
     "alternates": []
   },
-  "1628446": {
-    "jis": "13104",
-    "kana": "(カブ) ジエイテイ-ビ-パブリツシング",
-    "name": "（株）　ＪＴＢパブリッシング",
-    "prefecture": "東京都",
-    "city": "新宿区",
-    "neighborhood": "払方町",
-    "banchi": "25-5",
-    "postal_code": "1628446",
-    "old_code": "162  ",
-    "post_office": "牛込",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "シンジュクク",
-    "neighborhood_kana": "ハライカタマチ",
-    "alternates": []
-  },
   "1628415": {
     "jis": "13104",
     "kana": "アンステイチユ・フランセトウキヨウ",
     "name": "アンスティチュ・フランセ東京",
     "prefecture": "東京都",
     "city": "新宿区",
     "neighborhood": "市谷船河原町",
@@ -130799,15 +130818,15 @@
     "neighborhood": "若松町",
     "banchi": "2-2",
     "postal_code": "1628480",
     "old_code": "162  ",
     "post_office": "牛込",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ワカマツチョウ",
     "alternates": []
   },
   "1628644": {
     "jis": "13104",
@@ -131376,14 +131395,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ニシシンジュク",
     "alternates": []
   },
+  "1638620": {
+    "jis": "13104",
+    "kana": "ソンガイホケンジヤパン カブシキガイシヤ",
+    "name": "損害保険ジャパン　株式会社",
+    "prefecture": "東京都",
+    "city": "新宿区",
+    "neighborhood": "西新宿",
+    "banchi": "1-26-1",
+    "postal_code": "1638620",
+    "old_code": "163  ",
+    "post_office": "新宿",
+    "type": "office",
+    "multiple": true,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "シンジュクク",
+    "neighborhood_kana": "ニシシンジュク",
+    "alternates": []
+  },
   "1630261": {
     "jis": "13104",
     "kana": "ヒカリビジネスフオ-ム カブシキガイシヤ",
     "name": "光ビジネスフォーム　株式会社",
     "prefecture": "東京都",
     "city": "新宿区",
     "neighborhood": "西新宿",
@@ -142682,14 +142720,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "コウトウク",
     "neighborhood_kana": "アオミ",
     "alternates": []
   },
+  "1358165": {
+    "jis": "13108",
+    "kana": "カブシキガイシヤ ジエイテイビ-パブリツシング",
+    "name": "株式会社　ＪＴＢパブリッシング",
+    "prefecture": "東京都",
+    "city": "江東区",
+    "neighborhood": "豊洲",
+    "banchi": "5-6-36豊洲プライムスクエア11階",
+    "postal_code": "1358165",
+    "old_code": "135  ",
+    "post_office": "晴海",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "コウトウク",
+    "neighborhood_kana": "トヨス",
+    "alternates": []
+  },
   "1358451": {
     "jis": "13108",
     "kana": "カブシキガイシヤ ジエイピ-ビジネスサ-ビス",
     "name": "株式会社　ＪＰビジネスサービス",
     "prefecture": "東京都",
     "city": "江東区",
     "neighborhood": "深川",
@@ -146408,14 +146465,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シナガワク",
     "neighborhood_kana": "ミナミオオイ",
     "alternates": []
   },
+  "1408574": {
+    "jis": "13109",
+    "kana": "カブシキカイシヤ ヒタチセイサクシヨデジタルシステムアンドサ-ビストウカツホンブ",
+    "name": "株式会社　日立製作所デジタルシステム＆サービス統括本部",
+    "prefecture": "東京都",
+    "city": "品川区",
+    "neighborhood": "南大井",
+    "banchi": "六丁目26-1大森ベルポートA館",
+    "postal_code": "1408574",
+    "old_code": "140  ",
+    "post_office": "品川",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "シナガワク",
+    "neighborhood_kana": "ミナミオオイ",
+    "alternates": []
+  },
   "1408619": {
     "jis": "13109",
     "kana": "カブシキガイシヤ アクセスコクサイネツトワ-ク",
     "name": "株式会社　アクセス国際ネットワーク",
     "prefecture": "東京都",
     "city": "品川区",
     "neighborhood": "東品川",
@@ -178281,26 +178357,26 @@
     "prefecture_kana": "トウキョウト",
     "city_kana": "マチダシ",
     "neighborhood_kana": "ミナミオオヤ",
     "alternates": []
   },
   "1940297": {
     "jis": "13209",
-    "kana": "イリヨウホウジンシヤダン コウリユウカイタマキユウリヨウビヨウイン",
-    "name": "医療法人社団　幸隆会多摩丘陵病院",
+    "kana": "イリヨウホウジンシヤダン コウリユウカイ タマキユウリヨウリハビリテ-シヨンビヨウイン",
+    "name": "医療法人社団　幸隆会　多摩丘陵リハビリテーション病院",
     "prefecture": "東京都",
     "city": "町田市",
     "neighborhood": "下小山田町",
     "banchi": "1491",
     "postal_code": "1940297",
     "old_code": "19402",
     "post_office": "町田西",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "マチダシ",
     "neighborhood_kana": "シモオヤマダマチ",
     "alternates": []
   },
   "1940294": {
     "jis": "13209",
@@ -195540,21 +195616,21 @@
   "2498686": {
     "jis": "14208",
     "kana": "ズシシヤクシヨ",
     "name": "逗子市役所",
     "prefecture": "神奈川県",
     "city": "逗子市",
     "neighborhood": "逗子",
-    "banchi": "5丁目2-16(逗子郵便局私書箱第26号)",
+    "banchi": "5丁目2-16",
     "postal_code": "2498686",
     "old_code": "249  ",
     "post_office": "逗子",
-    "type": "box",
+    "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ズシシ",
     "neighborhood_kana": "ズシ",
     "alternates": []
   },
   "2380292": {
     "jis": "14210",
@@ -197908,33 +197984,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ニイガタケン",
     "city_kana": "ニイガタシキタク",
     "neighborhood_kana": "シマミチョウ",
     "alternates": []
   },
-  "9503393": {
-    "jis": "15101",
-    "kana": "ニイガタシキタクヤクシヨ",
-    "name": "新潟市北区役所",
-    "prefecture": "新潟県",
-    "city": "新潟市北区",
-    "neighborhood": "葛塚",
-    "banchi": "3197",
-    "postal_code": "9503393",
-    "old_code": "95033",
-    "post_office": "豊栄",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "ニイガタケン",
-    "city_kana": "ニイガタシキタク",
-    "neighborhood_kana": "クズツカ",
-    "alternates": []
-  },
   "9508735": {
     "jis": "15102",
     "kana": "イチマサカマボコ カブシキガイシヤ",
     "name": "一正蒲鉾　株式会社",
     "prefecture": "新潟県",
     "city": "新潟市東区",
     "neighborhood": "津島屋",
@@ -198054,15 +198111,15 @@
     "neighborhood": "宝町",
     "banchi": "13-5",
     "postal_code": "9508730",
     "old_code": "950  ",
     "post_office": "新潟中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ニイガタケン",
     "city_kana": "ニイガタシヒガシク",
     "neighborhood_kana": "タカラマチ",
     "alternates": []
   },
   "9508725": {
     "jis": "15102",
@@ -203317,15 +203374,15 @@
     "neighborhood": "学校町",
     "banchi": "1丁目1番1号",
     "postal_code": "9408530",
     "old_code": "940  ",
     "post_office": "長岡",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ニイガタケン",
     "city_kana": "ナガオカシ",
     "neighborhood_kana": "ガッコウチョウ",
     "alternates": []
   },
   "9408583": {
     "jis": "15202",
@@ -205007,18 +205064,18 @@
     "name": "柏崎厚生病院",
     "prefecture": "新潟県",
     "city": "柏崎市",
     "neighborhood": "大字茨目",
     "banchi": "字二ツ池2071-1",
     "postal_code": "9451392",
     "old_code": "94513",
-    "post_office": "田尻",
+    "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451395": {
     "jis": "15205",
@@ -205026,18 +205083,18 @@
     "name": "株式会社　サイカワ",
     "prefecture": "新潟県",
     "city": "柏崎市",
     "neighborhood": "大字安田",
     "banchi": "7586",
     "postal_code": "9451395",
     "old_code": "94513",
-    "post_office": "田尻",
+    "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451393": {
     "jis": "15205",
@@ -205045,18 +205102,18 @@
     "name": "新潟産業大学",
     "prefecture": "新潟県",
     "city": "柏崎市",
     "neighborhood": "大字軽井川",
     "banchi": "4730",
     "postal_code": "9451393",
     "old_code": "94513",
-    "post_office": "田尻",
+    "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451397": {
     "jis": "15205",
@@ -205064,18 +205121,18 @@
     "name": "新潟産業大学附属高等学校",
     "prefecture": "新潟県",
     "city": "柏崎市",
     "neighborhood": "大字安田",
     "banchi": "2510-2",
     "postal_code": "9451397",
     "old_code": "94513",
-    "post_office": "田尻",
+    "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451398": {
     "jis": "15205",
@@ -205083,18 +205140,18 @@
     "name": "富士ゼロックスマニュファクチュアリング　株式会社　新潟事業所",
     "prefecture": "新潟県",
     "city": "柏崎市",
     "neighborhood": "大字安田",
     "banchi": "7546",
     "postal_code": "9451398",
     "old_code": "94513",
-    "post_office": "田尻",
+    "post_office": "柏崎",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "9451595": {
     "jis": "15205",
@@ -210504,15 +210561,15 @@
     "neighborhood": "牛島新町",
     "banchi": "11番7号",
     "postal_code": "9308554",
     "old_code": "930  ",
     "post_office": "富山南",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トヤマケン",
     "city_kana": "トヤマシ",
     "neighborhood_kana": "ウシジマシンマチ",
     "alternates": []
   },
   "9308518": {
     "jis": "16201",
@@ -210949,26 +211006,26 @@
     "prefecture_kana": "トヤマケン",
     "city_kana": "トヤマシ",
     "neighborhood_kana": "ヒガシクロマキ",
     "alternates": []
   },
   "9301392": {
     "jis": "16201",
-    "kana": "トヤマシオオヤマソウゴウギヨウセイセンタ-",
-    "name": "富山市大山総合行政センター",
+    "kana": "トヤマシオオヤマカイカン(オオヤマギヨウセイサ-ビスセンタ-・オオヤマホケンフクシセンタ-)",
+    "name": "富山市大山会館（大山行政サービスセンター・大山保健福祉センター）",
     "prefecture": "富山県",
     "city": "富山市",
     "neighborhood": "上滝",
-    "banchi": "525",
+    "banchi": "567",
     "postal_code": "9301392",
     "old_code": "93013",
     "post_office": "上滝",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トヤマケン",
     "city_kana": "トヤマシ",
     "neighborhood_kana": "カミダキ",
     "alternates": []
   },
   "9302198": {
     "jis": "16201",
@@ -211910,15 +211967,15 @@
     "neighborhood": "楡原",
     "banchi": "1128番地",
     "postal_code": "9392192",
     "old_code": "93921",
     "post_office": "細入",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トヤマケン",
     "city_kana": "トヤマシ",
     "neighborhood_kana": "ニレハラ",
     "alternates": []
   },
   "9392297": {
     "jis": "16201",
@@ -211986,15 +212043,15 @@
     "neighborhood": "高内",
     "banchi": "365番地",
     "postal_code": "9392293",
     "old_code": "93922",
     "post_office": "大沢野",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トヤマケン",
     "city_kana": "トヤマシ",
     "neighborhood_kana": "タカウチ",
     "alternates": []
   },
   "9392292": {
     "jis": "16201",
@@ -216872,15 +216929,15 @@
     "neighborhood": "浅野本町",
     "banchi": "1丁目10-10",
     "postal_code": "9208611",
     "old_code": "920  ",
     "post_office": "金沢中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "カナザワシ",
     "neighborhood_kana": "アサノホンマチ",
     "alternates": []
   },
   "9208619": {
     "jis": "17201",
@@ -218723,14 +218780,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "カナザワシ",
     "neighborhood_kana": "マツシマ",
     "alternates": []
   },
+  "9201184": {
+    "jis": "17201",
+    "kana": "イオンリテ-ル カブシキガイシヤ イオンモリノサトテン",
+    "name": "イオンリテール　株式会社　イオンもりの里店",
+    "prefecture": "石川県",
+    "city": "金沢市",
+    "neighborhood": "もりの里",
+    "banchi": "1丁目70",
+    "postal_code": "9201184",
+    "old_code": "92011",
+    "post_office": "金沢中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "イシカワケン",
+    "city_kana": "カナザワシ",
+    "neighborhood_kana": "モリノサト",
+    "alternates": []
+  },
   "9201185": {
     "jis": "17201",
     "kana": "イリヨウホウジン ジユウゼンカイ",
     "name": "医療法人　十全会",
     "prefecture": "石川県",
     "city": "金沢市",
     "neighborhood": "田上本町",
@@ -218780,33 +218856,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "カナザワシ",
     "neighborhood_kana": "カクママチ",
     "alternates": []
   },
-  "9201184": {
-    "jis": "17201",
-    "kana": "ホクリクジヤスコ モリノサトシヨツピングセンタ-",
-    "name": "北陸ジャスコ　杜の里ＳＣ",
-    "prefecture": "石川県",
-    "city": "金沢市",
-    "neighborhood": "もりの里",
-    "banchi": "1丁目70",
-    "postal_code": "9201184",
-    "old_code": "92011",
-    "post_office": "金沢中央",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "イシカワケン",
-    "city_kana": "カナザワシ",
-    "neighborhood_kana": "モリノサト",
-    "alternates": []
-  },
   "9201180": {
     "jis": "17201",
     "kana": "ホクリクダイガク",
     "name": "北陸大学",
     "prefecture": "石川県",
     "city": "金沢市",
     "neighborhood": "太陽が丘",
@@ -232255,26 +232312,26 @@
     "prefecture_kana": "ヤマナシケン",
     "city_kana": "ミナミコマグンフジカワチョウ",
     "neighborhood_kana": "サイショウジ",
     "alternates": []
   },
   "4000593": {
     "jis": "19368",
-    "kana": "ニスカ カブシキガイシヤ",
-    "name": "ニスカ　株式会社",
+    "kana": "キヤノンフアインテツクニスカ カブシキガイシヤ",
+    "name": "キャノンファインテックニスカ　株式会社",
     "prefecture": "山梨県",
     "city": "南巨摩郡富士川町",
     "neighborhood": "小林",
     "banchi": "430番地1",
     "postal_code": "4000593",
     "old_code": "40005",
     "post_office": "青柳",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "ヤマナシケン",
     "city_kana": "ミナミコマグンフジカワチョウ",
     "neighborhood_kana": "コバヤシ",
     "alternates": []
   },
   "4000592": {
     "jis": "19368",
@@ -232298,21 +232355,21 @@
   "4000693": {
     "jis": "19368",
     "kana": "カジカザワゼイムシヨ",
     "name": "鰍沢税務署",
     "prefecture": "山梨県",
     "city": "南巨摩郡富士川町",
     "neighborhood": "鰍沢",
-    "banchi": "1502-1",
+    "banchi": "1760番地1富士川地方合同庁舎3階",
     "postal_code": "4000693",
     "old_code": "40006",
     "post_office": "鰍沢",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "ヤマナシケン",
     "city_kana": "ミナミコマグンフジカワチョウ",
     "neighborhood_kana": "カジカザワ",
     "alternates": []
   },
   "4000695": {
     "jis": "19368",
@@ -237201,25 +237258,25 @@
   },
   "3868666": {
     "jis": "20203",
     "kana": "シンワアドヴアンス カブシキガイシヤ",
     "name": "シンワアドヴァンス　株式会社",
     "prefecture": "長野県",
     "city": "上田市",
-    "neighborhood": "材木町",
-    "banchi": "2丁目9-4産業振興ビル6階",
+    "neighborhood": "住吉",
+    "banchi": "21番地5",
     "postal_code": "3868666",
     "old_code": "386  ",
     "post_office": "上田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "ナガノケン",
     "city_kana": "ウエダシ",
-    "neighborhood_kana": "ザイモクチョウ",
+    "neighborhood_kana": "スミヨシ",
     "alternates": []
   },
   "3868705": {
     "jis": "20203",
     "kana": "チユウブデンリヨクパワ-グリツド カブシキガイシヤ ウエダエイギヨウシヨ",
     "name": "中部電力パワーグリッド　株式会社　上田営業所",
     "prefecture": "長野県",
@@ -237425,29 +237482,29 @@
     "prefecture_kana": "ナガノケン",
     "city_kana": "ウエダシ",
     "neighborhood_kana": "テンジン",
     "alternates": []
   },
   "3860192": {
     "jis": "20203",
-    "kana": "トウキヨウトクシユデンセン カブシキカイシヤ",
-    "name": "東京特殊電線　株式会社",
+    "kana": "カブシキガイシヤ トウトク",
+    "name": "株式会社　ＴＯＴＯＫＵ",
     "prefecture": "長野県",
     "city": "上田市",
-    "neighborhood": "大字大屋",
-    "banchi": "300",
+    "neighborhood": "大屋",
+    "banchi": "300番地",
     "postal_code": "3860192",
     "old_code": "38601",
-    "post_office": "大屋",
+    "post_office": "上田",
     "type": "office",
     "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
+    "new": true,
+    "prefecture_kana": "ナガノケン",
+    "city_kana": "ウエダシ",
+    "neighborhood_kana": "オオヤ",
     "alternates": []
   },
   "3868505": {
     "jis": "20203",
     "kana": "ニツシンコウギヨウ カブシキガイシヤ",
     "name": "日信工業　株式会社",
     "prefecture": "長野県",
@@ -247097,33 +247154,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ギフケン",
     "city_kana": "オオガキシ",
     "neighborhood_kana": "カミイシヅチョウオツサカ",
     "alternates": []
   },
-  "5038553": {
-    "jis": "21202",
-    "kana": "カブシキガイシヤ ヨシダハム",
-    "name": "株式会社　吉田ハム",
-    "prefecture": "岐阜県",
-    "city": "大垣市",
-    "neighborhood": "寿町",
-    "banchi": "1-1",
-    "postal_code": "5038553",
-    "old_code": "503  ",
-    "post_office": "大垣",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "ギフケン",
-    "city_kana": "オオガキシ",
-    "neighborhood_kana": "コトブキチョウ",
-    "alternates": []
-  },
   "5038550": {
     "jis": "21202",
     "kana": "ギフケイザイダイガク",
     "name": "岐阜経済大学",
     "prefecture": "岐阜県",
     "city": "大垣市",
     "neighborhood": "北方町",
@@ -247192,14 +247230,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ギフケン",
     "city_kana": "オオガキシ",
     "neighborhood_kana": "モトイマチョウ",
     "alternates": []
   },
+  "5038553": {
+    "jis": "21202",
+    "kana": "ジエイエイゼンノウミ-トフ-ズ カブシキガイシヤ チユウブエイギヨウホンブ ヨシダハムシテン",
+    "name": "ＪＡ全農ミートフーズ　株式会社　中部営業本部　吉田ハム支店",
+    "prefecture": "岐阜県",
+    "city": "大垣市",
+    "neighborhood": "寿町",
+    "banchi": "1番地の1",
+    "postal_code": "5038553",
+    "old_code": "503  ",
+    "post_office": "大垣",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ギフケン",
+    "city_kana": "オオガキシ",
+    "neighborhood_kana": "コトブキチョウ",
+    "alternates": []
+  },
   "5038567": {
     "jis": "21202",
     "kana": "スイトピアセンタ-",
     "name": "スイトピアセンター",
     "prefecture": "岐阜県",
     "city": "大垣市",
     "neighborhood": "室本町",
@@ -248250,15 +248307,15 @@
     "neighborhood": "音羽町",
     "banchi": "1丁目233番地",
     "postal_code": "5078787",
     "old_code": "507  ",
     "post_office": "多治見",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ギフケン",
     "city_kana": "タジミシ",
     "neighborhood_kana": "オトワチョウ",
     "alternates": []
   },
   "5078608": {
     "jis": "21204",
@@ -250036,15 +250093,15 @@
     "neighborhood": "塩河",
     "banchi": "2232",
     "postal_code": "5090289",
     "old_code": "50902",
     "post_office": "可児",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ギフケン",
     "city_kana": "カニシ",
     "neighborhood_kana": "シュウガ",
     "alternates": []
   },
   "5090298": {
     "jis": "21214",
@@ -273410,15 +273467,15 @@
     "neighborhood": "錦",
     "banchi": "二丁目11番6号エフリードビル7階",
     "postal_code": "4608628",
     "old_code": "460  ",
     "post_office": "名古屋中",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシナカク",
     "neighborhood_kana": "ニシキ",
     "alternates": []
   },
   "4608585": {
     "jis": "23106",
@@ -279129,15 +279186,15 @@
     "neighborhood": "勢子坊",
     "banchi": "二丁目1501番地",
     "postal_code": "4658650",
     "old_code": "465  ",
     "post_office": "名東",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシメイトウク",
     "neighborhood_kana": "セコボウ",
     "alternates": []
   },
   "4658620": {
     "jis": "23115",
@@ -284546,15 +284603,15 @@
     "neighborhood": "白鳥町",
     "banchi": "兎足1番16号",
     "postal_code": "4428550",
     "old_code": "442  ",
     "post_office": "豊川",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "トヨカワシ",
     "neighborhood_kana": "シロトリチョウ",
     "alternates": []
   },
   "4428531": {
     "jis": "23207",
@@ -291361,21 +291418,21 @@
   "4411692": {
     "jis": "23221",
     "kana": "シンシロシ ホウライソウゴウシシヨ",
     "name": "新城市　鳳来総合支所",
     "prefecture": "愛知県",
     "city": "新城市",
     "neighborhood": "長篠",
-    "banchi": "字下り筬1-2",
+    "banchi": "字仲野16番地11",
     "postal_code": "4411692",
     "old_code": "44116",
     "post_office": "長篠",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "アイチケン",
     "city_kana": "シンシロシ",
     "neighborhood_kana": "ナガシノ",
     "alternates": []
   },
   "4768666": {
     "jis": "23222",
@@ -294167,50 +294224,50 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ヤトミシ",
     "neighborhood_kana": "マエガスチョウ",
     "alternates": []
   },
-  "4700297": {
+  "4700292": {
     "jis": "23236",
-    "kana": "シヨウワブツサン カブシキガイシヤ",
-    "name": "昌和物産　株式会社",
+    "kana": "エヌシ-エ-",
+    "name": "ＮＣＡ",
     "prefecture": "愛知県",
     "city": "みよし市",
-    "neighborhood": "福谷町",
-    "banchi": "下地念古67",
-    "postal_code": "4700297",
-    "old_code": "470  ",
+    "neighborhood": "莇生町",
+    "banchi": "下永井田20",
+    "postal_code": "4700292",
+    "old_code": "47002",
     "post_office": "三好",
     "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ミヨシシ",
-    "neighborhood_kana": "ウキガイチョウ",
+    "neighborhood_kana": "アザブチョウ",
     "alternates": []
   },
-  "4700292": {
+  "4700297": {
     "jis": "23236",
-    "kana": "エヌシ-エ-",
-    "name": "ＮＣＡ",
+    "kana": "カブシキカイシヤ コウソク チユウキヨウエイギヨウブ",
+    "name": "株式会社　高速　中京営業部",
     "prefecture": "愛知県",
     "city": "みよし市",
-    "neighborhood": "莇生町",
-    "banchi": "下永井田20",
-    "postal_code": "4700292",
+    "neighborhood": "根浦町",
+    "banchi": "七丁目2番地1",
+    "postal_code": "4700297",
     "old_code": "47002",
     "post_office": "三好",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "アイチケン",
     "city_kana": "ミヨシシ",
-    "neighborhood_kana": "アザブチョウ",
+    "neighborhood_kana": "ネウラマチ",
     "alternates": []
   },
   "4700294": {
     "jis": "23236",
     "kana": "カブシキガイシヤ サンゴ",
     "name": "株式会社　三五",
     "prefecture": "愛知県",
@@ -295796,15 +295853,15 @@
     "neighborhood": "栄町",
     "banchi": "一丁目941",
     "postal_code": "5148515",
     "old_code": "514  ",
     "post_office": "津中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ミエケン",
     "city_kana": "ツシ",
     "neighborhood_kana": "サカエマチ",
     "alternates": []
   },
   "5148530": {
     "jis": "24201",
@@ -311754,21 +311811,21 @@
   "5378911": {
     "jis": "27115",
     "kana": "ザ・パツク カブシキガイシヤ",
     "name": "ザ・パック　株式会社",
     "prefecture": "大阪府",
     "city": "大阪市東成区",
     "neighborhood": "東小橋",
-    "banchi": "2丁目9番9号",
+    "banchi": "2丁目9番3号",
     "postal_code": "5378911",
     "old_code": "537  ",
     "post_office": "東成",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシヒガシナリク",
     "neighborhood_kana": "ヒガシオバセ",
     "alternates": []
   },
   "5378501": {
     "jis": "27115",
@@ -317801,25 +317858,25 @@
   },
   "5418589": {
     "jis": "27128",
     "kana": "オザツクス カブシキガイシヤ",
     "name": "オザックス　株式会社",
     "prefecture": "大阪府",
     "city": "大阪市中央区",
-    "neighborhood": "博労町",
-    "banchi": "1丁目6-6",
+    "neighborhood": "北浜",
+    "banchi": "3丁目5番29号-13階",
     "postal_code": "5418589",
     "old_code": "541  ",
     "post_office": "大阪東",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
-    "neighborhood_kana": "バクロウマチ",
+    "neighborhood_kana": "キタハマ",
     "alternates": []
   },
   "5418526": {
     "jis": "27128",
     "kana": "オノヤクヒンコウギヨウ カブシキガイシヤ",
     "name": "小野薬品工業　株式会社",
     "prefecture": "大阪府",
@@ -317852,14 +317909,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
     "neighborhood_kana": "アワジマチ",
     "alternates": []
   },
+  "5418528": {
+    "jis": "27128",
+    "kana": "カブシキカイシヤ ニツケンセツケイ",
+    "name": "株式会社　日建設計",
+    "prefecture": "大阪府",
+    "city": "大阪市中央区",
+    "neighborhood": "瓦町",
+    "banchi": "3-6-5",
+    "postal_code": "5418528",
+    "old_code": "541  ",
+    "post_office": "大阪東",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "オオサカフ",
+    "city_kana": "オオサカシチュウオウク",
+    "neighborhood_kana": "カワラマチ",
+    "alternates": []
+  },
   "5416666": {
     "jis": "27128",
     "kana": "カブシキガイシヤ オオニシ",
     "name": "株式会社　大西",
     "prefecture": "大阪府",
     "city": "大阪市中央区",
     "neighborhood": "久太郎町",
@@ -317909,33 +317985,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
     "neighborhood_kana": "カワラマチ",
     "alternates": []
   },
-  "5418528": {
-    "jis": "27128",
-    "kana": "カブシキガイシヤ ニツケンセツケイ",
-    "name": "株式会社　日建設計",
-    "prefecture": "大阪府",
-    "city": "大阪市中央区",
-    "neighborhood": "高麗橋",
-    "banchi": "4丁目6-2",
-    "postal_code": "5418528",
-    "old_code": "541  ",
-    "post_office": "大阪東",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "オオサカフ",
-    "city_kana": "オオサカシチュウオウク",
-    "neighborhood_kana": "コウライバシ",
-    "alternates": []
-  },
   "5418515": {
     "jis": "27128",
     "kana": "カブシキガイシヤ ニホンケイザイシンブンシヤ オオサカホンシヤ",
     "name": "株式会社　日本経済新聞社　大阪本社",
     "prefecture": "大阪府",
     "city": "大阪市中央区",
     "neighborhood": "高麗橋",
@@ -318029,25 +318086,25 @@
   },
   "5418575": {
     "jis": "27128",
     "kana": "カブシキガイシヤ メイセイシヨウカイ",
     "name": "株式会社　明成商会",
     "prefecture": "大阪府",
     "city": "大阪市中央区",
-    "neighborhood": "伏見町",
-    "banchi": "4丁目4-1日生伏見町ビル本館5F",
+    "neighborhood": "今橋",
+    "banchi": "2丁目4番10号淀屋橋北浜センタービル2階",
     "postal_code": "5418575",
     "old_code": "541  ",
     "post_office": "大阪東",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
-    "neighborhood_kana": "フシミマチ",
+    "neighborhood_kana": "イマバシ",
     "alternates": []
   },
   "5418517": {
     "jis": "27128",
     "kana": "カブシキガイシヤ モリモトグミ",
     "name": "株式会社　森本組",
     "prefecture": "大阪府",
@@ -320716,15 +320773,15 @@
     "neighborhood": "名神口",
     "banchi": "1丁目10-1",
     "postal_code": "5618530",
     "old_code": "561  ",
     "post_office": "豊中南",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "トヨナカシ",
     "neighborhood_kana": "メイシングチ",
     "alternates": []
   },
   "5618558": {
     "jis": "27203",
@@ -323230,14 +323287,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "ヤオシ",
     "neighborhood_kana": "キタカメイチョウ",
     "alternates": []
   },
+  "5818502": {
+    "jis": "27212",
+    "kana": "ジエイピ-ラクテンロジステイクス カブシキガイシヤ ラクテンフルフイルメントセンタ-ヤオ",
+    "name": "ＪＰ楽天ロジスティクス　株式会社　楽天フルフィルメントセンター八尾",
+    "prefecture": "大阪府",
+    "city": "八尾市",
+    "neighborhood": "郡川",
+    "banchi": "一丁目557GLP八尾Ⅰ",
+    "postal_code": "5818502",
+    "old_code": "581  ",
+    "post_office": "八尾",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "オオサカフ",
+    "city_kana": "ヤオシ",
+    "neighborhood_kana": "コオリガワ",
+    "alternates": []
+  },
   "5818505": {
     "jis": "27212",
     "kana": "ミキシヨウコウ カブシキガイシヤ",
     "name": "三起商行　株式会社",
     "prefecture": "大阪府",
     "city": "八尾市",
     "neighborhood": "若林町",
@@ -330298,33 +330374,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ヒョウゴケン",
     "city_kana": "アマガサキシ",
     "neighborhood_kana": "ヒガシハマチョウ",
     "alternates": []
   },
-  "6608510": {
-    "jis": "28202",
-    "kana": "カブシキガイシヤ モノタロウ アマガサキデイストリビユ-シヨンセンタ-",
-    "name": "株式会社　ＭｏｎｏｔａＲＯ　尼崎ディストリビューションセンター",
-    "prefecture": "兵庫県",
-    "city": "尼崎市",
-    "neighborhood": "西向島町",
-    "banchi": "75-1プロロジスパーク尼崎3",
-    "postal_code": "6608510",
-    "old_code": "660  ",
-    "post_office": "尼崎",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "ヒョウゴケン",
-    "city_kana": "アマガサキシ",
-    "neighborhood_kana": "ニシムコウジマチョウ",
-    "alternates": []
-  },
   "6608558": {
     "jis": "28202",
     "kana": "カンサイデンリヨクソウハイデン カブシキガイシヤ ハンシンハイデンエイギヨウシヨ",
     "name": "関西電力送配電　株式会社　阪神配電営業所",
     "prefecture": "兵庫県",
     "city": "尼崎市",
     "neighborhood": "西長洲町",
@@ -341312,15 +341369,15 @@
     "neighborhood": "立川町",
     "banchi": "7丁目101番地",
     "postal_code": "6808634",
     "old_code": "680  ",
     "post_office": "鳥取中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トットリケン",
     "city_kana": "トットリシ",
     "neighborhood_kana": "タチカワチョウ",
     "alternates": []
   },
   "6808577": {
     "jis": "31201",
@@ -343009,14 +343066,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トットリケン",
     "city_kana": "ヒノグンニチナンチョウ",
     "neighborhood_kana": "カスミ",
     "alternates": []
   },
+  "6908601": {
+    "jis": "32201",
+    "kana": "エヌエイチケイ マツエホウソウキヨク",
+    "name": "ＮＨＫ　松江放送局",
+    "prefecture": "島根県",
+    "city": "松江市",
+    "neighborhood": "灘町",
+    "banchi": "101-6(松江中央郵便局私書箱第7号)",
+    "postal_code": "6908601",
+    "old_code": "690  ",
+    "post_office": "松江中央",
+    "type": "box",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "シマネケン",
+    "city_kana": "マツエシ",
+    "neighborhood_kana": "ナダマチ",
+    "alternates": []
+  },
   "6908550": {
     "jis": "32201",
     "kana": "カナツギケンコウギヨウ カブシキガイシヤ",
     "name": "カナツ技建工業　株式会社",
     "prefecture": "島根県",
     "city": "松江市",
     "neighborhood": "春日町",
@@ -344187,33 +344263,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "マツエシ",
     "neighborhood_kana": "トノマチ",
     "alternates": []
   },
-  "6908601": {
-    "jis": "32201",
-    "kana": "ニホンホウソウキヨウカイ マツエホウソウキヨク",
-    "name": "日本放送協会　松江放送局",
-    "prefecture": "島根県",
-    "city": "松江市",
-    "neighborhood": "灘町",
-    "banchi": "1-21(松江中央郵便局私書箱第7号)",
-    "postal_code": "6908601",
-    "old_code": "69091",
-    "post_office": "松江中央",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "シマネケン",
-    "city_kana": "マツエシ",
-    "neighborhood_kana": "ナダマチ",
-    "alternates": []
-  },
   "6990492": {
     "jis": "32201",
     "kana": "シマネケンリツ シンジコウトウガツコウ",
     "name": "島根県立　宍道高等学校",
     "prefecture": "島根県",
     "city": "松江市",
     "neighborhood": "宍道町宍道",
@@ -344947,14 +345004,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "マスダシ",
     "neighborhood_kana": "トキワチョウ",
     "alternates": []
   },
+  "6988506": {
+    "jis": "32204",
+    "kana": "ソニ-ネツトワ-クコミユニケ-シヨンズ カブシキガイシヤ",
+    "name": "ソニーネットワークコミュニケーションズ　株式会社",
+    "prefecture": "島根県",
+    "city": "益田市",
+    "neighborhood": "駅前町",
+    "banchi": "17-1益田駅前ビルEAGA3F",
+    "postal_code": "6988506",
+    "old_code": "698  ",
+    "post_office": "益田",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "シマネケン",
+    "city_kana": "マスダシ",
+    "neighborhood_kana": "エキマエチョウ",
+    "alternates": []
+  },
   "6988651": {
     "jis": "32204",
     "kana": "マスダ ゼイムシヨ",
     "name": "益田　税務署",
     "prefecture": "島根県",
     "city": "益田市",
     "neighborhood": "元町",
@@ -350647,14 +350723,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "オカヤマケン",
     "city_kana": "クラシキシ",
     "neighborhood_kana": "タマシマアガサキ",
     "alternates": []
   },
+  "7138588": {
+    "jis": "33202",
+    "kana": "サクヨウガクエンコウトウガツコウ",
+    "name": "作陽学園高等学校",
+    "prefecture": "岡山県",
+    "city": "倉敷市",
+    "neighborhood": "玉島八島",
+    "banchi": "1541番1",
+    "postal_code": "7138588",
+    "old_code": "713  ",
+    "post_office": "玉島",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "オカヤマケン",
+    "city_kana": "クラシキシ",
+    "neighborhood_kana": "タマシマヤシマ",
+    "alternates": []
+  },
   "7138501": {
     "jis": "33202",
     "kana": "スミトモジユウキカイコウギヨウ カブシキカイシヤ オカヤマセイゾウシヨ",
     "name": "住友重機械工業　株式会社　岡山製造所",
     "prefecture": "岡山県",
     "city": "倉敷市",
     "neighborhood": "玉島乙島",
@@ -382988,15 +383083,15 @@
     "neighborhood": "春野町西分",
     "banchi": "15",
     "postal_code": "7810392",
     "old_code": "78103",
     "post_office": "春野",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "コウチケン",
     "city_kana": "コウチシ",
     "neighborhood_kana": "ハルノチョウニシブン",
     "alternates": []
   },
   "7815192": {
     "jis": "39201",
@@ -386358,33 +386453,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "キタキュウシュウシコクラミナミク",
     "neighborhood_kana": "キタガタ",
     "alternates": []
   },
-  "8028529": {
-    "jis": "40107",
-    "kana": "コクラコウチシシヨ",
-    "name": "小倉拘置支所",
-    "prefecture": "福岡県",
-    "city": "北九州市小倉南区",
-    "neighborhood": "葉山町",
-    "banchi": "1丁目1番8号",
-    "postal_code": "8028529",
-    "old_code": "802  ",
-    "post_office": "北九州中央",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "フクオカケン",
-    "city_kana": "キタキュウシュウシコクラミナミク",
-    "neighborhood_kana": "ハヤマチョウ",
-    "alternates": []
-  },
   "8028533": {
     "jis": "40107",
     "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ コクライリヨウセンタ-",
     "name": "独立行政法人　国立病院機構　小倉医療センター",
     "prefecture": "福岡県",
     "city": "北九州市小倉南区",
     "neighborhood": "春ケ丘",
@@ -387859,47 +387935,28 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "フクオカシヒガシク",
     "neighborhood_kana": "カシイハマフトウ",
     "alternates": []
   },
-  "8138568": {
-    "jis": "40131",
-    "kana": "カブシキガイシヤ ヤマヤ",
-    "name": "株式会社　やまや",
-    "prefecture": "福岡県",
-    "city": "福岡市東区",
-    "neighborhood": "松島",
-    "banchi": "5丁目27-5",
-    "postal_code": "8138568",
-    "old_code": "813  ",
-    "post_office": "福岡東",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "フクオカケン",
-    "city_kana": "フクオカシヒガシク",
-    "neighborhood_kana": "マツシマ",
-    "alternates": []
-  },
   "8138533": {
     "jis": "40131",
     "kana": "カブシキガイシヤ ルルア-ク",
     "name": "株式会社　ルルアーク",
     "prefecture": "福岡県",
     "city": "福岡市東区",
     "neighborhood": "松島",
     "banchi": "3丁目30-23",
     "postal_code": "8138533",
     "old_code": "813  ",
     "post_office": "福岡東",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "フクオカシヒガシク",
     "neighborhood_kana": "マツシマ",
     "alternates": []
   },
   "8138680": {
     "jis": "40131",
@@ -388068,33 +388125,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "フクオカシヒガシク",
     "neighborhood_kana": "チハヤ",
     "alternates": []
   },
-  "8138578": {
-    "jis": "40131",
-    "kana": "ヤマヤチヨクハン カブシキガイシヤ",
-    "name": "やまや直販　株式会社",
-    "prefecture": "福岡県",
-    "city": "福岡市東区",
-    "neighborhood": "松島",
-    "banchi": "3丁目31-1",
-    "postal_code": "8138578",
-    "old_code": "813  ",
-    "post_office": "福岡東",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "フクオカケン",
-    "city_kana": "フクオカシヒガシク",
-    "neighborhood_kana": "マツシマ",
-    "alternates": []
-  },
   "8138626": {
     "jis": "40131",
     "kana": "ユニ-ク カブシキガイシヤ",
     "name": "ユニーク　株式会社",
     "prefecture": "福岡県",
     "city": "福岡市東区",
     "neighborhood": "多の津",
@@ -392268,14 +392306,53 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "フクオカシチュウオウク",
     "neighborhood_kana": "クサガエ",
     "alternates": []
   },
+  "8108571": {
+    "jis": "40133",
+    "kana": "キユウシユウアサヒホウソウ カブシキガイシヤ",
+    "name": "九州朝日放送　株式会社",
+    "prefecture": "福岡県",
+    "city": "福岡市中央区",
+    "neighborhood": "長浜",
+    "banchi": "1丁目1-1",
+    "postal_code": "8108571",
+    "old_code": "810  ",
+    "post_office": "福岡中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "フクオカケン",
+    "city_kana": "フクオカシチュウオウク",
+    "neighborhood_kana": "ナガハマ",
+    "alternates": [
+      {
+        "jis": "40133",
+        "kana": "ケ-ビ-シ-グル-プホ-ルデイングス カブシキガイシヤ",
+        "name": "ＫＢＣグループホールディングス　株式会社",
+        "prefecture": "福岡県",
+        "city": "福岡市中央区",
+        "neighborhood": "長浜",
+        "banchi": "1丁目1-1",
+        "postal_code": "8108571",
+        "old_code": "810  ",
+        "post_office": "福岡中央",
+        "type": "office",
+        "multiple": false,
+        "new": true,
+        "prefecture_kana": "フクオカケン",
+        "city_kana": "フクオカシチュウオウク",
+        "neighborhood_kana": "ナガハマ",
+        "alternates": []
+      }
+    ]
+  },
   "8108560": {
     "jis": "40133",
     "kana": "キユウシユウダイガク ロツポンマツチクブキヨク(ダイガクキヨウイクケンキユウセンタ-.ダイガクインヒカクシヤカイブンカケンキユウカ.ゲンゴブンカブ)",
     "name": "九州大学　六本松地区部局（大学教育研究センター、大学院比較社会文化研究科、言語文化部）",
     "prefecture": "福岡県",
     "city": "福岡市中央区",
     "neighborhood": "六本松",
@@ -393427,33 +393504,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "フクオカシチュウオウク",
     "neighborhood_kana": "アカサカ",
     "alternates": []
   },
-  "8108571": {
-    "jis": "40133",
-    "kana": "キユウシユウアサヒホウソウ カブシキガイシヤ",
-    "name": "九州朝日放送　株式会社",
-    "prefecture": "福岡県",
-    "city": "福岡市中央区",
-    "neighborhood": "長浜",
-    "banchi": "1丁目1-1",
-    "postal_code": "8108571",
-    "old_code": "81071",
-    "post_office": "福岡中央",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "フクオカケン",
-    "city_kana": "フクオカシチュウオウク",
-    "neighborhood_kana": "ナガハマ",
-    "alternates": []
-  },
   "8108577": {
     "jis": "40133",
     "kana": "ニホンホウソウキヨウカイ フクオカホウソウキヨク",
     "name": "日本放送協会　福岡放送局",
     "prefecture": "福岡県",
     "city": "福岡市中央区",
     "neighborhood": "六本松",
@@ -394847,15 +394905,15 @@
     "neighborhood": "田村",
     "banchi": "2丁目15-1",
     "postal_code": "8140193",
     "old_code": "81401",
     "post_office": "城南",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "フクオカシサワラク",
     "neighborhood_kana": "タムラ",
     "alternates": []
   },
   "8148555": {
     "jis": "40137",
@@ -398938,14 +398996,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
+  "8112498": {
+    "jis": "40342",
+    "kana": "カブシキガイシヤ ヤマヤコミユニケ-シヨンズ",
+    "name": "株式会社　やまやコミュニケーションズ",
+    "prefecture": "福岡県",
+    "city": "糟屋郡篠栗町",
+    "neighborhood": "彩り台",
+    "banchi": "1番1号",
+    "postal_code": "8112498",
+    "old_code": "81124",
+    "post_office": "粕屋南",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "フクオカケン",
+    "city_kana": "カスヤグンササグリマチ",
+    "neighborhood_kana": "イロドリダイ",
+    "alternates": []
+  },
   "8112492": {
     "jis": "40342",
     "kana": "ササグリマチヤクバ",
     "name": "篠栗町役場",
     "prefecture": "福岡県",
     "city": "糟屋郡篠栗町",
     "neighborhood": "大字篠栗",
@@ -406582,25 +406659,25 @@
   },
   "8608506": {
     "jis": "43101",
     "kana": "カブシキカイシヤ クマモトニチニチシンブンシヤ",
     "name": "株式会社　熊本日日新聞社",
     "prefecture": "熊本県",
     "city": "熊本市中央区",
-    "neighborhood": "世安町",
-    "banchi": "172番地",
+    "neighborhood": "世安",
+    "banchi": "1丁目5番1号",
     "postal_code": "8608506",
     "old_code": "860  ",
     "post_office": "熊本中央",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "クマモトケン",
     "city_kana": "クマモトシチュウオウク",
-    "neighborhood_kana": "ヨヤスマチ",
+    "neighborhood_kana": "ヨヤス",
     "alternates": []
   },
   "8608539": {
     "jis": "43101",
     "kana": "カブシキカイシヤ トリニテイ",
     "name": "株式会社　トリニティ",
     "prefecture": "熊本県",
```

### Comparing `posuto-2023.4.0/posuto/postaldata.db` & `posuto-2023.5.0/posuto/postaldata.db`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -13691,15 +13691,15 @@
 INSERT INTO postal_data VALUES('9872262','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872262", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテカラタケバヤシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館唐竹林", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館唐竹林');
 INSERT INTO postal_data VALUES('9872228','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872228", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテカワゾエ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館川添", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館川添');
 INSERT INTO postal_data VALUES('9872212','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872212", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテキド", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館木戸", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館木戸');
 INSERT INTO postal_data VALUES('9872261','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872261", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテキュウデン", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館久伝", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館久伝');
 INSERT INTO postal_data VALUES('9872204','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872204", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテクロセ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館黒瀬", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館黒瀬');
 INSERT INTO postal_data VALUES('9872211','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872211", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテゲンコウ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館源光", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館源光');
 INSERT INTO postal_data VALUES('9872273','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872273", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコエダテ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館左足", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館左足');
-INSERT INTO postal_data VALUES('9872265','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコブチニシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館小淵西", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコブチヒガシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館小淵東", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}, {"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサカイダ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館境田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}, {"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサノハラ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館佐野原", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','宮城県','栗原市','築館小淵西');
+INSERT INTO postal_data VALUES('9872265','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコブチニシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館小淵西", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテコブチヒガシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館小淵東", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}, {"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサカイダ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館境田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}, {"jisx0402": "04213", "old_code": "98722", "postal_code": "9872265", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサノハラ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館左野原", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}], "note": null}','宮城県','栗原市','築館小淵西');
 INSERT INTO postal_data VALUES('9872232','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872232", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテサワイリ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館沢入", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館沢入');
 INSERT INTO postal_data VALUES('9872247','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872247", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシモタカモリ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館下高森", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館下高森');
 INSERT INTO postal_data VALUES('9872221','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872221", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシモマチイ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館下待井", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館下待井');
 INSERT INTO postal_data VALUES('9872203','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872203", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシモミヤノ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館下宮野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館下宮野');
 INSERT INTO postal_data VALUES('9872202','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872202", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテジョウノ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館城生野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','栗原市','築館城生野');
 INSERT INTO postal_data VALUES('9872263','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872263", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシンデン", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館新田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872263", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテヤクシガオカ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館薬師ケ丘", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','宮城県','栗原市','築館新田');
 INSERT INTO postal_data VALUES('9872274','{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872274", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテシンナリタニシ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館新成田西", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04213", "old_code": "98722", "postal_code": "9872274", "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテナリタ", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館成田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','宮城県','栗原市','築館新成田西');
@@ -14348,15 +14348,15 @@
 INSERT INTO postal_data VALUES('9810136','{"jisx0402": "04406", "old_code": "98101", "postal_code": "9810136", "prefecture_kana": "ミヤギケン", "city_kana": "ミヤギグンリフチョウ", "neighborhood_kana": "ミナノオカ", "prefecture": "宮城県", "city": "宮城郡利府町", "neighborhood": "皆の丘", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','宮城郡利府町','皆の丘');
 INSERT INTO postal_data VALUES('9810103','{"jisx0402": "04406", "old_code": "98101", "postal_code": "9810103", "prefecture_kana": "ミヤギケン", "city_kana": "ミヤギグンリフチョウ", "neighborhood_kana": "モリゴウ", "prefecture": "宮城県", "city": "宮城郡利府町", "neighborhood": "森郷", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','宮城郡利府町','森郷');
 INSERT INTO postal_data VALUES('9810112','{"jisx0402": "04406", "old_code": "98101", "postal_code": "9810112", "prefecture_kana": "ミヤギケン", "city_kana": "ミヤギグンリフチョウ", "neighborhood_kana": "リフ", "prefecture": "宮城県", "city": "宮城郡利府町", "neighborhood": "利府", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','宮城郡利府町','利府');
 INSERT INTO postal_data VALUES('9813600','{"jisx0402": "04421", "old_code": "98136", "postal_code": "9813600", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "04424", "old_code": "98136", "postal_code": "9813600", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンオオヒラムラ", "neighborhood_kana": "", "prefecture": "宮城県", "city": "黒川郡大衡村", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}], "note": "以下に掲載がない場合"}','宮城県','黒川郡大和町','');
 INSERT INTO postal_data VALUES('9813404','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813404", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイアイカワ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合相川", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合相川');
 INSERT INTO postal_data VALUES('9813401','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813401", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイサンガウチ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合三ケ内", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合三ケ内');
 INSERT INTO postal_data VALUES('9813406','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813406", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイヒルブクロ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合蒜袋", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合蒜袋');
-INSERT INTO postal_data VALUES('9813403','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813403", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイヒワダ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合檜和田", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合檜和田');
+INSERT INTO postal_data VALUES('9813403','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813403", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイヒワダ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合桧和田", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合桧和田');
 INSERT INTO postal_data VALUES('9813402','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813402", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイホウオンジ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合報恩寺", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合報恩寺');
 INSERT INTO postal_data VALUES('9813405','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813405", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイマイノ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合舞野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合舞野');
 INSERT INTO postal_data VALUES('9813407','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813407", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オチアイマツサカ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "落合松坂", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','落合松坂');
 INSERT INTO postal_data VALUES('9813623','{"jisx0402": "04421", "old_code": "98136", "postal_code": "9813623", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "オノ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "小野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','小野');
 INSERT INTO postal_data VALUES('9813271','{"jisx0402": "04421", "old_code": "981  ", "postal_code": "9813271", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "ガクエン", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "学苑", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','学苑');
 INSERT INTO postal_data VALUES('9813414','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813414", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "ツルスオオタ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "鶴巣太田", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','鶴巣太田');
 INSERT INTO postal_data VALUES('9813411','{"jisx0402": "04421", "old_code": "98134", "postal_code": "9813411", "prefecture_kana": "ミヤギケン", "city_kana": "クロカワグンタイワチョウ", "neighborhood_kana": "ツルスオオダイラ", "prefecture": "宮城県", "city": "黒川郡大和町", "neighborhood": "鶴巣大平", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','宮城県','黒川郡大和町','鶴巣大平');
@@ -23316,15 +23316,15 @@
 INSERT INTO postal_data VALUES('3030022','{"jisx0402": "08211", "old_code": "303  ", "postal_code": "3030022", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ミツカイドウフチガシラマチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "水海道淵頭町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','水海道淵頭町');
 INSERT INTO postal_data VALUES('3030026','{"jisx0402": "08211", "old_code": "303  ", "postal_code": "3030026", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ミツカイドウホンチョウ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "水海道本町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','水海道本町');
 INSERT INTO postal_data VALUES('3030004','{"jisx0402": "08211", "old_code": "303  ", "postal_code": "3030004", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ミツカイドウモトマチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "水海道元町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','水海道元町');
 INSERT INTO postal_data VALUES('3030005','{"jisx0402": "08211", "old_code": "303  ", "postal_code": "3030005", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ミツカイドウモリシタマチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "水海道森下町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','水海道森下町');
 INSERT INTO postal_data VALUES('3030031','{"jisx0402": "08211", "old_code": "303  ", "postal_code": "3030031", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ミツカイドウヤマダマチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "水海道山田町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','水海道山田町');
 INSERT INTO postal_data VALUES('3030013','{"jisx0402": "08211", "old_code": "303  ", "postal_code": "3030013", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ミノワマチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "箕輪町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','箕輪町');
 INSERT INTO postal_data VALUES('3002742','{"jisx0402": "08211", "old_code": "30027", "postal_code": "3002742", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ムコウイシゲ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "向石下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','向石下');
-INSERT INTO postal_data VALUES('3002508','{"jisx0402": "08211", "old_code": "30025", "postal_code": "3002508", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ムスビマチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "むすびまち", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','むすびまち');
+INSERT INTO postal_data VALUES('3002508','{"jisx0402": "08211", "old_code": "30025", "postal_code": "3002508", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ムスビマチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "むすびまち", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','むすびまち');
 INSERT INTO postal_data VALUES('3002707','{"jisx0402": "08211", "old_code": "30027", "postal_code": "3002707", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "モトイシゲ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "本石下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','本石下');
 INSERT INTO postal_data VALUES('3002711','{"jisx0402": "08211", "old_code": "30027", "postal_code": "3002711", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "モトトヨダ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "本豊田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','本豊田');
 INSERT INTO postal_data VALUES('3002715','{"jisx0402": "08211", "old_code": "30027", "postal_code": "3002715", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ヤマグチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "山口", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','山口');
 INSERT INTO postal_data VALUES('3002522','{"jisx0402": "08211", "old_code": "30025", "postal_code": "3002522", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ヨコゾネシンデンマチ", "prefecture": "茨城県", "city": "常総市", "neighborhood": "横曽根新田町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','横曽根新田町');
 INSERT INTO postal_data VALUES('3002701','{"jisx0402": "08211", "old_code": "30027", "postal_code": "3002701", "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ワカミヤド", "prefecture": "茨城県", "city": "常総市", "neighborhood": "若宮戸", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常総市','若宮戸');
 INSERT INTO postal_data VALUES('3130000','{"jisx0402": "08212", "old_code": "313  ", "postal_code": "3130000", "prefecture_kana": "イバラキケン", "city_kana": "ヒタチオオタシ", "neighborhood_kana": "", "prefecture": "茨城県", "city": "常陸太田市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}','茨城県','常陸太田市','');
 INSERT INTO postal_data VALUES('3130102','{"jisx0402": "08212", "old_code": "31301", "postal_code": "3130102", "prefecture_kana": "イバラキケン", "city_kana": "ヒタチオオタシ", "neighborhood_kana": "アカヅチチョウ", "prefecture": "茨城県", "city": "常陸太田市", "neighborhood": "赤土町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','常陸太田市','赤土町');
@@ -39150,15 +39150,15 @@
 INSERT INTO postal_data VALUES('2060032','{"jisx0402": "13224", "old_code": "206  ", "postal_code": "2060032", "prefecture_kana": "トウキョウト", "city_kana": "タマシ", "neighborhood_kana": "ミナミノ", "prefecture": "東京都", "city": "多摩市", "neighborhood": "南野", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','多摩市','南野');
 INSERT INTO postal_data VALUES('2060004','{"jisx0402": "13224", "old_code": "206  ", "postal_code": "2060004", "prefecture_kana": "トウキョウト", "city_kana": "タマシ", "neighborhood_kana": "モグサ", "prefecture": "東京都", "city": "多摩市", "neighborhood": "百草", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','多摩市','百草');
 INSERT INTO postal_data VALUES('2060021','{"jisx0402": "13224", "old_code": "206  ", "postal_code": "2060021", "prefecture_kana": "トウキョウト", "city_kana": "タマシ", "neighborhood_kana": "レンコウジ", "prefecture": "東京都", "city": "多摩市", "neighborhood": "連光寺", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','多摩市','連光寺');
 INSERT INTO postal_data VALUES('2060001','{"jisx0402": "13224", "old_code": "206  ", "postal_code": "2060001", "prefecture_kana": "トウキョウト", "city_kana": "タマシ", "neighborhood_kana": "ワダ", "prefecture": "東京都", "city": "多摩市", "neighborhood": "和田", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','多摩市','和田');
 INSERT INTO postal_data VALUES('2060801','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060801", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "オオマル", "prefecture": "東京都", "city": "稲城市", "neighborhood": "大丸", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','大丸');
 INSERT INTO postal_data VALUES('2060811','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060811", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "オシタテ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "押立", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','押立');
 INSERT INTO postal_data VALUES('2060803','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060803", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "コウヨウダイ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "向陽台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','向陽台');
-INSERT INTO postal_data VALUES('2060822','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060822", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "サカハマ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "坂浜", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','坂浜');
+INSERT INTO postal_data VALUES('2060822','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060822", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "サカハマ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "坂浜", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','坂浜');
 INSERT INTO postal_data VALUES('2060821','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060821", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "ナガミネ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "長峰", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','長峰');
 INSERT INTO postal_data VALUES('2060802','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060802", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "ヒガシナガヌマ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "東長沼", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','東長沼');
 INSERT INTO postal_data VALUES('2060823','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060823", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "ヒラオ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "平尾", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','平尾');
 INSERT INTO postal_data VALUES('2060804','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060804", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "モムラ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "百村", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','百村');
 INSERT INTO postal_data VALUES('2060812','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060812", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "ヤノクチ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "矢野口", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','矢野口');
 INSERT INTO postal_data VALUES('2060824','{"jisx0402": "13225", "old_code": "206  ", "postal_code": "2060824", "prefecture_kana": "トウキョウト", "city_kana": "イナギシ", "neighborhood_kana": "ワカバダイ", "prefecture": "東京都", "city": "稲城市", "neighborhood": "若葉台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','東京都','稲城市','若葉台');
 INSERT INTO postal_data VALUES('2050000','{"jisx0402": "13227", "old_code": "205  ", "postal_code": "2050000", "prefecture_kana": "トウキョウト", "city_kana": "ハムラシ", "neighborhood_kana": "", "prefecture": "東京都", "city": "羽村市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}','東京都','羽村市','');
@@ -42086,14 +42086,15 @@
 INSERT INTO postal_data VALUES('9500131','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500131", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "フクロヅ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "袋津", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','袋津');
 INSERT INTO postal_data VALUES('9500202','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500202", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "フジヤマ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "藤山", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','藤山');
 INSERT INTO postal_data VALUES('9500153','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500153", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "フナトヤマ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "船戸山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','船戸山');
 INSERT INTO postal_data VALUES('9500328','{"jisx0402": "15104", "old_code": "95003", "postal_code": "9500328", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マイガタ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "舞潟", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','舞潟');
 INSERT INTO postal_data VALUES('9500112','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500112", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マツヤマ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "松山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','松山');
 INSERT INTO postal_data VALUES('9500146','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500146", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マルガタ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "丸潟", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','丸潟');
 INSERT INTO postal_data VALUES('9500115','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500115", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マルヤマ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "丸山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','丸山');
+INSERT INTO postal_data VALUES('9500117','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500117", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "マルヤマノウチゼンノジョウグミ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "丸山ノ内善之丞組", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','丸山ノ内善之丞組');
 INSERT INTO postal_data VALUES('9500114','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500114", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ミョウガダニ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "茗荷谷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','茗荷谷');
 INSERT INTO postal_data VALUES('9500143','{"jisx0402": "15104", "old_code": "95001", "postal_code": "9500143", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "モトマチ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "元町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','元町');
 INSERT INTO postal_data VALUES('9500204','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500204", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越');
 INSERT INTO postal_data VALUES('9500210','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500210", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシカミチョウ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越上町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越上町');
 INSERT INTO postal_data VALUES('9500211','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500211", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシカワネチョウ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越川根町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越川根町');
 INSERT INTO postal_data VALUES('9500208','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500208", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシチュウオウ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越中央", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越中央');
 INSERT INTO postal_data VALUES('9500209','{"jisx0402": "15104", "old_code": "95002", "postal_code": "9500209", "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシコウナンク", "neighborhood_kana": "ヨコゴシヒガシチョウ", "prefecture": "新潟県", "city": "新潟市江南区", "neighborhood": "横越東町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','新潟市江南区','横越東町');
@@ -46378,15 +46379,15 @@
 INSERT INTO postal_data VALUES('9460063','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460063", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "チュウカ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "中家", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460063", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "チュウカシンデン", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "中家新田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','新潟県','魚沼市','中家');
 INSERT INTO postal_data VALUES('9460065','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460065", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "チュウシザワ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "中子沢", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','中子沢');
 INSERT INTO postal_data VALUES('9460035','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460035", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "トオカマチ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "十日町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','十日町');
 INSERT INTO postal_data VALUES('9497418','{"jisx0402": "15225", "old_code": "94974", "postal_code": "9497418", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "トクダ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "徳田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','徳田');
 INSERT INTO postal_data VALUES('9460057','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460057", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナカジマ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "中島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','中島');
 INSERT INTO postal_data VALUES('9460058','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460058", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナカジマシンデン", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "中島新田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','中島新田');
 INSERT INTO postal_data VALUES('9460212','{"jisx0402": "15225", "old_code": "94602", "postal_code": "9460212", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナガトリ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "長鳥", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','長鳥');
-INSERT INTO postal_data VALUES('9460006','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460006", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナカノシマ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "中ノ島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','中ノ島');
+INSERT INTO postal_data VALUES('9460006','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460006", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナカノシマ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "中ノ島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','中ノ島');
 INSERT INTO postal_data VALUES('9460024','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460024", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナカハラ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "中原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','中原');
 INSERT INTO postal_data VALUES('9460053','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460053", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナガマツ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "長松", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','長松');
 INSERT INTO postal_data VALUES('9460071','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460071", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナノカイチ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "七日市", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','七日市');
 INSERT INTO postal_data VALUES('9460072','{"jisx0402": "15225", "old_code": "946  ", "postal_code": "9460072", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナノカイチシンデン", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "七日市新田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','七日市新田');
 INSERT INTO postal_data VALUES('9460111','{"jisx0402": "15225", "old_code": "94601", "postal_code": "9460111", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ナミヤナギ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "並柳", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','並柳');
 INSERT INTO postal_data VALUES('9460204','{"jisx0402": "15225", "old_code": "94602", "postal_code": "9460204", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ニシミョウ", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "西名", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','西名');
 INSERT INTO postal_data VALUES('9460206','{"jisx0402": "15225", "old_code": "94602", "postal_code": "9460206", "prefecture_kana": "ニイガタケン", "city_kana": "ウオヌマシ", "neighborhood_kana": "ニシミョウシンデン", "prefecture": "新潟県", "city": "魚沼市", "neighborhood": "西名新田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','新潟県','魚沼市','西名新田');
@@ -55880,16 +55881,16 @@
 INSERT INTO postal_data VALUES('3990039','{"jisx0402": "20202", "old_code": "399  ", "postal_code": "3990039", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "コヤキタ", "prefecture": "長野県", "city": "松本市", "neighborhood": "小屋北", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','小屋北');
 INSERT INTO postal_data VALUES('3990038','{"jisx0402": "20202", "old_code": "399  ", "postal_code": "3990038", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "コヤミナミ", "prefecture": "長野県", "city": "松本市", "neighborhood": "小屋南", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','小屋南');
 INSERT INTO postal_data VALUES('3990033','{"jisx0402": "20202", "old_code": "399  ", "postal_code": "3990033", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ササガ", "prefecture": "長野県", "city": "松本市", "neighborhood": "笹賀", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','笹賀');
 INSERT INTO postal_data VALUES('3900847','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900847", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ササベ", "prefecture": "長野県", "city": "松本市", "neighborhood": "笹部", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','笹部');
 INSERT INTO postal_data VALUES('3900221','{"jisx0402": "20202", "old_code": "39002", "postal_code": "3900221", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "サトヤマベ", "prefecture": "長野県", "city": "松本市", "neighborhood": "里山辺", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','里山辺');
 INSERT INTO postal_data VALUES('3900877','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900877", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "サワムラ", "prefecture": "長野県", "city": "松本市", "neighborhood": "沢村", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','沢村');
 INSERT INTO postal_data VALUES('3900301','{"jisx0402": "20202", "old_code": "39003", "postal_code": "3900301", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シナグラ", "prefecture": "長野県", "city": "松本市", "neighborhood": "稲倉", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','稲倉');
+INSERT INTO postal_data VALUES('3900851','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900851", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シマウチ", "prefecture": "長野県", "city": "松本市", "neighborhood": "島内", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "1〜9819、9822、9831〜9863番地"}','長野県','松本市','島内');
 INSERT INTO postal_data VALUES('3998251','{"jisx0402": "20202", "old_code": "39982", "postal_code": "3998251", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シマウチ", "prefecture": "長野県", "city": "松本市", "neighborhood": "島内", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "9820、9821、9823〜9830、9864番地以上"}','長野県','松本市','島内');
-INSERT INTO postal_data VALUES('3900851','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900851", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シマウチ", "prefecture": "長野県", "city": "松本市", "neighborhood": "島内", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "その他"}','長野県','松本市','島内');
 INSERT INTO postal_data VALUES('3900852','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900852", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シマダチ", "prefecture": "長野県", "city": "松本市", "neighborhood": "島立", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','島立');
 INSERT INTO postal_data VALUES('3900805','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900805", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シミズ", "prefecture": "長野県", "city": "松本市", "neighborhood": "清水", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','清水');
 INSERT INTO postal_data VALUES('3900875','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900875", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ジョウセイ", "prefecture": "長野県", "city": "松本市", "neighborhood": "城西", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','城西');
 INSERT INTO postal_data VALUES('3900807','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900807", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ジョウトウ", "prefecture": "長野県", "city": "松本市", "neighborhood": "城東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','城東');
 INSERT INTO postal_data VALUES('3900828','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900828", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ショウナイ", "prefecture": "長野県", "city": "松本市", "neighborhood": "庄内", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','庄内');
 INSERT INTO postal_data VALUES('3900866','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900866", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ジョウヤマ", "prefecture": "長野県", "city": "松本市", "neighborhood": "城山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','城山');
 INSERT INTO postal_data VALUES('3900863','{"jisx0402": "20202", "old_code": "390  ", "postal_code": "3900863", "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "シライタ", "prefecture": "長野県", "city": "松本市", "neighborhood": "白板", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','長野県','松本市','白板');
@@ -73973,15 +73974,15 @@
 INSERT INTO postal_data VALUES('5250054','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250054", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ヒガシヤグラ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "東矢倉", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','東矢倉');
 INSERT INTO postal_data VALUES('5250023','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250023", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ヒライ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "平井", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','平井');
 INSERT INTO postal_data VALUES('5250024','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250024", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ヒライチョウ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "平井町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','平井町');
 INSERT INTO postal_data VALUES('5250064','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250064", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ミクラチョウ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "御倉町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','御倉町');
 INSERT INTO postal_data VALUES('5250056','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250056", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ミナミガサチョウ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "南笠町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','南笠町');
 INSERT INTO postal_data VALUES('5250071','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250071", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ミナミガサヒガシ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "南笠東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','南笠東');
 INSERT INTO postal_data VALUES('5250050','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250050", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ミナミクサツ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "南草津", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','南草津');
-INSERT INTO postal_data VALUES('5250068','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250068", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ミナミクサツプリムタウン", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "南草津プリムタウン", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','南草津プリムタウン');
+INSERT INTO postal_data VALUES('5250068','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250068", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ミナミクサツプリムタウン", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "南草津プリムタウン", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','南草津プリムタウン');
 INSERT INTO postal_data VALUES('5250063','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250063", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ミナミヤマダチョウ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "南山田町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','南山田町');
 INSERT INTO postal_data VALUES('5250053','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250053", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ヤグラ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "矢倉", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','矢倉');
 INSERT INTO postal_data VALUES('5250066','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250066", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ヤバセチョウ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "矢橋町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','矢橋町');
 INSERT INTO postal_data VALUES('5250062','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250062", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ヤマダチョウ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "山田町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','山田町');
 INSERT INTO postal_data VALUES('5250042','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250042", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ヤマデラチョウ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "山寺町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','山寺町');
 INSERT INTO postal_data VALUES('5250045','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250045", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ワカクサ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "若草", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','若草');
 INSERT INTO postal_data VALUES('5250031','{"jisx0402": "25206", "old_code": "525  ", "postal_code": "5250031", "prefecture_kana": "シガケン", "city_kana": "クサツシ", "neighborhood_kana": "ワカタケチョウ", "prefecture": "滋賀県", "city": "草津市", "neighborhood": "若竹町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','草津市','若竹町');
@@ -80456,15 +80457,15 @@
 INSERT INTO postal_data VALUES('6100111','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100111", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "トノ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "富野", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','富野');
 INSERT INTO postal_data VALUES('6100113','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100113", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "ナカ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "中", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','中');
 INSERT INTO postal_data VALUES('6100112','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100112", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "ナガイケ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "長池", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','長池');
 INSERT INTO postal_data VALUES('6100116','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100116", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "ナシマ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "奈島", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','奈島');
 INSERT INTO postal_data VALUES('6100101','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100101", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "ヒラカワ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "平川", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','平川');
 INSERT INTO postal_data VALUES('6100117','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100117", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "ビワノショウ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "枇杷庄", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','枇杷庄');
 INSERT INTO postal_data VALUES('6100118','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100118", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "ミズシ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "水主", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','水主');
-INSERT INTO postal_data VALUES('6100119','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100119", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "レイリョウツムギ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "令涼つむぎ", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','令涼つむぎ');
+INSERT INTO postal_data VALUES('6100119','{"jisx0402": "26207", "old_code": "61001", "postal_code": "6100119", "prefecture_kana": "キョウトフ", "city_kana": "ジョウヨウシ", "neighborhood_kana": "レイリョウツムギ", "prefecture": "京都府", "city": "城陽市", "neighborhood": "令涼つむぎ", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','城陽市','令涼つむぎ');
 INSERT INTO postal_data VALUES('6170000','{"jisx0402": "26208", "old_code": "617  ", "postal_code": "6170000", "prefecture_kana": "キョウトフ", "city_kana": "ムコウシ", "neighborhood_kana": "", "prefecture": "京都府", "city": "向日市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "26209", "old_code": "617  ", "postal_code": "6170000", "prefecture_kana": "キョウトフ", "city_kana": "ナガオカキョウシ", "neighborhood_kana": "", "prefecture": "京都府", "city": "長岡京市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}], "note": "以下に掲載がない場合"}','京都府','向日市','');
 INSERT INTO postal_data VALUES('6170004','{"jisx0402": "26208", "old_code": "617  ", "postal_code": "6170004", "prefecture_kana": "キョウトフ", "city_kana": "ムコウシ", "neighborhood_kana": "カイデチョウ", "prefecture": "京都府", "city": "向日市", "neighborhood": "鶏冠井町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','向日市','鶏冠井町');
 INSERT INTO postal_data VALUES('6170006','{"jisx0402": "26208", "old_code": "617  ", "postal_code": "6170006", "prefecture_kana": "キョウトフ", "city_kana": "ムコウシ", "neighborhood_kana": "カミウエノチョウ", "prefecture": "京都府", "city": "向日市", "neighborhood": "上植野町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','向日市','上植野町');
 INSERT INTO postal_data VALUES('6170002','{"jisx0402": "26208", "old_code": "617  ", "postal_code": "6170002", "prefecture_kana": "キョウトフ", "city_kana": "ムコウシ", "neighborhood_kana": "テラドチョウ", "prefecture": "京都府", "city": "向日市", "neighborhood": "寺戸町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','向日市','寺戸町');
 INSERT INTO postal_data VALUES('6170005','{"jisx0402": "26208", "old_code": "617  ", "postal_code": "6170005", "prefecture_kana": "キョウトフ", "city_kana": "ムコウシ", "neighborhood_kana": "ムコウチョウ", "prefecture": "京都府", "city": "向日市", "neighborhood": "向日町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','向日市','向日町');
 INSERT INTO postal_data VALUES('6170001','{"jisx0402": "26208", "old_code": "617  ", "postal_code": "6170001", "prefecture_kana": "キョウトフ", "city_kana": "ムコウシ", "neighborhood_kana": "モズメチョウ", "prefecture": "京都府", "city": "向日市", "neighborhood": "物集女町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','向日市','物集女町');
 INSERT INTO postal_data VALUES('6170003','{"jisx0402": "26208", "old_code": "617  ", "postal_code": "6170003", "prefecture_kana": "キョウトフ", "city_kana": "ムコウシ", "neighborhood_kana": "モリモトチョウ", "prefecture": "京都府", "city": "向日市", "neighborhood": "森本町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','京都府','向日市','森本町');
@@ -85698,14 +85699,15 @@
 INSERT INTO postal_data VALUES('6550006','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550006", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ホンタモン", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "本多聞", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','本多聞');
 INSERT INTO postal_data VALUES('6550044','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550044", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マイコザカ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "舞子坂", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','舞子坂');
 INSERT INTO postal_data VALUES('6550046','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550046", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マイコダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "舞子台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','舞子台');
 INSERT INTO postal_data VALUES('6550051','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550051", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マイタモンニシ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "舞多聞西", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','舞多聞西');
 INSERT INTO postal_data VALUES('6550052','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550052", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マイタモンヒガシ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "舞多聞東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','舞多聞東');
 INSERT INTO postal_data VALUES('6550004','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550004", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "マナビガオカ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "学が丘", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','学が丘');
 INSERT INTO postal_data VALUES('6550025','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550025", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミズガオカ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "瑞ケ丘", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','瑞ケ丘');
+INSERT INTO postal_data VALUES('6550855','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550855", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミズキダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "みずき台", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "住居表示の実施", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','みずき台');
 INSERT INTO postal_data VALUES('6550022','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550022", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミズホドオリ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "瑞穂通", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','瑞穂通');
 INSERT INTO postal_data VALUES('6550043','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550043", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミナミタモンダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "南多聞台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','南多聞台');
 INSERT INTO postal_data VALUES('6550874','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550874", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミヤマダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "美山台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','美山台');
 INSERT INTO postal_data VALUES('6550028','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550028", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミヤモトチョウ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "宮本町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','宮本町');
 INSERT INTO postal_data VALUES('6550852','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550852", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ミョウダニチョウ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "名谷町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','名谷町');
 INSERT INTO postal_data VALUES('6550854','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550854", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "モモヤマダイ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "桃山台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','桃山台');
 INSERT INTO postal_data VALUES('6550891','{"jisx0402": "28108", "old_code": "655  ", "postal_code": "6550891", "prefecture_kana": "ヒョウゴケン", "city_kana": "コウベシタルミク", "neighborhood_kana": "ヤマテ", "prefecture": "兵庫県", "city": "神戸市垂水区", "neighborhood": "山手", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','兵庫県','神戸市垂水区','山手');
@@ -100838,15 +100840,15 @@
 INSERT INTO postal_data VALUES('7520903','{"jisx0402": "35201", "old_code": "752  ", "postal_code": "7520903", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カズミツチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "員光町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','員光町');
 INSERT INTO postal_data VALUES('7510884','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510884", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カタチヤマ", "prefecture": "山口県", "city": "下関市", "neighborhood": "形山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','形山');
 INSERT INTO postal_data VALUES('7510888','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510888", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カタチヤマチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "形山町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','形山町');
 INSERT INTO postal_data VALUES('7510885','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510885", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カタチヤマミドリマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "形山みどり町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','形山みどり町');
 INSERT INTO postal_data VALUES('7500061','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500061", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カミシンチチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "上新地町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','上新地町');
 INSERT INTO postal_data VALUES('7500009','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500009", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カミタナカマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "上田中町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','上田中町');
 INSERT INTO postal_data VALUES('7520925','{"jisx0402": "35201", "old_code": "752  ", "postal_code": "7520925", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カメハマチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "亀浜町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','亀浜町');
-INSERT INTO postal_data VALUES('7596602','{"jisx0402": "35201", "old_code": "75966", "postal_code": "7596602", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カモウノ", "prefecture": "山口県", "city": "下関市", "neighborhood": "蒲生野", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','蒲生野');
+INSERT INTO postal_data VALUES('7596602','{"jisx0402": "35201", "old_code": "75966", "postal_code": "7596602", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カモノ", "prefecture": "山口県", "city": "下関市", "neighborhood": "蒲生野", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','山口県','下関市','蒲生野');
 INSERT INTO postal_data VALUES('7500005','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500005", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カラトチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "唐戸町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','唐戸町');
 INSERT INTO postal_data VALUES('7510859','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510859", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カワナカホンマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "川中本町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','川中本町');
 INSERT INTO postal_data VALUES('7510853','{"jisx0402": "35201", "old_code": "751  ", "postal_code": "7510853", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カワナカユタカマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "川中豊町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','川中豊町');
 INSERT INTO postal_data VALUES('7500032','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500032", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カンセイチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "関西町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','関西町');
 INSERT INTO postal_data VALUES('7500022','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500022", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カンセイホンマチ", "prefecture": "山口県", "city": "下関市", "neighborhood": "関西本町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','関西本町');
 INSERT INTO postal_data VALUES('7520907','{"jisx0402": "35201", "old_code": "752  ", "postal_code": "7520907", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カンダ", "prefecture": "山口県", "city": "下関市", "neighborhood": "神田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','神田');
 INSERT INTO postal_data VALUES('7500044','{"jisx0402": "35201", "old_code": "750  ", "postal_code": "7500044", "prefecture_kana": "ヤマグチケン", "city_kana": "シモノセキシ", "neighborhood_kana": "カンダチョウ", "prefecture": "山口県", "city": "下関市", "neighborhood": "神田町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','山口県','下関市','神田町');
@@ -119707,29 +119709,29 @@
 INSERT INTO postal_data VALUES('9000031','{"jisx0402": "47201", "old_code": "900  ", "postal_code": "9000031", "prefecture_kana": "オキナワケン", "city_kana": "ナハシ", "neighborhood_kana": "ワカサ", "prefecture": "沖縄県", "city": "那覇市", "neighborhood": "若狭", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','那覇市','若狭');
 INSERT INTO postal_data VALUES('9012200','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012200", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}','沖縄県','宜野湾市','');
 INSERT INTO postal_data VALUES('9012206','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012206", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "アイチ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "愛知", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','愛知');
 INSERT INTO postal_data VALUES('9012205','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012205", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "アカミチ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "赤道", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','赤道');
 INSERT INTO postal_data VALUES('9012201','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012201", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "アラグスク", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "新城", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','新城');
 INSERT INTO postal_data VALUES('9012221','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012221", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "イサ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "伊佐", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','伊佐');
 INSERT INTO postal_data VALUES('9012204','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012204", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "ウエハラ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "上原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','上原');
-INSERT INTO postal_data VALUES('9012227','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012227", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "ウチドマリ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "宇地泊", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "住居表示の実施", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','宇地泊');
-INSERT INTO postal_data VALUES('9012225','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012225", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "オオジャナ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "大謝名", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','大謝名');
+INSERT INTO postal_data VALUES('9012227','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012227", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "ウチドマリ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "宇地泊", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','宇地泊');
+INSERT INTO postal_data VALUES('9012225','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012225", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "オオジャナ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "大謝名", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','大謝名');
 INSERT INTO postal_data VALUES('9012223','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012223", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "オオヤマ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "大山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','大山');
 INSERT INTO postal_data VALUES('9012226','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012226", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "カカズ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "嘉数", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','嘉数');
 INSERT INTO postal_data VALUES('9012214','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012214", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "ガネコ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "我如古", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','我如古');
 INSERT INTO postal_data VALUES('9012207','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012207", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "カミヤマ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "神山", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','神山');
 INSERT INTO postal_data VALUES('9012211','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012211", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "ギノワン", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "宜野湾", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','宜野湾');
 INSERT INTO postal_data VALUES('9012222','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012222", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "キユウナ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "喜友名", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','喜友名');
 INSERT INTO postal_data VALUES('9012216','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012216", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "サマシタ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "佐真下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','佐真下');
 INSERT INTO postal_data VALUES('9012213','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012213", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "シマシ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "志真志", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','志真志');
 INSERT INTO postal_data VALUES('9012212','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012212", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "ナガタ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "長田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','長田');
 INSERT INTO postal_data VALUES('9012203','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012203", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "ノダケ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "野嵩", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','野嵩');
 INSERT INTO postal_data VALUES('9012202','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012202", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "フテンマ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "普天間", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','普天間');
 INSERT INTO postal_data VALUES('9012215','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012215", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "マエハラ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "真栄原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','真栄原');
-INSERT INTO postal_data VALUES('9012224','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012224", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "マシキ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "真志喜", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "住居表示の実施", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','真志喜');
+INSERT INTO postal_data VALUES('9012224','{"jisx0402": "47205", "old_code": "90122", "postal_code": "9012224", "prefecture_kana": "オキナワケン", "city_kana": "ギノワンシ", "neighborhood_kana": "マシキ", "prefecture": "沖縄県", "city": "宜野湾市", "neighborhood": "真志喜", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','宜野湾市','真志喜');
 INSERT INTO postal_data VALUES('9070000','{"jisx0402": "47207", "old_code": "907  ", "postal_code": "9070000", "prefecture_kana": "オキナワケン", "city_kana": "イシガキシ", "neighborhood_kana": "", "prefecture": "沖縄県", "city": "石垣市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "47381", "old_code": "907  ", "postal_code": "9070000", "prefecture_kana": "オキナワケン", "city_kana": "ヤエヤマグンタケトミチョウ", "neighborhood_kana": "", "prefecture": "沖縄県", "city": "八重山郡竹富町", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}], "note": "以下に掲載がない場合"}','沖縄県','石垣市','');
 INSERT INTO postal_data VALUES('9070024','{"jisx0402": "47207", "old_code": "907  ", "postal_code": "9070024", "prefecture_kana": "オキナワケン", "city_kana": "イシガキシ", "neighborhood_kana": "アラカワ", "prefecture": "沖縄県", "city": "石垣市", "neighborhood": "新川", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','石垣市','新川');
 INSERT INTO postal_data VALUES('9070023','{"jisx0402": "47207", "old_code": "907  ", "postal_code": "9070023", "prefecture_kana": "オキナワケン", "city_kana": "イシガキシ", "neighborhood_kana": "イシガキ", "prefecture": "沖縄県", "city": "石垣市", "neighborhood": "石垣", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','石垣市','石垣');
 INSERT INTO postal_data VALUES('9070332','{"jisx0402": "47207", "old_code": "90703", "postal_code": "9070332", "prefecture_kana": "オキナワケン", "city_kana": "イシガキシ", "neighborhood_kana": "イバルマ", "prefecture": "沖縄県", "city": "石垣市", "neighborhood": "伊原間", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','石垣市','伊原間');
 INSERT INTO postal_data VALUES('9070022','{"jisx0402": "47207", "old_code": "907  ", "postal_code": "9070022", "prefecture_kana": "オキナワケン", "city_kana": "イシガキシ", "neighborhood_kana": "オオカワ", "prefecture": "沖縄県", "city": "石垣市", "neighborhood": "大川", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','石垣市','大川');
 INSERT INTO postal_data VALUES('9070001','{"jisx0402": "47207", "old_code": "907  ", "postal_code": "9070001", "prefecture_kana": "オキナワケン", "city_kana": "イシガキシ", "neighborhood_kana": "オオハマ", "prefecture": "沖縄県", "city": "石垣市", "neighborhood": "大浜", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','石垣市','大浜');
 INSERT INTO postal_data VALUES('9070453','{"jisx0402": "47207", "old_code": "90704", "postal_code": "9070453", "prefecture_kana": "オキナワケン", "city_kana": "イシガキシ", "neighborhood_kana": "カビラ", "prefecture": "沖縄県", "city": "石垣市", "neighborhood": "川平", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','沖縄県','石垣市','川平');
@@ -120985,25 +120987,25 @@
 INSERT INTO office_data VALUES('0788502','{"jis": "01204", "kana": "アサヒカワチホウホウムキヨク", "name": "旭川地方法務局", "prefecture": "北海道", "city": "旭川市", "neighborhood": "宮前１条", "banchi": "3丁目3-15", "postal_code": "0788502", "old_code": "078  ", "post_office": "旭川東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "アサヒカワシ", "neighborhood_kana": "ミヤマエ１ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0788504','{"jis": "01204", "kana": "アサヒカワナカゼイムシヨ", "name": "旭川中税務署", "prefecture": "北海道", "city": "旭川市", "neighborhood": "宮前１条", "banchi": "3丁目3-15", "postal_code": "0788504", "old_code": "078  ", "post_office": "旭川東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "アサヒカワシ", "neighborhood_kana": "ミヤマエ１ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0788505','{"jis": "01204", "kana": "アサヒカワロウドウキジユンカントクシヨ", "name": "旭川労働基準監督署", "prefecture": "北海道", "city": "旭川市", "neighborhood": "宮前１条", "banchi": "3丁目3-15", "postal_code": "0788505", "old_code": "078  ", "post_office": "旭川東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "アサヒカワシ", "neighborhood_kana": "ミヤマエ１ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0788507','{"jis": "01204", "kana": "サツポロコクゼイキヨクギヨウムセンタ- アサヒカワブンシツ", "name": "札幌国税局業務センター　旭川分室", "prefecture": "北海道", "city": "旭川市", "neighborhood": "宮前一条", "banchi": "3丁目3番15号(旭川合同庁舎)", "postal_code": "0788507", "old_code": "078  ", "post_office": "旭川東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0788555','{"jis": "01204", "kana": "チユウシヨウキギヨウダイガクコウアサヒカワコウ", "name": "中小企業大学校旭川校", "prefecture": "北海道", "city": "旭川市", "neighborhood": "緑が丘東三条", "banchi": "2丁目2番1号", "postal_code": "0788555", "old_code": "078  ", "post_office": "旭川東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0788506','{"jis": "01204", "kana": "ノウリンスイサンシヨウ ホツカイドウノウセイジムシヨ アサヒカワチイキキヨテン", "name": "農林水産省　北海道農政事務所　旭川地域拠点", "prefecture": "北海道", "city": "旭川市", "neighborhood": "宮前１条", "banchi": "3丁目3-15", "postal_code": "0788506", "old_code": "078  ", "post_office": "旭川東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "アサヒカワシ", "neighborhood_kana": "ミヤマエ１ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0788511','{"jis": "01204", "kana": "ホツカイドウケイサツアサヒカワホウメンホンブ", "name": "北海道警察旭川方面本部", "prefecture": "北海道", "city": "旭川市", "neighborhood": "一条通", "banchi": "25丁目", "postal_code": "0788511", "old_code": "078  ", "post_office": "旭川東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0798501','{"jis": "01204", "kana": "アサヒカワシリツダイガク・アサヒカワシリツダイガクタンキダイガクブ", "name": "旭川市立大学・旭川市立大学短期大学部", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山三条", "banchi": "23丁目1番9番", "postal_code": "0798501", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('0798501','{"jis": "01204", "kana": "アサヒカワシリツダイガク・アサヒカワシリツダイガクタンキダイガクブ", "name": "旭川市立大学・旭川市立大学短期大学部", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山三条", "banchi": "23丁目1番9番", "postal_code": "0798501", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798509','{"jis": "01204", "kana": "カブシキカイシヤ カンデイハウス", "name": "株式会社　カンディハウス", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山北二条", "banchi": "6丁目", "postal_code": "0798509", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798511','{"jis": "01204", "kana": "カブシキカイシヤ ナカノメイボクテン", "name": "株式会社　中野銘木店", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山北一条", "banchi": "8丁目37-1", "postal_code": "0798511", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798652','{"jis": "01204", "kana": "カブシキガイシヤ イチジルシ アサヒカワサカナオロシウリシジヨウ", "name": "株式会社　一印　旭川魚卸売市場", "prefecture": "北海道", "city": "旭川市", "neighborhood": "流通団地一条", "banchi": "3丁目(永山郵便局私書箱第3号)", "postal_code": "0798652", "old_code": "079  ", "post_office": "永山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798555','{"jis": "01204", "kana": "カブシキガイシヤ コハタ", "name": "株式会社　コハタ", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山二条", "banchi": "3丁目2-16", "postal_code": "0798555", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798507','{"jis": "01204", "kana": "カブシキガイシヤ スハラシヨクヒン", "name": "株式会社　スハラ食品", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山十条", "banchi": "2丁目", "postal_code": "0798507", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798503','{"jis": "01204", "kana": "カブシキガイシヤ トワニ アサヒカワテン", "name": "株式会社　トワニ　旭川店", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山一条", "banchi": "3丁目", "postal_code": "0798503", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798585','{"jis": "01204", "kana": "カブシキガイシヤ フジ", "name": "株式会社　ふじ", "prefecture": "北海道", "city": "旭川市", "neighborhood": "流通団地一条", "banchi": "1丁目33番地の1", "postal_code": "0798585", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798513','{"jis": "01204", "kana": "カブシキガイシヤ ホクヤク アサヒカワシテン", "name": "株式会社　ほくやく　旭川支店", "prefecture": "北海道", "city": "旭川市", "neighborhood": "秋月二条", "banchi": "2丁目5番22号", "postal_code": "0798513", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798656','{"jis": "01204", "kana": "カブシキガイシヤ ホクレンユキサ-ビス アサヒカワシテン", "name": "（株）　ホクレン油機サービス　旭川支店", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山二条", "banchi": "13丁目1番28号(永山郵便局私書箱第6号)", "postal_code": "0798656", "old_code": "079  ", "post_office": "永山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0798505','{"jis": "01204", "kana": "ガツコウホウジン アサヒカワシホウガクイン・アサヒカワシホウコウトウガツコウ", "name": "学校法人　旭川志峯学院・旭川志峯高等学校", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山七条", "banchi": "16丁目3番16号", "postal_code": "0798505", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('0798505','{"jis": "01204", "kana": "ガツコウホウジン アサヒカワシホウガクイン・アサヒカワシホウコウトウガツコウ", "name": "学校法人　旭川志峯学院・旭川志峯高等学校", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山七条", "banchi": "16丁目3番16号", "postal_code": "0798505", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798516','{"jis": "01204", "kana": "ジヤパンケンザイ カブシキガイシヤ アサヒカワエイギヨウシヨ", "name": "ジャパン建材　（株）　旭川営業所", "prefecture": "北海道", "city": "旭川市", "neighborhood": "流通団地三条", "banchi": "5丁目", "postal_code": "0798516", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798550','{"jis": "01204", "kana": "ネツツトヨタタイセツ カブシキガイシヤ", "name": "ネッツトヨタたいせつ　株式会社", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山三条", "banchi": "12丁目", "postal_code": "0798550", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798508','{"jis": "01204", "kana": "ホツカイドウアサヒカワエイリヨウコウトウガツコウ", "name": "北海道旭川永嶺高等学校", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山町", "banchi": "3丁目102番地", "postal_code": "0798508", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "アサヒカワシ", "neighborhood_kana": "ナガヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0798610','{"jis": "01204", "kana": "ホツカイドウカミカワソウゴウシンコウキヨク", "name": "北海道上川総合振興局", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山六条", "banchi": "19丁目1-1", "postal_code": "0798610", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798613','{"jis": "01204", "kana": "ホツカイドウカミカワソウゴウシンコウキヨク アサヒカワケンセツカンリブ", "name": "北海道上川総合振興局　旭川建設管理部", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山六条", "banchi": "19丁目1-1", "postal_code": "0798613", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798611','{"jis": "01204", "kana": "ホツカイドウカミカワホケンジヨ", "name": "北海道上川保健所", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山六条", "banchi": "19丁目", "postal_code": "0798611", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0798612','{"jis": "01204", "kana": "ホツカイドウキヨウイクチヨウ カミカワキヨウイクキヨク", "name": "北海道教育庁　上川教育局", "prefecture": "北海道", "city": "旭川市", "neighborhood": "永山六条", "banchi": "19丁目", "postal_code": "0798612", "old_code": "079  ", "post_office": "永山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -121866,18 +121868,17 @@
 INSERT INTO office_data VALUES('0392286','{"jis": "02412", "kana": "ニホンフ-ドパツカ- カブシキガイシヤ アオモリコウジヨウ", "name": "日本フードパッカー　株式会社　青森工場", "prefecture": "青森県", "city": "上北郡おいらせ町", "neighborhood": "松原", "banchi": "2丁目132-1", "postal_code": "0392286", "old_code": "03922", "post_office": "百石", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "カミキタグンオイラセチョウ", "neighborhood_kana": "マツバラ", "alternates": []}');
 INSERT INTO office_data VALUES('0392293','{"jis": "02412", "kana": "モモカワ カブシキガイシヤ", "name": "桃川　株式会社", "prefecture": "青森県", "city": "上北郡おいらせ町", "neighborhood": "上明堂", "banchi": "112", "postal_code": "0392293", "old_code": "03922", "post_office": "百石", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "カミキタグンオイラセチョウ", "neighborhood_kana": "カミアケドウ", "alternates": []}');
 INSERT INTO office_data VALUES('0394692','{"jis": "02423", "kana": "オオママチヤクバ", "name": "大間町役場", "prefecture": "青森県", "city": "下北郡大間町", "neighborhood": "大字大間", "banchi": "字大間104番地", "postal_code": "0394692", "old_code": "03946", "post_office": "大間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0394293','{"jis": "02424", "kana": "トウホクデンリヨク カブシキガイシヤ ヒガシドオリゲンシリヨクハツデンシヨ", "name": "東北電力　株式会社　東通原子力発電所", "prefecture": "青森県", "city": "下北郡東通村", "neighborhood": "大字白糠", "banchi": "字前坂下34-4", "postal_code": "0394293", "old_code": "03942", "post_office": "白糠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0394292','{"jis": "02424", "kana": "ヒガシドオリムラヤクバ", "name": "東通村役場", "prefecture": "青森県", "city": "下北郡東通村", "neighborhood": "大字砂子又", "banchi": "字沢内5番地34", "postal_code": "0394292", "old_code": "03942", "post_office": "白糠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0390198','{"jis": "02441", "kana": "サンノヘマチヤクバ", "name": "三戸町役場", "prefecture": "青森県", "city": "三戸郡三戸町", "neighborhood": "大字在府小路町", "banchi": "43", "postal_code": "0390198", "old_code": "03901", "post_office": "三戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0390292','{"jis": "02443", "kana": "タツコマチヤクバ", "name": "田子町役場", "prefecture": "青森県", "city": "三戸郡田子町", "neighborhood": "大字田子", "banchi": "字天神堂平81", "postal_code": "0390292", "old_code": "03902", "post_office": "田子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0390195','{"jis": "02445", "kana": "ナンブチヨウヤクバ ナンブブンチヨウシヤ", "name": "南部町役場　南部分庁舎", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字沖田面", "banchi": "字沖中46", "postal_code": "0390195", "old_code": "03901", "post_office": "三戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0390595','{"jis": "02445", "kana": "ナンブチヨウヤクバ ナガワブンチヨウシヤ", "name": "南部町役場　名川分庁舎", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字平", "banchi": "字広場22", "postal_code": "0390595", "old_code": "03905", "post_office": "上名久井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0390592','{"jis": "02445", "kana": "ナンブチヨウヤクバ ホンチヨウシヤ", "name": "南部町役場　本庁舎", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字平", "banchi": "字広場28番地1", "postal_code": "0390592", "old_code": "03905", "post_office": "上名久井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0390892','{"jis": "02445", "kana": "ナンブチヨウヤクバ", "name": "南部町役場", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字苫米地", "banchi": "字下宿23-1", "postal_code": "0390892", "old_code": "03908", "post_office": "福地", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('0390195','{"jis": "02445", "kana": "ナンブシシヨ", "name": "南部支所", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字沖田面", "banchi": "字沖中46", "postal_code": "0390195", "old_code": "03901", "post_office": "三戸", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('0390592','{"jis": "02445", "kana": "ナンブチヨウヤクバ", "name": "南部町役場", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字平", "banchi": "字広場28番地1", "postal_code": "0390592", "old_code": "03905", "post_office": "上名久井", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('0390892','{"jis": "02445", "kana": "フクチシシヨ", "name": "福地支所", "prefecture": "青森県", "city": "三戸郡南部町", "neighborhood": "大字苫米地", "banchi": "字下宿23-1", "postal_code": "0390892", "old_code": "03908", "post_office": "福地", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0208584','{"jis": "03201", "kana": "イツパンシヤダンホウジン イワテケンイシカイ", "name": "一般社団法人　岩手県医師会", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "菜園", "banchi": "2丁目8番20号", "postal_code": "0208584", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "サイエン", "alternates": []}');
 INSERT INTO office_data VALUES('0208505','{"jis": "03201", "kana": "イワテイカダイガクフゾク ウチマルメデイカルセンタ-", "name": "岩手医科大学附属　内丸メディカルセンター", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "内丸", "banchi": "19番1号", "postal_code": "0208505", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "ウチマル", "alternates": []}');
 INSERT INTO office_data VALUES('0208540','{"jis": "03201", "kana": "イワテケン ケイサツホンブ", "name": "岩手県　警察本部", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "内丸", "banchi": "8-10", "postal_code": "0208540", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "ウチマル", "alternates": []}');
 INSERT INTO office_data VALUES('0208577','{"jis": "03201", "kana": "イワテケンエイセイケンキユウジヨ", "name": "岩手県衛生研究所", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "飯岡新田", "banchi": "1丁目36-1", "postal_code": "0208577", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "イイオカシンデン", "alternates": []}');
 INSERT INTO office_data VALUES('0208510','{"jis": "03201", "kana": "イワテケンジチカイカン", "name": "岩手県自治会館", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "山王町", "banchi": "4-1", "postal_code": "0208510", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "サンノウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0208543','{"jis": "03201", "kana": "イワテケンリツ トリヨウコウトウガツコウ", "name": "岩手県立　杜陵高等学校", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "上田", "banchi": "2丁目3-1", "postal_code": "0208543", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "ウエダ", "alternates": []}');
 INSERT INTO office_data VALUES('0208515','{"jis": "03201", "kana": "イワテケンリツ モリオカダイイチコウトウガツコウ", "name": "岩手県立　盛岡第一高等学校", "prefecture": "岩手県", "city": "盛岡市", "neighborhood": "上田", "banchi": "3丁目2-1", "postal_code": "0208515", "old_code": "020  ", "post_office": "盛岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イワテケン", "city_kana": "モリオカシ", "neighborhood_kana": "ウエダ", "alternates": []}');
@@ -122394,15 +122395,15 @@
 INSERT INTO office_data VALUES('9894792','{"jis": "04212", "kana": "トメシ イシコシソウゴウシシヨ", "name": "登米市　石越総合支所", "prefecture": "宮城県", "city": "登米市", "neighborhood": "石越町", "banchi": "字愛宕81", "postal_code": "9894792", "old_code": "98947", "post_office": "石越", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9872195','{"jis": "04213", "kana": "イトウハムデイリ- カブシキガイシヤ", "name": "伊藤ハムディリー　株式会社", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "高清水来光沢", "banchi": "20", "postal_code": "9872195", "old_code": "98721", "post_office": "高清水", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "タカシミズライコウザワ", "alternates": []}');
 INSERT INTO office_data VALUES('9872293','{"jis": "04213", "kana": "クリハラシヤクシヨ", "name": "栗原市役所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館薬師", "banchi": "1丁目7-1", "postal_code": "9872293", "old_code": "98722", "post_office": "築館", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテヤクシ", "alternates": []}');
 INSERT INTO office_data VALUES('9872292','{"jis": "04213", "kana": "ツキダテゼイムシヨ", "name": "築館税務署", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "築館伊豆", "banchi": "3丁目1番10号", "postal_code": "9872292", "old_code": "98722", "post_office": "築館", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ツキダテイズ", "alternates": []}');
 INSERT INTO office_data VALUES('9872392','{"jis": "04213", "kana": "クリハラシ イチハサマソウゴウシシヨ", "name": "栗原市　一迫総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "一迫真坂", "banchi": "字清水田河前5", "postal_code": "9872392", "old_code": "98723", "post_office": "一迫", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "イチハサママサカ", "alternates": []}');
 INSERT INTO office_data VALUES('9872592','{"jis": "04213", "kana": "クリハラシヤクシヨ ハナヤマソウゴウシシヨ", "name": "栗原市役所　花山総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "花山本沢北ノ前", "banchi": "77", "postal_code": "9872592", "old_code": "98725", "post_office": "花山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9872593','{"jis": "04213", "kana": "コクリツ ハナヤマセイシヨウネンシゼンノイエ", "name": "国立　花山青少年自然の家", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "花山", "banchi": "字本沢沼山61-1", "postal_code": "9872593", "old_code": "98725", "post_office": "花山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9894592','{"jis": "04213", "kana": "クリハラシ セミネソウゴウシシヨ", "name": "栗原市　瀬峰総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "瀬峰", "banchi": "下藤沢118-1", "postal_code": "9894592", "old_code": "98945", "post_office": "高清水", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9894592','{"jis": "04213", "kana": "クリハラシ セミネソウゴウシシヨ", "name": "栗原市　瀬峰総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "瀬峰", "banchi": "長者原37番地2", "postal_code": "9894592", "old_code": "98945", "post_office": "高清水", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9895392','{"jis": "04213", "kana": "クリハラシ クリコマソウゴウシシヨ", "name": "栗原市　栗駒総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "栗駒岩ケ崎", "banchi": "円鏡寺後155", "postal_code": "9895392", "old_code": "98953", "post_office": "栗駒", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "クリコマイワガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('9895492','{"jis": "04213", "kana": "クリハラシヤクシヨ ウグイスザワソウゴウシシヨ", "name": "栗原市役所　鶯沢総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "鶯沢", "banchi": "南郷辻前74-1", "postal_code": "9895492", "old_code": "98954", "post_office": "鴬沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9895592','{"jis": "04213", "kana": "クリハラシ ワカヤナギソウゴウシシヨ", "name": "栗原市　若柳総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "若柳川南", "banchi": "戸ノ西4", "postal_code": "9895592", "old_code": "98955", "post_office": "若柳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "ワカヤナギカワミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('9895693','{"jis": "04213", "kana": "クリツコノウギヨウキヨウドウクミアイ", "name": "栗っこ農業協同組合", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "志波姫堀口", "banchi": "見渡2-1", "postal_code": "9895693", "old_code": "98956", "post_office": "志波姫", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "シワヒメホリグチ", "alternates": []}');
 INSERT INTO office_data VALUES('9895692','{"jis": "04213", "kana": "クリハラシ シワヒメソウゴウシシヨ", "name": "栗原市　志波姫総合支所", "prefecture": "宮城県", "city": "栗原市", "neighborhood": "志波姫沼崎", "banchi": "堰畑143", "postal_code": "9895692", "old_code": "98956", "post_office": "志波姫", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "クリハラシ", "neighborhood_kana": "シワヒメヌマザキ", "alternates": []}');
 INSERT INTO office_data VALUES('9810394','{"jis": "04214", "kana": "サメガウラスイヨウビユウビンキヨク", "name": "鮫ヶ浦水曜日郵便局", "prefecture": "宮城県", "city": "東松島市", "neighborhood": "宮戸字観音山", "banchi": "5番地", "postal_code": "9810394", "old_code": "98104", "post_office": "鳴瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9871395','{"jis": "04215", "kana": "オオサキシ マツヤマソウゴウシシヨ", "name": "大崎市　松山総合支所", "prefecture": "宮城県", "city": "大崎市", "neighborhood": "松山千石", "banchi": "字広田30", "postal_code": "9871395", "old_code": "98713", "post_office": "鹿島台", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤギケン", "city_kana": "オオサキシ", "neighborhood_kana": "マツヤマセンゴク", "alternates": []}');
@@ -122912,14 +122913,15 @@
 INSERT INTO office_data VALUES('9638670','{"jis": "07203", "kana": "タカラカセイキキ カブシキガイシヤ", "name": "宝化成機器　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "喜久田町卸", "banchi": "1丁目62-1(郡山卸町郵便局私書箱第355号)", "postal_code": "9638670", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "キクタマチオロシ", "alternates": []}');
 INSERT INTO office_data VALUES('9638661','{"jis": "07203", "kana": "ダイワシヨウケン カブシキガイシヤ コオリヤマシテン", "name": "大和証券　株式会社　郡山支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "10-10(郡山中町郵便局私書箱第603号)", "postal_code": "9638661", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638570','{"jis": "07203", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ フクシマシテン", "name": "東京海上日動火災保険　株式会社　福島支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "長者", "banchi": "1丁目7-20", "postal_code": "9638570", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "チョウジャ", "alternates": []}');
 INSERT INTO office_data VALUES('9638506','{"jis": "07203", "kana": "トウジルシコオリヤマセイカ カブシキガイシヤ", "name": "東印郡山青果　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富久山町久保田", "banchi": "字太郎殿前193", "postal_code": "9638506", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "フクヤママチクボタ", "alternates": []}');
 INSERT INTO office_data VALUES('9638676','{"jis": "07203", "kana": "トウホクアルフレツサ カブシキガイシヤ", "name": "東北アルフレッサ　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "喜久田町卸", "banchi": "1丁目46-1(郡山卸町郵便局私書箱第357号)", "postal_code": "9638676", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "キクタマチオロシ", "alternates": []}');
 INSERT INTO office_data VALUES('9638575','{"jis": "07203", "kana": "トウホクデンリヨク カブシキガイシヤ コオリヤマエイギヨウシヨ", "name": "東北電力　株式会社　郡山営業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "細沼町", "banchi": "1-5", "postal_code": "9638575", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ホソヌママチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638551','{"jis": "07203", "kana": "ニツポンホウソウキヨウカイ フクシマホウソウキヨク コオリヤマシキヨク", "name": "日本放送協会　福島放送局　郡山支局", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目5-21", "postal_code": "9638551", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": []}');
+INSERT INTO office_data VALUES('9638637','{"jis": "07203", "kana": "ニデツクプレシジヨン カブシキガイシヤ コオリヤマジギヨウシヨ", "name": "ニデックプレシジョン　株式会社　郡山事業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字諏訪内37(郡山郵便局私書箱第37号)", "postal_code": "9638637", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": true, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638580','{"jis": "07203", "kana": "ニホンセイメイホケン ソウゴガイシヤ コオリヤマシシヤ", "name": "日本生命保険　相互会社　郡山支社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "駅前", "banchi": "2丁目12-2", "postal_code": "9638580", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "エキマエ", "alternates": []}');
 INSERT INTO office_data VALUES('9638508','{"jis": "07203", "kana": "ニホンタバコサンギヨウ カブシキガイシヤ コオリヤマコウジヨウ", "name": "日本たばこ産業　株式会社　郡山工場", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字外河原", "banchi": "8-1", "postal_code": "9638508", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638556','{"jis": "07203", "kana": "パナソニツク インダストリ- カブシキガイシヤ コオリヤマジギヨウシヨ", "name": "パナソニック　インダストリー　株式会社　郡山事業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字石塚", "banchi": "111番地", "postal_code": "9638556", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638540','{"jis": "07203", "kana": "フクシマケンキヨウイクチヨウケンチユウキヨウイクジムシヨ", "name": "福島県教育庁県中教育事務所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目1番1号", "postal_code": "9638540", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": [{"jis": "07203", "kana": "フクシマケンケンチユウチホウシンコウキヨク", "name": "福島県県中地方振興局", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目1番1号", "postal_code": "9638540", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": []}]}');
 INSERT INTO office_data VALUES('9638668','{"jis": "07203", "kana": "フクシマケンシヨウコウシンヨウクミアイ", "name": "福島県商工信用組合", "prefecture": "福島県", "city": "郡山市", "neighborhood": "堂前町", "banchi": "7-7(郡山中町郵便局私書箱第616号)", "postal_code": "9638668", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ドウマエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638502','{"jis": "07203", "kana": "フクシマサクラノウギヨウキヨウドウクミアイ", "name": "福島さくら農業協同組合", "prefecture": "福島県", "city": "郡山市", "neighborhood": "朝日", "banchi": "2丁目14-7", "postal_code": "9638502", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アサヒ", "alternates": []}');
 INSERT INTO office_data VALUES('9638664','{"jis": "07203", "kana": "フクシマシンヨウハンバイ カブシキガイシヤ", "name": "福島信用販売　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "14-26(郡山中町郵便局私書箱第628号)", "postal_code": "9638664", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
@@ -122948,25 +122950,24 @@
 INSERT INTO office_data VALUES('9631388','{"jis": "07203", "kana": "トウホクカザイ カブシキガイシヤ", "name": "東北花材　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "熱海町安子島", "banchi": "字薬師堂125", "postal_code": "9631388", "old_code": "96313", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アタミマチアコガシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9631386','{"jis": "07203", "kana": "ナカヤマシヨウジ カブシキガイシヤ コオリヤマエイギヨウシヨ", "name": "中山商事　株式会社　郡山営業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "熱海町安子島", "banchi": "字南原13-1", "postal_code": "9631386", "old_code": "96313", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アタミマチアコガシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9631387','{"jis": "07203", "kana": "ホテルハナノユ", "name": "ホテル華の湯", "prefecture": "福島県", "city": "郡山市", "neighborhood": "熱海町熱海", "banchi": "5丁目8-60", "postal_code": "9631387", "old_code": "96313", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アタミマチアタミ", "alternates": []}');
 INSERT INTO office_data VALUES('9638622','{"jis": "07203", "kana": "カブシキガイシヤ ダイトウギンコウ", "name": "株式会社　大東銀行", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "19-1(郡山郵便局私書箱第8号)", "postal_code": "9638622", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638602','{"jis": "07203", "kana": "カブシキガイシヤ トウホウギンコウ コオリヤマシテン", "name": "株式会社　東邦銀行　郡山支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "虎丸町", "banchi": "20-58(郡山郵便局私書箱第20号)", "postal_code": "9638602", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トラマルマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638611','{"jis": "07203", "kana": "ガツコウホウジン セイセンガクシヤ オウウダイガク", "name": "学校法人　晴川学舎　奥羽大学", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字三角堂31-1(郡山郵便局私書箱第3号)", "postal_code": "9638611", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638630','{"jis": "07203", "kana": "コオリヤマシンヨウキンコ", "name": "郡山信用金庫", "prefecture": "福島県", "city": "郡山市", "neighborhood": "清水台", "banchi": "2丁目13-26(郡山郵便局私書箱第6号)", "postal_code": "9638630", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "シミズダイ", "alternates": []}');
-INSERT INTO office_data VALUES('9638637','{"jis": "07203", "kana": "ニホンデンサンコパル カブシキガイシヤ コオリヤマギジユツカイハツセンタ-", "name": "日本電産コパル　株式会社　郡山技術開発センター", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字諏訪内37(郡山郵便局私書箱第37号)", "postal_code": "9638637", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638794','{"jis": "07203", "kana": "コオリヤマテン ホウジンサ-ビスブ", "name": "郡山店　法人サービス部", "prefecture": "福島県", "city": "郡山市", "neighborhood": "清水台", "banchi": "2丁目13-21", "postal_code": "9638794", "old_code": "96399", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "シミズダイ", "alternates": []}');
 INSERT INTO office_data VALUES('9708611','{"jis": "07204", "kana": "イワキゼイムシヨ", "name": "いわき税務署", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字菱川町6-3", "postal_code": "9708611", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708551','{"jis": "07204", "kana": "イワキメイセイダイガク", "name": "いわき明星大学", "prefecture": "福島県", "city": "いわき市", "neighborhood": "中央台飯野", "banchi": "5丁目5-1", "postal_code": "9708551", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "チュウオウダイイイノ", "alternates": []}');
 INSERT INTO office_data VALUES('9708703','{"jis": "07204", "kana": "イワキロウドウキジユンカントクシヨ", "name": "いわき労働基準監督署", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字堂根町4-11", "postal_code": "9708703", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708625','{"jis": "07204", "kana": "オカダデンキサンギヨウ カブシキガイシヤ", "name": "岡田電気産業　株式会社", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平谷川瀬", "banchi": "一丁目6-1(いわき郵便局私書箱第25号)", "postal_code": "9708625", "old_code": "970  ", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラヤガワセ", "alternates": []}');
 INSERT INTO office_data VALUES('9708511','{"jis": "07204", "kana": "カブシキカイシヤエヌテイテイヒガシニホンフクシマ イワキシテン", "name": "株式会社　ＮＴＴ東日本－福島　いわき支店", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字堂根町3-2", "postal_code": "9708511", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708516','{"jis": "07204", "kana": "ザイダンホウジン イワキサイセイカイ マツムラソウゴウビヨウイン", "name": "財団法人　磐城済世会　松村総合病院", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字小太郎町1-1", "postal_code": "9708516", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708501','{"jis": "07204", "kana": "ニツポンネンキンキコウ タイラネンキンジムシヨ", "name": "日本年金機構　平年金事務所", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字童子町3-21", "postal_code": "9708501", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708410','{"jis": "07204", "kana": "ホテルビ-フオ-テイ- エスパルイワキ", "name": "ホテルＢ４Ｔ　エスパルいわき", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字田町1", "postal_code": "9708410", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
-INSERT INTO office_data VALUES('9701192','{"jis": "07204", "kana": "アルパイン カブシキガイシヤ イワキジギヨウシヨ", "name": "アルパイン　株式会社　いわき事業所", "prefecture": "福島県", "city": "いわき市", "neighborhood": "好間工業団地", "banchi": "20-1", "postal_code": "9701192", "old_code": "97011", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ヨシマコウギョウダンチ", "alternates": []}');
+INSERT INTO office_data VALUES('9701192','{"jis": "07204", "kana": "アルプスアルパイン カブシキガイシヤ イワキカイハツセンタ-", "name": "アルプスアルパイン　株式会社　いわき開発センター", "prefecture": "福島県", "city": "いわき市", "neighborhood": "好間工業団地", "banchi": "20-1", "postal_code": "9701192", "old_code": "97011", "post_office": "いわき", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ヨシマコウギョウダンチ", "alternates": []}');
 INSERT INTO office_data VALUES('9701193','{"jis": "07204", "kana": "アルプスデンキ カブシキガイシヤ ペリフエラルジギヨウブ タイラコウジヨウ", "name": "アルプス電気　株式会社　ペリフェラル事業部　平工場", "prefecture": "福島県", "city": "いわき市", "neighborhood": "好間町小谷作", "banchi": "字作畑39-1", "postal_code": "9701193", "old_code": "97011", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ヨシママチオヤサク", "alternates": []}');
 INSERT INTO office_data VALUES('9701194','{"jis": "07204", "kana": "ユウゲンガイシヤ ナガクボシヨクヒン", "name": "有限会社　長久保食品", "prefecture": "福島県", "city": "いわき市", "neighborhood": "好間町中好間", "banchi": "字鍛冶内28-2", "postal_code": "9701194", "old_code": "97011", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ヨシママチナカヨシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9708686','{"jis": "07204", "kana": "イワキシヤクシヨ", "name": "いわき市役所", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字梅本21(いわき郵便局私書箱第55号)", "postal_code": "9708686", "old_code": "97091", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708646','{"jis": "07204", "kana": "カブシキガイシヤ カチワグミ", "name": "株式会社　加地和組", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字小太郎町4-11(いわき郵便局私書箱第46号)", "postal_code": "9708646", "old_code": "97091", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708635','{"jis": "07204", "kana": "サトウ カブシキガイシヤ イワキシテン", "name": "佐藤　株式会社　いわき支店", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字五町目18-5(いわき郵便局私書箱第35号)", "postal_code": "9708635", "old_code": "97091", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9718555','{"jis": "07204", "kana": "イオンモ-ルイワキオナハマ イオンモ-ルジムシヨ", "name": "イオンモールいわき小名浜　イオンモール事務所", "prefecture": "福島県", "city": "いわき市", "neighborhood": "小名浜", "banchi": "字辰巳町79番地", "postal_code": "9718555", "old_code": "971  ", "post_office": "小名浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "オナハマ", "alternates": []}');
 INSERT INTO office_data VALUES('9728555','{"jis": "07204", "kana": "ジヨウバンコウサン カブシキガイシヤ スパ・リゾ-ト・ハワイアンズ", "name": "常磐興産　株式会社　スパ・リゾート・ハワイアンズ", "prefecture": "福島県", "city": "いわき市", "neighborhood": "常磐藤原町", "banchi": "蕨平50", "postal_code": "9728555", "old_code": "972  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "ジョウバンフジワラマチ", "alternates": []}');
@@ -123185,15 +123186,15 @@
 INSERT INTO office_data VALUES('3038501','{"jis": "08211", "kana": "ジヨウソウシヤクシヨ", "name": "常総市役所", "prefecture": "茨城県", "city": "常総市", "neighborhood": "水海道諏訪町", "banchi": "3222-3", "postal_code": "3038501", "old_code": "303  ", "post_office": "水海道", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ジョウソウシ", "neighborhood_kana": "ミツカイドウスワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3138666','{"jis": "08212", "kana": "イバラキケンヒタチオオタケンゼイジムシヨ", "name": "茨城県常陸太田県税事務所", "prefecture": "茨城県", "city": "常陸太田市", "neighborhood": "山下町", "banchi": "4119", "postal_code": "3138666", "old_code": "313  ", "post_office": "常陸太田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ヒタチオオタシ", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3138686','{"jis": "08212", "kana": "オオタ ゼイムシヨ", "name": "太田　税務署", "prefecture": "茨城県", "city": "常陸太田市", "neighborhood": "金井町", "banchi": "3662(常陸太田郵便局私書箱第7号)", "postal_code": "3138686", "old_code": "313  ", "post_office": "常陸太田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ヒタチオオタシ", "neighborhood_kana": "カナイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3138511','{"jis": "08212", "kana": "カワサキビヨウイン", "name": "川崎病院", "prefecture": "茨城県", "city": "常陸太田市", "neighborhood": "木崎二町", "banchi": "2040", "postal_code": "3138511", "old_code": "313  ", "post_office": "常陸太田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ヒタチオオタシ", "neighborhood_kana": "キザキニチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3138611','{"jis": "08212", "kana": "ヒタチオオタシヤクシヨ", "name": "常陸太田市役所", "prefecture": "茨城県", "city": "常陸太田市", "neighborhood": "金井町", "banchi": "3690", "postal_code": "3138611", "old_code": "313  ", "post_office": "常陸太田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ヒタチオオタシ", "neighborhood_kana": "カナイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3188511','{"jis": "08214", "kana": "タカハギシヤクシヨ", "name": "高萩市役所", "prefecture": "茨城県", "city": "高萩市", "neighborhood": "本町", "banchi": "1丁目100番1号", "postal_code": "3188511", "old_code": "318  ", "post_office": "高萩", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "タカハギシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3188501','{"jis": "08214", "kana": "トウブダイケンコウギヨウ カブシキガイシヤ", "name": "東部大建工業　株式会社", "prefecture": "茨城県", "city": "高萩市", "neighborhood": "赤浜", "banchi": "160番地の1", "postal_code": "3188501", "old_code": "318  ", "post_office": "高萩", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "タカハギシ", "neighborhood_kana": "アカハマ", "alternates": []}');
-INSERT INTO office_data VALUES('3188505','{"jis": "08214", "kana": "ニツポンケミコン カブシキガイシヤ タカハギコウジヨウ", "name": "日本ケミコン　株式会社　高萩工場", "prefecture": "茨城県", "city": "高萩市", "neighborhood": "安良川", "banchi": "字下ノ内363", "postal_code": "3188505", "old_code": "318  ", "post_office": "高萩", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "タカハギシ", "neighborhood_kana": "アラカワ", "alternates": []}');
+INSERT INTO office_data VALUES('3188505','{"jis": "08214", "kana": "ニツポンケミコン カブシキガイシヤ タカハギコウジヨウ", "name": "日本ケミコン　株式会社　高萩工場", "prefecture": "茨城県", "city": "高萩市", "neighborhood": "安良川", "banchi": "字下ノ内363", "postal_code": "3188505", "old_code": "318  ", "post_office": "高萩", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "タカハギシ", "neighborhood_kana": "アラカワ", "alternates": []}');
 INSERT INTO office_data VALUES('3191592','{"jis": "08215", "kana": "キタイバラキシヤクシヨ", "name": "北茨城市役所", "prefecture": "茨城県", "city": "北茨城市", "neighborhood": "磯原町磯原", "banchi": "1630", "postal_code": "3191592", "old_code": "31915", "post_office": "北茨城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "キタイバラキシ", "neighborhood_kana": "イソハラチョウイソハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3191593','{"jis": "08215", "kana": "ユニマテツク カブシキガイシヤ", "name": "ユニマテック　株式会社", "prefecture": "茨城県", "city": "北茨城市", "neighborhood": "磯原町上相田", "banchi": "831-2", "postal_code": "3191593", "old_code": "31915", "post_office": "北茨城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "キタイバラキシ", "neighborhood_kana": "イソハラチョウカミソウダ", "alternates": []}');
 INSERT INTO office_data VALUES('3091698','{"jis": "08216", "kana": "カサマシヤクシヨ カサマシシヨ", "name": "笠間市役所　笠間支所", "prefecture": "茨城県", "city": "笠間市", "neighborhood": "笠間", "banchi": "1532", "postal_code": "3091698", "old_code": "30916", "post_office": "笠間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カサマシ", "neighborhood_kana": "カサマ", "alternates": []}');
 INSERT INTO office_data VALUES('3091793','{"jis": "08216", "kana": "イバラキケンリツ チユウオウビヨウイン", "name": "茨城県立　中央病院", "prefecture": "茨城県", "city": "笠間市", "neighborhood": "鯉淵", "banchi": "6528", "postal_code": "3091793", "old_code": "30917", "post_office": "友部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カサマシ", "neighborhood_kana": "コイブチ", "alternates": []}');
 INSERT INTO office_data VALUES('3091792','{"jis": "08216", "kana": "カサマシヤクシヨ", "name": "笠間市役所", "prefecture": "茨城県", "city": "笠間市", "neighborhood": "中央", "banchi": "3丁目2-1", "postal_code": "3091792", "old_code": "30917", "post_office": "友部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カサマシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3091797','{"jis": "08216", "kana": "カブシキガイシヤ モノタロウ カサマデイストリビユ-シヨンセンタ-", "name": "株式会社　ＭｏｎｏｔａＲＯ　笠間ディストリビューションセンター", "prefecture": "茨城県", "city": "笠間市", "neighborhood": "平町", "banchi": "1877-3", "postal_code": "3091797", "old_code": "30917", "post_office": "友部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カサマシ", "neighborhood_kana": "タイラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3190292','{"jis": "08216", "kana": "イバラキケンノウギヨウソウゴウセンタ-", "name": "茨城県農業総合センター", "prefecture": "茨城県", "city": "笠間市", "neighborhood": "安居", "banchi": "3165-1", "postal_code": "3190292", "old_code": "31902", "post_office": "岩間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カサマシ", "neighborhood_kana": "アゴ", "alternates": []}');
@@ -123544,23 +123545,24 @@
 INSERT INTO office_data VALUES('3238601','{"jis": "09208", "kana": "フルカワキカイキンゾク カブシキガイシヤ オヤマコウジヨウ", "name": "古河機械金属　株式会社　小山工場", "prefecture": "栃木県", "city": "小山市", "neighborhood": "若木町", "banchi": "1丁目23-15(小山郵便局私書箱第9号)", "postal_code": "3238601", "old_code": "323  ", "post_office": "小山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オヤマシ", "neighborhood_kana": "ワカギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3214392','{"jis": "09209", "kana": "エスエイチピ-ピ-ジヤパン ゴウドウカイシヤ", "name": "ＳＨＰＰジャパン　合同会社", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "鬼怒ケ丘", "banchi": "2番地2", "postal_code": "3214392", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "キヌガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3214393','{"jis": "09209", "kana": "ダイイチデンシコウギヨウ カブシキガイシヤ", "name": "第一電子工業　株式会社", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "松山町", "banchi": "14", "postal_code": "3214393", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "マツヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3214396','{"jis": "09209", "kana": "フジフアイバ-グラス カブシキガイシヤ", "name": "富士ファイバーグラス　株式会社", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "鬼怒ケ丘", "banchi": "6", "postal_code": "3214396", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "キヌガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3214398','{"jis": "09209", "kana": "モオカケンゼイジムシヨ", "name": "真岡県税事務所", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "荒町", "banchi": "116-1", "postal_code": "3214398", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "アラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3214395','{"jis": "09209", "kana": "モオカシヤクシヨ", "name": "真岡市役所", "prefecture": "栃木県", "city": "真岡市", "neighborhood": "荒町", "banchi": "5191", "postal_code": "3214395", "old_code": "32143", "post_office": "真岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "モオカシ", "neighborhood_kana": "アラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3248642','{"jis": "09210", "kana": "オオタワラ ゼイムシヨ", "name": "大田原　税務署", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "紫塚", "banchi": "1丁目5-54(大田原郵便局私書箱第11号)", "postal_code": "3248642", "old_code": "324  ", "post_office": "大田原", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ムラサキヅカ", "alternates": []}');
-INSERT INTO office_data VALUES('3248551','{"jis": "09210", "kana": "オオタワラケンゼイジムシヨ", "name": "大田原県税事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "中央", "banchi": "1丁目9-9", "postal_code": "3248551", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
+INSERT INTO office_data VALUES('3248551','{"jis": "09210", "kana": "オオタワラケンゼイジムシヨ", "name": "大田原県税事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2丁目2828-4", "postal_code": "3248551", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248641','{"jis": "09210", "kana": "オオタワラシヤクシヨ", "name": "大田原市役所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "1丁目4-1", "postal_code": "3248641", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('3248765','{"jis": "09210", "kana": "オオタワラドボクジムシヨ", "name": "大田原土木事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2-2828-4", "postal_code": "3248765", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248625','{"jis": "09210", "kana": "カブシキガイシヤ トチギニコン", "name": "株式会社　栃木ニコン", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "実取", "banchi": "770", "postal_code": "3248625", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ミドリ", "alternates": []}');
 INSERT INTO office_data VALUES('3248520','{"jis": "09210", "kana": "カブシキガイシヤ トチギニコンプレシジヨン", "name": "株式会社　栃木ニコンプレシジョン", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "実取", "banchi": "760番地", "postal_code": "3248520", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ミドリ", "alternates": []}');
 INSERT INTO office_data VALUES('3248550','{"jis": "09210", "kana": "キヤノンデンシカンデバイス カブシキガイシヤ", "name": "キヤノン電子管デバイス　株式会社", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "下石上", "banchi": "1385番地", "postal_code": "3248550", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "シモイシガミ", "alternates": [{"jis": "09210", "kana": "キヤノンメデイカルシステムズ カブシキガイシヤ", "name": "キヤノンメディカルシステムズ　株式会社", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "下石上", "banchi": "1385", "postal_code": "3248550", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "シモイシガミ", "alternates": []}]}');
 INSERT INTO office_data VALUES('3248501','{"jis": "09210", "kana": "コクサイイリヨウフクシダイガク", "name": "国際医療福祉大学", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "北金丸", "banchi": "2600-1", "postal_code": "3248501", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "キタカネマル", "alternates": []}');
 INSERT INTO office_data VALUES('3248516','{"jis": "09210", "kana": "ダイニツポントリヨウ カブシキガイシヤ ナスコウジヨウ", "name": "大日本塗料　株式会社　那須工場", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "下石上", "banchi": "1382-12", "postal_code": "3248516", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "シモイシガミ", "alternates": []}');
+INSERT INTO office_data VALUES('3248585','{"jis": "09210", "kana": "トチギケンケンポクケンコウフクシセンタ-", "name": "栃木県県北健康福祉センター", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "2丁目2828-4", "postal_code": "3248585", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248686','{"jis": "09210", "kana": "ナスセキジユウジビヨウイン", "name": "那須赤十字病院", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "中田原", "banchi": "1081番地4(大田原郵便局私書箱第15号)", "postal_code": "3248686", "old_code": "324  ", "post_office": "大田原", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ナカダワラ", "alternates": []}');
-INSERT INTO office_data VALUES('3248585','{"jis": "09210", "kana": "ナスフクシジムシヨ", "name": "那須福祉事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "中央", "banchi": "1丁目9-9", "postal_code": "3248585", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248540','{"jis": "09210", "kana": "ニツポンネンキンキコウ オオタワラネンキンジムシヨ", "name": "日本年金機構　大田原年金事務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "本町", "banchi": "1丁目2695-22", "postal_code": "3248540", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3248555','{"jis": "09210", "kana": "フジツウ カブシキガイシヤ ナスコウジヨウ", "name": "富士通　株式会社　那須工場", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "下石上", "banchi": "1388", "postal_code": "3248555", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "シモイシガミ", "alternates": []}');
 INSERT INTO office_data VALUES('3248510','{"jis": "09210", "kana": "フジデンキ カブシキガイシヤ オオタワラコウジヨウ", "name": "富士電機　株式会社　大田原工場", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "中田原", "banchi": "1043", "postal_code": "3248510", "old_code": "324  ", "post_office": "大田原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ナカダワラ", "alternates": []}');
 INSERT INTO office_data VALUES('3240292','{"jis": "09210", "kana": "オオタワラシヤクシヨ クロバネシシヨ", "name": "大田原市役所　黒羽支所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "黒羽田町", "banchi": "848", "postal_code": "3240292", "old_code": "32402", "post_office": "黒羽", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "クロバネタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3240293','{"jis": "09210", "kana": "クロバネケイムシヨ", "name": "黒羽刑務所", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "寒井", "banchi": "1466-2", "postal_code": "3240293", "old_code": "32402", "post_office": "黒羽", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "サブイ", "alternates": []}');
 INSERT INTO office_data VALUES('3240492','{"jis": "09210", "kana": "オオタワラシヤクシヨ ユヅカミチヨウシヤ", "name": "大田原市役所　湯津上庁舎", "prefecture": "栃木県", "city": "大田原市", "neighborhood": "湯津上", "banchi": "5-1081", "postal_code": "3240492", "old_code": "32404", "post_office": "佐良土", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "オオタワラシ", "neighborhood_kana": "ユヅカミ", "alternates": []}');
 INSERT INTO office_data VALUES('3292192','{"jis": "09211", "kana": "ヤイタシヤクシヨ", "name": "矢板市役所", "prefecture": "栃木県", "city": "矢板市", "neighborhood": "本町", "banchi": "5-4", "postal_code": "3292192", "old_code": "32921", "post_office": "矢板", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "ヤイタシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
@@ -123825,14 +123827,15 @@
 INSERT INTO office_data VALUES('3758604','{"jis": "10209", "kana": "グンマギンコウ", "name": "群馬銀行", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "391(藤岡郵便局私書箱第1号)", "postal_code": "3758604", "old_code": "375  ", "post_office": "藤岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758503','{"jis": "10209", "kana": "コウリツ フジオカソウゴウビヨウイン", "name": "公立　藤岡総合病院", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "中栗須", "banchi": "813番地1", "postal_code": "3758503", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "ナカクリス", "alternates": []}');
 INSERT INTO office_data VALUES('3758603','{"jis": "10209", "kana": "タノシンヨウキンコ", "name": "多野信用金庫", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "314(藤岡郵便局私書箱第10号)", "postal_code": "3758603", "old_code": "375  ", "post_office": "藤岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758602','{"jis": "10209", "kana": "フジオカ ゼイムシヨ", "name": "藤岡　税務署", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "668-1(藤岡郵便局私書箱第5号)", "postal_code": "3758602", "old_code": "375  ", "post_office": "藤岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758504','{"jis": "10209", "kana": "フジオカコウコウ", "name": "藤岡高校", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "1485", "postal_code": "3758504", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758601','{"jis": "10209", "kana": "フジオカシヤクシヨ", "name": "藤岡市役所", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "中栗須", "banchi": "327(藤岡郵便局私書箱第9号)", "postal_code": "3758601", "old_code": "375  ", "post_office": "藤岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "ナカクリス", "alternates": []}');
 INSERT INTO office_data VALUES('3758506','{"jis": "10209", "kana": "フジオカシヨウコウカイギシヨ", "name": "藤岡商工会議所", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "853-1", "postal_code": "3758506", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
+INSERT INTO office_data VALUES('3758507','{"jis": "10209", "kana": "ミサトコウギヨウ カブシキカイシヤ", "name": "美里工業　株式会社", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "藤岡", "banchi": "1360", "postal_code": "3758507", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": true, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "フジオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3758501','{"jis": "10209", "kana": "ミツビシエンピツ カブシキガイシヤ グンマコウジヨウ", "name": "三菱鉛筆　株式会社　群馬工場", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "立石", "banchi": "1091", "postal_code": "3758501", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "タツイシ", "alternates": []}');
 INSERT INTO office_data VALUES('3758502','{"jis": "10209", "kana": "ヨシモトポ-ル カブシキガイシヤ", "name": "ヨシモトポール　株式会社", "prefecture": "群馬県", "city": "藤岡市", "neighborhood": "中栗須", "banchi": "508", "postal_code": "3758502", "old_code": "375  ", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "フジオカシ", "neighborhood_kana": "ナカクリス", "alternates": []}');
 INSERT INTO office_data VALUES('3702398','{"jis": "10210", "kana": "カブシキガイシヤ アイエイチアイエアロスペ-ス トミオカジギヨウシヨ", "name": "株式会社　ＩＨＩエアロスペース　富岡事業所", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "藤木", "banchi": "900番地", "postal_code": "3702398", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "フジキ", "alternates": []}');
 INSERT INTO office_data VALUES('3702396','{"jis": "10210", "kana": "カンラトミオカノウギヨウ キヨウドウクミアイ", "name": "甘楽富岡農業　協同組合", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "富岡", "banchi": "2638-1", "postal_code": "3702396", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "トミオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3702393','{"jis": "10210", "kana": "コウリツトミオカソウゴウビヨウイン", "name": "公立富岡総合病院", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "富岡", "banchi": "2073-1", "postal_code": "3702393", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "トミオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3702395','{"jis": "10210", "kana": "シノノメシンヨウキンコ", "name": "しののめ信用金庫", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "富岡", "banchi": "1123番地", "postal_code": "3702395", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "トミオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3702392','{"jis": "10210", "kana": "トミオカシヤクシヨ", "name": "富岡市役所", "prefecture": "群馬県", "city": "富岡市", "neighborhood": "富岡", "banchi": "1460-1", "postal_code": "3702392", "old_code": "37023", "post_office": "富岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "トミオカシ", "neighborhood_kana": "トミオカ", "alternates": []}');
@@ -124531,15 +124534,15 @@
 INSERT INTO office_data VALUES('3490292','{"jis": "11246", "kana": "シラオカシヤクシヨ", "name": "白岡市役所", "prefecture": "埼玉県", "city": "白岡市", "neighborhood": "千駄野", "banchi": "432番地", "postal_code": "3490292", "old_code": "34902", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "シラオカシ", "neighborhood_kana": "センダノ", "alternates": []}');
 INSERT INTO office_data VALUES('3490293','{"jis": "11246", "kana": "タイセイラミツク カブシキガイシヤ", "name": "大成ラミック　株式会社", "prefecture": "埼玉県", "city": "白岡市", "neighborhood": "下大崎", "banchi": "873", "postal_code": "3490293", "old_code": "34902", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "シラオカシ", "neighborhood_kana": "シモオオサキ", "alternates": []}');
 INSERT INTO office_data VALUES('3490294','{"jis": "11246", "kana": "ニツサンカガクコウギヨウ カブシキガイシヤ", "name": "日産化学工業　株式会社", "prefecture": "埼玉県", "city": "白岡市", "neighborhood": "白岡", "banchi": "1470", "postal_code": "3490294", "old_code": "34902", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "シラオカシ", "neighborhood_kana": "シラオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3628517','{"jis": "11301", "kana": "イナマチヤクバ", "name": "伊奈町役場", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小室", "banchi": "9493", "postal_code": "3628517", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3628539','{"jis": "11301", "kana": "カブシキガイシヤ サイサン", "name": "株式会社　サイサン", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小室", "banchi": "字道上10360", "postal_code": "3628539", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3628553','{"jis": "11301", "kana": "カブシキガイシヤ ニツポンアクセス イナチルドブツリユウセンタ-", "name": "株式会社　日本アクセス　伊奈チルド物流センター", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小針新宿", "banchi": "字梶川847番地", "postal_code": "3628553", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3628542','{"jis": "11301", "kana": "カブシキガイシヤ ニツポンアクセス サイタマシテン", "name": "株式会社　日本アクセス　埼玉支店", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小針新宿", "banchi": "字梶川833番地", "postal_code": "3628542", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3628577','{"jis": "11301", "kana": "ダイニツポンインキカガクコウギヨウ カブシキガイシヤ サイタマコウジヨウ", "name": "大日本インキ化学工業　株式会社　埼玉工場", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "大字小室", "banchi": "4472-1", "postal_code": "3628577", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('3628577','{"jis": "11301", "kana": "デイ-アイシ- カブシキガイシヤ サイタマコウジヨウ", "name": "ＤＩＣ　株式会社　埼玉工場", "prefecture": "埼玉県", "city": "北足立郡伊奈町", "neighborhood": "小室", "banchi": "4472-1", "postal_code": "3628577", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": true, "prefecture_kana": "サイタマケン", "city_kana": "キタアダチグンイナマチ", "neighborhood_kana": "コムロ", "alternates": []}');
 INSERT INTO office_data VALUES('3548565','{"jis": "11324", "kana": "アスクル ロジ パ-ク シユトケン", "name": "ＡＳＫＵＬ　Ｌｏｇｉ　ＰＡＲＫ　首都圏", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "上富", "banchi": "1163", "postal_code": "3548565", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "イルマグンミヨシマチ", "neighborhood_kana": "カミトメ", "alternates": []}');
 INSERT INTO office_data VALUES('3548501','{"jis": "11324", "kana": "オオサキデンキ カブシキガイシヤ サイタマジギヨウシヨ", "name": "大崎電気　株式会社　埼玉事業所", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "大字藤久保", "banchi": "1131", "postal_code": "3548501", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3548504','{"jis": "11324", "kana": "カブシキガイシヤ ガツケンロジステイクス", "name": "（株）　学研ロジスティクス", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "大字上富", "banchi": "279-1", "postal_code": "3548504", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3548505','{"jis": "11324", "kana": "カブシキガイシヤ シユフノトモシヤ", "name": "株式会社　主婦の友社", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "みよし台", "banchi": "13-10", "postal_code": "3548505", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "イルマグンミヨシマチ", "neighborhood_kana": "ミヨシダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3548577','{"jis": "11324", "kana": "カブシキガイシヤ テイ-アンドケイトオカ", "name": "株式会社　Ｔ＆Ｋ　ＴＯＫＡ", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "大字竹間沢", "banchi": "283-1", "postal_code": "3548577", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3548533','{"jis": "11324", "kana": "カブシキガイシヤシユフノトモシヤ ツウハンジギヨウブ", "name": "株式会社主婦の友社　通販事業部", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "竹間沢東", "banchi": "7番地5", "postal_code": "3548533", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "イルマグンミヨシマチ", "neighborhood_kana": "チクマザワヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('3548510','{"jis": "11324", "kana": "シユクトクダイガク コクサイコミユニケ-シヨンガクブ", "name": "淑徳大学　国際コミュニケーション学部", "prefecture": "埼玉県", "city": "入間郡三芳町", "neighborhood": "大字藤久保", "banchi": "1150-1", "postal_code": "3548510", "old_code": "354  ", "post_office": "三芳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -124622,15 +124625,15 @@
 INSERT INTO office_data VALUES('2608626','{"jis": "12101", "kana": "カブシキガイシヤ ミツイフドウサンホテルマネジメント ミツイガ-デンホテルチバ", "name": "株式会社　三井不動産ホテルマネジメント　三井ガーデンホテル千葉", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "中央", "banchi": "1丁目11-1", "postal_code": "2608626", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608631','{"jis": "12101", "kana": "カブシキガイシヤ ミツコシイセタン ミツコシチバテン", "name": "株式会社　三越伊勢丹　三越千葉店", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "富士見", "banchi": "2丁目6-1", "postal_code": "2608631", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('2608636','{"jis": "12101", "kana": "カブシキガイシヤ ミツビシトウキヨウユーエフジエイギンコウ チバシテン、 チバチユウオウシテン", "name": "株式会社　三菱東京ＵＦＪ銀行　千葉支店、千葉中央支店", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "富士見", "banchi": "2-3-1", "postal_code": "2608636", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('2608588','{"jis": "12101", "kana": "カブシキガイシヤ ライフランド", "name": "株式会社　ライフランド", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "祐光", "banchi": "4丁目18-3", "postal_code": "2608588", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ユウコウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608601','{"jis": "12101", "kana": "ガツコウホウジン ウエクサガクエン", "name": "学校法人　植草学園", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "弁天", "banchi": "2丁目8番9号", "postal_code": "2608601", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ベンテン", "alternates": []}');
 INSERT INTO office_data VALUES('2608685','{"jis": "12101", "kana": "ガツコウホウジン チバメイトクガクエン", "name": "学校法人　千葉明徳学園", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "南生実町", "banchi": "1412", "postal_code": "2608685", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ミナミオユミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608572','{"jis": "12101", "kana": "ガツコウホウジン ハナザワガクエン", "name": "学校法人　花沢学園", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "本千葉町", "banchi": "10-23", "postal_code": "2608572", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ホンチバチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('2608661','{"jis": "12101", "kana": "コウエキザイダンホウジン チバケンブンカシンコウザイダン", "name": "公益財団法人　千葉県文化振興財団", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "青葉町", "banchi": "977-1青葉の森公園芸術文化ホール内", "postal_code": "2608661", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "アオバチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('2608661','{"jis": "12101", "kana": "コウエキザイダンホウジン チバケンブンカシンコウザイダン", "name": "公益財団法人　千葉県文化振興財団", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "青葉町", "banchi": "977-1青葉の森公園芸術文化ホール内", "postal_code": "2608661", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "アオバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608566','{"jis": "12101", "kana": "コウエキシヤダンホウジン チバケンボウハンキヨウカイ", "name": "公益社団法人　千葉県防犯協会", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "中央", "banchi": "4丁目13番10号千葉県教育会館別館4階", "postal_code": "2608566", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608619','{"jis": "12101", "kana": "コウリツガツコウキヨウサイクミアイ チバシブ", "name": "公立学校共済組合　千葉支部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "市場町", "banchi": "1-1", "postal_code": "2608619", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "イチバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608534','{"jis": "12101", "kana": "コバヤシシヨウジ カブシキガイシヤ", "name": "小林商事　株式会社", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "問屋町", "banchi": "14-2", "postal_code": "2608534", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "トンヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608559','{"jis": "12101", "kana": "サンケイリビングシンブンシヤ チバホンブ", "name": "サンケイリビング新聞社　千葉本部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "新町", "banchi": "3-13千葉TNビル5F", "postal_code": "2608559", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "シンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('2608629','{"jis": "12101", "kana": "ザイダンホウジン チバケンコウリツガツコウキヨウシヨクインゴジヨカイ", "name": "財団法人　千葉県公立学校教職員互助会", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "市場町", "banchi": "1番1号", "postal_code": "2608629", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "イチバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608562','{"jis": "12101", "kana": "ザイダンホウジン ニホンボウサイツウシンキヨウカイ チバケンシブ", "name": "財団法人　日本防災通信協会　千葉県支部", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "都町", "banchi": "1丁目1-30千葉県警都町庁舎内", "postal_code": "2608562", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ミヤコチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2608607','{"jis": "12101", "kana": "ザイムシヨウ カントウザイムキヨク チバザイムジムシヨ", "name": "財務省　関東財務局　千葉財務事務所", "prefecture": "千葉県", "city": "千葉市中央区", "neighborhood": "椿森", "banchi": "5丁目6-1", "postal_code": "2608607", "old_code": "260  ", "post_office": "千葉中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシチュウオウク", "neighborhood_kana": "ツバキモリ", "alternates": []}');
@@ -125038,15 +125041,15 @@
 INSERT INTO office_data VALUES('2995292','{"jis": "12218", "kana": "カツウラシヤクシヨ", "name": "勝浦市役所", "prefecture": "千葉県", "city": "勝浦市", "neighborhood": "新官", "banchi": "1343-1", "postal_code": "2995292", "old_code": "29952", "post_office": "勝浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カツウラシ", "neighborhood_kana": "シンカン", "alternates": []}');
 INSERT INTO office_data VALUES('2995295','{"jis": "12218", "kana": "コクサイブドウダイガク", "name": "国際武道大学", "prefecture": "千葉県", "city": "勝浦市", "neighborhood": "新官", "banchi": "841", "postal_code": "2995295", "old_code": "29952", "post_office": "勝浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カツウラシ", "neighborhood_kana": "シンカン", "alternates": []}');
 INSERT INTO office_data VALUES('2908566','{"jis": "12219", "kana": "アサヒガラス カブシキガイシヤ チバコウジヨウ", "name": "旭硝子　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井海岸", "banchi": "10", "postal_code": "2908566", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908510','{"jis": "12219", "kana": "アサヒガラスエンジニアリング カブシキガイシヤ", "name": "旭硝子エンジニアリング　株式会社", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "38", "postal_code": "2908510", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908501','{"jis": "12219", "kana": "イチハラシヤクシヨ", "name": "市原市役所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "国分寺台中央", "banchi": "1丁目1-1", "postal_code": "2908501", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "コクブンジダイチュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2908540','{"jis": "12219", "kana": "ウエルシアヤツキヨク カブシキガイシヤ ネツトジギヨウブ", "name": "ウエルシア薬局　株式会社　ネット事業部", "prefecture": "千葉県", "city": "市原市", "neighborhood": "南国分寺台", "banchi": "4-1-1-2F", "postal_code": "2908540", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ミナミコクブンジダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2908577','{"jis": "12219", "kana": "カブシキガイシヤ ヒノツクス", "name": "株式会社　ヒノックス", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井中央西", "banchi": "1丁目2-2", "postal_code": "2908577", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイチュウオウニシ", "alternates": []}');
-INSERT INTO office_data VALUES('2908567','{"jis": "12219", "kana": "カブシキガイシヤ レゾナツク ゴイジギヨウシヨ", "name": "株式会社　レゾナック　五井事業所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "14", "postal_code": "2908567", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
+INSERT INTO office_data VALUES('2908567','{"jis": "12219", "kana": "カブシキガイシヤ レゾナツク ゴイジギヨウシヨ", "name": "株式会社　レゾナック　五井事業所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "14", "postal_code": "2908567", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908560','{"jis": "12219", "kana": "ケイエイチネオケム カブシキカイシヤ チバコウジヨウ", "name": "ＫＨネオケム　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "11番地1", "postal_code": "2908560", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908558','{"jis": "12219", "kana": "コスモセキユ カブシキガイシヤ チバセイユジヨ", "name": "コスモ石油　株式会社　千葉製油所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井海岸", "banchi": "2", "postal_code": "2908558", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908551','{"jis": "12219", "kana": "ジエイエヌシ-セキユカガク カブシキガイシヤ イチハラセイゾウシヨ", "name": "ＪＮＣ石油化学　株式会社　市原製造所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井海岸", "banchi": "5番地の1", "postal_code": "2908551", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908585','{"jis": "12219", "kana": "デイ-アイシ- カブシキガイシヤ チバコウジヨウ", "name": "ＤＩＣ　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "12", "postal_code": "2908585", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908588','{"jis": "12219", "kana": "デンキカガクコウギヨウ カブシキガイシヤ チバコウジヨウ", "name": "電気化学工業　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "6", "postal_code": "2908588", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908530','{"jis": "12219", "kana": "ニホンソウダ カブシキガイシヤ チバコウジヨウ", "name": "日本曹達　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "12-8", "postal_code": "2908530", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908610','{"jis": "12219", "kana": "フジサツシ カブシキガイシヤ チバコウジヨウ", "name": "不二サッシ　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "13", "postal_code": "2908610", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
@@ -125441,15 +125444,15 @@
 INSERT INTO office_data VALUES('1008251','{"jis": "13101", "kana": "ミツビシケミカル カブシキガイシヤ", "name": "三菱ケミカル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "1-1-1パレスビル", "postal_code": "1008251", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008350','{"jis": "13101", "kana": "ミツビシシヨウジプラスチツク カブシキガイシヤ", "name": "三菱商事プラスチック　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "1-8-3", "postal_code": "1008350", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008133','{"jis": "13101", "kana": "ミツビシジシヨ カブシキガイシヤ", "name": "三菱地所　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目1番1号", "postal_code": "1008133", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008113','{"jis": "13101", "kana": "ミツビシジシヨリアルエステ-トサ-ビス カブシキガイシヤ", "name": "三菱地所リアルエステートサービス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "2丁目2-1", "postal_code": "1008113", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008189','{"jis": "13101", "kana": "ミツビシジシヨレジデンス カブシキカイシヤ", "name": "三菱地所レジデンス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目9番2号大手町フィナンシャルシティグランキューブ", "postal_code": "1008189", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008332','{"jis": "13101", "kana": "ミツビシジユウコウギヨウ カブシキカイシヤ", "name": "三菱重工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目2番3号丸の内二重橋ビル", "postal_code": "1008332", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008310','{"jis": "13101", "kana": "ミツビシデンキ カブシキガイシヤ", "name": "三菱電機　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "2丁目2-3", "postal_code": "1008310", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
-INSERT INTO office_data VALUES('1008335','{"jis": "13101", "kana": "ミツビシデンキビルソリユ-シヨンズ カブシキガイシヤ", "name": "三菱電機ビルソリューションズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "2-7-3", "postal_code": "1008335", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
+INSERT INTO office_data VALUES('1008335','{"jis": "13101", "kana": "ミツビシデンキビルソリユ-シヨンズ カブシキガイシヤ", "name": "三菱電機ビルソリューションズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "2-7-3", "postal_code": "1008335", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008303','{"jis": "13101", "kana": "ミツビシデンセンコウギヨウ カブシキガイシヤ", "name": "三菱電線工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目4-1", "postal_code": "1008303", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008338','{"jis": "13101", "kana": "ミツビシマテリアル カブシキガイシヤ", "name": "三菱マテリアル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目3-1", "postal_code": "1008338", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008117','{"jis": "13101", "kana": "ミツビシマテリアル カブシキガイシヤ", "name": "三菱マテリアル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目2番3号丸の内二重橋ビル22階", "postal_code": "1008117", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008127','{"jis": "13101", "kana": "ミツビシユ-エフジエイモルガン・スタンレ-シヨウケン カブシキガイシヤ", "name": "三菱ＵＦＪモルガン・スタンレー証券　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目9番2号大手町フィナンシャルシティグランキューブ", "postal_code": "1008127", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1006262','{"jis": "13101", "kana": "メ-ルボツクス・エトセトラ トウキヨウエキテン", "name": "メールボックス・エトセトラ　東京駅店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "1丁目11-1パシフィックセンチュリープレイス丸の内地下1階", "postal_code": "1006262", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008311','{"jis": "13101", "kana": "メイワサンギヨウ カブシキガイシヤ", "name": "明和産業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目3-1", "postal_code": "1008311", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1006066','{"jis": "13101", "kana": "モリロク カブシキカイシヤ", "name": "森六　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "霞が関", "banchi": "3丁目2-5霞ヶ関ビル6階", "postal_code": "1006066", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カスミガセキ", "alternates": []}');
@@ -125815,15 +125818,15 @@
 INSERT INTO office_data VALUES('1028679','{"jis": "13101", "kana": "カブシキガイシヤ ソニ-・マガジンズ", "name": "株式会社　ソニー・マガジンズ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "五番町", "banchi": "12-1(麹町郵便局私書箱第79号)", "postal_code": "1028679", "old_code": "102  ", "post_office": "麹町", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ゴバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028633','{"jis": "13101", "kana": "カブシキガイシヤ タイヨウキヨウサイ", "name": "株式会社　たいよう共済", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目3-6", "postal_code": "1028633", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028388','{"jis": "13101", "kana": "カブシキガイシヤ タカラジマシヤ", "name": "株式会社　宝島社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一番町", "banchi": "25", "postal_code": "1028388", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イチバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028139','{"jis": "13101", "kana": "カブシキガイシヤ タナカシカキカイテン", "name": "株式会社　田中歯科器械店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "1丁目3-8", "postal_code": "1028139", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028186','{"jis": "13101", "kana": "カブシキガイシヤ ツバキモトチエイン トウキヨウシシヤ", "name": "株式会社　椿本チエイン　東京支社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "3丁目2-4メヂカルフレンドビル", "postal_code": "1028186", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028142','{"jis": "13101", "kana": "カブシキガイシヤ テツゲン", "name": "株式会社　鐵原", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "1丁目4-4", "postal_code": "1028142", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028617','{"jis": "13101", "kana": "カブシキガイシヤ デイ-エムジエイ", "name": "株式会社　ディーエムジェイ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "3丁目5番9号", "postal_code": "1028617", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
-INSERT INTO office_data VALUES('1028513','{"jis": "13101", "kana": "カブシキガイシヤ デイ-テイ-ダイナミクス", "name": "株式会社　ＤＴダイナミクス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028513", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
+INSERT INTO office_data VALUES('1028513','{"jis": "13101", "kana": "カブシキガイシヤ デイ-テイ-ダイナミクス", "name": "株式会社　ＤＴダイナミクス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028513", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028181','{"jis": "13101", "kana": "カブシキガイシヤ ニツカンコウギヨウシンブンシヤ", "name": "株式会社　日刊工業新聞社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "1丁目8-10", "postal_code": "1028181", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028117','{"jis": "13101", "kana": "カブシキガイシヤ ニツケンセツケイ", "name": "株式会社　日建設計", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "2丁目18-3", "postal_code": "1028117", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028350','{"jis": "13101", "kana": "カブシキガイシヤ ニツシン", "name": "株式会社　日新", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "1丁目6番4号", "postal_code": "1028350", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028569','{"jis": "13101", "kana": "カブシキガイシヤ ニツポンホウソウプロジエクト", "name": "株式会社　ニッポン放送プロジェクト", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-6", "postal_code": "1028569", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028512','{"jis": "13101", "kana": "カブシキガイシヤ ニホンエデイタ-ズ", "name": "株式会社　日本エディターズ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "4-6-13-704", "postal_code": "1028512", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028578','{"jis": "13101", "kana": "カブシキガイシヤ ニユ-・オ-タニ", "name": "株式会社　ニュー・オータニ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "4番1号", "postal_code": "1028578", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028260','{"jis": "13101", "kana": "カブシキガイシヤ バイフウカン", "name": "株式会社　培風館", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "4丁目3-12", "postal_code": "1028260", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
@@ -125837,17 +125840,17 @@
 INSERT INTO office_data VALUES('1028604','{"jis": "13101", "kana": "カブシキガイシヤ ホウソウシユツパンエ-ジエンシ-", "name": "株式会社　放送出版エージェンシー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "3丁目7-4秩父屋ビル7階", "postal_code": "1028604", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028602','{"jis": "13101", "kana": "カブシキガイシヤ ホウソウシユツパンプロモ-シヨン", "name": "株式会社　放送出版プロモーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "3丁目7-4秩父屋ビル7階", "postal_code": "1028602", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028155','{"jis": "13101", "kana": "カブシキガイシヤ ホケンドウジンシヤ", "name": "株式会社　保健同人社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一番町", "banchi": "4番地4", "postal_code": "1028155", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イチバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028433','{"jis": "13101", "kana": "カブシキガイシヤ ホソカワヨウコウ", "name": "株式会社　細川洋行", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "11-5", "postal_code": "1028433", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028519','{"jis": "13101", "kana": "カブシキガイシヤ ポプラシヤ", "name": "株式会社　ポプラ社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "4丁目2番地6住友不動産麹町ファーストビル", "postal_code": "1028519", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028019','{"jis": "13101", "kana": "カブシキガイシヤ マツグガ-デン", "name": "株式会社　マッグガーデン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "五番町", "banchi": "6-2ホーマットホライゾンビル5F", "postal_code": "1028019", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ゴバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028520','{"jis": "13101", "kana": "カブシキガイシヤ ミカミ", "name": "株式会社　ミカミ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "1丁目10-1", "postal_code": "1028520", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1028582','{"jis": "13101", "kana": "カブシキガイシヤ ミスミ", "name": "株式会社　ミスミ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028582", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
-INSERT INTO office_data VALUES('1028343','{"jis": "13101", "kana": "カブシキガイシヤ ミスミ カスタマ-・サ-ビス・センタ-", "name": "株式会社　ミスミ　カスタマー・サービス・センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028343", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
-INSERT INTO office_data VALUES('1028583','{"jis": "13101", "kana": "カブシキガイシヤ ミスミグル-プホンシヤ", "name": "株式会社　ミスミグループ本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028583", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
+INSERT INTO office_data VALUES('1028582','{"jis": "13101", "kana": "カブシキガイシヤ ミスミ", "name": "株式会社　ミスミ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028582", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
+INSERT INTO office_data VALUES('1028343','{"jis": "13101", "kana": "カブシキガイシヤ ミスミ カスタマ-・サ-ビス・センタ-", "name": "株式会社　ミスミ　カスタマー・サービス・センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028343", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
+INSERT INTO office_data VALUES('1028583','{"jis": "13101", "kana": "カブシキガイシヤ ミスミグル-プホンシヤ", "name": "株式会社　ミスミグループ本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "一丁目6番5号", "postal_code": "1028583", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028621','{"jis": "13101", "kana": "カブシキガイシヤ ミライケンセツグル-プ", "name": "株式会社　みらい建設グループ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "1丁目4-9", "postal_code": "1028621", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028372','{"jis": "13101", "kana": "カブシキガイシヤ メイコウシヨウカイ", "name": "株式会社　明光商会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "五番町", "banchi": "1-1", "postal_code": "1028372", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ゴバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028642','{"jis": "13101", "kana": "カブシキガイシヤ ユ-ラシアリヨコウシヤ", "name": "株式会社　ユーラシア旅行社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目7-4", "postal_code": "1028642", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028417','{"jis": "13101", "kana": "カブシキガイシヤ ヨ-クマ-ト", "name": "株式会社　ヨークマート", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "8-8", "postal_code": "1028417", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028609','{"jis": "13101", "kana": "カブシキガイシヤ ヨミウリジヨウホウカイハツ ヨミウリフアミリ-・サ-クル", "name": "株式会社　読売情報開発　読売ファミリー・サークル", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目13-3", "postal_code": "1028609", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028401','{"jis": "13101", "kana": "カブシキガイシヤ リビングプロシ-ド", "name": "株式会社　リビングプロシード", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-23文芸春秋ビル新館", "postal_code": "1028401", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028357','{"jis": "13101", "kana": "ガツコウホウジン オオツマガクイン オオツマジヨシダイガク オオツマジヨシダイガクタンキダイガクブ オオツマチユウガツコウ オオツマコウトウガツコウ", "name": "学校法人　大妻学院　大妻女子大学　大妻女子大学短期大学部　大妻中学校　大妻高等学校", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三番町", "banchi": "12番地", "postal_code": "1028357", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "サンバンチョウ", "alternates": []}');
@@ -125905,15 +125908,15 @@
 INSERT INTO office_data VALUES('1028610','{"jis": "13101", "kana": "セイカツキヨウドウクミアイゼンコクトシシヨクインサイガイキヨウサイカイ", "name": "生活協同組合全国都市職員災害共済会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目4-2全国都市会館内", "postal_code": "1028610", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028645','{"jis": "13101", "kana": "セコムソンガイホケン カブシキガイシヤ", "name": "セコム損害保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目6-2", "postal_code": "1028645", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028125','{"jis": "13101", "kana": "セントラルソウゴウカイハツ カブシキガイシヤ", "name": "セントラル総合開発　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "3丁目3番7号", "postal_code": "1028125", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028120','{"jis": "13101", "kana": "ゼネラルエレクトリツクキヤピタルカ-システム カブシキガイシヤ", "name": "ゼネラルエレクトリックキャピタルカーシステム　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "1丁目12-7", "postal_code": "1028120", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028630','{"jis": "13101", "kana": "ゼンコクキヨウサイノウギヨウキヨウドウクミアイレンゴウカイ ゼンコクホンブ", "name": "全国共済農業協同組合連合会　全国本部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目7番9号JA共済ビル", "postal_code": "1028630", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028016','{"jis": "13101", "kana": "ゼンコクケンコウホケンキヨウカイ センインホケンブ", "name": "全国健康保険協会　船員保険部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目7-2ステージビルディング14階", "postal_code": "1028016", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028635','{"jis": "13101", "kana": "ゼンコクシチヨウカイ", "name": "全国市長会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "2丁目4-2", "postal_code": "1028635", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1028532','{"jis": "13101", "kana": "ゼンコクドボクケンチク コクミンケンコウホケンクミアイ カントウジムシヨ", "name": "全国土木建築　国民健康保険組合　関東事務所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "3丁目2麹町共同ビル", "postal_code": "1028532", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
+INSERT INTO office_data VALUES('1028532','{"jis": "13101", "kana": "ゼンコクドボクケンチク コクミンケンコウホケンクミアイ カントウジムシヨ", "name": "全国土木建築　国民健康保険組合　関東事務所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "一丁目五番九号厚生会館", "postal_code": "1028532", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028564','{"jis": "13101", "kana": "ゼンコクドボクケンチクコクミンケンコウホケンクミアイ", "name": "全国土木建築国民健康保険組合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "平河町", "banchi": "1-5-9厚生会館", "postal_code": "1028564", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒラカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028464','{"jis": "13101", "kana": "ゼンニホンジチダンタイ ロウドウクミアイ", "name": "全日本自治団体　労働組合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "六番町", "banchi": "1", "postal_code": "1028464", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ロクバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028795','{"jis": "13101", "kana": "ソウムシヨウ カントウソウゴウツウシンキヨク", "name": "総務省　関東総合通信局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "1丁目2-1", "postal_code": "1028795", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028170','{"jis": "13101", "kana": "タカヤマコウギヨウ カブシキガイシヤ", "name": "高山工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "1丁目11-21", "postal_code": "1028170", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028430','{"jis": "13101", "kana": "ダイイチカサイカイジヨウホケン ソウゴガイシヤ", "name": "第一火災海上保険　相互会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "5-1", "postal_code": "1028430", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028175','{"jis": "13101", "kana": "ダイダン カブシキガイシヤ トウキヨウホンシヤ", "name": "ダイダン　株式会社　東京本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目15-10", "postal_code": "1028175", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028730','{"jis": "13101", "kana": "ダイトロン カブシキガイシヤ", "name": "ダイトロン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "3丁目6番地住友不動産麹町ビル3号館", "postal_code": "1028730", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
@@ -126110,15 +126113,15 @@
 INSERT INTO office_data VALUES('1038689','{"jis": "13102", "kana": "スルガギンコウ カブシキガイシヤ トウキヨウシテン", "name": "スルガ銀行　株式会社　東京支店", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "1丁目7-1(日本橋郵便局私書箱第59号)", "postal_code": "1038689", "old_code": "103  ", "post_office": "日本橋", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1038351','{"jis": "13102", "kana": "ゼリアシンヤクコウギヨウ (カブ)", "name": "ゼリア新薬工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋小舟町", "banchi": "10-11", "postal_code": "1038351", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシコブナチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038473','{"jis": "13102", "kana": "ゼリアシンヤクコウギヨウ カブシキガイシヤ トウキヨウシテン", "name": "ゼリア新薬工業　株式会社　東京支店", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋小舟町", "banchi": "10-6", "postal_code": "1038473", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシコブナチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038212','{"jis": "13102", "kana": "ゼンコクケイザイジギヨウキヨウドウクミアイ", "name": "全国経済事業協同組合連合会", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋茅場町", "banchi": "2丁目8-4", "postal_code": "1038212", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカヤバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038506','{"jis": "13102", "kana": "ゼンコクケンセツコウジギヨウコクミンケンコウホケンクミアイ", "name": "全国建設工事業国民健康保険組合", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋箱崎町", "banchi": "12-4", "postal_code": "1038506", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシハコザキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038346','{"jis": "13102", "kana": "ゼンコクシヤカイホケンロウムシカイレンゴウカイ", "name": "全国社会保険労務士会連合会", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本石町", "banchi": "3丁目2-12", "postal_code": "1038346", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンゴクチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038347','{"jis": "13102", "kana": "ゼンコクシヤカイホケンロウムシカイレンゴウカイ シヤカイホケンロウムシシケンセンタ-", "name": "全国社会保険労務士会連合会　社会保険労務士試験センター", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本石町", "banchi": "3丁目2-12", "postal_code": "1038347", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンゴクチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1038366','{"jis": "13102", "kana": "ソダコウリヨウ カブシキガイシヤ", "name": "曽田香料　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋馬喰町", "banchi": "1-12-3", "postal_code": "1038366", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシバクロチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1038366','{"jis": "13102", "kana": "ソダコウリヨウ カブシキガイシヤ", "name": "曽田香料　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋馬喰町", "banchi": "1-12-3", "postal_code": "1038366", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシバクロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038501','{"jis": "13102", "kana": "ソフトバンク (カブ)", "name": "ソフトバンク　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋箱崎町", "banchi": "24-1", "postal_code": "1038501", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシハコザキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038255','{"jis": "13102", "kana": "ソンガイホケンジヤパンニツポンコウア カブシキガイシヤ", "name": "損害保険ジャパン日本興亜　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "2丁目2-10", "postal_code": "1038255", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038235','{"jis": "13102", "kana": "タカシマヤクレジツト カブシキガイシヤ", "name": "高島屋クレジット　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋茅場町", "banchi": "2-12-7高栄茅場町ビル", "postal_code": "1038235", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカヤバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038218','{"jis": "13102", "kana": "タカシマヤスペ-スクリエイツ カブシキガイシヤ", "name": "高島屋スペースクリエイツ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "2丁目12番10号", "postal_code": "1038218", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038232','{"jis": "13102", "kana": "タカラシユゾウ カブシキガイシヤ シユトケンシシヤ", "name": "宝酒造　株式会社　首都圏支社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "2丁目15-10", "postal_code": "1038232", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038668','{"jis": "13102", "kana": "タケダヤクヒンコウギヨウ カブシキガイシヤ", "name": "武田薬品工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "2丁目1-1(日本橋郵便局私書箱第41号)", "postal_code": "1038668", "old_code": "103  ", "post_office": "日本橋", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038206','{"jis": "13102", "kana": "タナカキキンゾクコウギヨウ (カブ)", "name": "田中貴金属工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋茅場町", "banchi": "2丁目6-6", "postal_code": "1038206", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカヤバチョウ", "alternates": []}');
@@ -126129,15 +126132,15 @@
 INSERT INTO office_data VALUES('1038511','{"jis": "13102", "kana": "ダイトウボウ カブシキガイシヤ", "name": "ダイトウボウ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "1-6-1丸柏タマビル7階", "postal_code": "1038511", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038383','{"jis": "13102", "kana": "ダイニチセイカコウギヨウ (カブ)", "name": "大日精化工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋馬喰町", "banchi": "1丁目7-6", "postal_code": "1038383", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシバクロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038240','{"jis": "13102", "kana": "ダイワセイカン (カブ)", "name": "大和製罐　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "2丁目1-10", "postal_code": "1038240", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038324','{"jis": "13102", "kana": "チユウガイセイヤク カブシキガイシヤ", "name": "中外製薬　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "2丁目1-1日本橋三井タワー15F", "postal_code": "1038324", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1038404','{"jis": "13102", "kana": "ツカモト (カブ)", "name": "ツカモト　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "1丁目6-5", "postal_code": "1038404", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038423','{"jis": "13102", "kana": "デイ-エムミツイセイトウ カブシキガイシヤ", "name": "ＤＭ三井製糖　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋箱崎町", "banchi": "36-2Daiwaリバーゲート12階", "postal_code": "1038423", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシハコザキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038233','{"jis": "13102", "kana": "デイアイシ- カブシキガイシヤ", "name": "ＤＩＣ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "3丁目7-20", "postal_code": "1038233", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
-INSERT INTO office_data VALUES('1038338','{"jis": "13102", "kana": "デンカ カブシキカイシヤ", "name": "デンカ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "二丁目1番1号", "postal_code": "1038338", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
+INSERT INTO office_data VALUES('1038338','{"jis": "13102", "kana": "デンカ カブシキカイシヤ", "name": "デンカ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "二丁目1番1号", "postal_code": "1038338", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1038566','{"jis": "13102", "kana": "デンヨ- カブシキガイシヤ", "name": "デンヨー　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋堀留町", "banchi": "2丁目8-5", "postal_code": "1038566", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホリドメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038554','{"jis": "13102", "kana": "トウキヨウオリモノケンコウホケンクミアイ", "name": "東京織物健康保険組合", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋堀留町", "banchi": "1丁目9-6", "postal_code": "1038554", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホリドメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038465','{"jis": "13102", "kana": "トウキヨウジツギヨウケンコウホケンクミアイ", "name": "東京実業健康保険組合", "prefecture": "東京都", "city": "中央区", "neighborhood": "東日本橋", "banchi": "3丁目10-4", "postal_code": "1038465", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヒガシニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038285','{"jis": "13102", "kana": "トウキヨウタテモノ カブシキガイシヤ", "name": "東京建物　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "1丁目4番16号", "postal_code": "1038285", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
 INSERT INTO office_data VALUES('1038360','{"jis": "13102", "kana": "トウキヨウトニホンバシトクベツシユツチヨウジヨ", "name": "東京都中央区日本橋特別出張所", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋蛎殻町", "banchi": "1丁目31-1", "postal_code": "1038360", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカキガラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038407','{"jis": "13102", "kana": "トウヨウケミカルズ (カブ)", "name": "東洋ケミカルズ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "4丁目5-16", "postal_code": "1038407", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038584','{"jis": "13102", "kana": "トスコ (カブ)", "name": "トスコ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋人形町", "banchi": "1丁目1-10", "postal_code": "1038584", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシニンギョウチョウ", "alternates": []}');
@@ -126370,24 +126373,24 @@
 INSERT INTO office_data VALUES('1048378','{"jis": "13102", "kana": "トウヨウインキ カブシキガイシヤ", "name": "東洋インキ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目2-1", "postal_code": "1048378", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048377','{"jis": "13102", "kana": "トウヨウインキエスシ-ホ-ルデイングス カブシキガイシヤ", "name": "東洋インキＳＣホールディングス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目2-1", "postal_code": "1048377", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048678','{"jis": "13102", "kana": "トウヨウシヨウケン カブシキガイシヤ", "name": "東洋証券　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八丁堀", "banchi": "4丁目7番1号(晴海郵便局私書箱第15号)", "postal_code": "1048678", "old_code": "104  ", "post_office": "晴海", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハッチョウボリ", "alternates": []}');
 INSERT INTO office_data VALUES('1048324','{"jis": "13102", "kana": "トウヨウネツコウギヨウ カブシキガイシヤ", "name": "東洋熱工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目5番12号", "postal_code": "1048324", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048345','{"jis": "13102", "kana": "トウヨウボウ カブシキガイシヤ", "name": "東洋紡　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "1丁目17番10号住友商事京橋ビル", "postal_code": "1048345", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048388','{"jis": "13102", "kana": "トダケンセツ カブシキガイシヤ", "name": "戸田建設　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八丁堀", "banchi": "2-8-5", "postal_code": "1048388", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハッチョウボリ", "alternates": []}');
 INSERT INTO office_data VALUES('1048416','{"jis": "13102", "kana": "トリンプ・インタ-ナシヨナル・ジヤパン カブシキガイシヤ", "name": "トリンプ・インターナショナル・ジャパン　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "5-6-4浜離宮三井ビルディング", "postal_code": "1048416", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
-INSERT INTO office_data VALUES('1048112','{"jis": "13102", "kana": "ドクリツギヨウセイホウジン ニホンガクセイシエンキコウ", "name": "独立行政法人　日本学生支援機構", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "6-18-2野村不動産銀座ビル", "postal_code": "1048112", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": true, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
+INSERT INTO office_data VALUES('1048112','{"jis": "13102", "kana": "ドクリツギヨウセイホウジン ニホンガクセイシエンキコウ", "name": "独立行政法人　日本学生支援機構", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "6-18-2野村不動産銀座ビル", "postal_code": "1048112", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048530','{"jis": "13102", "kana": "ナラサキサンギヨウ カブシキガイシヤ", "name": "ナラサキ産業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "入船", "banchi": "3-3-8ヒューリック築地イーストビル", "postal_code": "1048530", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "イリフネ", "alternates": []}');
 INSERT INTO office_data VALUES('1048555','{"jis": "13102", "kana": "ニチアス カブシキガイシヤ", "name": "ニチアス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八丁堀", "banchi": "1丁目6番1号", "postal_code": "1048555", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハッチョウボリ", "alternates": []}');
 INSERT INTO office_data VALUES('1048424','{"jis": "13102", "kana": "ニツカンスポ-ツシユツパンシヤ", "name": "日刊スポーツ出版社", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "3-5-10", "postal_code": "1048424", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048444','{"jis": "13102", "kana": "ニツシヨウエレクトロニクス カブシキガイシヤ", "name": "日商エレクトロニクス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "7丁目3-1", "postal_code": "1048444", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048285','{"jis": "13102", "kana": "ニツシンオイリオグル-プ カブシキガイシヤ", "name": "日清オイリオグループ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "1丁目23-1", "postal_code": "1048285", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048556','{"jis": "13102", "kana": "ニツセイドウワソンガイホケン カブシキガイシヤ", "name": "ニッセイ同和損害保険　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "明石町", "banchi": "8-1", "postal_code": "1048556", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "アカシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1048406','{"jis": "13102", "kana": "ニツツウシヨウジ カブシキガイシヤ", "name": "日通商事　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "5丁目6-10", "postal_code": "1048406", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048167','{"jis": "13102", "kana": "ニツポウ カブシキガイシヤ", "name": "日放　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "6丁目17番2号(日産ビルネット館-2)", "postal_code": "1048167", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
-INSERT INTO office_data VALUES('1048175','{"jis": "13102", "kana": "ニツポンネンキンキコウ チユウオウネンキンジムシヨ", "name": "日本年金機構　中央年金事務所", "prefecture": "東京都", "city": "中央区", "neighborhood": "明石町", "banchi": "8-1聖路加タワー1階・16階", "postal_code": "1048175", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "アカシチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1048175','{"jis": "13102", "kana": "ニツポンネンキンキコウ チユウオウネンキンジムシヨ", "name": "日本年金機構　中央年金事務所", "prefecture": "東京都", "city": "中央区", "neighborhood": "明石町", "banchi": "8-1聖路加タワー1階・16階", "postal_code": "1048175", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "アカシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1048365','{"jis": "13102", "kana": "ニツポンヤキンコウギヨウ カブシキガイシヤ", "name": "日本冶金工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "1丁目5-8", "postal_code": "1048365", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048656','{"jis": "13102", "kana": "ニホンカミパルプシヨウジ カブシキガイシヤ", "name": "日本紙パルプ商事　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "勝どき", "banchi": "3-12-1フォアフロントタワー", "postal_code": "1048656", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "カチドキ", "alternates": []}');
 INSERT INTO office_data VALUES('1048401','{"jis": "13102", "kana": "ニホンカンザイセンタ- カブシキガイシヤ", "name": "日本管材センター　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八丁堀", "banchi": "2-24-3", "postal_code": "1048401", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハッチョウボリ", "alternates": []}');
 INSERT INTO office_data VALUES('1048559','{"jis": "13102", "kana": "ニホンシユルイハンバイ カブシキガイシヤ", "name": "日本酒類販売　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "勝どき", "banchi": "3丁目4-13", "postal_code": "1048559", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "カチドキ", "alternates": []}');
 INSERT INTO office_data VALUES('1048254','{"jis": "13102", "kana": "ニホンシユルイハンバイ カブシキガイシヤ", "name": "日本酒類販売　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "1丁目25番4号", "postal_code": "1048254", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048257','{"jis": "13102", "kana": "ニホンジユウカガクコウギヨウ カブシキガイシヤ", "name": "日本重化学工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "1丁目17-25", "postal_code": "1048257", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048386','{"jis": "13102", "kana": "ニホンノウヤク カブシキガイシヤ", "name": "日本農薬　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "1丁目19番8号京橋OMビル", "postal_code": "1048386", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
@@ -126398,15 +126401,15 @@
 INSERT INTO office_data VALUES('1048205','{"jis": "13102", "kana": "フクトクチヨウシユルイ カブシキガイシヤ", "name": "福徳長酒類　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "6丁目2-10", "postal_code": "1048205", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048122','{"jis": "13102", "kana": "フジカサイカイジヨウホケン カブシキガイシヤ", "name": "富士火災海上保険　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "2丁目12-18", "postal_code": "1048122", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048523','{"jis": "13102", "kana": "フジデンキアイテイソリユ-シヨン カブシキガイシヤ", "name": "富士電機ＩＴソリューション　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八丁堀", "banchi": "2丁目20-8", "postal_code": "1048523", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハッチョウボリ", "alternates": []}');
 INSERT INTO office_data VALUES('1048521','{"jis": "13102", "kana": "フジデンキソウセツ カブシキガイシヤ", "name": "富士電機総設　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八丁堀", "banchi": "2丁目20-8東急ビル", "postal_code": "1048521", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハッチョウボリ", "alternates": []}');
 INSERT INTO office_data VALUES('1048351','{"jis": "13102", "kana": "マエザワコウギヨウ カブシキガイシヤ", "name": "前澤工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "1丁目5-17", "postal_code": "1048351", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048281','{"jis": "13102", "kana": "マツイケンセツ カブシキカイシヤ", "name": "松井建設　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "1丁目17-22", "postal_code": "1048281", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048502','{"jis": "13102", "kana": "マルゼンセキユカガク カブシキガイシヤ", "name": "丸善石油化学　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "入船", "banchi": "2丁目1番1号", "postal_code": "1048502", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "イリフネ", "alternates": []}');
-INSERT INTO office_data VALUES('1048481','{"jis": "13102", "kana": "ミズホシヨウケン カブシキガイシヤ", "name": "みずほ証券　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "2丁目1番1号YANMARTOKYO10階", "postal_code": "1048481", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
+INSERT INTO office_data VALUES('1048481','{"jis": "13102", "kana": "ミズホシヨウケン カブシキガイシヤ", "name": "みずほ証券　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "2丁目1番1号YANMARTOKYO10階", "postal_code": "1048481", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
 INSERT INTO office_data VALUES('1048546','{"jis": "13102", "kana": "ミツイスミシヨウケンザイ カブシキガイシヤ", "name": "三井住商建材　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "晴海", "banchi": "1丁目8番8号トリトンスクエアオフィスタワーW12・13階", "postal_code": "1048546", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハルミ", "alternates": []}');
 INSERT INTO office_data VALUES('1048258','{"jis": "13102", "kana": "ミツイスミトモカイジヨウアイオイセイメイホケン カブシキカイシヤ", "name": "三井住友海上あいおい生命保険　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "2-27-2", "postal_code": "1048258", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048252','{"jis": "13102", "kana": "ミツイスミトモカイジヨウカサイホケン カブシキガイシヤ", "name": "三井住友海上火災保険　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "新川", "banchi": "2丁目27-2", "postal_code": "1048252", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "シンカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1048439','{"jis": "13102", "kana": "ミツイゾウセン カブシキカイシヤ", "name": "三井造船　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "5丁目6番4号", "postal_code": "1048439", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048550','{"jis": "13102", "kana": "ミツビシセイコウ カブシキガイシヤ", "name": "三菱製鋼　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "月島", "banchi": "4丁目16番13号Daiwa月島ビル4階", "postal_code": "1048550", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキシマ", "alternates": []}');
 INSERT INTO office_data VALUES('1048002','{"jis": "13102", "kana": "メイジ セイカ フアルマ カブシキガイシヤ", "name": "Ｍｅｉｊｉ　Ｓｅｉｋａ　ファルマ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目4番16号", "postal_code": "1048002", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048125','{"jis": "13102", "kana": "ヤマトウンユ カブシキガイシヤ", "name": "ヤマト運輸　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "2丁目16番10号", "postal_code": "1048125", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
@@ -126459,15 +126462,14 @@
 INSERT INTO office_data VALUES('1058320','{"jis": "13103", "kana": "カブシキガイシヤ キヨウワキカク", "name": "株式会社　協和企画", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "1-10-5日土地虎ノ門ビル", "postal_code": "1058320", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058468','{"jis": "13103", "kana": "カブシキガイシヤ グルメキネヤ トウキヨウシシヤ", "name": "株式会社　グルメ杵屋　東京支社", "prefecture": "東京都", "city": "港区", "neighborhood": "浜松町", "banchi": "2丁目13-10", "postal_code": "1058468", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ハママツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1058318','{"jis": "13103", "kana": "カブシキガイシヤ コウサイドウホ-ルデイングス", "name": "株式会社　広済堂ホールディングス", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目2番3号シーバンスS館", "postal_code": "1058318", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1058475','{"jis": "13103", "kana": "カブシキガイシヤ コウボガイドシヤ", "name": "株式会社　公募ガイド社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝公園", "banchi": "1-8-21芝公園リッジビル5階", "postal_code": "1058475", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバコウエン", "alternates": []}');
 INSERT INTO office_data VALUES('1058642','{"jis": "13103", "kana": "カブシキガイシヤ コシダテツク", "name": "株式会社　コシダテック", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "2丁目2-9", "postal_code": "1058642", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058670','{"jis": "13103", "kana": "カブシキガイシヤ ゴルフダイジエストシヤ", "name": "株式会社　ゴルフダイジェスト社", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "6丁目18-5", "postal_code": "1058670", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058310','{"jis": "13103", "kana": "カブシキガイシヤ シセイドウ", "name": "株式会社　資生堂", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目6-2", "postal_code": "1058310", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
-INSERT INTO office_data VALUES('1058688','{"jis": "13103", "kana": "カブシキガイシヤ シヨウセンミツイ", "name": "株式会社　商船三井", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "2丁目1-1(芝郵便局私書箱第5号)", "postal_code": "1058688", "old_code": "105  ", "post_office": "芝", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058335','{"jis": "13103", "kana": "カブシキガイシヤ ジエイテイ-ビ-コミユニケ-シヨンデザイン", "name": "株式会社　ＪＴＢコミュニケーションデザイン", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3丁目23番1号セレスティン芝三井ビルディング12階", "postal_code": "1058335", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058407','{"jis": "13103", "kana": "カブシキガイシヤ ジヤパンエナジ-", "name": "（株）　ジャパンエナジー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "2丁目10-1", "postal_code": "1058407", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1056050','{"jis": "13103", "kana": "カブシキガイシヤ スタ-・チヤンネル", "name": "株式会社　スター・チャンネル", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4-3-1城山トラストタワー23階", "postal_code": "1056050", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058415','{"jis": "13103", "kana": "カブシキガイシヤ ソニ-・ピクチヤ-ズエンタテインメント", "name": "株式会社　ソニー・ピクチャーズエンタテインメント", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目1-28虎ノ門タワーズオフィス", "postal_code": "1058415", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058658','{"jis": "13103", "kana": "カブシキガイシヤ ダイコウ", "name": "株式会社　大広", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "2丁目14-5", "postal_code": "1058658", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058656','{"jis": "13103", "kana": "カブシキガイシヤ ダイコウウイドウ", "name": "株式会社　大広ＷＥＤＯ", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "2丁目14-5", "postal_code": "1058656", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058505','{"jis": "13103", "kana": "カブシキガイシヤ テイチクエンタテインメント", "name": "株式会社　テイチクエンタテインメント", "prefecture": "東京都", "city": "港区", "neighborhood": "芝公園", "banchi": "2-4-1芝パークビルB館8F", "postal_code": "1058505", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバコウエン", "alternates": []}');
@@ -126580,14 +126582,15 @@
 INSERT INTO office_data VALUES('1058681','{"jis": "13103", "kana": "ニツポンケイキンゾクグル-プ", "name": "日本軽金属グループ", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "1丁目1番13号アーバンネット内幸町ビル", "postal_code": "1058681", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058322','{"jis": "13103", "kana": "ニツポンツウウン カブシキガイシヤ", "name": "日本通運　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目9-3", "postal_code": "1058322", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058540','{"jis": "13103", "kana": "ニツポンデンキ カブシキガイシヤ セレステインビル", "name": "日本電気　株式会社　セレスティンビル", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3-23-1セレスティン芝三井ビルディング", "postal_code": "1058540", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058456','{"jis": "13103", "kana": "ニツポンポラロイド カブシキガイシヤ", "name": "日本ポラロイド　（株）", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "3丁目18-19虎ノ門マリンビル", "postal_code": "1058456", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058617','{"jis": "13103", "kana": "ニツポンユウセイ カブシキガイシヤ シユクハクジギヨウブ", "name": "日本郵政　株式会社　宿泊事業部", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "6-19-15", "postal_code": "1058617", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058788','{"jis": "13103", "kana": "ニツポンユウセイ カブシキガイシヤ シユトケンシセツセンタ-", "name": "日本郵政　株式会社　首都圏施設センター", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "3丁目17番1号TOKYUREIT虎ノ門ビル7階", "postal_code": "1058788", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058408','{"jis": "13103", "kana": "ニホンギジユツボウエキ カブシキガイシヤ", "name": "日本技術貿易　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目7-13虎ノ門イーストビルディング", "postal_code": "1058408", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
+INSERT INTO office_data VALUES('1058467','{"jis": "13103", "kana": "ニホンコクドカイハツ (カ)", "name": "日本国土開発　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目3-13ヒューリック神谷町ビル5F", "postal_code": "1058467", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058521','{"jis": "13103", "kana": "ニホンセキジユウジシヤ", "name": "日本赤十字社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝大門", "banchi": "1丁目1-3", "postal_code": "1058521", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバダイモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058508','{"jis": "13103", "kana": "ニホンタタ・コンサルタンシ-・サ-ビシズ カブシキガイシヤ", "name": "日本タタ・コンサルタンシー・サービシズ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝公園", "banchi": "4丁目1番4号", "postal_code": "1058508", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバコウエン", "alternates": []}');
 INSERT INTO office_data VALUES('1057444','{"jis": "13103", "kana": "ニホンテレビホウソウモウ カブシキガイシヤ", "name": "日本テレビ放送網　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目6-1", "postal_code": "1057444", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058457','{"jis": "13103", "kana": "ニホンデスコ カブシキガイシヤ", "name": "日本デスコ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目3-13秀和神谷町ビル", "postal_code": "1058457", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058578','{"jis": "13103", "kana": "ニホンビジネスシステムズ カブシキガイシヤ", "name": "日本ビジネスシステムズ　（株）", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3丁目8番2号芝公園ファーストビル13F", "postal_code": "1058578", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058579','{"jis": "13103", "kana": "ニホンマスタ-トラストシンタクギンコウ カブシキガイシヤ", "name": "日本マスタートラスト信託銀行　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "浜松町", "banchi": "2丁目11-3MTBJビル", "postal_code": "1058579", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ハママツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1058301','{"jis": "13103", "kana": "パナソニツク カブシキガイシヤ", "name": "パナソニック　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目5-1", "postal_code": "1058301", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
@@ -127078,15 +127081,16 @@
 INSERT INTO office_data VALUES('1608522','{"jis": "13104", "kana": "ジヨシガクセイカイカン <メイセン>", "name": "女子学生会館　「明泉」", "prefecture": "東京都", "city": "新宿区", "neighborhood": "南元町", "banchi": "6-2", "postal_code": "1608522", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ミナミモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1608512','{"jis": "13104", "kana": "セイカツキヨウドウクミアイ トウキヨウマイコ-プ", "name": "生活協同組合　東京マイコープ", "prefecture": "東京都", "city": "新宿区", "neighborhood": "四谷", "banchi": "4丁目28-7", "postal_code": "1608512", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヨツヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1630831','{"jis": "13104", "kana": "セントラルケイビホシヨウ カブシキガイシヤ", "name": "セントラル警備保障　（株）", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目4-1新宿NSビル", "postal_code": "1630831", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608361','{"jis": "13104", "kana": "ゼンケンホンシヤ カブシキガイシヤ", "name": "全研本社　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "6-18-1住友不動産新宿セントラルパークタワー18階・19階", "postal_code": "1608361", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608507','{"jis": "13104", "kana": "ゼンコクケンコウホケンキヨウカイ ホンブ", "name": "全国健康保険協会　本部", "prefecture": "東京都", "city": "新宿区", "neighborhood": "四谷", "banchi": "1丁目6番1号6階", "postal_code": "1608507", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヨツヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1608373','{"jis": "13104", "kana": "ゼンホレン カブシキガイシヤ", "name": "全保連　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-24-1エステック情報ビル16F", "postal_code": "1608373", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608583','{"jis": "13104", "kana": "ソウカガツカイ", "name": "創価学会", "prefecture": "東京都", "city": "新宿区", "neighborhood": "信濃町", "banchi": "32", "postal_code": "1608583", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シナノマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1608338','{"jis": "13104", "kana": "ソンガイホケンジヤパンニツポンコウア カブシキガイシヤ", "name": "損害保険ジャパン日本興亜　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1608338", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
+INSERT INTO office_data VALUES('1608313','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1608313", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": true, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
+INSERT INTO office_data VALUES('1608338','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1608338", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": true, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638626','{"jis": "13104", "kana": "ソンポジヤパンニツポンコウアヒマワリセイメイホケン カブシキガイシヤ", "name": "損保ジャパン日本興亜ひまわり生命保険　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "6丁目13番1号新宿セントラルパークビル(新宿郵便局私書箱第123号)", "postal_code": "1638626", "old_code": "160  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638639','{"jis": "13104", "kana": "タイセイヤツカコウギヨウ", "name": "大正薬化工業", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新宿", "banchi": "3丁目10-8(新宿郵便局私書箱第343号)", "postal_code": "1638639", "old_code": "160  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608401','{"jis": "13104", "kana": "ダイワシヨウケン カブシキガイシヤ シンジユクシテン", "name": "大和証券　株式会社　新宿支店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新宿", "banchi": "3丁目30-11", "postal_code": "1608401", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630663','{"jis": "13104", "kana": "ダイワシヨウケン カブシキガイシヤ シンジユクセンタ-ビルシテン", "name": "大和証券　株式会社　新宿センタービル支店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目25-1新宿センタービル", "postal_code": "1630663", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608327','{"jis": "13104", "kana": "チユウオウシヨクギヨウノウリヨクカイハツキヨウカイ", "name": "中央職業能力開発協会", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "7丁目5番25号西新宿木村屋ビルディング", "postal_code": "1608327", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1631053','{"jis": "13104", "kana": "トウキヨウガストシカイハツ カブシキガイシヤ", "name": "東京ガス都市開発　（株）", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3丁目7-1新宿パークタワー", "postal_code": "1631053", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630560','{"jis": "13104", "kana": "トウキヨウジツギヨウケンコウホケンクミアイ ジヨウサイシブ", "name": "東京実業健康保険組合　城西支部", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目26-2新宿野村ビル", "postal_code": "1630560", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
@@ -127154,15 +127158,14 @@
 INSERT INTO office_data VALUES('1618528','{"jis": "13104", "kana": "ジエイエ-ゼンノウタマゴ カブシキガイシヤ", "name": "ＪＡ全農たまご　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "中落合", "banchi": "2丁目7-1", "postal_code": "1618528", "old_code": "161  ", "post_office": "落合", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ナカオチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('1618567','{"jis": "13104", "kana": "トウキヨウニツサンモ-タ- カブシキガイシヤ マルヤマテン", "name": "東京日産モーター　株式会社　丸山店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西落合", "banchi": "2丁目1-12", "postal_code": "1618567", "old_code": "161  ", "post_office": "落合", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシオチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('1618560','{"jis": "13104", "kana": "ニホンコウデンコウギヨウ カブシキガイシヤ", "name": "日本光電工業　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西落合", "banchi": "1丁目31-4", "postal_code": "1618560", "old_code": "161  ", "post_office": "落合", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシオチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('1618539','{"jis": "13104", "kana": "メジロガクエン", "name": "目白学園", "prefecture": "東京都", "city": "新宿区", "neighborhood": "中落合", "banchi": "4丁目31-1", "postal_code": "1618539", "old_code": "161  ", "post_office": "落合", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ナカオチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('1618522','{"jis": "13104", "kana": "メジロケンシンチユウガツコウ・コウトウガツコウ", "name": "目白研心中学校・高等学校", "prefecture": "東京都", "city": "新宿区", "neighborhood": "中落合", "banchi": "4丁目31番1号", "postal_code": "1618522", "old_code": "161  ", "post_office": "落合", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ナカオチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('1618575','{"jis": "13104", "kana": "ヤチヨエンジニヤリング カブシキガイシヤ", "name": "八千代エンジニヤリング　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西落合", "banchi": "2丁目18-12", "postal_code": "1618575", "old_code": "161  ", "post_office": "落合", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシオチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('1618520','{"jis": "13104", "kana": "ライオンキカク カブシキガイシヤ", "name": "ライオン企画　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "中落合", "banchi": "1丁目6-12", "postal_code": "1618520", "old_code": "161  ", "post_office": "落合", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ナカオチアイ", "alternates": []}');
-INSERT INTO office_data VALUES('1628446','{"jis": "13104", "kana": "(カブ) ジエイテイ-ビ-パブリツシング", "name": "（株）　ＪＴＢパブリッシング", "prefecture": "東京都", "city": "新宿区", "neighborhood": "払方町", "banchi": "25-5", "postal_code": "1628446", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ハライカタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628415','{"jis": "13104", "kana": "アンステイチユ・フランセトウキヨウ", "name": "アンスティチュ・フランセ東京", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷船河原町", "banchi": "15", "postal_code": "1628415", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤフナガワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628616','{"jis": "13104", "kana": "イカロスシユツパン カブシキガイシヤ", "name": "イカロス出版　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷本村町", "banchi": "2-3", "postal_code": "1628616", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤホンムラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628707','{"jis": "13104", "kana": "カブシキガイシヤ アサクラシヨテン", "name": "株式会社　朝倉書店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新小川町", "banchi": "6-29", "postal_code": "1628707", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628535','{"jis": "13104", "kana": "カブシキガイシヤ アプラス", "name": "株式会社　アプラス", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新小川町", "banchi": "4-1アプラス東京ビル", "postal_code": "1628535", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628455','{"jis": "13104", "kana": "カブシキガイシヤ イダリヨウゴクドウ", "name": "株式会社　井田両国堂", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷本村町", "banchi": "1-1住友市ケ谷ビル", "postal_code": "1628455", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤホンムラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628680','{"jis": "13104", "kana": "カブシキガイシヤ オウブンシヤ", "name": "株式会社　旺文社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "横寺町", "banchi": "55", "postal_code": "1628680", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヨコテラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628716','{"jis": "13104", "kana": "カブシキガイシヤ オンガクノトモシヤ", "name": "株式会社　音楽之友社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "神楽坂", "banchi": "6丁目30", "postal_code": "1628716", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "カグラザカ", "alternates": []}');
@@ -127226,15 +127229,15 @@
 INSERT INTO office_data VALUES('1628636','{"jis": "13104", "kana": "ドクリツギヨウセイホウジン コクリツケンコウ・エイヨウケンキユウジヨ", "name": "独立行政法人　国立健康・栄養研究所", "prefecture": "東京都", "city": "新宿区", "neighborhood": "戸山", "banchi": "1丁目23-1", "postal_code": "1628636", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "トヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('1628412','{"jis": "13104", "kana": "ドクリツギヨウセイホウジン ニホンガクセイシエンキコウ", "name": "独立行政法人　日本学生支援機構", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷本村町", "banchi": "10-7", "postal_code": "1628412", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤホンムラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628407','{"jis": "13104", "kana": "ニホンホウキシユツパン カブシキガイシヤ", "name": "新日本法規出版　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷砂土原町", "banchi": "2丁目6", "postal_code": "1628407", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤサドハラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628861','{"jis": "13104", "kana": "ボウエイシセツチヨウ ナイブブキヨク", "name": "防衛施設庁　内部部局", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷本村町", "banchi": "5-1", "postal_code": "1628861", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤホンムラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628808','{"jis": "13104", "kana": "ボウエイシヨウボウエイケンキユウジヨ", "name": "防衛省防衛研究所", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷本村町", "banchi": "5-1", "postal_code": "1628808", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤホンムラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628451','{"jis": "13104", "kana": "モチダセイヤク カブシキガイシヤ ホンシヤベツカン", "name": "持田製薬　株式会社　本社別館", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷本村町", "banchi": "2-12", "postal_code": "1628451", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤホンムラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628422','{"jis": "13104", "kana": "リヨウデンエレベ-タシセツ カブシキガイシヤ", "name": "菱電エレベータ施設　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷砂土原町", "banchi": "2丁目4番地", "postal_code": "1628422", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤサドハラチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1628480','{"jis": "13104", "kana": "ワセダダイガク センタンセイメイイカガクセンタ-", "name": "早稲田大学　先端生命医科学センター", "prefecture": "東京都", "city": "新宿区", "neighborhood": "若松町", "banchi": "2-2", "postal_code": "1628480", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ワカマツチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1628480','{"jis": "13104", "kana": "ワセダダイガク センタンセイメイイカガクセンタ-", "name": "早稲田大学　先端生命医科学センター", "prefecture": "東京都", "city": "新宿区", "neighborhood": "若松町", "banchi": "2-2", "postal_code": "1628480", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ワカマツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628644','{"jis": "13104", "kana": "ワセダダイガク ダイイチブンガクブ", "name": "早稲田大学　第一文学部", "prefecture": "東京都", "city": "新宿区", "neighborhood": "戸山", "banchi": "1丁目24-1", "postal_code": "1628644", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "トヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('1628020','{"jis": "13104", "kana": "ワラベヤニチヨウ カブシキガイシヤ", "name": "わらべや日洋　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "富久町", "banchi": "13番19号", "postal_code": "1628020", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "トミヒサチョウ", "alternates": [{"jis": "13104", "kana": "ワラベヤニチヨウホ-ルデイングス カブシキガイシヤ", "name": "わらべや日洋ホールディングス　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "富久町", "banchi": "13番19号", "postal_code": "1628020", "old_code": "162  ", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "トミヒサチョウ", "alternates": []}]}');
 INSERT INTO office_data VALUES('1628001','{"jis": "13104", "kana": "ダイニツポンインサツ カブシキガイシヤ", "name": "大日本印刷　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷加賀町", "banchi": "1丁目1-1(牛込郵便局私書箱第75号)", "postal_code": "1628001", "old_code": "16201", "post_office": "牛込", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤカガチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628448','{"jis": "13104", "kana": "イツパンシヤダンホウジン イエノヒカリキヨウカイ", "name": "一般社団法人　家の光協会", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷船河原町", "banchi": "11", "postal_code": "1628448", "old_code": "16208", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤフナガワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628558','{"jis": "13104", "kana": "カブシキガイシヤ アスク", "name": "株式会社　アスク", "prefecture": "東京都", "city": "新宿区", "neighborhood": "下宮比町", "banchi": "2-6", "postal_code": "1628558", "old_code": "16208", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シモミヤビチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628476','{"jis": "13104", "kana": "カブシキガイシヤ インテリジエンス", "name": "株式会社　インテリジェンス", "prefecture": "東京都", "city": "新宿区", "neighborhood": "市谷田町", "banchi": "1丁目18", "postal_code": "1628476", "old_code": "16208", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "イチガヤタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628515','{"jis": "13104", "kana": "カブシキガイシヤ ゲンダイシヨリン", "name": "株式会社　現代書林", "prefecture": "東京都", "city": "新宿区", "neighborhood": "原町", "banchi": "3丁目61桂ビル", "postal_code": "1628515", "old_code": "16208", "post_office": "牛込", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ハラマチ", "alternates": []}');
@@ -127256,14 +127259,15 @@
 INSERT INTO office_data VALUES('1628717','{"jis": "13104", "kana": "カブシキガイシヤ ガクブンシヤ", "name": "株式会社　学文社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "早稲田町", "banchi": "5-4(牛込郵便局私書箱第77号)", "postal_code": "1628717", "old_code": "16291", "post_office": "牛込", "type": "box", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ワセダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628718','{"jis": "13104", "kana": "カブシキガイシヤ ガクブンシヤ", "name": "株式会社　学文社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "早稲田町", "banchi": "5-4(牛込郵便局私書箱第77号)", "postal_code": "1628718", "old_code": "16291", "post_office": "牛込", "type": "box", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ワセダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1628711','{"jis": "13104", "kana": "カブシキガイシヤ シンチヨウシヤ", "name": "株式会社　新潮社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "矢来町", "banchi": "71(牛込郵便局私書箱第20号)", "postal_code": "1628711", "old_code": "16291", "post_office": "牛込", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヤライチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1628710','{"jis": "13104", "kana": "カブシキガイシヤ ト-ハン", "name": "株式会社　トーハン", "prefecture": "東京都", "city": "新宿区", "neighborhood": "東五軒町", "banchi": "6-24(牛込郵便局私書箱第5号)", "postal_code": "1628710", "old_code": "16291", "post_office": "牛込", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヒガシゴケンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1631537','{"jis": "13104", "kana": "エムエステイホケンサ-ビス (カ", "name": "エムエスティ保険サービス　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-6-1新宿エルタワー10階", "postal_code": "1631537", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630553','{"jis": "13104", "kana": "ケ-オ-デンタル カブシキカイシヤ", "name": "ケーオーデンタル　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-2新宿野村ビル19階(新宿野村ビル内郵便局私書箱第3074号)", "postal_code": "1630553", "old_code": "163  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630287','{"jis": "13104", "kana": "シホウシヨシホウジン チユウオウジムシヨ", "name": "司法書士法人　中央事務所", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2-6-1新宿住友ビル16階", "postal_code": "1630287", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
+INSERT INTO office_data VALUES('1638620','{"jis": "13104", "kana": "ソンガイホケンジヤパン カブシキガイシヤ", "name": "損害保険ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-1", "postal_code": "1638620", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": true, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630261','{"jis": "13104", "kana": "ヒカリビジネスフオ-ム カブシキガイシヤ", "name": "光ビジネスフォーム　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目6番1号新宿住友ビル19階", "postal_code": "1630261", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638019','{"jis": "13104", "kana": "ヒガシニホンデンシンデンワ カブシキカイシヤ", "name": "東日本電信電話　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3-19-2", "postal_code": "1638019", "old_code": "163  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638602','{"jis": "13104", "kana": "ミツビシユ-エフジエイシンタクギンコウ カブシキガイシヤ シンジユクシテン", "name": "三菱ＵＦＪ信託銀行　株式会社　新宿支店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-10-2(新宿郵便局私書箱第227号)", "postal_code": "1638602", "old_code": "163  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630575','{"jis": "13104", "kana": "スミコウジユンカツザイ カブシキガイシヤ", "name": "住鉱潤滑剤　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1-26-2新宿野村ビル14階", "postal_code": "1630575", "old_code": "16305", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630570','{"jis": "13104", "kana": "リ-ドエグジビシヨンジヤパン カブシキガイシヤ", "name": "リードエグジビションジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目26-2新宿野村ビル", "postal_code": "1630570", "old_code": "16305", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630727','{"jis": "13104", "kana": "セキスイカセイヒンコウギヨウ カブシキガイシヤ トウキヨウホンブ", "name": "積水化成品工業　株式会社　東京本部", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目7-1小田急第一生命ビル", "postal_code": "1630727", "old_code": "16306", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630655','{"jis": "13104", "kana": "テイ-ビイ-シ-グル-プ カブシキガイシヤ", "name": "ＴＢＣグループ　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目25-1新宿センタービル43F", "postal_code": "1630655", "old_code": "16306", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
@@ -127848,14 +127852,15 @@
 INSERT INTO office_data VALUES('1358717','{"jis": "13108", "kana": "カブシキガイシヤ オ-トバツクスセブン", "name": "株式会社　オートバックスセブン", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5丁目6番52号", "postal_code": "1358717", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358567','{"jis": "13108", "kana": "カブシキガイシヤ クメセツケイ", "name": "株式会社　久米設計", "prefecture": "東京都", "city": "江東区", "neighborhood": "潮見", "banchi": "2丁目1-22", "postal_code": "1358567", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358659','{"jis": "13108", "kana": "カブシキガイシヤ コツクス", "name": "株式会社　コックス", "prefecture": "東京都", "city": "江東区", "neighborhood": "新大橋", "banchi": "1丁目8-11三井生命新大橋ビル", "postal_code": "1358659", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンオオハシ", "alternates": []}');
 INSERT INTO office_data VALUES('1358402','{"jis": "13108", "kana": "カブシキガイシヤ ザ マイラ", "name": "株式会社　ザ　マイラ", "prefecture": "東京都", "city": "江東区", "neighborhood": "佐賀", "banchi": "1丁目1-14", "postal_code": "1358402", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "サガ", "alternates": []}');
 INSERT INTO office_data VALUES('1358670','{"jis": "13108", "kana": "カブシキガイシヤ システムソフト トウキヨウセンタ-", "name": "株式会社　システムソフト　東京センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "潮見", "banchi": "2丁目10-24", "postal_code": "1358670", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358303','{"jis": "13108", "kana": "カブシキガイシヤ シモダ", "name": "株式会社　シモダ", "prefecture": "東京都", "city": "江東区", "neighborhood": "森下", "banchi": "3丁目8-11", "postal_code": "1358303", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "モリシタ", "alternates": []}');
 INSERT INTO office_data VALUES('1358668','{"jis": "13108", "kana": "カブシキガイシヤ ジエイ・スポ-ツ", "name": "株式会社　ジェイ・スポーツ", "prefecture": "東京都", "city": "江東区", "neighborhood": "青海", "banchi": "2-5-10テレコムセンタービル20F", "postal_code": "1358668", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アオミ", "alternates": []}');
+INSERT INTO office_data VALUES('1358165','{"jis": "13108", "kana": "カブシキガイシヤ ジエイテイビ-パブリツシング", "name": "株式会社　ＪＴＢパブリッシング", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5-6-36豊洲プライムスクエア11階", "postal_code": "1358165", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358451','{"jis": "13108", "kana": "カブシキガイシヤ ジエイピ-ビジネスサ-ビス", "name": "株式会社　ＪＰビジネスサービス", "prefecture": "東京都", "city": "江東区", "neighborhood": "深川", "banchi": "2丁目2-18", "postal_code": "1358451", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "フカガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1008666','{"jis": "13108", "kana": "カブシキガイシヤ スポ-ツニツポンシンブンシヤ", "name": "株式会社　スポーツニッポン新聞社", "prefecture": "東京都", "city": "江東区", "neighborhood": "越中島", "banchi": "2丁目1-30(銀座郵便局私書箱第277号)", "postal_code": "1008666", "old_code": "135  ", "post_office": "銀座", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エッチュウジマ", "alternates": []}');
 INSERT INTO office_data VALUES('1358555','{"jis": "13108", "kana": "カブシキガイシヤ タキネツト", "name": "株式会社　タキネット", "prefecture": "東京都", "city": "江東区", "neighborhood": "新大橋", "banchi": "2丁目13-4", "postal_code": "1358555", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンオオハシ", "alternates": []}');
 INSERT INTO office_data VALUES('1358461','{"jis": "13108", "kana": "カブシキガイシヤ ダイワソウケン トウキヨウセンタ-", "name": "株式会社　大和総研　東京センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "1丁目14-6大和永代ビル", "postal_code": "1358461", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
 INSERT INTO office_data VALUES('1358460','{"jis": "13108", "kana": "カブシキガイシヤ ダイワソウケン ホンシヤ", "name": "株式会社　大和総研　本社", "prefecture": "東京都", "city": "江東区", "neighborhood": "冬木", "banchi": "15-6", "postal_code": "1358460", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "フユキ", "alternates": []}');
 INSERT INTO office_data VALUES('1358150','{"jis": "13108", "kana": "カブシキガイシヤ チユウオウコンピユ-タシステム", "name": "株式会社　中央コンピュータシステム", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "6丁目4番34号メブクス豊洲", "postal_code": "1358150", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358502','{"jis": "13108", "kana": "カブシキガイシヤ トウシバパ-ソナルアンドクライアントソリユ-シヨンシヤ", "name": "株式会社　東芝パーソナル＆クライアントソリューション社", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5丁目6番15号", "postal_code": "1358502", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
@@ -128042,14 +128047,15 @@
 INSERT INTO office_data VALUES('1408522','{"jis": "13109", "kana": "イリヨウホウジンシヤダンミドリノカイ トウキヨウシナガワビヨウイン", "name": "医療法人社団緑野会　東京品川病院", "prefecture": "東京都", "city": "品川区", "neighborhood": "東大井", "banchi": "6-3-22", "postal_code": "1408522", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408547','{"jis": "13109", "kana": "インタ-ワイヤ-ド カブシキガイシヤ", "name": "インターワイヤード　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "5丁目19-8", "postal_code": "1408547", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408688','{"jis": "13109", "kana": "オキデンキコウジ カブシキガイシヤ", "name": "沖電気工事　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "北品川", "banchi": "1丁目19-4", "postal_code": "1408688", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "キタシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408511','{"jis": "13109", "kana": "カブシキカイシヤ ニツセイコム", "name": "株式会社　ニッセイコム", "prefecture": "東京都", "city": "品川区", "neighborhood": "大井", "banchi": "1丁目47-1", "postal_code": "1408511", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "オオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408572','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシングル-プ", "name": "株式会社　日立製作所　情報・通信グループ", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6丁目27-18日立大森第二別館", "postal_code": "1408572", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408573','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシングル-プ", "name": "株式会社　日立製作所　情報・通信グループ", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6丁目26-2大森ベルポートB館", "postal_code": "1408573", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408512','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシンシステムシヤ", "name": "株式会社　日立製作所　情報・通信システム社", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6-23-1日立大森ビル", "postal_code": "1408512", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
+INSERT INTO office_data VALUES('1408574','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨデジタルシステムアンドサ-ビストウカツホンブ", "name": "株式会社　日立製作所デジタルシステム＆サービス統括本部", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "六丁目26-1大森ベルポートA館", "postal_code": "1408574", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408619','{"jis": "13109", "kana": "カブシキガイシヤ アクセスコクサイネツトワ-ク", "name": "株式会社　アクセス国際ネットワーク", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目4番11号野村不動産天王洲ビル", "postal_code": "1408619", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408630','{"jis": "13109", "kana": "カブシキガイシヤ ウエツクス", "name": "株式会社　ＵＥＸ", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目2-24", "postal_code": "1408630", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408702','{"jis": "13109", "kana": "カブシキガイシヤ カツマタデンキセイサクジヨ", "name": "株式会社　勝亦電機製作所", "prefecture": "東京都", "city": "品川区", "neighborhood": "北品川", "banchi": "4-10-9", "postal_code": "1408702", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "キタシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408538','{"jis": "13109", "kana": "カブシキガイシヤ カトウセイサクシヨ", "name": "株式会社　加藤製作所", "prefecture": "東京都", "city": "品川区", "neighborhood": "東大井", "banchi": "1丁目9-37", "postal_code": "1408538", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408614','{"jis": "13109", "kana": "カブシキガイシヤ コスモトレ-ドアンドサ-ビス", "name": "株式会社　コスモトレード＆サービス", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目5-8", "postal_code": "1408614", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408678','{"jis": "13109", "kana": "カブシキガイシヤ コニシデンキ", "name": "株式会社　古西電機", "prefecture": "東京都", "city": "品川区", "neighborhood": "南品川", "banchi": "2丁目16-6", "postal_code": "1408678", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408611','{"jis": "13109", "kana": "カブシキガイシヤ サンゲツ トウキヨウテン", "name": "株式会社　サンゲツ　東京店", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "3丁目20-17", "postal_code": "1408611", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
@@ -129702,15 +129708,15 @@
 INSERT INTO office_data VALUES('1948577','{"jis": "13209", "kana": "ホ-チキ カブシキガイシヤ マチダジギヨウシヨ", "name": "ホーチキ　株式会社　町田事業所", "prefecture": "東京都", "city": "町田市", "neighborhood": "南町田", "banchi": "3丁目7番1号", "postal_code": "1948577", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ミナミマチダ", "alternates": []}');
 INSERT INTO office_data VALUES('1948520','{"jis": "13209", "kana": "マチダシヤクシヨ", "name": "町田市役所", "prefecture": "東京都", "city": "町田市", "neighborhood": "森野", "banchi": "2-2-22", "postal_code": "1948520", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "モリノ", "alternates": []}');
 INSERT INTO office_data VALUES('1948580','{"jis": "13209", "kana": "マチダシヤクシヨ シミンカ", "name": "町田市役所　市民課", "prefecture": "東京都", "city": "町田市", "neighborhood": "森野", "banchi": "2丁目2番22号", "postal_code": "1948580", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "モリノ", "alternates": []}');
 INSERT INTO office_data VALUES('1948567','{"jis": "13209", "kana": "マチダゼイムシヨ", "name": "町田税務署", "prefecture": "東京都", "city": "町田市", "neighborhood": "中町", "banchi": "3丁目3-6", "postal_code": "1948567", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1948501','{"jis": "13209", "kana": "マチダトウキユウツインズ", "name": "町田東急ツインズ", "prefecture": "東京都", "city": "町田市", "neighborhood": "原町田", "banchi": "6丁目4番1号", "postal_code": "1948501", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ハラマチダ", "alternates": []}');
 INSERT INTO office_data VALUES('1948586','{"jis": "13209", "kana": "マチダユウビンチヨキンチイキブンカカツドウシエンシセツ", "name": "町田郵便貯金地域文化活動支援施設", "prefecture": "東京都", "city": "町田市", "neighborhood": "原町田", "banchi": "4丁目1-14", "postal_code": "1948586", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ハラマチダ", "alternates": []}');
 INSERT INTO office_data VALUES('1948511','{"jis": "13209", "kana": "ミツビシカガクセイメイカガクケンキユウジヨ", "name": "三菱化学生命科学研究所", "prefecture": "東京都", "city": "町田市", "neighborhood": "南大谷", "banchi": "11号", "postal_code": "1948511", "old_code": "194  ", "post_office": "町田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "ミナミオオヤ", "alternates": []}');
-INSERT INTO office_data VALUES('1940297','{"jis": "13209", "kana": "イリヨウホウジンシヤダン コウリユウカイタマキユウリヨウビヨウイン", "name": "医療法人社団　幸隆会多摩丘陵病院", "prefecture": "東京都", "city": "町田市", "neighborhood": "下小山田町", "banchi": "1491", "postal_code": "1940297", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "シモオヤマダマチ", "alternates": []}');
+INSERT INTO office_data VALUES('1940297','{"jis": "13209", "kana": "イリヨウホウジンシヤダン コウリユウカイ タマキユウリヨウリハビリテ-シヨンビヨウイン", "name": "医療法人社団　幸隆会　多摩丘陵リハビリテーション病院", "prefecture": "東京都", "city": "町田市", "neighborhood": "下小山田町", "banchi": "1491", "postal_code": "1940297", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "シモオヤマダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1940294','{"jis": "13209", "kana": "オウビリンガクエン", "name": "桜美林学園", "prefecture": "東京都", "city": "町田市", "neighborhood": "常盤町", "banchi": "3758", "postal_code": "1940294", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "トキワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1940295','{"jis": "13209", "kana": "カブシキガイシヤ オ-クセイサクシヨ", "name": "株式会社　オーク製作所", "prefecture": "東京都", "city": "町田市", "neighborhood": "小山ケ丘", "banchi": "3丁目9-6", "postal_code": "1940295", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1940293','{"jis": "13209", "kana": "チユウオウキヨウドウクミアイガクエン", "name": "中央協同組合学園", "prefecture": "東京都", "city": "町田市", "neighborhood": "相原町", "banchi": "4771", "postal_code": "1940293", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "アイハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1940292','{"jis": "13209", "kana": "トウキヨウカセイガクインダイガク", "name": "東京家政学院大学", "prefecture": "東京都", "city": "町田市", "neighborhood": "相原町", "banchi": "2600", "postal_code": "1940292", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "アイハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1940296','{"jis": "13209", "kana": "トウキヨウコウクウケイキ カブシキガイシヤ", "name": "東京航空計器　株式会社", "prefecture": "東京都", "city": "町田市", "neighborhood": "小山ヶ丘", "banchi": "2丁目2番6号", "postal_code": "1940296", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "オヤマガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('1940298','{"jis": "13209", "kana": "ホウセイダイガク", "name": "法政大学", "prefecture": "東京都", "city": "町田市", "neighborhood": "相原町", "banchi": "4342", "postal_code": "1940298", "old_code": "19402", "post_office": "町田西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "アイハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1958555','{"jis": "13209", "kana": "ガツコウホウジン ワコウガクエン", "name": "学校法人　和光学園", "prefecture": "東京都", "city": "町田市", "neighborhood": "金井町", "banchi": "2160番地", "postal_code": "1958555", "old_code": "195  ", "post_office": "鶴川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "マチダシ", "neighborhood_kana": "カナイマチ", "alternates": []}');
@@ -130606,15 +130612,15 @@
 INSERT INTO office_data VALUES('2538660','{"jis": "14207", "kana": "チガサキシホケンジヨ", "name": "茅ヶ崎市保健所", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "茅ヶ崎", "banchi": "一丁目8番7号", "postal_code": "2538660", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "チガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('2538686','{"jis": "14207", "kana": "チガサキシヤクシヨ", "name": "茅ヶ崎市役所", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "茅ヶ崎", "banchi": "1丁目1-1(茅ヶ崎郵便局私書箱第6号)", "postal_code": "2538686", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "チガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('2538577','{"jis": "14207", "kana": "ト-ト- カブシキガイシヤ チガサキコウジヨウ", "name": "ＴＯＴＯ株式会社　茅ヶ崎工場", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "本村", "banchi": "2丁目8-1", "postal_code": "2538577", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "ホンソン", "alternates": []}');
 INSERT INTO office_data VALUES('2538510','{"jis": "14207", "kana": "トウホウチタニウム カブシキガイシヤ", "name": "東邦チタニウム　株式会社", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "茅ヶ崎", "banchi": "3丁目3-5", "postal_code": "2538510", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "チガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('2538550','{"jis": "14207", "kana": "ブンキヨウダイガク シヨウナンコウシヤ ブンキヨウダイガク ジヨシタンキダイガクブ", "name": "文教大学　湘南校舎　文教大学　女子短期大学部", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "行谷", "banchi": "1100", "postal_code": "2538550", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "ナメガヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2538588','{"jis": "14207", "kana": "モリタミヤタコウギヨウ カブシキガイシヤ チガサキコウジヨウ", "name": "モリタ宮田工業　株式会社　茅ヶ崎工場", "prefecture": "神奈川県", "city": "茅ヶ崎市", "neighborhood": "下町屋", "banchi": "1丁目1-1", "postal_code": "2538588", "old_code": "253  ", "post_office": "茅ヶ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "チガサキシ", "neighborhood_kana": "シモマチヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2498510','{"jis": "14208", "kana": "ズシカイセイチユウガク・コウトウガツコウ", "name": "逗子開成中学・高等学校", "prefecture": "神奈川県", "city": "逗子市", "neighborhood": "新宿", "banchi": "2丁目5-1", "postal_code": "2498510", "old_code": "249  ", "post_office": "逗子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ズシシ", "neighborhood_kana": "シンジュク", "alternates": []}');
-INSERT INTO office_data VALUES('2498686','{"jis": "14208", "kana": "ズシシヤクシヨ", "name": "逗子市役所", "prefecture": "神奈川県", "city": "逗子市", "neighborhood": "逗子", "banchi": "5丁目2-16(逗子郵便局私書箱第26号)", "postal_code": "2498686", "old_code": "249  ", "post_office": "逗子", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ズシシ", "neighborhood_kana": "ズシ", "alternates": []}');
+INSERT INTO office_data VALUES('2498686','{"jis": "14208", "kana": "ズシシヤクシヨ", "name": "逗子市役所", "prefecture": "神奈川県", "city": "逗子市", "neighborhood": "逗子", "banchi": "5丁目2-16", "postal_code": "2498686", "old_code": "249  ", "post_office": "逗子", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ズシシ", "neighborhood_kana": "ズシ", "alternates": []}');
 INSERT INTO office_data VALUES('2380292','{"jis": "14210", "kana": "ソノラス・コ-トアブラツボ", "name": "ソノラス・コート油壺", "prefecture": "神奈川県", "city": "三浦市", "neighborhood": "尾上町", "banchi": "18", "postal_code": "2380292", "old_code": "23802", "post_office": "三浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ミウラシ", "neighborhood_kana": "オガミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2380298','{"jis": "14210", "kana": "ミウラシヤクシヨ", "name": "三浦市役所", "prefecture": "神奈川県", "city": "三浦市", "neighborhood": "城山町", "banchi": "1-1", "postal_code": "2380298", "old_code": "23802", "post_office": "三浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ミウラシ", "neighborhood_kana": "シロヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2578502','{"jis": "14211", "kana": "カブシキガイシヤ ワイデイ-ケ-テクノロジ-ズ", "name": "株式会社　ＹＤＫテクノロジーズ", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "曽屋", "banchi": "500", "postal_code": "2578502", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "ソヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2578511','{"jis": "14211", "kana": "キヨウセラ カブシキガイシヤ カナガワハダノコウジヨウ", "name": "京セラ　株式会社　神奈川秦野工場", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "曽屋", "banchi": "1204番地", "postal_code": "2578511", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "ソヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2578566','{"jis": "14211", "kana": "クア-ズテツク カブシキガイシヤ ハダノジギヨウシヨ", "name": "クアーズテック　株式会社　秦野事業所", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "曽屋", "banchi": "30", "postal_code": "2578566", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "ソヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2578585','{"jis": "14211", "kana": "コクリツリヨウヨウジヨ カナガワビヨウイン", "name": "国立療養所　神奈川病院", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "落合", "banchi": "666-1", "postal_code": "2578585", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "オチアイ", "alternates": []}');
 INSERT INTO office_data VALUES('2578523','{"jis": "14211", "kana": "シヨクヒンヤクヒンアンゼンセンタ-", "name": "食品薬品安全センター", "prefecture": "神奈川県", "city": "秦野市", "neighborhood": "落合", "banchi": "729-5", "postal_code": "2578523", "old_code": "257  ", "post_office": "秦野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ハダノシ", "neighborhood_kana": "オチアイ", "alternates": []}');
@@ -130731,22 +130737,21 @@
 INSERT INTO office_data VALUES('2590396','{"jis": "14384", "kana": "ドクリツギヨウセイホウジン チイキイリヨウキノウスイシンキコウ ユガワラビヨウイン", "name": "独立行政法人　地域医療機能推進機構　湯河原病院", "prefecture": "神奈川県", "city": "足柄下郡湯河原町", "neighborhood": "中央", "banchi": "2-21-6", "postal_code": "2590396", "old_code": "25903", "post_office": "湯河原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "アシガラシモグンユガワラマチ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2590392','{"jis": "14384", "kana": "ユガワラマチヤクバ", "name": "湯河原町役場", "prefecture": "神奈川県", "city": "足柄下郡湯河原町", "neighborhood": "中央", "banchi": "2丁目2-1", "postal_code": "2590392", "old_code": "25903", "post_office": "湯河原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "アシガラシモグンユガワラマチ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2430392','{"jis": "14401", "kana": "アイカワマチヤクバ", "name": "愛川町役場", "prefecture": "神奈川県", "city": "愛甲郡愛川町", "neighborhood": "角田", "banchi": "251-1", "postal_code": "2430392", "old_code": "24308", "post_office": "厚木北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "アイコウグンアイカワマチ", "neighborhood_kana": "スミダ", "alternates": []}');
 INSERT INTO office_data VALUES('2430195','{"jis": "14402", "kana": "キヨカワムラヤクバ", "name": "清川村役場", "prefecture": "神奈川県", "city": "愛甲郡清川村", "neighborhood": "煤ヶ谷", "banchi": "2216番地", "postal_code": "2430195", "old_code": "24301", "post_office": "厚木北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "アイコウグンキヨカワムラ", "neighborhood_kana": "ススガヤ", "alternates": []}');
 INSERT INTO office_data VALUES('9503195','{"jis": "15101", "kana": "サンコウセイカ カブシキガイシヤ", "name": "三幸製菓　株式会社", "prefecture": "新潟県", "city": "新潟市北区", "neighborhood": "新崎", "banchi": "2丁目6番1号", "postal_code": "9503195", "old_code": "95031", "post_office": "松浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシキタク", "neighborhood_kana": "ニイザキ", "alternates": []}');
 INSERT INTO office_data VALUES('9503198','{"jis": "15101", "kana": "ニイガタイリヨウフクシダイガク", "name": "新潟医療福祉大学", "prefecture": "新潟県", "city": "新潟市北区", "neighborhood": "島見町", "banchi": "1398番地", "postal_code": "9503198", "old_code": "95031", "post_office": "松浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシキタク", "neighborhood_kana": "シマミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9503197','{"jis": "15101", "kana": "ニイガタシヨクリヨウノウギヨウダイガク ニイガタキヤンパス", "name": "新潟食料農業大学　新潟キャンパス", "prefecture": "新潟県", "city": "新潟市北区", "neighborhood": "島見町", "banchi": "940番地", "postal_code": "9503197", "old_code": "95031", "post_office": "松浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシキタク", "neighborhood_kana": "シマミチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('9503393','{"jis": "15101", "kana": "ニイガタシキタクヤクシヨ", "name": "新潟市北区役所", "prefecture": "新潟県", "city": "新潟市北区", "neighborhood": "葛塚", "banchi": "3197", "postal_code": "9503393", "old_code": "95033", "post_office": "豊栄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシキタク", "neighborhood_kana": "クズツカ", "alternates": []}');
 INSERT INTO office_data VALUES('9508735','{"jis": "15102", "kana": "イチマサカマボコ カブシキガイシヤ", "name": "一正蒲鉾　株式会社", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "津島屋", "banchi": "7丁目77", "postal_code": "9508735", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "ツシマヤ", "alternates": []}');
 INSERT INTO office_data VALUES('9508723','{"jis": "15102", "kana": "イデミツコウサン カブシキガイシヤ ニイガタセキユセイヒンユニユウキチ", "name": "出光興産　株式会社　新潟石油製品輸入基地", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "臨港町", "banchi": "3丁目4914番479", "postal_code": "9508723", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "リンコウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508640','{"jis": "15102", "kana": "カブシキガイシヤ ダイヤメツト", "name": "株式会社　ダイヤメット", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "小金町", "banchi": "3丁目1番1号", "postal_code": "9508640", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "コガネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508715','{"jis": "15102", "kana": "カブシキガイシヤ ナビツク", "name": "株式会社　ナビック", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "松島", "banchi": "1丁目2-8", "postal_code": "9508715", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "マツシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9508707','{"jis": "15102", "kana": "カブシキガイシヤ ニイガタヒタチ", "name": "株式会社　新潟日立", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "竹尾卸新町", "banchi": "752-10", "postal_code": "9508707", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "タケオオロシシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9508680','{"jis": "15102", "kana": "コウリツダイガクホウジン ニイガタケンリツダイガク", "name": "公立大学法人　新潟県立大学", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "海老ケ瀬", "banchi": "471", "postal_code": "9508680", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "エビガセ", "alternates": []}');
-INSERT INTO office_data VALUES('9508730','{"jis": "15102", "kana": "サトウシヨクヒン カブシキガイシヤ", "name": "サトウ食品　株式会社", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "宝町", "banchi": "13-5", "postal_code": "9508730", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "タカラマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9508730','{"jis": "15102", "kana": "サトウシヨクヒン カブシキガイシヤ", "name": "サトウ食品　株式会社", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "宝町", "banchi": "13-5", "postal_code": "9508730", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "タカラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9508725','{"jis": "15102", "kana": "シヤカイイリヨウホウジン ニイガタリンコウホケンカイ ニイガタリンコウビヨウイン", "name": "社会医療法人　新潟臨港保健会　新潟臨港病院", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "桃山町", "banchi": "1丁目114番地3", "postal_code": "9508725", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "モモヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508720','{"jis": "15102", "kana": "シロセシヨウジ カブシキガイシヤ", "name": "白勢商事　株式会社", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "山木戸", "banchi": "8丁目8-1", "postal_code": "9508720", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "ヤマキド", "alternates": []}');
 INSERT INTO office_data VALUES('9508678','{"jis": "15102", "kana": "ジヤスコ カブシキガイシヤ ニイガタヒガシシテン", "name": "ジャスコ　株式会社　新潟東支店", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "大形本町", "banchi": "3丁目1-2", "postal_code": "9508678", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "オオガタホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508744','{"jis": "15102", "kana": "トウホクデンリヨク カブシキガイシヤ ニイガタカリヨクハツデンシヨ", "name": "東北電力　株式会社　新潟火力発電所", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "桃山町", "banchi": "2丁目200", "postal_code": "9508744", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "モモヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508639','{"jis": "15102", "kana": "ニイガタケンリツ ニイガタヒガシコウトウガツコウ", "name": "新潟県立　新潟東高等学校", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "小金町", "banchi": "2丁目6-1", "postal_code": "9508639", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "コガネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508677','{"jis": "15102", "kana": "ニイガタケンリツ ニイガタヨウゴガツコウ", "name": "新潟県立　新潟養護学校", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "海老ケ瀬", "banchi": "994", "postal_code": "9508677", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "エビガセ", "alternates": []}');
 INSERT INTO office_data VALUES('9508709','{"jis": "15102", "kana": "ニイガタシヒガシクヤクシヨ", "name": "新潟市東区役所", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "下木戸", "banchi": "1丁目4番1号", "postal_code": "9508709", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "シモキド", "alternates": []}');
@@ -131015,15 +131020,15 @@
 INSERT INTO office_data VALUES('9408532','{"jis": "15202", "kana": "ナガオカコウギヨウコウトウセンモンガツコウ", "name": "長岡工業高等専門学校", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "西片貝町", "banchi": "888", "postal_code": "9408532", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ニシカタカイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9408501','{"jis": "15202", "kana": "ナガオカシヤクシヨ", "name": "長岡市役所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "大手通", "banchi": "1丁目4番地10", "postal_code": "9408501", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "オオテドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('9408660','{"jis": "15202", "kana": "ナガオカシンヨウキンコ", "name": "長岡信用金庫", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "大手通", "banchi": "2丁目4-7(長岡郵便局私書箱第50号)", "postal_code": "9408660", "old_code": "940  ", "post_office": "長岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "オオテドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('9408654','{"jis": "15202", "kana": "ナガオカゼイムシヨ", "name": "長岡税務署", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "千歳", "banchi": "1丁目3番88号長岡地方合同庁舎", "postal_code": "9408654", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "センザイ", "alternates": []}');
 INSERT INTO office_data VALUES('9408653','{"jis": "15202", "kana": "ナガオカチユウオウソウゴウビヨウイン", "name": "長岡中央綜合病院", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "川崎町", "banchi": "2041", "postal_code": "9408653", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "カワサキマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9408554','{"jis": "15202", "kana": "ニイガタケン キヨウイクチヨウチユウエツキヨウイクジムシヨ", "name": "新潟県　教育庁中越教育事務所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "四郎丸町", "banchi": "173-2長岡総合庁舎内", "postal_code": "9408554", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "シロウマルマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9408567','{"jis": "15202", "kana": "ニイガタケン ナガオカチイキシンコウキヨク", "name": "新潟県　長岡地域振興局", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "四郎丸町", "banchi": "173番地2", "postal_code": "9408567", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "シロウマルマチ", "alternates": []}');
-INSERT INTO office_data VALUES('9408530','{"jis": "15202", "kana": "ニイガタダイガクフゾクガツコウブナガオカフゾクガツコウ", "name": "新潟大学附属学校部長岡附属学校", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "学校町", "banchi": "1丁目1番1号", "postal_code": "9408530", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ガッコウチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('9408530','{"jis": "15202", "kana": "ニイガタダイガクフゾクガツコウブナガオカフゾクガツコウ", "name": "新潟大学附属学校部長岡附属学校", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "学校町", "banchi": "1丁目1番1号", "postal_code": "9408530", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ガッコウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9408583','{"jis": "15202", "kana": "ニイガタト-ヨ- カブシキガイシヤ", "name": "新潟トーヨー　株式会社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "北陽", "banchi": "2丁目14番地16", "postal_code": "9408583", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ホクヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('9408580','{"jis": "15202", "kana": "ニホンセイキ カブシキカイシヤ", "name": "日本精機　株式会社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "東蔵王", "banchi": "2丁目2-34", "postal_code": "9408580", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ヒガシザオウ", "alternates": []}');
 INSERT INTO office_data VALUES('9408686','{"jis": "15202", "kana": "ニホンセイメイホケン ソウゴガイシヤ ナガオカシシヤ", "name": "日本生命保険　相互会社　長岡支社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "東坂之上町", "banchi": "3丁目2-6(長岡郵便局私書箱第59号)", "postal_code": "9408686", "old_code": "940  ", "post_office": "長岡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ヒガシサカノウエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9408577','{"jis": "15202", "kana": "フナヤマ カブシキガイシヤ", "name": "船山　株式会社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "稲保", "banchi": "4丁目713番地2", "postal_code": "9408577", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "イナホ", "alternates": []}');
 INSERT INTO office_data VALUES('9408508','{"jis": "15202", "kana": "ヘアドクタ-ハツモウカガクケンキユウジヨ", "name": "ヘアドクター発毛科学研究所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "城内町", "banchi": "3丁目8-7", "postal_code": "9408508", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ジョウナイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9408631','{"jis": "15202", "kana": "マルセンセンイ カブシキカイシヤ", "name": "丸専繊維　株式会社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "大手通", "banchi": "2丁目1-8", "postal_code": "9408631", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "オオテドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('9408588','{"jis": "15202", "kana": "マルベニ カブシキカイシヤ ナガオカシテン", "name": "丸紅　株式会社　長岡支店", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "東坂之上町", "banchi": "2丁目1-1", "postal_code": "9408588", "old_code": "940  ", "post_office": "長岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ヒガシサカノウエマチ", "alternates": []}');
@@ -131102,19 +131107,19 @@
 INSERT INTO office_data VALUES('9458540','{"jis": "15205", "kana": "カブシキガイシヤ ウエキグミ", "name": "株式会社　植木組", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "駅前", "banchi": "1丁目5番45号", "postal_code": "9458540", "old_code": "945  ", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "エキマエ", "alternates": []}');
 INSERT INTO office_data VALUES('9458585','{"jis": "15205", "kana": "コクリツビヨウインキコウ ニイガタビヨウイン", "name": "国立病院機構　新潟病院", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "赤坂町", "banchi": "3-52", "postal_code": "9458585", "old_code": "945  ", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "アカサカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9450192','{"jis": "15205", "kana": "カシワザキユ-エステツク カブシキガイシヤ", "name": "柏崎ユーエステック　株式会社", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字藤井", "banchi": "字西沖1350", "postal_code": "9450192", "old_code": "94501", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9450194','{"jis": "15205", "kana": "カトウスプリング カブシキガイシヤ", "name": "カトウスプリング　株式会社", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字藤井", "banchi": "字西沖1355番地2", "postal_code": "9450194", "old_code": "94501", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9450193','{"jis": "15205", "kana": "カブシキガイシヤ アドバネクス", "name": "株式会社　アドバネクス", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字藤井", "banchi": "字西沖1355", "postal_code": "9450193", "old_code": "94501", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9458601','{"jis": "15205", "kana": "トウキヨウデンリヨク カブシキガイシヤ カシワザキカリワゲンシリヨクハツデンシヨ", "name": "東京電力　株式会社　柏崎刈羽原子力発電所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "青山町", "banchi": "16-46", "postal_code": "9458601", "old_code": "94503", "post_office": "柏崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "アオヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9451195','{"jis": "15205", "kana": "ニイガタコウカダイガク", "name": "新潟工科大学", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字藤橋", "banchi": "1719", "postal_code": "9451195", "old_code": "94511", "post_office": "新道", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451392','{"jis": "15205", "kana": "カシワザキコウセイビヨウイン", "name": "柏崎厚生病院", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字茨目", "banchi": "字二ツ池2071-1", "postal_code": "9451392", "old_code": "94513", "post_office": "田尻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451395','{"jis": "15205", "kana": "カブシキガイシヤ サイカワ", "name": "株式会社　サイカワ", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "7586", "postal_code": "9451395", "old_code": "94513", "post_office": "田尻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451393','{"jis": "15205", "kana": "ニイガタサンギヨウダイガク", "name": "新潟産業大学", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字軽井川", "banchi": "4730", "postal_code": "9451393", "old_code": "94513", "post_office": "田尻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451397','{"jis": "15205", "kana": "ニイガタサンギヨウダイガクフゾクコウトウガツコウ", "name": "新潟産業大学附属高等学校", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "2510-2", "postal_code": "9451397", "old_code": "94513", "post_office": "田尻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9451398','{"jis": "15205", "kana": "フジゼロツクスマニユフアクチユアリング カブシキガイシヤ ニイガタジギヨウシヨ", "name": "富士ゼロックスマニュファクチュアリング　株式会社　新潟事業所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "7546", "postal_code": "9451398", "old_code": "94513", "post_office": "田尻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451392','{"jis": "15205", "kana": "カシワザキコウセイビヨウイン", "name": "柏崎厚生病院", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字茨目", "banchi": "字二ツ池2071-1", "postal_code": "9451392", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451395','{"jis": "15205", "kana": "カブシキガイシヤ サイカワ", "name": "株式会社　サイカワ", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "7586", "postal_code": "9451395", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451393','{"jis": "15205", "kana": "ニイガタサンギヨウダイガク", "name": "新潟産業大学", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字軽井川", "banchi": "4730", "postal_code": "9451393", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451397','{"jis": "15205", "kana": "ニイガタサンギヨウダイガクフゾクコウトウガツコウ", "name": "新潟産業大学附属高等学校", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "2510-2", "postal_code": "9451397", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('9451398','{"jis": "15205", "kana": "フジゼロツクスマニユフアクチユアリング カブシキガイシヤ ニイガタジギヨウシヨ", "name": "富士ゼロックスマニュファクチュアリング　株式会社　新潟事業所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "大字安田", "banchi": "7546", "postal_code": "9451398", "old_code": "94513", "post_office": "柏崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9451595','{"jis": "15205", "kana": "カシワザキシヤクシヨ タカヤナギマチジムシヨ", "name": "柏崎市役所　高柳町事務所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "高柳町岡野町", "banchi": "1849-1", "postal_code": "9451595", "old_code": "94515", "post_office": "中鯖石", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "タカヤナギチョウオカノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9494194','{"jis": "15205", "kana": "イキイキカン", "name": "いきいき館", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "西山町池浦", "banchi": "877", "postal_code": "9494194", "old_code": "94941", "post_office": "礼拝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "ニシヤマチョウイケウラ", "alternates": []}');
 INSERT INTO office_data VALUES('9494193','{"jis": "15205", "kana": "カシワザキシヤクシヨ ニシヤママチジムシヨ", "name": "柏崎市役所　西山町事務所", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "西山町池浦", "banchi": "117-2", "postal_code": "9494193", "old_code": "94941", "post_office": "礼拝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "ニシヤマチョウイケウラ", "alternates": []}');
 INSERT INTO office_data VALUES('9494192','{"jis": "15205", "kana": "ナガイコンクリ-トコウギヨウ カブシキガイシヤ", "name": "永井コンクリート工業　株式会社", "prefecture": "新潟県", "city": "柏崎市", "neighborhood": "西山町礼拝", "banchi": "457", "postal_code": "9494192", "old_code": "94941", "post_office": "礼拝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "カシワザキシ", "neighborhood_kana": "ニシヤマチョウライハイ", "alternates": []}');
 INSERT INTO office_data VALUES('9578701','{"jis": "15206", "kana": "キヨウセラ カブシキガイシヤ ニイガタシバタコウジヨウ", "name": "京セラ　株式会社　新潟新発田工場", "prefecture": "新潟県", "city": "新発田市", "neighborhood": "五十公野", "banchi": "字山崎5270番地", "postal_code": "9578701", "old_code": "957  ", "post_office": "新発田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "シバタシ", "neighborhood_kana": "イジミノ", "alternates": []}');
 INSERT INTO office_data VALUES('9578585','{"jis": "15206", "kana": "ケイワガクエンダイガク", "name": "敬和学園大学", "prefecture": "新潟県", "city": "新発田市", "neighborhood": "大字富塚", "banchi": "1270", "postal_code": "9578585", "old_code": "957  ", "post_office": "新発田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9578601','{"jis": "15206", "kana": "シバタケンセツ カブシキガイシヤ", "name": "新発田建設　株式会社", "prefecture": "新潟県", "city": "新発田市", "neighborhood": "富塚", "banchi": "1942(新発田郵便局私書箱第25号)", "postal_code": "9578601", "old_code": "957  ", "post_office": "新発田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -131383,15 +131388,15 @@
 INSERT INTO office_data VALUES('9308506','{"jis": "16201", "kana": "ニツポンネンキンキコウ トヤマジムセンタ-", "name": "日本年金機構　富山事務センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "桜橋通り", "banchi": "5-13富山興銀ビル8階", "postal_code": "9308506", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "サクラバシドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('9308571','{"jis": "16201", "kana": "ニツポンネンキンキコウ トヤマネンキンジムシヨ", "name": "日本年金機構　富山年金事務所", "prefecture": "富山県", "city": "富山市", "neighborhood": "牛島新町", "banchi": "7-1", "postal_code": "9308571", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ウシジマシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9308588','{"jis": "16201", "kana": "ニホンカイガス カブシキガイシヤ", "name": "日本海ガス　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "城北町", "banchi": "2-36", "postal_code": "9308588", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ジョウホクマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9308610','{"jis": "16201", "kana": "ニホンセイメイホケン ソウゴガイシヤ トヤマシシヤ", "name": "日本生命保険　相互会社　富山支社", "prefecture": "富山県", "city": "富山市", "neighborhood": "総曲輪", "banchi": "1丁目5-24", "postal_code": "9308610", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ソウガワ", "alternates": []}');
 INSERT INTO office_data VALUES('9308516','{"jis": "16201", "kana": "ネツツトヨタトヤマ カブシキガイシヤ", "name": "ネッツトヨタ富山　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "新庄本町", "banchi": "3丁目3-33", "postal_code": "9308516", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "シンジョウホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9308604','{"jis": "16201", "kana": "ノムラシヨウケン カブシキガイシヤ トヤマシテン", "name": "野村證券　株式会社　富山支店", "prefecture": "富山県", "city": "富山市", "neighborhood": "堤町通り", "banchi": "1丁目4-3", "postal_code": "9308604", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ツツミチョウドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('9308525','{"jis": "16201", "kana": "ホクギンリ-ス カブシキガイシヤ", "name": "北銀リース　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "荒町", "banchi": "2-21", "postal_code": "9308525", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "アラマチ", "alternates": []}');
-INSERT INTO office_data VALUES('9308554','{"jis": "16201", "kana": "ホクリクザイムキヨク トヤマザイムジムシヨ", "name": "北陸財務局　富山財務事務所", "prefecture": "富山県", "city": "富山市", "neighborhood": "牛島新町", "banchi": "11番7号", "postal_code": "9308554", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ウシジマシンマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9308554','{"jis": "16201", "kana": "ホクリクザイムキヨク トヤマザイムジムシヨ", "name": "北陸財務局　富山財務事務所", "prefecture": "富山県", "city": "富山市", "neighborhood": "牛島新町", "banchi": "11番7号", "postal_code": "9308554", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ウシジマシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9308518','{"jis": "16201", "kana": "ホクリクツウシンコウギヨウ", "name": "北陸通信工業", "prefecture": "富山県", "city": "富山市", "neighborhood": "綾田町", "banchi": "1丁目7-23", "postal_code": "9308518", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "アイデンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9308543','{"jis": "16201", "kana": "ホクリクデンリヨク カブシキガイシヤ トヤマシテン", "name": "北陸電力　株式会社　富山支店", "prefecture": "富山県", "city": "富山市", "neighborhood": "桜橋通り", "banchi": "3番1号(電気ビル内)", "postal_code": "9308543", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "サクラバシドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('9308686','{"jis": "16201", "kana": "ホクリクデンリヨク カブシキガイシヤ ホンテン", "name": "北陸電力　株式会社　本店", "prefecture": "富山県", "city": "富山市", "neighborhood": "牛島", "banchi": "15-1", "postal_code": "9308686", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9308687','{"jis": "16201", "kana": "ホクリクデンリヨクソウハイデン カブシキガイシヤ", "name": "北陸電力送配電　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "牛島町", "banchi": "15番1号", "postal_code": "9308687", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ウシジマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9308603','{"jis": "16201", "kana": "マルサンカイハツコウキ カブシキガイシヤ", "name": "丸三開発工機　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "上飯野", "banchi": "32", "postal_code": "9308603", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "カミイイノ", "alternates": []}');
 INSERT INTO office_data VALUES('9308666','{"jis": "16201", "kana": "メイシヨウ カブシキガイシヤ", "name": "明祥　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "問屋町", "banchi": "1丁目4-15", "postal_code": "9308666", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9308552','{"jis": "16201", "kana": "ユアサシヨウジ カブシキガイシヤ", "name": "ユアサ商事　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "桜橋通り", "banchi": "6-11富山フコク生命第2ビル6階", "postal_code": "9308552", "old_code": "930  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "サクラバシドオリ", "alternates": []}');
@@ -131407,15 +131412,15 @@
 INSERT INTO office_data VALUES('9308517','{"jis": "16201", "kana": "トヤマケン シチヨウソンシヨクインキヨウサイクミアイ", "name": "富山県　市町村職員共済組合", "prefecture": "富山県", "city": "富山市", "neighborhood": "下野", "banchi": "995-5", "postal_code": "9308517", "old_code": "93008", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "シモノ", "alternates": []}');
 INSERT INTO office_data VALUES('9308540','{"jis": "16201", "kana": "トヤマケンリツ トヤマシヨウギヨウコウトウガツコウ", "name": "富山県立　富山商業高等学校", "prefecture": "富山県", "city": "富山市", "neighborhood": "庄高田", "banchi": "413", "postal_code": "9308540", "old_code": "93008", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ショウタカタ", "alternates": []}');
 INSERT INTO office_data VALUES('9308555','{"jis": "16201", "kana": "トヤマダイガク", "name": "富山大学", "prefecture": "富山県", "city": "富山市", "neighborhood": "五福", "banchi": "3190", "postal_code": "9308555", "old_code": "93008", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ゴフク", "alternates": []}');
 INSERT INTO office_data VALUES('9308556','{"jis": "16201", "kana": "トヤマダイガク キヨウイクガクブフゾクガツコウ", "name": "富山大学　教育学部附属学校", "prefecture": "富山県", "city": "富山市", "neighborhood": "五艘", "banchi": "1300", "postal_code": "9308556", "old_code": "93008", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ゴソウ", "alternates": []}');
 INSERT INTO office_data VALUES('9301295','{"jis": "16201", "kana": "カブシキガイシヤ イチカワゴルフコウギヨウ", "name": "株式会社　市川ゴルフ興業", "prefecture": "富山県", "city": "富山市", "neighborhood": "東福沢", "banchi": "130", "postal_code": "9301295", "old_code": "93012", "post_office": "上滝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヒガシフクサワ", "alternates": []}');
 INSERT INTO office_data VALUES('9301298','{"jis": "16201", "kana": "トヤマコクサイシヨクゲイガクエン", "name": "富山国際職藝学園", "prefecture": "富山県", "city": "富山市", "neighborhood": "東黒牧", "banchi": "298", "postal_code": "9301298", "old_code": "93012", "post_office": "上滝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヒガシクロマキ", "alternates": []}');
 INSERT INTO office_data VALUES('9301292','{"jis": "16201", "kana": "トヤマコクサイダイガク", "name": "富山国際大学", "prefecture": "富山県", "city": "富山市", "neighborhood": "東黒牧", "banchi": "65-1", "postal_code": "9301292", "old_code": "93012", "post_office": "上滝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヒガシクロマキ", "alternates": []}');
-INSERT INTO office_data VALUES('9301392','{"jis": "16201", "kana": "トヤマシオオヤマソウゴウギヨウセイセンタ-", "name": "富山市大山総合行政センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "上滝", "banchi": "525", "postal_code": "9301392", "old_code": "93013", "post_office": "上滝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "カミダキ", "alternates": []}');
+INSERT INTO office_data VALUES('9301392','{"jis": "16201", "kana": "トヤマシオオヤマカイカン(オオヤマギヨウセイサ-ビスセンタ-・オオヤマホケンフクシセンタ-)", "name": "富山市大山会館（大山行政サービスセンター・大山保健福祉センター）", "prefecture": "富山県", "city": "富山市", "neighborhood": "上滝", "banchi": "567", "postal_code": "9301392", "old_code": "93013", "post_office": "上滝", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "カミダキ", "alternates": []}');
 INSERT INTO office_data VALUES('9302198','{"jis": "16201", "kana": "トヤマシヤマダソウゴウギヨウセイセンタ-", "name": "富山市山田総合行政センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "山田湯", "banchi": "780", "postal_code": "9302198", "old_code": "93021", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヤマダユ", "alternates": []}');
 INSERT INTO office_data VALUES('9318515','{"jis": "16201", "kana": "ダイイチヤクヒンコウギヨウ カブシキガイシヤ", "name": "第一薬品工業　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "草島", "banchi": "15-1", "postal_code": "9318515", "old_code": "93022", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "クサジマ", "alternates": []}');
 INSERT INTO office_data VALUES('9318585','{"jis": "16201", "kana": "トヤマツウウン カブシキガイシヤ", "name": "富山通運　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "八町", "banchi": "3309", "postal_code": "9318585", "old_code": "93022", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ハッチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9318522','{"jis": "16201", "kana": "ニホンカイセキユ カブシキガイシヤ", "name": "日本海石油　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "四方北窪", "banchi": "字前島平均500", "postal_code": "9318522", "old_code": "93022", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヨカタキタクボ", "alternates": []}');
 INSERT INTO office_data VALUES('9318523','{"jis": "16201", "kana": "ユ-デイ-トラツクス カブシキガイシヤ", "name": "ＵＤトラックス　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "八町", "banchi": "7900番地", "postal_code": "9318523", "old_code": "93022", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ハッチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9318543','{"jis": "16201", "kana": "カブシキガイシヤ アライドマテリアル トヤマセイサクシヨ", "name": "株式会社　アライドマテリアル　富山製作所", "prefecture": "富山県", "city": "富山市", "neighborhood": "岩瀬古志町", "banchi": "2", "postal_code": "9318543", "old_code": "931  ", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "イワセコシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9318511','{"jis": "16201", "kana": "カブシキガイシヤ フジコシマテリアルセイゾウジヨ", "name": "株式会社　不二越マテリアル製造所", "prefecture": "富山県", "city": "富山市", "neighborhood": "米田町", "banchi": "3丁目1-1", "postal_code": "9318511", "old_code": "931  ", "post_office": "富山北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヨネダマチ", "alternates": []}');
@@ -131457,19 +131462,19 @@
 INSERT INTO office_data VALUES('9398515','{"jis": "16201", "kana": "ニツシンボウセキ カブシキガイシヤ トヤマコウジヨウ", "name": "日清紡績　株式会社　富山工場", "prefecture": "富山県", "city": "富山市", "neighborhood": "堀", "banchi": "15", "postal_code": "9398515", "old_code": "939  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ホリ", "alternates": []}');
 INSERT INTO office_data VALUES('9398558','{"jis": "16201", "kana": "ネツツ トヨタノヴエルトヤマ カブシキガイシヤ", "name": "ネッツ　トヨタノヴェルとやま　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "山室", "banchi": "新町41", "postal_code": "9398558", "old_code": "939  ", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヤマムロ", "alternates": []}');
 INSERT INTO office_data VALUES('9398572','{"jis": "16201", "kana": "ホクリクデンキコウジ カブシキガイシヤ", "name": "北陸電気工事　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "小中", "banchi": "269", "postal_code": "9398572", "old_code": "939  ", "post_office": "富山南", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "コナカ", "alternates": []}');
 INSERT INTO office_data VALUES('9398571','{"jis": "16201", "kana": "ホクリクデンキコウジ カブシキガイシヤ", "name": "北陸電気工事　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "小中", "banchi": "269", "postal_code": "9398571", "old_code": "939  ", "post_office": "富山南", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "コナカ", "alternates": []}');
 INSERT INTO office_data VALUES('9393593','{"jis": "16201", "kana": "カブシキガイシヤ セキノコウサン", "name": "株式会社　セキノ興産", "prefecture": "富山県", "city": "富山市", "neighborhood": "水橋開発", "banchi": "277-12(水橋郵便局私書箱第7号)", "postal_code": "9393593", "old_code": "93905", "post_office": "水橋", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ミズハシカイホツ", "alternates": []}');
 INSERT INTO office_data VALUES('9390592','{"jis": "16201", "kana": "カブシキガイシヤ リツチエル", "name": "株式会社　リッチェル", "prefecture": "富山県", "city": "富山市", "neighborhood": "水橋桜木", "banchi": "136", "postal_code": "9390592", "old_code": "93905", "post_office": "水橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9368502','{"jis": "16201", "kana": "ユウゲンガイシヤ ウスイコウサン", "name": "有限会社　ウスイ興産", "prefecture": "富山県", "city": "富山市", "neighborhood": "水橋五郎丸", "banchi": "2007番地", "postal_code": "9368502", "old_code": "93905", "post_office": "滑川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ミズハシゴロウマル", "alternates": []}');
-INSERT INTO office_data VALUES('9392192','{"jis": "16201", "kana": "トヤマシホソイリチユウカクガタチクセンタ-", "name": "富山市細入中核型地区センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "楡原", "banchi": "1128番地", "postal_code": "9392192", "old_code": "93921", "post_office": "細入", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ニレハラ", "alternates": []}');
+INSERT INTO office_data VALUES('9392192','{"jis": "16201", "kana": "トヤマシホソイリチユウカクガタチクセンタ-", "name": "富山市細入中核型地区センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "楡原", "banchi": "1128番地", "postal_code": "9392192", "old_code": "93921", "post_office": "細入", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ニレハラ", "alternates": []}');
 INSERT INTO office_data VALUES('9392297','{"jis": "16201", "kana": "カブシキガイシヤ トヤマゴルフ", "name": "株式会社　富山ゴルフ", "prefecture": "富山県", "city": "富山市", "neighborhood": "万願寺", "banchi": "1-166", "postal_code": "9392297", "old_code": "93922", "post_office": "大沢野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "マンガンジ", "alternates": []}');
 INSERT INTO office_data VALUES('9392298','{"jis": "16201", "kana": "シヤカイフクシホウジン セ-ナ-エン", "name": "社会福祉法人　セーナー苑", "prefecture": "富山県", "city": "富山市", "neighborhood": "坂本", "banchi": "3110", "postal_code": "9392298", "old_code": "93922", "post_office": "大沢野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "サカモト", "alternates": []}');
 INSERT INTO office_data VALUES('9392295','{"jis": "16201", "kana": "トヤマコバヤシセイヤク カブシキガイシヤ", "name": "富山小林製薬　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "中大久保", "banchi": "100-1", "postal_code": "9392295", "old_code": "93922", "post_office": "大沢野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ナカオオクボ", "alternates": []}');
-INSERT INTO office_data VALUES('9392293','{"jis": "16201", "kana": "トヤマシオオサワノギヨウセイサ-ビスセンタ-", "name": "富山市大沢野行政サービスセンター", "prefecture": "富山県", "city": "富山市", "neighborhood": "高内", "banchi": "365番地", "postal_code": "9392293", "old_code": "93922", "post_office": "大沢野", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "タカウチ", "alternates": []}');
+INSERT INTO office_data VALUES('9392293','{"jis": "16201", "kana": "トヤマシオオサワノギヨウセイサ-ビスセンタ-", "name": "富山市大沢野行政サービスセンター", "prefecture": "富山県", "city": "富山市", "neighborhood": "高内", "banchi": "365番地", "postal_code": "9392293", "old_code": "93922", "post_office": "大沢野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "タカウチ", "alternates": []}');
 INSERT INTO office_data VALUES('9392292','{"jis": "16201", "kana": "ホクリクデンキコウギヨウ カブシキガイシヤ", "name": "北陸電気工業　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "下大久保", "banchi": "3158", "postal_code": "9392292", "old_code": "93922", "post_office": "大沢野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9392393','{"jis": "16201", "kana": "カブシキガイシヤ コクサイ エレクトリツク トヤマジギヨウシヨ", "name": "株式会社　ＫＯＫＵＳＡＩ　ＥＬＥＣＴＲＩＣ　富山事業所", "prefecture": "富山県", "city": "富山市", "neighborhood": "八尾町保内", "banchi": "2丁目1", "postal_code": "9392393", "old_code": "93923", "post_office": "越中八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヤツオマチヤスウチ", "alternates": []}');
 INSERT INTO office_data VALUES('9392398','{"jis": "16201", "kana": "トヤマシヤツオソウゴウギヨウセイセンタ-", "name": "富山市八尾総合行政センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "八尾町福島", "banchi": "151", "postal_code": "9392398", "old_code": "93923", "post_office": "越中八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヤツオマチフクジマ", "alternates": []}');
 INSERT INTO office_data VALUES('9392392','{"jis": "16201", "kana": "フジツウ カブシキガイシヤ", "name": "富士通　株式会社", "prefecture": "富山県", "city": "富山市", "neighborhood": "八尾町保内", "banchi": "2-2-1", "postal_code": "9392392", "old_code": "93923", "post_office": "越中八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "ヤツオマチヤスウチ", "alternates": []}');
 INSERT INTO office_data VALUES('9392694','{"jis": "16201", "kana": "トヤマカンイホケンホヨウセンタ-", "name": "富山簡易保険保養センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "婦中町羽根", "banchi": "5691-2", "postal_code": "9392694", "old_code": "93926", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "フチュウマチハネ", "alternates": []}');
 INSERT INTO office_data VALUES('9392692','{"jis": "16201", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ トヤマビヨウイン", "name": "独立行政法人　国立病院機構　富山病院", "prefecture": "富山県", "city": "富山市", "neighborhood": "婦中町新町", "banchi": "3145", "postal_code": "9392692", "old_code": "93926", "post_office": "富山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "フチュウマチアラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9392798','{"jis": "16201", "kana": "トヤマシフチユウソウゴウギヨウセイセンタ-", "name": "富山市婦中総合行政センター", "prefecture": "富山県", "city": "富山市", "neighborhood": "婦中町速星", "banchi": "754", "postal_code": "9392798", "old_code": "93927", "post_office": "富山南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トヤマケン", "city_kana": "トヤマシ", "neighborhood_kana": "フチュウマチハヤホシ", "alternates": []}');
@@ -131711,15 +131716,15 @@
 INSERT INTO office_data VALUES('9208688','{"jis": "17201", "kana": "カブシキカイシヤ カナザワニユ-グランドホテル", "name": "株式会社　金沢ニューグランドホテル", "prefecture": "石川県", "city": "金沢市", "neighborhood": "高岡町", "banchi": "1-50", "postal_code": "9208688", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タカオカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208797','{"jis": "17201", "kana": "カブシキカイシヤ ユウチヨギンコウ カナザワシテン", "name": "株式会社　ゆうちょ銀行　金沢支店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "上堤町", "banchi": "1-15", "postal_code": "9208797", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カミツツミチョウ", "alternates": [{"jis": "17201", "kana": "カブシキガイシヤ カンポセイメイ カナザワシテン", "name": "株式会社　かんぽ生命　金沢支店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "上堤町", "banchi": "1-15", "postal_code": "9208797", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カミツツミチョウ", "alternates": []}, {"jis": "17201", "kana": "ニホンユウビン カブシキガイシヤ ホクリクシシヤ", "name": "日本郵便　株式会社　北陸支社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "上堤町", "banchi": "1-15", "postal_code": "9208797", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カミツツミチョウ", "alternates": []}]}');
 INSERT INTO office_data VALUES('9208513','{"jis": "17201", "kana": "カブシキガイシヤ アイ・オ-・デ-タキキ", "name": "株式会社　アイ・オー・データ機器", "prefecture": "石川県", "city": "金沢市", "neighborhood": "桜田町", "banchi": "2-84", "postal_code": "9208513", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "サクラダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208606','{"jis": "17201", "kana": "カブシキガイシヤ アサムラ", "name": "株式会社　浅村", "prefecture": "石川県", "city": "金沢市", "neighborhood": "浅野本町", "banchi": "2丁目18-40", "postal_code": "9208606", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "アサノホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208601','{"jis": "17201", "kana": "カブシキガイシヤ イシカワトヨペツトカロ-ラ", "name": "株式会社　石川トヨペットカローラ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "浅野本町", "banchi": "ロ104番地", "postal_code": "9208601", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "アサノホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208628','{"jis": "17201", "kana": "カブシキガイシヤ イセキカンサイチユウブホクリクシシヤ", "name": "株式会社　ヰセキ関西中部北陸支社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "問屋町", "banchi": "1丁目32番地", "postal_code": "9208628", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208661','{"jis": "17201", "kana": "カブシキガイシヤ ウイルコムカナザワエイギヨウシヨ", "name": "株式会社　ウィルコム金沢営業所", "prefecture": "石川県", "city": "金沢市", "neighborhood": "本町", "banchi": "1丁目5-2リファーレ10階", "postal_code": "9208661", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
-INSERT INTO office_data VALUES('9208611','{"jis": "17201", "kana": "カブシキガイシヤ エイデイアイドツトジ-", "name": "株式会社　ＡＤＩ．Ｇ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "浅野本町", "banchi": "1丁目10-10", "postal_code": "9208611", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "アサノホンマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9208611','{"jis": "17201", "kana": "カブシキガイシヤ エイデイアイドツトジ-", "name": "株式会社　ＡＤＩ．Ｇ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "浅野本町", "banchi": "1丁目10-10", "postal_code": "9208611", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "アサノホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208619','{"jis": "17201", "kana": "カブシキガイシヤ エヌ・テイ・テイ・デ-タホクリク", "name": "株式会社　エヌ・ティ・ティ・データ北陸", "prefecture": "石川県", "city": "金沢市", "neighborhood": "彦三町", "banchi": "1丁目1番1号", "postal_code": "9208619", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ヒコソマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208630','{"jis": "17201", "kana": "カブシキガイシヤ エヌ・テイ・テイ・ドコモホクリク", "name": "株式会社　エヌ・ティ・ティ・ドコモ北陸", "prefecture": "石川県", "city": "金沢市", "neighborhood": "大手町", "banchi": "12-8", "postal_code": "9208630", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208605','{"jis": "17201", "kana": "カブシキガイシヤ エフエムイシカワ", "name": "株式会社　エフエム石川", "prefecture": "石川県", "city": "金沢市", "neighborhood": "香林坊", "banchi": "2丁目4番30号(香林坊ラモーダ)", "postal_code": "9208605", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コウリンボウ", "alternates": []}');
 INSERT INTO office_data VALUES('9208670','{"jis": "17201", "kana": "カブシキガイシヤ エフデイ-アドバイザリ-", "name": "株式会社　ＦＤアドバイザリー", "prefecture": "石川県", "city": "金沢市", "neighborhood": "広岡", "banchi": "2丁目12番6号(金沢中央郵便局私書箱第29号)", "postal_code": "9208670", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ヒロオカ", "alternates": [{"jis": "17201", "kana": "カブシキガイシヤ シ-シ-イノベ-シヨン", "name": "株式会社　ＣＣイノベーション", "prefecture": "石川県", "city": "金沢市", "neighborhood": "広岡", "banchi": "2丁目12番6号(金沢中央郵便局私書箱第29号)", "postal_code": "9208670", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ヒロオカ", "alternates": []}, {"jis": "17201", "kana": "カブシキガイシヤ ホツコクギンコウ", "name": "株式会社　北國銀行", "prefecture": "石川県", "city": "金沢市", "neighborhood": "広岡", "banchi": "2丁目12番6号(金沢中央郵便局私書箱第29号)", "postal_code": "9208670", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ヒロオカ", "alternates": []}, {"jis": "17201", "kana": "カブシキガイシヤ ホツコクフイナンシヤルホ-ルデイングス", "name": "株式会社　北國フィナンシャルホールディングス", "prefecture": "石川県", "city": "金沢市", "neighborhood": "広岡", "banchi": "2丁目12番6号(金沢中央郵便局私書箱第29号)", "postal_code": "9208670", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ヒロオカ", "alternates": []}]}');
 INSERT INTO office_data VALUES('9208721','{"jis": "17201", "kana": "カブシキガイシヤ クマガイグミ ホクリクシテン", "name": "株式会社　熊谷組　北陸支店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "広岡", "banchi": "2丁目13番5号MHM金沢ビル2階", "postal_code": "9208721", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ヒロオカ", "alternates": []}');
 INSERT INTO office_data VALUES('9208567','{"jis": "17201", "kana": "カブシキガイシヤ シミズシンテツク", "name": "株式会社　シミズシンテック", "prefecture": "石川県", "city": "金沢市", "neighborhood": "玉川町", "banchi": "5-36", "postal_code": "9208567", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タマガワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9208522','{"jis": "17201", "kana": "カブシキガイシヤ トウキヨウストア-", "name": "株式会社　東京ストアー", "prefecture": "石川県", "city": "金沢市", "neighborhood": "西都", "banchi": "2丁目4番地", "postal_code": "9208522", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "セイト", "alternates": []}');
@@ -131805,18 +131810,18 @@
 INSERT INTO office_data VALUES('9200398','{"jis": "17201", "kana": "カブシキガイシヤ イシカワコンピユ-タセンタ-", "name": "株式会社　石川コンピュータセンター", "prefecture": "石川県", "city": "金沢市", "neighborhood": "無量寺町", "banchi": "ハ6-1", "postal_code": "9200398", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ムリョウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9218531','{"jis": "17201", "kana": "カブシキガイシヤ ジエスクホリウチ", "name": "株式会社　ジェスクホリウチ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "古府", "banchi": "2丁目74番地", "postal_code": "9218531", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コブ", "alternates": []}');
 INSERT INTO office_data VALUES('9200386','{"jis": "17201", "kana": "テレビカナザワ", "name": "テレビ金沢", "prefecture": "石川県", "city": "金沢市", "neighborhood": "古府", "banchi": "2丁目136", "postal_code": "9200386", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コブ", "alternates": []}');
 INSERT INTO office_data VALUES('9200396','{"jis": "17201", "kana": "ニツセイビルドコウギヨウ カブシキガイシヤ", "name": "日成ビルド工業　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "金石北", "banchi": "3丁目16-10", "postal_code": "9200396", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カナイワキタ", "alternates": []}');
 INSERT INTO office_data VALUES('9200393','{"jis": "17201", "kana": "ホクリクアサヒホウソウ カブシキガイシヤ", "name": "北陸朝日放送　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "松島", "banchi": "1丁目32-2", "postal_code": "9200393", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "マツシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9200381','{"jis": "17201", "kana": "ホクリヨウデンコウ カブシキガイシヤ", "name": "北菱電興　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "古府", "banchi": "3丁目12", "postal_code": "9200381", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コブ", "alternates": []}');
 INSERT INTO office_data VALUES('9200385','{"jis": "17201", "kana": "マルブンツウシヨウ カブシキガイシヤ", "name": "丸文通商　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "松島", "banchi": "1丁目40", "postal_code": "9200385", "old_code": "92003", "post_office": "新金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "マツシマ", "alternates": []}');
+INSERT INTO office_data VALUES('9201184','{"jis": "17201", "kana": "イオンリテ-ル カブシキガイシヤ イオンモリノサトテン", "name": "イオンリテール　株式会社　イオンもりの里店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "もりの里", "banchi": "1丁目70", "postal_code": "9201184", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "モリノサト", "alternates": []}');
 INSERT INTO office_data VALUES('9201185','{"jis": "17201", "kana": "イリヨウホウジン ジユウゼンカイ", "name": "医療法人　十全会", "prefecture": "石川県", "city": "金沢市", "neighborhood": "田上本町", "banchi": "カ45-1", "postal_code": "9201185", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タガミホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201182','{"jis": "17201", "kana": "カナザワケイムシヨ", "name": "金沢刑務所", "prefecture": "石川県", "city": "金沢市", "neighborhood": "田上町", "banchi": "公1", "postal_code": "9201182", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タガミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201192','{"jis": "17201", "kana": "カナザワダイガク (カクマキヤンパス)", "name": "金沢大学　（角間キャンパス）", "prefecture": "石川県", "city": "金沢市", "neighborhood": "角間町", "banchi": "1", "postal_code": "9201192", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カクママチ", "alternates": []}');
-INSERT INTO office_data VALUES('9201184','{"jis": "17201", "kana": "ホクリクジヤスコ モリノサトシヨツピングセンタ-", "name": "北陸ジャスコ　杜の里ＳＣ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "もりの里", "banchi": "1丁目70", "postal_code": "9201184", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "モリノサト", "alternates": []}');
 INSERT INTO office_data VALUES('9201180','{"jis": "17201", "kana": "ホクリクダイガク", "name": "北陸大学", "prefecture": "石川県", "city": "金沢市", "neighborhood": "太陽が丘", "banchi": "1丁目1", "postal_code": "9201180", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タイヨウガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('9201181','{"jis": "17201", "kana": "ホクリクダイガク ヤクガクブ", "name": "北陸大学　薬学部", "prefecture": "石川県", "city": "金沢市", "neighborhood": "金川町", "banchi": "ホ3", "postal_code": "9201181", "old_code": "92011", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "カナガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201397','{"jis": "17201", "kana": "イシカワケンリツ タツミガオカコウトウガツコウ", "name": "石川県立　辰巳丘高等学校", "prefecture": "石川県", "city": "金沢市", "neighborhood": "末町", "banchi": "ニ18", "postal_code": "9201397", "old_code": "92013", "post_office": "犀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "スエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201392','{"jis": "17201", "kana": "カナザワガクインダイガク", "name": "金沢学院大学", "prefecture": "石川県", "city": "金沢市", "neighborhood": "末町", "banchi": "10-5-1", "postal_code": "9201392", "old_code": "92013", "post_office": "犀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "スエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201393','{"jis": "17201", "kana": "カナザワガクインダイガクフゾクコウトウガツコウ", "name": "金沢学院大学付属高等学校", "prefecture": "石川県", "city": "金沢市", "neighborhood": "末町", "banchi": "10", "postal_code": "9201393", "old_code": "92013", "post_office": "犀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "スエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9201396','{"jis": "17201", "kana": "ホクリクガクインタンキダイガク", "name": "北陸学院短期大学", "prefecture": "石川県", "city": "金沢市", "neighborhood": "三小牛町", "banchi": "イ11", "postal_code": "9201396", "old_code": "92013", "post_office": "犀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ミツコウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9218517','{"jis": "17201", "kana": "イシカワケンリツ カナザワイズミガオカコウトウガツコウ", "name": "石川県立　金沢泉丘高等学校", "prefecture": "石川県", "city": "金沢市", "neighborhood": "泉野出町", "banchi": "3丁目10-10", "postal_code": "9218517", "old_code": "921  ", "post_office": "金沢南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "イズミノデマチ", "alternates": []}');
@@ -132513,17 +132518,17 @@
 INSERT INTO office_data VALUES('4092193','{"jis": "19366", "kana": "ジエイエイフジカワ トミザワシテン", "name": "ＪＡふじかわ　富沢支店", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "福士", "banchi": "2705-3", "postal_code": "4092193", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "フクシ", "alternates": []}');
 INSERT INTO office_data VALUES('4092195','{"jis": "19366", "kana": "ズイエンカントリ-クラブ センチユリ-フジコ-ス", "name": "随縁カントリー倶楽部　センチュリー富士コース", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "万沢", "banchi": "7079-1", "postal_code": "4092195", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "マンザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4092196','{"jis": "19366", "kana": "チユウオウカガク (カブ) ヤマナシコウジヨウ ダイニジギヨウシヨ", "name": "中央化学　（株）　山梨工場　第二事業所", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "福士", "banchi": "28505-4", "postal_code": "4092196", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "フクシ", "alternates": []}');
 INSERT INTO office_data VALUES('4092192','{"jis": "19366", "kana": "ナンブチヨウヤクバ", "name": "南部町役場", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "福士", "banchi": "28505-2", "postal_code": "4092192", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "フクシ", "alternates": []}');
 INSERT INTO office_data VALUES('4092194','{"jis": "19366", "kana": "フジロイヤルカントリ-クラブ", "name": "富士ロイヤルカントリークラブ", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "万沢", "banchi": "7483", "postal_code": "4092194", "old_code": "40921", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "マンザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4092398','{"jis": "19366", "kana": "ナンブチヨウヤクバ ナンブブンチヨウシヤ", "name": "南部町役場　南部分庁舎", "prefecture": "山梨県", "city": "南巨摩郡南部町", "neighborhood": "内船", "banchi": "4473-1", "postal_code": "4092398", "old_code": "40923", "post_office": "南部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンナンブチョウ", "neighborhood_kana": "ウツブナ", "alternates": []}');
 INSERT INTO office_data VALUES('4000598','{"jis": "19368", "kana": "カブシキガイシヤ ハクバク", "name": "株式会社　はくばく", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "最勝寺", "banchi": "1351", "postal_code": "4000598", "old_code": "40005", "post_office": "青柳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "サイショウジ", "alternates": []}');
-INSERT INTO office_data VALUES('4000593','{"jis": "19368", "kana": "ニスカ カブシキガイシヤ", "name": "ニスカ　株式会社", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "小林", "banchi": "430番地1", "postal_code": "4000593", "old_code": "40005", "post_office": "青柳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "コバヤシ", "alternates": []}');
+INSERT INTO office_data VALUES('4000593','{"jis": "19368", "kana": "キヤノンフアインテツクニスカ カブシキガイシヤ", "name": "キャノンファインテックニスカ　株式会社", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "小林", "banchi": "430番地1", "postal_code": "4000593", "old_code": "40005", "post_office": "青柳", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "コバヤシ", "alternates": []}');
 INSERT INTO office_data VALUES('4000592','{"jis": "19368", "kana": "フジカワチヨウヤクバ", "name": "富士川町役場", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "天神中條", "banchi": "1134番地", "postal_code": "4000592", "old_code": "40005", "post_office": "青柳", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "テンジンナカジョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4000693','{"jis": "19368", "kana": "カジカザワゼイムシヨ", "name": "鰍沢税務署", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "鰍沢", "banchi": "1502-1", "postal_code": "4000693", "old_code": "40006", "post_office": "鰍沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "カジカザワ", "alternates": []}');
+INSERT INTO office_data VALUES('4000693','{"jis": "19368", "kana": "カジカザワゼイムシヨ", "name": "鰍沢税務署", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "鰍沢", "banchi": "1760番地1富士川地方合同庁舎3階", "postal_code": "4000693", "old_code": "40006", "post_office": "鰍沢", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "カジカザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4000695','{"jis": "19368", "kana": "フジカワチヨウヤクバ ブンチヨウシヤ", "name": "富士川町役場　分庁舎", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "鰍沢", "banchi": "1599番地5", "postal_code": "4000695", "old_code": "40006", "post_office": "鰍沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "カジカザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4000692','{"jis": "19368", "kana": "ヤマナシケン キヨウナンチイキケンミンセンタ-", "name": "山梨県　峡南地域県民センター", "prefecture": "山梨県", "city": "南巨摩郡富士川町", "neighborhood": "鰍沢", "banchi": "771-2", "postal_code": "4000692", "old_code": "40006", "post_office": "鰍沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミコマグンフジカワチョウ", "neighborhood_kana": "カジカザワ", "alternates": []}');
 INSERT INTO office_data VALUES('4093897','{"jis": "19384", "kana": "カブシキガイシヤ アピオ", "name": "株式会社　アピオ", "prefecture": "山梨県", "city": "中巨摩郡昭和町", "neighborhood": "西条", "banchi": "3600", "postal_code": "4093897", "old_code": "40938", "post_office": "田富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ナカコマグンショウワチョウ", "neighborhood_kana": "サイジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4093880','{"jis": "19384", "kana": "シヨウワチヨウヤクバ", "name": "昭和町役場", "prefecture": "山梨県", "city": "中巨摩郡昭和町", "neighborhood": "押越", "banchi": "542-2", "postal_code": "4093880", "old_code": "40938", "post_office": "田富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ナカコマグンショウワチョウ", "neighborhood_kana": "オシコシ", "alternates": []}');
 INSERT INTO office_data VALUES('4093883','{"jis": "19384", "kana": "スミトモデンコウデバイス・イノベ-シヨン カブシキガイシヤ", "name": "住友電工デバイス・イノベーション　株式会社", "prefecture": "山梨県", "city": "中巨摩郡昭和町", "neighborhood": "紙漉阿原", "banchi": "1000番地", "postal_code": "4093883", "old_code": "40938", "post_office": "田富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ナカコマグンショウワチョウ", "neighborhood_kana": "カミスキアワラ", "alternates": []}');
 INSERT INTO office_data VALUES('4093895','{"jis": "19384", "kana": "パナソニツクフアクトリ-ソリユ-シヨンズ カブシキガイシヤ", "name": "パナソニックファクトリーソリューションズ　株式会社", "prefecture": "山梨県", "city": "中巨摩郡昭和町", "neighborhood": "紙漉阿原", "banchi": "1375", "postal_code": "4093895", "old_code": "40938", "post_office": "田富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ナカコマグンショウワチョウ", "neighborhood_kana": "カミスキアワラ", "alternates": []}');
 INSERT INTO office_data VALUES('4010592','{"jis": "19424", "kana": "オシノムラヤクバ", "name": "忍野村役場", "prefecture": "山梨県", "city": "南都留郡忍野村", "neighborhood": "忍草", "banchi": "1514", "postal_code": "4010592", "old_code": "40105", "post_office": "山中湖", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマナシケン", "city_kana": "ミナミツルグンオシノムラ", "neighborhood_kana": "シボクサ", "alternates": []}');
@@ -132770,27 +132775,27 @@
 INSERT INTO office_data VALUES('3868551','{"jis": "20203", "kana": "カブシキガイシヤ ニイムラ", "name": "株式会社　新村", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字秋和", "banchi": "199-4", "postal_code": "3868551", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3868710','{"jis": "20203", "kana": "カブシキガイシヤ ハチジユウニギンコウ ウエダシテン", "name": "株式会社　八十二銀行　上田支店", "prefecture": "長野県", "city": "上田市", "neighborhood": "中央", "banchi": "2丁目2-12(上田郵便局私書箱第1号)", "postal_code": "3868710", "old_code": "386  ", "post_office": "上田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3868638','{"jis": "20203", "kana": "カブシキガイシヤ ミツバセイサクジヨ", "name": "株式会社　三葉製作所", "prefecture": "長野県", "city": "上田市", "neighborhood": "中央東", "banchi": "5-14", "postal_code": "3868638", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "チュウオウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('3868634','{"jis": "20203", "kana": "サンヨウデンキ カブシキガイシヤ ウエダジギヨウシヨ カンガワコウジヨウ", "name": "山洋電気　株式会社　上田事業所　神川工場", "prefecture": "長野県", "city": "上田市", "neighborhood": "殿城", "banchi": "5-4", "postal_code": "3868634", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "トノシロ", "alternates": []}');
 INSERT INTO office_data VALUES('3868668','{"jis": "20203", "kana": "シンシユウウエダ ノウギヨウキヨウドウクミアイ", "name": "信州うえだ　農業協同組合", "prefecture": "長野県", "city": "上田市", "neighborhood": "大手", "banchi": "2丁目7-10", "postal_code": "3868668", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "オオテ", "alternates": []}');
 INSERT INTO office_data VALUES('3868567','{"jis": "20203", "kana": "シンシユウダイガク センイガクブ", "name": "信州大学　繊維学部", "prefecture": "長野県", "city": "上田市", "neighborhood": "常田", "banchi": "3丁目15-1", "postal_code": "3868567", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "トキダ", "alternates": []}');
 INSERT INTO office_data VALUES('3868686','{"jis": "20203", "kana": "シンシユウハム カブシキガイシヤ", "name": "信州ハム　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字下塩尻", "banchi": "950", "postal_code": "3868686", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3868666','{"jis": "20203", "kana": "シンワアドヴアンス カブシキガイシヤ", "name": "シンワアドヴァンス　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "材木町", "banchi": "2丁目9-4産業振興ビル6階", "postal_code": "3868666", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "ザイモクチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('3868666','{"jis": "20203", "kana": "シンワアドヴアンス カブシキガイシヤ", "name": "シンワアドヴァンス　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "住吉", "banchi": "21番地5", "postal_code": "3868666", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "スミヨシ", "alternates": []}');
 INSERT INTO office_data VALUES('3868705','{"jis": "20203", "kana": "チユウブデンリヨクパワ-グリツド カブシキガイシヤ ウエダエイギヨウシヨ", "name": "中部電力パワーグリッド　株式会社　上田営業所", "prefecture": "長野県", "city": "上田市", "neighborhood": "中央", "banchi": "1-7-22", "postal_code": "3868705", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3868610','{"jis": "20203", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ シンシユウウエダイリヨウセンター", "name": "独立行政法人　国立病院機構　信州上田医療センター", "prefecture": "長野県", "city": "上田市", "neighborhood": "緑が丘", "banchi": "1-27-21", "postal_code": "3868610", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "ミドリガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3868588','{"jis": "20203", "kana": "ナガイプラスチツク コウギヨウカブシキガイシヤ", "name": "永井プラスチック工業　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "国分", "banchi": "1丁目3-37", "postal_code": "3868588", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "コクブ", "alternates": []}');
 INSERT INTO office_data VALUES('3868501','{"jis": "20203", "kana": "ナガノケイキ カブシキガイシヤ", "name": "長野計器　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字秋和", "banchi": "1150", "postal_code": "3868501", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3868715','{"jis": "20203", "kana": "ナガノケン ウエダコウトウガツコウ", "name": "長野県　上田高等学校", "prefecture": "長野県", "city": "上田市", "neighborhood": "大手", "banchi": "1-4-32", "postal_code": "3868715", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "オオテ", "alternates": []}');
 INSERT INTO office_data VALUES('3868555','{"jis": "20203", "kana": "ナガノケン ウエダゴウドウチヨウシヤ", "name": "長野県　上田合同庁舎", "prefecture": "長野県", "city": "上田市", "neighborhood": "材木町", "banchi": "1丁目2-6", "postal_code": "3868555", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "ザイモクチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3868685','{"jis": "20203", "kana": "ナガノケン ウエダソメヤオカコウトウガツコウ", "name": "長野県　上田染谷丘高等学校", "prefecture": "長野県", "city": "上田市", "neighborhood": "", "banchi": "西丘1710", "postal_code": "3868685", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3868585','{"jis": "20203", "kana": "ナガノケン ウエダチクマコウトウガツコウ", "name": "長野県　上田千曲高等学校", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字中之条", "banchi": "626", "postal_code": "3868585", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3868683','{"jis": "20203", "kana": "ナガノケン ウエダヒガシコウトウガツコウ", "name": "長野県　上田東高等学校", "prefecture": "長野県", "city": "上田市", "neighborhood": "常田", "banchi": "3丁目5-68", "postal_code": "3868683", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "トキダ", "alternates": []}');
 INSERT INTO office_data VALUES('3868553','{"jis": "20203", "kana": "ナベリン カブシキガイシヤ ウエダシテン", "name": "鍋林　株式会社　上田支店", "prefecture": "長野県", "city": "上田市", "neighborhood": "常入", "banchi": "1丁目14-67", "postal_code": "3868553", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "トキイリ", "alternates": []}');
 INSERT INTO office_data VALUES('3868609','{"jis": "20203", "kana": "ハロ-ワ-クウエダ(ウエダコウキヨウシヨクギヨウアンテイジヨ)", "name": "ハローワーク上田（上田公共職業安定所）", "prefecture": "長野県", "city": "上田市", "neighborhood": "天神", "banchi": "2丁目4-70", "postal_code": "3868609", "old_code": "386  ", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "テンジン", "alternates": []}');
-INSERT INTO office_data VALUES('3860192','{"jis": "20203", "kana": "トウキヨウトクシユデンセン カブシキカイシヤ", "name": "東京特殊電線　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字大屋", "banchi": "300", "postal_code": "3860192", "old_code": "38601", "post_office": "大屋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('3860192','{"jis": "20203", "kana": "カブシキガイシヤ トウトク", "name": "株式会社　ＴＯＴＯＫＵ", "prefecture": "長野県", "city": "上田市", "neighborhood": "大屋", "banchi": "300番地", "postal_code": "3860192", "old_code": "38601", "post_office": "上田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "オオヤ", "alternates": []}');
 INSERT INTO office_data VALUES('3868505','{"jis": "20203", "kana": "ニツシンコウギヨウ カブシキガイシヤ", "name": "日信工業　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "大字国分", "banchi": "840", "postal_code": "3868505", "old_code": "38601", "post_office": "上田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3860396','{"jis": "20203", "kana": "カケユビヨウイン", "name": "鹿教湯病院", "prefecture": "長野県", "city": "上田市", "neighborhood": "鹿教湯温泉", "banchi": "1308", "postal_code": "3860396", "old_code": "38603", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カケユオンセン", "alternates": []}');
 INSERT INTO office_data VALUES('3860393','{"jis": "20203", "kana": "ミサヤマビヨウイン", "name": "三才山病院", "prefecture": "長野県", "city": "上田市", "neighborhood": "鹿教湯温泉", "banchi": "1777", "postal_code": "3860393", "old_code": "38603", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カケユオンセン", "alternates": []}');
 INSERT INTO office_data VALUES('3860493','{"jis": "20203", "kana": "イリヨウホウジン マルヤマカイ マルコチユウオウソウゴウビヨウイン", "name": "医療法人　丸山会　丸子中央総合病院", "prefecture": "長野県", "city": "上田市", "neighborhood": "上丸子", "banchi": "335-3(丸子郵便局私書箱第10号)", "postal_code": "3860493", "old_code": "38604", "post_office": "丸子", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カミマルコ", "alternates": []}');
 INSERT INTO office_data VALUES('3860492','{"jis": "20203", "kana": "ウエダシヤクシヨ マルコチイキジチセンタ-", "name": "上田市役所　丸子地域自治センター", "prefecture": "長野県", "city": "上田市", "neighborhood": "上丸子", "banchi": "1612", "postal_code": "3860492", "old_code": "38604", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カミマルコ", "alternates": []}');
 INSERT INTO office_data VALUES('3860498','{"jis": "20203", "kana": "シナノケンシ カブシキカイシヤ", "name": "シナノケンシ　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "上丸子", "banchi": "1078", "postal_code": "3860498", "old_code": "38604", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "カミマルコ", "alternates": []}');
 INSERT INTO office_data VALUES('3860495','{"jis": "20203", "kana": "ニホンデンサンセイミツ カブシキガイシヤ", "name": "日本電産セイミツ　株式会社", "prefecture": "長野県", "city": "上田市", "neighborhood": "中丸子", "banchi": "1771", "postal_code": "3860495", "old_code": "38604", "post_office": "丸子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ウエダシ", "neighborhood_kana": "ナカマルコ", "alternates": []}');
@@ -133286,19 +133291,19 @@
 INSERT INTO office_data VALUES('5038517','{"jis": "21202", "kana": "オオミツ", "name": "大光", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "浅草", "banchi": "2丁目66", "postal_code": "5038517", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "アサクサ", "alternates": []}');
 INSERT INTO office_data VALUES('5038508','{"jis": "21202", "kana": "カ)デリカスイト", "name": "株式会社　デリカスイト", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "築捨町", "banchi": "5丁目77", "postal_code": "5038508", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ツキズテチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038516','{"jis": "21202", "kana": "カブシキガイシヤ ウサミグミ", "name": "株式会社　宇佐美組", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "浅草", "banchi": "1丁目280", "postal_code": "5038516", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "アサクサ", "alternates": []}');
 INSERT INTO office_data VALUES('5038562','{"jis": "21202", "kana": "カブシキガイシヤ オオガキムラタセイサクシヨ", "name": "株式会社　大垣村田製作所", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "荒尾町", "banchi": "1122", "postal_code": "5038562", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "アラオチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038514','{"jis": "21202", "kana": "カブシキガイシヤ カワグチヤス-パ-チエン", "name": "株式会社　川口屋スーパーチェン", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "河間町", "banchi": "1丁目65番地", "postal_code": "5038514", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ガマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038509','{"jis": "21202", "kana": "カブシキガイシヤ セイノ-シヨウジ", "name": "株式会社　セイノー商事", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "田口町", "banchi": "1", "postal_code": "5038509", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "タグチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5031696','{"jis": "21202", "kana": "カブシキガイシヤ マルジユン", "name": "株式会社　丸順", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "上石津町乙坂", "banchi": "130-1", "postal_code": "5031696", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カミイシヅチョウオツサカ", "alternates": []}');
-INSERT INTO office_data VALUES('5038553','{"jis": "21202", "kana": "カブシキガイシヤ ヨシダハム", "name": "株式会社　吉田ハム", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "寿町", "banchi": "1-1", "postal_code": "5038553", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "コトブキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038550','{"jis": "21202", "kana": "ギフケイザイダイガク", "name": "岐阜経済大学", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "北方町", "banchi": "5丁目50", "postal_code": "5038550", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "キタガタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038569','{"jis": "21202", "kana": "コウエキザイダンホウジン ソフトピアジヤパン", "name": "公益財団法人　ソフトピアジャパン", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "加賀野", "banchi": "4丁目1番地の7", "postal_code": "5038569", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カガノ", "alternates": []}');
 INSERT INTO office_data VALUES('5038518','{"jis": "21202", "kana": "サンメツセ カブシキガイシヤ", "name": "サンメッセ　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "久瀬川町", "banchi": "7丁目5-1", "postal_code": "5038518", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "クゼガワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038505','{"jis": "21202", "kana": "シンコウゾウキ", "name": "神鋼造機", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "本今町", "banchi": "1682-2", "postal_code": "5038505", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "モトイマチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5038553','{"jis": "21202", "kana": "ジエイエイゼンノウミ-トフ-ズ カブシキガイシヤ チユウブエイギヨウホンブ ヨシダハムシテン", "name": "ＪＡ全農ミートフーズ　株式会社　中部営業本部　吉田ハム支店", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "寿町", "banchi": "1番地の1", "postal_code": "5038553", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "コトブキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038567','{"jis": "21202", "kana": "スイトピアセンタ-", "name": "スイトピアセンター", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "室本町", "banchi": "5丁目51", "postal_code": "5038567", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ムロホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5038512','{"jis": "21202", "kana": "セイノ-ジヨウホウサ-ビス", "name": "セイノー情報サービス", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "田口町", "banchi": "1", "postal_code": "5038512", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "タグチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038501','{"jis": "21202", "kana": "セイノウウンユ カブシキガイシヤ", "name": "西濃運輸　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "田口町", "banchi": "1", "postal_code": "5038501", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "タグチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038519','{"jis": "21202", "kana": "タイヘイヨウセイコウ", "name": "太平洋精工", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "久瀬川町", "banchi": "7丁目5-8", "postal_code": "5038519", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "クゼガワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038515','{"jis": "21202", "kana": "ダイマルマツシタシヨクヒン カブシキガイシヤ", "name": "大丸松下食品　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "本今", "banchi": "5丁目141", "postal_code": "5038515", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "モトイマ", "alternates": []}');
 INSERT INTO office_data VALUES('5038557','{"jis": "21202", "kana": "ニチデンセイミツコウギヨウ カブシキガイシヤ", "name": "日電精密工業　株式会社", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "三塚町", "banchi": "336", "postal_code": "5038557", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "ミツヅカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5038504','{"jis": "21202", "kana": "ニツポンゴウセイ", "name": "日本合成", "prefecture": "岐阜県", "city": "大垣市", "neighborhood": "神田町", "banchi": "2丁目35", "postal_code": "5038504", "old_code": "503  ", "post_office": "大垣", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "オオガキシ", "neighborhood_kana": "カンダチョウ", "alternates": []}');
@@ -133346,15 +133351,15 @@
 INSERT INTO office_data VALUES('5078605','{"jis": "21204", "kana": "ギフケンリツタジミコウギヨウコウトウガツコウ", "name": "岐阜県立多治見工業高等学校", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "陶元町", "banchi": "207", "postal_code": "5078605", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "トウゲンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078522','{"jis": "21204", "kana": "ギフケンリツタジミビヨウイン", "name": "岐阜県立多治見病院", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "前畑町", "banchi": "5丁目161", "postal_code": "5078522", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "マエバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078603','{"jis": "21204", "kana": "サンギヨウブンカセンタ- シテイカンリシヤ カブシキガイシヤ", "name": "産業文化センター　指定管理者　株式会社", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "新町", "banchi": "1丁目23番地", "postal_code": "5078603", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "シンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5078511','{"jis": "21204", "kana": "シヤカイイリヨウホウジンコウセイカイ タジミシミンビヨウイン", "name": "社会医療法人厚生会　多治見市民病院", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "前畑町", "banchi": "3丁目43", "postal_code": "5078511", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "マエバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078568','{"jis": "21204", "kana": "セレツク カブシキガイシヤ", "name": "セレック　株式会社", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "大薮町", "banchi": "341", "postal_code": "5078568", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "オオヤブチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078523','{"jis": "21204", "kana": "タイヨウシヤデンキ カブシキガイシヤ", "name": "太陽社電気　株式会社", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "小田町", "banchi": "6丁目1", "postal_code": "5078523", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "オダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5078703','{"jis": "21204", "kana": "タジミシヤクシヨ", "name": "多治見市役所", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "日ノ出町", "banchi": "2丁目15(多治見郵便局私書箱第23号)", "postal_code": "5078703", "old_code": "507  ", "post_office": "多治見", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "ヒノデマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5078787','{"jis": "21204", "kana": "タジミシヤクシヨ エキキタチヨウシヤ", "name": "多治見市役所　駅北庁舎", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "音羽町", "banchi": "1丁目233番地", "postal_code": "5078787", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "オトワチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5078787','{"jis": "21204", "kana": "タジミシヤクシヨ エキキタチヨウシヤ", "name": "多治見市役所　駅北庁舎", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "音羽町", "banchi": "1丁目233番地", "postal_code": "5078787", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "オトワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078608','{"jis": "21204", "kana": "タジミシヨウコウカイギシヨ", "name": "多治見商工会議所", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "新町", "banchi": "1丁目23", "postal_code": "5078608", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "シンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5078706','{"jis": "21204", "kana": "タジミゼイムシヨ", "name": "多治見税務署", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "白山町", "banchi": "1丁目29番地の1(多治見郵便局私書箱第46号)", "postal_code": "5078706", "old_code": "507  ", "post_office": "多治見", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "ハクサンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078527','{"jis": "21204", "kana": "チユウブデンリヨク カブシキガイシヤ タジミデンリヨクシヨ", "name": "中部電力　株式会社　多治見電力所", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "上野町", "banchi": "5丁目1番地", "postal_code": "5078527", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "ウエノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078702','{"jis": "21204", "kana": "トウノウシンヨウキンコ", "name": "東濃信用金庫", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "本町", "banchi": "2丁目5-1(多治見郵便局私書箱第2号)", "postal_code": "5078702", "old_code": "507  ", "post_office": "多治見", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5078708','{"jis": "21204", "kana": "トウノセイブソウゴウチヨウシヤ", "name": "東濃西部総合庁舎", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "上野町", "banchi": "5丁目68-1(多治見郵便局私書箱第58号)", "postal_code": "5078708", "old_code": "507  ", "post_office": "多治見", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "ウエノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078701','{"jis": "21204", "kana": "マエバタトウキ カブシキガイシヤ", "name": "前畑陶器　株式会社", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "前畑町", "banchi": "2丁目12(多治見郵便局私書箱第44号)", "postal_code": "5078701", "old_code": "507  ", "post_office": "多治見", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "マエバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5078602','{"jis": "21204", "kana": "ミノホウザイ カブシキガイシヤ", "name": "美濃包材　株式会社", "prefecture": "岐阜県", "city": "多治見市", "neighborhood": "京町", "banchi": "4丁目19-1", "postal_code": "5078602", "old_code": "507  ", "post_office": "多治見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "タジミシ", "neighborhood_kana": "キョウマチ", "alternates": []}');
@@ -133440,15 +133445,15 @@
 INSERT INTO office_data VALUES('5090198','{"jis": "21213", "kana": "(カブ) ヤハタネジ エイチ・アイジギヨウブ", "name": "（株）　八幡ねじ　Ｈ・Ｉ事業部", "prefecture": "岐阜県", "city": "各務原市", "neighborhood": "鵜沼大伊木町", "banchi": "5丁目265-1", "postal_code": "5090198", "old_code": "50901", "post_office": "各務原東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カカミガハラシ", "neighborhood_kana": "ウヌマオオイギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5048710','{"jis": "21213", "kana": "カワサキジユウコウギヨウ カブシキガイシヤ", "name": "川崎重工業　株式会社", "prefecture": "岐阜県", "city": "各務原市", "neighborhood": "川崎町", "banchi": "1(各務原郵便局私書箱第10号)", "postal_code": "5048710", "old_code": "50901", "post_office": "各務原", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カカミガハラシ", "neighborhood_kana": "カワサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5090192','{"jis": "21213", "kana": "ギフシヤタイコウギヨウ カブシキガイシヤ", "name": "岐阜車体工業　株式会社", "prefecture": "岐阜県", "city": "各務原市", "neighborhood": "鵜沼三ツ池町", "banchi": "6丁目455", "postal_code": "5090192", "old_code": "50901", "post_office": "各務原東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カカミガハラシ", "neighborhood_kana": "ウヌマミツイケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5090197','{"jis": "21213", "kana": "セイカツキヨウドウクミアイコ-プギフ", "name": "生活協同組合コープぎふ", "prefecture": "岐阜県", "city": "各務原市", "neighborhood": "鵜沼各務原町", "banchi": "1丁目4番地の1", "postal_code": "5090197", "old_code": "50901", "post_office": "各務原東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カカミガハラシ", "neighborhood_kana": "ウヌマカカミガハラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5090294','{"jis": "21214", "kana": "エフエムラインウエ-ブ カブシキガイシヤ", "name": "ＦＭラインウェーブ　株式会社", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "広見", "banchi": "7-90ケーブルテレビ可児社屋内4F", "postal_code": "5090294", "old_code": "50902", "post_office": "可児", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "ヒロミ", "alternates": []}');
 INSERT INTO office_data VALUES('5090292','{"jis": "21214", "kana": "カニシヤクシヨ", "name": "可児市役所", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "広見", "banchi": "1丁目1(可児郵便局私書箱第2号)", "postal_code": "5090292", "old_code": "50902", "post_office": "可児", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "ヒロミ", "alternates": []}');
 INSERT INTO office_data VALUES('5090296','{"jis": "21214", "kana": "カブシキガイシヤ ニツトクスパ-クテツクトウノウ", "name": "株式会社　日特スパークテック東濃", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "二野", "banchi": "字南山2706番3", "postal_code": "5090296", "old_code": "50902", "post_office": "可児", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "ニノ", "alternates": []}');
-INSERT INTO office_data VALUES('5090289','{"jis": "21214", "kana": "カブシキガイシヤ ベルメゾンロジスコ カニデイストリビユ-シヨンセンタ-", "name": "株式会社　ベルメゾンロジスコ　可児ディストリビューションセンター", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "塩河", "banchi": "2232", "postal_code": "5090289", "old_code": "50902", "post_office": "可児", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "シュウガ", "alternates": []}');
+INSERT INTO office_data VALUES('5090289','{"jis": "21214", "kana": "カブシキガイシヤ ベルメゾンロジスコ カニデイストリビユ-シヨンセンタ-", "name": "株式会社　ベルメゾンロジスコ　可児ディストリビューションセンター", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "塩河", "banchi": "2232", "postal_code": "5090289", "old_code": "50902", "post_office": "可児", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "シュウガ", "alternates": []}');
 INSERT INTO office_data VALUES('5090298','{"jis": "21214", "kana": "カヤバコウギヨウ カブシキガイシヤ ギフキタコウジヨウ", "name": "カヤバ工業　株式会社　岐阜北工場", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "土田", "banchi": "2548", "postal_code": "5090298", "old_code": "50902", "post_office": "可児", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "ドタ", "alternates": []}');
 INSERT INTO office_data VALUES('5090297','{"jis": "21214", "kana": "カヤバコウギヨウ カブシキガイシヤ ギフミナミコウジヨウ", "name": "カヤバ工業　株式会社　岐阜南工場", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "土田", "banchi": "505", "postal_code": "5090297", "old_code": "50902", "post_office": "可児", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "ドタ", "alternates": []}');
 INSERT INTO office_data VALUES('5090293','{"jis": "21214", "kana": "ギフイリヨウカガクダイガク カニキヤンパス", "name": "岐阜医療科学大学　可児キャンパス", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "虹ケ丘", "banchi": "四丁目3番地3", "postal_code": "5090293", "old_code": "50902", "post_office": "可児", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "ニジガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('5090295','{"jis": "21214", "kana": "ダイオウセイシ カブシキガイシヤ カニコウジヨウ", "name": "大王製紙　株式会社　可児工場", "prefecture": "岐阜県", "city": "可児市", "neighborhood": "土田", "banchi": "500番地", "postal_code": "5090295", "old_code": "50902", "post_office": "可児", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "カニシ", "neighborhood_kana": "ドタ", "alternates": []}');
 INSERT INTO office_data VALUES('5012192','{"jis": "21215", "kana": "ヤマガタシヤクシヨ", "name": "山県市役所", "prefecture": "岐阜県", "city": "山県市", "neighborhood": "高木", "banchi": "1000番地の1", "postal_code": "5012192", "old_code": "50121", "post_office": "高富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "ヤマガタシ", "neighborhood_kana": "タカキ", "alternates": []}');
 INSERT INTO office_data VALUES('5012292','{"jis": "21215", "kana": "キタムラゴウキンセイサクシヨ カブシキガイシヤ", "name": "喜多村合金製作所　株式会社", "prefecture": "岐阜県", "city": "山県市", "neighborhood": "富永", "banchi": "868", "postal_code": "5012292", "old_code": "50122", "post_office": "高富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "ヤマガタシ", "neighborhood_kana": "トミナガ", "alternates": []}');
 INSERT INTO office_data VALUES('5010296','{"jis": "21216", "kana": "アサヒダイガク", "name": "朝日大学", "prefecture": "岐阜県", "city": "瑞穂市", "neighborhood": "穂積", "banchi": "1851-1", "postal_code": "5010296", "old_code": "50102", "post_office": "穂積", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "ミズホシ", "neighborhood_kana": "ホヅミ", "alternates": []}');
@@ -134661,15 +134666,15 @@
 INSERT INTO office_data VALUES('4608417','{"jis": "23106", "kana": "ニツセキミツビシ カブシキガイシヤ チユウブシテン", "name": "日石三菱　株式会社　中部支店", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "新栄町", "banchi": "1丁目5番地", "postal_code": "4608417", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "シンサカエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4608525','{"jis": "23106", "kana": "ニツポンデンキ カブシキガイシヤ トウカイシシヤ", "name": "日本電気　株式会社　東海支社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "1丁目17-1NEC中部ビル", "postal_code": "4608525", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
 INSERT INTO office_data VALUES('4608617','{"jis": "23106", "kana": "ニホンカミパルプシヨウジ カブシキカイシヤ チユウブシシヤ", "name": "日本紙パルプ商事　株式会社　中部支社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "丸の内", "banchi": "3丁目22番24号名古屋桜通ビル12階", "postal_code": "4608617", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('4608366','{"jis": "23106", "kana": "ニホンケイザイシンブンシヤ ナゴヤシシヤ", "name": "日本経済新聞社　名古屋支社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "栄", "banchi": "4丁目16-33", "postal_code": "4608366", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "サカエ", "alternates": []}');
 INSERT INTO office_data VALUES('4608506','{"jis": "23106", "kana": "ニホンデンシンデンワ カブシキガイシヤ ナゴヤシテン", "name": "日本電信電話　株式会社　名古屋支店", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "三の丸", "banchi": "1丁目9-1", "postal_code": "4608506", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "サンノマル", "alternates": []}');
 INSERT INTO office_data VALUES('4608567','{"jis": "23106", "kana": "ニホンメナ-ドケシヨウヒン カブシキカイシヤ", "name": "日本メナード化粧品　株式会社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "丸の内", "banchi": "3丁目18-15", "postal_code": "4608567", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('4698793','{"jis": "23106", "kana": "ニホンユウビン カブシキガイシヤ トウカイシシヤ ユウビンジギヨウホンブ (サンシユ)", "name": "日本郵便　株式会社　東海支社　郵便事業本部　（三種）", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "丸の内", "banchi": "3丁目2-5", "postal_code": "4698793", "old_code": "460  ", "post_office": "名古屋神宮", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "マルノウチ", "alternates": []}');
-INSERT INTO office_data VALUES('4608628','{"jis": "23106", "kana": "ニワコウ カブシキガイシヤ", "name": "丹羽幸　株式会社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "二丁目11番6号エフリードビル7階", "postal_code": "4608628", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
+INSERT INTO office_data VALUES('4608628','{"jis": "23106", "kana": "ニワコウ カブシキガイシヤ", "name": "丹羽幸　株式会社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "二丁目11番6号エフリードビル7階", "postal_code": "4608628", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
 INSERT INTO office_data VALUES('4608585','{"jis": "23106", "kana": "フジツウ カブシキガイシヤ トウカイシシヤ", "name": "富士通　株式会社　東海支社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "1丁目10-1", "postal_code": "4608585", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
 INSERT INTO office_data VALUES('4608404','{"jis": "23106", "kana": "フジフイルム カブシキガイシヤ", "name": "富士フイルム　株式会社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "栄", "banchi": "1-12-17富士フイルム名古屋ビル", "postal_code": "4608404", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "サカエ", "alternates": []}');
 INSERT INTO office_data VALUES('4608415','{"jis": "23106", "kana": "ポツカサツポロフ-ドアンドビバレツジ カブシキガイシヤ", "name": "ポッカサッポロフード＆ビバレッジ　株式会社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "栄", "banchi": "4丁目2番29号名古屋広小路プレイス", "postal_code": "4608415", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "サカエ", "alternates": []}');
 INSERT INTO office_data VALUES('4608531','{"jis": "23106", "kana": "マスダ カブシキガイシヤ", "name": "マスダ　株式会社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "丸の内", "banchi": "1丁目8-12", "postal_code": "4608531", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('4608605','{"jis": "23106", "kana": "マツクスバリユチユウブ カブシキカイシヤ ホンシヤジムシヨ", "name": "マックスバリュ中部　株式会社　本社事務所", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "1丁目18番22号", "postal_code": "4608605", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
 INSERT INTO office_data VALUES('4608711','{"jis": "23106", "kana": "マルベニ カブシキガイシヤ チユウブシシヤ", "name": "丸紅　株式会社　中部支社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "2丁目2番2号", "postal_code": "4608711", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
 INSERT INTO office_data VALUES('4608616','{"jis": "23106", "kana": "マンヒヨウ カブシキガイシヤ", "name": "万兵　株式会社", "prefecture": "愛知県", "city": "名古屋市中区", "neighborhood": "錦", "banchi": "2丁目12-14", "postal_code": "4608616", "old_code": "460  ", "post_office": "名古屋中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカク", "neighborhood_kana": "ニシキ", "alternates": []}');
@@ -134962,15 +134967,15 @@
 INSERT INTO office_data VALUES('4658651','{"jis": "23115", "kana": "エレツクヒシキ カブシキガイシヤ", "name": "エレックヒシキ　株式会社", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "一社", "banchi": "4丁目22", "postal_code": "4658651", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "イッシャ", "alternates": []}');
 INSERT INTO office_data VALUES('4658612','{"jis": "23115", "kana": "カブシキガイシヤ アトム", "name": "株式会社　アトム", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "上社", "banchi": "3丁目801", "postal_code": "4658612", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "カミヤシロ", "alternates": []}');
 INSERT INTO office_data VALUES('4658520','{"jis": "23115", "kana": "カブシキガイシヤ コムラ", "name": "株式会社　コムラ", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "社台", "banchi": "3丁目1", "postal_code": "4658520", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "ヤシロダイ", "alternates": []}');
 INSERT INTO office_data VALUES('4658501','{"jis": "23115", "kana": "カブシキガイシヤ チヨダ チユウブチクホンブ", "name": "株式会社　チヨダ　中部地区本部", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "社台", "banchi": "3丁目124", "postal_code": "4658501", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "ヤシロダイ", "alternates": []}');
 INSERT INTO office_data VALUES('4658552','{"jis": "23115", "kana": "カブシキガイシヤ トヨマツク", "name": "株式会社　トヨマック", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "本郷", "banchi": "3丁目147", "postal_code": "4658552", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "ホンゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('4658550','{"jis": "23115", "kana": "カブシキガイシヤ フジ", "name": "株式会社　富士", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "本郷", "banchi": "3丁目148", "postal_code": "4658550", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "ホンゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('4658565','{"jis": "23115", "kana": "カブシキガイシヤ プロトコ-ポレ-シヨン", "name": "株式会社　プロトコーポレーション", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "藤森西町", "banchi": "806-2", "postal_code": "4658565", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "フジモリニシマチ", "alternates": []}');
-INSERT INTO office_data VALUES('4658650','{"jis": "23115", "kana": "コウリツダイガクホウジン ナゴヤシリツダイガク イガクブフゾク ミライコウセイビヨウイン", "name": "公立大学法人　名古屋市立大学　医学部付属　みらい光生病院", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "勢子坊", "banchi": "二丁目1501番地", "postal_code": "4658650", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "セコボウ", "alternates": []}');
+INSERT INTO office_data VALUES('4658650','{"jis": "23115", "kana": "コウリツダイガクホウジン ナゴヤシリツダイガク イガクブフゾク ミライコウセイビヨウイン", "name": "公立大学法人　名古屋市立大学　医学部付属　みらい光生病院", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "勢子坊", "banchi": "二丁目1501番地", "postal_code": "4658650", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "セコボウ", "alternates": []}');
 INSERT INTO office_data VALUES('4658620','{"jis": "23115", "kana": "コクリツリヨウヨウジヨ ヒガシナゴヤビヨウイン", "name": "国立療養所　東名古屋病院", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "梅森坂", "banchi": "5丁目101", "postal_code": "4658620", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "ウメモリザカ", "alternates": []}');
 INSERT INTO office_data VALUES('4658505','{"jis": "23115", "kana": "サンコ-シヨウジ カブシキガイシヤ", "name": "サンコー商事　株式会社", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "高社", "banchi": "2丁目245", "postal_code": "4658505", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "タカヤシロ", "alternates": []}');
 INSERT INTO office_data VALUES('4658567','{"jis": "23115", "kana": "シヨウワヤクヒン カブシキガイシヤ トウカイオフイス", "name": "アルフレッサ　株式会社　東海オフィス", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "本郷", "banchi": "2丁目173-2", "postal_code": "4658567", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "ホンゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('4658510','{"jis": "23115", "kana": "シントウジヨウホウセンタ- カブシキガイシヤ", "name": "新統情報センター　株式会社", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "社台", "banchi": "3丁目109", "postal_code": "4658510", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "ヤシロダイ", "alternates": []}');
 INSERT INTO office_data VALUES('4658560','{"jis": "23115", "kana": "チユウキヨウサンヨウ カブシキガイシヤ", "name": "中京三洋　株式会社", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "本郷", "banchi": "3丁目91", "postal_code": "4658560", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "ホンゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('4658670','{"jis": "23115", "kana": "ト-ヨ-キツチンアンドリビング カブシキガイシヤ", "name": "トーヨーキッチンアンドリビング　株式会社", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "一社", "banchi": "2丁目21番地", "postal_code": "4658670", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシメイトウク", "neighborhood_kana": "イッシャ", "alternates": []}');
 INSERT INTO office_data VALUES('4658611','{"jis": "23115", "kana": "トウカイコ-プジギヨウレンゴウ・メイキンセイキヨウ", "name": "東海コープ事業連合・めいきん生協", "prefecture": "愛知県", "city": "名古屋市名東区", "neighborhood": "猪高町大字上社", "banchi": "字井堀25-1", "postal_code": "4658611", "old_code": "465  ", "post_office": "名東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -135245,15 +135250,15 @@
 INSERT INTO office_data VALUES('4411294','{"jis": "23207", "kana": "オ-エスジ- カブシキガイシヤ", "name": "オーエスジー　株式会社", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "一宮町", "banchi": "上新切450", "postal_code": "4411294", "old_code": "44112", "post_office": "三河一宮", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "イチノミヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4411295','{"jis": "23207", "kana": "カブシキガイシヤ ユ-エ-シ-ジエ-ドウカン", "name": "株式会社　ＵＡＣＪ銅管", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "大木町", "banchi": "新道100", "postal_code": "4411295", "old_code": "44112", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "オオギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4411292','{"jis": "23207", "kana": "トヨカワシイチノミヤソウゴウシシヨ", "name": "豊川市一宮総合支所", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "一宮町", "banchi": "豊1", "postal_code": "4411292", "old_code": "44112", "post_office": "三河一宮", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "イチノミヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4411293','{"jis": "23207", "kana": "トヨカワシンヨウキンコ ジムセンタ-", "name": "豊川信用金庫　事務センター", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "一宮町", "banchi": "幸6(三河一宮郵便局私書箱第1号)", "postal_code": "4411293", "old_code": "44112", "post_office": "三河一宮", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "イチノミヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4428586','{"jis": "23207", "kana": "アイチケンリツコウコウトウガツコウ", "name": "愛知県立国府高等学校", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "国府町", "banchi": "下坊入10-1", "postal_code": "4428586", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "コウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4428573','{"jis": "23207", "kana": "アイチケンリツトヨカワコウギヨウコウトウガツコウ", "name": "愛知県立豊川工業高等学校", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "新道町", "banchi": "1丁目3", "postal_code": "4428573", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "シンミチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4428509','{"jis": "23207", "kana": "アサヒテツク カブシキガイシヤ トヨカワジギヨウシヨ", "name": "旭テック　株式会社　豊川事業所", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "穂ノ原", "banchi": "2丁目10", "postal_code": "4428509", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "ホノハラ", "alternates": []}');
-INSERT INTO office_data VALUES('4428550','{"jis": "23207", "kana": "イオンモ-ルトヨカワ", "name": "イオンモール豊川", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "白鳥町", "banchi": "兎足1番16号", "postal_code": "4428550", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "シロトリチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4428550','{"jis": "23207", "kana": "イオンモ-ルトヨカワ", "name": "イオンモール豊川", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "白鳥町", "banchi": "兎足1番16号", "postal_code": "4428550", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "シロトリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4428531','{"jis": "23207", "kana": "イシグロシヨウジ ユウゲンガイシヤ", "name": "石黒商事　有限会社", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "豊川元町", "banchi": "35", "postal_code": "4428531", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "トヨカワモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4428587','{"jis": "23207", "kana": "イトモル カブシキガイシヤ", "name": "イトモル　株式会社", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "穂ノ原", "banchi": "2丁目1-17", "postal_code": "4428587", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "ホノハラ", "alternates": []}');
 INSERT INTO office_data VALUES('4428588','{"jis": "23207", "kana": "イトモルセイミツカブシキガイシヤ", "name": "イトモル精密株式会社", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "穂ノ原", "banchi": "2丁目1-17", "postal_code": "4428588", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "ホノハラ", "alternates": []}');
 INSERT INTO office_data VALUES('4428543','{"jis": "23207", "kana": "オ-エスジ- カブシキガイシヤ", "name": "オーエスジー　株式会社", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "本野ケ原", "banchi": "3丁目22", "postal_code": "4428543", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "ホンノガハラ", "alternates": []}');
 INSERT INTO office_data VALUES('4428544','{"jis": "23207", "kana": "オ-エスジ- カブシキガイシヤ ア-ルアンドデイ-センタ-", "name": "オーエスジー　株式会社　Ｒ＆Ｄセンター", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "本野ケ原", "banchi": "1丁目15", "postal_code": "4428544", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "ホンノガハラ", "alternates": []}');
 INSERT INTO office_data VALUES('4428577','{"jis": "23207", "kana": "オカダケンセツ カブシキガイシヤ", "name": "岡田建設　株式会社", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "白鳥町", "banchi": "京次52-1", "postal_code": "4428577", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "シロトリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4428576','{"jis": "23207", "kana": "カブシキガイシヤ アイイ-メカトロニクス", "name": "株式会社　アイイーメカトロニクス", "prefecture": "愛知県", "city": "豊川市", "neighborhood": "白鳥町", "banchi": "野口前9番地の5", "postal_code": "4428576", "old_code": "442  ", "post_office": "豊川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨカワシ", "neighborhood_kana": "シロトリチョウ", "alternates": []}');
@@ -135604,15 +135609,15 @@
 INSERT INTO office_data VALUES('4958505','{"jis": "23220", "kana": "アイチケンリツ キヨウワコウトウガツコウ", "name": "愛知県立　杏和高等学校", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町二俣", "banchi": "宮西1番地1", "postal_code": "4958505", "old_code": "495  ", "post_office": "祖父江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウフタマタ", "alternates": []}');
 INSERT INTO office_data VALUES('4958511','{"jis": "23220", "kana": "イナザワシ ソブエシシヨ", "name": "稲沢市　祖父江支所", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町山崎", "banchi": "鶴塚275番地1", "postal_code": "4958511", "old_code": "495  ", "post_office": "一宮", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウヤマザキ", "alternates": []}');
 INSERT INTO office_data VALUES('4958601','{"jis": "23220", "kana": "オウジマテリア カブシキガイシヤ ソブエコウジヨウ", "name": "王子マテリア　株式会社　祖父江工場", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町祖父江", "banchi": "外平150番地", "postal_code": "4958601", "old_code": "495  ", "post_office": "祖父江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウソブエ", "alternates": []}');
 INSERT INTO office_data VALUES('4958517','{"jis": "23220", "kana": "カブシキガイシヤ コメツトカトウ", "name": "株式会社　コメットカトウ", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町甲新田", "banchi": "イ九-65", "postal_code": "4958517", "old_code": "495  ", "post_office": "祖父江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウカブトシンデン", "alternates": []}');
 INSERT INTO office_data VALUES('4958510','{"jis": "23220", "kana": "テイジンテクロス カブシキガイシヤ", "name": "帝人テクロス　株式会社", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "祖父江町四貫", "banchi": "堤外22番地", "postal_code": "4958510", "old_code": "495  ", "post_office": "祖父江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ソブエチョウヨツノキ", "alternates": []}');
 INSERT INTO office_data VALUES('4411392','{"jis": "23221", "kana": "シンシロシヤクシヨ", "name": "新城市役所", "prefecture": "愛知県", "city": "新城市", "neighborhood": "字東入船", "banchi": "115番地", "postal_code": "4411392", "old_code": "44113", "post_office": "新城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4411492','{"jis": "23221", "kana": "シンシロシ ツクデソウゴウシシヨ", "name": "新城市　作手総合支所", "prefecture": "愛知県", "city": "新城市", "neighborhood": "作手高里", "banchi": "字縄手上32番地", "postal_code": "4411492", "old_code": "44114", "post_office": "作手", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "シンシロシ", "neighborhood_kana": "ツクデタカサト", "alternates": []}');
-INSERT INTO office_data VALUES('4411692','{"jis": "23221", "kana": "シンシロシ ホウライソウゴウシシヨ", "name": "新城市　鳳来総合支所", "prefecture": "愛知県", "city": "新城市", "neighborhood": "長篠", "banchi": "字下り筬1-2", "postal_code": "4411692", "old_code": "44116", "post_office": "長篠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "シンシロシ", "neighborhood_kana": "ナガシノ", "alternates": []}');
+INSERT INTO office_data VALUES('4411692','{"jis": "23221", "kana": "シンシロシ ホウライソウゴウシシヨ", "name": "新城市　鳳来総合支所", "prefecture": "愛知県", "city": "新城市", "neighborhood": "長篠", "banchi": "字仲野16番地11", "postal_code": "4411692", "old_code": "44116", "post_office": "長篠", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "シンシロシ", "neighborhood_kana": "ナガシノ", "alternates": []}');
 INSERT INTO office_data VALUES('4768666','{"jis": "23222", "kana": "アイチセイコウ カブシキガイシヤ", "name": "愛知製鋼　株式会社", "prefecture": "愛知県", "city": "東海市", "neighborhood": "荒尾町", "banchi": "ワノ割1(東海北郵便局私書箱第3号)", "postal_code": "4768666", "old_code": "476  ", "post_office": "東海北", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "アラオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768585','{"jis": "23222", "kana": "カゴメ カブシキガイシヤ ウエノコウジヨウ", "name": "カゴメ　株式会社　上野工場", "prefecture": "愛知県", "city": "東海市", "neighborhood": "荒尾町", "banchi": "東屋敷108", "postal_code": "4768585", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "アラオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768577','{"jis": "23222", "kana": "カブシキガイシヤ バンカク ソウホンポ", "name": "株式会社　坂角　総本舗", "prefecture": "愛知県", "city": "東海市", "neighborhood": "荒尾町", "banchi": "甚造15-1", "postal_code": "4768577", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "アラオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768588','{"jis": "23222", "kana": "ガツコウホウジン ナゴヤイシダガクエン セイジヨウダイガク", "name": "学校法人　名古屋石田学園　星城大学", "prefecture": "愛知県", "city": "東海市", "neighborhood": "富貴ノ台", "banchi": "2丁目172", "postal_code": "4768588", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "フキノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('4768510','{"jis": "23222", "kana": "キヨウエイコウギヨウカブシキガイシヤ.キヨウエイコウキカブシキガイシヤ.キヨウエイウンユカブシキガイシヤ.キヨウエイコウアツガスカブシキガイシヤ", "name": "協栄興業株式会社、協栄工機株式会社、協栄運輸株式会社、協栄高圧ガス株式会社", "prefecture": "愛知県", "city": "東海市", "neighborhood": "南柴田町", "banchi": "ルノ割426-4", "postal_code": "4768510", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "ミナミシバタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768686','{"jis": "23222", "kana": "シンニホンセイテツ カブシキガイシヤ ナゴヤセイテツシヨ", "name": "新日本製鐵　株式會社　名古屋製鐵所", "prefecture": "愛知県", "city": "東海市", "neighborhood": "東海町", "banchi": "5丁目3番地1(東海北郵便局私書箱第1号)", "postal_code": "4768686", "old_code": "476  ", "post_office": "東海北", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "トウカイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4768503','{"jis": "23222", "kana": "タイヨウプラスチツク", "name": "大洋プラスチック", "prefecture": "愛知県", "city": "東海市", "neighborhood": "富木島町伏見", "banchi": "4丁目1-8", "postal_code": "4768503", "old_code": "476  ", "post_office": "東海北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トウカイシ", "neighborhood_kana": "フキシママチフシミ", "alternates": []}');
@@ -135751,16 +135756,16 @@
 INSERT INTO office_data VALUES('4818535','{"jis": "23234", "kana": "ナゴヤゲイジユツダイガク ニシキヤンパス", "name": "名古屋芸術大学　西キャンパス", "prefecture": "愛知県", "city": "北名古屋市", "neighborhood": "徳重", "banchi": "西沼65番地", "postal_code": "4818535", "old_code": "481  ", "post_office": "西春", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "キタナゴヤシ", "neighborhood_kana": "トクシゲ", "alternates": []}');
 INSERT INTO office_data VALUES('4818502','{"jis": "23234", "kana": "ナゴヤジユウガクイン", "name": "名古屋自由学院", "prefecture": "愛知県", "city": "北名古屋市", "neighborhood": "熊之庄", "banchi": "古井281", "postal_code": "4818502", "old_code": "481  ", "post_office": "西春", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "キタナゴヤシ", "neighborhood_kana": "クマノショウ", "alternates": []}');
 INSERT INTO office_data VALUES('4818504','{"jis": "23234", "kana": "ナゴヤジユウガクイン タンキダイガク", "name": "名古屋自由学院　短期大学", "prefecture": "愛知県", "city": "北名古屋市", "neighborhood": "熊之庄", "banchi": "古井281", "postal_code": "4818504", "old_code": "481  ", "post_office": "西春", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "キタナゴヤシ", "neighborhood_kana": "クマノショウ", "alternates": []}');
 INSERT INTO office_data VALUES('4818508','{"jis": "23234", "kana": "ニツシンデンキ カブシキガイシヤ", "name": "日進電気　株式会社", "prefecture": "愛知県", "city": "北名古屋市", "neighborhood": "六ツ師", "banchi": "女夫越5", "postal_code": "4818508", "old_code": "481  ", "post_office": "西春", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "キタナゴヤシ", "neighborhood_kana": "ムツシ", "alternates": []}');
 INSERT INTO office_data VALUES('4988502','{"jis": "23235", "kana": "アイチケンコウセイノウギヨウキヨウドウクミアイレンゴウカイ カイナンビヨウイン", "name": "愛知県厚生農業協同組合連合会　海南病院", "prefecture": "愛知県", "city": "弥富市", "neighborhood": "前ケ須町", "banchi": "南本田396", "postal_code": "4988502", "old_code": "498  ", "post_office": "弥富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヤトミシ", "neighborhood_kana": "マエガスチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4988505','{"jis": "23235", "kana": "カブシキガイシヤ カワスミ", "name": "株式会社　川スミ", "prefecture": "愛知県", "city": "弥富市", "neighborhood": "鯏浦町", "banchi": "南前新田215", "postal_code": "4988505", "old_code": "498  ", "post_office": "弥富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヤトミシ", "neighborhood_kana": "ウグイウラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4988501','{"jis": "23235", "kana": "ヤトミシヤクシヨ", "name": "弥富市役所", "prefecture": "愛知県", "city": "弥富市", "neighborhood": "前ケ須町", "banchi": "南本田335", "postal_code": "4988501", "old_code": "498  ", "post_office": "弥富", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヤトミシ", "neighborhood_kana": "マエガスチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4700297','{"jis": "23236", "kana": "シヨウワブツサン カブシキガイシヤ", "name": "昌和物産　株式会社", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "福谷町", "banchi": "下地念古67", "postal_code": "4700297", "old_code": "470  ", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "ウキガイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4700292','{"jis": "23236", "kana": "エヌシ-エ-", "name": "ＮＣＡ", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "莇生町", "banchi": "下永井田20", "postal_code": "4700292", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "アザブチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4700297','{"jis": "23236", "kana": "カブシキカイシヤ コウソク チユウキヨウエイギヨウブ", "name": "株式会社　高速　中京営業部", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "根浦町", "banchi": "七丁目2番地1", "postal_code": "4700297", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "ネウラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4700294','{"jis": "23236", "kana": "カブシキガイシヤ サンゴ", "name": "株式会社　三五", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "福田町", "banchi": "宮下1番1", "postal_code": "4700294", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "フクタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4700293','{"jis": "23236", "kana": "ノリタケカンパニ-", "name": "ノリタケカンパニー", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "三好町", "banchi": "東山300", "postal_code": "4700293", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "ミヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4700295','{"jis": "23236", "kana": "ミヨシシヤクシヨ", "name": "みよし市役所", "prefecture": "愛知県", "city": "みよし市", "neighborhood": "三好町", "banchi": "小坂50", "postal_code": "4700295", "old_code": "47002", "post_office": "三好", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ミヨシシ", "neighborhood_kana": "ミヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4901198','{"jis": "23237", "kana": "アマシヤクシヨ ジモクジチヨウシヤ", "name": "あま市役所　甚目寺庁舎", "prefecture": "愛知県", "city": "あま市", "neighborhood": "甚目寺", "banchi": "二伴田76番地", "postal_code": "4901198", "old_code": "49011", "post_office": "甚目寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アマシ", "neighborhood_kana": "ジモクジ", "alternates": []}');
 INSERT INTO office_data VALUES('4901194','{"jis": "23237", "kana": "カブシキガイシヤ カマクラハム", "name": "株式会社　鎌倉ハム", "prefecture": "愛知県", "city": "あま市", "neighborhood": "中萱津", "banchi": "紺屋田30", "postal_code": "4901194", "old_code": "49011", "post_office": "甚目寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アマシ", "neighborhood_kana": "ナカカヤヅ", "alternates": []}');
 INSERT INTO office_data VALUES('4901193','{"jis": "23237", "kana": "カブシキガイシヤ コ-ワ", "name": "株式会社　コーワ", "prefecture": "愛知県", "city": "あま市", "neighborhood": "西今宿", "banchi": "平割一22", "postal_code": "4901193", "old_code": "49011", "post_office": "甚目寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アマシ", "neighborhood_kana": "ニシイマジュク", "alternates": []}');
 INSERT INTO office_data VALUES('4901296','{"jis": "23237", "kana": "アサヒチユウブシザイ カブシキカイシヤ", "name": "旭中部資材　株式会社", "prefecture": "愛知県", "city": "あま市", "neighborhood": "乙之子", "banchi": "八反田12", "postal_code": "4901296", "old_code": "49012", "post_office": "美和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アマシ", "neighborhood_kana": "オトノコ", "alternates": []}');
@@ -135835,15 +135840,15 @@
 INSERT INTO office_data VALUES('4440192','{"jis": "23501", "kana": "コウタチヨウヤクバ", "name": "幸田町役場", "prefecture": "愛知県", "city": "額田郡幸田町", "neighborhood": "大字菱池", "banchi": "字元林1-1", "postal_code": "4440192", "old_code": "44401", "post_office": "幸田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4440194','{"jis": "23501", "kana": "ソニ-イ-エムシ-エス カブシキカイシヤ コウダテツク", "name": "ソニーイーエムシーエス　株式会社　幸田テック", "prefecture": "愛知県", "city": "額田郡幸田町", "neighborhood": "大字坂崎", "banchi": "字雀ケ入1番地", "postal_code": "4440194", "old_code": "44401", "post_office": "幸田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4490293','{"jis": "23562", "kana": "トウエイイリヨウセンタ-", "name": "東栄医療センター", "prefecture": "愛知県", "city": "北設楽郡東栄町", "neighborhood": "大字三輪", "banchi": "字上栗5番地", "postal_code": "4490293", "old_code": "44902", "post_office": "東栄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4490292','{"jis": "23562", "kana": "トウエイチヨウヤクバ", "name": "東栄町役場", "prefecture": "愛知県", "city": "北設楽郡東栄町", "neighborhood": "大字本郷", "banchi": "字上前畑25", "postal_code": "4490292", "old_code": "44902", "post_office": "東栄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('5100392','{"jis": "24201", "kana": "ツシ カワゲソウゴウシシヨ", "name": "津市　河芸総合支所", "prefecture": "三重県", "city": "津市", "neighborhood": "河芸町浜田", "banchi": "808", "postal_code": "5100392", "old_code": "51003", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "カワゲチョウハマダ", "alternates": []}');
 INSERT INTO office_data VALUES('5148568','{"jis": "24201", "kana": "イオンリテ-ル カブシキガイシヤ イオンツテン", "name": "イオンリテール　株式会社　イオン津店", "prefecture": "三重県", "city": "津市", "neighborhood": "桜橋", "banchi": "3-446", "postal_code": "5148568", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "サクラバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5148501','{"jis": "24201", "kana": "イセワンシリヨウチクサン カブシキガイシヤ", "name": "伊勢湾飼料畜産　株式会社", "prefecture": "三重県", "city": "津市", "neighborhood": "島崎町", "banchi": "24-1", "postal_code": "5148501", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "シマザキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('5148515','{"jis": "24201", "kana": "イツパンシヤダンホウジン ミエケントラツクキヨウカイ", "name": "一般社団法人　三重県トラック協会", "prefecture": "三重県", "city": "津市", "neighborhood": "栄町", "banchi": "一丁目941", "postal_code": "5148515", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
+INSERT INTO office_data VALUES('5148515','{"jis": "24201", "kana": "イツパンシヤダンホウジン ミエケントラツクキヨウカイ", "name": "一般社団法人　三重県トラック協会", "prefecture": "三重県", "city": "津市", "neighborhood": "栄町", "banchi": "一丁目941", "postal_code": "5148515", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5148530','{"jis": "24201", "kana": "イムラヤセイカ カブシキガイシヤ", "name": "井村屋製菓　株式会社", "prefecture": "三重県", "city": "津市", "neighborhood": "高茶屋", "banchi": "7丁目1-1", "postal_code": "5148530", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "タカヂャヤ", "alternates": []}');
 INSERT INTO office_data VALUES('5148508','{"jis": "24201", "kana": "イリヨウホウジン ナガイビヨウイン", "name": "医療法人　永井病院", "prefecture": "三重県", "city": "津市", "neighborhood": "西丸之内", "banchi": "29-29", "postal_code": "5148508", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "ニシマルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('5148557','{"jis": "24201", "kana": "カブシキガイシヤ ゼツトテイヴイ", "name": "株式会社　ＺＴＶ", "prefecture": "三重県", "city": "津市", "neighborhood": "あのつ台", "banchi": "4丁目7番地1", "postal_code": "5148557", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "アノツダイ", "alternates": []}');
 INSERT INTO office_data VALUES('5148585','{"jis": "24201", "kana": "カブシキガイシヤ ト-エネツク ミエシテン", "name": "株式会社　トーエネック　三重支店", "prefecture": "三重県", "city": "津市", "neighborhood": "桜橋", "banchi": "2丁目177-1", "postal_code": "5148585", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "サクラバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5148513','{"jis": "24201", "kana": "カブシキガイシヤ ヒサイヤ", "name": "株式会社　久居屋", "prefecture": "三重県", "city": "津市", "neighborhood": "岩田", "banchi": "7-23", "postal_code": "5148513", "old_code": "514  ", "post_office": "津中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "イワタ", "alternates": []}');
 INSERT INTO office_data VALUES('5148666','{"jis": "24201", "kana": "カブシキガイシヤ ヒヤクゴギンコウ", "name": "株式会社　百五銀行", "prefecture": "三重県", "city": "津市", "neighborhood": "岩田", "banchi": "21番27号(津中央郵便局私書箱第5号)", "postal_code": "5148666", "old_code": "514  ", "post_office": "津中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "イワタ", "alternates": []}');
 INSERT INTO office_data VALUES('5148667','{"jis": "24201", "kana": "カブシキガイシヤ ヒヤクゴギンコウ", "name": "株式会社　百五銀行", "prefecture": "三重県", "city": "津市", "neighborhood": "丸之内", "banchi": "31番21号(津中央郵便局私書箱第36号)", "postal_code": "5148667", "old_code": "514  ", "post_office": "津中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ツシ", "neighborhood_kana": "マルノウチ", "alternates": []}');
@@ -136667,15 +136672,15 @@
 INSERT INTO office_data VALUES('5338555','{"jis": "27114", "kana": "カブシキガイシヤ キ-エンス", "name": "株式会社　キーエンス", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "東中島", "banchi": "1丁目3-14", "postal_code": "5338555", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ヒガシナカジマ", "alternates": []}');
 INSERT INTO office_data VALUES('5338585','{"jis": "27114", "kana": "カブシキガイシヤ ダイヤモンドプレス", "name": "株式会社　ダイヤモンドプレス", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "豊新", "banchi": "4丁目21-1", "postal_code": "5338585", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ホウシン", "alternates": []}');
 INSERT INTO office_data VALUES('5338651','{"jis": "27114", "kana": "サンテンセイヤク カブシキガイシヤ", "name": "参天製薬　株式会社", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "下新庄", "banchi": "3丁目9番31号", "postal_code": "5338651", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "シモシンジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5338502','{"jis": "27114", "kana": "スギモトシヨウジ カブシキガイシヤ ホンシヤ", "name": "杉本商事　株式会社　本社", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "豊新", "banchi": "5-6-27", "postal_code": "5338502", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ホウシン", "alternates": []}');
 INSERT INTO office_data VALUES('5338501','{"jis": "27114", "kana": "ヒガシヨドガワクヤクシヨ", "name": "東淀川区役所", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "豊新", "banchi": "2丁目1-4", "postal_code": "5338501", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ホウシン", "alternates": []}');
 INSERT INTO office_data VALUES('5338558','{"jis": "27114", "kana": "ライフコ-ポレ-シヨン", "name": "ライフコーポレーション", "prefecture": "大阪府", "city": "大阪市東淀川区", "neighborhood": "東中島", "banchi": "1丁目19-4", "postal_code": "5338558", "old_code": "533  ", "post_office": "東淀川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシヨドガワク", "neighborhood_kana": "ヒガシナカジマ", "alternates": []}');
 INSERT INTO office_data VALUES('5378686','{"jis": "27115", "kana": "コクヨ カブシキガイシヤ", "name": "コクヨ　（株）", "prefecture": "大阪府", "city": "大阪市東成区", "neighborhood": "大今里南", "banchi": "6丁目1-1(東成郵便局私書箱第5号)", "postal_code": "5378686", "old_code": "537  ", "post_office": "東成", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシナリク", "neighborhood_kana": "オオイマザトミナミ", "alternates": []}');
-INSERT INTO office_data VALUES('5378911','{"jis": "27115", "kana": "ザ・パツク カブシキガイシヤ", "name": "ザ・パック　株式会社", "prefecture": "大阪府", "city": "大阪市東成区", "neighborhood": "東小橋", "banchi": "2丁目9番9号", "postal_code": "5378911", "old_code": "537  ", "post_office": "東成", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシナリク", "neighborhood_kana": "ヒガシオバセ", "alternates": []}');
+INSERT INTO office_data VALUES('5378911','{"jis": "27115", "kana": "ザ・パツク カブシキガイシヤ", "name": "ザ・パック　株式会社", "prefecture": "大阪府", "city": "大阪市東成区", "neighborhood": "東小橋", "banchi": "2丁目9番3号", "postal_code": "5378911", "old_code": "537  ", "post_office": "東成", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシナリク", "neighborhood_kana": "ヒガシオバセ", "alternates": []}');
 INSERT INTO office_data VALUES('5378501','{"jis": "27115", "kana": "ヒガシナリクヤクシヨ", "name": "東成区役所", "prefecture": "大阪府", "city": "大阪市東成区", "neighborhood": "大今里西", "banchi": "2丁目8-4", "postal_code": "5378501", "old_code": "537  ", "post_office": "東成", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシヒガシナリク", "neighborhood_kana": "オオイマザトニシ", "alternates": []}');
 INSERT INTO office_data VALUES('5448501','{"jis": "27116", "kana": "イクノクヤクシヨ", "name": "生野区役所", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "勝山南", "banchi": "3丁目1-19", "postal_code": "5448501", "old_code": "544  ", "post_office": "生野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "カツヤマミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('5448555','{"jis": "27116", "kana": "イクノゼイムシヨ", "name": "生野税務署", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "勝山北", "banchi": "5丁目22-14", "postal_code": "5448555", "old_code": "544  ", "post_office": "生野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "カツヤマキタ", "alternates": []}');
 INSERT INTO office_data VALUES('5448585','{"jis": "27116", "kana": "カブシキガイシヤ モリタホ-ルデイングス", "name": "株式会社　モリタホールディングス", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "小路東", "banchi": "5丁目5番20号", "postal_code": "5448585", "old_code": "544  ", "post_office": "生野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "ショウジヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('5448686','{"jis": "27116", "kana": "シヨウエイインサツ カブシキガイシヤ", "name": "昌栄印刷　株式会社", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "桃谷", "banchi": "1丁目3番23号", "postal_code": "5448686", "old_code": "544  ", "post_office": "生野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "モモダニ", "alternates": []}');
 INSERT INTO office_data VALUES('5448666','{"jis": "27116", "kana": "ロ-トセイヤク カブシキガイシヤ", "name": "ロート製薬　株式会社", "prefecture": "大阪府", "city": "大阪市生野区", "neighborhood": "巽西", "banchi": "1丁目8-1(生野郵便局私書箱第1号)", "postal_code": "5448666", "old_code": "544  ", "post_office": "生野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシイクノク", "neighborhood_kana": "タツミニシ", "alternates": []}');
 INSERT INTO office_data VALUES('5358555','{"jis": "27117", "kana": "アサヒ ゼイムシヨ", "name": "旭　税務署", "prefecture": "大阪府", "city": "大阪市旭区", "neighborhood": "大宮", "banchi": "1丁目1-25", "postal_code": "5358555", "old_code": "535  ", "post_office": "大阪旭", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシアサヒク", "neighborhood_kana": "オオミヤ", "alternates": []}');
@@ -136970,27 +136975,27 @@
 INSERT INTO office_data VALUES('5418572','{"jis": "27128", "kana": "エスエムビ-シ-フアイナンスサ-ビス (カ", "name": "ＳＭＢＣファイナンスサービス　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "4丁目5番15号", "postal_code": "5418572", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418540','{"jis": "27128", "kana": "エヌアイテイジンシヨウジ カブシキガイシヤ", "name": "ＮＩ帝人商事　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南本町", "banchi": "1丁目6-7", "postal_code": "5418540", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418765','{"jis": "27128", "kana": "エレコム カブシキガイシヤ", "name": "エレコム　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "4丁目1番1号明治安田生命大阪御堂筋ビル9階", "postal_code": "5418765", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418541','{"jis": "27128", "kana": "オ-ミケンシ カブシキカイシヤ", "name": "オーミケンシ　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南本町", "banchi": "4-1-1", "postal_code": "5418541", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418567','{"jis": "27128", "kana": "オオサカコクサイガンセンタ-", "name": "大阪国際がんセンター", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "3丁目1番69号", "postal_code": "5418567", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5418531','{"jis": "27128", "kana": "オオサカシシヨクインロウドウクミアイ", "name": "大阪市職員労働組合", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "2丁目4番7号新瓦町ビル7階", "postal_code": "5418531", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418518','{"jis": "27128", "kana": "オオサカシチユウオウクヤクジヨ", "name": "大阪市中央区役所", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "1丁目2-27", "postal_code": "5418518", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5418589','{"jis": "27128", "kana": "オザツクス カブシキガイシヤ", "name": "オザックス　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "博労町", "banchi": "1丁目6-6", "postal_code": "5418589", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "バクロウマチ", "alternates": []}');
+INSERT INTO office_data VALUES('5418589','{"jis": "27128", "kana": "オザツクス カブシキガイシヤ", "name": "オザックス　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "北浜", "banchi": "3丁目5番29号-13階", "postal_code": "5418589", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キタハマ", "alternates": []}');
 INSERT INTO office_data VALUES('5418526','{"jis": "27128", "kana": "オノヤクヒンコウギヨウ カブシキガイシヤ", "name": "小野薬品工業　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "道修町", "banchi": "2丁目1-5", "postal_code": "5418526", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ドショウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418560','{"jis": "27128", "kana": "カネマツ カブシキガイシヤ オオサカシシヤ", "name": "兼松　株式会社　大阪支社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "淡路町", "banchi": "3-1-9", "postal_code": "5418560", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "アワジマチ", "alternates": []}');
+INSERT INTO office_data VALUES('5418528','{"jis": "27128", "kana": "カブシキカイシヤ ニツケンセツケイ", "name": "株式会社　日建設計", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "3-6-5", "postal_code": "5418528", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5416666','{"jis": "27128", "kana": "カブシキガイシヤ オオニシ", "name": "株式会社　大西", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "3-4-12", "postal_code": "5416666", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418630','{"jis": "27128", "kana": "カブシキガイシヤ オオバヤシグミ", "name": "株式会社　大林組", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "北浜", "banchi": "三丁目5番29号", "postal_code": "5418630", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キタハマ", "alternates": []}');
 INSERT INTO office_data VALUES('5418561','{"jis": "27128", "kana": "カブシキガイシヤ サンケイリビングシンブンシヤ", "name": "株式会社　サンケイリビング新聞社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "2丁目6番6号", "postal_code": "5418561", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5418528','{"jis": "27128", "kana": "カブシキガイシヤ ニツケンセツケイ", "name": "株式会社　日建設計", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "高麗橋", "banchi": "4丁目6-2", "postal_code": "5418528", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "コウライバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418515','{"jis": "27128", "kana": "カブシキガイシヤ ニホンケイザイシンブンシヤ オオサカホンシヤ", "name": "株式会社　日本経済新聞社　大阪本社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "高麗橋", "banchi": "1丁目4番2号", "postal_code": "5418515", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "コウライバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418503','{"jis": "27128", "kana": "カブシキガイシヤ プロル-トマルコウ", "name": "株式会社　プロルート丸光", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "2丁目1-5", "postal_code": "5418503", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5408630','{"jis": "27128", "kana": "カブシキガイシヤ ミズホギンコウ オオサカシテン", "name": "株式会社　みずほ銀行　大阪支店", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "4丁目2-1(大阪東郵便局私書箱第145号)", "postal_code": "5408630", "old_code": "541  ", "post_office": "大阪東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418535','{"jis": "27128", "kana": "カブシキガイシヤ ミツビシトウキヨウユ-エフジエイギンコウ オオサカチユウオウシテン", "name": "株式会社　三菱東京ＵＦＪ銀行　大阪中央支店", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "3丁目5-6", "postal_code": "5418535", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418530','{"jis": "27128", "kana": "カブシキガイシヤ ミツビシユ-エフジエイギンコウ", "name": "株式会社　三菱ＵＦＪ銀行", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "3-5-6", "postal_code": "5418530", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5418575','{"jis": "27128", "kana": "カブシキガイシヤ メイセイシヨウカイ", "name": "株式会社　明成商会", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "4丁目4-1日生伏見町ビル本館5F", "postal_code": "5418575", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
+INSERT INTO office_data VALUES('5418575','{"jis": "27128", "kana": "カブシキガイシヤ メイセイシヨウカイ", "name": "株式会社　明成商会", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "2丁目4番10号淀屋橋北浜センタービル2階", "postal_code": "5418575", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418517','{"jis": "27128", "kana": "カブシキガイシヤ モリモトグミ", "name": "株式会社　森本組", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南本町", "banchi": "2-6-12サンマリオンNBFタワー", "postal_code": "5418517", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418523','{"jis": "27128", "kana": "カンサイペイント カブシキガイシヤ", "name": "関西ペイント　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "今橋", "banchi": "2丁目6-14", "postal_code": "5418523", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "イマバシ", "alternates": []}');
 INSERT INTO office_data VALUES('5418513','{"jis": "27128", "kana": "キスコ カブシキガイシヤ オオサカホンシヤ", "name": "ＫＩＳＣＯ　株式会社　大阪本社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "伏見町", "banchi": "三丁目3番7号", "postal_code": "5418513", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "フシミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418519','{"jis": "27128", "kana": "キヨクトウカイハツコウギヨウ カブシキカイシヤ", "name": "極東開発工業　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "淡路町", "banchi": "二丁目5番11号", "postal_code": "5418519", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "アワジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418563','{"jis": "27128", "kana": "キヨクヨウ カブシキガイシヤ", "name": "旭洋　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "瓦町", "banchi": "3-1-15", "postal_code": "5418563", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "カワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418506','{"jis": "27128", "kana": "キヨハラ カブシキガイシヤ", "name": "清原　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南久宝寺町", "banchi": "4丁目5-2", "postal_code": "5418506", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミキュウホウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5418581','{"jis": "27128", "kana": "クラシキボウセキ カブシキガイシヤ", "name": "倉敷紡績　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "2丁目4-31", "postal_code": "5418581", "old_code": "541  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
@@ -137118,15 +137123,15 @@
 INSERT INTO office_data VALUES('5608560','{"jis": "27203", "kana": "トヨナカネンキンジムシヨ", "name": "豊中年金事務所", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "岡上の町", "banchi": "4丁目3-40", "postal_code": "5608560", "old_code": "560  ", "post_office": "豊中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "オカカミノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5608552','{"jis": "27203", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ トネヤマビヨウイン", "name": "独立行政法人　国立病院機構　刀根山病院", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "刀根山", "banchi": "5丁目1番1号", "postal_code": "5608552", "old_code": "560  ", "post_office": "豊中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "トネヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('5608551','{"jis": "27203", "kana": "ハンキユウバス カブシキガイシヤ", "name": "阪急バス　株式会社", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "岡上の町", "banchi": "1丁目1番16号", "postal_code": "5608551", "old_code": "560  ", "post_office": "豊中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "オカカミノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5608543','{"jis": "27203", "kana": "パナソニツク ホ-ムズ カブシキカイシヤ", "name": "パナソニック　ホームズ　株式会社", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "新千里西町", "banchi": "1丁目1番4号", "postal_code": "5608543", "old_code": "560  ", "post_office": "豊中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "シンセンリニシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5618550','{"jis": "27203", "kana": "カブシキガイシヤ イ-パツク", "name": "株式会社　イーパック", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "日出町", "banchi": "1丁目6-22", "postal_code": "5618550", "old_code": "561  ", "post_office": "豊中南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "ヒノデチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5618555','{"jis": "27203", "kana": "ガツコウホウジン オオサカオンガクダイガク", "name": "学校法人　大阪音楽大学", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "庄内幸町", "banchi": "1丁目1-8", "postal_code": "5618555", "old_code": "561  ", "post_office": "豊中南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "ショウナイサイワイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5618577','{"jis": "27203", "kana": "ガツコウホウジン ダイシヨウガクエン ダイシヨウガクエンコウトウガツコウ", "name": "学校法人　大商学園　大商学園高等学校", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "利倉東", "banchi": "1丁目2番1号", "postal_code": "5618577", "old_code": "561  ", "post_office": "豊中南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "トクラヒガシ", "alternates": []}');
-INSERT INTO office_data VALUES('5618530','{"jis": "27203", "kana": "シキシマセイパン カブシキガイシヤ パスコウエストカンパニ-オオサカトヨナカコウジヨウ", "name": "敷島製パン　株式会社　パスコウエストカンパニー大阪豊中工場", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "名神口", "banchi": "1丁目10-1", "postal_code": "5618530", "old_code": "561  ", "post_office": "豊中南", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "メイシングチ", "alternates": []}');
+INSERT INTO office_data VALUES('5618530','{"jis": "27203", "kana": "シキシマセイパン カブシキガイシヤ パスコウエストカンパニ-オオサカトヨナカコウジヨウ", "name": "敷島製パン　株式会社　パスコウエストカンパニー大阪豊中工場", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "名神口", "banchi": "1丁目10-1", "postal_code": "5618530", "old_code": "561  ", "post_office": "豊中南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "メイシングチ", "alternates": []}');
 INSERT INTO office_data VALUES('5618558','{"jis": "27203", "kana": "マツオデンキ カブシキガイシヤ", "name": "松尾電機　株式会社", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "千成町", "banchi": "3丁目5-3", "postal_code": "5618558", "old_code": "561  ", "post_office": "豊中南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "センナリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5608579','{"jis": "27203", "kana": "カブシキガイシヤ オ-トバツクスセブン", "name": "株式会社　オートバックスセブン", "prefecture": "大阪府", "city": "豊中市", "neighborhood": "新千里東町", "banchi": "1丁目5-3", "postal_code": "5608579", "old_code": "565  ", "post_office": "吹田千里", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "トヨナカシ", "neighborhood_kana": "シンセンリヒガシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5638588','{"jis": "27204", "kana": "オオサカフ トヨノフゼイジムシヨ", "name": "大阪府　豊能府税事務所", "prefecture": "大阪府", "city": "池田市", "neighborhood": "城南", "banchi": "1丁目1番1号", "postal_code": "5638588", "old_code": "563  ", "post_office": "池田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イケダシ", "neighborhood_kana": "ジョウナン", "alternates": []}');
 INSERT INTO office_data VALUES('5638567','{"jis": "27204", "kana": "オオサカホウムキヨク イケダシユツチヨウシヨ", "name": "大阪法務局　池田出張所", "prefecture": "大阪府", "city": "池田市", "neighborhood": "満寿美町", "banchi": "9番25号", "postal_code": "5638567", "old_code": "563  ", "post_office": "池田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イケダシ", "neighborhood_kana": "マスミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5638510','{"jis": "27204", "kana": "シリツ イケダビヨウイン", "name": "市立　池田病院", "prefecture": "大阪府", "city": "池田市", "neighborhood": "城南", "banchi": "3丁目1番18号", "postal_code": "5638510", "old_code": "563  ", "post_office": "池田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イケダシ", "neighborhood_kana": "ジョウナン", "alternates": []}');
 INSERT INTO office_data VALUES('5638577','{"jis": "27204", "kana": "ドクリツギヨウセイホウジン サンギヨウギジユツソウゴウケンキユウシヨ カンサイセンタ-", "name": "独立行政法人　産業技術総合研究所　関西センター", "prefecture": "大阪府", "city": "池田市", "neighborhood": "緑丘", "banchi": "1丁目8番31号", "postal_code": "5638577", "old_code": "563  ", "post_office": "池田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イケダシ", "neighborhood_kana": "ミドリガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('5648511','{"jis": "27205", "kana": "オオサカガクインダイガク", "name": "大阪学院大学", "prefecture": "大阪府", "city": "吹田市", "neighborhood": "岸部南", "banchi": "2丁目36-1", "postal_code": "5648511", "old_code": "564  ", "post_office": "吹田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "スイタシ", "neighborhood_kana": "キシベミナミ", "alternates": []}');
@@ -137251,14 +137256,15 @@
 INSERT INTO office_data VALUES('5678520','{"jis": "27211", "kana": "マルカキカイ カブシキガイシヤ", "name": "マルカキカイ　株式会社", "prefecture": "大阪府", "city": "茨木市", "neighborhood": "五日市緑町", "banchi": "2-28", "postal_code": "5678520", "old_code": "567  ", "post_office": "茨木", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イバラキシ", "neighborhood_kana": "イツカイチミドリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5678570','{"jis": "27211", "kana": "リツメイカンダイガク オオサカイバラキキヤンパス", "name": "立命館大学　大阪いばらきキャンパス", "prefecture": "大阪府", "city": "茨木市", "neighborhood": "岩倉町", "banchi": "2-150", "postal_code": "5678570", "old_code": "567  ", "post_office": "茨木", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イバラキシ", "neighborhood_kana": "イワクラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5818511','{"jis": "27212", "kana": "オオサカケイザイホウカダイガク", "name": "大阪経済法科大学", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "楽音寺", "banchi": "6-10", "postal_code": "5818511", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ガクオンジ", "alternates": []}');
 INSERT INTO office_data VALUES('5818686','{"jis": "27212", "kana": "カブシキカイシヤ クボタ キユウホウジジギヨウセンタ-", "name": "株式会社　クボタ　久宝寺事業センター", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "神武町", "banchi": "2番35号", "postal_code": "5818686", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ジンムチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5818558','{"jis": "27212", "kana": "カブシキガイシヤ ミキハウス", "name": "株式会社　ミキハウス", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "若林町", "banchi": "1丁目76-2", "postal_code": "5818558", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ワカバヤシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5818539','{"jis": "27212", "kana": "カブシキガイシヤ ヤラカスカン プロダクトセンタ-", "name": "（株）　ヤラカス舘　プロダクトセンター", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "若林町", "banchi": "2丁目119", "postal_code": "5818539", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ワカバヤシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5818585','{"jis": "27212", "kana": "シヤ-プ カブシキガイシヤ スマ-トアプライアンスアンドソリユ-シヨンジギヨウホンブ", "name": "シャープ　株式会社　Ｓｍａｒｔ　Ａｐｐｌｉａｎｃｅｓ＆Ｓｏｌｕｔｉｏｎｓ事業本部", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "北亀井町", "banchi": "3丁目1番72号", "postal_code": "5818585", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "キタカメイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5818502','{"jis": "27212", "kana": "ジエイピ-ラクテンロジステイクス カブシキガイシヤ ラクテンフルフイルメントセンタ-ヤオ", "name": "ＪＰ楽天ロジスティクス　株式会社　楽天フルフィルメントセンター八尾", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "郡川", "banchi": "一丁目557GLP八尾Ⅰ", "postal_code": "5818502", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "コオリガワ", "alternates": []}');
 INSERT INTO office_data VALUES('5818505','{"jis": "27212", "kana": "ミキシヨウコウ カブシキガイシヤ", "name": "三起商行　株式会社", "prefecture": "大阪府", "city": "八尾市", "neighborhood": "若林町", "banchi": "1丁目76-2", "postal_code": "5818505", "old_code": "581  ", "post_office": "八尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヤオシ", "neighborhood_kana": "ワカバヤシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5498522','{"jis": "27213", "kana": "キタカウンタ- カンサイクウコウタ-ミナル 4エフコクサイセンシユツパツロビ-・1エフコクサイセントウチヤクロビ-", "name": "北カウンター　関西空港ターミナル　４Ｆ国際線出発ロビー・１Ｆ国際線到着ロビー", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "泉州空港北", "banchi": "1番地", "postal_code": "5498522", "old_code": "549  ", "post_office": "大阪国際", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "センシュウクウコウキタ", "alternates": []}');
 INSERT INTO office_data VALUES('5988503','{"jis": "27213", "kana": "イズミサノ ゼイムシヨ", "name": "泉佐野　税務署", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "日根野", "banchi": "3683-1", "postal_code": "5988503", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "ヒネノ", "alternates": []}');
 INSERT INTO office_data VALUES('5988550','{"jis": "27213", "kana": "イズミサノシヤクシヨ", "name": "泉佐野市役所", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "市場東", "banchi": "1丁目295-3", "postal_code": "5988550", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "イチバヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('5988560','{"jis": "27213", "kana": "オオサカフリツ サノコウギヨウコウトウガツコウ", "name": "大阪府立　佐野工業高等学校", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "高松東", "banchi": "1丁目3-50", "postal_code": "5988560", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "タカマツヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('5988531','{"jis": "27213", "kana": "オオサカフリツダイガク リンクウキヤンパス", "name": "大阪府立大学　りんくうキャンパス", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "りんくう往来北", "banchi": "1-58", "postal_code": "5988531", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "リンクウオウライキタ", "alternates": []}');
 INSERT INTO office_data VALUES('5988522','{"jis": "27213", "kana": "カンサイエアポ-トワシントンホテル", "name": "関西エアポートワシントンホテル", "prefecture": "大阪府", "city": "泉佐野市", "neighborhood": "りんくう往来北", "banchi": "1-7", "postal_code": "5988522", "old_code": "598  ", "post_office": "泉佐野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "イズミサノシ", "neighborhood_kana": "リンクウオウライキタ", "alternates": []}');
@@ -137623,15 +137629,14 @@
 INSERT INTO office_data VALUES('6728666','{"jis": "28201", "kana": "ヨコタセキユ カブシキガイシヤ", "name": "横田石油　株式会社", "prefecture": "兵庫県", "city": "姫路市", "neighborhood": "飾磨区恵美酒", "banchi": "147(姫路南郵便局私書箱第6号)", "postal_code": "6728666", "old_code": "672  ", "post_office": "姫路南", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "ヒメジシ", "neighborhood_kana": "シカマクエビス", "alternates": []}');
 INSERT INTO office_data VALUES('6794298','{"jis": "28201", "kana": "ヤエガキ カブシキガイシヤ", "name": "ヤヱガキ　株式会社", "prefecture": "兵庫県", "city": "姫路市", "neighborhood": "林田町六九谷", "banchi": "681(林田郵便局私書箱第1号)", "postal_code": "6794298", "old_code": "67942", "post_office": "林田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "ヒメジシ", "neighborhood_kana": "ハヤシダチョウムクダニ", "alternates": []}');
 INSERT INTO office_data VALUES('6608544','{"jis": "28202", "kana": "アマガサキ ゼイムシヨ", "name": "尼崎　税務署", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "西難波町", "banchi": "1丁目8-1", "postal_code": "6608544", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ニシナニワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608501','{"jis": "28202", "kana": "アマガサキシヤクシヨ", "name": "尼崎市役所", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "東七松町", "banchi": "1丁目23-1", "postal_code": "6608501", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ヒガシナナマツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608582','{"jis": "28202", "kana": "アマゾンアマガサキエフシ-", "name": "アマゾン尼崎ＦＣ", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "東海岸町", "banchi": "20-1", "postal_code": "6608582", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ヒガシカイガンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608540','{"jis": "28202", "kana": "カブシキガイシヤ エデイオン", "name": "株式会社　エディオン", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "潮江", "banchi": "1丁目1-50", "postal_code": "6608540", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "シオエ", "alternates": []}');
 INSERT INTO office_data VALUES('6608533','{"jis": "28202", "kana": "カブシキガイシヤ オオサカチタニウムテクノロジ-ズ", "name": "株式会社　大阪チタニウムテクノロジーズ", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "東浜町", "banchi": "1番地", "postal_code": "6608533", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ヒガシハマチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('6608510','{"jis": "28202", "kana": "カブシキガイシヤ モノタロウ アマガサキデイストリビユ-シヨンセンタ-", "name": "株式会社　ＭｏｎｏｔａＲＯ　尼崎ディストリビューションセンター", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "西向島町", "banchi": "75-1プロロジスパーク尼崎3", "postal_code": "6608510", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ニシムコウジマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608558','{"jis": "28202", "kana": "カンサイデンリヨクソウハイデン カブシキガイシヤ ハンシンハイデンエイギヨウシヨ", "name": "関西電力送配電　株式会社　阪神配電営業所", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "西長洲町", "banchi": "2丁目33-60", "postal_code": "6608558", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ニシナガスチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608567','{"jis": "28202", "kana": "キムラカコウキ カブシキガイシヤ", "name": "木村化工機　株式会社", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "杭瀬寺島", "banchi": "2丁目1番2号", "postal_code": "6608567", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "クイセテラジマ", "alternates": []}');
 INSERT INTO office_data VALUES('6608511','{"jis": "28202", "kana": "ドクリツギヨウセイホウジン ロウドウシヤケンコウフクシキコウ カンサイロウサイビヨウイン", "name": "独立行政法人　労働者健康福祉機構　関西労災病院", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "稲葉荘", "banchi": "3丁目1-69", "postal_code": "6608511", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "イナバソウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608580','{"jis": "28202", "kana": "ニホンヤマムラガラス カブシキガイシヤ", "name": "日本山村硝子　株式会社", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "西向島町", "banchi": "15-1", "postal_code": "6608580", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ニシムコウジマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608555','{"jis": "28202", "kana": "ハンシンミナミケンミンキヨク アマガサキケンゼイジムシヨ", "name": "阪神南県民局　尼崎県税事務所", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "東難波町", "banchi": "5丁目21-8", "postal_code": "6608555", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ヒガシナニワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608588','{"jis": "28202", "kana": "ヒヨウゴケン ハンシンミナミケンミンキヨク", "name": "兵庫県　阪神南県民局", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "東難波町", "banchi": "5丁目21-8", "postal_code": "6608588", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ヒガシナニワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6608550','{"jis": "28202", "kana": "ヒヨウゴケンリツアマガサキソウゴウイリヨウセンタ-", "name": "兵庫県立尼崎総合医療センター", "prefecture": "兵庫県", "city": "尼崎市", "neighborhood": "東難波町", "banchi": "二丁目17番77号", "postal_code": "6608550", "old_code": "660  ", "post_office": "尼崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アマガサキシ", "neighborhood_kana": "ヒガシナニワチョウ", "alternates": []}');
@@ -138202,15 +138207,15 @@
 INSERT INTO office_data VALUES('6492198','{"jis": "30404", "kana": "ユウゲンガイシヤ フカミウメテン", "name": "有限会社　深見梅店", "prefecture": "和歌山県", "city": "西牟婁郡上富田町", "neighborhood": "岩田", "banchi": "2483-1", "postal_code": "6492198", "old_code": "64921", "post_office": "上富田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ワカヤマケン", "city_kana": "ニシムログンカミトンダチョウ", "neighborhood_kana": "イワダ", "alternates": []}');
 INSERT INTO office_data VALUES('6493592','{"jis": "30428", "kana": "クシモトチヨウヤクバ", "name": "串本町役場", "prefecture": "和歌山県", "city": "東牟婁郡串本町", "neighborhood": "串本", "banchi": "1800(串本郵便局私書箱第15号)", "postal_code": "6493592", "old_code": "64935", "post_office": "串本", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ワカヤマケン", "city_kana": "ヒガシムログンクシモトチョウ", "neighborhood_kana": "クシモト", "alternates": []}');
 INSERT INTO office_data VALUES('6494192','{"jis": "30428", "kana": "クシモトチヨウヤクバ コザブンチヨウシヤ", "name": "串本町役場　古座分庁舎", "prefecture": "和歌山県", "city": "東牟婁郡串本町", "neighborhood": "西向", "banchi": "359番地", "postal_code": "6494192", "old_code": "64941", "post_office": "串本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ワカヤマケン", "city_kana": "ヒガシムログンクシモトチョウ", "neighborhood_kana": "ニシムカイ", "alternates": []}');
 INSERT INTO office_data VALUES('6808575','{"jis": "31201", "kana": "カブシキカイシヤ ジヤパンデイスプレイ", "name": "株式会社　ジャパンディスプレイ", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "南吉方", "banchi": "3丁目117-2", "postal_code": "6808575", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "ミナミヨシカタ", "alternates": []}');
 INSERT INTO office_data VALUES('6808588','{"jis": "31201", "kana": "カブシキガイシヤ サンインカラ-ソウゴウゲンゾウジヨ", "name": "株式会社　山陰カラー綜合現像所", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "富安", "banchi": "2丁目70", "postal_code": "6808588", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "トミヤス", "alternates": []}');
 INSERT INTO office_data VALUES('6808533','{"jis": "31201", "kana": "カブシキガイシヤ ナカニシ", "name": "株式会社　ナカニシ", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "富安", "banchi": "2丁目70", "postal_code": "6808533", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "トミヤス", "alternates": []}');
 INSERT INTO office_data VALUES('6808601','{"jis": "31201", "kana": "カブシキガイシヤ マルユウ", "name": "株式会社　丸由", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "今町", "banchi": "2丁目151番地", "postal_code": "6808601", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "イママチ", "alternates": []}');
-INSERT INTO office_data VALUES('6808634','{"jis": "31201", "kana": "カブシキガイシヤ リムノ", "name": "株式会社　ＬＩＭＮＯ", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "立川町", "banchi": "7丁目101番地", "postal_code": "6808634", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "タチカワチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('6808634','{"jis": "31201", "kana": "カブシキガイシヤ リムノ", "name": "株式会社　ＬＩＭＮＯ", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "立川町", "banchi": "7丁目101番地", "postal_code": "6808634", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "タチカワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6808577','{"jis": "31201", "kana": "サンヨウエプソンイメ-ジングデバイス カブシキカイシヤ トツトリジギヨウシヨ", "name": "三洋エプソンイメージングデバイス　株式会社　鳥取事業所", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "南吉方", "banchi": "3丁目101", "postal_code": "6808577", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "ミナミヨシカタ", "alternates": []}');
 INSERT INTO office_data VALUES('6808510','{"jis": "31201", "kana": "スミトモセイメイホケン ソウゴガイシヤ トツトリシシヤ", "name": "住友生命保険　相互会社　鳥取支社", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "今町", "banchi": "1丁目103", "postal_code": "6808510", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "イママチ", "alternates": []}');
 INSERT INTO office_data VALUES('6808502','{"jis": "31201", "kana": "ゼンコクノウギヨウキヨウドウクミアイレンゴウカイ トツトリケンホンブ", "name": "全国農業協同組合連合会　鳥取県本部", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "末広温泉町", "banchi": "724", "postal_code": "6808502", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "スエヒロオンセンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6808511','{"jis": "31201", "kana": "ダイワシヨウケン カブシキガイシヤ トツトリシテン", "name": "大和証券　株式会社　鳥取支店", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "今町", "banchi": "1丁目121", "postal_code": "6808511", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "イママチ", "alternates": []}');
 INSERT INTO office_data VALUES('6808531','{"jis": "31201", "kana": "トツトリケン シヤカイホケンシンリヨウホウシユウシハライキキン", "name": "鳥取県　社会保険診療報酬支払基金", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "扇町", "banchi": "117", "postal_code": "6808531", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "オウギマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6808585','{"jis": "31201", "kana": "トツトリケンイシカイ", "name": "鳥取県医師会", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "戎町", "banchi": "317", "postal_code": "6808585", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "エビスマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6808520','{"jis": "31201", "kana": "トツトリケンケイサツホンブ", "name": "鳥取県警察本部", "prefecture": "鳥取県", "city": "鳥取市", "neighborhood": "東町", "banchi": "1丁目271番地", "postal_code": "6808520", "old_code": "680  ", "post_office": "鳥取中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トットリシ", "neighborhood_kana": "ヒガシマチ", "alternates": []}');
@@ -138292,14 +138297,15 @@
 INSERT INTO office_data VALUES('6892395','{"jis": "31371", "kana": "トウハクチヨウノウギヨウ キヨウドウクミアイ", "name": "東伯町農業　協同組合", "prefecture": "鳥取県", "city": "東伯郡琴浦町", "neighborhood": "大字徳万", "banchi": "558-1", "postal_code": "6892395", "old_code": "68923", "post_office": "東伯", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6892293','{"jis": "31372", "kana": "カブシキガイシヤ サンセキ", "name": "株式会社　サンセキ", "prefecture": "鳥取県", "city": "東伯郡北栄町", "neighborhood": "東園", "banchi": "323-1", "postal_code": "6892293", "old_code": "68922", "post_office": "倉吉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トウハクグンホクエイチョウ", "neighborhood_kana": "ヒガシソノ", "alternates": []}');
 INSERT INTO office_data VALUES('6892298','{"jis": "31372", "kana": "ジエイエイトツトリチユウオウ ダイエイシシヨ", "name": "ＪＡ鳥取中央　大栄支所", "prefecture": "鳥取県", "city": "東伯郡北栄町", "neighborhood": "由良宿", "banchi": "561", "postal_code": "6892298", "old_code": "68922", "post_office": "倉吉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トウハクグンホクエイチョウ", "neighborhood_kana": "ユラシュク", "alternates": []}');
 INSERT INTO office_data VALUES('6892295','{"jis": "31372", "kana": "トツトリケンリツ トツトリチユウオウイクエイコウトウガツコウ", "name": "鳥取県立　鳥取中央育英高等学校", "prefecture": "鳥取県", "city": "東伯郡北栄町", "neighborhood": "由良宿", "banchi": "291-1", "postal_code": "6892295", "old_code": "68922", "post_office": "倉吉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トウハクグンホクエイチョウ", "neighborhood_kana": "ユラシュク", "alternates": []}');
 INSERT INTO office_data VALUES('6892292','{"jis": "31372", "kana": "ホクエイチヨウヤクバ ダイエイチヨウシヤ", "name": "北栄町役場　大栄庁舎", "prefecture": "鳥取県", "city": "東伯郡北栄町", "neighborhood": "由良宿", "banchi": "423-1", "postal_code": "6892292", "old_code": "68922", "post_office": "倉吉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "トウハクグンホクエイチョウ", "neighborhood_kana": "ユラシュク", "alternates": []}');
 INSERT INTO office_data VALUES('6894292','{"jis": "31390", "kana": "ホウキチヨウヤクバ ミゾグチブンチヨウシヤ", "name": "伯耆町役場　溝口分庁舎", "prefecture": "鳥取県", "city": "西伯郡伯耆町", "neighborhood": "溝口", "banchi": "647", "postal_code": "6894292", "old_code": "68942", "post_office": "米子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "サイハクグンホウキチョウ", "neighborhood_kana": "ミゾクチ", "alternates": []}');
 INSERT INTO office_data VALUES('6895292','{"jis": "31401", "kana": "ニチナンチヨウヤクバ", "name": "日南町役場", "prefecture": "鳥取県", "city": "日野郡日南町", "neighborhood": "霞", "banchi": "800", "postal_code": "6895292", "old_code": "68952", "post_office": "日南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トットリケン", "city_kana": "ヒノグンニチナンチョウ", "neighborhood_kana": "カスミ", "alternates": []}');
+INSERT INTO office_data VALUES('6908601','{"jis": "32201", "kana": "エヌエイチケイ マツエホウソウキヨク", "name": "ＮＨＫ　松江放送局", "prefecture": "島根県", "city": "松江市", "neighborhood": "灘町", "banchi": "101-6(松江中央郵便局私書箱第7号)", "postal_code": "6908601", "old_code": "690  ", "post_office": "松江中央", "type": "box", "multiple": false, "new": true, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ナダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908550','{"jis": "32201", "kana": "カナツギケンコウギヨウ カブシキガイシヤ", "name": "カナツ技建工業　株式会社", "prefecture": "島根県", "city": "松江市", "neighborhood": "春日町", "banchi": "636", "postal_code": "6908550", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "カスガチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908555','{"jis": "32201", "kana": "カブシキガイシヤ イチバタヒヤツカテン", "name": "株式会社　一畑百貨店", "prefecture": "島根県", "city": "松江市", "neighborhood": "朝日町", "banchi": "661", "postal_code": "6908555", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "アサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908508','{"jis": "32201", "kana": "カブシキガイシヤ エフエムサンイン", "name": "株式会社　エフエム山陰", "prefecture": "島根県", "city": "松江市", "neighborhood": "学園南", "banchi": "1丁目2番1号くにびきメッセ西棟2階", "postal_code": "6908508", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ガクエンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('6908539','{"jis": "32201", "kana": "カブシキガイシヤ サンインゴウドウギンコウ クレジツトカ-ドセンタ-", "name": "株式会社　山陰合同銀行　クレジットカードセンター", "prefecture": "島根県", "city": "松江市", "neighborhood": "", "banchi": "白潟本町23(松江中央郵便局私書箱第62号)", "postal_code": "6908539", "old_code": "690  ", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6908580','{"jis": "32201", "kana": "カブシキガイシヤ サンインゴウドウギンコウ ジムセンタ-", "name": "株式会社　山陰合同銀行　事務センター", "prefecture": "島根県", "city": "松江市", "neighborhood": "袖師町", "banchi": "6-10(松江中央郵便局私書箱第20号)", "postal_code": "6908580", "old_code": "690  ", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ソデシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908530','{"jis": "32201", "kana": "カブシキガイシヤ マイカルマツエサテイ", "name": "株式会社　マイカル松江サティ", "prefecture": "島根県", "city": "松江市", "neighborhood": "東朝日町", "banchi": "151", "postal_code": "6908530", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヒガシアサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908558','{"jis": "32201", "kana": "カブシキガイシヤ ユニコン", "name": "株式会社　ユニコン", "prefecture": "島根県", "city": "松江市", "neighborhood": "東朝日町", "banchi": "29", "postal_code": "6908558", "old_code": "690  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヒガシアサヒマチ", "alternates": []}');
@@ -138354,15 +138360,14 @@
 INSERT INTO office_data VALUES('6902198','{"jis": "32201", "kana": "コマツデンキサンギヨウ カブシキガイシヤ", "name": "小松電機産業　株式会社", "prefecture": "島根県", "city": "松江市", "neighborhood": "八雲町東岩坂", "banchi": "180", "postal_code": "6902198", "old_code": "69021", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヤクモチョウヒガシイワサカ", "alternates": []}');
 INSERT INTO office_data VALUES('6902192','{"jis": "32201", "kana": "マツエシヤクシヨ ヤクモシシヨ", "name": "松江市役所　八雲支所", "prefecture": "島根県", "city": "松江市", "neighborhood": "八雲町西岩坂", "banchi": "316", "postal_code": "6902192", "old_code": "69021", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヤクモチョウニシイワサカ", "alternates": []}');
 INSERT INTO office_data VALUES('6908686','{"jis": "32201", "kana": "カブシキガイシヤ サンインゴウドウギンコウ", "name": "株式会社　山陰合同銀行", "prefecture": "島根県", "city": "松江市", "neighborhood": "魚町", "banchi": "10(松江中央郵便局私書箱第1号)", "postal_code": "6908686", "old_code": "69091", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ウオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908668','{"jis": "32201", "kana": "カブシキガイシヤ サンインチユウオウシンポウシヤ", "name": "株式会社　山陰中央新報社", "prefecture": "島根県", "city": "松江市", "neighborhood": "殿町", "banchi": "383(松江中央郵便局私書箱第2号)", "postal_code": "6908668", "old_code": "69091", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "トノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908688','{"jis": "32201", "kana": "カブシキガイシヤ シマネギンコウ", "name": "株式会社　島根銀行", "prefecture": "島根県", "city": "松江市", "neighborhood": "東本町", "banchi": "2丁目35(松江中央郵便局私書箱第42号)", "postal_code": "6908688", "old_code": "69091", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヒガシホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6908611','{"jis": "32201", "kana": "カブシキガイシヤ センチヤソウ", "name": "株式会社　千茶荘", "prefecture": "島根県", "city": "松江市", "neighborhood": "矢田町", "banchi": "250-98(松江中央郵便局私書箱第95号)", "postal_code": "6908611", "old_code": "69091", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヤダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6908660','{"jis": "32201", "kana": "シマネケンシンヨウノウギヨウキヨウドウクミアイレンゴウカイ", "name": "島根県信用農業協同組合連合会", "prefecture": "島根県", "city": "松江市", "neighborhood": "殿町", "banchi": "19-1(松江中央郵便局私書箱第22号)", "postal_code": "6908660", "old_code": "69091", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "トノマチ", "alternates": []}');
-INSERT INTO office_data VALUES('6908601','{"jis": "32201", "kana": "ニホンホウソウキヨウカイ マツエホウソウキヨク", "name": "日本放送協会　松江放送局", "prefecture": "島根県", "city": "松江市", "neighborhood": "灘町", "banchi": "1-21(松江中央郵便局私書箱第7号)", "postal_code": "6908601", "old_code": "69091", "post_office": "松江中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ナダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6990492','{"jis": "32201", "kana": "シマネケンリツ シンジコウトウガツコウ", "name": "島根県立　宍道高等学校", "prefecture": "島根県", "city": "松江市", "neighborhood": "宍道町宍道", "banchi": "1586番地", "postal_code": "6990492", "old_code": "699  ", "post_office": "松江中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "シンジチョウシンジ", "alternates": []}');
 INSERT INTO office_data VALUES('6990192','{"jis": "32201", "kana": "ヒガシイズモチヨウヤクバ", "name": "東出雲町役場", "prefecture": "島根県", "city": "松江市", "neighborhood": "東出雲町揖屋", "banchi": "1142", "postal_code": "6990192", "old_code": "69901", "post_office": "東出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヒガシイズモチョウイヤ", "alternates": []}');
 INSERT INTO office_data VALUES('6990193','{"jis": "32201", "kana": "フジキコ-ポレ-シヨン カブシキガイシヤ", "name": "フジキコーポレーション　株式会社", "prefecture": "島根県", "city": "松江市", "neighborhood": "東出雲町意宇南", "banchi": "2丁目1-1", "postal_code": "6990193", "old_code": "69901", "post_office": "東出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "ヒガシイズモチョウイウナン", "alternates": []}');
 INSERT INTO office_data VALUES('6990293','{"jis": "32201", "kana": "ドクリツギヨウセイホウジン チイキイリヨウキノウスイシンキコウ タマツクリビヨウイン", "name": "独立行政法人　地域医療機能推進機構　玉造病院", "prefecture": "島根県", "city": "松江市", "neighborhood": "玉湯町湯町", "banchi": "1-2", "postal_code": "6990293", "old_code": "69902", "post_office": "玉造", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "タマユチョウユマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6990292','{"jis": "32201", "kana": "マツエシヤクシヨ タマユシシヨ", "name": "松江市役所　玉湯支所", "prefecture": "島根県", "city": "松江市", "neighborhood": "玉湯町湯町", "banchi": "1793", "postal_code": "6990292", "old_code": "69902", "post_office": "玉造", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "タマユチョウユマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6990496','{"jis": "32201", "kana": "カブシキガイシヤ ハラシヨウ", "name": "株式会社　原商", "prefecture": "島根県", "city": "松江市", "neighborhood": "宍道町白石", "banchi": "81-10", "postal_code": "6990496", "old_code": "69904", "post_office": "宍道", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マツエシ", "neighborhood_kana": "シンジチョウハクイシ", "alternates": []}');
 INSERT INTO office_data VALUES('6978585','{"jis": "32202", "kana": "エヌテイテイニシニホンデンシンデンワ カブシキカイシヤ シマネニシシテン (カブ) エヌテイテイネオメイト チユウゴクハマダエイギヨウシヨ", "name": "ＮＴＴ西日本電信電話　株式会社　島根西支店　（株）　ＮＴＴネオメイト　中国浜田営業所", "prefecture": "島根県", "city": "浜田市", "neighborhood": "殿町", "banchi": "2", "postal_code": "6978585", "old_code": "697  ", "post_office": "浜田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ハマダシ", "neighborhood_kana": "トノマチ", "alternates": []}');
@@ -138394,14 +138399,15 @@
 INSERT INTO office_data VALUES('6990588','{"jis": "32203", "kana": "イツパンシヤダンホウジン ニホンアマチユアムセンレンメイ ジエイエ-ア-ルエル キユ-エスエルビユ-ロ-", "name": "一般社団法人　日本アマチュア無線連盟　ＪＡＲＬ　ＱＳＬビューロー", "prefecture": "島根県", "city": "出雲市", "neighborhood": "斐川町神庭", "banchi": "1324-3", "postal_code": "6990588", "old_code": "69905", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "ヒカワチョウカンバ", "alternates": []}');
 INSERT INTO office_data VALUES('6990593','{"jis": "32203", "kana": "シマネケンノウギヨウキヨウドウクミアイ ヒカワチクホンブ", "name": "島根県農業協同組合　斐川地区本部", "prefecture": "島根県", "city": "出雲市", "neighborhood": "斐川町荘原", "banchi": "2172番地3", "postal_code": "6990593", "old_code": "69905", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "ヒカワチョウショウバラ", "alternates": []}');
 INSERT INTO office_data VALUES('6990696','{"jis": "32203", "kana": "カブシキガイシヤ イズモムラタセイサクシヨ", "name": "株式会社　出雲村田製作所", "prefecture": "島根県", "city": "出雲市", "neighborhood": "斐川町上直江", "banchi": "2308", "postal_code": "6990696", "old_code": "69906", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "ヒカワチョウカミナオエ", "alternates": []}');
 INSERT INTO office_data VALUES('6990697','{"jis": "32203", "kana": "ジエイエイゼンノウ シマネケンホンブ", "name": "ＪＡ全農　島根県本部", "prefecture": "島根県", "city": "出雲市", "neighborhood": "斐川町直江", "banchi": "5030", "postal_code": "6990697", "old_code": "69906", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "ヒカワチョウナオエ", "alternates": []}');
 INSERT INTO office_data VALUES('6990792','{"jis": "32203", "kana": "イズモシヤクシヨ タイシヤシシヨ", "name": "出雲市役所　大社支所", "prefecture": "島根県", "city": "出雲市", "neighborhood": "大社町杵築南", "banchi": "1395", "postal_code": "6990792", "old_code": "69907", "post_office": "出雲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "イズモシ", "neighborhood_kana": "タイシャチョウキヅキミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('6988504','{"jis": "32204", "kana": "カブシキカイシヤ イズミユメタウンマスダ", "name": "株式会社　イズミゆめタウン益田", "prefecture": "島根県", "city": "益田市", "neighborhood": "高津", "banchi": "7丁目21-12", "postal_code": "6988504", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "タカツ", "alternates": []}');
 INSERT INTO office_data VALUES('6988503','{"jis": "32204", "kana": "カブシキカイシヤ キヌヤ", "name": "株式会社　キヌヤ", "prefecture": "島根県", "city": "益田市", "neighborhood": "常盤町", "banchi": "4番38号", "postal_code": "6988503", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "トキワチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('6988506','{"jis": "32204", "kana": "ソニ-ネツトワ-クコミユニケ-シヨンズ カブシキガイシヤ", "name": "ソニーネットワークコミュニケーションズ　株式会社", "prefecture": "島根県", "city": "益田市", "neighborhood": "駅前町", "banchi": "17-1益田駅前ビルEAGA3F", "postal_code": "6988506", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "エキマエチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6988651','{"jis": "32204", "kana": "マスダ ゼイムシヨ", "name": "益田　税務署", "prefecture": "島根県", "city": "益田市", "neighborhood": "元町", "banchi": "12-11(益田郵便局私書箱第5号)", "postal_code": "6988651", "old_code": "698  ", "post_office": "益田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "モトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6988505','{"jis": "32204", "kana": "マスダサテイ", "name": "益田サティ", "prefecture": "島根県", "city": "益田市", "neighborhood": "乙吉町", "banchi": "イ95-10", "postal_code": "6988505", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "オトヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6988650','{"jis": "32204", "kana": "マスダシヤクシヨ", "name": "益田市役所", "prefecture": "島根県", "city": "益田市", "neighborhood": "常盤町", "banchi": "1-1(益田郵便局私書箱第4号)", "postal_code": "6988650", "old_code": "698  ", "post_office": "益田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "トキワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6988501','{"jis": "32204", "kana": "マスダセキジユウジビヨウイン", "name": "益田赤十字病院", "prefecture": "島根県", "city": "益田市", "neighborhood": "乙吉町", "banchi": "イ103-1", "postal_code": "6988501", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "オトヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6980292','{"jis": "32204", "kana": "マスダシヤクシヨミトソウゴウシシヨ", "name": "益田市役所美都総合支所", "prefecture": "島根県", "city": "益田市", "neighborhood": "美都町都茂", "banchi": "1803-1", "postal_code": "6980292", "old_code": "69802", "post_office": "美都", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "ミトチョウツモ", "alternates": []}');
 INSERT INTO office_data VALUES('6948501','{"jis": "32205", "kana": "イワミオオダゼイムシヨ", "name": "石見大田税務署", "prefecture": "島根県", "city": "大田市", "neighborhood": "大田町大田", "banchi": "イ289-2", "postal_code": "6948501", "old_code": "694  ", "post_office": "石見大田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "オオダシ", "neighborhood_kana": "オオダチョウオオダ", "alternates": []}');
 INSERT INTO office_data VALUES('6948502','{"jis": "32205", "kana": "オオダシヤクシヨ", "name": "大田市役所", "prefecture": "島根県", "city": "大田市", "neighborhood": "大田町大田", "banchi": "ロ1111番地", "postal_code": "6948502", "old_code": "694  ", "post_office": "石見大田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "オオダシ", "neighborhood_kana": "オオダチョウオオダ", "alternates": []}');
@@ -138694,14 +138700,15 @@
 INSERT INTO office_data VALUES('7128525','{"jis": "33202", "kana": "ミツビシガスカガク カブシキガイシヤ ミズシマコウジヨウ", "name": "三菱ガス化学　株式会社　水島工場", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "水島海岸通", "banchi": "3丁目10", "postal_code": "7128525", "old_code": "712  ", "post_office": "水島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "ミズシマカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7128501','{"jis": "33202", "kana": "ミツビシジドウシヤコウギヨウ カブシキガイシヤ セイサン・ブツリユウホンブ ミズシマセイサクシヨ", "name": "三菱自動車工業　株式会社　生産・物流本部　水島製作所", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "水島海岸通", "banchi": "1丁目1番地", "postal_code": "7128501", "old_code": "712  ", "post_office": "水島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "ミズシマカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7138713','{"jis": "33202", "kana": "アカザワヤ カブシキガイシヤ", "name": "赤澤屋　株式会社", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島阿賀崎", "banchi": "1丁目4-11(玉島郵便局私書箱第5号)", "postal_code": "7138713", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマアガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('7138668','{"jis": "33202", "kana": "オカヤマケンリツ タマシマコウトウガツコウ", "name": "岡山県立　玉島高等学校", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島阿賀崎", "banchi": "3丁目1-1(玉島郵便局私書箱第4号)", "postal_code": "7138668", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマアガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('7138550','{"jis": "33202", "kana": "カブシキガイシヤ クラレ クラシキジギヨウシヨ (タマシマ)", "name": "株式会社　クラレ　倉敷事業所　（玉島）", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島乙島", "banchi": "7471", "postal_code": "7138550", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマオトシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7138666','{"jis": "33202", "kana": "カブシキガイシヤ タイソウ", "name": "株式会社　鯛惣", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島勇崎", "banchi": "1292(玉島郵便局私書箱第6号)", "postal_code": "7138666", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマユウザキ", "alternates": []}');
 INSERT INTO office_data VALUES('7138565','{"jis": "33202", "kana": "クラシキシ タマシマシシヨ", "name": "倉敷市　玉島支所", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島阿賀崎", "banchi": "1丁目1-1", "postal_code": "7138565", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマアガサキ", "alternates": []}');
+INSERT INTO office_data VALUES('7138588','{"jis": "33202", "kana": "サクヨウガクエンコウトウガツコウ", "name": "作陽学園高等学校", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島八島", "banchi": "1541番1", "postal_code": "7138588", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマヤシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7138501','{"jis": "33202", "kana": "スミトモジユウキカイコウギヨウ カブシキカイシヤ オカヤマセイゾウシヨ", "name": "住友重機械工業　株式会社　岡山製造所", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島乙島", "banchi": "8230", "postal_code": "7138501", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマオトシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7138577','{"jis": "33202", "kana": "タチバナヨウキ カブシキガイシヤ", "name": "立花容器　株式会社", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島柏島", "banchi": "7047", "postal_code": "7138577", "old_code": "713  ", "post_office": "玉島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマカシワジマ", "alternates": []}');
 INSERT INTO office_data VALUES('7138601','{"jis": "33202", "kana": "タマシマ ゼイムシヨ", "name": "玉島　税務署", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島阿賀崎", "banchi": "2丁目1-50(玉島郵便局私書箱第14号)", "postal_code": "7138601", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマアガサキ", "alternates": []}');
 INSERT INTO office_data VALUES('7138686','{"jis": "33202", "kana": "タマシマシンヨウキンコ", "name": "玉島信用金庫", "prefecture": "岡山県", "city": "倉敷市", "neighborhood": "玉島", "banchi": "1438(玉島郵便局私書箱第7号)", "postal_code": "7138686", "old_code": "713  ", "post_office": "玉島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "クラシキシ", "neighborhood_kana": "タマシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7088520','{"jis": "33203", "kana": "アルネ・ツヤマ", "name": "アルネ・津山", "prefecture": "岡山県", "city": "津山市", "neighborhood": "新魚町", "banchi": "17", "postal_code": "7088520", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "シンウオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7088515','{"jis": "33203", "kana": "イズミツヤマテン", "name": "イズミ津山店", "prefecture": "岡山県", "city": "津山市", "neighborhood": "伏見町", "banchi": "50", "postal_code": "7088515", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "フシミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7088506','{"jis": "33203", "kana": "オカヤマケン ミマサカケンミンキヨク", "name": "岡山県美作県民局", "prefecture": "岡山県", "city": "津山市", "neighborhood": "山下", "banchi": "53", "postal_code": "7088506", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "サンゲ", "alternates": []}');
@@ -140376,15 +140383,15 @@
 INSERT INTO office_data VALUES('7819525','{"jis": "39201", "kana": "トウヨウデンカコウギヨウ カブシキガイシヤ", "name": "東洋電化工業　株式会社", "prefecture": "高知県", "city": "高知市", "neighborhood": "萩町", "banchi": "2丁目2-25", "postal_code": "7819525", "old_code": "781  ", "post_office": "高知東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ハギマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7818543','{"jis": "39201", "kana": "トサガス カブシキガイシヤ", "name": "土佐ガス　株式会社", "prefecture": "高知県", "city": "高知市", "neighborhood": "葛島", "banchi": "2丁目3-75", "postal_code": "7818543", "old_code": "781  ", "post_office": "高知東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "カヅラシマ", "alternates": []}');
 INSERT INTO office_data VALUES('7819556','{"jis": "39201", "kana": "ニツポンネンキンキコウ コウチヒガシネンキンジムシヨ", "name": "日本年金機構　高知東年金事務所", "prefecture": "高知県", "city": "高知市", "neighborhood": "桟橋通", "banchi": "4丁目13番3号", "postal_code": "7819556", "old_code": "781  ", "post_office": "高知東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "サンバシドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7819519','{"jis": "39201", "kana": "ブル-チツプ コウチセンタ- シヨウヒンコウカンウケツケガカリ", "name": "ブルーチップ　高知センター　商品交換受付係", "prefecture": "高知県", "city": "高知市", "neighborhood": "知寄町", "banchi": "2丁目1-37ちより街テラス4階", "postal_code": "7819519", "old_code": "781  ", "post_office": "高知東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "チヨリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7819683','{"jis": "39201", "kana": "マルニシヨウジ カブシキガイシヤ", "name": "丸仁商事　株式会社", "prefecture": "高知県", "city": "高知市", "neighborhood": "南久保", "banchi": "80(高知卸団地郵便局私書箱第21号)", "postal_code": "7819683", "old_code": "781  ", "post_office": "高知東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ミナミクボ", "alternates": []}');
 INSERT INTO office_data VALUES('7819689','{"jis": "39201", "kana": "マルミシヨウジ カブシキガイシヤ", "name": "丸美商事　（株）", "prefecture": "高知県", "city": "高知市", "neighborhood": "南久保", "banchi": "140(高知卸団地郵便局私書箱第51号)", "postal_code": "7819689", "old_code": "781  ", "post_office": "高知東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ミナミクボ", "alternates": []}');
 INSERT INTO office_data VALUES('7818555','{"jis": "39201", "kana": "コウチイリヨウセンタ-", "name": "高知医療センター", "prefecture": "高知県", "city": "高知市", "neighborhood": "池", "banchi": "2125-1", "postal_code": "7818555", "old_code": "78101", "post_office": "高知東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "イケ", "alternates": []}');
-INSERT INTO office_data VALUES('7810392','{"jis": "39201", "kana": "コウチシ ハルノチヨウシヤ", "name": "高知市　春野庁舎", "prefecture": "高知県", "city": "高知市", "neighborhood": "春野町西分", "banchi": "15", "postal_code": "7810392", "old_code": "78103", "post_office": "春野", "type": "office", "multiple": false, "new": true, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ハルノチョウニシブン", "alternates": []}');
+INSERT INTO office_data VALUES('7810392','{"jis": "39201", "kana": "コウチシ ハルノチヨウシヤ", "name": "高知市　春野庁舎", "prefecture": "高知県", "city": "高知市", "neighborhood": "春野町西分", "banchi": "15", "postal_code": "7810392", "old_code": "78103", "post_office": "春野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ハルノチョウニシブン", "alternates": []}');
 INSERT INTO office_data VALUES('7815192','{"jis": "39201", "kana": "アサヒシヨクヒンカブシキガイシヤ コウチヒガシシテン", "name": "旭食品株式会社　高知東支店", "prefecture": "高知県", "city": "高知市", "neighborhood": "介良", "banchi": "乙3242", "postal_code": "7815192", "old_code": "78151", "post_office": "高知東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ケラ", "alternates": []}');
 INSERT INTO office_data VALUES('7815195','{"jis": "39201", "kana": "カブシキガイシヤ ギケンセイサクシヨ", "name": "株式会社　技研製作所", "prefecture": "高知県", "city": "高知市", "neighborhood": "布師田", "banchi": "3948-1", "postal_code": "7815195", "old_code": "78151", "post_office": "高知東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ヌノシダ", "alternates": []}');
 INSERT INTO office_data VALUES('7817185','{"jis": "39202", "kana": "ムロトシヤクシヨ", "name": "室戸市役所", "prefecture": "高知県", "city": "室戸市", "neighborhood": "浮津", "banchi": "25-1", "postal_code": "7817185", "old_code": "78171", "post_office": "室戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "ムロトシ", "neighborhood_kana": "ウキツ", "alternates": []}');
 INSERT INTO office_data VALUES('7848501','{"jis": "39203", "kana": "アキシヤクシヨ", "name": "安芸市役所", "prefecture": "高知県", "city": "安芸市", "neighborhood": "矢ノ丸", "banchi": "1丁目4-40", "postal_code": "7848501", "old_code": "784  ", "post_office": "安芸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "アキシ", "neighborhood_kana": "ヤノマル", "alternates": []}');
 INSERT INTO office_data VALUES('7848503','{"jis": "39203", "kana": "コウチケンノウギヨウキヨウドウクミアイ アキチクホンブ", "name": "高知県農業協同組合　安芸地区本部", "prefecture": "高知県", "city": "安芸市", "neighborhood": "幸町", "banchi": "1-16", "postal_code": "7848503", "old_code": "784  ", "post_office": "安芸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "アキシ", "neighborhood_kana": "サイワイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7848505','{"jis": "39203", "kana": "コウチケンリツ アキコウトウガツコウ", "name": "高知県立　安芸高等学校", "prefecture": "高知県", "city": "安芸市", "neighborhood": "清和町", "banchi": "1-54", "postal_code": "7848505", "old_code": "784  ", "post_office": "安芸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "アキシ", "neighborhood_kana": "セイワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7838555','{"jis": "39204", "kana": "アサヒシヨクヒン カブシキガイシヤ シコクシシヤ", "name": "旭食品　株式会社　四国支社", "prefecture": "高知県", "city": "南国市", "neighborhood": "領石", "banchi": "246", "postal_code": "7838555", "old_code": "783  ", "post_office": "南国", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "ナンコクシ", "neighborhood_kana": "リョウセキ", "alternates": [{"jis": "39204", "kana": "アサヒシヨクヒン カブシキガイシヤ ホンシヤ", "name": "旭食品　株式会社　本社", "prefecture": "高知県", "city": "南国市", "neighborhood": "領石", "banchi": "246", "postal_code": "7838555", "old_code": "783  ", "post_office": "南国", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "ナンコクシ", "neighborhood_kana": "リョウセキ", "alternates": []}]}');
@@ -140553,15 +140560,14 @@
 INSERT INTO office_data VALUES('8000285','{"jis": "40107", "kana": "サニ-サイドモ-ル コクラ", "name": "サニーサイドモール　小倉", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "下曽根新町", "banchi": "10-1", "postal_code": "8000285", "old_code": "80002", "post_office": "曽根", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "シモソネシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8000286','{"jis": "40107", "kana": "サンデ-キタキユウシユウ", "name": "サンデー北九州", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "葛原", "banchi": "5丁目3-3", "postal_code": "8000286", "old_code": "80002", "post_office": "曽根", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "クズハラ", "alternates": []}');
 INSERT INTO office_data VALUES('8000293','{"jis": "40107", "kana": "ト-ト- カブシキガイシヤ コクラダイニコウジヨウ", "name": "ＴＯＴＯ　株式会社　小倉第二工場", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "朽網東", "banchi": "5丁目1-1", "postal_code": "8000293", "old_code": "80002", "post_office": "曽根", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "クサミヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('8000282','{"jis": "40107", "kana": "メイジヤシヨウジ カブシキガイシヤ キタキユウシユウテン", "name": "明治屋商事　株式会社　北九州店", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "上葛原", "banchi": "1丁目18番1号", "postal_code": "8000282", "old_code": "80002", "post_office": "曽根", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "カミクズハラ", "alternates": []}');
 INSERT INTO office_data VALUES('8028540','{"jis": "40107", "kana": "カブシキガイシヤ タカギ", "name": "株式会社　タカギ", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "石田南", "banchi": "2丁目4-1", "postal_code": "8028540", "old_code": "802  ", "post_office": "北九州中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "イシダミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('8028510','{"jis": "40107", "kana": "キタキユウシユウシコクラミナミクヤクシヨ", "name": "北九州市　小倉南区役所", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "若園", "banchi": "5丁目1-2", "postal_code": "8028510", "old_code": "802  ", "post_office": "北九州中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "ワカゾノ", "alternates": []}');
 INSERT INTO office_data VALUES('8028577','{"jis": "40107", "kana": "キタキユウシユウシリツダイガク", "name": "北九州市立大学", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "北方", "banchi": "4丁目2-1", "postal_code": "8028577", "old_code": "802  ", "post_office": "北九州中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "キタガタ", "alternates": []}');
-INSERT INTO office_data VALUES('8028529','{"jis": "40107", "kana": "コクラコウチシシヨ", "name": "小倉拘置支所", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "葉山町", "banchi": "1丁目1番8号", "postal_code": "8028529", "old_code": "802  ", "post_office": "北九州中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "ハヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8028533','{"jis": "40107", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ コクライリヨウセンタ-", "name": "独立行政法人　国立病院機構　小倉医療センター", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "春ケ丘", "banchi": "10番1号", "postal_code": "8028533", "old_code": "802  ", "post_office": "北九州中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "ハルガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('8028567','{"jis": "40107", "kana": "リクジヨウジエイタイ コクラチユウトンチ", "name": "陸上自衛隊　小倉駐屯地", "prefecture": "福岡県", "city": "北九州市小倉南区", "neighborhood": "北方", "banchi": "5丁目1-1", "postal_code": "8028567", "old_code": "802  ", "post_office": "北九州中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシコクラミナミク", "neighborhood_kana": "キタガタ", "alternates": []}');
 INSERT INTO office_data VALUES('8058508','{"jis": "40108", "kana": "イリヨウホウジンシヤダン シンニツテツヤハタキネンビヨウイン", "name": "医療法人社団　新日鐵八幡記念病院", "prefecture": "福岡県", "city": "北九州市八幡東区", "neighborhood": "春の町", "banchi": "1丁目1-1", "postal_code": "8058508", "old_code": "805  ", "post_office": "八幡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシヤハタヒガシク", "neighborhood_kana": "ハルノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8058507','{"jis": "40108", "kana": "カブシキガイシヤ アステツクイリエ", "name": "株式会社　アステック入江", "prefecture": "福岡県", "city": "北九州市八幡東区", "neighborhood": "西本町", "banchi": "3丁目1番1号", "postal_code": "8058507", "old_code": "805  ", "post_office": "八幡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシヤハタヒガシク", "neighborhood_kana": "ニシホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8058538','{"jis": "40108", "kana": "カブシキガイシヤ アリゾノセイサクシヨ", "name": "株式会社　有薗製作所", "prefecture": "福岡県", "city": "北九州市八幡東区", "neighborhood": "東田", "banchi": "1丁目7番5号", "postal_code": "8058538", "old_code": "805  ", "post_office": "八幡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシヤハタヒガシク", "neighborhood_kana": "ヒガシダ", "alternates": []}');
 INSERT INTO office_data VALUES('8058531','{"jis": "40108", "kana": "カブシキガイシヤ オクムラグミ キユウシユウシテン", "name": "株式会社　奥村組　九州支店", "prefecture": "福岡県", "city": "北九州市八幡東区", "neighborhood": "山王", "banchi": "2丁目19-1", "postal_code": "8058531", "old_code": "805  ", "post_office": "八幡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシヤハタヒガシク", "neighborhood_kana": "サンノウ", "alternates": []}');
 INSERT INTO office_data VALUES('8058535','{"jis": "40108", "kana": "カブシキガイシヤ スガハラ", "name": "株式会社　菅原", "prefecture": "福岡県", "city": "北九州市八幡東区", "neighborhood": "西本町", "banchi": "3丁目2-5", "postal_code": "8058535", "old_code": "805  ", "post_office": "八幡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシヤハタヒガシク", "neighborhood_kana": "ニシホンマチ", "alternates": []}');
@@ -140632,26 +140638,24 @@
 INSERT INTO office_data VALUES('8128588','{"jis": "40131", "kana": "メイジヤシヨウジ カブシキガイシヤ フクオカシテン", "name": "明治屋商事　株式会社　福岡支店", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "箱崎ふ頭", "banchi": "5丁目7-17", "postal_code": "8128588", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "ハコザキフトウ", "alternates": []}');
 INSERT INTO office_data VALUES('8128581','{"jis": "40131", "kana": "キユウシユウダイガクハコザキチクブキヨク", "name": "九州大学箱崎地区部局", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "箱崎", "banchi": "6丁目10-1", "postal_code": "8128581", "old_code": "81281", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "ハコザキ", "alternates": []}');
 INSERT INTO office_data VALUES('8128582','{"jis": "40131", "kana": "キユウシユウダイガクビヨウインチクブキヨク", "name": "九州大学病院地区部局", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "馬出", "banchi": "3丁目1-1", "postal_code": "8128582", "old_code": "81282", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "マイダシ", "alternates": []}');
 INSERT INTO office_data VALUES('8138585','{"jis": "40131", "kana": "アビスパフクオカ カブシキガイシヤ", "name": "アビスパ福岡　株式会社", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "香椎浜ふ頭", "banchi": "1丁目2-17", "postal_code": "8138585", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "カシイハマフトウ", "alternates": []}');
 INSERT INTO office_data VALUES('8138588','{"jis": "40131", "kana": "イリヨウホウジン ハラドイビヨウイン", "name": "医療法人　原土井病院", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "青葉", "banchi": "6丁目40-8", "postal_code": "8138588", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "アオバ", "alternates": []}');
 INSERT INTO office_data VALUES('8138681','{"jis": "40131", "kana": "カシイゼイムシヨ", "name": "香椎税務署", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "千早", "banchi": "6丁目2-1(福岡東郵便局私書箱第8号)", "postal_code": "8138681", "old_code": "813  ", "post_office": "福岡東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "チハヤ", "alternates": []}');
 INSERT INTO office_data VALUES('8138555','{"jis": "40131", "kana": "カブシキガイシヤ アトル", "name": "株式会社　アトル", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "香椎浜ふ頭", "banchi": "2丁目5番1号", "postal_code": "8138555", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "カシイハマフトウ", "alternates": []}');
-INSERT INTO office_data VALUES('8138568','{"jis": "40131", "kana": "カブシキガイシヤ ヤマヤ", "name": "株式会社　やまや", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "松島", "banchi": "5丁目27-5", "postal_code": "8138568", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "マツシマ", "alternates": []}');
-INSERT INTO office_data VALUES('8138533','{"jis": "40131", "kana": "カブシキガイシヤ ルルア-ク", "name": "株式会社　ルルアーク", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "松島", "banchi": "3丁目30-23", "postal_code": "8138533", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "マツシマ", "alternates": []}');
+INSERT INTO office_data VALUES('8138533','{"jis": "40131", "kana": "カブシキガイシヤ ルルア-ク", "name": "株式会社　ルルアーク", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "松島", "banchi": "3丁目30-23", "postal_code": "8138533", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "マツシマ", "alternates": []}');
 INSERT INTO office_data VALUES('8138680','{"jis": "40131", "kana": "カブシキガイシヤト-ホ- キユウシユウシテン", "name": "株式会社トーホー　九州支店", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "松島", "banchi": "3丁目11-1(福岡流通センター内郵便局私書箱第31号)", "postal_code": "8138680", "old_code": "813  ", "post_office": "福岡東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "マツシマ", "alternates": []}');
 INSERT INTO office_data VALUES('8138503','{"jis": "40131", "kana": "ガツコウホウジン ナカムラサンギヨウガクエン キユウシユウサンギヨウダイガク", "name": "学校法人　中村産業学園　九州産業大学", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "松香台", "banchi": "2丁目3-1", "postal_code": "8138503", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "マツカダイ", "alternates": []}');
 INSERT INTO office_data VALUES('8138577','{"jis": "40131", "kana": "キユウシユウウンユキヨク フクオカウンユシキヨク", "name": "九州運輸局　福岡運輸支局", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "千早", "banchi": "3丁目10-40", "postal_code": "8138577", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "チハヤ", "alternates": []}');
 INSERT INTO office_data VALUES('8138513','{"jis": "40131", "kana": "キユウシユウデンリヨク カブシキガイシヤ フクオカヒガシエイギヨウシヨ", "name": "九州電力　株式会社　福岡東営業所", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "名島", "banchi": "2丁目19-12", "postal_code": "8138513", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "ナジマ", "alternates": []}');
 INSERT INTO office_data VALUES('8138501','{"jis": "40131", "kana": "コツカコウムイントウキヨウサイクミアイレンゴウカイ チハヤビヨウイン", "name": "国家公務員等共済組合連合会　千早病院", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "千早", "banchi": "2丁目30-1", "postal_code": "8138501", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "チハヤ", "alternates": []}');
 INSERT INTO office_data VALUES('8138519','{"jis": "40131", "kana": "シヨウコウクミアイチユウオウキンコ フクオカリユウツウセンタ-シユツチヨウシヨ", "name": "商工組合中央金庫　福岡流通センター出張所", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "多の津", "banchi": "1丁目7-1", "postal_code": "8138519", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "タノツ", "alternates": []}');
 INSERT INTO office_data VALUES('8138623','{"jis": "40131", "kana": "ニツサンデイ-ゼルフクオカハンバイ カブシキガイシヤ", "name": "日産ディーゼル福岡販売　株式会社", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "多の津", "banchi": "1丁目39-4(福岡流通センター内郵便局私書箱第232号)", "postal_code": "8138623", "old_code": "813  ", "post_office": "福岡東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "タノツ", "alternates": []}');
 INSERT INTO office_data VALUES('8138529','{"jis": "40131", "kana": "フクオカジヨシダイガク", "name": "福岡女子大学", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "香住ケ丘", "banchi": "1丁目1-1", "postal_code": "8138529", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8138609','{"jis": "40131", "kana": "フクオカヒガシコウキヨウシヨクギヨウアンテイシヨ", "name": "福岡東公共職業安定所", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "千早", "banchi": "6丁目1番1号", "postal_code": "8138609", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "チハヤ", "alternates": []}');
-INSERT INTO office_data VALUES('8138578','{"jis": "40131", "kana": "ヤマヤチヨクハン カブシキガイシヤ", "name": "やまや直販　株式会社", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "松島", "banchi": "3丁目31-1", "postal_code": "8138578", "old_code": "813  ", "post_office": "福岡東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "マツシマ", "alternates": []}');
 INSERT INTO office_data VALUES('8138626','{"jis": "40131", "kana": "ユニ-ク カブシキガイシヤ", "name": "ユニーク　株式会社", "prefecture": "福岡県", "city": "福岡市東区", "neighborhood": "多の津", "banchi": "1丁目10-5(福岡流通センター内郵便局私書箱第26号)", "postal_code": "8138626", "old_code": "813  ", "post_office": "福岡東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシヒガシク", "neighborhood_kana": "タノツ", "alternates": []}');
 INSERT INTO office_data VALUES('8108604','{"jis": "40132", "kana": "カブシキガイシヤ フクオカタマヤ", "name": "株式会社　福岡玉屋", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "中洲", "banchi": "3丁目7-30", "postal_code": "8108604", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ナカス", "alternates": []}');
 INSERT INTO office_data VALUES('8108629','{"jis": "40132", "kana": "カブシキガイシヤ フクヤ", "name": "株式会社　ふくや", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "中洲", "banchi": "2丁目6-10", "postal_code": "8108629", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ナカス", "alternates": []}');
 INSERT INTO office_data VALUES('8108666','{"jis": "40132", "kana": "ソンガイホケンジヤパンニツポンコウア カブシキカイシヤ", "name": "損害保険ジャパン日本興亜　株式会社", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "中洲中島町", "banchi": "2-8", "postal_code": "8108666", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ナカスナカシママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8108625','{"jis": "40132", "kana": "ユキジルシニユウギヨウ カブシキガイシヤ キユウシユウシシヤ", "name": "雪印乳業　株式会社　九州支社", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "中洲中島町", "banchi": "2番8号", "postal_code": "8108625", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ナカスナカシママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8108731','{"jis": "40132", "kana": "コジマヨウシ カブシキガイシヤ", "name": "児島洋紙　株式会社", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "中洲中島町", "banchi": "2-1(福岡中央郵便局私書箱第191号)", "postal_code": "8108731", "old_code": "81091", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ナカスナカシママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8128511','{"jis": "40132", "kana": "アサヒシンブン フクオカホンブ", "name": "朝日新聞　福岡本部", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "博多駅前", "banchi": "2丁目1-1", "postal_code": "8128511", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ハカタエキマエ", "alternates": []}');
@@ -140862,14 +140866,15 @@
 INSERT INTO office_data VALUES('8108557','{"jis": "40133", "kana": "カブシキガイシヤ リクル-ト キユウシユウシシヤ", "name": "株式会社　リクルート　九州支社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "舞鶴", "banchi": "1丁目1-3", "postal_code": "8108557", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "マイヅル", "alternates": []}');
 INSERT INTO office_data VALUES('8108512','{"jis": "40133", "kana": "カブシキガイシヤカミグミフクオカシテン", "name": "株式会社　上組福岡支店", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "那の津", "banchi": "3丁目2-10", "postal_code": "8108512", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナノツ", "alternates": []}');
 INSERT INTO office_data VALUES('8108565','{"jis": "40133", "kana": "カブシキガイシヤキユウシユウコクサイエフエム(LOVE FM76.1)", "name": "株式会社九州国際エフエム（ＬＯＶＥ　ＦＭ７６．１）", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "2丁目5-35NTT-Tビル7階", "postal_code": "8108565", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108631','{"jis": "40133", "kana": "カブシキガイシヤトウシヨク フクオカシテン", "name": "株式会社東食　福岡支店", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "1丁目14-16三栄ビル5階", "postal_code": "8108631", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108619','{"jis": "40133", "kana": "ガツコウホウジン カワイジユク フクオカコウ", "name": "学校法人　河合塾　福岡校", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "渡辺通", "banchi": "4丁目2-11", "postal_code": "8108619", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ワタナベドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('8108588','{"jis": "40133", "kana": "キユ-サイ カブシキカイシヤ", "name": "キューサイ　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "薬院", "banchi": "1-1-1", "postal_code": "8108588", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ヤクイン", "alternates": []}');
 INSERT INTO office_data VALUES('8108606','{"jis": "40133", "kana": "キユ-サイ カブシキガイシヤ", "name": "キューサイ　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "草香江", "banchi": "1丁目7-16", "postal_code": "8108606", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "クサガエ", "alternates": []}');
+INSERT INTO office_data VALUES('8108571','{"jis": "40133", "kana": "キユウシユウアサヒホウソウ カブシキガイシヤ", "name": "九州朝日放送　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "長浜", "banchi": "1丁目1-1", "postal_code": "8108571", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナガハマ", "alternates": [{"jis": "40133", "kana": "ケ-ビ-シ-グル-プホ-ルデイングス カブシキガイシヤ", "name": "ＫＢＣグループホールディングス　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "長浜", "banchi": "1丁目1-1", "postal_code": "8108571", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナガハマ", "alternates": []}]}');
 INSERT INTO office_data VALUES('8108560','{"jis": "40133", "kana": "キユウシユウダイガク ロツポンマツチクブキヨク(ダイガクキヨウイクケンキユウセンタ-.ダイガクインヒカクシヤカイブンカケンキユウカ.ゲンゴブンカブ)", "name": "九州大学　六本松地区部局（大学教育研究センター、大学院比較社会文化研究科、言語文化部）", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "六本松", "banchi": "4丁目2-1", "postal_code": "8108560", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ロッポンマツ", "alternates": []}');
 INSERT INTO office_data VALUES('8108617','{"jis": "40133", "kana": "キユウシユウツウシンネツトワ-ク カブシキガイシヤ", "name": "九州通信ネットワーク　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "1丁目12-20-8F", "postal_code": "8108617", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108705','{"jis": "40133", "kana": "キユウシユウデンリヨクソウハイデン カブシキガイシヤ ホンテン", "name": "九州電力送配電　株式会社　本店", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "渡辺通", "banchi": "二丁目1番82号(福岡中央郵便局私書箱第94号)", "postal_code": "8108705", "old_code": "810  ", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ワタナベドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('8108636','{"jis": "40133", "kana": "キユウシユウミツビシジドウシヤハンバイ カブシキガイシヤ", "name": "九州三菱自動車販売　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "薬院", "banchi": "3丁目2-23", "postal_code": "8108636", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ヤクイン", "alternates": []}');
 INSERT INTO office_data VALUES('8108509','{"jis": "40133", "kana": "キユウシユウロウドウキンコ", "name": "九州労働金庫", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "大手門", "banchi": "3丁目3-3", "postal_code": "8108509", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "オオテモン", "alternates": []}');
 INSERT INTO office_data VALUES('8108532','{"jis": "40133", "kana": "キリンビ-ル カブシキガイシヤ キユウシユウシシヤ", "name": "キリンビール　株式会社　九州支社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "2丁目14-8FTCビル15F", "postal_code": "8108532", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108601','{"jis": "40133", "kana": "ゲツカンウルトラマンボウ カブシキガイシヤ ア-トライン", "name": "月刊うるとらマンボウ　株式会社　アートライン", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "4丁目9-15文化ビル1F", "postal_code": "8108601", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
@@ -140923,15 +140928,14 @@
 INSERT INTO office_data VALUES('8108506','{"jis": "40133", "kana": "マツオケンセツ カブシキガイシヤ フクオカシテン", "name": "松尾建設　株式会社　福岡支店", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "薬院", "banchi": "3丁目4-9", "postal_code": "8108506", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ヤクイン", "alternates": []}');
 INSERT INTO office_data VALUES('8108530','{"jis": "40133", "kana": "マツシタデンコウ カブシキガイシヤ キユウシユウチクタントウブ", "name": "松下電工　株式会社　九州地区担当部", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "薬院", "banchi": "3丁目1-24", "postal_code": "8108530", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ヤクイン", "alternates": []}');
 INSERT INTO office_data VALUES('8108683','{"jis": "40133", "kana": "ミツイスミトモカイジヨウカサイホケン カブシキガイシヤ", "name": "三井住友海上火災保険　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "赤坂", "banchi": "1丁目16-14(福岡中央郵便局私書箱第26号)", "postal_code": "8108683", "old_code": "810  ", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('8108527','{"jis": "40133", "kana": "ミツイマツシマサンギヨウ カブシキガイシヤ", "name": "三井松島産業　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "大手門", "banchi": "1丁目1-12", "postal_code": "8108527", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "オオテモン", "alternates": []}');
 INSERT INTO office_data VALUES('8108725','{"jis": "40133", "kana": "ユ-エフジエ-シンタクギンコウ カブシキガイシヤ フクオカシテン", "name": "ＵＦＪ信託銀行　株式会社　福岡支店", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "1丁目14-1(福岡中央郵便局私書箱第224号)", "postal_code": "8108725", "old_code": "810  ", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108546','{"jis": "40133", "kana": "ユウゲンガイシヤ サウンドトラツク", "name": "有限会社　サウンドトラック", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "渡辺通", "banchi": "2丁目3-461F", "postal_code": "8108546", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ワタナベドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('8108581','{"jis": "40133", "kana": "ヨミウリシンブン セイブホンシヤ", "name": "読売新聞　西部本社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "赤坂", "banchi": "1丁目16-5", "postal_code": "8108581", "old_code": "810  ", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "アカサカ", "alternates": []}');
-INSERT INTO office_data VALUES('8108571','{"jis": "40133", "kana": "キユウシユウアサヒホウソウ カブシキガイシヤ", "name": "九州朝日放送　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "長浜", "banchi": "1丁目1-1", "postal_code": "8108571", "old_code": "81071", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ナガハマ", "alternates": []}');
 INSERT INTO office_data VALUES('8108577','{"jis": "40133", "kana": "ニホンホウソウキヨウカイ フクオカホウソウキヨク", "name": "日本放送協会　福岡放送局", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "六本松", "banchi": "1丁目1-10", "postal_code": "8108577", "old_code": "81077", "post_office": "福岡中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ロッポンマツ", "alternates": []}');
 INSERT INTO office_data VALUES('8108675','{"jis": "40133", "kana": "カブシキガイシヤ デンツウキユウシユウ", "name": "株式会社　電通九州", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "赤坂", "banchi": "1丁目16-10(福岡中央郵便局私書箱第187号)", "postal_code": "8108675", "old_code": "81091", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('8108717','{"jis": "40133", "kana": "カブシキガイシヤ ハカタダイマル", "name": "株式会社　博多大丸", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "1丁目4-1(福岡中央郵便局私書箱第249号)", "postal_code": "8108717", "old_code": "81091", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108727','{"jis": "40133", "kana": "カブシキガイシヤ フクオカギンコウ", "name": "株式会社　福岡銀行", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "2丁目13-1(福岡中央郵便局私書箱第133号)", "postal_code": "8108727", "old_code": "81091", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8108676','{"jis": "40133", "kana": "カブシキガイシヤ フクオカチユウオウギンコウ", "name": "株式会社　福岡中央銀行", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "大名", "banchi": "2丁目12-1(福岡中央郵便局私書箱第64号)", "postal_code": "8108676", "old_code": "81091", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ダイミョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8108720','{"jis": "40133", "kana": "キユウシユウデンリヨク カブシキガイシヤ", "name": "九州電力　株式会社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "渡辺通", "banchi": "2丁目1-82(福岡中央郵便局私書箱第69号)", "postal_code": "8108720", "old_code": "81091", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "ワタナベドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('8108707','{"jis": "40133", "kana": "ニホンセイメイホケン ソウゴガイシヤ フクオカソウシシヤ", "name": "日本生命保険　相互会社　福岡総支社", "prefecture": "福岡県", "city": "福岡市中央区", "neighborhood": "天神", "banchi": "1丁目14-1(福岡中央郵便局私書箱第92号)", "postal_code": "8108707", "old_code": "81091", "post_office": "福岡中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシチュウオウク", "neighborhood_kana": "テンジン", "alternates": []}');
@@ -140996,15 +141000,15 @@
 INSERT INTO office_data VALUES('8148510','{"jis": "40137", "kana": "フクオカケンリツシユウユウカンコウトウガツコウ", "name": "福岡県立　修猷館高等学校", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "西新", "banchi": "6丁目1-10", "postal_code": "8148510", "old_code": "814  ", "post_office": "早良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "ニシジン", "alternates": []}');
 INSERT INTO office_data VALUES('8148503','{"jis": "40137", "kana": "フクオカコウチシヨ", "name": "福岡拘置所", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "百道", "banchi": "2丁目16-10", "postal_code": "8148503", "old_code": "814  ", "post_office": "早良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "モモチ", "alternates": []}');
 INSERT INTO office_data VALUES('8148501','{"jis": "40137", "kana": "フクオカシ サワラクシクシヨ", "name": "福岡市　早良区役所", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "百道", "banchi": "2丁目1-1", "postal_code": "8148501", "old_code": "814  ", "post_office": "早良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "モモチ", "alternates": []}');
 INSERT INTO office_data VALUES('8148522','{"jis": "40137", "kana": "フクオカダイガクニシジンビヨウイン", "name": "福岡大学西新病院", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "祖原", "banchi": "15-7", "postal_code": "8148522", "old_code": "814  ", "post_office": "早良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "ソハラ", "alternates": []}');
 INSERT INTO office_data VALUES('8148524','{"jis": "40137", "kana": "フクオカホウムキヨク ニシジンシユツチヨウシヨ", "name": "福岡法務局　西新出張所", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "祖原", "banchi": "14-15", "postal_code": "8148524", "old_code": "814  ", "post_office": "早良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "ソハラ", "alternates": []}');
 INSERT INTO office_data VALUES('8148588','{"jis": "40137", "kana": "フジツウ キユウシユウア-ルアンドデイ-センタ-", "name": "富士通　九州Ｒ＆Ｄセンター", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "百道浜", "banchi": "2丁目2-1", "postal_code": "8148588", "old_code": "814  ", "post_office": "早良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "モモチハマ", "alternates": []}');
 INSERT INTO office_data VALUES('8148550','{"jis": "40137", "kana": "ボ-ダフオン カブシキガイシヤ", "name": "ボーダフォン　株式会社", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "百道浜", "banchi": "2丁目3-2-16F", "postal_code": "8148550", "old_code": "814  ", "post_office": "早良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "モモチハマ", "alternates": []}');
-INSERT INTO office_data VALUES('8140193','{"jis": "40137", "kana": "フクオカガクエン", "name": "福岡学園", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "田村", "banchi": "2丁目15-1", "postal_code": "8140193", "old_code": "81401", "post_office": "城南", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "タムラ", "alternates": []}');
+INSERT INTO office_data VALUES('8140193','{"jis": "40137", "kana": "フクオカガクエン", "name": "福岡学園", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "田村", "banchi": "2丁目15-1", "postal_code": "8140193", "old_code": "81401", "post_office": "城南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "タムラ", "alternates": []}');
 INSERT INTO office_data VALUES('8148555','{"jis": "40137", "kana": "カブシキガイシヤ テレビニシニホン", "name": "株式会社　テレビ西日本", "prefecture": "福岡県", "city": "福岡市早良区", "neighborhood": "百道浜", "banchi": "2丁目3-2", "postal_code": "8148555", "old_code": "81479", "post_office": "早良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシサワラク", "neighborhood_kana": "モモチハマ", "alternates": []}');
 INSERT INTO office_data VALUES('8368585','{"jis": "40202", "kana": "アリアケコウギヨウコウトウセンモンガツコウ", "name": "有明工業高等専門学校", "prefecture": "福岡県", "city": "大牟田市", "neighborhood": "東萩尾町", "banchi": "150", "postal_code": "8368585", "old_code": "836  ", "post_office": "大牟田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "オオムタシ", "neighborhood_kana": "ヒガシハギオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8368666','{"jis": "40202", "kana": "オオムタシヤクシヨ", "name": "大牟田市役所", "prefecture": "福岡県", "city": "大牟田市", "neighborhood": "有明町", "banchi": "2丁目3(大牟田郵便局私書箱第24号)", "postal_code": "8368666", "old_code": "836  ", "post_office": "大牟田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "オオムタシ", "neighborhood_kana": "ユウメイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8368686','{"jis": "40202", "kana": "オオムタゼイムシヨ", "name": "大牟田税務署", "prefecture": "福岡県", "city": "大牟田市", "neighborhood": "不知火町", "banchi": "1丁目3-16(大牟田郵便局私書箱第30号)", "postal_code": "8368686", "old_code": "836  ", "post_office": "大牟田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "オオムタシ", "neighborhood_kana": "シラヌヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8368533','{"jis": "40202", "kana": "オオムタヤナガワシンヨウキンコ", "name": "大牟田柳川信用金庫", "prefecture": "福岡県", "city": "大牟田市", "neighborhood": "有明町", "banchi": "2-2-17", "postal_code": "8368533", "old_code": "836  ", "post_office": "大牟田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "オオムタシ", "neighborhood_kana": "ユウメイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8368502','{"jis": "40202", "kana": "オオムタロウドウキジユンカントクシヨ", "name": "大牟田労働基準監督署", "prefecture": "福岡県", "city": "大牟田市", "neighborhood": "小浜町", "banchi": "24-13", "postal_code": "8368502", "old_code": "836  ", "post_office": "大牟田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "オオムタシ", "neighborhood_kana": "コハママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8368512','{"jis": "40202", "kana": "カブシキガイシヤ アリアケシンポウシヤ", "name": "株式会社　有明新報社", "prefecture": "福岡県", "city": "大牟田市", "neighborhood": "有明町", "banchi": "1丁目1-17", "postal_code": "8368512", "old_code": "836  ", "post_office": "大牟田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "オオムタシ", "neighborhood_kana": "ユウメイマチ", "alternates": []}');
@@ -141212,14 +141216,15 @@
 INSERT INTO office_data VALUES('8191392','{"jis": "40230", "kana": "イトシマシヤクシヨ シマチヨウシヤ", "name": "糸島市役所　志摩庁舎", "prefecture": "福岡県", "city": "糸島市", "neighborhood": "志摩初", "banchi": "30", "postal_code": "8191392", "old_code": "81913", "post_office": "前原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "イトシマシ", "neighborhood_kana": "シマハツ", "alternates": []}');
 INSERT INTO office_data VALUES('8191692','{"jis": "40230", "kana": "イトシマシヤクシヨ ニジヨウチヨウシヤ", "name": "糸島市役所　二丈庁舎", "prefecture": "福岡県", "city": "糸島市", "neighborhood": "二丈深江", "banchi": "1360", "postal_code": "8191692", "old_code": "81916", "post_office": "前原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "イトシマシ", "neighborhood_kana": "ニジョウフカエ", "alternates": []}');
 INSERT INTO office_data VALUES('8111292','{"jis": "40231", "kana": "ナカガワシヤクシヨ", "name": "那珂川市役所", "prefecture": "福岡県", "city": "那珂川市", "neighborhood": "西隈", "banchi": "1丁目1番1号", "postal_code": "8111292", "old_code": "81112", "post_office": "筑紫", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ナカガワシ", "neighborhood_kana": "ニシグマ", "alternates": []}');
 INSERT INTO office_data VALUES('8112192','{"jis": "40341", "kana": "ウミマチヤクバ", "name": "宇美町役場", "prefecture": "福岡県", "city": "糟屋郡宇美町", "neighborhood": "宇美", "banchi": "5丁目1-1", "postal_code": "8112192", "old_code": "81121", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンウミマチ", "neighborhood_kana": "ウミ", "alternates": []}');
 INSERT INTO office_data VALUES('8112195','{"jis": "40341", "kana": "サンドラツグ フクオカブツリユウセンタ-", "name": "サンドラッグ　福岡物流センター", "prefecture": "福岡県", "city": "糟屋郡宇美町", "neighborhood": "大字井野", "banchi": "字稲木369-8-10", "postal_code": "8112195", "old_code": "81121", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8112194','{"jis": "40341", "kana": "ダイレツクスフクオカマザ-センタ-", "name": "ダイレックス福岡マザーセンター", "prefecture": "福岡県", "city": "糟屋郡宇美町", "neighborhood": "大字井野", "banchi": "字稲木369-8-10", "postal_code": "8112194", "old_code": "81121", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8112495','{"jis": "40342", "kana": "エフコ-プ セイカツキヨウドウクミアイ", "name": "エフコープ　生活協同組合", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "大字篠栗", "banchi": "4826-1", "postal_code": "8112495", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('8112498','{"jis": "40342", "kana": "カブシキガイシヤ ヤマヤコミユニケ-シヨンズ", "name": "株式会社　やまやコミュニケーションズ", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "彩り台", "banchi": "1番1号", "postal_code": "8112498", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンササグリマチ", "neighborhood_kana": "イロドリダイ", "alternates": []}');
 INSERT INTO office_data VALUES('8112492','{"jis": "40342", "kana": "ササグリマチヤクバ", "name": "篠栗町役場", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "大字篠栗", "banchi": "4855-5", "postal_code": "8112492", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8112496','{"jis": "40342", "kana": "セイカツキヨウドウクミアイレンゴウカイ コ-プキユウシユウジギヨウレンゴウ", "name": "生活協同組合連合会　コープ九州事業連合", "prefecture": "福岡県", "city": "糟屋郡篠栗町", "neighborhood": "大字篠栗", "banchi": "4826-1", "postal_code": "8112496", "old_code": "81124", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8112294','{"jis": "40343", "kana": "カブシキガイシヤ サカグチ", "name": "株式会社　サカグチ", "prefecture": "福岡県", "city": "糟屋郡志免町", "neighborhood": "志免", "banchi": "4丁目1-24", "postal_code": "8112294", "old_code": "81122", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンシメマチ", "neighborhood_kana": "シメ", "alternates": []}');
 INSERT INTO office_data VALUES('8112293','{"jis": "40343", "kana": "カブシキガイシヤ セイユウ シメテン", "name": "株式会社　西友　志免店", "prefecture": "福岡県", "city": "糟屋郡志免町", "neighborhood": "志免中央", "banchi": "3丁目4-1", "postal_code": "8112293", "old_code": "81122", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンシメマチ", "neighborhood_kana": "シメチュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('8112295','{"jis": "40343", "kana": "ギケンコウギヨウ カブシキガイシヤ", "name": "技研工業　株式会社", "prefecture": "福岡県", "city": "糟屋郡志免町", "neighborhood": "志免", "banchi": "3丁目14-1", "postal_code": "8112295", "old_code": "81122", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンシメマチ", "neighborhood_kana": "シメ", "alternates": []}');
 INSERT INTO office_data VALUES('8112292','{"jis": "40343", "kana": "シメマチヤクバ", "name": "志免町役場", "prefecture": "福岡県", "city": "糟屋郡志免町", "neighborhood": "志免中央", "banchi": "1丁目1-1", "postal_code": "8112292", "old_code": "81122", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンシメマチ", "neighborhood_kana": "シメチュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('8112196','{"jis": "40344", "kana": "サガワグロ-バルロジステイクス カブシキガイシヤ キユウシユウシテン スエエイギヨウシヨ", "name": "佐川グローバルロジスティクス　株式会社　九州支店　須恵営業所", "prefecture": "福岡県", "city": "糟屋郡須惠町", "neighborhood": "大字新原", "banchi": "16-10", "postal_code": "8112196", "old_code": "81121", "post_office": "粕屋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -141614,15 +141619,15 @@
 INSERT INTO office_data VALUES('8570392','{"jis": "42391", "kana": "サザチヨウヤクバ", "name": "佐々町役場", "prefecture": "長崎県", "city": "北松浦郡佐々町", "neighborhood": "本田原免", "banchi": "168-2", "postal_code": "8570392", "old_code": "85703", "post_office": "佐々", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "キタマツウラグンサザチョウ", "neighborhood_kana": "ホンタバルメン", "alternates": []}');
 INSERT INTO office_data VALUES('8532392','{"jis": "42411", "kana": "シンカミゴトウチヨウヤクバ ワカマツシシヨ", "name": "新上五島町役場　若松支所", "prefecture": "長崎県", "city": "南松浦郡新上五島町", "neighborhood": "若松郷", "banchi": "277-7", "postal_code": "8532392", "old_code": "85323", "post_office": "若松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ミナミマツウラグンシンカミゴトウチョウ", "neighborhood_kana": "ワカマツゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('8574495','{"jis": "42411", "kana": "シンカミゴトウチヨウヤクバ", "name": "新上五島町役場", "prefecture": "長崎県", "city": "南松浦郡新上五島町", "neighborhood": "青方郷", "banchi": "1585-1", "postal_code": "8574495", "old_code": "85744", "post_office": "青方", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ミナミマツウラグンシンカミゴトウチョウ", "neighborhood_kana": "アオカタゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('8574592','{"jis": "42411", "kana": "シンカミゴトウチヨウヤクバ シンウオノメシシヨ", "name": "新上五島町役場　新魚目支所", "prefecture": "長崎県", "city": "南松浦郡新上五島町", "neighborhood": "榎津郷", "banchi": "491", "postal_code": "8574592", "old_code": "85745", "post_office": "青方", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ミナミマツウラグンシンカミゴトウチョウ", "neighborhood_kana": "エノキヅゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608543','{"jis": "43101", "kana": "エヌ・テイ・テイフアイナンス カブシキガイシヤ ミナミキユウシユウシテン", "name": "ＮＴＴファイナンス　株式会社　南九州支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "4-1太陽生命熊本第2ビル7F", "postal_code": "8608543", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608519','{"jis": "43101", "kana": "エヌテイテイニシニホン クマモトシテン", "name": "ＮＴＴ西日本　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "桜町", "banchi": "3-1", "postal_code": "8608519", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "サクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608536','{"jis": "43101", "kana": "カブシキカイシヤ クマニチカイカン", "name": "株式会社　熊日会館", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "上通町", "banchi": "2番33号", "postal_code": "8608536", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カミトオリチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('8608506','{"jis": "43101", "kana": "カブシキカイシヤ クマモトニチニチシンブンシヤ", "name": "株式会社　熊本日日新聞社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "世安町", "banchi": "172番地", "postal_code": "8608506", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヨヤスマチ", "alternates": []}');
+INSERT INTO office_data VALUES('8608506','{"jis": "43101", "kana": "カブシキカイシヤ クマモトニチニチシンブンシヤ", "name": "株式会社　熊本日日新聞社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "世安", "banchi": "1丁目5番1号", "postal_code": "8608506", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヨヤス", "alternates": []}');
 INSERT INTO office_data VALUES('8608539','{"jis": "43101", "kana": "カブシキカイシヤ トリニテイ", "name": "株式会社　トリニティ", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "妙体寺町", "banchi": "5番4号", "postal_code": "8608539", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ミョウタイジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608797','{"jis": "43101", "kana": "カブシキカイシヤ ユウチヨギンコウ クマモトシテン", "name": "株式会社　ゆうちょ銀行　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "1番1号", "postal_code": "8608797", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": [{"jis": "43101", "kana": "カブシキガイシヤ カンポセイメイ クマモトシテン", "name": "株式会社　かんぽ生命　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "1番1号", "postal_code": "8608797", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": []}, {"jis": "43101", "kana": "ニホンユウビン カブシキガイシヤ キユウシユウシシヤ", "name": "日本郵便　株式会社　九州支社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "1-1", "postal_code": "8608797", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": []}]}');
 INSERT INTO office_data VALUES('8608525','{"jis": "43101", "kana": "カブシキガイシヤ アステム クマモトエイギヨウブ", "name": "株式会社　アステム　熊本営業部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "八王寺町", "banchi": "33-57", "postal_code": "8608525", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハチオウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608509','{"jis": "43101", "kana": "カブシキガイシヤ カミヒロ", "name": "株式会社　紙弘", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "世安町", "banchi": "378-4", "postal_code": "8608509", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヨヤスマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608588','{"jis": "43101", "kana": "カブシキガイシヤ カリ-ノ", "name": "株式会社　カリーノ", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "安政町", "banchi": "1番2号", "postal_code": "8608588", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "アンセイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608619','{"jis": "43101", "kana": "カブシキガイシヤ キユウシユウシンキンクレジツトサ-ビス", "name": "株式会社　九州しんきんクレジットサービス", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "草葉町", "banchi": "4番20号熊本富士火災熊本ビル(熊本中央郵便局私書箱第129号)", "postal_code": "8608619", "old_code": "860  ", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "クサバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608501','{"jis": "43101", "kana": "カブシキガイシヤ クマモトギンコウ チユウオウシテン", "name": "株式会社　熊本銀行　中央支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "山崎町", "banchi": "44", "postal_code": "8608501", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヤマサキマチ", "alternates": []}');
```

### Comparing `posuto-2023.4.0/posuto/posuto.py` & `posuto-2023.5.0/posuto/posuto.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.4.0/posuto/prep.py` & `posuto-2023.5.0/posuto/prep.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.4.0/posuto/tests/test_basic.py` & `posuto-2023.5.0/posuto/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.4.0/posuto.egg-info/PKG-INFO` & `posuto-2023.5.0/posuto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `posuto-2023.4.0/setup.cfg` & `posuto-2023.5.0/setup.cfg`

 * *Files identical despite different names*

