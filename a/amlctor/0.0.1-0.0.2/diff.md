# Comparing `tmp/amlctor-0.0.1.tar.gz` & `tmp/amlctor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amlctor-0.0.1.tar", last modified: Sat Apr 29 11:52:15 2023, max compression
+gzip compressed data, was "amlctor-0.0.2.tar", last modified: Sun Apr 30 17:50:47 2023, max compression
```

## Comparing `amlctor-0.0.1.tar` & `amlctor-0.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rwxr-xr-x   0        0        0       60 2023-04-29 11:40:55.827359 amlctor-0.0.1/.gitignore
--rw-r--r--   0        0        0     1078 2023-04-26 11:53:55.773431 amlctor-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     9020 2023-04-24 10:36:05.672888 amlctor-0.0.1/README.md
--rwxr-xr-x   0        0        0       55 2023-04-29 11:52:03.866821 amlctor-0.0.1/amlctor/__init__.py
--rwxr-xr-x   0        0        0      171 2023-04-26 12:04:07.833727 amlctor-0.0.1/amlctor/__main__.py
--rwxr-xr-x   0        0        0        0 2023-02-25 04:17:23.449214 amlctor-0.0.1/amlctor/amlctor.py
--rwxr-xr-x   0        0        0        0 2023-02-23 16:48:42.440743 amlctor-0.0.1/amlctor/apply/__init__.py
--rwxr-xr-x   0        0        0     8791 2023-04-26 12:16:54.047808 amlctor-0.0.1/amlctor/apply/apply.py
--rwxr-xr-x   0        0        0        0 2023-02-19 20:11:02.961852 amlctor-0.0.1/amlctor/confs/__init__.py
--rwxr-xr-x   0        0        0      687 2023-04-28 18:20:16.796132 amlctor-0.0.1/amlctor/confs/configs.py
--rwxr-xr-x   0        0        0     5055 2023-04-25 12:46:11.091783 amlctor-0.0.1/amlctor/core.py
--rwxr-xr-x   0        0        0        0 2023-04-02 07:51:59.583621 amlctor-0.0.1/amlctor/denv/__init__.py
--rwxr-xr-x   0        0        0     4302 2023-04-28 18:28:53.978801 amlctor-0.0.1/amlctor/denv/denv.py
--rwxr-xr-x   0        0        0      803 2023-04-25 12:42:33.934318 amlctor-0.0.1/amlctor/denv/dot_env_loader.py
--rwxr-xr-x   0        0        0     2591 2023-03-31 19:45:35.301488 amlctor-0.0.1/amlctor/exceptions.py
--rwxr-xr-x   0        0        0        0 2023-02-23 16:48:40.988088 amlctor-0.0.1/amlctor/init/__init__.py
--rwxr-xr-x   0        0        0     9252 2023-04-26 12:29:03.865986 amlctor-0.0.1/amlctor/init/args_handling.py
--rwxr-xr-x   0        0        0     6578 2023-04-26 12:15:24.363525 amlctor-0.0.1/amlctor/init/init.py
--rwxr-xr-x   0        0        0     2518 2023-04-28 15:07:38.962403 amlctor-0.0.1/amlctor/init/init_structure.py
--rwxr-xr-x   0        0        0     4665 2023-04-25 12:43:48.131909 amlctor-0.0.1/amlctor/input.py
--rwxr-xr-x   0        0        0        0 2023-02-25 04:18:40.776054 amlctor-0.0.1/amlctor/rename/__init__.py
--rwxr-xr-x   0        0        0     3655 2023-04-23 09:56:52.168839 amlctor-0.0.1/amlctor/rename/rename.py
--rwxr-xr-x   0        0        0        0 2023-02-23 16:48:38.940819 amlctor-0.0.1/amlctor/run/__init__.py
--rwxr-xr-x   0        0        0     3606 2023-04-15 10:45:35.001519 amlctor-0.0.1/amlctor/run/run.py
--rwxr-xr-x   0        0        0     1622 2023-04-26 12:16:29.679730 amlctor-0.0.1/amlctor/schemas.py
--rwxr-xr-x   0        0        0        0 2023-02-19 14:56:55.871703 amlctor-0.0.1/amlctor/src/__init__.py
--rwxr-xr-x   0        0        0      177 2023-04-11 18:59:17.691227 amlctor-0.0.1/amlctor/src/templates/apply/aml
--rwxr-xr-x   0        0        0      483 2023-04-12 18:26:23.159935 amlctor-0.0.1/amlctor/src/templates/apply/data_loaders
--rwxr-xr-x   0        0        0      543 2023-03-01 17:56:39.337816 amlctor-0.0.1/amlctor/src/templates/init/conda_dependencies
--rwxr-xr-x   0        0        0      443 2023-04-22 05:55:24.837867 amlctor-0.0.1/amlctor/src/templates/init/dot_amlignore
--rwxr-xr-x   0        0        0      274 2023-04-22 08:11:36.650858 amlctor-0.0.1/amlctor/src/templates/init/dot_env
--rwxr-xr-x   0        0        0      776 2023-04-09 12:13:41.742028 amlctor-0.0.1/amlctor/src/templates/init/env_vars
--rwxr-xr-x   0        0        0     1442 2023-04-12 19:12:37.227543 amlctor-0.0.1/amlctor/src/templates/init/settings
--rwxr-xr-x   0        0        0        0 2023-02-19 14:57:07.938361 amlctor-0.0.1/amlctor/tests/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-21 17:33:46.575063 amlctor-0.0.1/amlctor/tests/apply/__init__.py
--rwxr-xr-x   0        0        0     2597 2023-04-26 12:18:34.780132 amlctor-0.0.1/amlctor/tests/apply/test_apply_path.py
--rwxr-xr-x   0        0        0        0 2023-02-21 17:33:39.745273 amlctor-0.0.1/amlctor/tests/core/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-21 17:33:31.748011 amlctor-0.0.1/amlctor/tests/init/__init__.py
--rwxr-xr-x   0        0        0     1477 2023-04-26 12:19:07.456238 amlctor-0.0.1/amlctor/tests/init/test_env_bank.py
--rwxr-xr-x   0        0        0        0 2023-02-21 17:33:54.684018 amlctor-0.0.1/amlctor/tests/run/__init__.py
--rwxr-xr-x   0        0        0     1316 2023-03-27 13:17:31.238203 amlctor-0.0.1/amlctor/tests/src/templates/settings
--rwxr-xr-x   0        0        0        0 2023-03-22 06:44:08.843972 amlctor-0.0.1/amlctor/update/__init__.py
--rwxr-xr-x   0        0        0     3008 2023-04-22 14:28:00.659045 amlctor-0.0.1/amlctor/update/update.py
--rwxr-xr-x   0        0        0     3666 2023-04-12 16:51:57.228332 amlctor-0.0.1/amlctor/utils.py
--rw-r--r--   0        0        0      848 2023-04-29 11:49:45.799198 amlctor-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0     6398 2023-02-19 13:45:48.604585 amlctor-0.0.1/requirements.txt
--rw-r--r--   0        0        0     9757 1970-01-01 00:00:00.000000 amlctor-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0       73 2023-04-30 17:49:09.441825 amlctor-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1078 2023-04-26 11:53:55.773431 amlctor-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     9020 2023-04-24 10:36:05.672888 amlctor-0.0.2/README.md
+-rwxr-xr-x   0        0        0       55 2023-04-30 17:39:36.853186 amlctor-0.0.2/amlctor/__init__.py
+-rwxr-xr-x   0        0        0      171 2023-04-26 12:04:07.833727 amlctor-0.0.2/amlctor/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-02-25 04:17:23.449214 amlctor-0.0.2/amlctor/amlctor.py
+-rwxr-xr-x   0        0        0        0 2023-02-23 16:48:42.440743 amlctor-0.0.2/amlctor/apply/__init__.py
+-rwxr-xr-x   0        0        0     8848 2023-04-30 17:48:10.777762 amlctor-0.0.2/amlctor/apply/apply.py
+-rwxr-xr-x   0        0        0        0 2023-02-19 20:11:02.961852 amlctor-0.0.2/amlctor/confs/__init__.py
+-rwxr-xr-x   0        0        0      687 2023-04-28 18:20:16.796132 amlctor-0.0.2/amlctor/confs/configs.py
+-rwxr-xr-x   0        0        0     5055 2023-04-25 12:46:11.091783 amlctor-0.0.2/amlctor/core.py
+-rwxr-xr-x   0        0        0        0 2023-04-02 07:51:59.583621 amlctor-0.0.2/amlctor/denv/__init__.py
+-rwxr-xr-x   0        0        0     4302 2023-04-28 18:28:53.978801 amlctor-0.0.2/amlctor/denv/denv.py
+-rwxr-xr-x   0        0        0      803 2023-04-25 12:42:33.934318 amlctor-0.0.2/amlctor/denv/dot_env_loader.py
+-rwxr-xr-x   0        0        0     2591 2023-03-31 19:45:35.301488 amlctor-0.0.2/amlctor/exceptions.py
+-rwxr-xr-x   0        0        0        0 2023-02-23 16:48:40.988088 amlctor-0.0.2/amlctor/init/__init__.py
+-rwxr-xr-x   0        0        0     9252 2023-04-26 12:29:03.865986 amlctor-0.0.2/amlctor/init/args_handling.py
+-rwxr-xr-x   0        0        0     6578 2023-04-26 12:15:24.363525 amlctor-0.0.2/amlctor/init/init.py
+-rwxr-xr-x   0        0        0     2518 2023-04-28 15:07:38.962403 amlctor-0.0.2/amlctor/init/init_structure.py
+-rwxr-xr-x   0        0        0     4665 2023-04-25 12:43:48.131909 amlctor-0.0.2/amlctor/input.py
+-rwxr-xr-x   0        0        0        0 2023-02-25 04:18:40.776054 amlctor-0.0.2/amlctor/rename/__init__.py
+-rwxr-xr-x   0        0        0     3655 2023-04-23 09:56:52.168839 amlctor-0.0.2/amlctor/rename/rename.py
+-rwxr-xr-x   0        0        0        0 2023-02-23 16:48:38.940819 amlctor-0.0.2/amlctor/run/__init__.py
+-rwxr-xr-x   0        0        0     3606 2023-04-15 10:45:35.001519 amlctor-0.0.2/amlctor/run/run.py
+-rwxr-xr-x   0        0        0     1622 2023-04-26 12:16:29.679730 amlctor-0.0.2/amlctor/schemas.py
+-rwxr-xr-x   0        0        0        0 2023-02-19 14:56:55.871703 amlctor-0.0.2/amlctor/src/__init__.py
+-rwxr-xr-x   0        0        0      177 2023-04-11 18:59:17.691227 amlctor-0.0.2/amlctor/src/templates/apply/aml
+-rwxr-xr-x   0        0        0      483 2023-04-12 18:26:23.159935 amlctor-0.0.2/amlctor/src/templates/apply/data_loaders
+-rwxr-xr-x   0        0        0      543 2023-03-01 17:56:39.337816 amlctor-0.0.2/amlctor/src/templates/init/conda_dependencies
+-rwxr-xr-x   0        0        0      443 2023-04-22 05:55:24.837867 amlctor-0.0.2/amlctor/src/templates/init/dot_amlignore
+-rwxr-xr-x   0        0        0      274 2023-04-22 08:11:36.650858 amlctor-0.0.2/amlctor/src/templates/init/dot_env
+-rwxr-xr-x   0        0        0      776 2023-04-09 12:13:41.742028 amlctor-0.0.2/amlctor/src/templates/init/env_vars
+-rwxr-xr-x   0        0        0     1442 2023-04-12 19:12:37.227543 amlctor-0.0.2/amlctor/src/templates/init/settings
+-rwxr-xr-x   0        0        0        0 2023-02-19 14:57:07.938361 amlctor-0.0.2/amlctor/tests/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-21 17:33:46.575063 amlctor-0.0.2/amlctor/tests/apply/__init__.py
+-rwxr-xr-x   0        0        0     2597 2023-04-26 12:18:34.780132 amlctor-0.0.2/amlctor/tests/apply/test_apply_path.py
+-rwxr-xr-x   0        0        0        0 2023-02-21 17:33:39.745273 amlctor-0.0.2/amlctor/tests/core/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-21 17:33:31.748011 amlctor-0.0.2/amlctor/tests/init/__init__.py
+-rwxr-xr-x   0        0        0     1477 2023-04-26 12:19:07.456238 amlctor-0.0.2/amlctor/tests/init/test_env_bank.py
+-rwxr-xr-x   0        0        0        0 2023-02-21 17:33:54.684018 amlctor-0.0.2/amlctor/tests/run/__init__.py
+-rwxr-xr-x   0        0        0     1316 2023-03-27 13:17:31.238203 amlctor-0.0.2/amlctor/tests/src/templates/settings
+-rwxr-xr-x   0        0        0        0 2023-03-22 06:44:08.843972 amlctor-0.0.2/amlctor/update/__init__.py
+-rwxr-xr-x   0        0        0     3008 2023-04-22 14:28:00.659045 amlctor-0.0.2/amlctor/update/update.py
+-rwxr-xr-x   0        0        0     3666 2023-04-12 16:51:57.228332 amlctor-0.0.2/amlctor/utils.py
+-rw-r--r--   0        0        0      848 2023-04-29 11:49:45.799198 amlctor-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0     6398 2023-02-19 13:45:48.604585 amlctor-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     9757 1970-01-01 00:00:00.000000 amlctor-0.0.2/PKG-INFO
```

### Comparing `amlctor-0.0.1/LICENSE` & `amlctor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/README.md` & `amlctor-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/apply/apply.py` & `amlctor-0.0.2/amlctor/apply/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,50 +30,54 @@
         for step in self.settingspy['STEPS']:
             step_path = self.path / step.name
             step_path.mkdir(mode=0o770, exist_ok=True)                 # create dir for pipe step
             self.create_files(step, step_path)          # create files inside step dir
 
 
     def create_files(self, step: StepSchema, step_path: Path):
