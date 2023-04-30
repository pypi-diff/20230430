# Comparing `tmp/aa-charlink-0.2.0.tar.gz` & `tmp/aa-charlink-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-charlink-0.2.0.tar", last modified: Fri Apr 21 13:07:54 2023, max compression
+gzip compressed data, was "aa-charlink-0.3.0.tar", last modified: Sun Apr 30 13:58:52 2023, max compression
```

## Comparing `aa-charlink-0.2.0.tar` & `aa-charlink-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/aa_charlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 13:07:54.000000 aa-charlink-0.2.0/aa_charlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/charlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/app_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/app_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/charlink/imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/corptools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/memberaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/miningtaxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/moonmining.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/moonstuff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/imports/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/charlink/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.594582 aa-charlink-0.2.0/charlink/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/charlink/templates/charlink/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/templates/charlink/charlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/charlink/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-21 13:07:42.000000 aa-charlink-0.2.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-04-21 13:07:54.598582 aa-charlink-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.168855 aa-charlink-0.3.0/aa_charlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:58:51.000000 aa-charlink-0.3.0/aa_charlink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 13:58:52.000000 aa-charlink-0.3.0/aa_charlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.168855 aa-charlink-0.3.0/charlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/app_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/app_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.168855 aa-charlink-0.3.0/charlink/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/charlink/imports/allianceauth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/allianceauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/allianceauth/corputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/corptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/memberaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/miningtaxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/moonmining.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/moonstuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/imports/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/charlink/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.164855 aa-charlink-0.3.0/charlink/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/charlink/templates/charlink/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/templates/charlink/charlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/charlink/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-30 13:58:37.000000 aa-charlink-0.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-04-30 13:58:52.172855 aa-charlink-0.3.0/setup.cfg
```

### Comparing `aa-charlink-0.2.0/LICENSE` & `aa-charlink-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.2.0/PKG-INFO` & `aa-charlink-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 0.2.0
+Version: 0.3.0
 Summary: Character Linker for Alliance Auth
 Home-page: https://github.com/Maestro-Zacht/aa-charlink
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_charlink,charlink,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-charlink-0.2.0/README.md` & `aa-charlink-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.2.0/aa_charlink.egg-info/PKG-INFO` & `aa-charlink-0.3.0/aa_charlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 0.2.0
+Version: 0.3.0
 Summary: Character Linker for Alliance Auth
 Home-page: https://github.com/Maestro-Zacht/aa-charlink
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_charlink,charlink,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-charlink-0.2.0/aa_charlink.egg-info/SOURCES.txt` & `aa-charlink-0.3.0/aa_charlink.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,9 +22,11 @@
 charlink/imports/__init__.py
 charlink/imports/corptools.py
 charlink/imports/memberaudit.py
 charlink/imports/miningtaxes.py
 charlink/imports/moonmining.py
 charlink/imports/moonstuff.py
 charlink/imports/structures.py
+charlink/imports/allianceauth/__init__.py
+charlink/imports/allianceauth/corputils.py
 charlink/migrations/__init__.py
 charlink/templates/charlink/charlink.html
```

### Comparing `aa-charlink-0.2.0/charlink/app_imports.py` & `aa-charlink-0.3.0/charlink/app_imports.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from importlib import import_module
 
 from django.conf import settings
 
 from allianceauth.services.hooks import get_extension_logger
+from allianceauth.authentication.models import CharacterOwnership
 
 logger = get_extension_logger(__name__)
 
 _supported_apps = {
     'add_character': {
         'field_label': 'Add Character (default)',
         'add_character': lambda request, token: None,
         'scopes': ['publicData'],
         'permissions': [],
+        'is_character_added': lambda character: CharacterOwnership.objects.filter(character=character).exists(),
     }
 }
 
 _imported = False
 
 
 def import_apps():
     global _imported
     if not _imported:
         for app in settings.INSTALLED_APPS:
