# Comparing `tmp/pyLegendBS-0.6.tar.gz` & `tmp/pyLegendBS-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLegendBS-0.6.tar", last modified: Thu Apr 20 06:37:45 2023, max compression
+gzip compressed data, was "pyLegendBS-0.7.tar", last modified: Sun Apr 30 01:31:06 2023, max compression
```

## Comparing `pyLegendBS-0.6.tar` & `pyLegendBS-0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 06:37:45.610034 pyLegendBS-0.6/
--rw-rw-rw-   0        0        0    35149 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-20 06:37:45.482025 pyLegendBS-0.6/LegendBS/
--rw-rw-rw-   0        0        0        1 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/__init__.py
--rw-rw-rw-   0        0        0      794 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/banall.py
--rw-rw-rw-   0        0        0     2536 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/birthday.py
--rw-rw-rw-   0        0        0        1 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/botspam.py
--rw-rw-rw-   0        0        0      369 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/error.py
--rw-rw-rw-   0        0        0      390 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/get_time.py
--rw-rw-rw-   0        0        0     2081 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/get_user.py
--rw-rw-rw-   0        0        0     1705 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/love.py
--rw-rw-rw-   0        0        0     3094 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/porn.py
--rw-rw-rw-   0        0        0    33658 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/raid.py
--rw-rw-rw-   0        0        0      911 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/start.py
--rw-rw-rw-   0        0        0      216 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/start_bot.py
--rw-rw-rw-   0        0        0        1 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/start_help.py
--rw-rw-rw-   0        0        0     3518 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/startup.py
--rw-rw-rw-   0        0        0    17800 2023-04-20 04:51:14.000000 pyLegendBS-0.6/LegendBS/yup.py
--rw-rw-rw-   0        0        0     1156 2023-04-20 06:37:45.601031 pyLegendBS-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-20 04:51:14.000000 pyLegendBS-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 06:37:45.598034 pyLegendBS-0.6/pyLegendBS.egg-info/
--rw-rw-rw-   0        0        0     1156 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 06:37:45.000000 pyLegendBS-0.6/pyLegendBS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 06:37:45.610034 pyLegendBS-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-04-20 04:51:14.000000 pyLegendBS-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:31:06.466300 pyLegendBS-0.7/
+-rw-rw-rw-   0        0        0    35149 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-30 01:31:06.375308 pyLegendBS-0.7/LegendBS/
+-rw-rw-rw-   0        0        0        1 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/__init__.py
+-rw-rw-rw-   0        0        0     6946 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/abuse.py
+-rw-rw-rw-   0        0        0      745 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/banall.py
+-rw-rw-rw-   0        0        0     2536 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/birthday.py
+-rw-rw-rw-   0        0        0      369 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/error.py
+-rw-rw-rw-   0        0        0      390 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/get_time.py
+-rw-rw-rw-   0        0        0     2081 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/get_user.py
+-rw-rw-rw-   0        0        0     1705 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/love.py
+-rw-rw-rw-   0        0        0     3094 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/porn.py
+-rw-rw-rw-   0        0        0    33658 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/raid.py
+-rw-rw-rw-   0        0        0      904 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/start.py
+-rw-rw-rw-   0        0        0     3028 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/start_bot.py
+-rw-rw-rw-   0        0        0        1 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/start_help.py
+-rw-rw-rw-   0        0        0     3528 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/startup.py
+-rw-rw-rw-   0        0        0    17800 2023-04-30 01:28:41.000000 pyLegendBS-0.7/LegendBS/yup.py
+-rw-rw-rw-   0        0        0     1156 2023-04-30 01:31:06.463300 pyLegendBS-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-30 01:28:41.000000 pyLegendBS-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 01:31:06.420285 pyLegendBS-0.7/pyLegendBS.egg-info/
+-rw-rw-rw-   0        0        0     1156 2023-04-30 01:31:05.000000 pyLegendBS-0.7/pyLegendBS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-04-30 01:31:06.000000 pyLegendBS-0.7/pyLegendBS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 01:31:05.000000 pyLegendBS-0.7/pyLegendBS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-30 01:31:05.000000 pyLegendBS-0.7/pyLegendBS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 01:31:05.000000 pyLegendBS-0.7/pyLegendBS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 01:31:06.466300 pyLegendBS-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2023-04-30 01:28:41.000000 pyLegendBS-0.7/setup.py
```

### Comparing `pyLegendBS-0.6/LICENSE` & `pyLegendBS-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.6/LegendBS/banall.py` & `pyLegendBS-0.7/LegendBS/banall.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 async def start_banall(Legend, message):
     chat = message.chat
