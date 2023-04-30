# Comparing `tmp/django-whatsapp-business-api-is-0.1.8.tar.gz` & `tmp/django-whatsapp-business-api-is-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-whatsapp-business-api-is-0.1.8.tar", last modified: Sun Nov  6 22:50:50 2022, max compression
+gzip compressed data, was "django-whatsapp-business-api-is-0.1.9.tar", last modified: Sun Nov  6 23:22:21 2022, max compression
```

## Comparing `django-whatsapp-business-api-is-0.1.8.tar` & `django-whatsapp-business-api-is-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-11-06 22:50:50.935591 django-whatsapp-business-api-is-0.1.8/
--rw-rw-rw-   0        0        0     1348 2022-11-06 22:49:41.000000 django-whatsapp-business-api-is-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       34 2022-11-05 23:01:44.000000 django-whatsapp-business-api-is-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      788 2022-11-06 22:50:50.935591 django-whatsapp-business-api-is-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      663 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-06 22:50:50.876056 django-whatsapp-business-api-is-0.1.8/django_whatsapp_business_api_is.egg-info/
--rw-rw-rw-   0        0        0      788 2022-11-06 22:50:50.000000 django-whatsapp-business-api-is-0.1.8/django_whatsapp_business_api_is.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1085 2022-11-06 22:50:50.000000 django-whatsapp-business-api-is-0.1.8/django_whatsapp_business_api_is.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-06 22:50:50.000000 django-whatsapp-business-api-is-0.1.8/django_whatsapp_business_api_is.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-11-06 22:50:50.000000 django-whatsapp-business-api-is-0.1.8/django_whatsapp_business_api_is.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2022-11-06 22:50:50.000000 django-whatsapp-business-api-is-0.1.8/django_whatsapp_business_api_is.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-11-06 00:03:58.000000 django-whatsapp-business-api-is-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      881 2022-11-06 22:50:50.937935 django-whatsapp-business-api-is-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0       38 2022-11-05 22:59:12.000000 django-whatsapp-business-api-is-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-06 22:50:50.920705 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/
--rw-rw-rw-   0        0        0        0 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/__init__.py
--rw-rw-rw-   0        0        0      351 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/admin.py
--rw-rw-rw-   0        0        0     1499 2022-11-06 04:03:31.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/apps.py
--rw-rw-rw-   0        0        0      445 2022-11-06 03:28:02.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/bot_functions.py
--rw-rw-rw-   0        0        0       99 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-11-06 22:50:50.922716 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/management/
--rw-rw-rw-   0        0        0        0 2022-11-06 02:15:18.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/management/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-06 22:50:50.927330 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/management/commands/
--rw-rw-rw-   0        0        0        0 2022-11-06 02:15:18.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1322 2022-11-06 03:01:22.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/management/commands/register_360dialog_webhook.py
--rw-rw-rw-   0        0        0     6372 2022-11-06 22:48:14.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/messages.py
-drwxrwxrwx   0        0        0        0 2022-11-06 22:50:50.934579 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/migrations/
--rw-rw-rw-   0        0        0     3394 2022-11-05 21:58:34.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/migrations/__init__.py
--rw-rw-rw-   0        0        0     3821 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/models.py
--rw-rw-rw-   0        0        0      627 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/singelton.py
--rw-rw-rw-   0        0        0     7985 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/tasks.py
--rw-rw-rw-   0        0        0      785 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/urls.py
--rw-rw-rw-   0        0        0     1791 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/user_msg.py
--rw-rw-rw-   0        0        0     5838 2022-11-06 03:54:58.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/utils.py
--rw-rw-rw-   0        0        0      844 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/views.py
+drwxrwxrwx   0        0        0        0 2022-11-06 23:22:21.919646 django-whatsapp-business-api-is-0.1.9/
+-rw-rw-rw-   0        0        0     1348 2022-11-06 22:49:41.000000 django-whatsapp-business-api-is-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-11-05 23:01:44.000000 django-whatsapp-business-api-is-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      788 2022-11-06 23:22:21.919646 django-whatsapp-business-api-is-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/README.rst
+drwxrwxrwx   0        0        0        0 2022-11-06 23:22:21.836425 django-whatsapp-business-api-is-0.1.9/django_whatsapp_business_api_is.egg-info/
+-rw-rw-rw-   0        0        0      788 2022-11-06 23:22:21.000000 django-whatsapp-business-api-is-0.1.9/django_whatsapp_business_api_is.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1085 2022-11-06 23:22:21.000000 django-whatsapp-business-api-is-0.1.9/django_whatsapp_business_api_is.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-06 23:22:21.000000 django-whatsapp-business-api-is-0.1.9/django_whatsapp_business_api_is.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2022-11-06 23:22:21.000000 django-whatsapp-business-api-is-0.1.9/django_whatsapp_business_api_is.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2022-11-06 23:22:21.000000 django-whatsapp-business-api-is-0.1.9/django_whatsapp_business_api_is.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-11-06 00:03:58.000000 django-whatsapp-business-api-is-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      881 2022-11-06 23:22:21.922655 django-whatsapp-business-api-is-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0       38 2022-11-05 22:59:12.000000 django-whatsapp-business-api-is-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-06 23:22:21.888930 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/
+-rw-rw-rw-   0        0        0        0 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/__init__.py
+-rw-rw-rw-   0        0        0      351 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/admin.py
+-rw-rw-rw-   0        0        0     1499 2022-11-06 04:03:31.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/apps.py
+-rw-rw-rw-   0        0        0      445 2022-11-06 03:28:02.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/bot_functions.py
+-rw-rw-rw-   0        0        0       99 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-11-06 23:22:21.890922 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/management/
+-rw-rw-rw-   0        0        0        0 2022-11-06 02:15:18.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/management/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-06 23:22:21.908602 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/management/commands/
+-rw-rw-rw-   0        0        0        0 2022-11-06 02:15:18.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1322 2022-11-06 03:01:22.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/management/commands/register_360dialog_webhook.py
+-rw-rw-rw-   0        0        0     6490 2022-11-06 23:21:32.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/messages.py
+drwxrwxrwx   0        0        0        0 2022-11-06 23:22:21.918500 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/migrations/
+-rw-rw-rw-   0        0        0     3394 2022-11-05 21:58:34.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3821 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/models.py
+-rw-rw-rw-   0        0        0      627 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/singelton.py
+-rw-rw-rw-   0        0        0     7985 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/tasks.py
+-rw-rw-rw-   0        0        0      785 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/urls.py
+-rw-rw-rw-   0        0        0     1791 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/user_msg.py
+-rw-rw-rw-   0        0        0     5838 2022-11-06 03:54:58.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/utils.py
+-rw-rw-rw-   0        0        0      844 2022-11-05 22:54:35.000000 django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/views.py
```

### Comparing `django-whatsapp-business-api-is-0.1.8/LICENSE` & `django-whatsapp-business-api-is-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/PKG-INFO` & `django-whatsapp-business-api-is-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-whatsapp-business-api-is
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django Whatsapp Business Api Infrastructure
 Home-page: https://github.com/roigreenberg/django-whatsapp-business-api-is
 License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `django-whatsapp-business-api-is-0.1.8/README.rst` & `django-whatsapp-business-api-is-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/django_whatsapp_business_api_is.egg-info/PKG-INFO` & `django-whatsapp-business-api-is-0.1.9/django_whatsapp_business_api_is.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-whatsapp-business-api-is
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django Whatsapp Business Api Infrastructure
 Home-page: https://github.com/roigreenberg/django-whatsapp-business-api-is
 License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `django-whatsapp-business-api-is-0.1.8/django_whatsapp_business_api_is.egg-info/SOURCES.txt` & `django-whatsapp-business-api-is-0.1.9/django_whatsapp_business_api_is.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/setup.cfg` & `django-whatsapp-business-api-is-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 7768 6174 7361   = django-whatsa
 00000020: 7070 2d62 7573 696e 6573 732d 6170 692d  pp-business-api-
 00000030: 6973 0d0a 7665 7273 696f 6e20 3d20 302e  is..version = 0.