-            try:
-                module = import_module(f'charlink.imports.{app}')
-            except ModuleNotFoundError:
-                pass
-            else:
-                _supported_apps[app] = {
-                    'field_label': module.field_label,
-                    'add_character': module.add_character,
-                    'scopes': module.scopes,
-                    'permissions': module.permissions,
-                }
+            if app != 'allianceauth':
+                try:
+                    module = import_module(f'charlink.imports.{app}')
+                except ModuleNotFoundError:
+                    logger.debug(f"Loading of {app} link: failed")
+                else:
+                    _supported_apps[app] = {
+                        'field_label': module.field_label,
+                        'add_character': module.add_character,
+                        'scopes': module.scopes,
+                        'permissions': module.permissions,
+                        'is_character_added': module.is_character_added,
+                    }
 
-                logger.debug(f"Loading of {app} link: success")
+                    logger.debug(f"Loading of {app} link: success")
 
         _imported = True
 
     return _supported_apps
```

### Comparing `aa-charlink-0.2.0/charlink/forms.py` & `aa-charlink-0.3.0/charlink/forms.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.2.0/charlink/imports/corptools.py` & `aa-charlink-0.3.0/charlink/imports/corptools.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,7 +11,11 @@
 permissions = []
 
 
 def add_character(request, token):
     CharacterAudit.objects.update_or_create(
         character=EveCharacter.objects.get_character_by_id(token.character_id))
     update_character.apply_async(args=[token.character_id], priority=6)
+
+
+def is_character_added(character: EveCharacter):
+    return CharacterAudit.objects.filter(character=character).exists()
```

### Comparing `aa-charlink-0.2.0/charlink/imports/memberaudit.py` & `aa-charlink-0.3.0/charlink/imports/memberaudit.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,7 +23,11 @@
         kwargs={"character_pk": character.pk},
         priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
     )
     if ComplianceGroupDesignation.objects.exists():
         tasks.update_compliance_groups_for_user.apply_async(
             args=[request.user.pk], priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
         )
+
+
+def is_character_added(character: EveCharacter):
+    return Character.objects.filter(eve_character=character).exists()
```

### Comparing `aa-charlink-0.2.0/charlink/imports/miningtaxes.py` & `aa-charlink-0.3.0/charlink/imports/miningtaxes.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,7 +13,11 @@
 
 
 def add_character(request, token):
     eve_character = EveCharacter.objects.get(character_id=token.character_id)
     with transaction.atomic():
         character, _ = Character.objects.update_or_create(eve_character=eve_character)
     tasks.update_character.delay(character_pk=character.pk)
+
+
+def is_character_added(character: EveCharacter):
+    return Character.objects.filter(eve_character=character).exists()
```

### Comparing `aa-charlink-0.2.0/charlink/imports/moonmining.py` & `aa-charlink-0.3.0/charlink/imports/moonmining.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from moonmining.models import Owner
 from moonmining import __title__, tasks
 from moonmining.app_settings import MOONMINING_ADMIN_NOTIFICATIONS_ENABLED
 
 from app_utils.messages import messages_plus
 from app_utils.allianceauth import notify_admins
 
-from allianceauth.eveonline.models import EveCorporationInfo
+from allianceauth.eveonline.models import EveCorporationInfo, EveCharacter
 
 field_label = __title__
 
 scopes = Owner.esi_scopes()
 
 permissions = ["moonmining.add_refinery_owner", "moonmining.basic_access"]
 
@@ -37,7 +37,13 @@
     messages_plus.success(request, f"Update of refineres started for {owner}.")
     if MOONMINING_ADMIN_NOTIFICATIONS_ENABLED:
         notify_admins(
             message=("%(corporation)s was added as new owner by %(user)s.")
             % {"corporation": owner, "user": request.user},
             title=f"{__title__}: Owner added: {owner}",
         )
+
+
+def is_character_added(character: EveCharacter):
+    return Owner.objects.filter(
+        character_ownership__character=character
+    ).exists()
```

### Comparing `aa-charlink-0.2.0/charlink/imports/structures.py` & `aa-charlink-0.3.0/charlink/imports/structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.utils import translation
 from django.utils.translation import gettext as _
 from django.utils.html import format_html
 
 from structures import __title__, tasks