-    a = await Legend.get_chat_member(chat.id, 'me')
-    if a.status == "administrator":
-        x = await Legend.send_message(chat.id, "Hey it's Legend Bot Spam")
-        done = 0
-        failed = 0
-        async for u in Legend.get_chat_members(chat.id):
-            user = u.user
-            try:
-                await Legend.ban_chat_member(chat.id, user.id)
-                done += 1
-            except Exception as err:
-                print(f"Legend Bot Spam- [INFO]: {str(err)}")
-                failed += 1
-        await x.delete()
-        await Legend.send_message(chat.id, f"Members Banned ✓ \n\n Banned {done} users\n failed {failed}")
-    else:
-        await Legend.send_message(chat.id, "Promote me to admin😭")
+    # a = await Legend.get_chat_member(chat.id, 'me')
+    # if a.status != "administrator":
+    #     return await Legend.send_message(chat.id, "Promote me to admin😭")
+    x = await Legend.send_message(chat.id, "Hey it's Legend Bot Spam")
+    done = 0
+    failed = 0
+    async for u in Legend.get_chat_members(chat.id):
+        user = u.user
+        try:
+            await Legend.ban_chat_member(chat.id, user.id)
+            done += 1
+        except Exception as err:
+            print(f"Legend Bot Spam- [INFO]: {str(err)}")
+            failed += 1
+    await x.delete()
+    await Legend.send_message(chat.id, f"Members Banned ✓ \n\n Banned {done} users\n failed {failed}")
```

### Comparing `pyLegendBS-0.6/LegendBS/birthday.py` & `pyLegendBS-0.7/LegendBS/birthday.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.6/LegendBS/get_user.py` & `pyLegendBS-0.7/LegendBS/get_user.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.6/LegendBS/love.py` & `pyLegendBS-0.7/LegendBS/love.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.6/LegendBS/porn.py` & `pyLegendBS-0.7/LegendBS/porn.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.6/LegendBS/raid.py` & `pyLegendBS-0.7/LegendBS/raid.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.6/LegendBS/start.py` & `pyLegendBS-0.7/LegendBS/start.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             InlineKeyboardButton(
                 text="🧸 Add me in your group 🧸",
                 url=f"https://t.me/{x.username}?startgroup=true",
             ),
         ],
         [
             InlineKeyboardButton(
-                text="❄️ Source Code ❄️", url=f"https://github.com/LEGEND-AI/BOTSPAM"
+                text="❄️ Repo ❄️", url=f"https://github.com/LEGEND-AI/BOTSPAM"
             ),
             InlineKeyboardButton(
                 text="☁️ Updates ☁️", url=f"https://t.me/LegendBot_AI"
             ),
         ],
     ]
     return START_OP
```

### Comparing `pyLegendBS-0.6/LegendBS/startup.py` & `pyLegendBS-0.7/LegendBS/startup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-
+import sys
 def bot_start():
     os.system("clear")
     ask = input("Do You Want to Start Bot Spam y/n: ")
     if ask.lower() == "y":
         os.system("python3 -m LegendGirl")
     elif ask.lower() == "n":
         print("\nOk! You Can Start It Later With by using; python3-m LegendGirl\n")
```

### Comparing `pyLegendBS-0.6/LegendBS/yup.py` & `pyLegendBS-0.7/LegendBS/yup.py`

 * *Files identical despite different names*

### Comparing `pyLegendBS-0.6/PKG-INFO` & `pyLegendBS-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendBS
-Version: 0.6
+Version: 0.7
 Summary: This is a simple package which is used in Bot Spam
 Home-page: https://github.com/LEGEND-AI/pyLegendBS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendBS,LegendBS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendBS-0.6/pyLegendBS.egg-info/PKG-INFO` & `pyLegendBS-0.7/pyLegendBS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendBS
-Version: 0.6
+Version: 0.7
 Summary: This is a simple package which is used in Bot Spam
 Home-page: https://github.com/LEGEND-AI/pyLegendBS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendBS,LegendBS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendBS-0.6/setup.py` & `pyLegendBS-0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyLegendBS",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.6",
+    version="0.7",
     description="This is a simple package which is used in Bot Spam",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyLegendBS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
@@ -34,9 +34,9 @@
         "Programming Language :: Python :: 3.10",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Build Tools",
 
     ],
     keywords=["pyLegendBS", "LegendBS"],
-    install_requires=["pyrogram"]
+    install_requires=["pyrogram", "datetime"]
 )
```

