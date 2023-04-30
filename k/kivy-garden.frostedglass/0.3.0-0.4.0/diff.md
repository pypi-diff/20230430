# Comparing `tmp/kivy_garden.frostedglass-0.3.0.tar.gz` & `tmp/kivy_garden.frostedglass-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivy_garden.frostedglass-0.3.0.tar", last modified: Thu Mar  2 04:08:25 2023, max compression
+gzip compressed data, was "kivy_garden.frostedglass-0.4.0.tar", last modified: Sun Apr 30 17:55:49 2023, max compression
```

## Comparing `kivy_garden.frostedglass-0.3.0.tar` & `kivy_garden.frostedglass-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-03-02 04:08:25.836043 kivy_garden.frostedglass-0.3.0/
--rw-r--r--   0 alpha     (1000) alpha     (1000)        7 2023-02-28 14:52:25.000000 kivy_garden.frostedglass-0.3.0/AUTHORS.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)     1096 2023-02-28 14:52:25.000000 kivy_garden.frostedglass-0.3.0/LICENSE.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)     7336 2023-03-02 04:08:25.836043 kivy_garden.frostedglass-0.3.0/PKG-INFO
--rw-r--r--   0 alpha     (1000) alpha     (1000)     6602 2023-03-02 02:58:26.000000 kivy_garden.frostedglass-0.3.0/README.md
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-03-02 04:08:25.836043 kivy_garden.frostedglass-0.3.0/kivy_garden/
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-03-02 04:08:25.836043 kivy_garden.frostedglass-0.3.0/kivy_garden/frostedglass/
--rw-r--r--   0 alpha     (1000) alpha     (1000)    23336 2023-03-02 03:13:55.000000 kivy_garden.frostedglass-0.3.0/kivy_garden/frostedglass/__init__.py
--rw-r--r--   0 alpha     (1000) alpha     (1000)       23 2023-03-02 02:58:26.000000 kivy_garden.frostedglass-0.3.0/kivy_garden/frostedglass/_version.py
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-03-02 04:08:25.836043 kivy_garden.frostedglass-0.3.0/kivy_garden/frostedglass/tests/
--rw-r--r--   0 alpha     (1000) alpha     (1000)      119 2023-02-28 14:52:25.000000 kivy_garden.frostedglass-0.3.0/kivy_garden/frostedglass/tests/test_import.py
-drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-03-02 04:08:25.836043 kivy_garden.frostedglass-0.3.0/kivy_garden.frostedglass.egg-info/
--rw-r--r--   0 alpha     (1000) alpha     (1000)     7336 2023-03-02 04:08:25.000000 kivy_garden.frostedglass-0.3.0/kivy_garden.frostedglass.egg-info/PKG-INFO
--rw-r--r--   0 alpha     (1000) alpha     (1000)      411 2023-03-02 04:08:25.000000 kivy_garden.frostedglass-0.3.0/kivy_garden.frostedglass.egg-info/SOURCES.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)        1 2023-03-02 04:08:25.000000 kivy_garden.frostedglass-0.3.0/kivy_garden.frostedglass.egg-info/dependency_links.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)       90 2023-03-02 04:08:25.000000 kivy_garden.frostedglass-0.3.0/kivy_garden.frostedglass.egg-info/requires.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)       12 2023-03-02 04:08:25.000000 kivy_garden.frostedglass-0.3.0/kivy_garden.frostedglass.egg-info/top_level.txt
--rw-r--r--   0 alpha     (1000) alpha     (1000)      200 2023-03-02 04:08:25.836043 kivy_garden.frostedglass-0.3.0/setup.cfg
--rw-r--r--   0 alpha     (1000) alpha     (1000)     1826 2023-03-02 04:05:41.000000 kivy_garden.frostedglass-0.3.0/setup.py
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/
+-rw-r--r--   0 alpha     (1000) alpha     (1000)        7 2023-03-02 15:32:43.000000 kivy_garden.frostedglass-0.4.0/AUTHORS.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     1096 2023-03-02 15:32:43.000000 kivy_garden.frostedglass-0.4.0/LICENSE.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     7333 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/PKG-INFO
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     6599 2023-03-02 15:33:41.000000 kivy_garden.frostedglass-0.4.0/README.md
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/kivy_garden/
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/
+-rw-r--r--   0 alpha     (1000) alpha     (1000)    25768 2023-04-30 17:10:34.000000 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/__init__.py
+-rw-r--r--   0 alpha     (1000) alpha     (1000)       23 2023-04-30 17:46:52.000000 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/_version.py
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/tests/
+-rw-r--r--   0 alpha     (1000) alpha     (1000)      119 2023-03-02 15:32:43.000000 kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/tests/test_import.py
+drwxr-xr-x   0 alpha     (1000) alpha     (1000)        0 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     7333 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/PKG-INFO
+-rw-r--r--   0 alpha     (1000) alpha     (1000)      411 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/SOURCES.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)        1 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/dependency_links.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)       90 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/requires.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)       12 2023-04-30 17:55:49.000000 kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/top_level.txt
+-rw-r--r--   0 alpha     (1000) alpha     (1000)      200 2023-04-30 17:55:49.317539 kivy_garden.frostedglass-0.4.0/setup.cfg
+-rw-r--r--   0 alpha     (1000) alpha     (1000)     1826 2023-03-02 15:33:04.000000 kivy_garden.frostedglass-0.4.0/setup.py
```

### Comparing `kivy_garden.frostedglass-0.3.0/LICENSE.txt` & `kivy_garden.frostedglass-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kivy_garden.frostedglass-0.3.0/PKG-INFO` & `kivy_garden.frostedglass-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy_garden.frostedglass
-Version: 0.3.0
+Version: 0.4.0
 Summary: FrostedGlass is a Kivy widget with frosted glass effect.
 Home-page: https://github.com/kivy-garden/frostedglass
 Author: Kivy
 Author-email: kivy@kivy.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/kivy-garden/frostedglass/issues
 Project-URL: Source, https://github.com/kivy-garden/frostedglass
