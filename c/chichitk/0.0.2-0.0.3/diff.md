# Comparing `tmp/chichitk-0.0.2.tar.gz` & `tmp/chichitk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chichitk-0.0.2.tar", last modified: Tue Apr 18 22:04:38 2023, max compression
+gzip compressed data, was "chichitk-0.0.3.tar", last modified: Sat Apr 29 23:45:06 2023, max compression
```

## Comparing `chichitk-0.0.2.tar` & `chichitk-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:38.036381 chichitk-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-16 02:22:07.000000 chichitk-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3223 2023-04-18 22:04:38.036381 chichitk-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2485 2023-04-18 21:24:18.000000 chichitk-0.0.2/Readme.md
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:38.006462 chichitk-0.0.2/chichitk/
--rw-rw-rw-   0        0        0      656 2023-04-17 16:30:35.000000 chichitk-0.0.2/chichitk/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-04-17 00:34:05.000000 chichitk-0.0.2/chichitk/aspect_frame.py
--rw-rw-rw-   0        0        0    26105 2023-04-16 23:33:38.000000 chichitk-0.0.2/chichitk/buttons.py
--rw-rw-rw-   0        0        0    49997 2023-04-16 02:08:01.000000 chichitk-0.0.2/chichitk/canvas_items.py
--rw-rw-rw-   0        0        0    16147 2023-03-25 14:30:32.000000 chichitk-0.0.2/chichitk/dropdowns.py
--rw-rw-rw-   0        0        0     8815 2023-03-28 22:48:12.000000 chichitk-0.0.2/chichitk/entry_boxes.py
--rw-rw-rw-   0        0        0     6098 2023-04-18 17:15:53.000000 chichitk-0.0.2/chichitk/file_dialog.py
--rw-rw-rw-   0        0        0     4288 2023-04-16 21:18:55.000000 chichitk-0.0.2/chichitk/function_progress.py
--rw-rw-rw-   0        0        0    34820 2023-04-18 17:09:52.000000 chichitk-0.0.2/chichitk/icons.py
--rw-rw-rw-   0        0        0    10583 2023-04-16 21:19:48.000000 chichitk-0.0.2/chichitk/labels.py
--rw-rw-rw-   0        0        0    10145 2023-04-18 17:35:06.000000 chichitk-0.0.2/chichitk/pdf_display.py
--rw-rw-rw-   0        0        0     7301 2023-04-16 23:35:43.000000 chichitk-0.0.2/chichitk/player.py
--rw-rw-rw-   0        0        0     5152 2023-03-24 16:40:10.000000 chichitk-0.0.2/chichitk/progress_bar.py
--rw-rw-rw-   0        0        0     3776 2023-03-28 23:26:56.000000 chichitk-0.0.2/chichitk/scrollable_frame.py
--rw-rw-rw-   0        0        0    66444 2023-04-17 23:52:20.000000 chichitk-0.0.2/chichitk/sliders.py
--rw-rw-rw-   0        0        0     4927 2023-03-24 17:01:52.000000 chichitk-0.0.2/chichitk/temp_menu.py
--rw-rw-rw-   0        0        0     9187 2023-04-04 22:46:09.000000 chichitk-0.0.2/chichitk/text_boxes.py
--rw-rw-rw-   0        0        0     9855 2023-04-15 18:26:04.000000 chichitk-0.0.2/chichitk/timer.py
--rw-rw-rw-   0        0        0     6880 2023-03-23 19:14:50.000000 chichitk-0.0.2/chichitk/tool_tip.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:04:38.034387 chichitk-0.0.2/chichitk.egg-info/
--rw-rw-rw-   0        0        0     3223 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 22:04:37.000000 chichitk-0.0.2/chichitk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1196 2023-04-18 22:03:48.000000 chichitk-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 22:04:38.037377 chichitk-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 23:45:06.329406 chichitk-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-16 02:22:07.000000 chichitk-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3375 2023-04-29 23:45:06.328408 chichitk-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2637 2023-04-22 16:09:51.000000 chichitk-0.0.3/Readme.md
+drwxrwxrwx   0        0        0        0 2023-04-29 23:45:06.303208 chichitk-0.0.3/chichitk/
+-rw-rw-rw-   0        0        0      699 2023-04-29 22:46:55.000000 chichitk-0.0.3/chichitk/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-04-17 00:34:05.000000 chichitk-0.0.3/chichitk/aspect_frame.py
+-rw-rw-rw-   0        0        0    26614 2023-04-21 01:55:06.000000 chichitk-0.0.3/chichitk/buttons.py
+-rw-rw-rw-   0        0        0    49997 2023-04-16 02:08:01.000000 chichitk-0.0.3/chichitk/canvas_items.py
+-rw-rw-rw-   0        0        0     6834 2023-04-29 23:10:26.000000 chichitk-0.0.3/chichitk/collapse_frame.py
+-rw-rw-rw-   0        0        0    16147 2023-03-25 14:30:32.000000 chichitk-0.0.3/chichitk/dropdowns.py
+-rw-rw-rw-   0        0        0     8943 2023-04-22 15:48:45.000000 chichitk-0.0.3/chichitk/entry_boxes.py
+-rw-rw-rw-   0        0        0     6098 2023-04-18 17:15:53.000000 chichitk-0.0.3/chichitk/file_dialog.py
+-rw-rw-rw-   0        0        0     4288 2023-04-16 21:18:55.000000 chichitk-0.0.3/chichitk/function_progress.py
+-rw-rw-rw-   0        0        0    34820 2023-04-18 17:09:52.000000 chichitk-0.0.3/chichitk/icons.py
+-rw-rw-rw-   0        0        0    23868 2023-04-29 03:36:03.000000 chichitk-0.0.3/chichitk/labels.py
+-rw-rw-rw-   0        0        0    10238 2023-04-21 01:24:23.000000 chichitk-0.0.3/chichitk/pdf_display.py
+-rw-rw-rw-   0        0        0     7301 2023-04-16 23:35:43.000000 chichitk-0.0.3/chichitk/player.py
+-rw-rw-rw-   0        0        0     5152 2023-03-24 16:40:10.000000 chichitk-0.0.3/chichitk/progress_bar.py
+-rw-rw-rw-   0        0        0     3990 2023-04-20 02:51:35.000000 chichitk-0.0.3/chichitk/scrollable_frame.py
+-rw-rw-rw-   0        0        0    66444 2023-04-17 23:52:20.000000 chichitk-0.0.3/chichitk/sliders.py
+-rw-rw-rw-   0        0        0     4927 2023-03-24 17:01:52.000000 chichitk-0.0.3/chichitk/temp_menu.py
+-rw-rw-rw-   0        0        0    11203 2023-04-19 18:24:06.000000 chichitk-0.0.3/chichitk/text_boxes.py
+-rw-rw-rw-   0        0        0     9855 2023-04-15 18:26:04.000000 chichitk-0.0.3/chichitk/timer.py
+-rw-rw-rw-   0        0        0     6880 2023-03-23 19:14:50.000000 chichitk-0.0.3/chichitk/tool_tip.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:45:06.326280 chichitk-0.0.3/chichitk.egg-info/
+-rw-rw-rw-   0        0        0     3375 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 23:45:03.000000 chichitk-0.0.3/chichitk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1161 2023-04-29 23:42:20.000000 chichitk-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 23:45:06.330404 chichitk-0.0.3/setup.cfg
```

### Comparing `chichitk-0.0.2/LICENSE` & `chichitk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/PKG-INFO` & `chichitk-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chichitk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python UI library built upon Tkinter
 Author-email: Samuel Gibson <samuelpgibson12@gmail.com>
 Project-URL: Homepage, https://github.com/SamGibson1/ChichiTk
 Project-URL: Documentation, https://github.com/SamGibson1/ChichiTk/wiki
 Project-URL: Bug Tracker, https://github.com/SamGibson1/ChichiTk/issues
 Keywords: python,tkinter,custom,widgets
 Classifier: Development Status :: 3 - Alpha
