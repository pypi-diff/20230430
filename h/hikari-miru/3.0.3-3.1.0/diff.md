# Comparing `tmp/hikari-miru-3.0.3.tar.gz` & `tmp/hikari-miru-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari-miru-3.0.3.tar", last modified: Mon Apr  3 10:44:21 2023, max compression
+gzip compressed data, was "hikari-miru-3.1.0.tar", last modified: Sun Apr 30 15:05:30 2023, max compression
```

## Comparing `hikari-miru-3.0.3.tar` & `hikari-miru-3.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.157258 hikari-miru-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-03 10:44:21.157258 hikari-miru-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/doc_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.153257 hikari-miru-3.0.3/hikari_miru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-03 10:44:21.000000 hikari-miru-3.0.3/hikari_miru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-03 10:44:21.000000 hikari-miru-3.0.3/hikari_miru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 10:44:21.000000 hikari-miru-3.0.3/hikari_miru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 10:44:20.000000 hikari-miru-3.0.3/hikari_miru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-03 10:44:21.000000 hikari-miru-3.0.3/hikari_miru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-03 10:44:21.000000 hikari-miru-3.0.3/hikari_miru.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.153257 hikari-miru-3.0.3/miru/
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.153257 hikari-miru-3.0.3/miru/abc/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/abc/item.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/abc/item_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.157258 hikari-miru-3.0.3/miru/context/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/context/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/context/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/context/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.149257 hikari-miru-3.0.3/miru/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.157258 hikari-miru-3.0.3/miru/ext/nav/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/ext/nav/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/ext/nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/ext/nav/items.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/ext/nav/navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/ext/nav/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.157258 hikari-miru-3.0.3/miru/ext/nav/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/ext/nav/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/ext/nav/utils/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:44:21.157258 hikari-miru-3.0.3/miru/select/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/select/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/select/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/select/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/select/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/select/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/select/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/text_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/miru/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 10:44:21.161258 hikari-miru-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-03 10:44:05.000000 hikari-miru-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.184303 hikari-miru-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-30 15:05:30.184303 hikari-miru-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.176303 hikari-miru-3.1.0/hikari_miru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-30 15:05:30.000000 hikari-miru-3.1.0/hikari_miru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-30 15:05:30.000000 hikari-miru-3.1.0/hikari_miru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 15:05:30.000000 hikari-miru-3.1.0/hikari_miru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 15:05:29.000000 hikari-miru-3.1.0/hikari_miru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-30 15:05:30.000000 hikari-miru-3.1.0/hikari_miru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 15:05:30.000000 hikari-miru-3.1.0/hikari_miru.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.180303 hikari-miru-3.1.0/miru/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.180303 hikari-miru-3.1.0/miru/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/abc/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/abc/item_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.180303 hikari-miru-3.1.0/miru/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/context/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/context/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/context/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.164302 hikari-miru-3.1.0/miru/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.180303 hikari-miru-3.1.0/miru/ext/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/ext/nav/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/ext/nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/ext/nav/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/ext/nav/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/ext/nav/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.184303 hikari-miru-3.1.0/miru/ext/nav/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/ext/nav/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/ext/nav/utils/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 15:05:30.184303 hikari-miru-3.1.0/miru/select/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/select/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/select/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/select/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/select/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/select/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/select/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/text_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/miru/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 15:05:30.184303 hikari-miru-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-30 15:05:18.000000 hikari-miru-3.1.0/setup.py
```

### Comparing `hikari-miru-3.0.3/LICENSE` & `hikari-miru-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/PKG-INFO` & `hikari-miru-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-miru
-Version: 3.0.3
+Version: 3.1.0
 Summary: An alternative component handler for hikari, inspired by discord.py's views.
 Home-page: https://github.com/HyperGH/hikari-miru
 Author: HyperGH
 Author-email: 46067571+HyperGH@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