-00000040: 312e 380d 0a64 6573 6372 6970 7469 6f6e  1.8..description
+00000040: 312e 390d 0a64 6573 6372 6970 7469 6f6e  1.9..description
 00000050: 203d 2044 6a61 6e67 6f20 5768 6174 7361   = Django Whatsa
 00000060: 7070 2042 7573 696e 6573 7320 4170 6920  pp Business Api 
 00000070: 496e 6672 6173 7472 7563 7475 7265 0d0a  Infrastructure..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 203d 2066 696c 653a 5245 4144 4d45 0d0a   = file:README..
 000000a0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
 000000b0: 7468 7562 2e63 6f6d 2f72 6f69 6772 6565  thub.com/roigree
```

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/apps.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/apps.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/management/commands/register_360dialog_webhook.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/management/commands/register_360dialog_webhook.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/messages.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,16 @@
     logging.debug(f"{components=}")
     message = get_template_message_data(user.number, wab_bot_message.template_name, components)
 
     if settings.DEMO_MODE:
         logging.info(f"{'*' * 20}\n*   {message=}\n{'*' * 20}")
         text = wab_bot_message.pk
         if wab_bot_message.quick_reply:
-            text = f"{text}: [{[r[1] for r in wab_bot_message.quick_reply]}]"
+            quick_replies = [list(reply.items())[0] for reply in wab_bot_message.quick_reply]
+            text = f"{text}: [{[r[1] for r in quick_replies]}]"
         message = get_text_message_data(user.number, text)
 
     if message:
         send_message(message)
 
 
 def send_media_message(user, wab_bot_message, message_text=None):
@@ -153,15 +154,15 @@
         body['text'] = message_text.format(**variables)
     else:
         parts['body'] = {'text': message_text}
 
     match wab_bot_message.type:  # there are other type that not implemented yet
         case 'quick_reply':
             parts['type'] = 'button'
-            buttons = wab_bot_message.quick_reply
+            buttons = [list(reply.items())[0] for reply in wab_bot_message.quick_reply]
             parts['action'] = {
                 "buttons": [create_button(id, name) for id, name in buttons]
             }
 
     message = get_interactive_message_data(parts, user.number)
 
     assert message
```

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/migrations/0001_initial.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/models.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/models.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/singelton.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/singelton.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/tasks.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/tasks.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/urls.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/urls.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/user_msg.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/user_msg.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/utils.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/utils.py`

 * *Files identical despite different names*

### Comparing `django-whatsapp-business-api-is-0.1.8/whatsapp_business_api_is/views.py` & `django-whatsapp-business-api-is-0.1.9/whatsapp_business_api_is/views.py`

 * *Files identical despite different names*

