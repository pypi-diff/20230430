# Comparing `tmp/appopener-1.6.tar.gz` & `tmp/appopener-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appopener-1.6.tar", last modified: Sun Jan 15 19:09:48 2023, max compression
+gzip compressed data, was "appopener-1.7.tar", last modified: Sun Apr 30 11:28:59 2023, max compression
```

## Comparing `appopener-1.6.tar` & `appopener-1.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-15 19:09:48.145351 appopener-1.6/
-drwxrwxrwx   0        0        0        0 2023-01-15 19:09:47.973502 appopener-1.6/AppOpener/
--rw-rw-rw-   0        0        0     5067 2023-01-14 14:54:53.000000 appopener-1.6/AppOpener/__init__.py
--rw-rw-rw-   0        0        0       66 2022-08-03 10:17:53.000000 appopener-1.6/AppOpener/__main__.py
--rw-rw-rw-   0        0        0     2663 2023-01-14 05:53:00.000000 appopener-1.6/AppOpener/check.py
--rw-rw-rw-   0        0        0      848 2022-12-24 19:43:57.000000 appopener-1.6/AppOpener/commands.py
--rw-rw-rw-   0        0        0     7048 2023-01-14 05:35:47.000000 appopener-1.6/AppOpener/features.py
--rw-rw-rw-   0        0        0     7619 2023-01-14 05:29:01.000000 appopener-1.6/AppOpener/update_list.py
--rw-rw-rw-   0        0        0     1071 2022-12-31 12:03:22.000000 appopener-1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     3917 2023-01-15 19:09:48.129740 appopener-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2497 2023-01-10 08:33:43.000000 appopener-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-01-15 19:09:48.114102 appopener-1.6/appopener.egg-info/
--rw-rw-rw-   0        0        0     3917 2023-01-15 19:09:45.000000 appopener-1.6/appopener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-01-15 19:09:47.000000 appopener-1.6/appopener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-15 19:09:45.000000 appopener-1.6/appopener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-01-15 19:09:45.000000 appopener-1.6/appopener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-15 19:09:46.000000 appopener-1.6/appopener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-15 19:09:48.145351 appopener-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1217 2022-12-31 15:57:25.000000 appopener-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:28:59.884106 appopener-1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:28:59.884106 appopener-1.7/AppOpener/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-30 11:28:50.000000 appopener-1.7/AppOpener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-30 11:28:50.000000 appopener-1.7/AppOpener/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-30 11:28:50.000000 appopener-1.7/AppOpener/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-30 11:28:50.000000 appopener-1.7/AppOpener/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-04-30 11:28:50.000000 appopener-1.7/AppOpener/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 11:28:50.000000 appopener-1.7/AppOpener/old_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-30 11:28:50.000000 appopener-1.7/AppOpener/update_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-30 11:28:50.000000 appopener-1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-30 11:28:59.884106 appopener-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-30 11:28:50.000000 appopener-1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:28:59.884106 appopener-1.7/appopener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-30 11:28:59.000000 appopener-1.7/appopener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-30 11:28:59.000000 appopener-1.7/appopener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:28:59.000000 appopener-1.7/appopener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-30 11:28:59.000000 appopener-1.7/appopener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 11:28:59.000000 appopener-1.7/appopener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:28:59.884106 appopener-1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-30 11:28:50.000000 appopener-1.7/setup.py
```

### Comparing `appopener-1.6/AppOpener/__init__.py` & `appopener-1.7/AppOpener/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.6"
+__version__ = "1.7"
 from . import check, update_list, commands, features
 import os, re
 
 check.check_os()
 # Checking if required files exists or not
 check.check_json()
 check.app_names()
@@ -44,15 +44,15 @@
 def run(self, output=True):
     print()
     print("'RUN' FUNCTION IS REPLACED BY 'OPEN' FUNCTION")
     print("TRY USING 'OPEN(app_name)'")
     print()
 
 # Open application (Regex implemented)
-def open(self, output=True, match_closest=False):
+def open(self, output=True, match_closest=False, throw_error=False):
     '''
     #### `open` is the function which is used to open applications.
     Examples:
     1: open("whatsapp")
     2: open("whatsapp, telegram")
     3: open("calcu", match_closest=True)
     4: open("whatsapp, telegram", output=False)
@@ -96,40 +96,39 @@
         update_list.pre_change()
         update_list.modify()
     elif val == "mklist":
         mklist(output=output)
     elif "find " in val:
         print()
         val2 = val.replace("find ","")
+        empty_list = []
         if "," in val2:
             splited = val2.split(",")
-            for i in splited:
-                j = i.strip()
-                if j != "":
-                    features.find_apps(j)
+            empty_list.extend(splited)
         else:
-            features.find_apps(val2)
+            empty_list.append(val2)
+        features.find_apps(app_names=empty_list)
         print()
     elif val == "log -c" or val == "log":
         print()
         val2 = val.replace("log -","")
         features.change_log(val)
         print()
     else:
         if "," in val:
             splited = val.split(",")
             for i in splited:
                 j = i.strip()
                 if j != "":
-                    features.open_things(j, output=output, match_closest=match_closest)
+                    features.open_things(j, output=output, match_closest=match_closest, throw_error=throw_error)
         else:
-           features.open_things(val, output=output, match_closest=match_closest)
+           features.open_things(val, output=output, match_closest=match_closest, throw_error=throw_error)
 
 # Close any application by just its name :)
-def close(self, output=True, match_closest=False):
+def close(self, output=True, match_closest=False, throw_error=False):
     '''
     #### `close` is the function which is used to close applications.
     Examples:
     1: close("whatsapp")
     2: close("whatsapp, telegram")
     3: close("calcu", match_closest=True)
     4: close("whatsapp, telegram", output=False)
@@ -143,11 +142,11 @@
     inp = (self).lower()
     val=(re.compile(r'[^a-zA-Z-^0-9?,>&+.]').sub(" ",inp)).strip()
     if "," in val:
         splited = val.split(",")
         for i in splited:
             j = i.strip()
             if j != "":
-                features.close_things(j, output=output, match_closest=match_closest)
+                features.close_things(j, output=output, match_closest=match_closest, throw_error=throw_error)
     else:
-        features.close_things(val, output=output, match_closest=match_closest)
+        features.close_things(val, output=output, match_closest=match_closest, throw_error=throw_error)
```

### Comparing `appopener-1.6/AppOpener/check.py` & `appopener-1.7/AppOpener/check.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,78 @@
-import os, json, re, sys, subprocess
-from . import update_list
-
-# check what os the library is running on
-def check_os():
-    os_name = os.name
-    if os_name != "nt":
-        print("Exception error: AppOpener only works on windows.")
-        exit()
-
-# Get path of working directory
-def get_path():
-    if getattr(sys, 'frozen', False):
-        main_path = os.path.dirname(sys.executable)
-        return main_path
-    elif __file__:
-        main_path = os.path.dirname(__file__)
-        return main_path
-
-main_path = os.path.join(get_path(), "Data")
-
-# Status of existance of required files
-check_data = os.path.isdir(main_path)
-check_json_list = os.path.exists(os.path.join(main_path,"data.json"))
-check_app_names = os.path.exists(os.path.join(main_path,"app_names.json"))
-
-# Convert text file to json format file
-def setup_files():
-    with open((os.path.join(main_path,"data.json")),"r") as data_file:
-        data_duplicate = json.load(data_file)
-        modified_data = {}
-        for key, value in data_duplicate.items():
-            is_digit = key[:1].isdigit()
-            if is_digit == False:
-                val=(re.compile(r'[^a-z-&]')).sub(" ",key)
-                final_app_name = re.sub(' +', ' ', val).strip()
-                modified_data[final_app_name] = value
-            if is_digit == True:
-                val=(re.compile(r'[^a-z-&^0-9]')).sub(" ",key)
-                final_app_name = re.sub(' +', ' ', val).strip()
-                modified_data[final_app_name] = value
-        with open((os.path.join(main_path,"data.json")),"w") as f:
-            json.dump(modified_data, f, indent=4)
-
-def create_file(print_text=True):
-    if check_data == False:
-        os.mkdir(main_path)
-        os.system(("attrib +h "+main_path))
-    if print_text:
+import os, json, re, sys, subprocess
+from . import update_list
+
+# check what os the library is running on
+def check_os():
+    os_name = os.name
+    if os_name != "nt":
+        raise Exception("AppOpener only works on Windows.")
+        exit()
+
+# Get path of working directory
+def get_path():
+    if getattr(sys, 'frozen', False):
+        main_path = os.path.dirname(sys.executable)
+        return main_path
+    elif __file__:
+        main_path = os.path.dirname(__file__)
+        return main_path
+
+main_path = os.path.join(get_path(), "Data")
+
+# Status of existance of required files
+check_data = os.path.isdir(main_path)
+check_json_list = os.path.exists(os.path.join(main_path,"data.json"))
+check_app_names = os.path.exists(os.path.join(main_path,"app_names.json"))
+
+# Convert text file to json format file
+def setup_files():
+    with open((os.path.join(main_path,"data.json")),"r") as data_file:
+        data_duplicate = json.load(data_file)
+        modified_data = {}
+        for key, value in data_duplicate.items():
+            is_digit = key[:1].isdigit()
+            if is_digit == False:
+                val=(re.compile(r'[^a-z-&]')).sub(" ",key)
+                final_app_name = re.sub(' +', ' ', val).strip()
+                modified_data[final_app_name] = value
+            if is_digit == True:
+                val=(re.compile(r'[^a-z-&^0-9]')).sub(" ",key)
+                final_app_name = re.sub(' +', ' ', val).strip()
+                modified_data[final_app_name] = value
+        with open((os.path.join(main_path,"data.json")),"w") as f:
+            json.dump(modified_data, f, indent=4)
+
+def create_file(print_text=True):
+    if check_data == False:
+        os.mkdir(main_path)
+        os.system(("attrib +h "+main_path))
+    if print_text:
         print("LOADING APPS... (JUST ONCE)")
-    cmd = 'powershell -ExecutionPolicy Bypass "Get-StartApps|convertto-json"'
-    result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, encoding='utf-8')
-    apps = json.loads(result.stdout)
-    names = {}
-    for each in apps:
-        names.update({each['Name'].lower():each['AppID']})
-    with open((os.path.join(main_path,"data.json")),"w") as outfile:
-        json.dump(names,outfile,indent = 4)
-    setup_files()
-
-def check_json():
-    if check_json_list == (False):
-        create_file()
-
-# Make seperate file for appnames (to perform various features)
-def app_names():
-    if check_app_names == (False):
-        update_list.check_app_names()
-    update_list.check_new_name()
-    update_list.pre_change()
-    update_list.modify()
+    cmd = 'powershell -ExecutionPolicy Bypass "Get-StartApps|convertto-json"'
+    try:
+        result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, encoding='utf-8')
+        # Exception if the result is Empty
+        # if not result.stdout:
+        #     raise Exception("No output returned by the command")
+        apps = json.loads(result.stdout)
+    except:
+        from . import old_style
+        return
+    names = {}
+    for each in apps:
+        names.update({each['Name'].lower():each['AppID']})
+    with open((os.path.join(main_path,"data.json")),"w") as outfile:
+        json.dump(names,outfile,indent = 4)
+    setup_files()
+
+def check_json():
+    if check_json_list == (False):
+        create_file()
+
+# Make seperate file for appnames (to perform various features)
+def app_names():
+    if check_app_names == (False):
+        update_list.check_app_names()
+    update_list.check_new_name()
+    update_list.pre_change()
+    update_list.modify()
```

### Comparing `appopener-1.6/AppOpener/commands.py` & `appopener-1.7/AppOpener/commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-def commands():
-    data = [['KEY', 'USE'],
-            ['(?)','DOCUMENTATION'],
-            ['(VERSION)','SEE APPOPENER VERSION'],
-            ['(LS)','LIST OF APPLICATIONS'],
-            ['(FIND XYZ)', "FIND APPLICATION"],
-            ['(UPDATE -M)','UPDATE APPNAMES MANUALLY'],
-            ['(UPDATE)','LOAD NEW DATA'],
-            ['(OLD > NEW)','UPDATE APP VIA CLI'],
-            ['(DEFAULT)','RESTORES DEFAULT APPNAMES'],
-            ['(LOG)','SEE CHANGED PETNAME(s)'],
-            ['(CLS)','CLEARS SCREEN'],
-            ['(Q)','EXIT PROGRAM']
-            ]
-    dash = '-' * 35
-    for i in range(len(data)):
-        if i == 0:
-            print(dash)
-            print('{:<15s}{:^15s}'.format(data[i][0],data[i][1]))
-            print(dash)
-        else:
+def commands():
+    data = [['KEY', 'USE'],
+            ['(?)','DOCUMENTATION'],
+            ['(VERSION)','SEE APPOPENER VERSION'],
+            ['(LS)','LIST OF APPLICATIONS'],
+            ['(FIND XYZ)', "FIND APPLICATION"],
+            ['(UPDATE -M)','UPDATE APPNAMES MANUALLY'],
+            ['(UPDATE)','LOAD NEW DATA'],
+            ['(OLD > NEW)','UPDATE APP VIA CLI'],
+            ['(DEFAULT)','RESTORES DEFAULT APPNAMES'],
+            ['(LOG)','SEE CHANGED PETNAME(s)'],
+            ['(CLS)','CLEARS SCREEN']
+            ]
+    dash = '-' * 35
+    for i in range(len(data)):
+        if i == 0:
+            print(dash)
+            print('{:<15s}{:^15s}'.format(data[i][0],data[i][1]))
+            print(dash)
+        else:
             print('{:<15s}{:^12s}'.format(data[i][0],data[i][1]))