@@ -63,15 +63,15 @@
     async def paper_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         await ctx.respond("Scissors!")
 
     @miru.button(label="Scissors", emoji="\N{BLACK SCISSORS}", style=hikari.ButtonStyle.PRIMARY)
     async def scissors_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         await ctx.respond("Rock!")
 
-    @miru.button(emoji="\N{BLACK SQUARE FOR STOP}", style=hikari.ButtonStyle.DANGER, row=2)
+    @miru.button(emoji="\N{BLACK SQUARE FOR STOP}", style=hikari.ButtonStyle.DANGER, row=1)
     async def stop_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         self.stop() # Stop listening for interactions
 
 
 bot = hikari.GatewayBot(token="...")
 miru.install(bot) # Load miru and attach it to the bot instance.
```

### Comparing `hikari-miru-3.0.3/README.md` & `hikari-miru-3.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     async def paper_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         await ctx.respond("Scissors!")
 
     @miru.button(label="Scissors", emoji="\N{BLACK SCISSORS}", style=hikari.ButtonStyle.PRIMARY)
     async def scissors_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         await ctx.respond("Rock!")
 
-    @miru.button(emoji="\N{BLACK SQUARE FOR STOP}", style=hikari.ButtonStyle.DANGER, row=2)
+    @miru.button(emoji="\N{BLACK SQUARE FOR STOP}", style=hikari.ButtonStyle.DANGER, row=1)
     async def stop_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         self.stop() # Stop listening for interactions
 
 
 bot = hikari.GatewayBot(token="...")
 miru.install(bot) # Load miru and attach it to the bot instance.
```

### Comparing `hikari-miru-3.0.3/hikari_miru.egg-info/PKG-INFO` & `hikari-miru-3.1.0/hikari_miru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-miru
-Version: 3.0.3
+Version: 3.1.0
 Summary: An alternative component handler for hikari, inspired by discord.py's views.
 Home-page: https://github.com/HyperGH/hikari-miru
 Author: HyperGH
 Author-email: 46067571+HyperGH@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
@@ -63,15 +63,15 @@
     async def paper_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         await ctx.respond("Scissors!")
 
     @miru.button(label="Scissors", emoji="\N{BLACK SCISSORS}", style=hikari.ButtonStyle.PRIMARY)
     async def scissors_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         await ctx.respond("Rock!")
 
-    @miru.button(emoji="\N{BLACK SQUARE FOR STOP}", style=hikari.ButtonStyle.DANGER, row=2)
+    @miru.button(emoji="\N{BLACK SQUARE FOR STOP}", style=hikari.ButtonStyle.DANGER, row=1)
     async def stop_button(self, button: miru.Button, ctx: miru.ViewContext) -> None:
         self.stop() # Stop listening for interactions
 
 
 bot = hikari.GatewayBot(token="...")
 miru.install(bot) # Load miru and attach it to the bot instance.
```

### Comparing `hikari-miru-3.0.3/hikari_miru.egg-info/SOURCES.txt` & `hikari-miru-3.1.0/hikari_miru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/__init__.py` & `hikari-miru-3.1.0/miru/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "mentionable_select",
     "TextInput",
     "MiruAware",
     "View",
     "get_view",
 )
 
-__version__ = "3.0.3"
+__version__ = "3.1.0"
 
 # MIT License
 #
 # Copyright (c) 2022-present HyperGH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `hikari-miru-3.0.3/miru/__main__.py` & `hikari-miru-3.1.0/miru/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/abc/__init__.py` & `hikari-miru-3.1.0/miru/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/abc/item.py` & `hikari-miru-3.1.0/miru/abc/item.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,34 +23,53 @@
 
 
 class Item(abc.ABC, t.Generic[BuilderT]):
     """
     An abstract base class for all components. Cannot be directly instantiated.
     """
 
