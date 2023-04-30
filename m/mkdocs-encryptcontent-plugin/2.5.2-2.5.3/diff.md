# Comparing `tmp/mkdocs-encryptcontent-plugin-2.5.2.tar.gz` & `tmp/mkdocs-encryptcontent-plugin-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-encryptcontent-plugin-2.5.2.tar", last modified: Fri Apr 14 08:38:14 2023, max compression
+gzip compressed data, was "mkdocs-encryptcontent-plugin-2.5.3.tar", last modified: Sun Apr 30 16:39:48 2023, max compression
```

## Comparing `mkdocs-encryptcontent-plugin-2.5.2.tar` & `mkdocs-encryptcontent-plugin-2.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.409063 mkdocs-encryptcontent-plugin-2.5.2/
--rw-rw-rw-   0        0        0     1070 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/LICENSE.md
--rw-rw-rw-   0        0        0    33922 2023-04-14 08:38:14.402063 mkdocs-encryptcontent-plugin-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    27028 2023-04-14 08:37:56.000000 mkdocs-encryptcontent-plugin-2.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.379067 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/
--rw-rw-rw-   0        0        0        0 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.374068 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/
-drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.374068 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/
-drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.381068 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/
--rw-rw-rw-   0        0        0    99860 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/lunr.js
--rw-rw-rw-   0        0        0     3670 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/main.js
--rw-rw-rw-   0        0        0     4195 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/worker.js
--rw-rw-rw-   0        0        0    14540 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/decrypt-contents.tpl.js
--rw-rw-rw-   0        0        0     1206 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/decrypt-form.tpl.html
--rw-rw-rw-   0        0        0    36217 2023-04-14 08:37:01.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/plugin.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.400065 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/
--rw-rw-rw-   0        0        0    33922 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 08:38:14.410066 mkdocs-encryptcontent-plugin-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1780 2023-04-14 08:37:53.000000 mkdocs-encryptcontent-plugin-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:39:48.115023 mkdocs-encryptcontent-plugin-2.5.3/
+-rw-rw-rw-   0        0        0     1070 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.3/LICENSE.md
+-rw-rw-rw-   0        0        0    34636 2023-04-30 16:39:48.115023 mkdocs-encryptcontent-plugin-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0    27652 2023-04-30 16:35:46.000000 mkdocs-encryptcontent-plugin-2.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 16:39:48.080019 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/
+-rw-rw-rw-   0        0        0        0 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:39:48.060023 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/
+drwxrwxrwx   0        0        0        0 2023-04-30 16:39:48.060023 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/templates/
+drwxrwxrwx   0        0        0        0 2023-04-30 16:39:48.083021 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/templates/search/
+-rw-rw-rw-   0        0        0    99860 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/templates/search/lunr.js
+-rw-rw-rw-   0        0        0     3670 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/templates/search/main.js
+-rw-rw-rw-   0        0        0     4195 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/templates/search/worker.js
+-rw-rw-rw-   0        0        0    14202 2023-04-30 16:33:21.000000 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/decrypt-contents.tpl.js
+-rw-rw-rw-   0        0        0     1206 2023-04-30 16:33:21.000000 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/decrypt-form.tpl.html
+-rw-rw-rw-   0        0        0    36125 2023-04-30 16:33:21.000000 mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:39:48.113022 mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/
+-rw-rw-rw-   0        0        0    34636 2023-04-30 16:39:47.000000 mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-04-30 16:39:48.000000 mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 16:39:47.000000 mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-04-30 16:39:47.000000 mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:39:47.000000 mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-30 16:39:47.000000 mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:39:48.116022 mkdocs-encryptcontent-plugin-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1780 2023-04-30 16:33:22.000000 mkdocs-encryptcontent-plugin-2.5.3/setup.py
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/LICENSE.md` & `mkdocs-encryptcontent-plugin-2.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/PKG-INFO` & `mkdocs-encryptcontent-plugin-2.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-encryptcontent-plugin
-Version: 2.5.2
+Version: 2.5.3
 Summary: A MkDocs plugin that encrypt/decrypt markdown content with AES
 Home-page: https://github.com/unverbuggt/mkdocs-encryptcontent-plugin
 Author: unverbuggt
 Author-email: unverbuggt@xn--rthlein-n2a.de
 License: MIT
 Description: # mkdocs-encryptcontent-plugin
         
