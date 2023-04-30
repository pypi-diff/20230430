# Comparing `tmp/baekjoonapi-0.2.1.tar.gz` & `tmp/baekjoonapi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baekjoonapi-0.2.1.tar", max compression
+gzip compressed data, was "baekjoonapi-0.2.2.tar", max compression
```

## Comparing `baekjoonapi-0.2.1.tar` & `baekjoonapi-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      456 2023-03-09 15:10:51.953488 baekjoonapi-0.2.1/LICENSE.md
--rw-r--r--   0        0        0       99 2023-03-09 15:10:51.953488 baekjoonapi-0.2.1/README.md
--rw-r--r--   0        0        0     5635 2023-03-09 15:50:03.495860 baekjoonapi-0.2.1/bojapi/__init__.py
--rw-r--r--   0        0        0      477 2023-03-09 15:50:28.336701 baekjoonapi-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 baekjoonapi-0.2.1/setup.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 baekjoonapi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      456 2023-04-30 07:05:06.371000 baekjoonapi-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0       99 2023-04-30 07:05:06.371000 baekjoonapi-0.2.2/README.md
+-rw-r--r--   0        0        0     5587 2023-04-30 07:11:24.351000 baekjoonapi-0.2.2/bojapi/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-30 07:13:12.259000 baekjoonapi-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 baekjoonapi-0.2.2/PKG-INFO
```

### Comparing `baekjoonapi-0.2.1/bojapi/__init__.py` & `baekjoonapi-0.2.2/bojapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,16 @@
     def __init__(self, name):
         """유저의 정보를 가져옵니다 (Get user information)"""
         tiers = ["Unranked", "Bronze V", "Bronze IV", "Bronze III", "Bronze II", "Bronze I", "Silver V", "Silver IV", "Silver III", "Silver II", "Silver I", "Gold V", "Gold IV", "Gold III", "Gold II", "Gold I", "Platinum V", "Platinum I",
                  "Diamond IV", "Diamond III", "Diamond II", "Diamond I", "Ruby V", "Ruby IV", "Ruby III", "Ruby II", "Ruby I", "Master"]
         self.name = name
         apire = get("https://solved.ac/api/v3/user/show", params={"handle": name}, headers={"Content-Type": "application/json"}).json()
         self.bio = apire["bio"]
-        self.organizations = apire["organizations"]
-        self.badge = apire["badge"]
-        self.background = apire["background"]
+        self.badge = apire["badgeId"]
+        self.background = apire["backgroundId"]
         self.profileimage = apire["profileImageUrl"]
         self.solved = apire["solvedCount"]
         self.cla = apire["class"]
         self.classDecoration = apire["classDecoration"]
         self.tier = tiers[apire["tier"]]
         self.rating = apire["rating"]
         self.ratingByProblemsSum = apire["ratingByProblemsSum"]
```

### Comparing `baekjoonapi-0.2.1/PKG-INFO` & `baekjoonapi-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baekjoonapi
-Version: 0.2.1
+Version: 0.2.2
 Summary: BaekjoonAPI for Python
 Home-page: https://github.com/misilelab/baekjoonapi
 License: MisileLab License
 Author: MisileLaboratory
 Requires-Python: >=3.7,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: lxml (==4.9.2)
 Requires-Dist: random-user-agent (==1.0.1)
-Requires-Dist: requests (==2.28.2)
+Requires-Dist: requests (==2.29.0)
 Project-URL: Repository, https://github.com/misilelab/baekjoonapi
 Description-Content-Type: text/markdown
 
 # BaekjoonAPI
 
 BaekjoonAPI for python
```

