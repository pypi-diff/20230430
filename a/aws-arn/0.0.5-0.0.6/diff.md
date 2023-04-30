# Comparing `tmp/aws-arn-0.0.5.tar.gz` & `tmp/aws-arn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-arn-0.0.5.tar", last modified: Sun Apr 30 13:30:51 2023, max compression
+gzip compressed data, was "aws-arn-0.0.6.tar", last modified: Sun Apr 30 14:16:30 2023, max compression
```

## Comparing `aws-arn-0.0.5.tar` & `aws-arn-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:30:51.479533 aws-arn-0.0.5/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:30:51.479418 aws-arn-0.0.5/PKG-INFO
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)    48465 2023-04-30 13:20:23.000000 aws-arn-0.0.5/README.md
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:30:51.478722 aws-arn-0.0.5/aws_arn/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2898 2023-04-30 12:56:06.000000 aws-arn-0.0.5/aws_arn/__init__.py
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)   157803 2023-04-30 11:54:55.000000 aws-arn-0.0.5/aws_arn/arn.py
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2913 2023-04-30 13:03:37.000000 aws-arn-0.0.5/aws_arn/get_parser.py
--rwxr-xr-x   0 gabrielsoltz   (501) staff       (20)     1179 2023-04-30 13:28:30.000000 aws-arn-0.0.5/aws_arn/main.py
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:30:51.479273 aws-arn-0.0.5/aws_arn.egg-info/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/PKG-INFO
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      249 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/SOURCES.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)        1 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/dependency_links.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)       41 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/entry_points.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)        8 2023-04-30 13:30:51.000000 aws-arn-0.0.5/aws_arn.egg-info/top_level.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)       38 2023-04-30 13:30:51.479564 aws-arn-0.0.5/setup.cfg
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      712 2023-04-30 13:30:48.000000 aws-arn-0.0.5/setup.py
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 14:16:30.903705 aws-arn-0.0.6/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 14:16:30.903571 aws-arn-0.0.6/PKG-INFO
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)    46366 2023-04-30 13:49:11.000000 aws-arn-0.0.6/README.md
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 14:16:30.902718 aws-arn-0.0.6/aws_arn/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)     3000 2023-04-30 14:16:08.000000 aws-arn-0.0.6/aws_arn/__init__.py
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)   157808 2023-04-30 14:14:12.000000 aws-arn-0.0.6/aws_arn/data.py
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2913 2023-04-30 13:47:03.000000 aws-arn-0.0.6/aws_arn/get_parser.py
+-rwxr-xr-x   0 gabrielsoltz   (501) staff       (20)     1115 2023-04-30 14:15:33.000000 aws-arn-0.0.6/aws_arn/main.py
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 14:16:30.903389 aws-arn-0.0.6/aws_arn.egg-info/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 14:16:30.000000 aws-arn-0.0.6/aws_arn.egg-info/PKG-INFO
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      250 2023-04-30 14:16:30.000000 aws-arn-0.0.6/aws_arn.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)        1 2023-04-30 14:16:30.000000 aws-arn-0.0.6/aws_arn.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)       41 2023-04-30 14:16:30.000000 aws-arn-0.0.6/aws_arn.egg-info/entry_points.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)        8 2023-04-30 14:16:30.000000 aws-arn-0.0.6/aws_arn.egg-info/top_level.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)       38 2023-04-30 14:16:30.903737 aws-arn-0.0.6/setup.cfg
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      712 2023-04-30 14:16:21.000000 aws-arn-0.0.6/setup.py
```

### Comparing `aws-arn-0.0.5/aws_arn/__init__.py` & `aws-arn-0.0.6/aws_arn/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 try:
-    from arn import aws_arn
+    from data import aws_arn_data
 except ModuleNotFoundError:
-    from aws_arn.arn import aws_arn
+    from aws_arn.data import aws_arn_data
 
 
 def list_services():
-    for i in aws_arn:
+    for i in aws_arn_data:
         print(i)
-    print("Total number of services: ", len(aws_arn))
+    print("Total number of services: ", len(aws_arn_data))
 
 def list_sub_services():
     count_resources = 0
-    for i in aws_arn.values():
+    for i in aws_arn_data.values():
         for j in i:
             print(j)
             count_resources += 1
     print("Total number of resources: ", count_resources)
 
 def list_sub_services_for_service(service):
-    for i in aws_arn[service]:
+    for i in aws_arn_data[service]:
         print(i)
 
 def list_asff_resources():
