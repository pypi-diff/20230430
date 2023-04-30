# Comparing `tmp/rum_with_telegram-0.8.6.tar.gz` & `tmp/rum_with_telegram-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.8.6.tar", last modified: Thu Apr 27 15:26:21 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.8.7.tar", last modified: Sun Apr 30 16:32:46 2023, max compression
```

## Comparing `rum_with_telegram-0.8.6.tar` & `rum_with_telegram-0.8.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:21.647324 rum_with_telegram-0.8.6/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.6/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-04-27 15:26:21.646350 rum_with_telegram-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.6/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:21.634358 rum_with_telegram-0.8.6/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-04-27 15:25:09.000000 rum_with_telegram-0.8.6/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-04-27 12:59:31.000000 rum_with_telegram-0.8.6/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    23983 2023-04-27 15:24:57.000000 rum_with_telegram-0.8.6/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.6/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.6/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:26:21.644356 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-27 15:26:21.000000 rum_with_telegram-0.8.6/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 15:26:21.648321 rum_with_telegram-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-04-27 15:25:09.000000 rum_with_telegram-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:32:46.395792 rum_with_telegram-0.8.7/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.7/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-04-30 16:32:46.394795 rum_with_telegram-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.7/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-30 16:32:46.383824 rum_with_telegram-0.8.7/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-04-30 16:32:07.000000 rum_with_telegram-0.8.7/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-04-27 12:59:31.000000 rum_with_telegram-0.8.7/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    23983 2023-04-30 16:32:13.000000 rum_with_telegram-0.8.7/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3112 2023-04-30 16:31:39.000000 rum_with_telegram-0.8.7/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.7/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:32:46.392827 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-30 16:32:46.000000 rum_with_telegram-0.8.7/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:32:46.396791 rum_with_telegram-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-04-30 16:32:07.000000 rum_with_telegram-0.8.7/setup.py
```

### Comparing `rum_with_telegram-0.8.6/LICENSE` & `rum_with_telegram-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.6/PKG-INFO` & `rum_with_telegram-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.8.6
+Version: 0.8.7
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.6/rum_with_telegram/config.py` & `rum_with_telegram-0.8.7/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.6/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.8.7/rum_with_telegram/data_exchanger.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.6/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.8.7/rum_with_telegram/db_handle.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,20 +45,27 @@
 
     def get_all(self, table, payload: dict, pk: str):
         with self.Session() as session:
             return session.query(table).filter_by(**{pk: payload[pk]}).all()
 
     def get_trx_sent(self, channel_message_id):
         with self.Session() as session:
-            relatins = (
+            relation = (
+                session.query(Relation)
+                .filter_by(channel_message_id=channel_message_id, chat_type="private")
+                .first()
+            )
+            if relation and relation.trx_id:
+                return relation
+            relations = (
                 session.query(Relation).filter_by(channel_message_id=channel_message_id).all()
             )
-            for i in relatins:
-                if i.trx_id:
-                    return i
+            for relation in relations:
+                if relation.trx_id:
+                    return relation
         return None
 
     def is_exist(self, table, payload: dict, pk: str):
         with self.Session() as session:
             return session.query(table).filter_by(**{pk: payload[pk]}).count() > 0
 
     def add_or_update(self, table, payload, pk):
```

### Comparing `rum_with_telegram-0.8.6/rum_with_telegram/module.py` & `rum_with_telegram-0.8.7/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.6/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.8.7/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.8.6
+Version: 0.8.7
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.6/setup.py` & `rum_with_telegram-0.8.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.8.6",
+    version="0.8.7",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

