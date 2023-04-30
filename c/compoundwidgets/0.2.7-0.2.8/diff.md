# Comparing `tmp/compoundwidgets-0.2.7.tar.gz` & `tmp/compoundwidgets-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compoundwidgets-0.2.7.tar", last modified: Wed Apr 26 10:08:27 2023, max compression
+gzip compressed data, was "compoundwidgets-0.2.8.tar", last modified: Sun Apr 30 12:29:22 2023, max compression
```

## Comparing `compoundwidgets-0.2.7.tar` & `compoundwidgets-0.2.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.503050 compoundwidgets-0.2.7/
--rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      332 2023-04-26 10:08:27.502051 compoundwidgets-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2023-04-21 13:55:20.000000 compoundwidgets-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.369835 compoundwidgets-0.2.7/compoundwidgets/
--rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.7/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
--rw-rw-rw-   0        0        0    54792 2023-04-26 10:05:01.000000 compoundwidgets-0.2.7/compoundwidgets/COMPOUND_WIDGETS.py
--rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.7/compoundwidgets/CUSTOM_BUTTONS.py
--rw-rw-rw-   0        0        0    16474 2023-04-17 20:34:54.000000 compoundwidgets-0.2.7/compoundwidgets/CUSTOM_FRAMES.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.436095 compoundwidgets-0.2.7/compoundwidgets/IMAGES/
--rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/__init__.py
--rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/add_new.png
--rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/add_to_form.png
--rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/back.png
--rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/calculate.png
--rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/clear.png
--rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/edit_form.png
--rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/help.png
--rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/no.png
--rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/quit.png
--rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/remove_from_form.png
--rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/save.png
--rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/trash_can.png
--rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/yes.png
--rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.7/compoundwidgets/LED_BUTTONS.py
--rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.7/compoundwidgets/MESSAGE_BOX_WIDGETS.py
--rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.7/compoundwidgets/SCRIPTS.py
--rw-rw-rw-   0        0        0     1843 2023-04-26 10:08:19.000000 compoundwidgets-0.2.7/compoundwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.411755 compoundwidgets-0.2.7/compoundwidgets.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 10:08:27.503050 compoundwidgets-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-04-26 10:08:19.000000 compoundwidgets-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.501052 compoundwidgets-0.2.7/test/
--rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.7/test/autocomplete_widget_test.py
--rw-rw-rw-   0        0        0    10106 2023-04-17 13:00:19.000000 compoundwidgets-0.2.7/test/compound_widgets_test_1.py
--rw-rw-rw-   0        0        0     7306 2023-04-17 12:42:39.000000 compoundwidgets-0.2.7/test/compound_widgets_test_2.py
--rw-rw-rw-   0        0        0      991 2023-04-26 10:06:43.000000 compoundwidgets-0.2.7/test/custom_buttons_test.py
--rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.7/test/custom_frames_test_1.py
--rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.7/test/custom_frames_test_2.py
--rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.7/test/custom_frames_test_3.py
--rw-rw-rw-   0        0        0     2745 2023-04-17 20:15:42.000000 compoundwidgets-0.2.7/test/custom_frames_test_4.py
--rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.7/test/led_buttons_test.py
--rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.7/test/message_box_test.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:29:22.241761 compoundwidgets-0.2.8/
+-rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      332 2023-04-30 12:29:22.240763 compoundwidgets-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2023-04-21 13:55:20.000000 compoundwidgets-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 12:29:22.078373 compoundwidgets-0.2.8/compoundwidgets/
+-rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.8/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
+-rw-rw-rw-   0        0        0    54974 2023-04-30 12:27:30.000000 compoundwidgets-0.2.8/compoundwidgets/COMPOUND_WIDGETS.py
+-rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.8/compoundwidgets/CUSTOM_BUTTONS.py
+-rw-rw-rw-   0        0        0    16474 2023-04-17 20:34:54.000000 compoundwidgets-0.2.8/compoundwidgets/CUSTOM_FRAMES.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:29:22.153353 compoundwidgets-0.2.8/compoundwidgets/IMAGES/
+-rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/__init__.py
+-rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/add_new.png
+-rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/add_to_form.png
+-rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/back.png
+-rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/calculate.png
+-rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/clear.png
+-rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/edit_form.png
+-rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/help.png
+-rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/no.png
+-rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/quit.png
+-rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/remove_from_form.png
+-rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/save.png
+-rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/trash_can.png
+-rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.8/compoundwidgets/IMAGES/yes.png
+-rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.8/compoundwidgets/LED_BUTTONS.py
+-rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.8/compoundwidgets/MESSAGE_BOX_WIDGETS.py
+-rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.8/compoundwidgets/SCRIPTS.py
+-rw-rw-rw-   0        0        0     1843 2023-04-30 12:29:00.000000 compoundwidgets-0.2.8/compoundwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:29:22.106787 compoundwidgets-0.2.8/compoundwidgets.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-30 12:29:21.000000 compoundwidgets-0.2.8/compoundwidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-04-30 12:29:21.000000 compoundwidgets-0.2.8/compoundwidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 12:29:21.000000 compoundwidgets-0.2.8/compoundwidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-30 12:29:21.000000 compoundwidgets-0.2.8/compoundwidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-30 12:29:21.000000 compoundwidgets-0.2.8/compoundwidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 12:29:22.241761 compoundwidgets-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-04-30 12:29:00.000000 compoundwidgets-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:29:22.238773 compoundwidgets-0.2.8/test/
+-rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.8/test/autocomplete_widget_test.py
+-rw-rw-rw-   0        0        0    10148 2023-04-26 10:36:20.000000 compoundwidgets-0.2.8/test/compound_widgets_test_1.py
+-rw-rw-rw-   0        0        0     7306 2023-04-17 12:42:39.000000 compoundwidgets-0.2.8/test/compound_widgets_test_2.py
+-rw-rw-rw-   0        0        0      991 2023-04-26 10:06:43.000000 compoundwidgets-0.2.8/test/custom_buttons_test.py
+-rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.8/test/custom_frames_test_1.py
+-rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.8/test/custom_frames_test_2.py
+-rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.8/test/custom_frames_test_3.py
+-rw-rw-rw-   0        0        0     2745 2023-04-17 20:15:42.000000 compoundwidgets-0.2.8/test/custom_frames_test_4.py
+-rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.8/test/led_buttons_test.py
+-rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.8/test/message_box_test.py
```

### Comparing `compoundwidgets-0.2.7/LICENSE.txt` & `compoundwidgets-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/MANIFEST.in` & `compoundwidgets-0.2.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/README.md` & `compoundwidgets-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/AUTOCOMPLETE_WIDGETS.py` & `compoundwidgets-0.2.8/compoundwidgets/AUTOCOMPLETE_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/COMPOUND_WIDGETS.py` & `compoundwidgets-0.2.8/compoundwidgets/COMPOUND_WIDGETS.py`

 * *Files 0% similar despite different names*

```diff
@@ -895,20 +895,24 @@
         self.is_locked = False
 
     def activate_self_conversion(self):
         self.unlock_unit()
         self.enable()
         self.entry.config(state='readonly')
         self.combobox_unit_conversion = True