-        script_name = self.settingspy['SCRIPT_MODULE_NAME']               # create script.py
-        if not script_name.endswith('.py'):
-                script_name = script_name + '.py'
+        """ creates modules """
+        # create script.py
+        script_name = self.settingspy['SCRIPT_MODULE_NAME']
+        script_name = self.ext(script_name, True) 
         if (step_path / script_name).exists():
             response = input(f"file '{(step_path / script_name)}' already exists. Type- overwrite: o; skip: s; cancel: c: ")
             if response.lower().strip() in ('o', 'overwrite'):
                 (step_path / script_name).touch(exist_ok=True)
             elif response.lower().strip() in ('s', 'skip'):
                 pass
 
             elif response.lower().strip() in ('c', 'cancel'):
                 raise SystemExit("Cancelled.")
             else:
                 raise ValueError(f"Incorrect answer '{response}'. It must be one of [o, s, c]")
+        else:
+            (step_path / script_name).touch(exist_ok=True)
             
         # create data_loader.py
         dataloader_name = self.settingspy['DATALOADER_MODULE_NAME'] 
         dataloader_name = self.ext(dataloader_name, True)                 # add .py
         content, keys = StructureApply.create_dataloader_content(step=step)
         
         with (step_path / dataloader_name).open(mode='w+') as dataloader:
             dataloader.write(content)