@@ -88,15 +88,15 @@
         font_size: dp(25)
 ```
 
 <br>
 
 ## FrostedGlass Showcase:
 
-**You can find the source code in the 🔷[examples folder](https://github.com/kivy-garden/frostedglass/tree/develop/examples)🔷**
+**You can find the source code in the 🔷[examples folder](https://github.com/kivy-garden/frostedglass/tree/main/examples)🔷**
 
 https://user-images.githubusercontent.com/73297572/214139558-f995ac2c-77bb-4952-a82b-212e2f31d65f.mp4
 
 <br>
 
 ## Overview of *FrostedGlass* creation process
```

### Comparing `kivy_garden.frostedglass-0.3.0/README.md` & `kivy_garden.frostedglass-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         font_size: dp(25)
 ```
 
 <br>
 
 ## FrostedGlass Showcase:
 
-**You can find the source code in the 🔷[examples folder](https://github.com/kivy-garden/frostedglass/tree/develop/examples)🔷**
+**You can find the source code in the 🔷[examples folder](https://github.com/kivy-garden/frostedglass/tree/main/examples)🔷**
 
 https://user-images.githubusercontent.com/73297572/214139558-f995ac2c-77bb-4952-a82b-212e2f31d65f.mp4
 
 <br>
 
 ## Overview of *FrostedGlass* creation process
```