-from structures.models import Owner, Webhook
+from structures.models import Owner, Webhook, OwnerCharacter
 from structures.app_settings import (
     STRUCTURES_ADMIN_NOTIFICATIONS_ENABLED,
     STRUCTURES_DEFAULT_LANGUAGE,
 )
 
 from app_utils.allianceauth import notify_admins
 from app_utils.messages import messages_plus
@@ -103,7 +103,13 @@
                         "character": token_char,
                         "corporation": owner,
                         "user": request.user.username,
                         "characters_count": owner.characters_count(),
                     },
                     title=_("%s: Character added to: %s") % (__title__, owner),
                 )
+
+
+def is_character_added(character: EveCharacter):
+    return OwnerCharacter.objects.filter(
+        character_ownership__character=character
+    ).exists()
```

### Comparing `aa-charlink-0.2.0/charlink/templates/charlink/charlink.html` & `aa-charlink-0.3.0/charlink/templates/charlink/charlink.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,193 @@
 00000000: 7b25 2065 7874 656e 6473 2027 616c 6c69  {% extends 'alli
 00000010: 616e 6365 6175 7468 2f62 6173 652e 6874  anceauth/base.ht
 00000020: 6d6c 2720 257d 0a7b 2520 6c6f 6164 2062  ml' %}.{% load b
 00000030: 6f6f 7473 7472 6170 2025 7d0a 0a7b 2520  ootstrap %}..{% 
 00000040: 626c 6f63 6b20 7061 6765 5f74 6974 6c65  block page_title
 00000050: 2025 7d43 6861 726c 696e 6b7b 2520 656e   %}Charlink{% en
 00000060: 6462 6c6f 636b 2070 6167 655f 7469 746c  dblock page_titl
-00000070: 6520 257d 0a0a 7b25 2062 6c6f 636b 2063  e %}..{% block c
-00000080: 6f6e 7465 6e74 2025 7d0a 2020 2020 3c64  ontent %}.    <d
-00000090: 6976 2063 6c61 7373 3d22 636f 6c2d 6c67  iv class="col-lg
-000000a0: 2d31 3222 3e0a 2020 2020 2020 2020 3c68  -12">.        <h
-000000b0: 3120 636c 6173 733d 2270 6167 652d 6865  1 class="page-he
-000000c0: 6164 6572 2074 6578 742d 6365 6e74 6572  ader text-center
-000000d0: 223e 4368 6172 6163 7465 7220 4c69 6e6b  ">Character Link
-000000e0: 696e 673c 2f68 313e 0a20 2020 2020 2020  ing</h1>.       
-000000f0: 203c 6469 7620 636c 6173 733d 2270 616e   <div class="pan
-00000100: 656c 2070 616e 656c 2d70 7269 6d61 7279  el panel-primary
-00000110: 2074 6578 742d 6365 6e74 6572 223e 0a20   text-center">. 
-00000120: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000130: 636c 6173 733d 2270 616e 656c 2d68 6561  class="panel-hea
-00000140: 6469 6e67 223e 0a20 2020 2020 2020 2020  ding">.         
-00000150: 2020 2020 2020 203c 6833 2063 6c61 7373         <h3 class
-00000160: 3d22 7061 6e65 6c2d 7469 746c 6520 7465  ="panel-title te
-00000170: 7874 2d63 656e 7465 7222 3e4c 6f67 696e  xt-center">Login
-00000180: 2046 6f72 6d3c 2f68 333e 0a20 2020 2020   Form</h3>.     
-00000190: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000001a0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000001b0: 6c61 7373 3d22 7061 6e65 6c2d 626f 6479  lass="panel-body
-000001c0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000001d0: 2020 203c 703e 5365 6c65 6374 2074 6865     <p>Select the
-000001e0: 2061 7070 7320 796f 7520 7761 6e74 2074   apps you want t
-000001f0: 6f20 6c69 6e6b 2066 726f 6d20 7468 6520  o link from the 
-00000200: 6c69 7374 2e20 596f 7520 7769 6c6c 2062  list. You will b
-00000210: 6520 7265 6469 7265 6374 6564 2074 6f20  e redirected to 
-00000220: 6576 656f 6e6c 696e 6520 7765 6273 6974  eveonline websit
-00000230: 6520 746f 2061 7574 6865 6e74 6963 6174  e to authenticat
-00000240: 6520 616e 6420 7072 6f76 6964 6520 7468  e and provide th
-00000250: 6520 746f 6b65 6e20 7769 7468 2061 6c6c  e token with all
-00000260: 2074 6865 2073 636f 7065 7320 6e65 6564   the scopes need
-00000270: 6564 2e3c 2f70 3e0a 2020 2020 2020 2020  ed.</p>.        
-00000280: 2020 2020 2020 2020 3c62 723e 0a20 2020          <br>.   
-00000290: 2020 2020 2020 2020 2020 2020 203c 666f               <fo
-000002a0: 726d 206d 6574 686f 643d 2270 6f73 7422  rm method="post"
-000002b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000002c0: 2020 2020 2020 7b25 2063 7372 665f 746f        {% csrf_to
-000002d0: 6b65 6e20 257d 0a20 2020 2020 2020 2020  ken %}.         
-000002e0: 2020 2020 2020 2020 2020 207b 7b20 666f             {{ fo
-000002f0: 726d 7c62 6f6f 7473 7472 6170 207d 7d0a  rm|bootstrap }}.
-00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000310: 2020 2020 3c62 7574 746f 6e20 7479 7065      <button type
-00000320: 3d22 7375 626d 6974 2220 636c 6173 733d  ="submit" class=
-00000330: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
-00000340: 223e 4c6f 6769 6e3c 2f62 7574 746f 6e3e  ">Login</button>
+00000070: 6520 257d 0a0a 7b25 2062 6c6f 636b 2065  e %}..{% block e
+00000080: 7874 7261 5f63 7373 2025 7d0a 2020 2020  xtra_css %}.    
+00000090: 3c73 7479 6c65 3e0a 2020 2020 2020 2020  <style>.        
+000000a0: 2e67 6c79 7068 6963 6f6e 2d6f 6b20 7b0a  .glyphicon-ok {.
+000000b0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+000000c0: 723a 2067 7265 656e 3b0a 2020 2020 2020  r: green;.      
+000000d0: 2020 7d0a 0a20 2020 2020 2020 202e 676c    }..        .gl
+000000e0: 7970 6869 636f 6e2d 7265 6d6f 7665 207b  yphicon-remove {
+000000f0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+00000100: 6f72 3a20 7265 643b 0a20 2020 2020 2020  or: red;.       
+00000110: 207d 0a20 2020 203c 2f73 7479 6c65 3e0a   }.    </style>.
+00000120: 7b25 2065 6e64 626c 6f63 6b20 6578 7472  {% endblock extr
+00000130: 615f 6373 7320 257d 0a0a 7b25 2062 6c6f  a_css %}..{% blo
+00000140: 636b 2063 6f6e 7465 6e74 2025 7d0a 2020  ck content %}.  
+00000150: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00000160: 6c2d 6c67 2d31 3222 3e0a 2020 2020 2020  l-lg-12">.      
+00000170: 2020 3c68 3120 636c 6173 733d 2270 6167    <h1 class="pag
+00000180: 652d 6865 6164 6572 2074 6578 742d 6365  e-header text-ce
+00000190: 6e74 6572 223e 4368 6172 6163 7465 7220  nter">Character 
+000001a0: 4c69 6e6b 696e 673c 2f68 313e 0a20 2020  Linking</h1>.   
+000001b0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000001c0: 2270 616e 656c 2070 616e 656c 2d70 7269  "panel panel-pri
+000001d0: 6d61 7279 2074 6578 742d 6365 6e74 6572  mary text-center
+000001e0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+000001f0: 6469 7620 636c 6173 733d 2270 616e 656c  div class="panel
+00000200: 2d68 6561 6469 6e67 223e 0a20 2020 2020  -heading">.     
+00000210: 2020 2020 2020 2020 2020 203c 6833 2063             <h3 c
+00000220: 6c61 7373 3d22 7061 6e65 6c2d 7469 746c  lass="panel-titl
+00000230: 6520 7465 7874 2d63 656e 7465 7222 3e4c  e text-center">L
+00000240: 6f67 696e 2046 6f72 6d3c 2f68 333e 0a20  ogin Form</h3>. 
+00000250: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000260: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+00000270: 6976 2063 6c61 7373 3d22 7061 6e65 6c2d  iv class="panel-
+00000280: 626f 6479 223e 0a20 2020 2020 2020 2020  body">.         
+00000290: 2020 2020 2020 203c 703e 5365 6c65 6374         <p>Select
+000002a0: 2074 6865 2061 7070 7320 796f 7520 7761   the apps you wa
+000002b0: 6e74 2074 6f20 6c69 6e6b 2066 726f 6d20  nt to link from 
+000002c0: 7468 6520 6c69 7374 2e20 596f 7520 7769  the list. You wi
+000002d0: 6c6c 2062 6520 7265 6469 7265 6374 6564  ll be redirected
+000002e0: 2074 6f20 6576 656f 6e6c 696e 6520 7765   to eveonline we
+000002f0: 6273 6974 6520 746f 2061 7574 6865 6e74  bsite to authent
+00000300: 6963 6174 6520 616e 6420 7072 6f76 6964  icate and provid
+00000310: 6520 7468 6520 746f 6b65 6e20 7769 7468  e the token with
+00000320: 2061 6c6c 2074 6865 2073 636f 7065 7320   all the scopes 
+00000330: 6e65 6564 6564 2e3c 2f70 3e0a 2020 2020  needed.</p>.    
+00000340: 2020 2020 2020 2020 2020 2020 3c62 723e              <br>
 00000350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000360: 203c 2f66 6f72 6d3e 0a20 2020 2020 2020   </form>.       
