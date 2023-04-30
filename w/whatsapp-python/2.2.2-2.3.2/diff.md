# Comparing `tmp/whatsapp-python-2.2.2.tar.gz` & `tmp/whatsapp-python-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-python-2.2.2.tar", last modified: Sat Apr  8 15:10:06 2023, max compression
+gzip compressed data, was "whatsapp-python-2.3.2.tar", last modified: Sun Apr 30 08:30:20 2023, max compression
```

## Comparing `whatsapp-python-2.2.2.tar` & `whatsapp-python-2.3.2.tar`

### file list

```diff
@@ -1,20 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:10:06.632844 whatsapp-python-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-08 15:10:06.632844 whatsapp-python-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 15:10:06.632844 whatsapp-python-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:10:06.632844 whatsapp-python-2.2.2/whatsapp/
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/whatsapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/whatsapp/_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/whatsapp/_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/whatsapp/_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/whatsapp/_send_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/whatsapp/_send_others.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-08 15:10:02.000000 whatsapp-python-2.2.2/whatsapp/_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:10:06.632844 whatsapp-python-2.2.2/whatsapp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-08 15:10:06.000000 whatsapp-python-2.2.2/whatsapp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-08 15:10:06.000000 whatsapp-python-2.2.2/whatsapp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 15:10:06.000000 whatsapp-python-2.2.2/whatsapp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 15:10:06.000000 whatsapp-python-2.2.2/whatsapp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 15:10:06.000000 whatsapp-python-2.2.2/whatsapp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 08:30:19.000000 whatsapp-python-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-30 08:30:19.000000 whatsapp-python-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-30 08:30:19.000000 whatsapp-python-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/whatsapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-04-30 08:30:19.000000 whatsapp-python-2.3.2/whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/whatsapp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/top_level.txt
```

### Comparing `whatsapp-python-2.2.2/LICENSE` & `whatsapp-python-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-python-2.2.2/PKG-INFO` & `whatsapp-python-2.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 2.2.2
+Version: 2.3.2
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Keywords: whatsapp,whatsapp-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Classifier: Development Status :: 4 - Beta
@@ -26,38 +26,39 @@
 [![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
 Unofficial Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
-## ⚠️ WARNING ⚠️
-Any version newer than 1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
-
-You can ignore this warning if it's your first time using the library.
-
 ## Supported features
 
 1. Sending messages
 2. Marking messages as read
 3. Sending Media (images, audio, video and documents)
 4. Sending location
 5. Sending interactive buttons
 6. Sending template messages
 7. Parsing messages and media received
 
 ## Switching from `Neurotech-HQ/heyoo`
+Any version newer than 1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
+
+You can ignore this warning if it's your first time using the library.
+
+
 Switching from heyoo to whatsapp-python doesn't require any change for versions up to 1.1.2: just uninstall the old, install the new and change the import name from `heyoo` to `whatsapp`.
 For version which are GREATER THEN 1.1.2, messages have became objects, so you need to change your code to use the new methods.
 
+Note: docs for version 1.1.2 are available in the [wiki dedicated page](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
 
 
 ## Documentation
 
-The documentation is available under the [wiki section](https://github.com/filipporomani/whatsapp/wiki)
+The documentation for the is available in the [wiki section](https://github.com/filipporomani/whatsapp/wiki)
 
 
 ## Issues
 
 If you are facing any issues or have any questions, please open an issue on the [GitHub repository](https://github.com/filipporomani/whatsapp/issues)
 
 ## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `whatsapp-python-2.2.2/README.md` & `whatsapp-python-2.3.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 [![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
 Unofficial Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
-## ⚠️ WARNING ⚠️
-Any version newer than 1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
-
-You can ignore this warning if it's your first time using the library.
-
 ## Supported features
 
 1. Sending messages
 2. Marking messages as read
 3. Sending Media (images, audio, video and documents)
 4. Sending location
 5. Sending interactive buttons
 6. Sending template messages
 7. Parsing messages and media received
 
 ## Switching from `Neurotech-HQ/heyoo`
+Any version newer than 1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
+
+You can ignore this warning if it's your first time using the library.
+
+
 Switching from heyoo to whatsapp-python doesn't require any change for versions up to 1.1.2: just uninstall the old, install the new and change the import name from `heyoo` to `whatsapp`.
 For version which are GREATER THEN 1.1.2, messages have became objects, so you need to change your code to use the new methods.
 
+Note: docs for version 1.1.2 are available in the [wiki dedicated page](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
 
 
 ## Documentation
 
-The documentation is available under the [wiki section](https://github.com/filipporomani/whatsapp/wiki)
+The documentation for the is available in the [wiki section](https://github.com/filipporomani/whatsapp/wiki)
 
 
 ## Issues
 
 If you are facing any issues or have any questions, please open an issue on the [GitHub repository](https://github.com/filipporomani/whatsapp/issues)
 
 ## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `whatsapp-python-2.2.2/setup.py` & `whatsapp-python-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="whatsapp-python",
-    version="2.2.2",
+    version="2.3.2",
     description="Opensource Python wrapper to WhatsApp Cloud API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipporomani/whatsapp",
     author="Filippo Romani",
     author_email="mail@filipporomani.it",
     license="MIT",
```

### Comparing `whatsapp-python-2.2.2/whatsapp/__init__.py` & `whatsapp-python-2.3.2/whatsapp/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Unofficial python wrapper for the WhatsApp Cloud API.
+Unofficial Python wrapper for the WhatsApp Cloud API.
 """
 from __future__ import annotations
 
 import requests
 from json import dumps
 import logging
 
@@ -17,30 +17,33 @@
     """
 
     def __init__(self, token: str = "", phone_number_id: str = "", logger: bool = True):
         """
         Initialize the WhatsApp Object
 
         Args:
-            token[str]: Token for the WhatsApp cloud API obtained from the developer portal
+            token[str]: Token for the WhatsApp cloud API obtained from the Facebook developer portal
             phone_number_id[str]: Phone number id for the WhatsApp cloud API obtained from the developer portal
             logger[bool]: Whether to enable logging or not (default: True)
         """
 
         # Check if the version is up to date
-        self.VERSION = "2.2.2"
+        self.VERSION = "2.3.3"
         latest = str(requests.get(
             "https://pypi.org/pypi/whatsapp-python/json").json()["info"]["version"])
         if self.VERSION != latest:
             version_int = int(self.VERSION.replace(".", ""))
             latest_int = int(latest.replace(".", ""))
             # this is to avoid the case where the version is 1.0.10 and the latest is 1.0.2 (possible if user is using the github version)
             if version_int < latest_int:
                 logging.critical(
                     f"Whatsapp-python is out of date. Please update to the latest version {latest}. READ THE CHANGELOG BEFORE UPDATING. NEW VERSIONS MAY BREAK YOUR CODE IF NOT PROPERLY UPDATED.")
+            if version_int > latest_int:
+                logging.critical(
+                    f"You are using a development version of whatsapp-python. Please report any issue on GitHub.")
 
         if token == "" or phone_number_id == "":
             logging.error("Token or phone number id not provided")
             raise ValueError(
                 "Token or phone number ID not provided but is required")
         self.token = token
         self.phone_number_id = phone_number_id
@@ -51,26 +54,23 @@
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.token}"
         }
         if logger is False:
             logging.disable(logging.INFO)
             logging.disable(logging.ERROR)
 
-    @property
-    def authorized(self) -> bool:
-        return requests.get(self.url, headers=self.headers).status_code != 401
-    
     # all the files starting with _ are imported here, and should not be imported directly.
 
-    from ._send_others import send_custom_json, send_contacts
-    from ._message import send_template
-    from ._send_media import send_image, send_video, send_audio, send_location, send_sticker, send_document
-    from ._media import upload_media, query_media_url, download_media, delete_media
-    from ._buttons import send_button, create_button, send_reply_button
-    from ._static import is_message, get_mobile, get_author, get_name, get_message, get_message_id, get_message_type, get_message_timestamp, get_audio, get_delivery, get_document, get_image, get_interactive_response, get_location, get_video, changed_field
+    from ext._property import authorized
+    from ext._send_others import send_custom_json, send_contacts
+    from ext._message import send_template
+    from ext._send_media import send_image, send_video, send_audio, send_location, send_sticker, send_document
+    from ext._media import upload_media, query_media_url, download_media, delete_media
+    from ext._buttons import send_button, create_button, send_reply_button
+    from ext._static import is_message, get_mobile, get_author, get_name, get_message, get_message_id, get_message_type, get_message_timestamp, get_audio, get_delivery, get_document, get_image, get_interactive_response, get_location, get_video, changed_field
     is_message = staticmethod(is_message)
     get_mobile = staticmethod(get_mobile)
     get_name = staticmethod(get_name)
     get_message = staticmethod(get_message)
     get_message_id = staticmethod(get_message_id)
     get_message_type = staticmethod(get_message_type)
     get_message_timestamp = staticmethod(get_message_timestamp)
@@ -79,53 +79,87 @@
     get_document = staticmethod(get_document)
     get_image = staticmethod(get_image)
     get_interactive_response = staticmethod(get_interactive_response)
     get_location = staticmethod(get_location)
     get_video = staticmethod(get_video)
     changed_field = staticmethod(changed_field)
     get_author = staticmethod(get_author)
+
+    authorized = property(authorized)
     
+    def create_message(self, **kwargs) -> Message:
+        """
+        Create a message object
+
+        Args:
+            data[dict]: The message data
+            content[str]: The message content
+            to[str]: The recipient
+            rec_type[str]: The recipient type (individual/group)
+        """
+        return Message(**kwargs, instance=self)
     
+
+
 class Message(object):
-    def __init__(self, data: dict = {}, instance: WhatsApp = None, content: str = "", to: str = "", rec_type: str = "individual"): # type: ignore
-        try: self.id = instance.get_message_id(data)
-        except: self.id = None
-        try: self.type = self.instance.get_message_type(data)
-        except: self.type = "text"
+    def __init__(self, data: dict = {}, instance: WhatsApp = None, content: str = "", to: str = "", rec_type: str = "individual"):  # type: ignore
+        try:
+            self.id = instance.get_message_id(data)
+        except:
+            self.id = None
+        try:
+            self.type = self.instance.get_message_type(data)
+        except:
+            self.type = "text"
         self.data = data
         self.rec = rec_type
         self.to = to
-        try: self.content = content if content != "" else self.instance.get_message(data)
-        except: self.content = content
-        try: self.sender = self.instance.get_mobile(data)
-        except: self.sender = None
-        try: self.name = self.instance.get_name(data)
-        except: self.name = None
-    
-    
+        try:
+            self.content = content if content != "" else self.instance.get_message(
+                data)
+        except:
+            self.content = content
+        try:
+            self.sender = self.instance.get_mobile(data)
+        except:
+            self.sender = None
+        try:
+            self.name = self.instance.get_name(data)
+        except:
+            self.name = None
+
         if self.type == "image":
-            try: self.image = self.instance.get_image(data)
-            except: self.image = None
+            try:
+                self.image = self.instance.get_image(data)
+            except:
+                self.image = None
         elif self.type == "video":
-            try: self.video = self.instance.get_video(data)
-            except: self.video = None
+            try:
+                self.video = self.instance.get_video(data)
+            except:
+                self.video = None
         elif self.type == "audio":
-            try: self.audio = self.instance.get_audio(data)
-            except: pass
+            try:
+                self.audio = self.instance.get_audio(data)
+            except:
+                pass
         elif self.type == "document":
-            try: self.document = self.instance.get_document(data)
-            except: pass
+            try:
+                self.document = self.instance.get_document(data)
+            except:
+                pass
         elif self.type == "location":
-            try: self.location = self.instance.get_location(data)
-            except: pass
+            try:
+                self.location = self.instance.get_location(data)
+            except:
+                pass
         elif self.type == "interactive":
-            try: self.interactive = self.instance.get_interactive_response(data)
-            except: pass
-        
-        
-        
+            try:
+                self.interactive = self.instance.get_interactive_response(data)
+            except:
+                pass
+
         self.instance = instance
         self.url = self.instance.url
         self.headers = self.instance.headers
-        
-        
-    from ._message import send, reply, mark_as_read
+
+    from ext._message import send, reply, mark_as_read
```

### Comparing `whatsapp-python-2.2.2/whatsapp_python.egg-info/PKG-INFO` & `whatsapp-python-2.3.2/whatsapp_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 2.2.2
+Version: 2.3.2
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Keywords: whatsapp,whatsapp-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Classifier: Development Status :: 4 - Beta
@@ -26,38 +26,39 @@
 [![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
 Unofficial Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
-## ⚠️ WARNING ⚠️
-Any version newer than 1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
-
-You can ignore this warning if it's your first time using the library.
-
 ## Supported features
 
 1. Sending messages
 2. Marking messages as read
 3. Sending Media (images, audio, video and documents)
 4. Sending location
 5. Sending interactive buttons
 6. Sending template messages
 7. Parsing messages and media received
 
 ## Switching from `Neurotech-HQ/heyoo`
+Any version newer than 1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
+
+You can ignore this warning if it's your first time using the library.
+
+
 Switching from heyoo to whatsapp-python doesn't require any change for versions up to 1.1.2: just uninstall the old, install the new and change the import name from `heyoo` to `whatsapp`.
 For version which are GREATER THEN 1.1.2, messages have became objects, so you need to change your code to use the new methods.
 
+Note: docs for version 1.1.2 are available in the [wiki dedicated page](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
 
 
 ## Documentation
 
-The documentation is available under the [wiki section](https://github.com/filipporomani/whatsapp/wiki)
+The documentation for the is available in the [wiki section](https://github.com/filipporomani/whatsapp/wiki)
 
 
 ## Issues
 
 If you are facing any issues or have any questions, please open an issue on the [GitHub repository](https://github.com/filipporomani/whatsapp/issues)
 
 ## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