+        if self.entry_method:
+            self.unit_combo.unbind("<<ComboboxSelected>>")
         self.unit_combo.bind("<<ComboboxSelected>>", self._convert_to_selected_unit)
 
     def deactivate_self_conversion(self):
         self.enable()
         self.combobox_unit_conversion = False
-        self.unit_combo.bind("<<ComboboxSelected>>", self.entry_method)
+        self.unit_combo.unbind("<<ComboboxSelected>>")
+        if self.entry_method:
+            self.unit_combo.bind("<<ComboboxSelected>>", self.entry_method)
 
     # Widget set and get methods ---------------------------------------------------------------------------------------
     def get_entry(self):
         return self.entry_variable.get()
 
     def set_entry(self, value):
         if str(self.entry.cget('state')) == 'disabled':
```

### Comparing `compoundwidgets-0.2.7/compoundwidgets/CUSTOM_BUTTONS.py` & `compoundwidgets-0.2.8/compoundwidgets/CUSTOM_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/CUSTOM_FRAMES.py` & `compoundwidgets-0.2.8/compoundwidgets/CUSTOM_FRAMES.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/add_new.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/add_new.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/add_to_form.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/add_to_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/back.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/back.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/calculate.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/calculate.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/clear.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/clear.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/edit_form.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/edit_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/help.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/help.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/no.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/no.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/quit.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/quit.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/remove_from_form.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/remove_from_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/save.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/save.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/trash_can.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/trash_can.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/IMAGES/yes.png` & `compoundwidgets-0.2.8/compoundwidgets/IMAGES/yes.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/LED_BUTTONS.py` & `compoundwidgets-0.2.8/compoundwidgets/LED_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/MESSAGE_BOX_WIDGETS.py` & `compoundwidgets-0.2.8/compoundwidgets/MESSAGE_BOX_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/SCRIPTS.py` & `compoundwidgets-0.2.8/compoundwidgets/SCRIPTS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/compoundwidgets/__init__.py` & `compoundwidgets-0.2.8/compoundwidgets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.07"
+__version__ = "0.2.08"
 __author__ = 'Andre Mariano'
 __all__ = ['AUTOCOMPLETE_WIDGETS',
            'COMPOUND_WIDGETS',
            'CUSTOM_BUTTONS',
            'CUSTOM_FRAMES',
            'MESSAGE_BOX_WIDGETS',
            'IMAGES',
```

### Comparing `compoundwidgets-0.2.7/compoundwidgets.egg-info/SOURCES.txt` & `compoundwidgets-0.2.8/compoundwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/setup.py` & `compoundwidgets-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='compoundwidgets',
-    version='0.2.07',
+    version='0.2.08',
     author='Andre Mariano',
     license="MIT",
     url='https://github.com/AndreMariano100/CompoundWidgets.git',
     description='Compound TTK Widgets with ttkbootstrap',
     author_email='andremariano100@gmail.com',
     packages=['compoundwidgets', 'compoundwidgets.IMAGES'],
     install_requires=['ttkbootstrap', 'Pillow'],
```

### Comparing `compoundwidgets-0.2.7/test/autocomplete_widget_test.py` & `compoundwidgets-0.2.8/test/autocomplete_widget_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/test/compound_widgets_test_1.py` & `compoundwidgets-0.2.8/test/compound_widgets_test_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,18 @@
     frame.columnconfigure(0, weight=1)
 
     local_list = ('1000', '2000.00', 'Label Entry', 'Label Entry', 'Very Long Label Entry')
     label_entry_list = []
     for i, item in enumerate(local_list):
         if i in range(3):
             w = cw.LabelEntry(frame, label_text=f'Label Entry {i+1}', label_width=10, entry_method=get_all_label_entries,
-                              entry_numeric=True, entry_value=item, entry_max_char=10)
+                              entry_numeric=True, entry_value=item, entry_max_char=10, trace_variable=True)
         else:
             w = cw.LabelEntry(frame, label_text=f'Label Entry {i+1}', label_width=10, entry_method=get_all_label_entries,
-                              entry_numeric=False, entry_value=item, entry_max_char=10)
+                              entry_numeric=False, entry_value=item, entry_max_char=10, trace_variable=True)
         w.grid(row=i, column=0, sticky='nsew', pady=2)
         label_entry_list.append(w)
         if i == 2:
             w.readonly()
         if i == 3:
             w.disable()
```

### Comparing `compoundwidgets-0.2.7/test/compound_widgets_test_2.py` & `compoundwidgets-0.2.8/test/compound_widgets_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/test/custom_buttons_test.py` & `compoundwidgets-0.2.8/test/custom_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/test/custom_frames_test_1.py` & `compoundwidgets-0.2.8/test/custom_frames_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/test/custom_frames_test_2.py` & `compoundwidgets-0.2.8/test/custom_frames_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/test/custom_frames_test_3.py` & `compoundwidgets-0.2.8/test/custom_frames_test_3.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/test/custom_frames_test_4.py` & `compoundwidgets-0.2.8/test/custom_frames_test_4.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/test/led_buttons_test.py` & `compoundwidgets-0.2.8/test/led_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.7/test/message_box_test.py` & `compoundwidgets-0.2.8/test/message_box_test.py`

 * *Files identical despite different names*

