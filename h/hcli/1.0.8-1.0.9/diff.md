# Comparing `tmp/hcli-1.0.8.tar.gz` & `tmp/hcli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcli-1.0.8.tar", last modified: Tue Apr  4 17:28:01 2023, max compression
+gzip compressed data, was "hcli-1.0.9.tar", last modified: Tue Apr  4 17:30:36 2023, max compression
```

## Comparing `hcli-1.0.8.tar` & `hcli-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:28:01.990709 hcli-1.0.8/
--rw-r--r--   0 joshuakock   (501) staff       (20)      187 2023-04-04 17:28:01.990547 hcli-1.0.8/PKG-INFO
--rw-r--r--   0 joshuakock   (501) staff       (20)     1195 2023-04-03 16:10:07.000000 hcli-1.0.8/README.md
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:28:01.985996 hcli-1.0.8/hcli/
--rw-r--r--   0 joshuakock   (501) staff       (20)        0 2023-04-03 12:59:31.000000 hcli-1.0.8/hcli/__init__.py
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:28:01.987148 hcli-1.0.8/hcli/api/
--rw-r--r--   0 joshuakock   (501) staff       (20)        0 2023-04-03 15:52:35.000000 hcli-1.0.8/hcli/api/__init__.py
--rw-r--r--   0 joshuakock   (501) staff       (20)      633 2023-04-04 16:58:26.000000 hcli-1.0.8/hcli/api/utils.py
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:28:01.989371 hcli-1.0.8/hcli/commands/
--rw-r--r--   0 joshuakock   (501) staff       (20)        0 2023-04-03 15:52:35.000000 hcli-1.0.8/hcli/commands/__init__.py
--rw-r--r--   0 joshuakock   (501) staff       (20)     1334 2023-04-03 12:58:06.000000 hcli-1.0.8/hcli/commands/auth.py
--rw-r--r--   0 joshuakock   (501) staff       (20)     6172 2023-04-04 17:10:12.000000 hcli-1.0.8/hcli/commands/machines.py
--rw-r--r--   0 joshuakock   (501) staff       (20)     1439 2023-04-04 17:19:00.000000 hcli-1.0.8/hcli/commands/organizations.py
--rw-r--r--   0 joshuakock   (501) staff       (20)     1672 2023-04-04 17:25:18.000000 hcli-1.0.8/hcli/commands/projects.py
--rw-r--r--   0 joshuakock   (501) staff       (20)     1430 2023-04-04 16:58:26.000000 hcli-1.0.8/hcli/commands/set.py
--rw-r--r--   0 joshuakock   (501) staff       (20)     5583 2023-04-04 17:02:47.000000 hcli-1.0.8/hcli/commands/stores.py
--rw-r--r--   0 joshuakock   (501) staff       (20)     1676 2023-04-04 17:12:04.000000 hcli-1.0.8/hcli/main.py
--rw-r--r--   0 joshuakock   (501) staff       (20)      859 2023-04-04 17:27:08.000000 hcli-1.0.8/hcli/permissions.py
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:28:01.990116 hcli-1.0.8/hcli/utils/
--rw-r--r--   0 joshuakock   (501) staff       (20)        0 2023-04-03 15:52:28.000000 hcli-1.0.8/hcli/utils/__init__.py
--rw-r--r--   0 joshuakock   (501) staff       (20)     1081 2023-04-03 15:58:33.000000 hcli-1.0.8/hcli/utils/permanent_storage.py
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:28:01.986890 hcli-1.0.8/hcli.egg-info/
--rw-r--r--   0 joshuakock   (501) staff       (20)      187 2023-04-04 17:28:01.000000 hcli-1.0.8/hcli.egg-info/PKG-INFO
--rw-r--r--   0 joshuakock   (501) staff       (20)      508 2023-04-04 17:28:01.000000 hcli-1.0.8/hcli.egg-info/SOURCES.txt
--rw-r--r--   0 joshuakock   (501) staff       (20)        1 2023-04-04 17:28:01.000000 hcli-1.0.8/hcli.egg-info/dependency_links.txt
--rw-r--r--   0 joshuakock   (501) staff       (20)       39 2023-04-04 17:28:01.000000 hcli-1.0.8/hcli.egg-info/entry_points.txt
--rw-r--r--   0 joshuakock   (501) staff       (20)       17 2023-04-04 17:28:01.000000 hcli-1.0.8/hcli.egg-info/requires.txt
--rw-r--r--   0 joshuakock   (501) staff       (20)        5 2023-04-04 17:28:01.000000 hcli-1.0.8/hcli.egg-info/top_level.txt
--rw-r--r--   0 joshuakock   (501) staff       (20)       38 2023-04-04 17:28:01.990756 hcli-1.0.8/setup.cfg
--rw-r--r--   0 joshuakock   (501) staff       (20)      435 2023-04-04 17:28:00.000000 hcli-1.0.8/setup.py
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:30:36.946668 hcli-1.0.9/
+-rw-r--r--   0 joshuakock   (501) staff       (20)      187 2023-04-04 17:30:36.946518 hcli-1.0.9/PKG-INFO
+-rw-r--r--   0 joshuakock   (501) staff       (20)     1195 2023-04-03 16:10:07.000000 hcli-1.0.9/README.md
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:30:36.939496 hcli-1.0.9/hcli/
+-rw-r--r--   0 joshuakock   (501) staff       (20)        0 2023-04-03 12:59:31.000000 hcli-1.0.9/hcli/__init__.py
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:30:36.941096 hcli-1.0.9/hcli/api/
+-rw-r--r--   0 joshuakock   (501) staff       (20)        0 2023-04-03 15:52:35.000000 hcli-1.0.9/hcli/api/__init__.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)      633 2023-04-04 16:58:26.000000 hcli-1.0.9/hcli/api/utils.py
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:30:36.945732 hcli-1.0.9/hcli/commands/
+-rw-r--r--   0 joshuakock   (501) staff       (20)        0 2023-04-03 15:52:35.000000 hcli-1.0.9/hcli/commands/__init__.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     1334 2023-04-03 12:58:06.000000 hcli-1.0.9/hcli/commands/auth.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     6172 2023-04-04 17:10:12.000000 hcli-1.0.9/hcli/commands/machines.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     1439 2023-04-04 17:19:00.000000 hcli-1.0.9/hcli/commands/organizations.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     1672 2023-04-04 17:25:18.000000 hcli-1.0.9/hcli/commands/projects.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     1430 2023-04-04 16:58:26.000000 hcli-1.0.9/hcli/commands/set.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     6111 2023-04-04 17:30:14.000000 hcli-1.0.9/hcli/commands/stores.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     1676 2023-04-04 17:12:04.000000 hcli-1.0.9/hcli/main.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)      859 2023-04-04 17:27:08.000000 hcli-1.0.9/hcli/permissions.py
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:30:36.946161 hcli-1.0.9/hcli/utils/
+-rw-r--r--   0 joshuakock   (501) staff       (20)        0 2023-04-03 15:52:28.000000 hcli-1.0.9/hcli/utils/__init__.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     1081 2023-04-03 15:58:33.000000 hcli-1.0.9/hcli/utils/permanent_storage.py
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-04-04 17:30:36.940830 hcli-1.0.9/hcli.egg-info/
+-rw-r--r--   0 joshuakock   (501) staff       (20)      187 2023-04-04 17:30:36.000000 hcli-1.0.9/hcli.egg-info/PKG-INFO
+-rw-r--r--   0 joshuakock   (501) staff       (20)      508 2023-04-04 17:30:36.000000 hcli-1.0.9/hcli.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuakock   (501) staff       (20)        1 2023-04-04 17:30:36.000000 hcli-1.0.9/hcli.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuakock   (501) staff       (20)       39 2023-04-04 17:30:36.000000 hcli-1.0.9/hcli.egg-info/entry_points.txt
+-rw-r--r--   0 joshuakock   (501) staff       (20)       17 2023-04-04 17:30:36.000000 hcli-1.0.9/hcli.egg-info/requires.txt
+-rw-r--r--   0 joshuakock   (501) staff       (20)        5 2023-04-04 17:30:36.000000 hcli-1.0.9/hcli.egg-info/top_level.txt
+-rw-r--r--   0 joshuakock   (501) staff       (20)       38 2023-04-04 17:30:36.946700 hcli-1.0.9/setup.cfg
+-rw-r--r--   0 joshuakock   (501) staff       (20)      435 2023-04-04 17:30:35.000000 hcli-1.0.9/setup.py
```

### Comparing `hcli-1.0.8/README.md` & `hcli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/api/utils.py` & `hcli-1.0.9/hcli/api/utils.py`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/commands/auth.py` & `hcli-1.0.9/hcli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/commands/machines.py` & `hcli-1.0.9/hcli/commands/machines.py`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/commands/organizations.py` & `hcli-1.0.9/hcli/commands/organizations.py`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/commands/projects.py` & `hcli-1.0.9/hcli/commands/projects.py`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/commands/set.py` & `hcli-1.0.9/hcli/commands/set.py`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/commands/stores.py` & `hcli-1.0.9/hcli/commands/stores.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import typer
 from rich import print
 from rich.table import Table
 
 from hcli.api.utils import ApiClient
+from hcli.permissions import auth_required, project_and_org_required
 from hcli.utils.permanent_storage import read_field
 
 app = typer.Typer()
 
 token = read_field("token")
 organization_id = read_field("organization_id")
 project_id = read_field("project_id")
 
 core_api = ApiClient(
     "https://api.huddu.io", headers={"Authorization": f"Token {token}"}
 )
 
 
 def make_store_client(client_id, management_token):
+    auth_required()
+    project_and_org_required()
     return ApiClient(
         f"https://store.huddu.io",
         headers={"X-Client-ID": client_id, "X-Client-Secret": management_token},
     )
 
 
 @app.command()
 def create(name: str = typer.Option(..., prompt=True)):
+    auth_required()
+    project_and_org_required()
     stores_api = ApiClient(
         f"https://store.huddu.io", headers={"Authorization": f"Token {token}"}
     )
 
     res = stores_api.request(
         "POST",
         "setup",
@@ -39,14 +44,16 @@
         print(res)
     else:
         print(f"[green]✨ Successfully created a new store [/green]")
 
 
 @app.command()
 def list(skip: int = 0):
+    auth_required()
+    project_and_org_required()
     res = core_api.request(
         "GET",
         f"/search?resource=resources&organization={organization_id}&q=type:store%20$and%20project:{project_id}&limit=10&skip={skip}",
     )
 
     table = Table()
 
@@ -65,28 +72,32 @@
         print(table)
     else:
         print("No entries. You can create a new store with huddu stores create")
 
 
 @app.command()
 def info(store_name: str, show_management_token: bool = False):
+    auth_required()
+    project_and_org_required()
     res = core_api.request(
         "GET",
         f"/search?resource=resources&organization={organization_id}&q=type:store $and project:{project_id} $and name:{store_name}&limit=1",
     )
 
     store_resource = res.get("data")[0]
     if not show_management_token:
         store_resource["management_token"] = "*****"
 
     print(store_resource)
 
 
 @app.command()
 def entries_get(store_name: str, key: str):
+    auth_required()
+    project_and_org_required()
     res = core_api.request(
         "GET",
         f"/search?resource=resources&organization={organization_id}&q=type:store $and project:{project_id} $and name:{store_name}&limit=1",
     )
     store_resource = res["data"][0]
 
     stores_api = make_store_client(
@@ -102,14 +113,16 @@
 
 @app.command()
 def entries_set(
         store_name: str,
         key: str,
         value: str = typer.Option(..., prompt=True),
 ):
+    auth_required()
+    project_and_org_required()
     res = core_api.request(
         "GET",
         f"/search?resource=resources&organization={organization_id}&q=type:store $and project:{project_id} $and name:{store_name}&limit=1",
     )
     store_resource = res["data"][0]
 
     stores_api = make_store_client(
@@ -129,14 +142,16 @@
 
 @app.command()
 def entries_update(
         store_name: str,
         key: str,
         value: str = typer.Option(..., prompt=True),
 ):
+    auth_required()
+    project_and_org_required()
     res = core_api.request(
         "GET",
         f"/search?resource=resources&organization={organization_id}&q=type:store $and project:{project_id} $and name:{store_name}&limit=1",
     )
     store_resource = res["data"][0]
 
     stores_api = make_store_client(
@@ -146,14 +161,16 @@
     stores_api.request("POST", f"documents", body={"key": key, "value": value})
 
     print("[green]Updated entry[/green]")
 
 
 @app.command()
 def entries_delete(store_name: str, key: str):
+    auth_required()
+    project_and_org_required()
     res = core_api.request(
         "GET",
         f"/search?resource=resources&organization={organization_id}&q=type:store $and project:{project_id} $and name:{store_name}&limit=1",
     )
     store_resource = res["data"][0]
 
     stores_api = make_store_client(
@@ -166,14 +183,16 @@
 
 
 @app.command()
 def delete(
         store_name: str,
         confirm_deletion: str = typer.Option(..., prompt="Are you sure? (y/n)"),
 ):
+    auth_required()
+    project_and_org_required()
     if confirm_deletion == "y":
         res = core_api.request(
             "GET",
             f"/search?resource=resources&organization={organization_id}&q=type:store $and project:{project_id} $and name:{store_name}&limit=1",
         )
         store_resource = res["data"][0]
```

### Comparing `hcli-1.0.8/hcli/main.py` & `hcli-1.0.9/hcli/main.py`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/permissions.py` & `hcli-1.0.9/hcli/permissions.py`

 * *Files identical despite different names*

### Comparing `hcli-1.0.8/hcli/utils/permanent_storage.py` & `hcli-1.0.9/hcli/utils/permanent_storage.py`

 * *Files identical despite different names*