-00000370: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000380: 2020 2020 3c2f 6469 763e 0a0a 2020 2020      </div>..    
-00000390: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000003a0: 7061 6e65 6c20 7061 6e65 6c2d 7375 6363  panel panel-succ
-000003b0: 6573 7320 7465 7874 2d63 656e 7465 7222  ess text-center"
-000003c0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
-000003d0: 6976 2063 6c61 7373 3d22 7061 6e65 6c2d  iv class="panel-
-000003e0: 6865 6164 696e 6722 3e0a 2020 2020 2020  heading">.      
-000003f0: 2020 2020 2020 2020 2020 3c68 3320 636c            <h3 cl
-00000400: 6173 733d 2270 616e 656c 2d74 6974 6c65  ass="panel-title
-00000410: 2074 6578 742d 6365 6e74 6572 223e 4170   text-center">Ap
-00000420: 706c 6963 6174 696f 6e73 2049 6e66 6f3c  plications Info<
-00000430: 2f68 333e 0a20 2020 2020 2020 2020 2020  /h3>.           
-00000440: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00000450: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000460: 7061 6e65 6c2d 626f 6479 223e 0a20 2020  panel-body">.   
-00000470: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00000480: 666f 7220 6170 7020 696e 2061 7070 7320  for app in apps 
-00000490: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000004a0: 2020 2020 2020 203c 7370 616e 3e7b 7b20         <span>{{ 
-000004b0: 6170 702e 6669 656c 645f 6c61 6265 6c20  app.field_label 
-000004c0: 7d7d 3c2f 7370 616e 3e0a 2020 2020 2020  }}</span>.      
-000004d0: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
-000004e0: 723e 3c62 723e 0a20 2020 2020 2020 2020  r><br>.         
-000004f0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
-00000500: 3e53 636f 7065 733a 3c2f 7370 616e 3e0a  >Scopes:</span>.
-00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000520: 2020 2020 7b7b 2061 7070 2e73 636f 7065      {{ app.scope
-00000530: 737c 756e 6f72 6465 7265 645f 6c69 7374  s|unordered_list
-00000540: 7c73 6166 6520 7d7d 0a20 2020 2020 2020  |safe }}.       
-00000550: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00000560: 6966 206e 6f74 2066 6f72 6c6f 6f70 2e6c  if not forloop.l
-00000570: 6173 7420 257d 3c68 723e 7b25 2065 6e64  ast %}<hr>{% end
-00000580: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-00000590: 2020 2020 2020 7b25 2065 6e64 666f 7220        {% endfor 
-000005a0: 257d 0a20 2020 2020 2020 2020 2020 203c  %}.            <
-000005b0: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
-000005c0: 6469 763e 0a20 2020 203c 2f64 6976 3e0a  div>.    </div>.
-000005d0: 7b25 2065 6e64 626c 6f63 6b20 636f 6e74  {% endblock cont
-000005e0: 656e 7420 257d                           ent %}
+00000360: 203c 666f 726d 206d 6574 686f 643d 2270   <form method="p
+00000370: 6f73 7422 3e0a 2020 2020 2020 2020 2020  ost">.          
+00000380: 2020 2020 2020 2020 2020 7b25 2063 7372            {% csr
+00000390: 665f 746f 6b65 6e20 257d 0a20 2020 2020  f_token %}.     
+000003a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000003b0: 7b20 666f 726d 7c62 6f6f 7473 7472 6170  { form|bootstrap
+000003c0: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
+000003d0: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
+000003e0: 7479 7065 3d22 7375 626d 6974 2220 636c  type="submit" cl
+000003f0: 6173 733d 2262 746e 2062 746e 2d70 7269  ass="btn btn-pri
+00000400: 6d61 7279 223e 4c6f 6769 6e3c 2f62 7574  mary">Login</but
+00000410: 746f 6e3e 0a20 2020 2020 2020 2020 2020  ton>.           
+00000420: 2020 2020 203c 2f66 6f72 6d3e 0a20 2020       </form>.   
+00000430: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00000440: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
+00000450: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000460: 7373 3d22 7061 6e65 6c20 7061 6e65 6c2d  ss="panel panel-
+00000470: 696e 666f 2074 6578 742d 6365 6e74 6572  info text-center
+00000480: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00000490: 6469 7620 636c 6173 733d 2270 616e 656c  div class="panel
+000004a0: 2d68 6561 6469 6e67 223e 0a20 2020 2020  -heading">.     
+000004b0: 2020 2020 2020 2020 2020 203c 6833 2063             <h3 c
+000004c0: 6c61 7373 3d22 7061 6e65 6c2d 7469 746c  lass="panel-titl
+000004d0: 6520 7465 7874 2d63 656e 7465 7222 3e4c  e text-center">L
+000004e0: 696e 6b65 6420 4368 6172 6163 7465 7273  inked Characters
+000004f0: 3c2f 6833 3e0a 2020 2020 2020 2020 2020  </h3>.          
+00000500: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000510: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000520: 2270 616e 656c 2d62 6f64 7922 3e0a 2020  "panel-body">.  
+00000530: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+00000540: 6162 6c65 2063 6c61 7373 3d22 7461 626c  able class="tabl
+00000550: 6520 7461 626c 652d 6161 223e 0a20 2020  e table-aa">.   
+00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000570: 203c 7468 6561 643e 0a20 2020 2020 2020   <thead>.       
+00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000590: 203c 7468 2063 6c61 7373 3d22 7465 7874   <th class="text
+000005a0: 2d63 656e 7465 7222 3e43 6861 7261 6374  -center">Charact
+000005b0: 6572 3c2f 7468 3e0a 2020 2020 2020 2020  er</th>.        
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 7b25 2066 6f72 2061 7070 2069 6e20 6368  {% for app in ch
+000005e0: 6172 6163 7465 7273 5f61 6464 6564 2e61  aracters_added.a
+000005f0: 7070 7320 257d 0a20 2020 2020 2020 2020  pps %}.         
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 2020 203c 7468 2073 636f 7065 3d22 726f     <th scope="ro
+00000620: 7722 2063 6c61 7373 3d22 7465 7874 2d63  w" class="text-c
+00000630: 656e 7465 7222 3e7b 7b20 6170 7020 7d7d  enter">{{ app }}
+00000640: 3c2f 7468 3e0a 2020 2020 2020 2020 2020  </th>.          
+00000650: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00000660: 2065 6e64 666f 7220 257d 0a20 2020 2020   endfor %}.     
+00000670: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000680: 2f74 6865 6164 3e0a 2020 2020 2020 2020  /thead>.        
+00000690: 2020 2020 2020 2020 2020 2020 3c74 626f              <tbo
+000006a0: 6479 3e0a 2020 2020 2020 2020 2020 2020  dy>.            
+000006b0: 2020 2020 2020 2020 2020 2020 7b25 2066              {% f
+000006c0: 6f72 2063 6861 722c 2061 7070 5f6c 6973  or char, app_lis
+000006d0: 7420 696e 2063 6861 7261 6374 6572 735f  t in characters_
+000006e0: 6164 6465 642e 6368 6172 6163 7465 7273  added.characters
+000006f0: 2e69 7465 6d73 2025 7d0a 2020 2020 2020  .items %}.      
+00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000710: 2020 2020 2020 3c74 723e 0a20 2020 2020        <tr>.     
+00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000730: 2020 2020 2020 2020 2020 203c 7464 3e7b             <td>{
+00000740: 7b20 6368 6172 207d 7d3c 2f74 643e 0a20  { char }}</td>. 
+00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000760: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000770: 2520 666f 7220 6973 5f61 6464 6564 2069  % for is_added i
+00000780: 6e20 6170 705f 6c69 7374 2025 7d0a 2020  n app_list %}.  
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2020 7b25 2069 6620 6973 5f61 6464 6564    {% if is_added
+000007c0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007e0: 2020 2020 2020 2020 2020 2020 3c74 643e              <td>
+000007f0: 3c73 7061 6e20 636c 6173 733d 2267 6c79  <span class="gly
+00000800: 7068 6963 6f6e 2067 6c79 7068 6963 6f6e  phicon glyphicon
+00000810: 2d6f 6b22 3e3c 2f73 7061 6e3e 3c2f 7464  -ok"></span></td
+00000820: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000840: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
+00000850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2020 2020 2020 2020 203c 7464 3e3c 7370           <td><sp
+00000880: 616e 2063 6c61 7373 3d22 676c 7970 6869  an class="glyphi
+00000890: 636f 6e20 676c 7970 6869 636f 6e2d 7265  con glyphicon-re
+000008a0: 6d6f 7665 223e 3c2f 7370 616e 3e3c 2f74  move"></span></t
+000008b0: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000008e0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 2020 207b 2520 656e 6466 6f72 2025 7d0a     {% endfor %}.
+00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000920: 2020 2020 2020 2020 2020 2020 3c2f 7472              </tr
+00000930: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000940: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00000950: 666f 7220 257d 0a20 2020 2020 2020 2020  for %}.         
+00000960: 2020 2020 2020 2020 2020 203c 2f74 626f             </tbo
+00000970: 6479 3e0a 2020 2020 2020 2020 2020 2020  dy>.            
+00000980: 2020 2020 3c2f 7461 626c 653e 0a20 2020      </table>.   
+00000990: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+000009a0: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
+000009b0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000009c0: 7373 3d22 7061 6e65 6c20 7061 6e65 6c2d  ss="panel panel-
+000009d0: 7375 6363 6573 7320 7465 7874 2d63 656e  success text-cen
+000009e0: 7465 7222 3e0a 2020 2020 2020 2020 2020  ter">.          
+000009f0: 2020 3c64 6976 2063 6c61 7373 3d22 7061    <div class="pa
+00000a00: 6e65 6c2d 6865 6164 696e 6722 3e0a 2020  nel-heading">.  
+00000a10: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
+00000a20: 3320 636c 6173 733d 2270 616e 656c 2d74  3 class="panel-t
+00000a30: 6974 6c65 2074 6578 742d 6365 6e74 6572  itle text-center
+00000a40: 223e 4170 706c 6963 6174 696f 6e73 2049  ">Applications I
+00000a50: 6e66 6f3c 2f68 333e 0a20 2020 2020 2020  nfo</h3>.       
+00000a60: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000a70: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000a80: 7373 3d22 7061 6e65 6c2d 626f 6479 223e  ss="panel-body">
+00000a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000aa0: 207b 2520 666f 7220 6170 7020 696e 2061   {% for app in a
+00000ab0: 7070 7320 257d 0a20 2020 2020 2020 2020  pps %}.         
+00000ac0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00000ad0: 3e7b 7b20 6170 702e 6669 656c 645f 6c61  >{{ app.field_la
+00000ae0: 6265 6c20 7d7d 3c2f 7370 616e 3e0a 2020  bel }}</span>.  
+00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b00: 2020 3c62 723e 3c62 723e 0a20 2020 2020    <br><br>.     
+00000b10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000b20: 7370 616e 3e53 636f 7065 733a 3c2f 7370  span>Scopes:</sp
+00000b30: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
+00000b40: 2020 2020 2020 2020 7b7b 2061 7070 2e73          {{ app.s
+00000b50: 636f 7065 737c 756e 6f72 6465 7265 645f  copes|unordered_
+00000b60: 6c69 7374 7c73 6166 6520 7d7d 0a20 2020  list|safe }}.   
+00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b80: 207b 2520 6966 206e 6f74 2066 6f72 6c6f   {% if not forlo
+00000b90: 6f70 2e6c 6173 7420 257d 3c68 723e 7b25  op.last %}<hr>{%
+00000ba0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+00000bb0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00000bc0: 666f 7220 257d 0a20 2020 2020 2020 2020  for %}.         
+00000bd0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000be0: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
+00000bf0: 6976 3e0a 7b25 2065 6e64 626c 6f63 6b20  iv>.{% endblock 
+00000c00: 636f 6e74 656e 7420 257d                 content %}
```

### Comparing `aa-charlink-0.2.0/charlink/views.py` & `aa-charlink-0.3.0/charlink/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.shortcuts import render, redirect
 from django.contrib.auth.decorators import login_required
 from django.contrib import messages
 
 from allianceauth.services.hooks import get_extension_logger