### Comparing `kivy_garden.frostedglass-0.3.0/kivy_garden/frostedglass/__init__.py` & `kivy_garden.frostedglass-0.4.0/kivy_garden/frostedglass/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 opacity, border radius and the outline (color and width).
 """
 
 __all__ = ("FrostedGlass",)
 
 from ._version import __version__
 
+import os
 from time import perf_counter as now
 
 from kivy.clock import Clock
 from kivy.core.window import Window
 from kivy.graphics import (
     BindTexture,
     ClearBuffers,
@@ -383,27 +384,32 @@
         self.last_fbo_pos = [None, None]
         self._pos = [0, 0]
         self.popup_parent = None
         self.parent_screen = None
         self.parents_list = []
         self.background_children_list = []
         self.background_parents_list = []
+        self._last_background_canvas = None
 
         self.is_movable = False
         self.adapted_fbo_size = False
 
         self._update_glsl_ev = Clock.create_trigger(self._update_glsl, 0)
         self._update_fbo_ev = Clock.create_trigger(self._update_fbo_effect, 0)
         self._update_texture_ev = Clock.create_trigger(
             self._set_final_texture, 0
         )
         self._refresh_effect_ev = Clock.create_trigger(
             self.refresh_effect, 0.033333, True
         )
 
+        if not os.environ.get("FG_ASK_UPDATE_CANVAS_ACTIVE"):
+            os.environ["FG_ASK_UPDATE_CANVAS_ACTIVE"] = "1"
+            Clock.schedule_interval(lambda dt: Window.canvas.ask_update(), 0)
+
     def update_effect(self, *args):
         self._update_glsl_ev()
 
     def refresh_effect(self, *args):
         self._update_fbo_ev()
         self._update_glsl_ev()
 
@@ -436,30 +442,27 @@
 
         self._update_texture_ev()
 
     def _set_final_texture(self, pos):
         if not self.background:
             return
 
-        if self.background.canvas not in self.h_blur.children:
-            self.h_blur.add(self.background.canvas)
-            self.h_blur.draw()
+        if self._last_background_canvas not in self.h_blur.children:
+            self.h_blur.add(self._last_background_canvas)
             self.v_blur.add(self.h_blur.rect)
-            self.v_blur.draw()
 
         if self.h_blur.rect.texture != self.h_blur.texture:
             self.h_blur.rect.texture = self.h_blur.texture
 
         self.h_blur.rect.size = self.size
         self.h_blur.rect.pos = self._pos
 
         self.h_blur.draw()
         self.v_blur.draw()
         self.v_blur.ask_update()
-        Window.canvas.ask_update()
 
         self.bt_1.texture = self.v_blur.texture
 
         if self._update_texture_ev.timeout == 0:
             self._update_texture_ev.timeout = -1
 
     def _update_noise_texture(self):
@@ -530,36 +533,48 @@
         blur_size = int(blur_size)
         if blur_size != self.last_blur_size_value:
             self.v_blur["blur_size"] = dp(blur_size)
             self.h_blur["blur_size"] = dp(blur_size)
             self.update_effect()
             self.last_blur_size_value = blur_size
 
-    def on_background(self, *args):
-        if not self.background:
+    def on_background(self, _, background):
+        if not background:
             return
+
+        if self._last_background_canvas in self.h_blur.children:
+            self.h_blur.remove(self._last_background_canvas)
+            self.update_effect()
+            self._unbind_parent_properties(self.background_parents_list)
+            self._unbind_children_properties(self.background_children_list)
+
+        self._last_background_canvas = background.canvas
+
         self.background_parents_list = self._get_all_parents(self.background)
         self.background_children_list = self._get_all_children(self.background)
         self._bind_parent_properties(self.background_parents_list)
         self._bind_children_properties(self.background_children_list)
 
-    def on_parent(self, *args):
-        self.parents_list = self._get_all_parents(self.parent)
+    def on_parent(self, _, parent):
+        if not parent:
+            return
+
+        self.parents_list = self._get_all_parents(parent)
         for p in self.parents_list:
             if isinstance(p, ModalView):
                 self.popup_parent = p
             if isinstance(p, Screen):
                 self.parent_screen = p
             if isinstance(p, ScrollView):
                 self.is_movable = True
         self._bind_parent_properties(self.parents_list)
 
     def _get_all_parents(self, widget):
         widgets_list = []
-        parent = self.parent
+        parent = widget
         while True:
             widgets_list.append(parent)
             if parent.parent and parent != parent.parent:
                 parent = parent.parent
             else:
                 break
         return widgets_list
@@ -588,69 +603,119 @@
         )
         for widget in children_list:
             for property in properties_to_bind:
                 try:
                     if property == "texture":
                         if isinstance(widget, Image):
                             widget.bind(
-                                texture=lambda *args:
-                                    self._trigger_update_effect()
+                                texture=self._trigger_update_effect
                             )
                         if isinstance(widget, Video):
                             widget.bind(
-                                position=lambda *args:
-                                    self._trigger_update_effect()
+                                position=self._trigger_update_effect
                             )
                     elif hasattr(widget, property):
                         widget.fbind(
                             property,
-                            lambda *args: self._trigger_update_effect(),
+                            self._trigger_update_effect,
                         )
                 except Exception as e:
                     print(e)
                     pass
 
     def _bind_parent_properties(self, parents_list):
         for widget in parents_list:
 
             if isinstance(widget, ScrollView):
                 widget.bind(
-                    size=lambda _, size: self._trigger_update_effect(size),
-                    pos=lambda _, pos: self._trigger_update_effect(pos),
-                    scroll_x=lambda _, scroll_x: self._trigger_update_effect(
-                        scroll_x
-                    ),
-                    scroll_y=lambda _, scroll_y: self._trigger_update_effect(
-                        scroll_y
-                    ),
+                    size=self._trigger_update_effect,
+                    pos=self._trigger_update_effect,
+                    scroll_x=self._trigger_update_effect,
+                    scroll_y=self._trigger_update_effect,
                 )
             if isinstance(widget, ModalView):
                 widget.bind(
-                    on_pre_open=lambda *args: self._trigger_update_effect()
+                    on_pre_open=self._trigger_update_effect
                 )
             elif isinstance(widget, Screen):
                 widget.bind(
                     on_pre_enter=lambda *args: self._refresh_effect_ev()
                 )
                 widget.bind(
                     on_enter=lambda *args: self._refresh_effect_ev.cancel()
                 )
 
             else:
-                widget.bind(
-                    size=lambda _, size: self._trigger_update_effect(size)
+                widget.bind(size=self._trigger_update_effect)
+                try:
+                    widget.bind(pos=self._trigger_update_effect)
+                except Exception:
+                    pass
+
+    def _unbind_children_properties(self, children_list):
+        properties_to_unbind = (
+            "pos",
+            "size",
+            "scroll_x",
+            "scroll_y",
+            "on_open",
+            "on_enter",
+            "texture",
+        )
+        for widget in children_list:
+            for property in properties_to_unbind:
+                try:
+                    if property == "texture":
+                        if isinstance(widget, Image):
+                            widget.unbind(
+                                texture=self._trigger_update_effect
+                            )
+                        if isinstance(widget, Video):
+                            widget.unbind(
+                                position=self._trigger_update_effect
+                            )
+                    elif hasattr(widget, property):
+                        widget.funbind(
+                            property,
+                            self._trigger_update_effect,
+                        )
+                except Exception as e:
+                    print(e)
+                    pass
+
+    def _unbind_parent_properties(self, parents_list):
+        for widget in parents_list:
+
+            if isinstance(widget, ScrollView):
+                widget.unbind(
+                    size=self._trigger_update_effect,
+                    pos=self._trigger_update_effect,
+                    scroll_x=self._trigger_update_effect,
+                    scroll_y=self._trigger_update_effect,
+                )
+            if isinstance(widget, ModalView):
+                widget.unbind(
+                    on_pre_open=self._trigger_update_effect
                 )
+            elif isinstance(widget, Screen):
+                widget.unbind(
+                    on_pre_enter=lambda *args: self._refresh_effect_ev()
+                )
+                widget.unbind(
+                    on_enter=lambda *args: self._refresh_effect_ev.cancel()
+                )
+
+            else:
+                widget.unbind(size=self._trigger_update_effect)
                 try:
-                    widget.bind(
-                        pos=lambda _, pos: self._trigger_update_effect(pos)
-                    )
+                    widget.unbind(pos=self._trigger_update_effect)
                 except Exception:
                     pass
 
-    def _trigger_update_effect(self, value=None):
+    def _trigger_update_effect(self, widget, value=None):
         if value is None and self.update_by_timeout:
             self.update_effect()
 
         if (
             (isinstance(value, int) or isinstance(value, float))
             and self.update_by_timeout
             and round(value, 3) != self.last_value
@@ -671,15 +736,15 @@
 
     @property
     def popup_closed(self):
         return self.popup_parent and not self.popup_parent.parent
 
     @property
     def not_current_screen(self):
-        if self.parent_screen is None:
+        if self.parent_screen is None or self.parent_screen.manager is None:
             return False
         return self.parent_screen.manager.current != self.parent_screen.name
 
     @property
     def out_of_the_window(self):
         x, y = self.to_window(self.x, self.y)
         right, top = self.to_window(self.right, self.top)
```

### Comparing `kivy_garden.frostedglass-0.3.0/kivy_garden.frostedglass.egg-info/PKG-INFO` & `kivy_garden.frostedglass-0.4.0/kivy_garden.frostedglass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy-garden.frostedglass
-Version: 0.3.0
+Version: 0.4.0
 Summary: FrostedGlass is a Kivy widget with frosted glass effect.
 Home-page: https://github.com/kivy-garden/frostedglass
 Author: Kivy
 Author-email: kivy@kivy.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/kivy-garden/frostedglass/issues
 Project-URL: Source, https://github.com/kivy-garden/frostedglass
@@ -88,15 +88,15 @@
         font_size: dp(25)
 ```
 
 <br>
 
 ## FrostedGlass Showcase:
 
-**You can find the source code in the 🔷[examples folder](https://github.com/kivy-garden/frostedglass/tree/develop/examples)🔷**
+**You can find the source code in the 🔷[examples folder](https://github.com/kivy-garden/frostedglass/tree/main/examples)🔷**
 
 https://user-images.githubusercontent.com/73297572/214139558-f995ac2c-77bb-4952-a82b-212e2f31d65f.mp4
 
 <br>
 
 ## Overview of *FrostedGlass* creation process
```

### Comparing `kivy_garden.frostedglass-0.3.0/setup.py` & `kivy_garden.frostedglass-0.4.0/setup.py`

 * *Files identical despite different names*