+
         # create aml.py
         aml_name = self.settingspy['AML_MODULE_NAME']
         aml_name = self.ext(aml_name, True)
         with (step_path / aml_name).open(mode='w+') as aml:
             aml_t = StructureApply.jinva_env.get_template('aml')
             dataloader_name = self.ext(dataloader_name, yes=False)     # no extention for importing in template
             content = aml_t.render(dataloader_name=dataloader_name, keys=keys)
             aml.write(content)
 
 
     
     def ext(self, filename: str, yes=True):
         """ 
-            Returns filename with or without '.py extention'.
+            Returns filename with or without '.py` extention.
             yes: if True then add '.py', else drop out.
         """
         filename = filename.strip()     # just 4 fun
 
         if filename.endswith('.py'): # has extention
             if yes is True:
                 return filename
```

### Comparing `amlctor-0.0.1/amlctor/confs/configs.py` & `amlctor-0.0.2/amlctor/confs/configs.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/core.py` & `amlctor-0.0.2/amlctor/core.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/denv/denv.py` & `amlctor-0.0.2/amlctor/denv/denv.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/denv/dot_env_loader.py` & `amlctor-0.0.2/amlctor/denv/dot_env_loader.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/exceptions.py` & `amlctor-0.0.2/amlctor/exceptions.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/init/args_handling.py` & `amlctor-0.0.2/amlctor/init/args_handling.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/init/init.py` & `amlctor-0.0.2/amlctor/init/init.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/init/init_structure.py` & `amlctor-0.0.2/amlctor/init/init_structure.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/input.py` & `amlctor-0.0.2/amlctor/input.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/rename/rename.py` & `amlctor-0.0.2/amlctor/rename/rename.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/run/run.py` & `amlctor-0.0.2/amlctor/run/run.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/schemas.py` & `amlctor-0.0.2/amlctor/schemas.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/src/templates/init/conda_dependencies` & `amlctor-0.0.2/amlctor/src/templates/init/conda_dependencies`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/src/templates/init/env_vars` & `amlctor-0.0.2/amlctor/src/templates/init/env_vars`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/src/templates/init/settings` & `amlctor-0.0.2/amlctor/src/templates/init/settings`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/tests/apply/test_apply_path.py` & `amlctor-0.0.2/amlctor/tests/apply/test_apply_path.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/tests/init/test_env_bank.py` & `amlctor-0.0.2/amlctor/tests/init/test_env_bank.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/tests/src/templates/settings` & `amlctor-0.0.2/amlctor/tests/src/templates/settings`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/update/update.py` & `amlctor-0.0.2/amlctor/update/update.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/amlctor/utils.py` & `amlctor-0.0.2/amlctor/utils.py`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/pyproject.toml` & `amlctor-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/requirements.txt` & `amlctor-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `amlctor-0.0.1/PKG-INFO` & `amlctor-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amlctor
-Version: 0.0.1
+Version: 0.0.2
 Summary: AML Pipeline Constructor 
 Keywords: azure,machine leaning,aml,pipeline
 Author-email: Aziz Nadirov <aziznadirov@yahoo.com>
 Requires-Python: >=3.9,<3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