+from allianceauth.eveonline.models import EveCharacter
 
 from .forms import LinkForm
 from .app_imports import import_apps
 from .decorators import charlink
 from .app_settings import CHARLINK_IGNORE_APPS
 
 logger = get_extension_logger(__name__)
@@ -36,17 +37,38 @@
             }
 
             return redirect('charlink:login')
 
     else:
         form = LinkForm(request.user)
 
+    characters = EveCharacter.objects.filter(character_ownership__user=request.user)
+
+    characters_added = {
+        'apps': [data['field_label'] for app, data in imported_apps.items() if app not in CHARLINK_IGNORE_APPS and request.user.has_perms(data['permissions'])],
+        'characters': {},
+    }
+
+    # for app, data in imported_apps.items():
+    #     if app not in CHARLINK_IGNORE_APPS and request.user.has_perms(data['permissions']):
+    #         for character in characters:
+    #             setattr(character, f'has_{app}', data['has_character'](character))
+
+    for character in characters:
+        characters_added['characters'][character.character_name] = []
+        for app, data in imported_apps.items():
+            if app not in CHARLINK_IGNORE_APPS and request.user.has_perms(data['permissions']):
+                characters_added['characters'][character.character_name].append(
+                    data['is_character_added'](character)
+                )
+
     context = {
         'form': form,
-        'apps': [data for app, data in imported_apps.items() if app != 'add_character' and app not in CHARLINK_IGNORE_APPS and request.user.has_perms(data['permissions'])],
+        'apps': [data for app, data in imported_apps.items() if app not in CHARLINK_IGNORE_APPS and request.user.has_perms(data['permissions'])],
+        'characters_added': characters_added,
     }
 
     return render(request, 'charlink/charlink.html', context=context)
 
 
 @login_required
 @charlink
@@ -61,8 +83,8 @@
                 imported_apps[app]['add_character'](request, token)
             except Exception as e:
                 logger.exception(e)
                 messages.error(request, f"Failed to add character to {imported_apps[app]['field_label']}")
             else:
                 messages.success(request, f"Character successfully added to {imported_apps[app]['field_label']}")
 
-    return redirect('authentication:dashboard')
+    return redirect('charlink:index')
```

### Comparing `aa-charlink-0.2.0/setup.cfg` & `aa-charlink-0.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.3.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
```