-    for services in aws_arn:
-        for sub_services in aws_arn[services]:
-            if aws_arn[services][sub_services]["asff_name"] != "":
-                print (aws_arn[services][sub_services]["asff_name"])
+    for services in aws_arn_data:
+        for sub_services in aws_arn_data[services]:
+            if aws_arn_data[services][sub_services]["asff_name"] != "":
+                print (aws_arn_data[services][sub_services]["asff_name"])
 
 def generate_markdown_table():
     header = "| Service | ARN Format |\n| --- | --- |\n"
     rows = []
-    for service in aws_arn:
+    for service in aws_arn_data:
         arn_breaks = ""
-        for sub_service in aws_arn[service]:
-            arn_breaks += sub_service + ": `" + aws_arn[service][sub_service]["arn_format"] + "`<br>"
+        for sub_service in aws_arn_data[service]:
+            arn_breaks += sub_service + ": `" + aws_arn_data[service][sub_service]["arn_format"] + "`<br>"
         rows.append(f"| {service} | {arn_breaks} |")
     return header + "\n".join(rows)
 
 def generate_arn(
     resource_id,
     resource_type,
     sub_resource_type,
     region,
     account,
     partition,
 ):
     try:
-        arn = aws_arn[resource_type][sub_resource_type]["arn_format"].format(
+        arn = aws_arn_data[resource_type][sub_resource_type]["arn_format"].format(
             partition=partition, region=region, account=account, resource_id=resource_id
         )
     except KeyError as e:
         print("Invalid resource type or sub resource type", e)
         return False
     return arn
 
 def check_resource_id_regexp(
     resource_id,
     resource_type,
     sub_resource_type
 ):
     import re
-    pattern = re.compile(aws_arn[resource_type][sub_resource_type]["id_regexp"])
-    # print (aws_arn[resource_type][sub_resource_type]["id_regexp"])
+    pattern = re.compile(aws_arn_data[resource_type][sub_resource_type]["id_regexp"])
+    # print (aws_arn_data[resource_type][sub_resource_type]["id_regexp"])
 
     return bool(re.search(pattern, resource_id))
 
 def get_resource_id_from_arn(arn):
     import re
     service = get_service_from_arn(arn)
     sub_service = get_sub_service_from_arn(arn)
-    regexp = aws_arn[service][sub_service]["id_regexp"]
+    regexp = aws_arn_data[service][sub_service]["id_regexp"]
     if regexp.startswith("^"):
         regexp = regexp[1:]
     pattern = re.compile(regexp)
     search = re.search(pattern, arn)
     if bool(search) == False:
         print ("No match found")
         return False
@@ -89,12 +89,12 @@
 def get_account_from_arn(arn):
     return arn.split(":")[4]
 
 def get_region_from_arn(arn):
     return arn.split(":")[3]
 
 def get_service_from_asff_resource(asff_resource):
-    for service in aws_arn:
-        for sub_service in aws_arn[service]:
-            if aws_arn[service][sub_service]["asff_name"] == asff_resource:
+    for service in aws_arn_data:
+        for sub_service in aws_arn_data[service]:
+            if aws_arn_data[service][sub_service]["asff_name"] == asff_resource:
                 return service, sub_service
     return False
```

### Comparing `aws-arn-0.0.5/aws_arn/arn.py` & `aws-arn-0.0.6/aws_arn/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-aws_arn = {
+aws_arn_data = {
     "acm": {
         "certificate": {
             "arn_format": "arn:{partition}:acm:{region}:{account}:certificate/{resource_id}",
             "id_name": "CertificateId",
             "id_regexp": "([a-z0-9-]+)",
             "asff_name": "AwsCertificateManagerCertificate",
             "cloudformation": "AWS::CertificateManager::Certificate",
```

### Comparing `aws-arn-0.0.5/aws_arn/get_parser.py` & `aws-arn-0.0.6/aws_arn/get_parser.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.5/aws_arn/main.py` & `aws-arn-0.0.6/aws_arn/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/env python3
 
 import sys
 
 
 try:
-    from arn import aws_arn
     from get_parser import get_parser
     from __init__ import *
 except ModuleNotFoundError:
-    from aws_arn.arn import aws_arn
     from aws_arn.get_parser import get_parser
     from aws_arn.__init__ import *
 
 def main():
     parser = get_parser()
     args = parser.parse_args()
     print("Args:", args)
```

### Comparing `aws-arn-0.0.5/setup.py` & `aws-arn-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='aws-arn',
-    version='0.0.5',
+    version='0.0.6',
     description='A library to work with AWS ARNs',
     packages=["aws_arn"],
     install_requires=[
     ],
     entry_points={
         'console_scripts': [
             'aws-arn = aws_arn:main',
```

