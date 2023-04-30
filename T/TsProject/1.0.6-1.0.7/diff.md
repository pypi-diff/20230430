# Comparing `tmp/TsProject-1.0.6.tar.gz` & `tmp/TsProject-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TsProject-1.0.6.tar", last modified: Sat Apr 29 13:23:20 2023, max compression
+gzip compressed data, was "TsProject-1.0.7.tar", last modified: Sun Apr 30 02:21:43 2023, max compression
```

## Comparing `TsProject-1.0.6.tar` & `TsProject-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 13:23:20.121132 TsProject-1.0.6/
--rw-rw-rw-   0        0        0       17 2023-04-29 11:59:06.000000 TsProject-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      566 2023-04-29 13:23:20.120142 TsProject-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-04-29 12:15:24.000000 TsProject-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 13:23:20.101282 TsProject-1.0.6/TsProject/
--rw-rw-rw-   0        0        0      400 2023-04-29 13:21:40.000000 TsProject-1.0.6/TsProject/TsExtra.py
--rw-rw-rw-   0        0        0        0 2023-04-29 12:28:22.000000 TsProject-1.0.6/TsProject/TsINIT.txt
--rw-rw-rw-   0        0        0     3238 2023-04-29 13:22:59.000000 TsProject-1.0.6/TsProject/TsPost.py
--rw-rw-rw-   0        0        0        0 2023-04-29 12:16:15.000000 TsProject-1.0.6/TsProject/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 13:23:20.118135 TsProject-1.0.6/TsProject.egg-info/
--rw-rw-rw-   0        0        0      566 2023-04-29 13:23:19.000000 TsProject-1.0.6/TsProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-29 13:23:20.000000 TsProject-1.0.6/TsProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 13:23:19.000000 TsProject-1.0.6/TsProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-29 13:23:20.000000 TsProject-1.0.6/TsProject.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 13:23:20.000000 TsProject-1.0.6/TsProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-29 13:23:20.000000 TsProject-1.0.6/TsProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-29 13:23:19.000000 TsProject-1.0.6/TsProject.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-29 13:23:20.121132 TsProject-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     4232 2023-04-29 13:23:04.000000 TsProject-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 02:21:43.003970 TsProject-1.0.7/
+-rw-rw-rw-   0        0        0       17 2023-04-29 11:59:06.000000 TsProject-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      566 2023-04-30 02:21:43.002958 TsProject-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-04-29 12:15:24.000000 TsProject-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 02:21:42.894264 TsProject-1.0.7/TsProject/
+-rw-rw-rw-   0        0        0      400 2023-04-30 02:20:55.000000 TsProject-1.0.7/TsProject/TsExtra.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 12:28:22.000000 TsProject-1.0.7/TsProject/TsINIT.txt
+-rw-rw-rw-   0        0        0     3631 2023-04-30 02:20:57.000000 TsProject-1.0.7/TsProject/TsPost.py
+-rw-rw-rw-   0        0        0      152 2023-04-30 02:20:35.000000 TsProject-1.0.7/TsProject/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 02:21:42.996485 TsProject-1.0.7/TsProject/__pycache__/
+-rw-rw-rw-   0        0        0     2367 2023-04-30 02:20:29.000000 TsProject-1.0.7/TsProject/__pycache__/TsPost.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-04-30 02:21:42.994515 TsProject-1.0.7/TsProject.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-04-30 02:21:42.000000 TsProject-1.0.7/TsProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-04-30 02:21:42.000000 TsProject-1.0.7/TsProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 02:21:42.000000 TsProject-1.0.7/TsProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-30 02:21:42.000000 TsProject-1.0.7/TsProject.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 02:21:42.000000 TsProject-1.0.7/TsProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-30 02:21:42.000000 TsProject-1.0.7/TsProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-29 13:23:19.000000 TsProject-1.0.7/TsProject.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-30 02:21:43.001452 TsProject-1.0.7/dist/
+-rw-rw-rw-   0        0        0     5654 2023-04-30 02:21:22.000000 TsProject-1.0.7/dist/TsProject-1.0.6-py3-none-any.whl
+-rw-rw-rw-   0        0        0    13032 2023-04-30 02:21:22.000000 TsProject-1.0.7/dist/TsProject-1.0.6.tar.gz
+-rw-rw-rw-   0        0        0       42 2023-04-30 02:21:43.003970 TsProject-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     4232 2023-04-30 02:21:36.000000 TsProject-1.0.7/setup.py
```

### Comparing `TsProject-1.0.6/PKG-INFO` & `TsProject-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsProject
-Version: 1.0.6
+Version: 1.0.7
 Summary: TsProject Init: File POST to Cloud
 Home-page: https://www.tsginkgo.cn
 Author: Kqy
 Author-email: 2765301200@qq.com
 License: MIT
 Project-URL: Bug Reports, https://www.tsginkgo.cn
 Project-URL: Funding, https://www.tsginkgo.cn