-    def __init__(self, *, custom_id: t.Optional[str] = None, row: t.Optional[int] = None) -> None:
+    def __init__(
+        self, *, custom_id: t.Optional[str] = None, row: t.Optional[int] = None, position: t.Optional[int] = None
+    ) -> None:
         self._rendered_row: t.Optional[int] = None
         """The row the item was placed at when rendered. None if this item was not sent to a message yet."""
 
         self.row = row
         """The row the item should occupy. Leave as None for automatic placement."""
 
+        self.position = position
+        """The position of the item within the row it occupies. Leave as None for automatic placement."""
+
         self._width: int = 1
         """The relative width of the item. 5 takes up a whole row."""
 
         self.custom_id = custom_id  # type: ignore[assignment]
         """The Discord custom_id of the item."""
 
         self._is_persistent: bool = bool(custom_id)
         """If True, the custom_id was provided by the user, and not randomly generated."""
 
         self._handler: t.Optional[ItemHandler[BuilderT]] = None
         """The handler the item was added to, if any."""
 
     @property
+    def position(self) -> t.Optional[int]:
+        """
+        The position of the item within the row it occupies.
+        """
+        return self._position
+
+    @position.setter
+    def position(self, value: t.Optional[int]) -> None:
+        if value is None or (self.width - 1) >= value >= 0:
+            self._position = value
+        else:
+            raise ValueError(f"Position of item {type(self).__name__} must be between 0 and {self.width-1}.")
+
+    @property
     def row(self) -> t.Optional[int]:
         """
         The row the item should occupy. Leave as None for automatic placement.
         """
         return self._row
 
     @row.setter
@@ -109,17 +128,22 @@
 
 class ViewItem(Item[hikari.impl.MessageActionRowBuilder], abc.ABC):
     """
     An abstract base class for view components. Cannot be directly instantiated.
     """
 
     def __init__(
-        self, *, custom_id: t.Optional[str] = None, row: t.Optional[int] = None, disabled: bool = False
+        self,
+        *,
+        custom_id: t.Optional[str] = None,
+        row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
+        disabled: bool = False,
     ) -> None:
-        super().__init__(custom_id=custom_id, row=row)
+        super().__init__(custom_id=custom_id, row=row, position=position)
         self._handler: t.Optional[View] = None
         self._disabled: bool = disabled
 
     @property
     def view(self) -> View:
         """
         The view this item is attached to.
@@ -166,17 +190,22 @@
 
 class ModalItem(Item[hikari.impl.ModalActionRowBuilder], abc.ABC):
     """
     An abstract base class for modal components. Cannot be directly instantiated.
     """
 
     def __init__(
-        self, *, custom_id: t.Optional[str] = None, row: t.Optional[int] = None, required: bool = False
+        self,
+        *,
+        custom_id: t.Optional[str] = None,
+        row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
+        required: bool = False,
     ) -> None:
-        super().__init__(custom_id=custom_id, row=row)
+        super().__init__(custom_id=custom_id, row=row, position=position)
         self._handler: t.Optional[Modal] = None
         self._required: bool = required
 
     @property
     def modal(self) -> t.Optional[Modal]:
         """
         The modal this item is attached to.
```

### Comparing `hikari-miru-3.0.3/miru/abc/item_handler.py` & `hikari-miru-3.1.0/miru/abc/item_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,16 +266,17 @@
             return []
 
         self._children.sort(key=lambda i: i._rendered_row if i._rendered_row is not None else sys.maxsize)
 
         action_rows = []
 
         for _, items in itertools.groupby(self.children, lambda i: i._rendered_row):
+            s_items = sorted(list(items), key=lambda i: i.position if i.position is not None else sys.maxsize)
             action_row = self._builder()