```

### Comparing `appopener-1.6/AppOpener/update_list.py` & `appopener-1.7/AppOpener/update_list.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-import os, json, sys
+import os, json, sys
 from . import check
-
-# Get path of working directory
-def get_path():
-    if getattr(sys, 'frozen', False):
-        main_path = os.path.dirname(sys.executable)
-        return main_path
-    elif __file__:
-        main_path = os.path.dirname(__file__)
-        return main_path
-
-main_path = os.path.join(get_path(),"Data")
-
-# RENAMING PETNAME IN APP_NAMES FILE
-def do_changes(app, petname):
-    with open(os.path.join(main_path, "app_names.json"), "r") as file:
-        data = json.load(file)
-    data[app] = petname.lower()
-    with open(os.path.join(main_path, "app_names.json"), "w") as file1:
-        json.dump(data, file1, indent=4)
-
-# CHANGE PRE / SEC NAME IN DATA FILE
-def pre_change():
-    with open((os.path.join(main_path,"app_names_temp.json")),"r") as file, open((os.path.join(main_path,"data.json")),"r") as data_file_read:
-        data_read = json.load(data_file_read)
-        data_file = json.load(file)
-        keys_file = list(data_file.keys())
-        values_file = list(data_file.values())
-        for app2 in keys_file:
-            if data_file[app2] != "":
-                position = keys_file.index(app2)
-                app=values_file[position]
-                try:
-                    data_read[app] = data_read.pop(app2)
-                except:
-                    pass
-    with open((os.path.join(main_path,"data.json")),"w") as f:
-        json.dump(data_read,f,indent=4)
-
-# CHANGES IN MAIN DATA FILE (PETNAME)
-def change_in_data(app, petname):
-    with open(os.path.join(main_path, "data.json"), "r") as file:
-        data = json.load(file)
-    data[petname] = data.pop(app, None)
-    with open(os.path.join(main_path, "data.json"), "w") as file1:
-        json.dump(data, file1, indent=4)
-
-# REVIEW CHANGES IN APP_NAMES FILE
-def modify():
-    with open((os.path.join(main_path,"app_names.json")),"r") as file:
-        data = json.load(file)
-        keys = list(data.keys())
-        values = list(data.values())
-        for petname in values:
-            if petname != "":
-                position = values.index(petname)
-                app = keys[position]
-                #print(app,petname)
-                change_in_data(app,petname)
-
-# CHANGE ALL PETNAMES TO DEFAULT APP NAMES
-def default(output=True):
-    if output:
-        print("RESTORING DEFAULT APP NAMES")
-    file1 = open((os.path.join(main_path,"app_names.json")),"r")
-    data1 = json.load(file1)
-    keys = list(data1.keys())
-    values = list(data1.values())
-    file2 = open((os.path.join(main_path,"app_names.json")),"r")
-    data2 = json.load(file2)
-    for petname in values:
-        if petname != "":
-            position = values.index(petname)
-            app=keys[position]
-            #print(app+" "+petname)
-            change = {app:app}
-            data2.update(change)
-    file3 = open((os.path.join(main_path,"app_names.json")),"w")
-    json.dump(data2,file3,indent=4)
-    if output:
-        print("DONE.")
-
-# EXECUTE CHANGES IN DATA FILE
-def check_new_name():
-    file = open((os.path.join(main_path,"app_names.json")),"r")
-    app_temp = open((os.path.join(main_path,"app_names_temp.json")),"r")
-    data_temp = json.load(app_temp)
-    data = json.load(file)
-    keys = list(data.keys())
-    values = list(data.values())
-    for app2 in values:
-        if app2 != "":
-            position = values.index(app2)
-            app = keys[position]
-            change = {app2:app}
-            data_temp.update(change)
-    with open((os.path.join(main_path,"app_names_temp.json")),"a+") as f:
-        g = open((os.path.join(main_path,"app_names_temp.json")),"r+")
-        g.truncate(0)
-        json.dump(data_temp,f,indent=4)
-
-# DEPENDENCY OF (3)
-def edit_things_cli(count,current_name,petname):
-    with open((os.path.join(main_path,"app_names.json")),"r") as app_file:
-        data = json.load(app_file)
-    for app_name in data:
-        if current_name == app_name:
-            change = {current_name:petname}
-            data.update(change)
-            with open((os.path.join(main_path,"app_names.json")),"a+") as f:
-                g = open((os.path.join(main_path,"app_names.json")),"r+")
-                g.truncate(0)
-                json.dump(data,f,indent=4)
-                if count == None:
-                    count = 1
-                print(str(count)+". "+current_name.upper()+" IS NOW "+petname.upper())
-
-# SORT MULTIPLE CHANGES OF APPS VIA CLI - 3
-def do_changes_cli(self):
-    if "," in self:
-        count = 0
-        splited=self.split(",")
-        for i in splited:
-            j = i.strip()
-            if j != "":
-                count += 1
-                split2 = j.split(">")
-                current_name = (split2[0]).strip()
-                petname = (split2[1]).strip()
-                edit_things_cli(count,current_name,petname)
-    else:
-        splited = self.split(">")
-        # print(splited)
-        current_name = (splited[0]).strip()
-        petname = (splited[1]).strip()
-        edit_things_cli(1,current_name,petname)
-
-# FETCH ALL NEW APPS
-def update(output=True):
-    if output:
-        print("FETCHING ALL NEW APPS (if any)")
-    check.create_file(print_text=False)
-    check.setup_files()
-    if output:
-        print("WRITING APP NAMES")
-    with open((os.path.join(main_path,"app_names.json")),"r") as old_AF:
-        old = json.load(old_AF)
-    with open((os.path.join(main_path,"app_names_temp.json")),"w+") as temp_af:
-        json.dump(old,temp_af,indent=4)
-    dictionary ={}
-    json_object = json.dumps(dictionary, indent = 4)
-    with open((os.path.join(main_path,"app_names.json")),"w") as outfile:
-        outfile.write(json_object)
-    with open((os.path.join(main_path,"data.json")),"r") as app_file:
-        data1 = json.load(app_file)
-    with open((os.path.join(main_path, "app_names.json")),"r") as file:
-        data = json.load(file)
-    for app_name in data1:
-        change = {app_name:""}
-        data.update(change)
-        with open((os.path.join(main_path,"app_names.json")),"a+") as f:
-            g = open((os.path.join(main_path,"app_names.json")),"r+")
-            g.truncate(0)
-            json.dump(data,f,indent=4)
-    with open((os.path.join(main_path,"app_names_temp.json")),"r") as file:
-        data = json.load(file)
-        values = list(data.values())
-        keys = list(data.keys())
-    for petname in values:
-        if petname != "":
-            position = values.index(petname)
-            app_old=keys[position]
-            # print(str(app_old)+" changed to "+str(petname))
-            do_changes(app_old,petname)
-    check_new_name()
-    if output:
-        print("LIST UPDATED.")
-
-# SETUP FILES - 1
-def check_app_names():
-    print()
-    print("PREPARING FOR INPUTS (JUST ONCE)")
-    empty_dictionary ={}
-    with open((os.path.join(main_path,"app_names.json")),"w") as outfile:
-        json.dump(empty_dictionary, outfile)
-    with open((os.path.join(main_path,"data.json")),"r") as app_file:
-        data = json.load(app_file)
-        keys = data.keys()
-        dictionary = {}
-    for app_name in keys:
-        change = {app_name:""}
-        dictionary.update(change)
-        with open((os.path.join(main_path,"app_names.json")),"a+") as f:
-            g = open((os.path.join(main_path,"app_names.json")),"r+")
-            g.truncate(0)
-            json.dump(dictionary,f,indent=4)
-    with open((os.path.join(main_path,"app_names_temp.json")),"w") as outfile:
-        json.dump(empty_dictionary, outfile)
+
+# Get path of working directory
+def get_path():
+    if getattr(sys, 'frozen', False):
+        main_path = os.path.dirname(sys.executable)
+        return main_path
+    elif __file__:
+        main_path = os.path.dirname(__file__)
+        return main_path
+
+main_path = os.path.join(get_path(),"Data")
+
+# RENAMING PETNAME IN APP_NAMES FILE
+def do_changes(app, petname):
+    with open(os.path.join(main_path, "app_names.json"), "r") as file:
+        data = json.load(file)
+    data[app] = petname.lower()
+    with open(os.path.join(main_path, "app_names.json"), "w") as file1:
+        json.dump(data, file1, indent=4)
+
+# CHANGE PRE / SEC NAME IN DATA FILE
+def pre_change():
+    with open((os.path.join(main_path,"app_names_temp.json")),"r") as file, open((os.path.join(main_path,"data.json")),"r") as data_file_read:
+        data_read = json.load(data_file_read)
+        data_file = json.load(file)
+        keys_file = list(data_file.keys())
+        values_file = list(data_file.values())
+        for app2 in keys_file:
+            if data_file[app2] != "":
+                position = keys_file.index(app2)
+                app=values_file[position]
+                try:
+                    data_read[app] = data_read.pop(app2)
+                except:
+                    pass
+    with open((os.path.join(main_path,"data.json")),"w") as f:
+        json.dump(data_read,f,indent=4)
+
+# CHANGES IN MAIN DATA FILE (PETNAME)
+def change_in_data(app, petname):
+    with open(os.path.join(main_path, "data.json"), "r") as file:
+        data = json.load(file)
+    data[petname] = data.pop(app, None)
+    with open(os.path.join(main_path, "data.json"), "w") as file1:
+        json.dump(data, file1, indent=4)
+
+# REVIEW CHANGES IN APP_NAMES FILE
+def modify():
+    with open((os.path.join(main_path,"app_names.json")),"r") as file:
+        data = json.load(file)
+        keys = list(data.keys())
+        values = list(data.values())
+        for petname in values:
+            if petname != "":
+                position = values.index(petname)
+                app = keys[position]
+                #print(app,petname)
+                change_in_data(app,petname)
+
+# CHANGE ALL PETNAMES TO DEFAULT APP NAMES
+def default(output=True):
+    if output:
+        print("RESTORING DEFAULT APP NAMES")
+    file1 = open((os.path.join(main_path,"app_names.json")),"r")
+    data1 = json.load(file1)
+    keys = list(data1.keys())
+    values = list(data1.values())
+    file2 = open((os.path.join(main_path,"app_names.json")),"r")
+    data2 = json.load(file2)
+    for petname in values:
+        if petname != "":
+            position = values.index(petname)
+            app=keys[position]
+            #print(app+" "+petname)
+            change = {app:app}
+            data2.update(change)
+    file3 = open((os.path.join(main_path,"app_names.json")),"w")
+    json.dump(data2,file3,indent=4)
+    if output:
+        print("DONE.")
+
+# EXECUTE CHANGES IN DATA FILE
+def check_new_name():
+    file = open((os.path.join(main_path,"app_names.json")),"r")
+    app_temp = open((os.path.join(main_path,"app_names_temp.json")),"r")
+    data_temp = json.load(app_temp)
+    data = json.load(file)
+    keys = list(data.keys())
+    values = list(data.values())
+    for app2 in values:
+        if app2 != "":
+            position = values.index(app2)
+            app = keys[position]
+            change = {app2:app}
+            data_temp.update(change)
+    with open((os.path.join(main_path,"app_names_temp.json")),"a+") as f:
+        g = open((os.path.join(main_path,"app_names_temp.json")),"r+")
+        g.truncate(0)
+        json.dump(data_temp,f,indent=4)
+
+# DEPENDENCY OF (3)
+def edit_things_cli(count,current_name,petname):
+    with open((os.path.join(main_path,"app_names.json")),"r") as app_file:
+        data = json.load(app_file)
+    for app_name in data:
+        if current_name == app_name:
+            change = {current_name:petname}
+            data.update(change)
+            with open((os.path.join(main_path,"app_names.json")),"a+") as f:
+                g = open((os.path.join(main_path,"app_names.json")),"r+")
+                g.truncate(0)
+                json.dump(data,f,indent=4)
+                if count == None:
+                    count = 1
+                print(str(count)+". "+current_name.upper()+" IS NOW "+petname.upper())
+
+# SORT MULTIPLE CHANGES OF APPS VIA CLI - 3
+def do_changes_cli(self):
+    if "," in self:
+        count = 0
+        splited=self.split(",")
+        for i in splited:
+            j = i.strip()
+            if j != "":
+                count += 1
+                split2 = j.split(">")
+                current_name = (split2[0]).strip()
+                petname = (split2[1]).strip()
+                edit_things_cli(count,current_name,petname)
+    else:
+        splited = self.split(">")
+        # print(splited)
+        current_name = (splited[0]).strip()
+        petname = (splited[1]).strip()
+        edit_things_cli(1,current_name,petname)
+
+# FETCH ALL NEW APPS
+def update(output=True):
+    if output:
+        print("FETCHING ALL NEW APPS (if any)")
+    check.create_file(print_text=False)
+    check.setup_files()
+    if output:
+        print("WRITING APP NAMES")
+    with open((os.path.join(main_path,"app_names.json")),"r") as old_AF:
+        old = json.load(old_AF)
+    with open((os.path.join(main_path,"app_names_temp.json")),"w+") as temp_af:
+        json.dump(old,temp_af,indent=4)
+    dictionary ={}
+    json_object = json.dumps(dictionary, indent = 4)
+    with open((os.path.join(main_path,"app_names.json")),"w") as outfile:
+        outfile.write(json_object)
+    with open((os.path.join(main_path,"data.json")),"r") as app_file:
+        data1 = json.load(app_file)
+    with open((os.path.join(main_path, "app_names.json")),"r") as file:
+        data = json.load(file)
+    for app_name in data1:
+        change = {app_name:""}
+        data.update(change)
+        with open((os.path.join(main_path,"app_names.json")),"a+") as f:
+            g = open((os.path.join(main_path,"app_names.json")),"r+")
+            g.truncate(0)
+            json.dump(data,f,indent=4)
+    with open((os.path.join(main_path,"app_names_temp.json")),"r") as file:
+        data = json.load(file)
+        values = list(data.values())
+        keys = list(data.keys())
+    for petname in values:
+        if petname != "":
+            position = values.index(petname)
+            app_old=keys[position]
+            # print(str(app_old)+" changed to "+str(petname))
+            do_changes(app_old,petname)
+    check_new_name()
+    if output:
+        print("LIST UPDATED.")
+
+# SETUP FILES - 1
+def check_app_names():
+    print()
+    print("PREPARING FOR INPUTS (JUST ONCE)")
+    empty_dictionary ={}
+    with open((os.path.join(main_path,"app_names.json")),"w") as outfile:
+        json.dump(empty_dictionary, outfile)
+    with open((os.path.join(main_path,"data.json")),"r") as app_file:
+        data = json.load(app_file)
+        keys = data.keys()
+        dictionary = {}
+    for app_name in keys:
+        change = {app_name:""}
+        dictionary.update(change)
+        with open((os.path.join(main_path,"app_names.json")),"a+") as f:
+            g = open((os.path.join(main_path,"app_names.json")),"r+")
+            g.truncate(0)
+            json.dump(dictionary,f,indent=4)
+    with open((os.path.join(main_path,"app_names_temp.json")),"w") as outfile:
+        json.dump(empty_dictionary, outfile)
```

### Comparing `appopener-1.6/LICENSE.txt` & `appopener-1.7/LICENSE.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2023 LABS CREATION
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Copyright © 2023 LABS CREATION
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `appopener-1.6/PKG-INFO` & `appopener-1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,105 @@
-Metadata-Version: 2.1
-Name: appopener
-Version: 1.6
-Summary: Open/Close any application by it's name.
-Home-page: https://github.com/athrvvvv/AppOpener/tree/module
-Download-URL: https://pypi.python.org/pypi/AppOpener
-Author: Athrv Chaulkar
-Author-email: athrvchaulkar@gmail.com
-Maintainer: athrvvvv
-Maintainer-email: athrvchaulkar@gmail.com
-License: MIT
-Project-URL: Documentation, https://appopener.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/athrvvvv/AppOpener/tree/module
-Project-URL: Tracker, https://github.com/athrvvvv/AppOpener/issues
-Keywords: appopener,open apps,App Ids,automation,close apps
-Platform: Windows 10
-Platform: Windows 8.1
-Platform: Windows 11
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-## AppOpener 🔓
-
-AppOpener is the python library to **open/close** any application **without knowing it's absoulute path**. The library works by making use of App Name and App Id.
-
-Library works on python version 3.5 or above python version 3.5+
-
-[![PyPI Downloads](https://img.shields.io/pypi/dm/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/status/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/v/AppOpener?label=AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![Windows Only](https://img.shields.io/badge/platform-windows-blue.svg)](https://shields.io/)
-
-Visit official documentation of AppOpener [here](https://AppOpener.readthedocs.io/en/latest/).
-
-The latest development version is always available at the [Github](https://github.com/athrvvvv/AppOpener) repository.
-
-All notable changes made to the module, will be documented [here](https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md).
-
----
-
-> ### Features:
-
-1. Open applications
-2. Close applicatons
-3. Create list of Apps & Ids
-
----
-
-### Integrating AppOpener
-
-![](https://github.com/athrvvvv/AppOpener/blob/module/docs/img/output.gif)
-
-See [Examples](https://github.com/athrvvvv/AppOpener/tree/module/Examples) for more.
----
-
-> ### Install Package 📦
-
-```
-pip install AppOpener
-```
-
-> ### Quick start ⚡
-
-``` python
-from AppOpener import open, close ,mklist, give_appnames
-open("telegram, whatsapp") # Open telegram & whatsapp
-close("telgrm", match_closest=True) # Closes telegram as "telgrm" is closest to "telegram"
-mklist(name="app_data.json") # Create list of Apps & Ids
-appnames = give_appnames() # Save appnames as dictionary
-```
-
----
-> ### Building package 🔨
-
-```
-git clone https://github.com/athrvvvv/AppOpener.git
-cd AppOpener
-python setup.py sdist bdist_wheel
-```
-The latest release is always available at the Github [releases](https://github.com/athrvvvv/AppOpener/releases).
-
----
-
-### Links 🔗
-
-- PYPI page - https://pypi.org/project/appopener/
-- Official documentation - https://AppOpener.readthedocs.io/en/latest/
-- Github releases - https://github.com/athrvvvv/AppOpener/releases/
-- Project changelog - https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md/
-- Issue tracker - https://github.com/athrvvvv/AppOpener/issues/
-
-### Stay connected 🤝
-
-- [Mail](mailto:athrvchaulkar@gmail.com)
-- [Twitter](https://twitter.com/athrvvvvv)
-- [YouTube](https://www.youtube.com/c/ACUNBOXING2017)
+Metadata-Version: 2.1
+Name: appopener
+Version: 1.7
+Summary: Open/Close any application by it's name.
+Home-page: https://github.com/athrvvvv/AppOpener/tree/module
+Download-URL: https://pypi.python.org/pypi/AppOpener
+Author: Athrv Chaulkar
+Author-email: athrvchaulkar@gmail.com
+Maintainer: athrvvvv
+Maintainer-email: athrvchaulkar@gmail.com
+License: MIT
+Project-URL: Documentation, https://appopener.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/athrvvvv/AppOpener/tree/module
+Project-URL: Tracker, https://github.com/athrvvvv/AppOpener/issues
+Keywords: appopener,open apps,App Ids,automation,close apps
+Platform: Windows 10
+Platform: Windows 8.1
+Platform: Windows 11
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+## AppOpener 🔓
+
+AppOpener is the python library to **open/close** any application **without knowing it's absoulute path**. The library works by making use of App Name and App Id.
+
+Library works on python version 3.5 or above python version 3.5+
+
+[![PyPI Downloads](https://img.shields.io/pypi/dm/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/status/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/v/AppOpener?label=AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![Windows Only](https://img.shields.io/badge/platform-windows-blue.svg)](https://shields.io/)
+
+Visit official documentation of AppOpener [here](https://AppOpener.readthedocs.io/en/latest/).
+
+The latest development version is always available at the [Github](https://github.com/athrvvvv/AppOpener) repository.
+
+All notable changes made to the module, will be documented [here](https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md).
+
+---
+
+> ### Features:
+
+1. Open applications
+2. Close applicatons
+3. Create list of Apps & Ids
+
+---
+
+### Integrating AppOpener
+
+![](https://github.com/athrvvvv/AppOpener/blob/module/docs/img/output.gif)
+
+See [Examples](https://github.com/athrvvvv/AppOpener/tree/module/Examples) for more.
+---
+
+> ### Install Package 📦
+
+```
+pip install AppOpener
+```
+
+> ### Quick start ⚡
+
+``` python
+from AppOpener import open, close, mklist, give_appnames
+open("telegram, whatsapp") # Opens telegram and whatsapp
+open("APPNAME", throw_error=True) # Raises Exception if App is not found (can be used in `close` function too)
+close("telgrm", match_closest=True) # Closes telegram as "telgrm" is closest to "telegram"
+mklist(name="app_data.json") # Generates an file, having key as AppName and value as AppIds.
+appnames = give_appnames() # Save appnames as dictionary
+```
+
+---
+> ### Building package 🔨
+
+```
+git clone https://github.com/athrvvvv/AppOpener.git
+cd AppOpener
+python setup.py sdist bdist_wheel
+```
+The latest release is always available at the Github [releases](https://github.com/athrvvvv/AppOpener/releases).
+
+---
+
+### Links 🔗
+
+- PYPI page - https://pypi.org/project/appopener/
+- Official documentation - https://AppOpener.readthedocs.io/en/latest/
+- Github releases - https://github.com/athrvvvv/AppOpener/releases/
+- Project changelog - https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md/
+- Issue tracker - https://github.com/athrvvvv/AppOpener/issues/
+
+### Stay connected 🤝
+
+- [Mail](mailto:athrvchaulkar@gmail.com)
+- [Twitter](https://twitter.com/athrvvvvv)
+- [YouTube](https://www.youtube.com/c/ACUNBOXING2017)
```