```

### Comparing `TsProject-1.0.6/TsProject/TsPost.py` & `TsProject-1.0.7/TsProject/TsPost.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 # -*- coding: utf-8 -*-
-# @Time : 2023/04/29 21:06
+# @Time : 2023/04/30 10:00
 # @Author : Kqy
-# @Version : 1.0.6
+# @Version : 1.0.7
 # @Website : https://www.tsginkgo.cn/
 
 import os;
 import json;
 import requests;
 
 global NowVersion, Use;
-NowVersion = "1.0.6";
+NowVersion = "1.0.7";
 
 # Edit The Lambda
 def TSFileUploadPost(FilePath=None, UploaderKey=None, Description=None):    # Def Post Lambda
     """
         你可以通过此函数来上传文件至云端
     """
 
     if (not Use):
-        return {"code": -1, "error": f'你需要更新到最新版本！'};
+        return {"code": -1, "error": '你需要更新到最新版本！'};
     
     if (not FilePath) or (not UploaderKey):
-        return {"code": -1, "error": f'文件地址与API KEY均必须填写！'};
+        return {"code": -1, "error": '文件地址与API KEY均必须填写！'};
 
     if (os.path.getsize(FilePath)>52428800):
         return {"code": -1, "error": f'文件{FilePath}超过最大大小限制50MB！'};
 
     UploadUrl = "https://www.tsginkgo.cn/file-uploader/api/upload/public/";
 
     try:
         data = {'UploaderKey': UploaderKey, 'Description': Description}; # Post Data
         files = {'file': open(FilePath, 'rb')};  # Post File
         res = requests.post(UploadUrl, data=data, files=files).text;    # Get Post  
-        return {"code": 0, "res": res};  # Return Result
+        return json.loads(res);
+        # return {"code": 0, "res": res};  # Return Result
     except Exception as e:
         return {"code": -1, "error": str(e)};
 
 def VersionCheck():
-    Req = requests.get("https://www.tsginkgo.cn/file-uploader/api/pypackage/NewVersion.json").text;
-    Req = json.loads(Req);
+    try:
+        Req = requests.get("https://www.tsginkgo.cn/file-uploader/api/pypackage/NewVersion.json").text;
+        Req = json.loads(Req);
 