-            for item in items:
+            for item in s_items:
                 item._build(action_row)
             action_rows.append(action_row)
         return action_rows
 
     async def on_timeout(self) -> None:
         """
         Called when the item handler times out. Override for custom timeout logic.
```

### Comparing `hikari-miru-3.0.3/miru/bootstrap.py` & `hikari-miru-3.1.0/miru/bootstrap.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from miru.exceptions import BootstrapFailureError
 
 from .abc.item_handler import ItemHandler
 from .events import EventHandler
 from .traits import MiruAware
 
-__all__ = ("install", "uninstall", "load", "unload")
+__all__ = ("install", "uninstall")
 
 logger = logging.getLogger(__name__)
 
 
 def install(bot: MiruAware) -> None:
     """Install miru and pass the current running application to it.
     Starts listeners for custom miru events.
@@ -48,26 +48,14 @@
     """
     ItemHandler._app = None
     if ItemHandler._events is not None:
         ItemHandler._events.close()
         ItemHandler._events = None
 
 
-def load(bot: MiruAware) -> None:
-    """DEPRECATED: Use miru.install instead."""
-    logger.warning("miru.load is deprecated, use miru.install instead. miru.load will be removed in 3.1.0!")
-    install(bot)
-
-
-def unload() -> None:
-    """DEPRECATED: Use miru.uninstall instead."""
-    logger.warning("miru.unload is deprecated, use miru.uninstall instead. miru.unload will be removed in 3.1.0!")
-    uninstall()
-
-
 # MIT License
 #
 # Copyright (c) 2022-present HyperGH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
```

### Comparing `hikari-miru-3.0.3/miru/button.py` & `hikari-miru-3.1.0/miru/button.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         The custom identifier of the button, by default None
     url : Optional[str], optional
         The URL of the button, by default None
     emoji : Union[hikari.Emoji, str, None], optional
         The emoji present on the button, by default None
     row : Optional[int], optional
         The row the button should be in, leave as None for auto-placement.
+    position : Optional[int], optional
+        The position the button should be in within a row, leave as None for auto-placement.
 
     Raises
     ------
     TypeError
         If both label and emoji are left empty.
     TypeError
         if both custom_id and url are provided.
@@ -50,16 +52,17 @@
         style: hikari.ButtonStyle = hikari.ButtonStyle.PRIMARY,
         label: t.Optional[str] = None,
         disabled: bool = False,
         custom_id: t.Optional[str] = None,
         url: t.Optional[str] = None,
         emoji: t.Union[hikari.Emoji, str, None] = None,
         row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
     ) -> None:
-        super().__init__(custom_id=custom_id, row=row, disabled=disabled)
+        super().__init__(custom_id=custom_id, row=row, position=position, disabled=disabled)
         self._emoji: t.Optional[hikari.Emoji] = hikari.Emoji.parse(emoji) if isinstance(emoji, str) else emoji
         self.label = label
         self.url = self._url = url
         self.style = self._style = style if self._url is None else hikari.ButtonStyle.LINK
 
         if self._is_persistent and self.url:
             raise TypeError("Cannot provide both 'url' and 'custom_id'.")
```

### Comparing `hikari-miru-3.0.3/miru/context/__init__.py` & `hikari-miru-3.1.0/miru/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/context/base.py` & `hikari-miru-3.1.0/miru/context/base.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/context/modal.py` & `hikari-miru-3.1.0/miru/context/modal.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/context/raw.py` & `hikari-miru-3.1.0/miru/context/raw.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/context/view.py` & `hikari-miru-3.1.0/miru/context/view.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/events.py` & `hikari-miru-3.1.0/miru/events.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/exceptions.py` & `hikari-miru-3.1.0/miru/exceptions.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/ext/nav/README.md` & `hikari-miru-3.1.0/miru/ext/nav/README.md`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/ext/nav/__init__.py` & `hikari-miru-3.1.0/miru/ext/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/ext/nav/items.py` & `hikari-miru-3.1.0/miru/ext/nav/items.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,22 @@
 )
 
 
 class NavItem(ViewItem, abc.ABC):
     """A baseclass for all navigation items. NavigatorView requires instances of this class as it's items."""
 
     def __init__(
-        self, *, custom_id: t.Optional[str] = None, row: t.Optional[int] = None, disabled: bool = False
+        self,
+        *,
+        custom_id: t.Optional[str] = None,
+        row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
+        disabled: bool = False,
     ) -> None:
-        super().__init__(custom_id=custom_id, row=row, disabled=disabled)
+        super().__init__(custom_id=custom_id, row=row, position=position, disabled=disabled)
         self._handler: t.Optional[NavigatorView] = None
 
     async def before_page_change(self) -> None:
         """
         Called when the navigator is about to transition to the next page. Also called before the first page is sent.
         """
         pass
@@ -90,16 +95,17 @@
         self,
         *,
         style: hikari.ButtonStyle = hikari.ButtonStyle.PRIMARY,
         label: t.Optional[str] = None,
         custom_id: t.Optional[str] = None,
         emoji: t.Union[hikari.Emoji, str, None] = chr(9654),
         row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
     ):
-        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row)
+        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row, position=position)
 
     async def callback(self, context: ViewContext) -> None:
         self.view.current_page += 1
         await self.view.send_page(context)
 
     async def before_page_change(self) -> None:
         if self.view.current_page == len(self.view.pages) - 1:
@@ -117,16 +123,17 @@
         self,
         *,
         style: hikari.ButtonStyle = hikari.ButtonStyle.PRIMARY,
         label: t.Optional[str] = None,
         custom_id: t.Optional[str] = None,
         emoji: t.Union[hikari.Emoji, str, None] = chr(9664),
         row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
     ):
-        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row)
+        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row, position=position)
 
     async def callback(self, context: ViewContext) -> None:
         self.view.current_page -= 1
         await self.view.send_page(context)
 
     async def before_page_change(self) -> None:
         if self.view.current_page == 0:
@@ -144,16 +151,17 @@
         self,
         *,
         style: hikari.ButtonStyle = hikari.ButtonStyle.PRIMARY,
         label: t.Optional[str] = None,
         custom_id: t.Optional[str] = None,
         emoji: t.Union[hikari.Emoji, str, None] = chr(9194),
         row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
     ):
-        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row)
+        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row, position=position)
 
     async def callback(self, context: ViewContext) -> None:
         self.view.current_page = 0
         await self.view.send_page(context)
 
     async def before_page_change(self) -> None:
         if self.view.current_page == 0:
@@ -171,16 +179,17 @@
         self,
         *,
         style: hikari.ButtonStyle = hikari.ButtonStyle.PRIMARY,
         label: t.Optional[str] = None,
         custom_id: t.Optional[str] = None,
         emoji: t.Union[hikari.Emoji, str, None] = chr(9193),
         row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
     ):
-        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row)
+        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row, position=position)
 
     async def callback(self, context: ViewContext) -> None:
         self.view.current_page = len(self.view.pages) - 1
         await self.view.send_page(context)
 
     async def before_page_change(self) -> None:
         if self.view.current_page == len(self.view.pages) - 1:
@@ -198,17 +207,20 @@
         self,
         *,
         style: hikari.ButtonStyle = hikari.ButtonStyle.SECONDARY,
         custom_id: t.Optional[str] = None,
         emoji: t.Union[hikari.Emoji, str, None] = None,
         disabled: bool = False,
         row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
     ):
         # Either label or emoji is required, so we pass a placeholder
-        super().__init__(style=style, label="0/0", custom_id=custom_id, emoji=emoji, disabled=disabled, row=row)
+        super().__init__(
+            style=style, label="0/0", custom_id=custom_id, emoji=emoji, disabled=disabled, row=row, position=position
+        )
 
     async def before_page_change(self) -> None:
         self.label = f"{self.view.current_page+1}/{len(self.view.pages)}"
         self.disabled = self.disabled if len(self.view.pages) != 1 else True
 
     async def callback(self, context: ViewContext) -> None:
         modal = Modal(title="Jump to page")