### Comparing `appopener-1.6/README.md` & `appopener-1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,79 @@
-## AppOpener 🔓
-
-AppOpener is the python library to **open/close** any application **without knowing it's absoulute path**. The library works by making use of App Name and App Id.
-
-Library works on python version 3.5 or above python version 3.5+
-
-[![PyPI Downloads](https://img.shields.io/pypi/dm/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/status/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/v/AppOpener?label=AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![Windows Only](https://img.shields.io/badge/platform-windows-blue.svg)](https://shields.io/)
-
-<!-- > **Note**
-> AppOpener is only functional on windows. -->
-
-Visit official documentation of AppOpener [here](https://AppOpener.readthedocs.io/en/latest/).
-
-The latest development version is always available at the [Github](https://github.com/athrvvvv/AppOpener) repository.
-
----
-
-> ### Features:
-
-1. Open applications
-2. Close applicatons
-3. Create list of Apps & Ids
-
----
-
-### Integrating AppOpener
-
-![](docs/img/output.gif)
-
-See [Examples](https://github.com/athrvvvv/AppOpener/tree/module/Examples) for more.
----
-
-> ### Install Package 📦
-
-```
-pip install AppOpener
-```
-
-> ### Quick start ⚡
-
-``` python
-from AppOpener import open, close, mklist
-open("telegram, whatsapp")
-close("telgrm", close_closest=True) # Closes telegram as "telgrm" is closest to "telegram"
-mklist(name="app_data.json")
-```
-
----
-> ### Building package 🔨
-
-```
-git clone https://github.com/athrvvvv/AppOpener.git
-cd AppOpener
-python setup.py sdist bdist_wheel
-```
-The latest release is always available at the Github [releases](https://github.com/athrvvvv/AppOpener/releases).
-
----
-> ### Contributing 🤝
-
-Contributions are welcomed. To know more visit [here](https://github.com/athrvvvv/AppOpener/blob/module/CONTRIBUTING.md).
-
----
-
-### Links 🔗
-
-- PYPI page - https://pypi.org/project/appopener/
-- Official documentation - https://AppOpener.readthedocs.io/en/latest/
-- Github releases - https://github.com/athrvvvv/AppOpener/releases/
-- Project changelog - https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md/
-- Issue tracker - https://github.com/athrvvvv/AppOpener/issues/
-
-### Stay connected 🤗
-
-- [Mail](mailto:athrvchaulkar@gmail.com)
-- [Twitter](https://twitter.com/athrvvvvv)
-- [YouTube](https://www.youtube.com/c/ACUNBOXING2017)
+## AppOpener 🔓
+
+AppOpener is the python library to **open/close** any application **without knowing it's absoulute path**. The library works by making use of App Name and App Id.
+
+Library works on python version 3.5 or above python version 3.5+
+
+[![PyPI Downloads](https://img.shields.io/pypi/dm/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/status/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/v/AppOpener?label=AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![Windows Only](https://img.shields.io/badge/platform-windows-blue.svg)](https://shields.io/)
+
+<!-- > **Note**
+> AppOpener is only functional on windows. -->
+
+Visit official documentation of AppOpener [here](https://AppOpener.readthedocs.io/en/latest/).
+
+The latest development version is always available at the [Github](https://github.com/athrvvvv/AppOpener) repository.
+
+---
+
+> ### Features:
+
+1. Open applications
+2. Close applicatons
+3. Create list of Apps & Ids
+
+---
+
+### Integrating AppOpener
+
+![](docs/img/output.gif)
+
+See [Examples](https://github.com/athrvvvv/AppOpener/tree/module/Examples) for more.
+---
+
+> ### Install Package 📦
+
+```
+pip install AppOpener
+```
+
+> ### Quick start ⚡
+
+``` python
+from AppOpener import open, close, mklist, give_appnames
+open("telegram, whatsapp") # Opens telegram and whatsapp
+open("APPNAME", throw_error=True) # Raises Exception if App is not found (can be used in `close` function too)
+close("telgrm", match_closest=True) # Closes telegram as "telgrm" is closest to "telegram"
+mklist(name="app_data.json") # Generates an file, having key as AppName and value as AppIds.
+appnames = give_appnames() # Save appnames as dictionary
+```
+
+---
+> ### Building package 🔨
+
+```
+git clone https://github.com/athrvvvv/AppOpener.git
+cd AppOpener
+python setup.py sdist bdist_wheel
+```
+The latest release is always available at the Github [releases](https://github.com/athrvvvv/AppOpener/releases).
+
+---
+> ### Contributing 🤝
+
+Contributions are welcomed. To know more visit [here](https://github.com/athrvvvv/AppOpener/blob/module/CONTRIBUTING.md).
+
+---
+
+### Links 🔗
+
+- PYPI page - https://pypi.org/project/appopener/
+- Official documentation - https://AppOpener.readthedocs.io/en/latest/
+- Github releases - https://github.com/athrvvvv/AppOpener/releases/
+- Project changelog - https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md/
+- Issue tracker - https://github.com/athrvvvv/AppOpener/issues/
+
+### Stay connected 🤗
+
+- [Mail](mailto:athrvchaulkar@gmail.com)
+- [Twitter](https://twitter.com/athrvvvvv)
+- [YouTube](https://www.youtube.com/c/ACUNBOXING2017)
```

### Comparing `appopener-1.6/appopener.egg-info/PKG-INFO` & `appopener-1.7/appopener.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,105 @@
-Metadata-Version: 2.1
-Name: appopener
-Version: 1.6
-Summary: Open/Close any application by it's name.
-Home-page: https://github.com/athrvvvv/AppOpener/tree/module
-Download-URL: https://pypi.python.org/pypi/AppOpener
-Author: Athrv Chaulkar
-Author-email: athrvchaulkar@gmail.com
-Maintainer: athrvvvv
-Maintainer-email: athrvchaulkar@gmail.com
-License: MIT
-Project-URL: Documentation, https://appopener.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/athrvvvv/AppOpener/tree/module
-Project-URL: Tracker, https://github.com/athrvvvv/AppOpener/issues
-Keywords: appopener,open apps,App Ids,automation,close apps
-Platform: Windows 10
-Platform: Windows 8.1
-Platform: Windows 11
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-## AppOpener 🔓
-
-AppOpener is the python library to **open/close** any application **without knowing it's absoulute path**. The library works by making use of App Name and App Id.
-
-Library works on python version 3.5 or above python version 3.5+
-
-[![PyPI Downloads](https://img.shields.io/pypi/dm/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/status/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/v/AppOpener?label=AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![Windows Only](https://img.shields.io/badge/platform-windows-blue.svg)](https://shields.io/)
-
-Visit official documentation of AppOpener [here](https://AppOpener.readthedocs.io/en/latest/).
-
-The latest development version is always available at the [Github](https://github.com/athrvvvv/AppOpener) repository.
-
-All notable changes made to the module, will be documented [here](https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md).
-
----
-
-> ### Features:
-
-1. Open applications
-2. Close applicatons
-3. Create list of Apps & Ids
-
----
-
-### Integrating AppOpener
-
-![](https://github.com/athrvvvv/AppOpener/blob/module/docs/img/output.gif)
-
-See [Examples](https://github.com/athrvvvv/AppOpener/tree/module/Examples) for more.
----
-
-> ### Install Package 📦
-
-```
-pip install AppOpener
-```
-
-> ### Quick start ⚡
-
-``` python
-from AppOpener import open, close ,mklist, give_appnames
-open("telegram, whatsapp") # Open telegram & whatsapp
-close("telgrm", match_closest=True) # Closes telegram as "telgrm" is closest to "telegram"
-mklist(name="app_data.json") # Create list of Apps & Ids
-appnames = give_appnames() # Save appnames as dictionary
-```
-
----
-> ### Building package 🔨
-
-```
-git clone https://github.com/athrvvvv/AppOpener.git
-cd AppOpener
-python setup.py sdist bdist_wheel
-```
-The latest release is always available at the Github [releases](https://github.com/athrvvvv/AppOpener/releases).
-
----
-
-### Links 🔗
-
-- PYPI page - https://pypi.org/project/appopener/
-- Official documentation - https://AppOpener.readthedocs.io/en/latest/
-- Github releases - https://github.com/athrvvvv/AppOpener/releases/
-- Project changelog - https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md/
-- Issue tracker - https://github.com/athrvvvv/AppOpener/issues/
-
-### Stay connected 🤝
-
-- [Mail](mailto:athrvchaulkar@gmail.com)
-- [Twitter](https://twitter.com/athrvvvvv)
-- [YouTube](https://www.youtube.com/c/ACUNBOXING2017)
+Metadata-Version: 2.1
+Name: appopener
+Version: 1.7
+Summary: Open/Close any application by it's name.
+Home-page: https://github.com/athrvvvv/AppOpener/tree/module
+Download-URL: https://pypi.python.org/pypi/AppOpener
+Author: Athrv Chaulkar
+Author-email: athrvchaulkar@gmail.com
+Maintainer: athrvvvv
+Maintainer-email: athrvchaulkar@gmail.com
+License: MIT
+Project-URL: Documentation, https://appopener.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/athrvvvv/AppOpener/tree/module
+Project-URL: Tracker, https://github.com/athrvvvv/AppOpener/issues
+Keywords: appopener,open apps,App Ids,automation,close apps
+Platform: Windows 10
+Platform: Windows 8.1
+Platform: Windows 11
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+## AppOpener 🔓
+
+AppOpener is the python library to **open/close** any application **without knowing it's absoulute path**. The library works by making use of App Name and App Id.
+
+Library works on python version 3.5 or above python version 3.5+
+
+[![PyPI Downloads](https://img.shields.io/pypi/dm/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/status/AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![PyPI Downloads](https://img.shields.io/pypi/v/AppOpener?label=AppOpener)](https://pypi.org/project/AppOpener/) &nbsp; [![Windows Only](https://img.shields.io/badge/platform-windows-blue.svg)](https://shields.io/)
+
+Visit official documentation of AppOpener [here](https://AppOpener.readthedocs.io/en/latest/).
+
+The latest development version is always available at the [Github](https://github.com/athrvvvv/AppOpener) repository.
+
+All notable changes made to the module, will be documented [here](https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md).
+
+---
+
+> ### Features:
+
+1. Open applications
+2. Close applicatons
+3. Create list of Apps & Ids
+
+---
+
+### Integrating AppOpener
+
+![](https://github.com/athrvvvv/AppOpener/blob/module/docs/img/output.gif)
+
+See [Examples](https://github.com/athrvvvv/AppOpener/tree/module/Examples) for more.
+---
+
+> ### Install Package 📦
+
+```
+pip install AppOpener
+```
+
+> ### Quick start ⚡
+
+``` python
+from AppOpener import open, close, mklist, give_appnames
+open("telegram, whatsapp") # Opens telegram and whatsapp
+open("APPNAME", throw_error=True) # Raises Exception if App is not found (can be used in `close` function too)
+close("telgrm", match_closest=True) # Closes telegram as "telgrm" is closest to "telegram"
+mklist(name="app_data.json") # Generates an file, having key as AppName and value as AppIds.
+appnames = give_appnames() # Save appnames as dictionary
+```
+
+---
+> ### Building package 🔨
+
+```
+git clone https://github.com/athrvvvv/AppOpener.git
+cd AppOpener
+python setup.py sdist bdist_wheel
+```
+The latest release is always available at the Github [releases](https://github.com/athrvvvv/AppOpener/releases).
+
+---
+
+### Links 🔗
+
+- PYPI page - https://pypi.org/project/appopener/
+- Official documentation - https://AppOpener.readthedocs.io/en/latest/
+- Github releases - https://github.com/athrvvvv/AppOpener/releases/
+- Project changelog - https://github.com/athrvvvv/AppOpener/blob/module/CHANGELOG.md/
+- Issue tracker - https://github.com/athrvvvv/AppOpener/issues/
+
+### Stay connected 🤝
+
+- [Mail](mailto:athrvchaulkar@gmail.com)
+- [Twitter](https://twitter.com/athrvvvvv)
+- [YouTube](https://www.youtube.com/c/ACUNBOXING2017)
```

### Comparing `appopener-1.6/setup.py` & `appopener-1.7/setup.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from distutils.core import setup
-
-exec(compile(open('release.py').read(), 'release.py', 'exec'))
-
-try:
-    from sphinx.setup_command import BuildDoc
-    cmd_class ={'build_sphinx': BuildDoc}
-except ImportError:
-    cmd_class = {}
-
-from release import *
-
-packages = ['AppOpener']
-
-
-setup(name=name,
-      version          = version,
-      description      = description,
-      long_description_content_type="text/markdown",
-      long_description = long_description,
-      author           = authors["Athrv"][0],
-      author_email     = authors["Athrv"][1],
-      maintainer       = authors["athrvvvv"][0],
-      maintainer_email = authors["athrvvvv"][1],
-      license          = license,
-      classifiers      = classifiers,
-      url              = url,
-      download_url     = download_url,
-      project_urls={
-        'Documentation': Documentation,
-        'Source': Source,
-        'Tracker': Tracker,
-    },
-      platforms        = platforms,
-      keywords         = keywords,
-      py_modules       = ['AppOpener'],
-      packages         = packages,
-      include_package_data=True,
-      install_requires=install_requires,
-      cmdclass = cmd_class
-      )
-
+from distutils.core import setup
+
+exec(compile(open('release.py').read(), 'release.py', 'exec'))
+
+try:
+    from sphinx.setup_command import BuildDoc
+    cmd_class ={'build_sphinx': BuildDoc}
+except ImportError:
+    cmd_class = {}
+
+from release import *
+
+packages = ['AppOpener']
+
+
+setup(name=name,
+      version          = version,
+      description      = description,
+      long_description_content_type="text/markdown",
+      long_description = long_description,
+      author           = authors["Athrv"][0],
+      author_email     = authors["Athrv"][1],
+      maintainer       = authors["athrvvvv"][0],
+      maintainer_email = authors["athrvvvv"][1],
+      license          = license,
+      classifiers      = classifiers,
+      url              = url,
+      download_url     = download_url,
+      project_urls={
+        'Documentation': Documentation,
+        'Source': Source,
+        'Tracker': Tracker,
+    },
+      platforms        = platforms,
+      keywords         = keywords,
+      py_modules       = ['AppOpener'],
+      packages         = packages,
+      include_package_data=True,
+      install_requires=install_requires,
+      cmdclass = cmd_class
+      )
+
```