-    for items in Req:
-        if items["Type"]=="Release":
-            NewVersion = items["NewVersion"];
-            DownloadCmd = items["DownloadCmd"];
-            MoreUrl = items["MoreUrl"];
-            Force = items["Force"];
-            BeginColorRed = '\033[1;31m';
-            BeginColorBlue = '\033[1;34m';
-            EndColor = '\033[0m';
-            if (NewVersion>NowVersion):
-                # print("Need Update");
-                print("-"*64);
-                print(f"{BeginColorRed}你的 TsProject 库需要更新！{EndColor}");
-                print(f"当前版本:{NowVersion}，最新版本:{NewVersion}");
-                if (Force):
-                    print(f"{BeginColorRed}新版本为强制更新版本，你必须更新到最新版本才能继续使用{EndColor}");
-                    print(f"你可以通过在终端使用'{BeginColorBlue}{DownloadCmd}{EndColor}'命令来获得更新");
-                    print(f"在{MoreUrl}了解更多");
+        for items in Req:
+            if items["Type"]=="Release":
+                NewVersion = items["NewVersion"];
+                DownloadCmd = items["DownloadCmd"];
+                MoreUrl = items["MoreUrl"];
+                Force = items["Force"];
+                BeginColorRed = '\033[1;31m';
+                BeginColorBlue = '\033[1;34m';
+                EndColor = '\033[0m';
+                if (NewVersion>NowVersion):
+                    # print("Need Update");
                     print("-"*64);
-                    Use = False;
-                    return False;
+                    print(f"{BeginColorRed}你的 TsProject 库需要更新！{EndColor}");
+                    print(f"当前版本:{NowVersion}，最新版本:{NewVersion}");
+                    if (Force):
+                        print(f"{BeginColorRed}新版本为强制更新版本，你必须更新到最新版本才能继续使用{EndColor}");
+                        print(f"你可以通过在终端使用'{BeginColorBlue}{DownloadCmd}{EndColor}'命令来获得更新");
+                        print(f"在{MoreUrl}了解更多");
+                        print("-"*64);
+                        Use = False;
+                        return False;
+                    else:
+                        print(f"{BeginColorBlue}新版本为不强制更新版本，你可以继续使用此旧版本{EndColor}");
+                        print(f"你可以通过在终端使用'{BeginColorBlue}{DownloadCmd}{EndColor}'命令来获得更新");
+                        print(f"在{MoreUrl}了解更多");
+                        print("-"*64);
+                        Use = True;
+                        return True;
                 else:
-                    print(f"{BeginColorBlue}新版本为不强制更新版本，你可以继续使用此旧版本{EndColor}");
-                    print(f"你可以通过在终端使用'{BeginColorBlue}{DownloadCmd}{EndColor}'命令来获得更新");
-                    print(f"在{MoreUrl}了解更多");
+                    print("-"*64);
+                    print(f"TsProject {BeginColorBlue}{NowVersion}{EndColor}");
                     print("-"*64);
                     Use = True;
                     return True;
-            else:
-                print("-"*64);
-                print(f"TsProject {BeginColorBlue}{NowVersion}{EndColor}");
-                print("-"*64);
-                Use = True;
-                return True;
+    except Exception as error:
+        print("-"*64);
+        print(f"TsProject {BeginColorBlue}{NowVersion}   OFFLINE{EndColor}");
+        print("-"*64);
+        Use = True;
+        return True;    
 
 Use = VersionCheck();
 
 if __name__ == "__main__":
     print(TSFileUploadPost());
```

### Comparing `TsProject-1.0.6/TsProject.egg-info/PKG-INFO` & `TsProject-1.0.7/TsProject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsProject
-Version: 1.0.6
+Version: 1.0.7
 Summary: TsProject Init: File POST to Cloud
 Home-page: https://www.tsginkgo.cn
 Author: Kqy
 Author-email: 2765301200@qq.com
 License: MIT
 Project-URL: Bug Reports, https://www.tsginkgo.cn
 Project-URL: Funding, https://www.tsginkgo.cn
```

### Comparing `TsProject-1.0.6/setup.py` & `TsProject-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="TsProject",
-    version="1.0.6",
+    version="1.0.7",
     keywords=['Tsginkgo', 'Ksuser', 'Kqy'],
     description="TsProject Init: File POST to Cloud",
     long_description=long_description,
     license="MIT",
     url="https://www.tsginkgo.cn",
     author="Kqy",
     author_email="2765301200@qq.com",
```