@@ -39,15 +39,15 @@
 Update as often as possible because this library is under active development.
 
 ## Documentation
 The **official** documentation can be found in the Wiki Tab here:
 
 **--> [ChichiTk Documentation](https://github.com/SamGibson1/ChichiTk/wiki)**
 
-## Example Program
+## Example Program - Stopwatch
 The following is a simple Stopwatch program that uses chichitk.Player to manage callbacks:
 ```python
 from tkinter import Tk, Frame, Label
 from chichitk import Player
 
 def time_text(time:int, f:int=100):
     hour = time // (3600 * f)
@@ -70,11 +70,17 @@
 Play = Player(frame, lambda t: label.config(text=time_text(t)), 0.01,
               bg='#1e1e22', frame_num=12001, frame_rate=100, step_increment=500)
 Play.pack(side='bottom', fill='x')
 
 app.mainloop()
 ```
 This results in the following window:
+
 <img src="documentation_images/stopwatch_example.jpg" width="600"/>
 
-<!-- ## Example Application - Password Manager
-Video here showing password manager and link to git repo for password manager -->
+## Example Application - Password Manager
+
+https://user-images.githubusercontent.com/74847576/233730056-cffb5a0d-41db-44e4-ad24-7276406f9ba1.mp4
+
+The Passwords App project can be found here:
+
+**--> [Project Link](https://github.com/SamGibson1/PasswordManager)**
```

### Comparing `chichitk-0.0.2/Readme.md` & `chichitk-0.0.3/Readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Update as often as possible because this library is under active development.
 
 ## Documentation
 The **official** documentation can be found in the Wiki Tab here:
 
 **--> [ChichiTk Documentation](https://github.com/SamGibson1/ChichiTk/wiki)**
 
-## Example Program
+## Example Program - Stopwatch
 The following is a simple Stopwatch program that uses chichitk.Player to manage callbacks:
 ```python
 from tkinter import Tk, Frame, Label
 from chichitk import Player
 
 def time_text(time:int, f:int=100):
     hour = time // (3600 * f)
@@ -52,11 +52,17 @@
 Play = Player(frame, lambda t: label.config(text=time_text(t)), 0.01,
               bg='#1e1e22', frame_num=12001, frame_rate=100, step_increment=500)
 Play.pack(side='bottom', fill='x')
 
 app.mainloop()
 ```
 This results in the following window:
+
 <img src="documentation_images/stopwatch_example.jpg" width="600"/>
 
-<!-- ## Example Application - Password Manager
-Video here showing password manager and link to git repo for password manager -->
+## Example Application - Password Manager
+
+https://user-images.githubusercontent.com/74847576/233730056-cffb5a0d-41db-44e4-ad24-7276406f9ba1.mp4
+
+The Passwords App project can be found here:
+
+**--> [Project Link](https://github.com/SamGibson1/PasswordManager)**
```

### Comparing `chichitk-0.0.2/chichitk/__init__.py` & `chichitk-0.0.3/chichitk/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __version__ = "0.0.1"
 
 # Import widgets
 from .aspect_frame import *
 from .buttons import *
+from .collapse_frame import CollapseFrame
 from .dropdowns import *
 from .entry_boxes import *
 from .file_dialog import *
 from .function_progress import *
 from .labels import *
 from .pdf_display import PdfDisplay
 from .player import *
```

### Comparing `chichitk-0.0.2/chichitk/aspect_frame.py` & `chichitk-0.0.3/chichitk/aspect_frame.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/buttons.py` & `chichitk-0.0.3/chichitk/buttons.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,60 +31,66 @@
 
         Optionally, a popup will appear when the user hovers the mouse over
         button. The popup is directly above the button by default, but its
         position is adjusted if necessary to keep the popup in view. For
         example, if the button is at the very top of the window, the popup will
         appear beneath the button instead.
     '''
-    def __init__(self, master, command, popup_label:str=None, font_name:str='Segoe UI', font_size:int=10,
-                padx:int=0, pady:int=0, selectable:bool=True, select_on_click:bool=True, selected=False,
-                tool_tip_font_name:str='Segoe UI', tool_tip_font_size:int=10, bar_height:int=0, bar_side='bottom',
-                active_bg:str='#070708', inactive_bg:str='#000000', active_hover_bg=None,
-                inactive_hover_bg=None, active_fg:str='#13ce12', inactive_fg:str='#888888',
-                active_hover_fg:str='#74d573', inactive_hover_fg:str='#74d573', popup_bg=None,
-                active_bar_color=None, inactive_bar_color=None, active_hover_bar_color:str=None,
-                inactive_hover_bar_color:str='#dcdcdc', off_fg:str='#555555'):
+    def __init__(self, master, command, popup_label:str=None, click_popup=None,
+                 font_name:str='Segoe UI', font_size:int=10, padx:int=0, pady:int=0,
+                 selectable:bool=True, select_on_click:bool=True, selected=False,
+                 tool_tip_font_name:str='Segoe UI', tool_tip_font_size:int=10,
+                 bar_height:int=0, bar_side='bottom', active_bg:str='#070708',
+                 inactive_bg:str='#000000', active_hover_bg=None,
+                 inactive_hover_bg=None, active_fg:str='#13ce12',
+                 inactive_fg:str='#888888', active_hover_fg:str='#74d573',
+                 inactive_hover_fg:str='#74d573', popup_bg=None,
+                 active_bar_color=None, inactive_bar_color=None,
+                 active_hover_bar_color:str=None,
+                 inactive_hover_bar_color:str='#dcdcdc', off_fg:str='#555555'):
         '''inherits from tk.Frame - base button for inheritance from IconButton, LabelButton, ToggleIconButton, etc
         BaseButton only contains bottom bar - everything else must be added by child class
         child class must contain function config_colors
 
         Parameters
         ----------
-            master : frame in which to put button
-            command : function - function to be executed when button is clicked
-            popup_label : str - text to appear as tool tip when cursor hovers on button
-            padx : Int - internal x pad for button
-            pady : Int - internal y pad for button
-            selectable : Boolean - if True, button can be selected
-            bar_height : Int - height of bar at the bottom of button
-            bar_side : Literal['top', 'bottom', 'left', 'right'] - pack side for bar if bar_height > 0
+            :param master: frame in which to put button
+            :param command: function - function to be executed when button is clicked
+            :param popup_label: str - text to appear as tool tip when cursor hovers on button
+            :param click_popup: str - popup label changes to click_popup temporarily when button is clicked
+            :param padx: Int - internal x pad for button
+            :param pady: Int - internal y pad for button
+            :param selectable: Boolean - if True, button can be selected
+            :param bar_height: Int - height of bar at the bottom of button
+            :param bar_side: Literal['top', 'bottom', 'left', 'right'] - pack side for bar if bar_height > 0
             
-            active_bg : str (hex code) - background when button is selected
-            inactive_bg : str (hex code) - background when button is not selected
-            active_hover_bg : str (hex code) - background when selected and cursor is hovering - if None: same as active_bg
-            inactive_hover_bg : str (hex code) - background when not selected and cursor if hovering - if None: same as inactive_bg
-
-            active_fg : str (hex code) - icon and label fg when button is selected
-            inactive_fg : str (hex code) - icon and label fg when button is not selected
-            active_hover_fg : str (hex code) - icon and label fg when selected and cursor is hovering - if None: same as active_fg
-            inactive_hover_fg : str (hex code) - icon and label fg when not selected and cursor is hovering - if None: same as inactive_fg
-
-            active_bar_color : str (hex code) - bar color when selected - if None: same as active_fg
-            inactive_bar_color : str (hex code) - bar color when not selected - if None: same as inactive_bg
-            active_hover_bar_color : str (hex code) - bar color when selected and cursor is hovering - if None: same as active_bar_color
-            inactive_hover_bar_color : str (hex code) - bar color when not selected and cursor is hovering - if None: same as inactive_bar_color
+            :param active_bg: str (hex code) - background when button is selected
+            :param inactive_bg: str (hex code) - background when button is not selected
+            :param active_hover_bg: str (hex code) - background when selected and cursor is hovering - if None: same as active_bg
+            :param inactive_hover_bg: str (hex code) - background when not selected and cursor if hovering - if None: same as inactive_bg
+
+            :param active_fg: str (hex code) - icon and label fg when button is selected
+            :param inactive_fg: str (hex code) - icon and label fg when button is not selected
+            :param active_hover_fg: str (hex code) - icon and label fg when selected and cursor is hovering - if None: same as active_fg
+            :param inactive_hover_fg: str (hex code) - icon and label fg when not selected and cursor is hovering - if None: same as inactive_fg
+
+            :param active_bar_color: str (hex code) - bar color when selected - if None: same as active_fg
+            :param inactive_bar_color: str (hex code) - bar color when not selected - if None: same as inactive_bg
+            :param active_hover_bar_color: str (hex code) - bar color when selected and cursor is hovering - if None: same as active_bar_color
+            :param inactive_hover_bar_color: str (hex code) - bar color when not selected and cursor is hovering - if None: same as inactive_bar_color
         '''
         Frame.__init__(self, master)
         self.padx, self.pady = padx, pady
         self.selected, self.hovering = selected, False
         self.active = True # if not active, button will not be responsive
         self.click_command = command
         self.font_name, self.font_size = font_name, font_size
         self.selectable, self.select_on_click = selectable, select_on_click
         self.popup_labels = [popup_label + ' : Inactive' if popup_label else None, popup_label] # either both text or both None
+        self.click_popup = click_popup
         self.off_fg = off_fg
         self.bg_colors = [[inactive_bg, inactive_hover_bg if inactive_hover_bg else inactive_bg],
                             [active_bg, active_hover_bg if active_hover_bg else active_bg]]
         self.fg_colors = [[inactive_fg, inactive_hover_fg if inactive_hover_fg else inactive_fg],
                             [active_fg, active_hover_fg if active_hover_fg else active_fg]]
         active_bar_color = active_bar_color if active_bar_color else active_fg
         inactive_bar_color = inactive_bar_color if inactive_bar_color else inactive_bg
@@ -147,14 +153,16 @@
             if self.popup_labels[0]: # remove tool tip
                 self.tool_tip.fadeout(1, event) # first argument is initial alpha
             if self.active:
                 self.config_colors()
             
     def click_button(self, event=None):
         if self.active:
+            if self.popup_labels[0] and self.click_popup:
+                self.tool_tip.set_text(self.click_popup)
             self.click_command()
             if self.select_on_click:
                 self.select()
 
     def select(self):
         if self.selectable and not self.selected:
             self.selected = True
@@ -390,15 +398,15 @@
         Background and foreground color can change based on select/hover status.
     '''
     def __init__(self, master, command, label:str='', **kwargs):
         '''just like IconButton but with no icon'''
         BaseButton.__init__(self, master, command, **kwargs)
         self.label_text = label
         self.label = Label(self, text=label, font=(self.font_name, self.font_size), bd=0)
-        self.label.pack(side='top', padx=self.padx, pady=self.pady)
+        self.label.pack(side='top', fill='both', expand=True, padx=self.padx, pady=self.pady)
         self.label.bind("<Button-1>", self.click_button)
 
         self.config_colors()
 
     def config_colors(self):
         '''sets colors based on self.selected, self.hovering, and self.active'''
         if self.active:
```

### Comparing `chichitk-0.0.2/chichitk/canvas_items.py` & `chichitk-0.0.3/chichitk/canvas_items.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/dropdowns.py` & `chichitk-0.0.3/chichitk/dropdowns.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/entry_boxes.py` & `chichitk-0.0.3/chichitk/entry_boxes.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,19 @@
             cursor_index = self.index('insert')
             # remove character that was just entered
             self.delete(str(cursor_index - 1), str(cursor_index))
             text = super().get() # update text to current text in entry box
         if self.__check_function is not None and not self.__check_function(text):
             self.config(bg=self.error_color)
 
+    def set_bg(self, bg:str):
+        '''updates background color'''
+        self.bg = bg
+        self.config(bg=self.bg)
+
     def get(self):
         '''returns text currently in CheckEntry'''
         return self.sv.get()
     
     def clear(self):
         '''
         Purpose:
```

### Comparing `chichitk-0.0.2/chichitk/file_dialog.py` & `chichitk-0.0.3/chichitk/file_dialog.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/function_progress.py` & `chichitk-0.0.3/chichitk/function_progress.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/icons.py` & `chichitk-0.0.3/chichitk/icons.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/pdf_display.py` & `chichitk-0.0.3/chichitk/pdf_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,16 @@
         self.label.pack(fill='both', expand=True)
 
     def download_pdf(self):
         '''opens dialog to download the current pdf file
         this can only ever be called when a pdf is being viewed'''
         destination = filedialog.asksaveasfilename(initialdir='/', title='Select destination file',
                                                     filetypes=(('PDF File', '*.pdf'), ('All Files', '*.*')))
+        if destination == '': # clicked 'cancel' instead of saving file
+            return
         if destination[-4:] != '.pdf':
             destination += '.pdf'
         shutil.copy2(self.filename, destination)
 
     def open_in_window(self):
         '''opens PDF in new window - can only ever be called when a PDF is being viewed'''
         PdfWindow(self.filename, self.bg)
```

### Comparing `chichitk-0.0.2/chichitk/player.py` & `chichitk-0.0.3/chichitk/player.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/progress_bar.py` & `chichitk-0.0.3/chichitk/progress_bar.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/scrollable_frame.py` & `chichitk-0.0.3/chichitk/scrollable_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,28 @@
         <MouseWheel> event must be bound to all widgets placed in the
         scrollable frame. By default, the <MouseWheel> event is only bound
         to the frame itself
         
         All widgets must be put in self.scrollable_frame, not self
     '''
     def __init__(self, master:tk.Frame, bg:str, include_scrollbar:bool=True,
-                 yscrollincrement:int=1, check_hover=False, *args, **kwargs):
+                 scrollbar_side='right', yscrollincrement:int=1,
+                 check_hover=False, *args, **kwargs):
         '''
         Parameters
         ----------
             :param master: tk.Frame - parent widget
             :param bg: str (hex code) - background color
             :param include_scrollbar: bool - if True, scrollbar is packed right
+            :param scrollbar_side: str - Literal['left', 'right']
             :param yscrollincrement: int - pixels scrolled per mouse scroll (70x)
             :param check_hover: bool - if True, will only respond to mousewheel
                                        events if the cursor is hovering on Frame
         '''
+        assert scrollbar_side in ['left', 'right'], f'Invalide scrollbar side: {scrollbar_side}'
         self.hovering = not check_hover
         super().__init__(master, *args, **kwargs)
         style = ttk.Style(master)
         style.theme_use("alt")
         style.layout('arrowless.Vertical.TScrollbar',
                      [('Vertical.Scrollbar.trough', 
                      {'children': [('Vertical.Scrollbar.thumb',
@@ -38,15 +41,15 @@
         self.scrollable_frame = tk.Frame(self.canvas, bg=bg)
         self.scrollable_frame.bind("<Configure>", self.OnFrameConfigure)
         self.canvas_id = self.canvas.create_window((0, 0), window=self.scrollable_frame, anchor="nw")
         if include_scrollbar:
             scrollbar = ttk.Scrollbar(self, orient="vertical", command=self.canvas.yview,
                                       style='arrowless.Vertical.TScrollbar')
             self.canvas.configure(yscrollcommand=scrollbar.set)
-            scrollbar.pack(side="right", fill="y")
+            scrollbar.pack(side=scrollbar_side, fill="y")
         self.canvas.pack(side="left", fill="both", expand=True)
         style.configure("arrowless.Vertical.TScrollbar", troughcolor=bg)
         self.canvas.bind('<Configure>', self.FrameWidth)
         self.canvas.bind("<MouseWheel>", self.on_mousewheel)
         self.scrollable_frame.bind("<MouseWheel>", self.on_mousewheel)
         if check_hover:
             self.bind('<Enter>', self.hover_enter)
```

### Comparing `chichitk-0.0.2/chichitk/sliders.py` & `chichitk-0.0.3/chichitk/sliders.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/temp_menu.py` & `chichitk-0.0.3/chichitk/temp_menu.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/text_boxes.py` & `chichitk-0.0.3/chichitk/text_boxes.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,59 +46,74 @@
     ''' Text widget that counts the lines just like a code editor and can
         call a callback function whenever the text is edited by the user
         
         TextBox can optionally display an error color when there are blank
         lines or consecutive spaces
     '''
     def __init__(self, master, callback=None, bg:str='#ffffff', fg:str='#000000',
-                 cursor_color=None, error_bg:str='#3c2525',
-                 error_highlight_bg:str='#ff0000', error_highlight_fg:str='#000000',
-                 track_fg:str='#bbbbbb', font_name:str='Consolas', font_size:int=15,
-                 width=None, height=None, focus_in_function=None, focus_out_function=None,
-                 check_blank_lines:bool=True, check_consecutive_spaces:bool=True):
+                 cursor_color=None, disabled_bg=None, disabled_fg=None,
+                 error_bg:str='#3c2525', error_highlight_bg:str='#ff0000',
+                 error_highlight_fg:str='#000000', track_fg:str='#bbbbbb',
+                 font_name:str='Consolas', font_size:int=15,  wrap='none',
+                 focus_in_function=None, focus_out_function=None,
+                 check_blank_lines:bool=True, check_consecutive_spaces:bool=True,
+                 line_numbers_labels=True, width=None, height=None,
+                 justify='left', inactive_justify='center'):
         '''Text box with number lines and callback when text box is edited
         
         Parameters
         ----------
             :param master: tk.Frame - parent widget
             :param callback: function (str) - called whenever text box is modified
             :param bg: str (hex code) - background color
             :param fg: str (hex code) - main text color
             :param cursor_color: str (hex code) - cursor color - if different from fg
+            :param disabled_bg: str (hex code) - background color when disabled
+            :param disabled_fg: str (hex code) - foreground color when disabled
             :param error_bg: str (hex code) - background color when there is an error
             :param error_highlight_bg: str (hex code) - highlight on text causing error
             :param error_highlight_fg: str (hex code) - color of text cauing error
             :param track_fg: str (hex code) - color of track text - line numbers
+            :param font_name: str - font for text box and line numbers
+            :param font_size: int - font size for text box and line numbers
+            :param wrap: str Literal['none', 'char', 'word'] - wrap setting
             :param focus_in_function: function () - called when text box takes focus
             :param focus_out_function: function () - called when text box loses focus
             :param check_blank_lines: bool - if True, show error when there are blank lines
             :param check_consecutive_spaces: bool - if True, show error when there are consecutive spaces
+            :param line_numbers_labels: bool - if True, show line numbers
         '''
         self.callback_function = callback
-        self.bg = bg
+        self.bg, self.fg = bg, fg
         self.error_bg = error_bg
         self.error_highlight_bg = error_highlight_bg
         self.error_highlight_fg = error_highlight_fg
+        self.disabled_bg = disabled_bg if disabled_bg else bg
+        self.disabled_fg = disabled_fg if disabled_fg else fg
+        self.justify, self.inactive_justify = justify, inactive_justify
         Frame.__init__(self, master, bg=bg)
         self.good_format = True # False if there are errors in the text box
         self.check_blank_lines = check_blank_lines
         self.check_consecutive_spaces = check_consecutive_spaces
         cursor_color = cursor_color if cursor_color else fg
 
         self.track = Text(self, width=4, height=height, font=(font_name, font_size),
                           bg=bg, fg=track_fg, wrap='none', bd=0,
                           yscrollcommand=lambda a, b: self.box.yview_moveto(a))
-        self.track.pack(side='left', fill='y')
+        if line_numbers_labels:
+            self.track.pack(side='left', fill='y')
         self.track.insert('end', '  1')
         self.track.config(state='disabled')
         # undo must be False because Ctrl+z causes infinite loop (no idea why)
         self.box = Text(self, width=width, height=height, font=(font_name, font_size),
-                        bg=bg, fg=fg, insertbackground=cursor_color, undo=False, wrap='none',
+                        bg=bg, fg=fg, insertbackground=cursor_color, undo=False, wrap=wrap,
                         yscrollcommand=lambda a, b: self.track.yview_moveto(a), bd=0)
         self.box.pack(side='right', fill='both', expand=True)
+        self.box.tag_add("justify", 1.0, "end")
+        self.box.tag_configure('justify', justify=self.justify)
         self.box.bind("<<TextModified>>", self.callback)
         #self.box.bind("<Key>", self.callback)
         if focus_in_function:
             self.box.bind("<FocusIn>", focus_in_function)
         if focus_out_function:
             self.box.bind("<FocusOut>", focus_out_function)
 
@@ -166,16 +181,23 @@
                 self.track.config(bg=self.error_bg)
 
         self.box.yview_moveto(y_pos)
         self.track.yview_moveto(y_pos)
         if self.callback_function:
             self.callback_function(text)
 
-    def get(self):
-        '''returns entire text in text box'''
+    def get(self, strip=True) -> str:
+        '''returns entire text in text box
+
+        Parameters
+        -----------
+            :param strip: bool - if True, removes spaces and newline characters for beginning and end
+        '''
+        if strip:
+            return self.box.get(0.0, 'end').strip()
         return self.box.get(0.0, 'end')
 
     def clear(self):
         '''clears all text from text box'''
         self.box.delete(0.0, 'end')
 
     def insert(self, text):
@@ -183,7 +205,27 @@
         self.box.insert('end', text)
 
     def clear_insert(self, text):
         '''clears all text from text box and adds text'''
         self.clear()
         self.insert(text)
 
+    def set_active(self):
+        '''
+        Purpose:
+            sets text box state to 'normal' so that it is interactable
+        '''
+        self.box.config(state='normal', bg=self.bg, fg=self.fg)
+        self.box.tag_add("justify", 1.0, "end")
+        self.box.tag_configure('justify', justify=self.justify)
+        self.track.config(bg=self.bg)
+
+    def set_inactive(self):
+        '''
+        Purpose:
+            sets text box state to 'disabled' so that it is not interactable
+        '''
+        self.box.config(state='disabled', bg=self.disabled_bg, fg=self.disabled_fg)
+        self.box.tag_add("justify", 1.0, "end")
+        self.box.tag_configure('justify', justify=self.inactive_justify)
+        self.track.config(bg=self.disabled_bg)
+
```

### Comparing `chichitk-0.0.2/chichitk/timer.py` & `chichitk-0.0.3/chichitk/timer.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk/tool_tip.py` & `chichitk-0.0.3/chichitk/tool_tip.py`

 * *Files identical despite different names*

### Comparing `chichitk-0.0.2/chichitk.egg-info/PKG-INFO` & `chichitk-0.0.3/chichitk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chichitk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python UI library built upon Tkinter
 Author-email: Samuel Gibson <samuelpgibson12@gmail.com>
 Project-URL: Homepage, https://github.com/SamGibson1/ChichiTk
 Project-URL: Documentation, https://github.com/SamGibson1/ChichiTk/wiki
 Project-URL: Bug Tracker, https://github.com/SamGibson1/ChichiTk/issues
 Keywords: python,tkinter,custom,widgets
 Classifier: Development Status :: 3 - Alpha
@@ -39,15 +39,15 @@
 Update as often as possible because this library is under active development.
 
 ## Documentation
 The **official** documentation can be found in the Wiki Tab here:
 
 **--> [ChichiTk Documentation](https://github.com/SamGibson1/ChichiTk/wiki)**
 
-## Example Program
+## Example Program - Stopwatch
 The following is a simple Stopwatch program that uses chichitk.Player to manage callbacks:
 ```python
 from tkinter import Tk, Frame, Label
 from chichitk import Player
 
 def time_text(time:int, f:int=100):
     hour = time // (3600 * f)
@@ -70,11 +70,17 @@
 Play = Player(frame, lambda t: label.config(text=time_text(t)), 0.01,
               bg='#1e1e22', frame_num=12001, frame_rate=100, step_increment=500)
 Play.pack(side='bottom', fill='x')
 
 app.mainloop()
 ```
 This results in the following window:
+
 <img src="documentation_images/stopwatch_example.jpg" width="600"/>
 
-<!-- ## Example Application - Password Manager
-Video here showing password manager and link to git repo for password manager -->
+## Example Application - Password Manager
+
+https://user-images.githubusercontent.com/74847576/233730056-cffb5a0d-41db-44e4-ad24-7276406f9ba1.mp4
+
+The Passwords App project can be found here:
+
+**--> [Project Link](https://github.com/SamGibson1/PasswordManager)**
```

### Comparing `chichitk-0.0.2/chichitk.egg-info/SOURCES.txt` & `chichitk-0.0.3/chichitk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 Readme.md
 pyproject.toml
 chichitk/__init__.py
 chichitk/aspect_frame.py
 chichitk/buttons.py
 chichitk/canvas_items.py
+chichitk/collapse_frame.py
 chichitk/dropdowns.py
 chichitk/entry_boxes.py
 chichitk/file_dialog.py
 chichitk/function_progress.py
 chichitk/icons.py
 chichitk/labels.py
 chichitk/pdf_display.py
```

### Comparing `chichitk-0.0.2/pyproject.toml` & `chichitk-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chichitk"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Samuel Gibson", email="samuelpgibson12@gmail.com" },
 ]
 description = "Python UI library built upon Tkinter"
 readme = "Readme.md"
 requires-python = ">=3.7"
 dependencies = ["opencv-python", "numpy", "Pillow", "PyMuPDF"]
@@ -19,13 +19,20 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools.packages.find]
 include = ["chichitk*"]  # package names should match these glob patterns (["*"] by default)
-exclude = ["chichitk_env*", "documentation_images*", "example.pdf", "example.docx", "example.py", "stopwatch_example.py"]  # exclude packages matching these glob patterns (empty by default)
+exclude = [
+    "chichitk_env*",
+    "documentation_images*",
+    "example.pdf",
+    "example.docx",
+    "example.py",
+    "stopwatch_example.py"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/SamGibson1/ChichiTk"
 "Documentation" = "https://github.com/SamGibson1/ChichiTk/wiki"
 "Bug Tracker" = "https://github.com/SamGibson1/ChichiTk/issues"
```