@@ -241,16 +253,17 @@
         self,
         *,
         style: hikari.ButtonStyle = hikari.ButtonStyle.DANGER,
         label: t.Optional[str] = None,
         custom_id: t.Optional[str] = None,
         emoji: t.Union[hikari.Emoji, str, None] = chr(9209),
         row: t.Optional[int] = None,
+        position: t.Optional[int] = None,
     ):
-        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row)
+        super().__init__(style=style, label=label, custom_id=custom_id, emoji=emoji, row=row, position=position)
 
     async def callback(self, context: ViewContext) -> None:
         if not self.view.message and not self.view._inter:
             return
 
         for item in self.view.children:
             if isinstance(item, (NavItem)):
```

### Comparing `hikari-miru-3.0.3/miru/ext/nav/navigator.py` & `hikari-miru-3.1.0/miru/ext/nav/navigator.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     def _get_page_payload(
         self, page: t.Union[str, hikari.Embed, t.Sequence[hikari.Embed]]
     ) -> t.MutableMapping[str, t.Any]:
         """Get the page content that is to be sent."""
 
         content = page if isinstance(page, str) else ""
-        if isinstance(page, t.Sequence):
+        if page and isinstance(page, t.Sequence) and isinstance(page[0], hikari.Embed):
             embeds = page
         else:
             embeds = [page] if isinstance(page, hikari.Embed) else []
 
         if not content and not embeds:
             raise TypeError(f"Expected type 'str' or 'hikari.Embed' to send as page, not '{page.__class__.__name__}'.")
```

### Comparing `hikari-miru-3.0.3/miru/ext/nav/utils/__init__.py` & `hikari-miru-3.1.0/miru/ext/nav/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/ext/nav/utils/paginator.py` & `hikari-miru-3.1.0/miru/ext/nav/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/modal.py` & `hikari-miru-3.1.0/miru/modal.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/select/base.py` & `hikari-miru-3.1.0/miru/select/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         custom_id: t.Optional[str] = None,
         placeholder: t.Optional[str] = None,
         min_values: int = 1,
         max_values: int = 1,
         disabled: bool = False,
         row: t.Optional[int] = None,
     ) -> None:
-        super().__init__(custom_id=custom_id, row=row, disabled=disabled)
+        super().__init__(custom_id=custom_id, row=row, position=0, disabled=disabled)
         self.placeholder = placeholder
         self.min_values = min_values
         self.max_values = max_values
 
     @property
     def placeholder(self) -> t.Optional[str]:
         """
```

### Comparing `hikari-miru-3.0.3/miru/select/channel.py` & `hikari-miru-3.1.0/miru/select/channel.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/select/mentionable.py` & `hikari-miru-3.1.0/miru/select/mentionable.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/select/role.py` & `hikari-miru-3.1.0/miru/select/role.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/select/text.py` & `hikari-miru-3.1.0/miru/select/text.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/select/user.py` & `hikari-miru-3.1.0/miru/select/user.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/text_input.py` & `hikari-miru-3.1.0/miru/text_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         value: t.Optional[str] = None,
         required: bool = False,
         min_length: t.Optional[int] = None,
         max_length: t.Optional[int] = None,
         custom_id: t.Optional[str] = None,
         row: t.Optional[int] = None,
     ) -> None:
-        super().__init__(custom_id=custom_id, row=row, required=required)
+        super().__init__(custom_id=custom_id, row=row, position=0, required=required)
         self._width: int = 5
         # Set value directly to avoid validation with missing values
         self._value: t.Optional[str] = str(value) if value else None
         self.style = style
         self.placeholder = placeholder
         self.label = label
         self.max_length = max_length
```

### Comparing `hikari-miru-3.0.3/miru/traits.py` & `hikari-miru-3.1.0/miru/traits.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/miru/view.py` & `hikari-miru-3.1.0/miru/view.py`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/pyproject.toml` & `hikari-miru-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari-miru-3.0.3/setup.py` & `hikari-miru-3.1.0/setup.py`

 * *Files identical despite different names*