@@ -28,18 +28,28 @@
         >
         > If a password is defined in an article or a page, it is always used even if there is a global password.
         >
         > If a password is defined as an empty character string, the content is not protected.
         
         ![encryptcontent_demo](https://user-images.githubusercontent.com/12155947/177001700-f0920d4b-0c41-4d11-8164-9f63d29d8a6a.gif)
         
-        # Todo for 2.6.x
+        # Version 3
         
-        * Rework password handling or inventory of some sort
-        * ...to be defined
+        Please check out the [pre-releases](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/releases) of version3:
+        
+        -  Introduce password inventory in mkdocs.yml or external yaml file, usable by `level` meta tag or `_global` #44.
+           - Allow multiple passwords per page #36.
+           - Allow username/password credentials
+           - Deprecation of `use_secret` as environment variables can be read by `!ENV` in password inventory
+        - The password is now hashed by PBKDF2 instead of MD5 #47.
+        - Allow special characters to be used in passwords (passwords are URLencoded).
+        - Allow signing of generated pages and files
+           - Check Ed25519 signatures with external canary script
+        
+        Please test and report issues. Thanks.
         
         # Table of Contents
         
           * [Installation](#installation)
           * [Usage](#usage)
             * [Global password protection](#global-password-protection)
             * [Secret from environment](#secret-from-environment)
@@ -73,15 +83,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-encryptcontent-plugin/
         python setup.py sdist bdist_wheel
-        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.2-py3-none-any.whl
+        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.3-py3-none-any.whl
         ```
         
         Enable the plugin in your `mkdocs.yml`:
         
         ```yaml
         plugins:
             - search: {}
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/README.md` & `mkdocs-encryptcontent-plugin-2.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,28 @@
 >
 > If a password is defined in an article or a page, it is always used even if there is a global password.
 >
 > If a password is defined as an empty character string, the content is not protected.
 
 ![encryptcontent_demo](https://user-images.githubusercontent.com/12155947/177001700-f0920d4b-0c41-4d11-8164-9f63d29d8a6a.gif)
 
-# Todo for 2.6.x
+# Version 3
 
-* Rework password handling or inventory of some sort
-* ...to be defined
+Please check out the [pre-releases](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/releases) of version3:
+
+-  Introduce password inventory in mkdocs.yml or external yaml file, usable by `level` meta tag or `_global` #44.
+   - Allow multiple passwords per page #36.
+   - Allow username/password credentials
+   - Deprecation of `use_secret` as environment variables can be read by `!ENV` in password inventory
+- The password is now hashed by PBKDF2 instead of MD5 #47.
+- Allow special characters to be used in passwords (passwords are URLencoded).
+- Allow signing of generated pages and files
+   - Check Ed25519 signatures with external canary script
+
+Please test and report issues. Thanks.
 
 # Table of Contents
 
   * [Installation](#installation)
   * [Usage](#usage)
     * [Global password protection](#global-password-protection)
     * [Secret from environment](#secret-from-environment)
@@ -65,15 +75,15 @@
 ```
 
 Install the package from source with pip:
 
 ```bash
 cd mkdocs-encryptcontent-plugin/
 python setup.py sdist bdist_wheel
-pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.2-py3-none-any.whl
+pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.3-py3-none-any.whl
 ```
 
 Enable the plugin in your `mkdocs.yml`:
 
 ```yaml
 plugins:
     - search: {}
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/lunr.js` & `mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/templates/search/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/main.js` & `mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/templates/search/main.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/worker.js` & `mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/contrib/templates/search/worker.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/decrypt-contents.tpl.js` & `mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/decrypt-contents.tpl.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,35 +1,25 @@
 /* encryptcontent/decrypt-contents.tpl.js */
 
-/* Strips the padding character from decrypted content. */
-function strip_padding(padded_content, padding_char) {
-    for (var i = padded_content.length; i > 0; i--) {
-        if (padded_content[i - 1] !== padding_char) {
-            return padded_content.slice(0, i);
-        }
-    }
-    return '';
-};
-
 /* Decrypts the content from the ciphertext bundle. */
 function decrypt_content(password, iv_b64, ciphertext_b64, padding_char) {
     var key = CryptoJS.MD5(password),
         iv = CryptoJS.enc.Base64.parse(iv_b64),
         ciphertext = CryptoJS.enc.Base64.parse(ciphertext_b64),
         bundle = {
             key: key,
             iv: iv,
             ciphertext: ciphertext
         };
     var plaintext = CryptoJS.AES.decrypt(bundle, key, {
         iv: iv,
-        padding: CryptoJS.pad.NoPadding
+        padding: CryptoJS.pad.Pkcs7
     });
     try {
-        return strip_padding(plaintext.toString(CryptoJS.enc.Utf8), padding_char);
+        return plaintext.toString(CryptoJS.enc.Utf8)
     } catch (err) {
         // encoding failed; wrong password
         return false;
     }
 };
 
 /* Split cyphertext bundle and try to decrypt it */
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/decrypt-form.tpl.html` & `mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/decrypt-form.tpl.html`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/plugin.py` & `mkdocs-encryptcontent-plugin-2.5.3/encryptcontent/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import base64
 import hashlib
 import logging
 import json
 import math
 from pathlib import Path
 from os.path import exists
-from Crypto import Random
 from jinja2 import Template
 from Crypto.Cipher import AES
+from Crypto.Random import get_random_bytes
+from Crypto.Util.Padding import pad
 from bs4 import BeautifulSoup
 from mkdocs.plugins import BasePlugin
 from mkdocs.config import config_options
 from urllib.parse import urlsplit
 from urllib.request import urlopen
 
 try:
@@ -22,15 +23,14 @@
 except ImportError:
     string_types = str
 
 JS_LIBRARIES = [
     ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/core.js','b55ae8027253d4d54c4f1ef3b6254646'],
     ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/enc-base64.js','f551ce1340a86e5edbfef4a6aefa798f'],
     ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/cipher-core.js','dfddc0e33faf7a794e0c3c140544490e'],
-    ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/pad-nopadding.js','e288e14e2cd299c3247120114e1178e6'],
     ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/md5.js','349498f298a6e6e6a85789d637e89109'],
     ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/aes.js','da81b91b1b57c279c29b3469649d9b86'],
 ]
 
 PLUGIN_DIR = os.path.dirname(os.path.realpath(__file__))
 
 SETTINGS = {
@@ -120,20 +120,20 @@
                     logger.error('Error downloading asset "' + filename.name + '" hash mismatch!')
                     os._exit(1)
 
     def __encrypt_text_aes__(self, text, password):
         """ Encrypts text with AES-256. """
         BLOCK_SIZE = 32
         PADDING_CHAR = b'^'
-        iv = Random.new().read(16)
+        iv = get_random_bytes(16)
         # key must be 32 bytes for AES-256, so the password is hashed with md5 first
         cipher = AES.new(self.__hash_md5__(password), AES.MODE_CBC, iv)
         plaintext = text.encode('utf-8')
         # plaintext must be padded to be a multiple of BLOCK_SIZE
-        plaintext_padded = plaintext + (BLOCK_SIZE - len(plaintext) % BLOCK_SIZE) * PADDING_CHAR
+        plaintext_padded = pad(plaintext, 16, style='pkcs7')
         ciphertext = cipher.encrypt(plaintext_padded)
         return (
             base64.b64encode(iv),
             base64.b64encode(ciphertext),
             PADDING_CHAR
         )
 
@@ -298,15 +298,15 @@
             self.config['mermaid2'] = False
         # Warn about deprecated features on Vervion 2.0.0
         deprecated_options_detected = False
 
         if deprecated_options_detected:
             logger.warning('DEPRECATED: Features marked as deprecated will be remove in next minor version !')
         # Enable experimental code .. :popcorn:
-        elif self.config['search_index'] == 'dynamically':
+        if self.config['search_index'] == 'dynamically':
             logger.info("EXPERIMENTAL search index encryption enabled.")
         self.setup['encrypted_something'] = {**self.config['inject'], **self.config['encrypted_something']} #add inject to encrypted_something
         # Get path to site in case of subdir in site_url
         self.setup['site_path'] = urlsplit(config.data["site_url"] or '/').path[1::]
 
         self.setup['search_plugin_found'] = False
         encryptcontent_plugin_found = False
@@ -349,14 +349,28 @@
                             config['theme'].dirs.append(path)
                             if 'search/main.js' not in config['extra_javascript']:
                                 config['extra_javascript'].append('search/main.js')
                             break
         except Exception as exp:
             logger.exception(exp)
 
+        # optionally download cryptojs
+        if self.config['selfhost'] and self.config['selfhost_download']:
+            logger.info('Downloading cryptojs for self-hosting (if needed)...')
+            if self.config['selfhost_dir']:
+                configpath = Path(config['config_file_path']).parents[0]
+                dlpath = configpath.joinpath(self.config['selfhost_dir'] + '/assets/javascripts/cryptojs/')
+            else:
+                dlpath = Path(config.data['docs_dir'] + '/assets/javascripts/cryptojs/')
+            dlpath.mkdir(parents=True, exist_ok=True)
+            for jsurl in JS_LIBRARIES:
+                dlurl = "https:" + jsurl[0]
+                filepath = dlpath.joinpath(jsurl[0].rsplit('/',1)[1])
+                self.__download_and_check__(filepath, dlurl, jsurl[1])
+
     def on_files(self, files, config, **kwargs):
         """
         The files event is called after the files collection is populated from the docs_dir.
         Use this event to add, remove, or alter files in the collection.
         Note that Page objects have not yet been associated with the file objects in the collection.
         Use Page Events to manipulate page specific data.
         """
@@ -644,28 +658,14 @@
                 with open(search_index_filename, "w") as f:
                     json.dump(search_entries, f)
             except:
                 logger.error('Search index needs modification, but could not write "search_index.json"!')
                 os._exit(1)
             logger.info('Modified search_index.')
 
-        # optionally download cryptojs
-        if self.config['selfhost'] and self.config['selfhost_download']:
-            logger.info('Downloading cryptojs for self-hosting (if needed)...')
-            if self.config['selfhost_dir']:
-                configpath = Path(config['config_file_path']).parents[0]
-                dlpath = configpath.joinpath(self.config['selfhost_dir'] + '/assets/javascripts/cryptojs/')
-            else:
-                dlpath = Path(config.data['docs_dir'] + '/assets/javascripts/cryptojs/')
-            dlpath.mkdir(parents=True, exist_ok=True)
-            for jsurl in JS_LIBRARIES:
-                dlurl = "https:" + jsurl[0]
-                filepath = dlpath.joinpath(jsurl[0].rsplit('/',1)[1])
-                self.__download_and_check__(filepath, dlurl, jsurl[1])
-
         passwords = set() #get all unique passwords
         for location in self.setup['locations'].keys():
             if not self.setup['locations'][location][1]:
                 passwords.add(self.setup['locations'][location][0])
         self.setup['locations'].clear()
         min_enttropy_spied_on, min_enttropy_secret = 0, 0
         for password in passwords:
@@ -673,9 +673,9 @@
             if min_enttropy_spied_on == 0 or enttropy_spied_on < min_enttropy_spied_on:
                 min_enttropy_spied_on = enttropy_spied_on
             if min_enttropy_secret == 0 or enttropy_secret < min_enttropy_secret:
                 min_enttropy_secret = enttropy_secret
         if min_enttropy_spied_on < 100 and min_enttropy_spied_on > 0:
             logger.warning('mkdocs-encryptcontent-plugin will always be vulnerable to brute-force attacks!'
                            ' Your weakest password only got {spied_on} bits of entropy, if someone watched you while typing'
-                           ' (and a maximum of {secret} bits total)!'.format(spied_on = math.ceil(enttropy_spied_on), secret = math.ceil(min_enttropy_secret))
+                           ' (and a maximum of {secret} bits total)!'.format(spied_on = math.ceil(min_enttropy_spied_on), secret = math.ceil(min_enttropy_secret))
                     )
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO` & `mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-encryptcontent-plugin
-Version: 2.5.2
+Version: 2.5.3
 Summary: A MkDocs plugin that encrypt/decrypt markdown content with AES
 Home-page: https://github.com/unverbuggt/mkdocs-encryptcontent-plugin
 Author: unverbuggt
 Author-email: unverbuggt@xn--rthlein-n2a.de
 License: MIT
 Description: # mkdocs-encryptcontent-plugin
         
@@ -28,18 +28,28 @@
         >
         > If a password is defined in an article or a page, it is always used even if there is a global password.
         >
         > If a password is defined as an empty character string, the content is not protected.
         
         ![encryptcontent_demo](https://user-images.githubusercontent.com/12155947/177001700-f0920d4b-0c41-4d11-8164-9f63d29d8a6a.gif)
         
-        # Todo for 2.6.x
+        # Version 3
         
-        * Rework password handling or inventory of some sort
-        * ...to be defined
+        Please check out the [pre-releases](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/releases) of version3:
+        
+        -  Introduce password inventory in mkdocs.yml or external yaml file, usable by `level` meta tag or `_global` #44.
+           - Allow multiple passwords per page #36.
+           - Allow username/password credentials
+           - Deprecation of `use_secret` as environment variables can be read by `!ENV` in password inventory
+        - The password is now hashed by PBKDF2 instead of MD5 #47.
+        - Allow special characters to be used in passwords (passwords are URLencoded).
+        - Allow signing of generated pages and files
+           - Check Ed25519 signatures with external canary script
+        
+        Please test and report issues. Thanks.
         
         # Table of Contents
         
           * [Installation](#installation)
           * [Usage](#usage)
             * [Global password protection](#global-password-protection)
             * [Secret from environment](#secret-from-environment)
@@ -73,15 +83,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-encryptcontent-plugin/
         python setup.py sdist bdist_wheel
-        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.2-py3-none-any.whl
+        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.3-py3-none-any.whl
         ```
         
         Enable the plugin in your `mkdocs.yml`:
         
         ```yaml
         plugins:
             - search: {}
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt` & `mkdocs-encryptcontent-plugin-2.5.3/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.2/setup.py` & `mkdocs-encryptcontent-plugin-2.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(file_path) as file:
         content = file.read()
     return content if content else 'no content read'
 
 
 setup(
     name='mkdocs-encryptcontent-plugin',
-    version='2.5.2',
+    version='2.5.3',
     author='unverbuggt',
     author_email='unverbuggt@xn--rthlein-n2a.de',
     description='A MkDocs plugin that encrypt/decrypt markdown content with AES',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown encrypt decrypt content',
     url='https://github.com/unverbuggt/mkdocs-encryptcontent-plugin',
```

