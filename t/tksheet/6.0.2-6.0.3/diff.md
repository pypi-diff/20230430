# Comparing `tmp/tksheet-6.0.2.tar.gz` & `tmp/tksheet-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.0.2.tar", last modified: Wed Apr 26 17:06:09 2023, max compression
+gzip compressed data, was "tksheet-6.0.3.tar", last modified: Sun Apr 30 15:35:43 2023, max compression
```

## Comparing `tksheet-6.0.2.tar` & `tksheet-6.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 17:06:09.864195 tksheet-6.0.2/
--rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3003 2023-04-26 17:06:09.864195 tksheet-6.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-04-24 17:49:11.000000 tksheet-6.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-04-26 17:06:09.864195 tksheet-6.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-04-24 17:51:18.000000 tksheet-6.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:06:09.848570 tksheet-6.0.2/tksheet/
--rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.2/tksheet/__init__.py
--rw-rw-rw-   0        0        0   164503 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0    99400 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0    10233 2023-04-24 07:09:26.000000 tksheet-6.0.2/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   329896 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12952 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0    99164 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5642 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    52264 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:06:09.864195 tksheet-6.0.2/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3003 2023-04-26 17:06:09.000000 tksheet-6.0.2/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-26 17:06:09.000000 tksheet-6.0.2/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 17:06:09.000000 tksheet-6.0.2/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 17:06:09.000000 tksheet-6.0.2/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 15:35:43.047748 tksheet-6.0.3/
+-rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3003 2023-04-30 15:35:43.047748 tksheet-6.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-04-29 12:52:53.000000 tksheet-6.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-30 15:35:43.047748 tksheet-6.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-04-26 17:49:39.000000 tksheet-6.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:35:43.032125 tksheet-6.0.3/tksheet/
+-rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.3/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   165005 2023-04-30 15:29:07.000000 tksheet-6.0.3/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   103939 2023-04-30 14:48:10.000000 tksheet-6.0.3/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0    10233 2023-04-24 07:09:26.000000 tksheet-6.0.3/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   321463 2023-04-30 11:33:25.000000 tksheet-6.0.3/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    14797 2023-04-30 11:47:18.000000 tksheet-6.0.3/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   102184 2023-04-30 08:50:43.000000 tksheet-6.0.3/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5646 2023-04-29 16:37:13.000000 tksheet-6.0.3/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    52360 2023-04-30 11:47:39.000000 tksheet-6.0.3/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:35:43.047748 tksheet-6.0.3/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3003 2023-04-30 15:35:43.000000 tksheet-6.0.3/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-30 15:35:43.000000 tksheet-6.0.3/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 15:35:43.000000 tksheet-6.0.3/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 15:35:43.000000 tksheet-6.0.3/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.0.2/LICENSE.txt` & `tksheet-6.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.2/PKG-INFO` & `tksheet-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.0.2
+Version: 6.0.3
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.0.2.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.3.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.0.2/README.md` & `tksheet-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.2/setup.py` & `tksheet-6.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.0.2',
+  version = '6.0.3',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.2.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.3.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.0.2/tksheet/_tksheet.py` & `tksheet-6.0.3/tksheet/_tksheet.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,22 +45,22 @@
                  data: list = None,
                  startup_select: tuple = None, #either (start row, end row, "rows"), (start column, end column, "rows") or (cells start row, cells start column, cells end row, cells end column, "cells")
                  startup_focus: bool = True,
                  total_columns: int = None,
                  total_rows: int = None,
                  column_width: int = 120,
                  header_height: str = "1", #str or int
-                 max_colwidth: str = "inf", #str or int
-                 max_rh: str = "inf", #str or int
+                 max_column_width: str = "inf", #str or int
+                 max_row_height: str = "inf", #str or int
                  max_header_height: str = "inf", #str or int
-                 max_row_width: str = "inf", #str or int
+                 max_index_width: str = "inf", #str or int
                  row_index: list = None,
                  index: list = None,
-                 after_redraw_time_ms: int = 50,
-                 row_index_width: int = 100,
+                 after_redraw_time_ms: int = 20,
+                 row_index_width: int = None,
                  auto_resize_default_row_index: bool = True,
                  set_all_heights_and_widths: bool = False,
                  row_height: str = "1", #str or int
                  font: tuple = get_font(),
                  header_font: tuple = get_heading_font(),
                  index_font: tuple = get_index_font(), #currently has no effect
                  popup_menu_font: tuple = get_font(),
@@ -145,17 +145,14 @@
         if width is not None and height is None:
             self.config(height = 300)
         if height is not None and width is None:
             self.config(width = 350)
         self.grid_columnconfigure(1, weight = 1)
         self.grid_rowconfigure(1, weight = 1)
         self.RI = RowIndex(parentframe = self,
-                           max_rh = max_rh,
-                           max_row_width = max_row_width,
-                           row_index_width = row_index_width,
                            row_index_align = self.convert_align(row_index_align),
                            index_bg = index_bg,
                            index_border_fg = index_border_fg,
                            index_grid_fg = index_grid_fg,
                            index_fg = index_fg,
                            index_selected_cells_bg = index_selected_cells_bg,
                            index_selected_cells_fg = index_selected_cells_fg,
@@ -165,16 +162,14 @@
                            drag_and_drop_bg = drag_and_drop_bg,
                            resizing_line_fg = resizing_line_fg,
                            row_drag_and_drop_perform = row_drag_and_drop_perform,
                            default_row_index = default_row_index,
                            auto_resize_width = auto_resize_default_row_index,
                            show_default_index_for_empty = show_default_index_for_empty)
         self.CH = ColumnHeaders(parentframe = self,
-                                max_colwidth = max_colwidth,
-                                max_header_height = max_header_height,
                                 default_header = default_header,
                                 header_align = self.convert_align(header_align),
                                 header_bg = header_bg,
                                 header_border_fg = header_border_fg,
                                 header_grid_fg = header_grid_fg,
                                 header_fg = header_fg,
                                 header_selected_cells_bg = header_selected_cells_bg,
@@ -183,38 +178,43 @@
                                 header_selected_columns_fg = header_selected_columns_fg,
                                 header_hidden_columns_expander_bg = header_hidden_columns_expander_bg,
                                 drag_and_drop_bg = drag_and_drop_bg,
                                 column_drag_and_drop_perform = column_drag_and_drop_perform,
                                 resizing_line_fg = resizing_line_fg,
                                 show_default_header_for_empty = show_default_header_for_empty)
         self.MT = MainTable(parentframe = self,
+                            max_column_width = max_column_width,
+                            max_header_height = max_header_height,
+                            max_row_height = max_row_height,
+                            max_index_width = max_index_width,
+                            row_index_width = row_index_width,
+                            header_height = header_height,
+                            column_width = column_width,
+                            row_height = row_height,
                             show_index = show_row_index,
                             show_header = show_header,
                             enable_edit_cell_auto_resize = enable_edit_cell_auto_resize,
                             edit_cell_validation = edit_cell_validation,
                             page_up_down_select_row = page_up_down_select_row,
                             expand_sheet_if_paste_too_big = expand_sheet_if_paste_too_big,
                             paste_insert_column_limit = paste_insert_column_limit,
                             paste_insert_row_limit = paste_insert_row_limit,
                             show_dropdown_borders = show_dropdown_borders,
                             arrow_key_down_right_scroll_page = arrow_key_down_right_scroll_page,
                             display_selected_fg_over_highlights = display_selected_fg_over_highlights,
                             show_vertical_grid = show_vertical_grid,
                             show_horizontal_grid = show_horizontal_grid,
-                            column_width = column_width,
-                            row_height = row_height,
                             to_clipboard_delimiter = to_clipboard_delimiter,
                             to_clipboard_quotechar = to_clipboard_quotechar,
                             to_clipboard_lineterminator = to_clipboard_lineterminator,
                             from_clipboard_delimiters = from_clipboard_delimiters,
                             column_headers_canvas = self.CH,
                             row_index_canvas = self.RI,
                             headers = headers,
                             header = header,
-                            header_height = header_height,
                             data_reference = data if data_reference is None else data_reference,
                             total_cols = total_columns,
                             total_rows = total_rows,
                             row_index = row_index,
                             index = index,
                             font = font,
                             header_font = header_font,
@@ -447,61 +447,68 @@
             if label in self.MT.extra_header_rc_menu_funcs:
                 del self.MT.extra_header_rc_menu_funcs[label]
             if label in self.MT.extra_empty_space_rc_menu_funcs:
                 del self.MT.extra_empty_space_rc_menu_funcs[label]
         self.MT.create_rc_menus()
 
     def extra_bindings(self, bindings, func = None):
+        if func is not None and isinstance(bindings, str) and bindings.lower() in emitted_events:
+            self.bind_event(bindings, func)
+        
         if isinstance(bindings, str) and bindings.lower() in ("all", "bind_all", "unbind_all"):
             self.MT.extra_begin_ctrl_c_func = func
             self.MT.extra_begin_ctrl_x_func = func
             self.MT.extra_begin_ctrl_v_func = func
             self.MT.extra_begin_ctrl_z_func = func
             self.MT.extra_begin_delete_key_func = func
             self.RI.ri_extra_begin_drag_drop_func = func
             self.CH.ch_extra_begin_drag_drop_func = func
             self.MT.extra_begin_del_rows_rc_func = func
             self.MT.extra_begin_del_cols_rc_func = func
             self.MT.extra_begin_insert_cols_rc_func = func
             self.MT.extra_begin_insert_rows_rc_func = func
-            
-            self.MT.extra_end_ctrl_c_func = func
-            self.MT.extra_end_ctrl_x_func = func
-            self.MT.extra_end_ctrl_v_func = func
-            self.MT.extra_end_ctrl_z_func = func
-            self.MT.extra_end_delete_key_func = func
-            
             self.MT.extra_begin_edit_cell_func = func
-            self.MT.extra_end_edit_cell_func = func
             self.CH.extra_begin_edit_cell_func = func
-            self.CH.extra_end_edit_cell_func = func
             self.RI.extra_begin_edit_cell_func = func
-            self.RI.extra_end_edit_cell_func = func
-            
-            self.RI.ri_extra_end_drag_drop_func = func
-            self.CH.ch_extra_end_drag_drop_func = func
-            self.MT.extra_end_del_rows_rc_func = func
-            self.MT.extra_end_del_cols_rc_func = func
-            self.MT.extra_end_insert_cols_rc_func = func
-            self.MT.extra_end_insert_rows_rc_func = func
+            self.CH.column_width_resize_func = func
+            self.RI.row_height_resize_func = func
             
+        if isinstance(bindings, str) and bindings.lower() in ("all", "bind_all", "unbind_all", "all_select_events", "select", "selectevents", "select_events"):
             self.MT.selection_binding_func = func
             self.MT.select_all_binding_func = func
             self.RI.selection_binding_func = func
             self.CH.selection_binding_func = func
             self.MT.drag_selection_binding_func = func
             self.RI.drag_selection_binding_func = func
             self.CH.drag_selection_binding_func = func
             self.MT.shift_selection_binding_func = func
             self.RI.shift_selection_binding_func = func
             self.CH.shift_selection_binding_func = func
+            self.MT.ctrl_selection_binding_func = func
+            self.RI.ctrl_selection_binding_func = func
+            self.CH.ctrl_selection_binding_func = func
             self.MT.deselection_binding_func = func
-
-            self.CH.column_width_resize_func = func
-            self.RI.row_height_resize_func = func
+            
+        if isinstance(bindings, str) and bindings.lower() in ("all", "bind_all", "unbind_all", "all_modified_events", 
+                                                              "sheetmodified", "sheet_modified" "modified_events", "modified"):
+            self.MT.extra_end_ctrl_c_func = func
+            self.MT.extra_end_ctrl_x_func = func
+            self.MT.extra_end_ctrl_v_func = func
+            self.MT.extra_end_ctrl_z_func = func
+            self.MT.extra_end_delete_key_func = func
+            self.RI.ri_extra_end_drag_drop_func = func
+            self.CH.ch_extra_end_drag_drop_func = func
+            self.MT.extra_end_del_rows_rc_func = func
+            self.MT.extra_end_del_cols_rc_func = func
+            self.MT.extra_end_insert_cols_rc_func = func
+            self.MT.extra_end_insert_rows_rc_func = func
+            self.MT.extra_end_edit_cell_func = func
+            self.CH.extra_end_edit_cell_func = func
+            self.RI.extra_end_edit_cell_func = func
+            
         else:
             if isinstance(bindings[0], str) and not isinstance(bindings, str):
                 iterable = [bindings]
             elif isinstance(bindings, str):
                 iterable = [(bindings, func)]
             else:
                 iterable = bindings
@@ -598,29 +605,37 @@
                     self.CH.drag_selection_binding_func = func
                 if binding == "shift_cell_select":
                     self.MT.shift_selection_binding_func = func
                 if binding == "shift_row_select":
                     self.RI.shift_selection_binding_func = func
                 if binding == "shift_column_select":
                     self.CH.shift_selection_binding_func = func
+                if binding == "ctrl_cell_select":
+                    self.MT.ctrl_selection_binding_func = func
+                if binding == "ctrl_row_select":
+                    self.RI.ctrl_selection_binding_func = func
+                if binding == "ctrl_column_select":
+                    self.CH.ctrl_selection_binding_func = func
                 if binding == "deselect":
                     self.MT.deselection_binding_func = func
-                    
-                if binding == "all_select_events":
-                    self.MT.selection_binding_func = func
-                    self.MT.select_all_binding_func = func
-                    self.RI.selection_binding_func = func
-                    self.CH.selection_binding_func = func
-                    self.MT.drag_selection_binding_func = func
-                    self.RI.drag_selection_binding_func = func
-                    self.CH.drag_selection_binding_func = func
-                    self.MT.shift_selection_binding_func = func
-                    self.RI.shift_selection_binding_func = func
-                    self.CH.shift_selection_binding_func = func
-                    self.MT.deselection_binding_func = func
+
+    def emit_modified_event(self, data = {}):
+        self.event_generate("<<SheetModified>>", data = data)
+
+    def bind_event(self, sequence, func, add = None):
+        widget = self
+        def _substitute(*args):
+            e = lambda: None 
+            e.data = eval(args[0])
+            e.widget = widget
+            return (e,)
+
+        funcid = widget._register(func, _substitute, needcleanup = 1)
+        cmd = '{0}if {{"[{1} %d]" == "break"}} break\n'.format('+' if add else '', funcid)
+        widget.tk.call('bind', widget._w, sequence, cmd)
 
     def bind(self, binding, func, add = None):
         if binding == "<ButtonPress-1>":
             self.MT.extra_b1_press_func = func
             self.CH.extra_b1_press_func = func
             self.RI.extra_b1_press_func = func
             self.TL.extra_b1_press_func = func
@@ -640,15 +655,15 @@
             self.RI.extra_double_b1_func = func
             self.TL.extra_double_b1_func = func
         elif binding == "<Motion>":
             self.MT.extra_motion_func = func
             self.CH.extra_motion_func = func
             self.RI.extra_motion_func = func
             self.TL.extra_motion_func = func
-        elif binding == get_rc_binding():
+        elif binding == rc_binding:
             self.MT.extra_rc_func = func
             self.CH.extra_rc_func = func
             self.RI.extra_rc_func = func
             self.TL.extra_rc_func = func
         else:
             self.MT.bind(binding, func, add =  add)
             self.CH.bind(binding, func, add =  add)
@@ -677,15 +692,15 @@
             self.RI.extra_double_b1_func = None
             self.TL.extra_double_b1_func = None
         elif binding == "<Motion>":
             self.MT.extra_motion_func = None
             self.CH.extra_motion_func = None
             self.RI.extra_motion_func = None
             self.TL.extra_motion_func = None
-        elif binding == get_rc_binding():
+        elif binding == rc_binding:
             self.MT.extra_rc_func = None
             self.CH.extra_rc_func = None
             self.RI.extra_rc_func = None
             self.TL.extra_rc_func = None
         else:
             self.MT.unbind(binding)
             self.CH.unbind(binding)
@@ -742,21 +757,21 @@
         elif ev_w == self.CH:
             if exclude_header:
                 return None
             else:
                 return self.MT.identify_col(x = event.x, allow_end = allow_end)
 
     def get_example_canvas_column_widths(self, total_cols = None):
-        colpos = int(self.MT.default_cw)
+        colpos = int(self.MT.default_column_width)
         if total_cols is not None:
             return list(accumulate(chain([0], (colpos for c in range(total_cols)))))
         return list(accumulate(chain([0], (colpos for c in range(len(self.MT.col_positions) - 1)))))
 
     def get_example_canvas_row_heights(self, total_rows = None):
-        rowpos = self.MT.default_rh[1]
+        rowpos = self.MT.default_row_height[1]
         if total_rows is not None:
             return list(accumulate(chain([0], (rowpos for c in range(total_rows)))))
         return list(accumulate(chain([0], (rowpos for c in range(len(self.MT.row_positions) - 1)))))
 
     def get_column_widths(self, canvas_positions = False):
         if canvas_positions:
             return [int(n) for n in self.MT.col_positions]
@@ -810,17 +825,20 @@
     def set_all_row_heights(self, height = None, only_set_if_too_small = False, redraw = True, recreate_selection_boxes = True):
         self.RI.set_height_of_all_rows(height = height, only_set_if_too_small = only_set_if_too_small, recreate = recreate_selection_boxes)
         self.set_refresh_timer(redraw)
 
     def set_cell_size_to_text(self, row, column, only_set_if_too_small = False, redraw = True):
         self.MT.set_cell_size_to_text(r = row, c = column, only_set_if_too_small = only_set_if_too_small)
         self.set_refresh_timer(redraw)
-
-    def set_width_of_index_to_text(self, recreate = True):
-        self.RI.set_width_of_index_to_text(recreate = recreate)
+                                                      # backwards compatibility
+    def set_width_of_index_to_text(self, text = None, *args, **kwargs):
+        self.RI.set_width_of_index_to_text(text = text)
+        
+    def set_height_of_header_to_text(self, text = None):
+        self.CH.set_height_of_header_to_text(text = text)
 
     def row_height(self, row = None, height = None, only_set_if_too_small = False, redraw = True):
         if row == "all":
             if height == "default":
                 self.MT.reset_row_positions()
         elif row == "displayed":
             if height == "text":
@@ -836,15 +854,15 @@
         self.set_refresh_timer(redraw)
 
     def set_row_heights(self, row_heights = None, canvas_positions = False, reset = False, verify = False):
         if reset:
             self.MT.reset_row_positions()
             return
         if is_iterable(row_heights):
-            qmin = self.MT.min_rh
+            qmin = self.MT.min_row_height
             if canvas_positions and isinstance(row_heights, list):
                 if verify:
                     self.MT.row_positions = list(accumulate(chain([0], (height if qmin < height else qmin
                                                                         for height in [x - z for z, x in zip(islice(row_heights, 0, None),
                                                                                                              islice(row_heights, 1, None))]))))
                 else:
                     self.MT.row_positions = row_heights
@@ -856,51 +874,53 @@
 
     def verify_row_heights(self, row_heights: list, canvas_positions = False):
         if row_heights[0] != 0 or isinstance(row_heights[0], bool):
             return False
         if not isinstance(row_heights, list):
             return False
         if canvas_positions:
-            if any(x - z < self.MT.min_rh or not isinstance(x, int) or isinstance(x, bool) for z, x in zip(islice(row_heights, 0, None), islice(row_heights, 1, None))):
+            if any(x - z < self.MT.min_row_height or not isinstance(x, int) or isinstance(x, bool) for z, x in zip(islice(row_heights, 0, None), islice(row_heights, 1, None))):
                 return False
         elif not canvas_positions:
-            if any(z < self.MT.min_rh or not isinstance(z, int) or isinstance(z, bool) for z in row_heights):
+            if any(z < self.MT.min_row_height or not isinstance(z, int) or isinstance(z, bool) for z in row_heights):
                 return False
         return True
 
     def verify_column_widths(self, column_widths: list, canvas_positions = False):
         if column_widths[0] != 0 or isinstance(column_widths[0], bool):
             return False
         if not isinstance(column_widths, list):
             return False
         if canvas_positions:
-            if any(x - z < self.MT.min_cw or not isinstance(x, int) or isinstance(x, bool) for z, x in zip(islice(column_widths, 0, None), islice(column_widths, 1, None))):
+            if any(x - z < self.MT.min_column_width or not isinstance(x, int) or isinstance(x, bool) for z, x in zip(islice(column_widths, 0, None), islice(column_widths, 1, None))):
                 return False
         elif not canvas_positions:
-            if any(z < self.MT.min_cw or not isinstance(z, int) or isinstance(z, bool) for z in column_widths):
+            if any(z < self.MT.min_column_width or not isinstance(z, int) or isinstance(z, bool) for z in column_widths):
                 return False
         return True
 
     def default_row_height(self, height = None):
         if height is not None:
-            self.MT.default_rh = (height if isinstance(height, str) else "pixels", height if isinstance(height, int) else self.MT.GetLinesHeight(int(height)))
-        return self.MT.default_rh[1]
+            self.MT.default_row_height = (height if isinstance(height, str) else "pixels", 
+                                          height if isinstance(height, int) else self.MT.get_lines_cell_height(int(height)))
+        return self.MT.default_row_height[1]
 
     def default_header_height(self, height = None):
         if height is not None:
-            self.MT.default_hh = (height if isinstance(height, str) else "pixels", height if isinstance(height, int) else self.MT.GetHdrLinesHeight(int(height)))
-        return self.MT.default_hh[1]
+            self.MT.default_header_height = (height if isinstance(height, str) else "pixels", 
+                                             height if isinstance(height, int) else self.MT.get_lines_cell_height(int(height), font = self.MT.header_font))
+        return self.MT.default_header_height[1]
 
     def default_column_width(self, width = None):
         if width is not None:
-            if width < self.MT.min_cw:
-                self.MT.default_cw = self.MT.min_cw + 20
+            if width < self.MT.min_column_width:
+                self.MT.default_column_width = self.MT.min_column_width + 20
             else:
-                self.MT.default_cw = int(width)
-        return self.MT.default_cw
+                self.MT.default_column_width = int(width)
+        return self.MT.default_column_width
 
     def cut(self, event = None):
         self.MT.ctrl_x()
 
     def copy(self, event = None):
         self.MT.ctrl_c()
 
@@ -909,17 +929,14 @@
 
     def delete(self, event = None):
         self.MT.delete_key()
 
     def undo(self, event = None):
         self.MT.ctrl_z()
 
-    def edit_cell(self, event = None, dropdown = False):
-        self.MT.edit_cell_(event = event, dropdown = dropdown)
-
     def delete_row_position(self, idx: int, deselect_all = False):
         self.MT.del_row_position(idx = idx,
                                  deselect_all = deselect_all)
 
     def delete_row(self, idx = 0, deselect_all = False, redraw = True):
         self.delete_rows(rows = {idx}, deselect_all = deselect_all, redraw = False)
         self.set_refresh_timer(redraw)
@@ -963,15 +980,15 @@
     def total_rows(self, number = None, mod_positions = True, mod_data = True):
         if number is None:
             return int(self.MT.total_data_rows())
         if not isinstance(number, int) or number < 0:
             raise ValueError("number argument must be integer and > 0")
         if number > len(self.MT.data):
             if mod_positions:
-                height = self.MT.GetLinesHeight(int(self.MT.default_rh[0]))
+                height = self.MT.get_lines_cell_height(int(self.MT.default_row_height[0]))
                 for r in range(number - len(self.MT.data)):
                     self.MT.insert_row_position("end", height)
         elif number < len(self.MT.data):
             if not self.MT.all_rows_displayed:
                 self.MT.display_rows(enable = False, reset_row_positions = False, deselect_all = True)
             self.MT.row_positions[number + 1:] = []
         if mod_data:
@@ -981,32 +998,32 @@
         total_cols = self.MT.total_data_cols()
         if number is None:
             return int(total_cols)
         if not isinstance(number, int) or number < 0:
             raise ValueError("number argument must be integer and > 0")
         if number > total_cols:
             if mod_positions:
-                width = self.MT.default_cw
+                width = self.MT.default_column_width
                 for c in range(number - total_cols):
                     self.MT.insert_col_position("end", width)
         elif number < total_cols:
             if not self.MT.all_columns_displayed:
                 self.MT.display_columns(enable = False, reset_col_positions = False, deselect_all = True)
             self.MT.col_positions[number + 1:] = []
         if mod_data:
             self.MT.data_dimensions(total_columns = number)
 
     def sheet_display_dimensions(self, total_rows = None, total_columns = None):
         if total_rows is None and total_columns is None:
             return len(self.MT.row_positions) - 1, len(self.MT.col_positions) - 1
         if total_rows is not None:
-            height = self.MT.GetLinesHeight(self.MT.default_rh)
+            height = self.MT.get_lines_cell_height(int(self.MT.default_row_height[0]))
             self.MT.row_positions = list(accumulate(chain([0], (height for row in range(total_rows)))))
         if total_columns is not None:
-            width = self.MT.default_cw
+            width = self.MT.default_column_width
             self.MT.col_positions = list(accumulate(chain([0], (width for column in range(total_columns)))))
 
     def set_sheet_data_and_display_dimensions(self, total_rows = None, total_columns = None):
         self.sheet_display_dimensions(total_rows = total_rows, total_columns = total_columns)
         self.MT.data_dimensions(total_rows = total_rows, total_columns = total_columns)
 
     def move_row_position(self, row: int, moveto: int):
@@ -1063,164 +1080,20 @@
     def move_column_position(self, column: int, moveto: int):
         self.MT.move_col_position(column, moveto)
 
     def move_column(self, column: int, moveto: int):
         self.move_columns(moveto, column, 1)
 
     def move_columns(self, moveto: int, to_move_min: int, number_of_columns: int, move_data: bool = True, index_type: str = "displayed", create_selections: bool = True, redraw = False):
-        if index_type.lower() == "displayed" or self.MT.all_columns_displayed:
-            new_selected, dispset = self.MT.move_columns_adjust_options_dict(moveto, to_move_min, number_of_columns, move_data, create_selections)
-        else:
-            dispset = {}
-            c = int(moveto)
-            to_move_max = to_move_min + number_of_columns
-            totalcols = int(number_of_columns)
-            to_del = to_move_max + number_of_columns
-            orig_selected = list(range(to_move_min, to_move_min + totalcols))
-            num_data_cols = self.MT.total_data_cols()
-            if c + totalcols > num_data_cols:
-                new_selected = tuple(range(num_data_cols - totalcols, num_data_cols))
-            else:
-                if to_move_min > c:
-                    new_selected = tuple(range(c, c + totalcols))
-                else:
-                    new_selected = tuple(range(c + 1 - totalcols, c + 1))
-            newcolsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
-            if to_move_min > c:
-                for rn in range(len(self.MT.data)):
-                    if len(self.MT.data[rn]) < to_move_max:
-                        self.MT.data[rn].extend(list(repeat("", to_move_max - len(self.MT.data[rn]) + 1)))
-                    self.MT.data[rn][c:c] = self.MT.data[rn][to_move_min:to_move_max]
-                    self.MT.data[rn][to_move_max:to_del] = []
-                if isinstance(self.MT._headers, list) and self.MT._headers:
-                    if len(self.MT._headers) < to_move_max:
-                        self.MT._headers.extend(list(repeat("", to_move_max - len(self.MT._headers) + 1)))
-                    self.MT._headers[c:c] = self.MT._headers[to_move_min:to_move_max]
-                    self.MT._headers[to_move_max:to_del] = []
-                self.CH.cell_options = {
-                    int(newcolsdct[k]) if k in newcolsdct else
-                    k + totalcols if k < to_move_min and k >= c else
-                    int(k): v for k, v in self.CH.cell_options.items()
-                }
-                self.MT.cell_options = {
-                    (k[0], int(newcolsdct[k[1]])) if k[1] in newcolsdct else
-                    (k[0], k[1] + totalcols) if k[1] < to_move_min and k[1] >= c else
-                    k: v for k, v in self.MT.cell_options.items()
-                }
-                self.MT.col_options = {
-                    int(newcolsdct[k]) if k in newcolsdct else
-                    k + totalcols if k < to_move_min and k >= c else
-                    int(k): v for k, v in self.MT.col_options.items()
-                }
-                self.MT.displayed_columns = sorted(int(newcolsdct[k]) if k in newcolsdct else k + totalcols if k < to_move_min and k >= c else int(k) for k in self.MT.displayed_columns)
-            else:
-                c += 1
-                if move_data:
-                    for rn in range(len(self.MT.data)):
-                        if len(self.MT.data[rn]) < c - 1:
-                            self.MT.data[rn].extend(list(repeat("", c - len(self.MT.data[rn]))))
-                        self.MT.data[rn][c:c] = self.MT.data[rn][to_move_min:to_move_max]
-                        self.MT.data[rn][to_move_min:to_move_max] = []
-                    if isinstance(self.MT._headers, list) and self.MT._headers:
-                        if len(self.MT._headers) < c:
-                            self.MT._headers.extend(list(repeat("", c - len(self.MT._headers))))
-                        self.MT._headers[c:c] = self.MT._headers[to_move_min:to_move_max]
-                        self.MT._headers[to_move_min:to_move_max] = []
-                self.CH.cell_options = {
-                    int(newcolsdct[k]) if k in newcolsdct else
-                    k - totalcols if k < c and k > to_move_min else
-                    int(k): v for k, v in self.CH.cell_options.items()
-                }
-                self.MT.cell_options = {
-                    (k[0], int(newcolsdct[k[1]])) if k[1] in newcolsdct else
-                    (k[0], k[1] - totalcols) if k[1] < c and k[1] > to_move_min else
-                    k: v for k, v in self.MT.cell_options.items()
-                }
-                self.MT.col_options = {
-                    int(newcolsdct[k]) if k in newcolsdct else
-                    k - totalcols if k < c and k > to_move_min else
-                    int(k): v for k, v in self.MT.col_options.items()
-                }
-                self.MT.displayed_columns = sorted(int(newcolsdct[k]) if k in newcolsdct else k - totalcols if k < c and k > to_move_min else int(k) for k in self.MT.displayed_columns)
+        new_selected, dispset = self.MT.move_columns_adjust_options_dict(moveto, to_move_min, number_of_columns, move_data, create_selections, index_type = index_type.lower())
         self.set_refresh_timer(redraw)
         return new_selected, dispset
         
     def move_rows(self, moveto: int, to_move_min: int, number_of_rows: int, move_data: bool = True, index_type: str = "displayed", create_selections: bool = True, redraw = False):
-        if index_type.lower() == "displayed" or self.MT.all_rows_displayed:
-            new_selected, dispset = self.MT.move_rows_adjust_options_dict(moveto, to_move_min, number_of_rows, move_data, create_selections)
-        else:
-            dispset = {}
-            r = int(moveto)
-            to_move_max = to_move_min + number_of_rows
-            totalrows = int(number_of_rows)
-            to_del = to_move_max + number_of_rows
-            orig_selected = list(range(to_move_min, to_move_min + totalrows))
-            num_data_rows = self.MT.total_data_rows()
-            if r + totalrows > num_data_rows:
-                new_selected = tuple(range(num_data_rows - totalrows, num_data_rows))
-            else:
-                if to_move_min > r:
-                    new_selected = tuple(range(r, r + totalrows))
-                else:
-                    new_selected = tuple(range(r + 1 - totalrows, r + 1))
-            newrowsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
-            if to_move_min > r:
-                if len(self.MT.data) < to_move_max:
-                    self.MT.data.extend(list(repeat("", to_move_max - len(self.MT.data) + 1)))
-                self.MT.data[r:r] = self.MT.data[to_move_min:to_move_max]
-                self.MT.data[to_move_max:to_del] = []
-                if isinstance(self.MT._row_index, list) and self.MT._row_index:
-                    if len(self.MT._row_index) < to_move_max:
-                        self.MT._row_index.extend(list(repeat("", to_move_max - len(self.MT._row_index) + 1)))
-                    self.MT._row_index[r:r] = self.MT._row_index[to_move_min:to_move_max]
-                    self.MT._row_index[to_move_max:to_del] = []
-                self.RI.cell_options = {
-                    int(newrowsdct[k]) if k in newrowsdct else
-                    k + totalrows if k < to_move_min and k >= r else
-                    int(k): v for k, v in self.RI.cell_options.items()
-                }
-                self.MT.cell_options = {
-                    (int(newrowsdct[k[0]]), k[1]) if k[0] in newrowsdct else
-                    (k[0] + totalrows, k[1]) if k[0] < to_move_min and k[0] >= r else
-                    k: v for k, v in self.MT.cell_options.items()
-                }
-                self.MT.row_options = {
-                    int(newrowsdct[k]) if k in newrowsdct else
-                    k + totalrows if k < to_move_min and k >= r else
-                    int(k): v for k, v in self.MT.row_options.items()
-                }
-                self.MT.displayed_rows = sorted(int(newrowsdct[k]) if k in newrowsdct else k + totalrows if k < to_move_min and k >= r else int(k) for k in self.MT.displayed_rows)
-            else:
-                r += 1
-                if move_data:
-                    if len(self.MT.data) < r - 1:
-                        self.MT.data.extend(list(repeat("", r - len(self.MT.data))))
-                    self.MT.data[r:r] = self.MT.data[to_move_min:to_move_max]
-                    self.MT.data[to_move_min:to_move_max] = []
-                    if isinstance(self.MT._row_index, list) and self.MT._row_index:
-                        if len(self.MT._row_index) < r:
-                            self.MT._row_index.extend(list(repeat("", r - len(self.MT._row_index))))
-                        self.MT._row_index[r:r] = self.MT._row_index[to_move_min:to_move_max]
-                        self.MT._row_index[to_move_min:to_move_max] = []
-                self.RI.cell_options = {
-                    int(newrowsdct[k]) if k in newrowsdct else
-                    k - totalrows if k < r and k > to_move_min else
-                    int(k): v for k, v in self.RI.cell_options.items()
-                }
-                self.MT.cell_options = {
-                    (int(newrowsdct[k[0]]), k[1]) if k[0] in newrowsdct else
-                    (k[0] - totalrows, k[1]) if k[0] < r and k[0] > to_move_min else
-                    k: v for k, v in self.MT.cell_options.items()
-                }
-                self.MT.row_options = {
-                    int(newrowsdct[k]) if k in newrowsdct else
-                    k - totalrows if k < r and k > to_move_min else
-                    int(k): v for k, v in self.MT.row_options.items()
-                }
-                self.MT.displayed_rows = sorted(int(newrowsdct[k]) if k in newrowsdct else k - totalrows if k < r and k > to_move_min else int(k) for k in self.MT.displayed_rows)
+        new_selected, dispset = self.MT.move_rows_adjust_options_dict(moveto, to_move_min, number_of_rows, move_data, create_selections, index_type = index_type.lower())
         self.set_refresh_timer(redraw)
         return new_selected, dispset
 
     # works on currently selected box
     def open_cell(self, ignore_existing_editor = True):
         self.MT.open_cell(event = GeneratedMouseEvent(), ignore_existing_editor = ignore_existing_editor)
         
@@ -1397,34 +1270,72 @@
     def row_selected(self, r):
         return self.MT.row_selected(r)
 
     def column_selected(self, c):
         return self.MT.col_selected(c)
     
     def anything_selected(self, exclude_columns = False, exclude_rows = False, exclude_cells = False):
-        return self.MT.anything_selected(exclude_columns = exclude_columns, exclude_rows = exclude_rows, exclude_cells = exclude_cells)
+        if self.MT.anything_selected(exclude_columns = exclude_columns, exclude_rows = exclude_rows, exclude_cells = exclude_cells):
+            return True
+        return False
 
     def all_selected(self):
         return self.MT.all_selected()
 
     def readonly_rows(self, rows = [], readonly = True, redraw = False):
-        self.MT.readonly_rows(rows = rows,
-                              readonly = readonly)
+        if isinstance(rows, int):
+            rows_ = [rows]
+        else:
+            rows_ = rows
+        if not readonly:
+            for r in rows_:
+                if r in self.MT.row_options and 'readonly' in self.MT.row_options[r]:
+                    del self.MT.row_options[r]['readonly']
+        else:
+            for r in rows_:
+                if r not in self.MT.row_options:
+                    self.MT.row_options[r] = {}
+                self.MT.row_options[r]['readonly'] = True
         self.set_refresh_timer(redraw)
 
     def readonly_columns(self, columns = [], readonly = True, redraw = False):
-        self.MT.readonly_columns(columns = columns,
-                                 readonly = readonly)
+        if isinstance(columns, int):
+            cols_ = [columns]
+        else:
+            cols_ = columns
+        if not readonly:
+            for c in cols_:
+                if c in self.MT.col_options and 'readonly' in self.MT.col_options[c]:
+                    del self.MT.col_options[c]['readonly']
+        else:
+            for c in cols_:
+                if c not in self.MT.col_options:
+                    self.MT.col_options[c] = {}
+                self.MT.col_options[c]['readonly'] = True
         self.set_refresh_timer(redraw)
 
     def readonly_cells(self, row = 0, column = 0, cells = [], readonly = True, redraw = False):
-        self.MT.readonly_cells(row = row,
-                               column = column,
-                               cells = cells,
-                               readonly = readonly)
+        if not readonly:
+            if cells:
+                for r, c in cells:
+                    if (r, c) in self.MT.cell_options and 'readonly' in self.MT.cell_options[(r, c)]:
+                        del self.MT.cell_options[(r, c)]['readonly']
+            else:
+                if (row, column) in self.MT.cell_options and 'readonly' in self.MT.cell_options[(row, column)]:
+                    del self.MT.cell_options[(row, column)]['readonly']
+        else:
+            if cells:
+                for (r, c) in cells:
+                    if (r, c) not in self.MT.cell_options:
+                        self.MT.cell_options[(r, c)] = {}
+                    self.MT.cell_options[(r, c)]['readonly'] = True
+            else:
+                if (row, column) not in self.MT.cell_options:
+                    self.MT.cell_options[(row, column)] = {}
+                self.MT.cell_options[(row, column)]['readonly'] = True
         self.set_refresh_timer(redraw)
             
     def readonly_header(self, columns = [], readonly = True, redraw = False):
         self.CH.readonly_header(columns = columns,
                                 readonly = readonly)
         self.set_refresh_timer(redraw)
             
@@ -1498,55 +1409,100 @@
                 try:
                     del self.CH.cell_options[c]['highlight']
                 except:
                     pass
         self.set_refresh_timer(redraw)
             
     def highlight_rows(self, rows = [], bg = None, fg = None, highlight_index = True, redraw = True, end_of_screen = False, overwrite = True):
-        self.MT.highlight_rows(rows = rows,
-                               bg = bg,
-                               fg = fg,
-                               highlight_index = highlight_index,
-                               redraw = False,
-                               end_of_screen = end_of_screen,
-                               overwrite = overwrite)
+        if bg is None and fg is None:
+            return
+        for r in (rows, ) if isinstance(rows, int) else rows:
+            if r not in self.MT.row_options:
+                self.MT.row_options[r] = {}
+            if 'highlight' in self.MT.row_options[r] and not overwrite:
+                self.MT.row_options[r]['highlight'] = (self.MT.row_options[r]['highlight'][0] if bg is None else bg,
+                                                       self.MT.row_options[r]['highlight'][1] if fg is None else fg,
+                                                       self.MT.row_options[r]['highlight'][2] if self.MT.row_options[r]['highlight'][2] != end_of_screen else end_of_screen)
+            else:
+                self.MT.row_options[r]['highlight'] = (bg, fg, end_of_screen)
+        if highlight_index:
+            self.highlight_cells(cells = rows, canvas = "index", bg = bg, fg = fg, redraw = False)
         self.set_refresh_timer(redraw)
 
     def highlight_columns(self, columns = [], bg = None, fg = None, highlight_header = True, redraw = True, overwrite = True):
-        self.MT.highlight_cols(cols = columns,
-                               bg = bg,
-                               fg = fg,
-                               highlight_header = highlight_header,
-                               redraw = False,
-                               overwrite = overwrite)
+        if bg is None and fg is None:
+            return
+        for c in (columns, ) if isinstance(columns, int) else columns:
+            if c not in self.MT.col_options:
+                self.MT.col_options[c] = {}
+            if 'highlight' in self.MT.col_options[c] and not overwrite:
+                self.MT.col_options[c]['highlight'] = (self.MT.col_options[c]['highlight'][0] if bg is None else bg,
+                                                       self.MT.col_options[c]['highlight'][1] if fg is None else fg)
+            else:
+                self.MT.col_options[c]['highlight'] = (bg, fg)
+        if highlight_header:
+            self.highlight_cells(cells = columns, canvas = "header", bg = bg, fg = fg, redraw = False)
         self.set_refresh_timer(redraw)
 
     def highlight_cells(self, row = 0, column = 0, cells = [], canvas = "table", bg = None, fg = None, redraw = True, overwrite = True):
+        if bg is None and fg is None:
+            return
         if canvas == "table":
-            self.MT.highlight_cells(r = row,
-                                    c = column,
-                                    cells = cells,
-                                    bg = bg,
-                                    fg = fg,
-                                    redraw = False,
-                                    overwrite = overwrite)
+            if cells:
+                for r_, c_ in cells:
+                    if (r_, c_) not in self.MT.cell_options:
+                        self.MT.cell_options[(r_, c_)] = {}
+                    if 'highlight' in self.MT.cell_options[(r_, c_)] and not overwrite:
+                        self.MT.cell_options[(r_, c_)]['highlight'] = (self.MT.cell_options[(r_, c_)]['highlight'][0] if bg is None else bg,
+                                                                       self.MT.cell_options[(r_, c_)]['highlight'][1] if fg is None else fg)
+                    else:
+                        self.MT.cell_options[(r_, c_)]['highlight'] = (bg, fg)
+            else:
+                if isinstance(row, str) and row.lower() == "all" and isinstance(column, int):
+                    riter = range(self.MT.total_data_rows())
+                    citer = (column, )
+                elif isinstance(column, str) and column.lower() == "all" and isinstance(row, int):
+                    riter = (row, )
+                    citer = range(self.MT.total_data_cols())
+                elif isinstance(row, int) and isinstance(column, int):
+                    riter = (row, )
+                    citer = (column, )
+                for r_ in riter:
+                    for c_ in citer:
+                        if (r_, c_) not in self.MT.cell_options:
+                            self.MT.cell_options[(r_, c_)] = {}
+                        if 'highlight' in self.MT.cell_options[(r_, c_)] and not overwrite:
+                            self.MT.cell_options[(r_, c_)]['highlight'] = (self.MT.cell_options[(r_, c_)]['highlight'][0] if bg is None else bg,
+                                                                           self.MT.cell_options[(r_, c_)]['highlight'][1] if fg is None else fg)
+                        else:
+                            self.MT.cell_options[(r_, c_)]['highlight'] = (bg, fg)
         elif canvas in ("row_index", "index"):
-            self.RI.highlight_cells(r = row,
-                                    cells = cells,
-                                    bg = bg,
-                                    fg = fg,
-                                    redraw = False,
-                                    overwrite = overwrite)
+            if bg is None and fg is None:
+                return
+            iterable = cells if (cells and not isinstance(cells, int)) else (cells, ) if isinstance(cells, int) else (row, )
+            for r_ in iterable:
+                if r_ not in self.RI.cell_options:
+                    self.RI.cell_options[r_] = {}
+                if 'highlight' in self.RI.cell_options[r_] and not overwrite:
+                    self.RI.cell_options[r_]['highlight'] = (self.RI.cell_options[r_]['highlight'][0] if bg is None else bg,
+                                                             self.RI.cell_options[r_]['highlight'][1] if fg is None else fg)
+                else:
+                    self.RI.cell_options[r_]['highlight'] = (bg, fg)
         elif canvas == "header":
-            self.CH.highlight_cells(c = column,
-                                    cells = cells,
-                                    bg = bg,
-                                    fg = fg,
-                                    redraw = False,
-                                    overwrite = overwrite)
+            if bg is None and fg is None:
+                return
+            iterable = cells if (cells and not isinstance(cells, int)) else (cells, ) if isinstance(cells, int) else (column, )
+            for c_ in iterable:
+                if c_ not in self.CH.cell_options:
+                    self.CH.cell_options[c_] = {}
+                if 'highlight' in self.CH.cell_options[c_] and not overwrite:
+                    self.CH.cell_options[c_]['highlight'] = (self.CH.cell_options[c_]['highlight'][0] if bg is None else bg,
+                                                             self.CH.cell_options[c_]['highlight'][1] if fg is None else fg)
+                else:
+                    self.CH.cell_options[c_]['highlight'] = (bg, fg)
         self.set_refresh_timer(redraw)
 
     def dehighlight_cells(self, row = 0, column = 0, cells = [], canvas = "table", all_ = False, redraw = True):
         if row == "all" and canvas == "table":
             for k, v in self.MT.cell_options.items():
                 if 'highlight' in v:
                     del self.MT.cell_options[k]['highlight']
@@ -1644,16 +1600,15 @@
         a = align.lower()
         if a in ("c", "center", "centre"):
             return "center"
         elif a in ("w", "west", "left"):
             return "w"
         elif a in ("e", "east", "right"):
             return "e"
-        else:
-            raise ValueError("Align must be one of the following values: c, center, w, west, left, e, east, right")
+        raise ValueError("Align must be one of the following values: c, center, w, west, left, e, east, right")
         
     def get_cell_alignments(self):
         return {(r, c): v['align'] for (r, c), v in self.MT.cell_options.items() if 'align' in v}
     
     def get_column_alignments(self):
         return {c: v['align'] for c, v in self.MT.col_options.items() if 'align' in v}
     
@@ -1804,19 +1759,19 @@
         if 'show_vertical_grid' in kwargs:
             self.MT.show_vertical_grid = kwargs['show_vertical_grid']
         if 'empty_horizontal' in kwargs:
             self.MT.empty_horizontal = kwargs['empty_horizontal']
         if 'empty_vertical' in kwargs:
             self.MT.empty_vertical = kwargs['empty_vertical']
         if 'row_height' in kwargs:
-            self.MT.default_rh = (kwargs['row_height'] if isinstance(kwargs['row_height'], str) else "pixels", kwargs['row_height'] if isinstance(kwargs['row_height'], int) else self.MT.GetLinesHeight(int(kwargs['row_height'])))
+            self.MT.default_row_height = (kwargs['row_height'] if isinstance(kwargs['row_height'], str) else "pixels", kwargs['row_height'] if isinstance(kwargs['row_height'], int) else self.MT.get_lines_cell_height(int(kwargs['row_height'])))
         if 'column_width' in kwargs:
-            self.MT.default_cw = self.MT.min_cw + 20 if kwargs['column_width'] < self.MT.min_cw else int(kwargs['column_width'])
+            self.MT.default_column_width = self.MT.min_column_width + 20 if kwargs['column_width'] < self.MT.min_column_width else int(kwargs['column_width'])
         if 'header_height' in kwargs:
-            self.MT.default_hh = (kwargs['header_height'] if isinstance(kwargs['header_height'], str) else "pixels", kwargs['header_height'] if isinstance(kwargs['header_height'], int) else self.MT.GetHdrLinesHeight(int(kwargs['header_height'])))
+            self.MT.default_header_height = (kwargs['header_height'] if isinstance(kwargs['header_height'], str) else "pixels", kwargs['header_height'] if isinstance(kwargs['header_height'], int) else self.MT.get_lines_cell_height(int(kwargs['header_height']), font = self.MT.header_font))
         if 'row_drag_and_drop_perform' in kwargs:
             self.RI.row_drag_and_drop_perform = kwargs['row_drag_and_drop_perform']
         if 'column_drag_and_drop_perform' in kwargs:
             self.CH.column_drag_and_drop_perform = kwargs['column_drag_and_drop_perform']
         if 'popup_menu_font' in kwargs:
             self.MT.popup_menu_font = kwargs['popup_menu_font']
         if 'popup_menu_fg' in kwargs:
@@ -1851,26 +1806,28 @@
             self.MT.table_selected_columns_bg = kwargs['table_selected_columns_bg']
         if 'table_selected_columns_fg' in kwargs:
             self.MT.table_selected_columns_fg = kwargs['table_selected_columns_fg']
         if 'default_header' in kwargs:
             self.CH.default_header = kwargs['default_header'].lower()
         if 'default_row_index' in kwargs:
             self.RI.default_index = kwargs['default_row_index'].lower()
-        if 'max_colwidth' in kwargs:
-            self.CH.max_cw = float(kwargs['max_colwidth'])
+        if 'max_column_width' in kwargs:
+            self.MT.max_column_width = float(kwargs['max_column_width'])
         if 'max_row_height' in kwargs:
-            self.RI.max_rh = float(kwargs['max_row_height'])
+            self.MT.max_row_height = float(kwargs['max_row_height'])
         if 'max_header_height' in kwargs:
-            self.CH.max_header_height = float(kwargs['max_header_height'])
-        if 'max_row_width' in kwargs:
-            self.RI.max_row_width = float(kwargs['max_row_width'])
+            self.MT.max_header_height = float(kwargs['max_header_height'])
+        if 'max_index_width' in kwargs:
+            self.MT.max_index_width = float(kwargs['max_index_width'])
         if 'font' in kwargs:
             self.MT.font(kwargs['font'])
         if 'header_font' in kwargs:
             self.MT.header_font(kwargs['header_font'])
+        if 'index_font' in kwargs:
+            self.MT.index_font(kwargs['index_font'])
         if 'theme' in kwargs:
             self.change_theme(kwargs['theme'])
         if 'show_selected_cells_border' in kwargs:
             self.MT.show_selected_cells_border = kwargs['show_selected_cells_border']
         if 'header_bg' in kwargs:
             self.CH.config(background = kwargs['header_bg'])
             self.CH.header_bg = kwargs['header_bg']
@@ -2018,15 +1975,15 @@
                 only_columns = (only_columns, )
             elif not is_iterable(only_columns):
                 raise ValueError(f"Argument 'only_columns' must be either int or iterable or None. Not {type(only_columns)}")
         if r >= self.MT.total_data_rows():
             raise IndexError(f"Row #{r} is out of range.")
         if r >= len(self.MT.data):
             total_data_cols = self.MT.total_data_cols()
-            self.MT.data.extend([list(repeat("", total_data_cols)) for i in range((r + 1) - len(self.MT.data))])
+            self.MT.fix_data_len(r, total_data_cols - 1)
         iterable = only_columns if only_columns is not None else range(len(self.MT.data[r]))
         if get_index:
             return ([self.get_index_data(r, get_displayed = get_index_displayed)] +
                     [self.MT.get_cell_data(r, c, get_displayed = get_displayed) for c in iterable])
         else:
             return [self.MT.get_cell_data(r, c, get_displayed = get_displayed) for c in iterable]
 
@@ -2119,15 +2076,15 @@
     def set_row_data(self, r, values = tuple(), add_columns = True, redraw = False, keep_formatting = True):
         if r >= len(self.MT.data):
             raise Exception("Row number is out of range")
         if not keep_formatting:
             self.MT.delete_row_format(r, clear_values = False)
         maxidx = len(self.MT.data[r]) - 1
         if not values:
-            self.MT.data[r][:] = list(repeat("", len(self.MT.data[r])))
+            self.MT.data[r][:] = self.MT.get_empty_row_seq(r, len(self.MT.data[r]))
         if add_columns:
             for c, v in enumerate(values):
                 if c > maxidx:
                     self.MT.data[r].append(v)
                     if self.MT.all_columns_displayed:
                         self.MT.insert_col_position("end")
                 else:
@@ -2142,30 +2099,30 @@
 
     def set_column_data(self, c, values = tuple(), add_rows = True, redraw = False, keep_formatting = True):
         if not keep_formatting:
             self.MT.delete_column_format(c, clear_values = False)
         if add_rows:
             maxidx = len(self.MT.data) - 1
             total_cols = None
-            height = self.MT.default_rh[1]
+            height = self.MT.default_row_height[1]
             for rn, v in enumerate(values):
                 if rn > maxidx:
                     if total_cols is None:
                         total_cols = self.MT.total_data_cols()
-                    self.MT.data.append(list(repeat("", total_cols)))
+                    self.MT.fix_data_len(rn, total_cols - 1)
                     if self.MT.all_rows_displayed:
                         self.MT.insert_row_position("end", height = height)
                     maxidx += 1
                 if c >= len(self.MT.data[rn]):
-                    self.MT.data[rn].extend(list(repeat("", c - len(self.MT.data[rn]))))
+                    self.MT.fix_row_len(rn, c)
                 self.set_cell_data(r = rn, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         else:
             for rn, v in enumerate(values):
                 if c >= len(self.MT.data[rn]):
-                    self.MT.data[rn].extend(list(repeat("", c - len(self.MT.data[rn]))))
+                    self.MT.fix_row_len(rn, c)
                 self.set_cell_data(r = rn, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         self.set_refresh_timer(redraw)
 
     def insert_column(self,
                       values: Union[list, tuple, int, None] = None, 
                       idx: Union[str, int] = "end", 
                       width = None, 
@@ -2196,15 +2153,16 @@
             old_total = self.MT.equalize_data_row_lengths()
         else:
             old_total = self.MT.total_data_cols()
         if isinstance(columns, int):
             if columns < 1:
                 raise ValueError(f"columns arg must be greater than 0, not {columns}")
             total_rows = self.MT.total_data_rows()
-            data = [list(repeat("", total_rows)) for i in range(columns)]
+            start = old_total if idx == "end" else idx
+            data = [self.MT.get_empty_row_seq(rn, end = start + columns, start = start, c_ops = idx == "end") for rn in range(total_rows)]
             numcols = columns
         else:
             data = columns
             numcols = len(columns)
         if self.MT.all_columns_displayed:
             if mod_column_positions:
                 self.MT.insert_col_positions(idx = idx,
@@ -2217,29 +2175,29 @@
                 inspos = bisect.bisect_left(self.MT.displayed_columns, idx)
                 self.MT.displayed_columns[inspos:inspos] = list(range(idx, idx + numcols))
                 self.MT.insert_col_positions(idx = inspos,
                                              widths = columns if isinstance(columns, int) and widths is None else widths,
                                              deselect_all = deselect_all)
         maxidx = len(self.MT.data) - 1
         if add_rows:
-            height = self.MT.default_rh[1]
+            height = self.MT.default_row_height[1]
             if idx == "end":
                 for values in reversed(data):
                     for rn, v in enumerate(values):
                         if rn > maxidx:
-                            self.MT.data.append(list(repeat("", old_total)))
+                            self.MT.data.append(self.MT.get_empty_row_seq(rn, old_total))
                             if self.MT.all_rows_displayed:
                                 self.MT.insert_row_position("end", height = height)
                             maxidx += 1
                         self.MT.data[rn].append(v)
             else:
                 for values in reversed(data):
                     for rn, v in enumerate(values):
                         if rn > maxidx:
-                            self.MT.data.append(list(repeat("", old_total)))
+                            self.MT.data.append(self.MT.get_empty_row_seq(rn, old_total))
                             if self.MT.all_rows_displayed:
                                 self.MT.insert_row_position("end", height = height)
                             maxidx += 1
                         self.MT.data[rn].insert(idx, v)
         else:
             if idx == "end":
                 for values in reversed(data):
@@ -2257,90 +2215,60 @@
             num_add = len(data)
             self.MT.cell_options = {(rn, cn if cn < idx else cn + num_add): t2 for (rn, cn), t2 in self.MT.cell_options.items()}
             self.MT.col_options = {cn if cn < idx else cn + num_add: t for cn, t in self.MT.col_options.items()}
             self.CH.cell_options = {cn if cn < idx else cn + num_add: t for cn, t in self.CH.cell_options.items()}
         self.set_refresh_timer(redraw)
 
     def insert_row(self, 
-                   values: Union[list, int, None] = None, 
+                   values: Union[list, None] = None, 
                    idx: Union[str, int] = "end", 
                    height = None, 
                    deselect_all = False, 
                    add_columns = False,
                    mod_row_positions = True,
                    redraw = True):
-        total_cols = None
-        if values is None:
-            total_cols = self.MT.total_data_cols()
-            data = list(repeat("", total_cols))
-        elif not isinstance(values, list):
-            data = list(values)
-        else:
-            data = values
-        if add_columns:
-            if total_cols is None:
-                total_cols = self.MT.total_data_cols()
-            if len(data) > total_cols:
-                self.MT.data[:] = [r + list(repeat("", len(data) - total_cols)) for r in self.MT.data]
-            elif len(data) < total_cols:
-                data += list(repeat("", total_cols - len(data)))
-            if self.MT.all_columns_displayed:
-                if not self.MT.col_positions:
-                    self.MT.col_positions = [0]
-                if len(data) > len(self.MT.col_positions) - 1:
-                    self.insert_column_positions("end", len(data) - (len(self.MT.col_positions) - 1))
-        if self.MT.all_rows_displayed and mod_row_positions:
-            inspos = idx
-        if not self.MT.all_rows_displayed:
-            if idx != "end":
-                self.MT.displayed_rows = [r if r < idx else r + 1 for r in self.MT.displayed_rows]
-            if mod_row_positions:
-                inspos = bisect.bisect_left(self.MT.displayed_rows, idx)
-                self.MT.displayed_rows[inspos:inspos] = list(range(idx, idx + 1))
-        if mod_row_positions:
-            self.MT.insert_row_position(idx = inspos, height = height, deselect_all = deselect_all)
-        if isinstance(idx, str) and idx.lower() == "end":
-            self.MT.data.append(data)
-        else:
-            self.MT.data.insert(idx, data)
-            self.MT.cell_options = {(rn if rn < idx else rn + 1, cn): t2 for (rn, cn), t2 in self.MT.cell_options.items()}
-            self.MT.row_options = {rn if rn < idx else rn + 1: t for rn, t in self.MT.row_options.items()}
-            self.RI.cell_options = {rn if rn < idx else rn + 1: t for rn, t in self.RI.cell_options.items()}
-        self.set_refresh_timer(redraw)
+        self.insert_rows(rows = 1 if values is None else [values],
+                         idx = idx,
+                         heights = height if height is None else [height],
+                         deselect_all = deselect_all,
+                         add_columns = add_columns,
+                         mod_row_positions = mod_row_positions,
+                         redraw = redraw)
 
     def insert_rows(self, 
                     rows: Union[list, int] = 1, 
                     idx: Union[str, int] = "end", 
                     heights = None, 
                     deselect_all = False, 
                     add_columns = True,
                     mod_row_positions = True, 
                     redraw = True):
         total_cols = None
+        datarn = len(self.MT.data) if idx == "end" else idx
         if isinstance(rows, int):
             if rows < 1:
                 raise ValueError(f"rows arg must be greater than 0, not {rows}")
             total_cols = self.MT.total_data_cols()
-            data = [list(repeat("", total_cols)) for i in range(rows)]
+            data = [self.MT.get_empty_row_seq(datarn + i, total_cols, r_ops = False) for i in range(rows)]
         elif not isinstance(rows, list):
             data = list(rows)
         else:
             data = rows
         try:
             data = [r if isinstance(r, list) else list(r) for r in data]
         except Exception as msg:
             raise ValueError(f"rows arg must be int or list of lists. {msg}")
         if add_columns:
             if total_cols is None:
                 total_cols = self.MT.total_data_cols()
             data_max_cols = len(max(data, key = len))
             if data_max_cols > total_cols:
-                self.MT.data[:] = [r + list(repeat("", data_max_cols - total_cols)) for r in self.MT.data]
-            else:
-                data[:] = [r + list(repeat("", total_cols - data_max_cols)) for r in data]
+                self.MT.equalize_data_row_lengths(total_columns = data_max_cols)
+            elif total_cols > data_max_cols:
+                data[:] = [r + self.MT.get_empty_row_seq(datarn + i, end = total_cols, start = data_max_cols, r_ops = False) for i in range(len(data))]
             if self.MT.all_columns_displayed:
                 if not self.MT.col_positions:
                     self.MT.col_positions = [0]
                 if data_max_cols > len(self.MT.col_positions) - 1:
                     self.insert_column_positions("end", data_max_cols - (len(self.MT.col_positions) - 1))
         if self.MT.all_rows_displayed and mod_row_positions:
             inspos = idx
@@ -2483,133 +2411,16 @@
 
     def redraw(self, redraw_header = True, redraw_row_index = True):
         self.MT.main_table_redraw_grid_and_text(redraw_header = redraw_header, redraw_row_index = redraw_row_index)
 
     def refresh(self, redraw_header = True, redraw_row_index = True):
         self.MT.main_table_redraw_grid_and_text(redraw_header = redraw_header, redraw_row_index = redraw_row_index)
         
-    def create_header_checkbox(self,
-                               c,
-                               checked = False,
-                               state = "normal",
-                               redraw = False,
-                               check_function = None,
-                               text = ""):
-        _kwargs = {'checked': checked, 'state': state, 'redraw': redraw, 'check_function': check_function, 'text': text}
-        if isinstance(c, str) and c.lower() == "all":
-            for c_ in range(self.MT.total_data_cols()):
-                self.CH.create_checkbox(datacn = c_,
-                                        **_kwargs)
-        else:
-            self.CH.create_checkbox(datacn = c,
-                                    **_kwargs)
-
-    def click_header_checkbox(self,
-                              c,
-                              checked = None):
-        if c in self.CH.cell_options and 'checkbox' in self.CH.cell_options[c]:
-            if not type(self.MT._headers[c]) == bool:
-                if checked is None:
-                    self.MT._headers[c] = False
-                else:
-                    self.MT._headers[c] = bool(checked)
-            else:
-                self.MT._headers[c] = not self.MT._headers[c]
-
-    def get_header_checkboxes(self):
-        return {k: v['checkbox'] for k, v in self.CH.cell_options.items() if 'checkbox' in v}
-
-    def delete_header_checkbox(self, c = 0):
-        if c == "all":
-            for c_ in self.CH.cell_options:
-                if 'checkbox' in self.CH.cell_options[c_]:
-                    self.CH.delete_checkbox(c_)
-        else:
-            self.CH.delete_checkbox(c)
-
-    def header_checkbox(self,
-                        c,
-                        checked = None,
-                        state = None,
-                        check_function = "",
-                        text = None):
-        if type(checked) == bool:
-            self.headers(newheaders = checked, index = c)
-        if check_function != "":
-            self.CH.cell_options[c]['checkbox']['check_function'] = check_function
-        if state and state.lower() in ("normal", "disabled"):
-            self.CH.cell_options[c]['checkbox']['state'] = state
-        if text is not None:
-            self.CH.cell_options[c]['checkbox']['text'] = text
-        return {**self.CH.cell_options[c]['checkbox'], 'checked': self.MT._headers[c]}
-    
-    def create_index_checkbox(self,
-                              r,
-                              checked = False,
-                              state = "normal",
-                              redraw = False,
-                              check_function = None,
-                              text = ""):
-        _kwargs = {'checked': checked, 'state': state, 'redraw': redraw, 'check_function': check_function, 'text': text}
-        if isinstance(r, str) and r.lower() == "all":
-            for r_ in range(self.MT.total_data_rows()):
-                self.RI.create_checkbox(datarn = r_,
-                                        **_kwargs)
-        else:
-            self.RI.create_checkbox(datarn = r,
-                                    **_kwargs)
-
-    def click_index_checkbox(self,
-                             r,
-                             checked = None):
-        if r in self.RI.cell_options and 'checkbox' in self.RI.cell_options[r]:
-            if not type(self.MT._row_index[r]) == bool:
-                if checked is None:
-                    self.MT._row_index[r] = False
-                else:
-                    self.MT._row_index[r] = bool(checked)
-            else:
-                self.MT._row_index[r] = not self.MT._row_index[r]
-
-    def get_index_checkboxes(self):
-        return {k: v['checkbox'] for k, v in self.RI.cell_options.items() if 'checkbox' in v}
-
-    def delete_index_checkbox(self, r = 0):
-        if r == "all":
-            for r_ in self.RI.cell_options:
-                if 'checkbox' in self.RI.cell_options[r_]:
-                    self.RI.delete_checkbox(r_)
-        else:
-            self.RI.delete_checkbox(r)
-
-    def index_checkbox(self,
-                       r,
-                       checked = None,
-                       state = None,
-                       check_function = "",
-                       text = None):
-        if type(checked) == bool:
-            self.row_index(newindex = checked, index = r)
-        if check_function != "":
-            self.RI.cell_options[r]['checkbox']['check_function'] = check_function
-        if state and state.lower() in ("normal", "disabled"):
-            self.RI.cell_options[r]['checkbox']['state'] = state
-        if text is not None:
-            self.RI.cell_options[r]['checkbox']['text'] = text
-        return {**self.RI.cell_options[r]['checkbox'], 'checked': self.MT._row_index[r]}
-
-    def create_checkbox(self,
-                        r,
-                        c,
-                        checked = False,
-                        state = "normal",
-                        redraw = False,
-                        check_function = None,
-                        text = ""):
-        _kwargs = {'checked': checked, 'state': state, 'redraw': redraw, 'check_function': check_function, 'text': text}
+    def create_checkbox(self, r = 0, c = 0, *args, **kwargs):
+        _kwargs = get_checkbox_kwargs(*args, **kwargs)
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_ in range(self.MT.total_data_rows()):
                 self.MT.create_checkbox(datarn = r_,
                                         datacn = c,
                                         **_kwargs)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
@@ -2619,291 +2430,516 @@
         elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             totalcols = self.MT.total_data_cols()
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(totalcols):
                     self.MT.create_checkbox(datarn = r_,
                                             datacn = c_,
                                             **_kwargs)
+        elif isinstance(r, int) and isinstance(c, int):
+            self.MT.create_checkbox(datarn = r, datacn = c, **_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+        
+    def checkbox_cell(self, r = 0, c = 0, *args, **kwargs):
+        self.create_checkbox(r = r, c = c, **get_checkbox_kwargs(*args, **kwargs))
+        
+    def create_header_checkbox(self, c = 0, *args, **kwargs):
+        _kwargs = get_checkbox_kwargs(*args, **kwargs)
+        if isinstance(c, str) and c.lower() == "all":
+            for c_ in range(self.MT.total_data_cols()):
+                self.CH.create_checkbox(datacn = c_, **_kwargs)
+        elif isinstance(c, int):
+            self.CH.create_checkbox(datacn = c, **_kwargs)
+        elif is_iterable(c):
+            for c_ in c:
+                self.CH.create_checkbox(datacn = c_, **_kwargs)
         else:
-            self.MT.create_checkbox(datarn = r,
-                                    datacn = c,
-                                    **_kwargs)
-
-    def click_checkbox(self,
-                       r,
-                       c,
-                       checked = None):
-        if (r, c) in self.MT.cell_options and 'checkbox' in self.MT.cell_options[(r, c)]:
-            if not type(self.MT.data[r][c]) == bool:
-                if checked is None:
-                    self.MT.data[r][c] = False
-                else:
-                    self.MT.data[r][c] = bool(checked)
-            else:
-                self.MT.data[r][c] = not self.MT.data[r][c]
-
-    def get_checkboxes(self):
-        return {k: v['checkbox'] for k, v in self.MT.cell_options.items() if 'checkbox' in v}
+            self.CH.checkbox_header(**_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+        
+    def create_index_checkbox(self, r = 0, *args, **kwargs):
+        _kwargs = get_checkbox_kwargs(*args, **kwargs)
+        if isinstance(r, str) and r.lower() == "all":
+            for r_ in range(self.MT.total_data_rows()):
+                self.RI.create_checkbox(datarn = r_, **_kwargs)
+        elif isinstance(r, int):
+            self.RI.create_checkbox(datarn = r, **_kwargs)
+        elif is_iterable(r):
+            for r_ in r:
+                self.RI.create_checkbox(datarn = r_, **_kwargs)
+        else:
+            self.RI.checkbox_index(**_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
 
+    def checkbox_row(self, r = 0, *args, **kwargs):
+        _kwargs = get_checkbox_kwargs(*args, **kwargs)
+        if isinstance(r, str) and r.lower() == "all":
+            for r_ in range(self.MT.total_data_rows()):
+                self.MT.checkbox_row(datarn = r_, **_kwargs)
+        elif isinstance(r, int):
+            self.MT.checkbox_row(datarn = r, **_kwargs)
+        elif is_iterable(r):
+            for r_ in r:
+                self.MT.checkbox_row(datarn = r_, **_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+                
+    def checkbox_column(self, c = 0, *args, **kwargs):
+        _kwargs = get_checkbox_kwargs(*args, **kwargs)
+        if isinstance(c, str) and c.lower() == "all":
+            for c in range(self.MT.total_data_cols()):
+                self.MT.checkbox_column(datacn = c, **_kwargs)
+        elif isinstance(c, int):
+            self.MT.checkbox_column(datacn = c, **_kwargs)
+        elif is_iterable(c):
+            for c_ in c:
+                self.MT.checkbox_column(datacn = c_, **_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+                
+    def checkbox_sheet(self, *args, **kwargs):
+        self.MT.checkbox_sheet(**get_checkbox_kwargs(*args, **kwargs))
+        
     def delete_checkbox(self, r = 0, c = 0):
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_, c_ in self.MT.cell_options:
                 if 'checkbox' in self.MT.cell_options[(r_, c)]:
-                    self.MT.delete_checkbox(r_, c)
+                    self.MT.delete_cell_options_checkbox(r_, c)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for r_, c_ in self.MT.cell_options:
                 if 'checkbox' in self.MT.cell_options[(r, c_)]:
-                    self.MT.delete_checkbox(r, c_)
+                    self.MT.delete_cell_options_checkbox(r, c_)
         elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             for r_, c_ in self.MT.cell_options:
                 if 'checkbox' in self.MT.cell_options[(r_, c_)]:
-                    self.MT.delete_checkbox(r_, c_)
-        else:
-            self.MT.delete_checkbox(r, c)
-
-    def checkbox(self,
-                 r,
-                 c,
-                 checked = None,
-                 state = None,
-                 check_function = "",
-                 text = None):
-        if type(checked) == bool:
-            self.set_cell_data(r, c, checked)
-        if check_function != "":
-            self.MT.cell_options[(r, c)]['checkbox']['check_function'] = check_function
-        if state and state.lower() in ("normal", "disabled"):
-            self.MT.cell_options[(r, c)]['checkbox']['state'] = state
-        if text is not None:
-            self.MT.cell_options[(r, c)]['checkbox']['text'] = text
-        return {**self.MT.cell_options[(r, c)]['checkbox'], 'checked': self.MT.data[r][c]}
+                    self.MT.delete_cell_options_checkbox(r_, c_)
+        elif isinstance(r, int) and isinstance(c, int):
+            self.MT.delete_cell_options_checkbox(r, c)
+            
+    def delete_cell_checkbox(self, r = 0, c = 0):
+        self.delete_checkbox(r, c)
+        
+    def delete_row_checkbox(self, r = 0):
+        if isinstance(r, str) and r.lower() == "all":
+            for r_ in self.MT.row_options:
+                self.MT.delete_row_options_checkbox(r_)
+        elif isinstance(r, int):
+            self.MT.delete_row_options_checkbox(r)
+        elif is_iterable(r):
+            for r_ in r:
+                self.MT.delete_row_options_checkbox(r_)
 
-    def create_header_dropdown(self,
-                               c = 0,
-                               values = [],
-                               set_value = None,
-                               state = "normal",
-                               redraw = False,
-                               selection_function = None,
-                               modified_function = None,
-                               search_function = dropdown_search_function,
-                               validate_input = True,
-                               text = None):
-        _kwargs = {'values': values, 'set_value': set_value, 'state': state, 'redraw': redraw, 'selection_function': selection_function,
-                   'modified_function': modified_function, 'search_function': dropdown_search_function, 'validate_input': validate_input, 'text': text}
+    def delete_column_checkbox(self, c = 0):
+        if isinstance(c, str) and c.lower() == "all":
+            for c_ in self.MT.col_options:
+                self.MT.delete_column_options_checkbox(c_)
+        elif isinstance(c, int):
+            self.MT.delete_column_options_checkbox(c)
+        elif is_iterable(c):
+            for c_ in c:
+                self.MT.delete_column_options_checkbox(c_)
+                
+    def delete_sheet_checkbox(self):
+        self.MT.delete_options_checkbox()
+        
+    def delete_header_checkbox(self, c = 0):
         if isinstance(c, str) and c.lower() == "all":
-            for c_ in range(self.MT.total_data_cols()):
-                self.CH.create_dropdown(datacn = c_,
-                                        **_kwargs)
-        else:
-            self.CH.create_dropdown(datacn = c,
-                                    **_kwargs)
-
-    def get_header_dropdown_value(self, c):
-        if 'dropdown' in self.CH.cell_options[c]:
-            return self.MT._headers[c]
-
-    def get_header_dropdown_values(self, c = 0):
-        return self.CH.cell_options[c]['dropdown']['values']
-
-    def header_dropdown_functions(self, c, selection_function = "", modified_function = ""):
-        if selection_function != "":
-            self.CH.cell_options[c]['dropdown']['select_function'] = selection_function
-        if modified_function != "":
-            self.CH.cell_options[c]['dropdown']['modified_function'] = modified_function
-        return self.CH.cell_options[c]['dropdown']['select_function'], self.CH.cell_options[c]['dropdown']['modified_function']
-
-    def set_header_dropdown_values(self, c = 0, set_existing_dropdown = False, values = [], set_value = None):
-        if set_existing_dropdown:
-            if self.CH.existing_dropdown_window is not None:
-                c_ = self.CH.existing_dropdown_window.c
-            else:
-                raise Exception("No dropdown box is currently open")
-        else:
-            c_ = c
-        self.CH.cell_options[c_]['dropdown']['values'] = values
-        if self.CH.cell_options[c_]['dropdown']['window'] != "no dropdown open":
-            self.CH.cell_options[c_]['dropdown']['window'].values(values)
-        if set_value is not None:
-            self.MT.headers(newheaders = set_value, index = c_)
-
-    def delete_header_dropdown(self, c = 0):
-        if c == "all":
             for c_ in self.CH.cell_options:
-                if 'dropdown' in self.CH.cell_options[c_]:
-                    self.CH.delete_dropdown(c_)
+                if 'checkbox' in self.CH.cell_options[c_]:
+                    self.CH.delete_cell_options_checkbox(c_)
+        if isinstance(c, int):
+            self.CH.delete_cell_options_checkbox(c)
         else:
-            self.CH.delete_dropdown(c)
-
-    def get_header_dropdowns(self):
-        return {k: v['dropdown'] for k, v in self.CH.cell_options.items() if 'dropdown' in v}
-    
-    def open_header_dropdown(self, c):
-        self.CH.open_dropdown_window(c)
-
-    def close_header_dropdown(self, c):
-        self.CH.close_dropdown_window(c)
-        
-    def create_index_dropdown(self,
-                              r = 0,
-                              values = [],
-                              set_value = None,
-                              state = "normal",
-                              redraw = False,
-                              selection_function = None,
-                              modified_function = None,
-                              search_function = dropdown_search_function,
-                              validate_input = True,
-                              text = None):
-        _kwargs = {'values': values, 'set_value': set_value, 'state': state, 'redraw': redraw, 'selection_function': selection_function,
-                   'modified_function': modified_function, 'search_function': dropdown_search_function, 'validate_input': validate_input, 'text': text}
+            self.CH.delete_options_checkbox()
+            
+    def delete_index_checkbox(self, r = 0):
         if isinstance(r, str) and r.lower() == "all":
-            for r_ in range(self.MT.total_data_rows()):
-                self.RI.create_dropdown(datarn = r_,
-                                        **_kwargs)
+            for r_ in self.RI.cell_options:
+                if 'checkbox' in self.RI.cell_options[r_]:
+                    self.RI.delete_cell_options_checkbox(r_)
+        if isinstance(r, int):
+            self.RI.delete_cell_options_checkbox(r)
         else:
-            self.RI.create_dropdown(datarn = r,
-                                    **_kwargs)
-
-    def get_index_dropdown_value(self, r):
-        if 'dropdown' in self.RI.cell_options[r]:
-            return self.MT._row_index[r]
-
-    def get_index_dropdown_values(self, r = 0):
-        return self.RI.cell_options[r]['dropdown']['values']
-
-    def index_dropdown_functions(self, r, selection_function = "", modified_function = ""):
-        if selection_function != "":
-            self.RI.cell_options[r]['dropdown']['select_function'] = selection_function
-        if modified_function != "":
-            self.RI.cell_options[r]['dropdown']['modified_function'] = modified_function
-        return self.RI.cell_options[r]['dropdown']['select_function'], self.RI.cell_options[r]['dropdown']['modified_function']
+            self.RI.delete_options_checkbox()
+        
+    def click_checkbox(self, r, c, checked = None):
+        kwargs = self.MT.get_cell_kwargs(r, c, key = 'checkbox')
+        if kwargs:
+            if not type(self.MT.data[r][c]) == bool:
+                if checked is None:
+                    self.MT.data[r][c] = False
+                else:
+                    self.MT.data[r][c] = bool(checked)
+            else:
+                self.MT.data[r][c] = not self.MT.data[r][c]
 
-    def set_index_dropdown_values(self, r = 0, set_existing_dropdown = False, values = [], set_value = None):
-        if set_existing_dropdown:
-            if self.RI.existing_dropdown_window is not None:
-                r_ = self.RI.existing_dropdown_window.r
+    def click_header_checkbox(self, c, checked = None):
+        kwargs = self.CH.get_cell_kwargs(c, key = 'checkbox')
+        if kwargs:
+            if not type(self.MT._headers[c]) == bool:
+                if checked is None:
+                    self.MT._headers[c] = False
+                else:
+                    self.MT._headers[c] = bool(checked)
             else:
-                raise Exception("No dropdown box is currently open")
-        else:
-            r_ = r
-        self.RI.cell_options[r_]['dropdown']['values'] = values
-        if self.RI.cell_options[r_]['dropdown']['window'] != "no dropdown open":
-            self.RI.cell_options[r_]['dropdown']['window'].values(values)
-        if set_value is not None:
-            self.MT.row_index(newindex = set_value, index = r_)
+                self.MT._headers[c] = not self.MT._headers[c]
+                
+    def click_index_checkbox(self, r, checked = None):
+        kwargs = self.RI.get_cell_kwargs(r, key = 'checkbox')
+        if kwargs:
+            if not type(self.MT._row_index[r]) == bool:
+                if checked is None:
+                    self.MT._row_index[r] = False
+                else:
+                    self.MT._row_index[r] = bool(checked)
+            else:
+                self.MT._row_index[r] = not self.MT._row_index[r]
+                
+    def get_checkboxes(self):
+        d = {**{k: v['checkbox'] for k, v in self.MT.cell_options.items() if 'checkbox' in v},
+             **{k: v['checkbox'] for k, v in self.MT.row_options.items() if 'checkbox' in v},
+             **{k: v['checkbox'] for k, v in self.MT.col_options.items() if 'checkbox' in v}}
+        if 'checkbox' in self.MT.options:
+            return {**d, 'checkbox': self.MT.options['checkbox']}
+        return d
 
-    def delete_index_dropdown(self, r = 0):
-        if r == "all":
-            for r_ in self.RI.cell_options:
-                if 'dropdown' in self.RI.cell_options[r_]:
-                    self.RI.delete_dropdown(r_)
-        else:
-            self.RI.delete_dropdown(r)
+    def get_header_checkboxes(self):
+        d = {k: v['checkbox'] for k, v in self.CH.cell_options.items() if 'checkbox' in v}
+        if 'checkbox' in self.CH.options:
+            return {**d, 'checkbox': self.CH.options['checkbox']}
+        return d
 
-    def get_index_dropdowns(self):
-        return {k: v['dropdown'] for k, v in self.RI.cell_options.items() if 'dropdown' in v}
+    def get_index_checkboxes(self):
+        d = {k: v['checkbox'] for k, v in self.RI.cell_options.items() if 'checkbox' in v}
+        if 'checkbox' in self.RI.options:
+            return {**d, 'checkbox': self.RI.options['checkbox']}
+        return d
     
-    def open_index_dropdown(self, r):
-        self.RI.open_dropdown_window(r)
+    def checkbox(self, r, c, checked = None, state = None, check_function = "", text = None):
+        if type(checked) == bool:
+            self.set_cell_data(r, c, checked)
+        kwargs = self.MT.get_cell_kwargs(r, c, key = 'checkbox')
+        if check_function != "":
+            kwargs['check_function'] = check_function
+        if state and state.lower() in ("normal", "disabled"):
+            kwargs['state'] = state
+        if text is not None:
+            kwargs['text'] = text
+        return {**kwargs, 'checked': self.MT.data[r][c]}
 
-    def close_index_dropdown(self, r):
-        self.RI.close_dropdown_window(r)
+    def header_checkbox(self, c, checked = None, state = None, check_function = "", text = None):
+        if type(checked) == bool:
+            self.headers(newheaders = checked, index = c)
+        kwargs = self.CH.get_cell_kwargs(c, key = 'checkbox')
+        if kwargs:
+            if check_function != "":
+                kwargs['check_function'] = check_function
+            if state and state.lower() in ("normal", "disabled"):
+                kwargs['state'] = state
+            if text is not None:
+                kwargs['text'] = text
+            return {**kwargs, 'checked': self.MT._headers[c]}
 
-    def create_dropdown(self,
-                        r = 0,
-                        c = 0,
-                        values = [],
-                        set_value = None,
-                        state = "normal",
-                        redraw = False,
-                        selection_function = None,
-                        modified_function = None,
-                        search_function = dropdown_search_function,
-                        validate_input = True,
-                        text = None):
-        _kwargs = {'values': values, 'set_value': set_value, 'state': state, 'redraw': redraw, 'selection_function': selection_function,
-                   'modified_function': modified_function, 'search_function': dropdown_search_function, 'validate_input': validate_input, 'text': text}
+    def index_checkbox(self, r, checked = None, state = None, check_function = "", text = None):
+        if type(checked) == bool:
+            self.row_index(newindex = checked, index = r)
+        kwargs = self.RI.get_cell_kwargs(r, key = 'checkbox')
+        if kwargs:
+            if check_function != "":
+                kwargs['check_function'] = check_function
+            if state and state.lower() in ("normal", "disabled"):
+                kwargs['state'] = state
+            if text is not None:
+                kwargs['text'] = text
+            return {**kwargs, 'checked': self.MT._row_index[r]}
+
+    def create_dropdown(self, r = 0, c = 0, *args, **kwargs):
+        _kwargs = get_dropdown_kwargs(*args, **kwargs)
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_ in range(self.MT.total_data_rows()):
-                self.MT.create_dropdown(datarn = r_,
-                                        datacn = c,
-                                        **_kwargs)
+                self.MT.create_dropdown(datarn = r_, datacn = c, **_kwargs)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
-                self.MT.create_dropdown(datarn = r,
-                                        datacn = c_,
-                                        **_kwargs)
+                self.MT.create_dropdown(datarn = r, datacn = c_, **_kwargs)
         elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             totalcols = self.MT.total_data_cols()
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(totalcols):
-                    self.MT.create_dropdown(datarn = r_,
-                                            datacn = c_,
-                                            **_kwargs)
-        else:
-            self.MT.create_dropdown(datarn = r,
-                                    datacn = c,
-                                    **_kwargs)
-
-    def get_dropdown_value(self, r, c):
-        return self.get_cell_data(r, c)
-
-    def get_dropdown_values(self, r = 0, c = 0):
-        return self.MT.cell_options[(r, c)]['dropdown']['values']
-
-    def dropdown_functions(self, r, c, selection_function = "", modified_function = ""):
-        if selection_function != "":
-            self.MT.cell_options[(r, c)]['dropdown']['select_function'] = selection_function
-        if modified_function != "":
-            self.MT.cell_options[(r, c)]['dropdown']['modified_function'] = modified_function
-        return self.MT.cell_options[(r, c)]['dropdown']['select_function'], self.MT.cell_options[(r, c)]['dropdown']['modified_function']
+                    self.MT.create_dropdown(datarn = r_, datacn = c_, **_kwargs)
+        elif isinstance(r, int) and isinstance(c, int):
+            self.MT.create_dropdown(datarn = r, datacn = c, **_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+        
+    def dropdown_cell(self, r = 0, c = 0, *args, **kwargs):
+        self.create_dropdown(r = r, c = c, **get_dropdown_kwargs(*args, **kwargs))
+        
+    def dropdown_row(self, r = 0, *args, **kwargs):
+        _kwargs = get_dropdown_kwargs(*args, **kwargs)
+        if isinstance(r, str) and r.lower() == "all":
+            for r_ in range(self.MT.total_data_rows()):
+                self.MT.dropdown_row(datarn = r_, **_kwargs)
+        elif isinstance(r, int):
+            self.MT.dropdown_row(datarn = r, **_kwargs)
+        elif is_iterable(r):
+            for r_ in r:
+                self.MT.dropdown_row(datarn = r_, **_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+                
+    def dropdown_column(self, c = 0, *args, **kwargs):
+        _kwargs = get_dropdown_kwargs(*args, **kwargs)
+        if isinstance(c, str) and c.lower() == "all":
+            for c_ in range(self.MT.total_data_cols()):
+                self.MT.dropdown_column(datacn = c_, **_kwargs)
+        elif isinstance(c, int):
+            self.MT.dropdown_column(datacn = c, **_kwargs)
+        elif is_iterable(c):
+            for c_ in c:
+                self.MT.dropdown_column(datacn = c_, **_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+                
+    def dropdown_sheet(self, *args, **kwargs):
+        _kwargs = get_dropdown_kwargs(*args, **kwargs)
+        self.MT.dropdown_sheet(**_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
 
+    def create_header_dropdown(self, c = 0, *args, **kwargs):
+        _kwargs = get_dropdown_kwargs(*args, **kwargs)
+        if isinstance(c, str) and c.lower() == "all":
+            for c_ in range(self.MT.total_data_cols()):
+                self.CH.create_dropdown(datacn = c_, **_kwargs)
+        elif isinstance(c, int):
+            self.CH.create_dropdown(datacn = c, **_kwargs)
+        elif is_iterable(c):
+            for c_ in c:
+                self.CH.create_dropdown(datacn = c_, **_kwargs)
+        elif c is None:
+            self.CH.dropdown_header(**_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+        
+    def create_index_dropdown(self, r = 0, *args, **kwargs):
+        _kwargs = get_dropdown_kwargs(*args, **kwargs)
+        if isinstance(r, str) and r.lower() == "all":
+            for r_ in range(self.MT.total_data_rows()):
+                self.RI.create_dropdown(datarn = r_, **_kwargs)
+        elif isinstance(r, int):
+            self.RI.create_dropdown(datarn = r, **_kwargs)
+        elif is_iterable(r):
+            for r_ in r:
+                self.RI.create_dropdown(datarn = r_, **_kwargs)
+        elif r is None:
+            self.RI.dropdown_index(**_kwargs)
+        self.set_refresh_timer(_kwargs['redraw'])
+        
+    def delete_dropdown(self, r = 0, c = 0):
+        if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
+            for r_, c_ in self.MT.cell_options:
+                if 'dropdown' in self.MT.cell_options[(r_, c)]:
+                    self.MT.delete_cell_options_dropdown(r_, c)
+        elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
+            for r_, c_ in self.MT.cell_options:
+                if 'dropdown' in self.MT.cell_options[(r, c_)]:
+                    self.MT.delete_cell_options_dropdown(r, c_)
+        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
+            for r_, c_ in self.MT.cell_options:
+                if 'dropdown' in self.MT.cell_options[(r_, c_)]:
+                    self.MT.delete_cell_options_dropdown(r_, c_)
+        elif isinstance(r, int) and isinstance(c, int):
+            self.MT.delete_cell_options_dropdown(r, c)
+        
+    def delete_cell_dropdown(self, r = 0, c = 0):
+        self.delete_dropdown(r = r, c = c)
+        
+    def delete_row_dropdown(self, r = "all"):
+        if isinstance(r, str) and r.lower() == "all":
+            for r_ in self.MT.row_options:
+                if 'dropdown' in self.MT.row_options[r_]:
+                    self.MT.delete_row_options_dropdown(datarn = r_)
+        elif isinstance(r, int):
+            self.MT.delete_row_options_dropdown(datarn = r)
+        elif is_iterable(r):
+            for r_ in r:
+                self.MT.delete_row_options_dropdown(datarn = r_)
+                
+    def delete_column_dropdown(self, r = "all"):
+        if isinstance(c, str) and c.lower() == "all":
+            for c_ in self.MT.col_options:
+                if 'dropdown' in self.MT.col_options[c_]:
+                    self.MT.delete_column_options_dropdown(datacn = c_)
+        elif isinstance(c, int):
+            self.MT.delete_column_options_dropdown(datacn = c)
+        elif is_iterable(c):
+            for c_ in c:
+                self.MT.delete_column_options_dropdown(datacn = c_)
+                
+    def delete_sheet_dropdown(self):
+        self.MT.delete_options_dropdown()
+        
+    def delete_header_dropdown(self, c = None):
+        if isinstance(c, str) and c.lower() == "all":
+            for c_ in self.CH.cell_options:
+                if 'dropdown' in self.CH.cell_options[c_]:
+                    self.CH.delete_cell_options_dropdown(c_)
+        elif isinstance(c, int):
+            self.CH.delete_cell_options_dropdown(c)
+        elif is_iterable(c):
+            for c_ in c:
+                self.CH.delete_cell_options_dropdown(c_)
+        elif c is None:
+            self.CH.delete_options_dropdown(c)
+        
+    def delete_index_dropdown(self, r = 0):
+        if isinstance(r, str) and r.lower() == "all":
+            for r_ in self.RI.cell_options:
+                if 'dropdown' in self.RI.cell_options[r_]:
+                    self.RI.delete_cell_options_dropdown(r_)
+        elif isinstance(r, int):
+            self.RI.delete_cell_options_dropdown(r)
+        elif is_iterable(r):
+            for r_ in r:
+                self.RI.delete_cell_options_dropdown(r_)
+        elif r is None:
+            self.RI.delete_options_dropdown()
+            
+    def get_dropdowns(self):
+        d = {**{k: v['dropdown'] for k, v in self.MT.cell_options.items() if 'dropdown' in v},
+             **{k: v['dropdown'] for k, v in self.MT.row_options.items() if 'dropdown' in v},
+             **{k: v['dropdown'] for k, v in self.MT.col_options.items() if 'dropdown' in v}}
+        if 'dropdown' in self.MT.options:
+            return {**d, 'dropdown': self.MT.options['dropdown']}
+        return d
+    
+    def get_header_dropdowns(self):
+        d = {k: v['dropdown'] for k, v in self.CH.cell_options.items() if 'dropdown' in v}
+        if 'dropdown' in self.CH.options:
+            return {**d, 'dropdown': self.CH.options['dropdown']}
+        return d
+    
+    def get_index_dropdowns(self):
+        d = {k: v['dropdown'] for k, v in self.RI.cell_options.items() if 'dropdown' in v}
+        if 'dropdown' in self.RI.options:
+            return {**d, 'dropdown': self.RI.options['dropdown']}
+        return d
+    
     def set_dropdown_values(self, r = 0, c = 0, set_existing_dropdown = False, values = [], set_value = None):
         if set_existing_dropdown:
             if self.MT.existing_dropdown_window is not None:
                 r_ = self.MT.existing_dropdown_window.r
                 c_ = self.MT.existing_dropdown_window.c
             else:
                 raise Exception("No dropdown box is currently open")
         else:
             r_ = r
             c_ = c
-        self.MT.cell_options[(r_, c_)]['dropdown']['values'] = values
-        if self.MT.cell_options[(r_, c_)]['dropdown']['window'] != "no dropdown open":
-            self.MT.cell_options[(r_, c_)]['dropdown']['window'].values(values)
+        kwargs = self.MT.get_cell_kwargs(r, c, key = 'dropdown')
+        kwargs['values'] = values
+        if kwargs['window'] != "no dropdown open":
+            kwargs['window'].values(values)
         if set_value is not None:
             self.set_cell_data(r_, c_, set_value)
-            if self.MT.cell_options[(r_, c_)]['dropdown']['window'] != "no dropdown open" and self.MT.text_editor_loc is not None and self.MT.text_editor is not None:
+            if kwargs['window'] != "no dropdown open" and self.MT.text_editor_loc is not None and self.MT.text_editor is not None:
                 self.MT.text_editor.set_text(set_value)
-
-    def delete_dropdown(self, r = 0, c = 0):
-        if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
-            for r_, c_ in self.MT.cell_options:
-                if 'dropdown' in self.MT.cell_options[(r_, c)]:
-                    self.MT.delete_dropdown(r_, c)
-        elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
-            for r_, c_ in self.MT.cell_options:
-                if 'dropdown' in self.MT.cell_options[(r, c_)]:
-                    self.MT.delete_dropdown(r, c_)
-        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
-            for r_, c_ in self.MT.cell_options:
-                if 'dropdown' in self.MT.cell_options[(r_, c_)]:
-                    self.MT.delete_dropdown(r_, c_)
+                
+    def set_header_dropdown_values(self, c = 0, set_existing_dropdown = False, values = [], set_value = None):
+        if set_existing_dropdown:
+            if self.CH.existing_dropdown_window is not None:
+                c_ = self.CH.existing_dropdown_window.c
+            else:
+                raise Exception("No dropdown box is currently open")
+        else:
+            c_ = c
+        kwargs = self.CH.get_cell_kwargs(c_, key = 'dropdown')
+        if kwargs:
+            kwargs['values'] = values
+            if kwargs['window'] != "no dropdown open":
+                kwargs['window'].values(values)
+            if set_value is not None:
+                self.MT.headers(newheaders = set_value, index = c_)
+                
+    def set_index_dropdown_values(self, r, set_existing_dropdown = False, values = [], set_value = None):
+        if set_existing_dropdown:
+            if self.RI.existing_dropdown_window is not None:
+                r_ = self.RI.existing_dropdown_window.r
+            else:
+                raise Exception("No dropdown box is currently open")
         else:
-            self.MT.delete_dropdown(r, c)
+            r_ = r
+        kwargs = self.RI.get_cell_kwargs(r_, key = 'dropdown')
+        if kwargs:
+            kwargs['values'] = values
+            if kwargs['window'] != "no dropdown open":
+                kwargs['window'].values(values)
+            if set_value is not None:
+                self.MT.row_index(newindex = set_value, index = r_)
 
-    def get_dropdowns(self):
-        return {k: v['dropdown'] for k, v in self.MT.cell_options.items() if 'dropdown' in v}
+    def get_dropdown_values(self, r = 0, c = 0):
+        kwargs = self.MT.get_cell_kwargs(r, c, key = 'dropdown')
+        if kwargs:
+            return kwargs['values']
+
+    def get_header_dropdown_values(self, c = 0):
+        kwargs = self.CH.get_cell_kwargs(c, key = 'dropdown')
+        if kwargs:
+            return kwargs['values']
+        
+    def get_index_dropdown_values(self, r = 0):
+        kwargs = self.RI.get_cell_kwargs(r, key = 'dropdown')
+        if kwargs:
+            kwargs['values']
+            
+    def dropdown_functions(self, r, c, selection_function = "", modified_function = ""):
+        kwargs = self.MT.get_cell_kwargs(r, c, key = 'dropdown')
+        if kwargs:
+            if selection_function != "":
+                kwargs['select_function'] = selection_function
+            if modified_function != "":
+                kwargs['modified_function'] = modified_function
+            return kwargs
+
+    def header_dropdown_functions(self, c, selection_function = "", modified_function = ""):
+        kwargs = self.CH.get_cell_kwargs(c, key = 'dropdown')
+        if selection_function != "":
+            kwargs['selection_function'] = selection_function
+        if modified_function != "":
+            kwargs['modified_function'] = modified_function
+        return kwargs
+    
+    def index_dropdown_functions(self, r, selection_function = "", modified_function = ""):
+        kwargs = self.RI.get_cell_kwargs(r, key = 'dropdown')
+        if selection_function != "":
+            kwargs['select_function'] = selection_function
+        if modified_function != "":
+            kwargs['modified_function'] = modified_function
+        return kwargs
+    
+    def get_dropdown_value(self, r = 0, c = 0):
+        if self.MT.get_cell_kwargs(r, c, key = 'dropdown'):
+            return self.get_cell_data(r, c)
+
+    def get_header_dropdown_value(self, c = 0):
+        if self.CH.get_cell_kwargs(c, key = 'dropdown'):
+            return self.MT._headers[c]
+
+    def get_index_dropdown_value(self, r = 0):
+        if self.RI.get_cell_kwargs(r, key = 'dropdown'):
+            return self.MT._row_index[r]
 
     def open_dropdown(self, r, c):
         self.MT.open_dropdown_window(r, c)
 
     def close_dropdown(self, r, c):
         self.MT.close_dropdown_window(r, c)
+    
+    def open_header_dropdown(self, c):
+        self.CH.open_dropdown_window(c)
+
+    def close_header_dropdown(self, c):
+        self.CH.close_dropdown_window(c)
+    
+    def open_index_dropdown(self, r):
+        self.RI.open_dropdown_window(r)
+
+    def close_index_dropdown(self, r):
+        self.RI.close_dropdown_window(r)
 
     def reapply_formatting(self):
         self.MT.reapply_formatting()
         
     def reapply_formatting(self):
         self.MT.reapply_formatting()
```

### Comparing `tksheet-6.0.2/tksheet/_tksheet_column_headers.py` & `tksheet-6.0.3/tksheet/_tksheet_column_headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self.extra_b1_release_func = None
         self.extra_double_b1_func = None
         self.ch_extra_begin_drag_drop_func = None
         self.ch_extra_end_drag_drop_func = None
         self.extra_rc_func = None
         self.selection_binding_func = None
         self.shift_selection_binding_func = None
+        self.ctrl_selection_binding_func = None
         self.drag_selection_binding_func = None
         self.column_width_resize_func = None
         self.width_resizing_enabled = False
         self.height_resizing_enabled = False
         self.double_click_resizing_enabled = False
         self.col_selection_enabled = False
         self.drag_and_drop_enabled = False
@@ -59,14 +60,15 @@
         self.rc_insert_col_enabled = False
         self.hide_columns_enabled = False
         self.edit_cell_enabled = False
         self.dragged_col = None
         self.visible_col_dividers = {}
         self.col_height_resize_bbox = tuple()
         self.cell_options = {}
+        self.options = {}
         self.rsz_w = None
         self.rsz_h = None
         self.new_col_height = 0
         self.lines_start_at = 0
         self.currently_resizing_width = False
         self.currently_resizing_height = False
         self.ch_rc_popup_menu = None
@@ -84,16 +86,14 @@
         self.hidd_fill_sels = {}
         self.hidd_resize_lines = {}
         self.hidd_dropdown = {}
         self.hidd_checkbox = {}
         
         self.column_drag_and_drop_perform = kwargs['column_drag_and_drop_perform']
         self.default_header = kwargs['default_header'].lower()
-        self.max_cw = float(kwargs['max_colwidth'])
-        self.max_header_height = float(kwargs['max_header_height'])
         self.header_bg = kwargs['header_bg']
         self.header_fg = kwargs['header_fg']
         self.header_grid_fg = kwargs['header_grid_fg']
         self.header_border_fg = kwargs['header_border_fg']
         self.header_selected_cells_bg = kwargs['header_selected_cells_bg']
         self.header_selected_cells_fg = kwargs['header_selected_cells_fg']
         self.header_selected_columns_bg = kwargs['header_selected_columns_bg']
@@ -108,23 +108,23 @@
     def basic_bindings(self, enable = True):
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
-            self.bind(get_rc_binding(), self.rc)
+            self.bind(rc_binding, self.rc)
             self.bind("<MouseWheel>", self.mousewheel)
         else:
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
-            self.unbind(get_rc_binding())
+            self.unbind(rc_binding)
             self.unbind("<MouseWheel>")
             
     def mousewheel(self, event = None):
         maxlines = 0
         if isinstance(self.MT._headers, int):
             if len(self.MT.data) > self.MT._headers:
                 maxlines = max(len(self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True).rstrip().split("\n")) for datacn in range(len(self.MT.data[self.MT._headers])))
@@ -206,20 +206,61 @@
                         self.toggle_select_col(c, redraw = True)
                     if self.MT.rc_popup_menus_enabled:
                         popup_menu = self.ch_rc_popup_menu
         if self.extra_rc_func is not None:
             self.extra_rc_func(event)
         if popup_menu is not None:
             popup_menu.tk_popup(event.x_root, event.y_root)
+            
+    def ctrl_b1_press(self, event = None):
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
+        if (self.drag_and_drop_enabled or self.col_selection_enabled) and self.MT.ctrl_select_enabled and self.rsz_h is None and self.rsz_w is None:
+            c = self.MT.identify_col(x = event.x)
+            if c < len(self.MT.col_positions) - 1:
+                c_selected = self.MT.col_selected(c)
+                if not c_selected and self.col_selection_enabled:
+                    self.add_selection(c, set_as_current = True)
+                    self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+                    if self.ctrl_selection_binding_func is not None:
+                        self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_columns", (c, c + 1)))
+                elif c_selected:
+                    self.dragged_col = DraggedRowColumn(dragged = c, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c))
+                    
+    def ctrl_shift_b1_press(self, event):
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
+        x = event.x
+        c = self.MT.identify_col(x = x)
+        if (self.drag_and_drop_enabled or self.col_selection_enabled) and self.MT.ctrl_select_enabled and self.rsz_h is None and self.rsz_w is None:
+            if c < len(self.MT.col_positions) - 1:
+                c_selected = self.MT.col_selected(c)
+                if not c_selected and self.col_selection_enabled:
+                    c = int(c)
+                    currently_selected = self.MT.currently_selected()
+                    if currently_selected and currently_selected.type_ == "column":
+                        min_c = int(currently_selected[1])
+                        if c > min_c:
+                            self.MT.create_selected(0, min_c, len(self.MT.row_positions) - 1, c + 1, "columns")
+                            func_event = tuple(range(min_c, c + 1))
+                        elif c < min_c:
+                            self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, min_c + 1, "columns")
+                            func_event = tuple(range(c, min_c + 1))
+                    else:
+                        self.add_selection(c, set_as_current = True)
+                        func_event = (c, )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+                    if self.ctrl_selection_binding_func is not None:
+                        self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_columns", func_event))
+                elif c_selected:
+                    self.dragged_col = DraggedRowColumn(dragged = c, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c))
 
     def shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         x = event.x
         c = self.MT.identify_col(x = x)
-        if self.drag_and_drop_enabled or self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+        if (self.drag_and_drop_enabled or self.col_selection_enabled) and self.rsz_h is None and self.rsz_w is None:
             if c < len(self.MT.col_positions) - 1:
                 c_selected = self.MT.col_selected(c)
                 if not c_selected and self.col_selection_enabled:
                     c = int(c)
                     currently_selected = self.MT.currently_selected()
                     if currently_selected and currently_selected.type_ == "column":
                         min_c = int(currently_selected[1])
@@ -233,15 +274,15 @@
                     else:
                         self.select_col(c)
                         func_event = (c, )
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.shift_selection_binding_func is not None:
                         self.shift_selection_binding_func(SelectionBoxEvent("shift_select_columns", func_event))
                 elif c_selected:
-                    self.dragged_col = c
+                    self.dragged_col = DraggedRowColumn(dragged = c, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c))
 
     def create_resize_line(self, x1, y1, x2, y2, width, fill, tag):
         if self.hidd_resize_lines:
             t, sh = self.hidd_resize_lines.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
                 self.itemconfig(t, width = width, fill = fill, tag = tag)
@@ -307,16 +348,16 @@
             c = self.MT.identify_col(x = event.x)
             if c < len(self.MT.col_positions) - 1:
                 if self.MT.single_selection_enabled:
                     self.select_col(c, redraw = True)
                 elif self.MT.toggle_selection_enabled:
                     self.toggle_select_col(c, redraw = True)
                 datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                if ((datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]) or
-                    (datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]) or
+                if (self.get_cell_kwargs(datacn, key = 'dropdown') or
+                    self.get_cell_kwargs(datacn, key = 'checkbox') or
                     self.edit_cell_enabled):
                     self.open_cell(event)
         self.rsz_w = None
         self.mouse_motion(event)
         if self.extra_double_b1_func is not None:
             self.extra_double_b1_func(event)
         
@@ -339,106 +380,66 @@
             self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
             self.create_resize_line(line2x, 0, line2x, self.current_height,width = 1, fill = self.resizing_line_fg, tag = "rwl2")
             self.MT.create_resize_line(line2x, y1, line2x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl2")
         elif self.height_resizing_enabled and self.rsz_w is None and self.rsz_h is not None:
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
             self.currently_resizing_height = True
             y = event.y
-            if y < self.MT.hdr_min_rh:
-                y = int(self.MT.hdr_min_rh)
+            if y < self.MT.min_header_height:
+                y = int(self.MT.min_header_height)
             self.new_col_height = y
             self.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
         elif self.MT.identify_col(x = event.x, allow_end = False) is None:
             self.MT.deselect("all")
         elif self.col_selection_enabled and self.rsz_w is None and self.rsz_h is None:
             if c < len(self.MT.col_positions) - 1:
-                if self.MT.col_selected(c):
-                    datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                    if ((datacn in self.cell_options and 'dropdown' in self.cell_options[datacn] and x < self.MT.col_positions[c + 1] and x > self.MT.col_positions[c + 1] - self.MT.hdr_txt_h - 4) or
-                        (datacn in self.cell_options and 'checkbox' in self.cell_options[datacn] and x < self.MT.col_positions[c] + self.MT.hdr_txt_h + 5)) and event.y < self.MT.hdr_txt_h + 5:
-                        pass
-                    else:
-                        self.dragged_col = c
+                datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+                if self.MT.col_selected(c) and not self.event_over_dropdown(c, datacn, event, x) and not self.event_over_checkbox(c, datacn, event, x):
+                    self.dragged_col = DraggedRowColumn(dragged = c, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c))
                 else:
                     self.being_drawn_rect = (0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
                     if self.MT.single_selection_enabled:
                         self.select_col(c, redraw = True)
                     elif self.MT.toggle_selection_enabled:
                         self.toggle_select_col(c, redraw = True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
     
     def b1_motion(self, event):
         x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
         if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             x = self.canvasx(event.x)
             size = x - self.MT.col_positions[self.rsz_w - 1]
-            if size >= self.MT.min_cw and size < self.max_cw:
-                self.delete_resize_lines()
-                self.MT.delete_resize_lines()
+            if size >= self.MT.min_column_width and size < self.MT.max_column_width:
+                self.delete_all_resize_and_ctrl_lines(ctrl_lines = False)
                 line2x = self.MT.col_positions[self.rsz_w - 1]
                 self.create_resize_line(x, 0, x, self.current_height, width = 1, fill = self.resizing_line_fg, tag = "rwl")
                 self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
                 self.create_resize_line(line2x, 0, line2x, self.current_height,width = 1, fill = self.resizing_line_fg, tag = "rwl2")
                 self.MT.create_resize_line(line2x, y1, line2x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl2")
         elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             evy = event.y
-            self.delete_resize_lines()
-            self.MT.delete_resize_lines()
+            self.delete_all_resize_and_ctrl_lines(ctrl_lines = False)
             if evy > self.current_height:
                 y = self.MT.canvasy(evy - self.current_height)
-                if evy > self.max_header_height:
-                    evy = int(self.max_header_height)
+                if evy > self.MT.max_header_height:
+                    evy = int(self.MT.max_header_height)
                     y = self.MT.canvasy(evy - self.current_height)
                 self.new_col_height = evy
                 self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
             else:
                 y = evy
-                if y < self.MT.hdr_min_rh:
-                    y = int(self.MT.hdr_min_rh)
+                if y < self.MT.min_header_height:
+                    y = int(self.MT.min_header_height)
                 self.new_col_height = y
                 self.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
         elif self.drag_and_drop_enabled and self.col_selection_enabled and self.MT.anything_selected(exclude_cells = True, exclude_rows = True) and self.rsz_h is None and self.rsz_w is None and self.dragged_col is not None:
             x = self.canvasx(event.x)
             if x > 0 and x < self.MT.col_positions[-1]:
-                x = event.x
-                wend = self.winfo_width()
-                xcheck = self.xview()
-                if x >= wend - 0 and len(xcheck) > 1 and xcheck[1] < 1:
-                    if x >= wend + 15:
-                        self.MT.xview_scroll(2, "units")
-                        self.xview_scroll(2, "units")
-                    else:
-                        self.MT.xview_scroll(1, "units")
-                        self.xview_scroll(1, "units")
-                    self.check_xview()
-                    self.MT.main_table_redraw_grid_and_text(redraw_header = True)
-                elif x <= 0 and len(xcheck) > 1 and xcheck[0] > 0:
-                    if x >= -15:
-                        self.MT.xview_scroll(-1, "units")
-                        self.xview_scroll(-1, "units")
-                    else:
-                        self.MT.xview_scroll(-2, "units")
-                        self.xview_scroll(-2, "units")
-                    self.check_xview()
-                    self.MT.main_table_redraw_grid_and_text(redraw_header = True)
-                col = self.MT.identify_col(x = event.x)
-                sels = self.MT.get_selected_cols()
-                selsmin = min(sels)
-                if col in sels:
-                    xpos = self.MT.col_positions[selsmin]
-                else:
-                    if col < selsmin:
-                        xpos = self.MT.col_positions[col]
-                    else:
-                        xpos = self.MT.col_positions[col + 1]
-                self.delete_resize_lines()
-                self.MT.delete_resize_lines()
-                self.create_resize_line(xpos, 0, xpos, self.current_height, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
-                self.MT.create_resize_line(xpos, y1, xpos, y2, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+                self.show_drag_and_drop_indicators(self.drag_and_drop_motion(event), y1, y2, self.dragged_col.to_move[0], self.dragged_col.to_move[-1])
         elif self.MT.drag_selection_enabled and self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             need_redraw = False
             end_col = self.MT.identify_col(x = event.x)
             currently_selected = self.MT.currently_selected()
             if end_col < len(self.MT.col_positions) - 1 and currently_selected:
                 if currently_selected.type_ == "column":
                     start_col = currently_selected[1]
@@ -451,90 +452,180 @@
                     if self.being_drawn_rect != rect:
                         need_redraw = True
                         self.MT.delete_selection_rects(delete_current = False)
                         self.MT.create_selected(*rect)
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
                             self.drag_selection_binding_func(SelectionBoxEvent("drag_select_columns", func_event))
-                xcheck = self.xview()
-                if event.x > self.winfo_width() and len(xcheck) > 1 and xcheck[1] < 1:
-                    try:
-                        self.MT.xview_scroll(1, "units")
-                        self.xview_scroll(1, "units")
-                    except:
-                        pass
-                    self.check_xview()
-                    need_redraw = True
-                elif event.x < 0 and self.canvasx(self.winfo_width()) > 0 and xcheck and xcheck[0] > 0:
-                    try:
-                        self.xview_scroll(-1, "units")
-                        self.MT.xview_scroll(-1, "units")
-                    except:
-                        pass
-                    self.check_xview()
+                if self.scroll_if_event_offscreen(event):
                     need_redraw = True
             if need_redraw:
                 self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False)
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
+            
+    def ctrl_b1_motion(self, event):
+        x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
+        if self.drag_and_drop_enabled and self.col_selection_enabled and self.MT.anything_selected(exclude_cells = True, exclude_rows = True) and self.rsz_h is None and self.rsz_w is None and self.dragged_col is not None:
+            x = self.canvasx(event.x)
+            if x > 0 and x < self.MT.col_positions[-1]:
+                self.show_drag_and_drop_indicators(self.drag_and_drop_motion(event), y1, y2, self.dragged_col.to_move[0], self.dragged_col.to_move[-1])
+        elif self.MT.ctrl_select_enabled and self.MT.drag_selection_enabled and self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+            need_redraw = False
+            end_col = self.MT.identify_col(x = event.x)
+            currently_selected = self.MT.currently_selected()
+            if end_col < len(self.MT.col_positions) - 1 and currently_selected:
+                if currently_selected.type_ == "column":
+                    start_col = currently_selected[1]
+                    if end_col >= start_col:
+                        rect = (0, start_col, len(self.MT.row_positions) - 1, end_col + 1, "columns")
+                        func_event = tuple(range(start_col, end_col + 1))
+                    elif end_col < start_col:
+                        rect = (0, end_col, len(self.MT.row_positions) - 1, start_col + 1, "columns")
+                        func_event = tuple(range(end_col, start_col + 1))
+                    if self.being_drawn_rect != rect:
+                        need_redraw = True
+                        if self.being_drawn_rect is not None:
+                            self.MT.delete_selected(*self.being_drawn_rect)
+                        self.MT.create_selected(*rect)
+                        self.being_drawn_rect = rect
+                        if self.drag_selection_binding_func is not None:
+                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_columns", func_event))
+                if self.scroll_if_event_offscreen(event):
+                    need_redraw = True
+            if need_redraw:
+                self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False)
+                
+    def drag_and_drop_motion(self, event):
+        x = event.x
+        wend = self.winfo_width()
+        xcheck = self.xview()
+        if x >= wend - 0 and len(xcheck) > 1 and xcheck[1] < 1:
+            if x >= wend + 15:
+                self.MT.xview_scroll(2, "units")
+                self.xview_scroll(2, "units")
+            else:
+                self.MT.xview_scroll(1, "units")
+                self.xview_scroll(1, "units")
+            self.fix_xview()
+            self.MT.main_table_redraw_grid_and_text(redraw_header = True)
+        elif x <= 0 and len(xcheck) > 1 and xcheck[0] > 0:
+            if x >= -15:
+                self.MT.xview_scroll(-1, "units")
+                self.xview_scroll(-1, "units")
+            else:
+                self.MT.xview_scroll(-2, "units")
+                self.xview_scroll(-2, "units")
+            self.fix_xview()
+            self.MT.main_table_redraw_grid_and_text(redraw_header = True)
+        col = self.MT.identify_col(x = event.x)
+        if col >= self.dragged_col.to_move[0] and col <= self.dragged_col.to_move[-1]:
+            xpos = self.MT.col_positions[self.dragged_col.to_move[0]]
+        else:
+            if col < self.dragged_col.to_move[0]:
+                xpos = self.MT.col_positions[col]
+            else:
+                xpos = self.MT.col_positions[col + 1]
+        return xpos
+
+    def show_drag_and_drop_indicators(self, xpos, y1, y2, start_col, end_col):
+        self.delete_all_resize_and_ctrl_lines()
+        self.create_resize_line(xpos, 0, xpos, self.current_height, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+        self.MT.create_resize_line(xpos, y1, xpos, y2, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+        self.MT.show_ctrl_outline(start_cell = (start_col, 0),
+                                  end_cell = (end_col + 1, len(self.MT.row_positions) - 1),
+                                  dash = (),
+                                  outline = self.drag_and_drop_bg,
+                                  delete_on_timer = False)
+        
+    def delete_all_resize_and_ctrl_lines(self, ctrl_lines = True):
+        self.delete_resize_lines()
+        self.MT.delete_resize_lines()
+        if ctrl_lines:
+            self.MT.delete_ctrl_outlines()
+
+    def scroll_if_event_offscreen(self, event):
+        xcheck = self.xview()
+        need_redraw = False
+        if event.x > self.winfo_width() and len(xcheck) > 1 and xcheck[1] < 1:
+            try:
+                self.MT.xview_scroll(1, "units")
+                self.xview_scroll(1, "units")
+            except:
+                pass
+            self.fix_xview()
+            need_redraw = True
+        elif event.x < 0 and self.canvasx(self.winfo_width()) > 0 and xcheck and xcheck[0] > 0:
+            try:
+                self.xview_scroll(-1, "units")
+                self.MT.xview_scroll(-1, "units")
+            except:
+                pass
+            self.fix_xview()
+            need_redraw = True
+        return need_redraw
 
-    def check_xview(self):
+    def fix_xview(self):
         xcheck = self.xview()
         if xcheck and xcheck[0] < 0:
             self.MT.set_xviews("moveto", 0)
         elif len(xcheck) > 1 and xcheck[1] > 1:
             self.MT.set_xviews("moveto", 1)
             
+    def event_over_dropdown(self, c, datacn, event, canvasx):
+        if (event.y < self.MT.header_txt_h + 5 and
+            self.get_cell_kwargs(datacn, key = 'dropdown') and 
+            canvasx < self.MT.col_positions[c + 1] and 
+            canvasx > self.MT.col_positions[c + 1] - self.MT.header_txt_h - 4):
+            return True
+        return False
+                    
+    def event_over_checkbox(self, c, datacn, event, canvasx):
+        if (event.y < self.MT.header_txt_h + 5 and
+            self.get_cell_kwargs(datacn, key = 'checkbox') and
+            canvasx < self.MT.col_positions[c] + self.MT.header_txt_h + 4):
+            return True
+        return False
+            
     def b1_release(self, event = None):
         if self.being_drawn_rect is not None:
+            self.MT.delete_selected(*self.being_drawn_rect)
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.MT.create_selected(*to_sel)
         self.MT.bind("<MouseWheel>", self.MT.mousewheel)
         if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             self.currently_resizing_width = False
             new_col_pos = int(self.coords("rwl")[0])
-            self.delete_resize_lines()
-            self.MT.delete_resize_lines()
+            self.delete_all_resize_and_ctrl_lines(ctrl_lines = False)
             old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
             size = new_col_pos - self.MT.col_positions[self.rsz_w - 1]
-            if size < self.MT.min_cw:
-                new_col_pos = ceil(self.MT.col_positions[self.rsz_w - 1] + self.MT.min_cw)
-            elif size > self.max_cw:
-                new_col_pos = floor(self.MT.col_positions[self.rsz_w - 1] + self.max_cw)
+            if size < self.MT.min_column_width:
+                new_col_pos = ceil(self.MT.col_positions[self.rsz_w - 1] + self.MT.min_column_width)
+            elif size > self.MT.max_column_width:
+                new_col_pos = floor(self.MT.col_positions[self.rsz_w - 1] + self.MT.max_column_width)
             increment = new_col_pos - self.MT.col_positions[self.rsz_w]
             self.MT.col_positions[self.rsz_w + 1:] = [e + increment for e in islice(self.MT.col_positions, self.rsz_w + 1, len(self.MT.col_positions))]
             self.MT.col_positions[self.rsz_w] = new_col_pos
             new_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
             self.MT.recreate_all_selection_boxes()
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
             if self.column_width_resize_func is not None and old_width != new_width:
                 self.column_width_resize_func(ResizeEvent("column_width_resize", self.rsz_w - 1, old_width, new_width))
         elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             self.currently_resizing_height = False
-            self.delete_resize_lines()
-            self.MT.delete_resize_lines()
-            self.set_height(self.new_col_height,set_TL = True)
+            self.delete_all_resize_and_ctrl_lines(ctrl_lines = False)
+            self.set_height(self.new_col_height, set_TL = True)
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         elif self.drag_and_drop_enabled and self.col_selection_enabled and self.MT.anything_selected(exclude_cells = True, exclude_rows = True) and self.rsz_h is None and self.rsz_w is None and self.dragged_col is not None:
-            self.delete_resize_lines()
-            self.MT.delete_resize_lines()
+            self.delete_all_resize_and_ctrl_lines()
             x = event.x
             c = self.MT.identify_col(x = x)
-            orig_selected = self.MT.get_selected_cols()
-            if c != self.dragged_col and c is not None and c not in orig_selected and len(orig_selected) != len(self.MT.col_positions) - 1:
-                orig_selected = sorted(orig_selected)
-                if len(orig_selected) > 1:
-                    start_idx = bisect.bisect_left(orig_selected, self.dragged_col)
-                    forward_gap = get_index_of_gap_in_sorted_integer_seq_forward(orig_selected, start_idx)
-                    reverse_gap = get_index_of_gap_in_sorted_integer_seq_reverse(orig_selected, start_idx)
-                    if forward_gap is not None:
-                        orig_selected[:] = orig_selected[:forward_gap]
-                    if reverse_gap is not None:
-                        orig_selected[:] = orig_selected[reverse_gap:]
+            orig_selected = self.dragged_col.to_move
+            if c != self.dragged_col.dragged and c is not None and (c < self.dragged_col.to_move[0] or c > self.dragged_col.to_move[-1]) and len(orig_selected) != len(self.MT.col_positions) - 1:
                 rm1start = orig_selected[0]
                 totalcols = len(orig_selected)
                 extra_func_success = True
                 if c >= len(self.MT.col_positions) - 1:
                     c -= 1
                 if self.ch_extra_begin_drag_drop_func is not None:
                     try:
@@ -543,41 +634,27 @@
                         extra_func_success = False
                 if extra_func_success:
                     new_selected, dispset = self.MT.move_columns_adjust_options_dict(c,
                                                                                      rm1start, 
                                                                                      totalcols,
                                                                                      move_data = self.column_drag_and_drop_perform)
                     if self.MT.undo_enabled:
-                        self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_cols",                 #0
-                                                                                int(orig_selected[0]),  #1
-                                                                                int(new_selected[0]),        #2
-                                                                                int(new_selected[-1]),       #3
-                                                                                sorted(orig_selected),  #4
-                                                                                dispset))))                  #5
+                        self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_cols",
+                                                                                orig_selected,
+                                                                                new_selected))))
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ch_extra_end_drag_drop_func is not None:
-                        self.ch_extra_end_drag_drop_func(EndDragDropEvent("end_column_header_drag_drop", tuple(orig_selected), new_selected, int(c)))
-                    self.event_generate("<<SheetDataChangeEvent>>")
+                        self.ch_extra_end_drag_drop_func(EndDragDropEvent("end_column_header_drag_drop", orig_selected, new_selected, int(c)))
+                    self.parentframe.emit_modified_event()
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             c = self.MT.identify_col(x = event.x)
             if c is not None and c < len(self.MT.col_positions) - 1 and c == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
                 datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
                 canvasx = self.canvasx(event.x)
-                if (event.y < self.MT.hdr_txt_h + 5 and
-                    (
-                     (datacn in self.cell_options and 
-                      'dropdown' in self.cell_options[datacn] and 
-                      canvasx < self.MT.col_positions[c + 1] and 
-                      canvasx > self.MT.col_positions[c + 1] - self.MT.hdr_txt_h - 4)
-                     or
-                     (datacn in self.cell_options and 
-                      'checkbox' in self.cell_options[datacn] and
-                      canvasx < self.MT.col_positions[c] + self.MT.hdr_txt_h + 5)
-                    )
-                ):
+                if self.event_over_dropdown(c, datacn, event, canvasx) or self.event_over_checkbox(c, datacn, event, canvasx):
                     self.open_cell(event)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases()
             self.b1_pressed_loc = None
             self.closed_dropdown = None
         self.dragged_col = None
         self.currently_resizing_width = False
@@ -599,45 +676,19 @@
                     del self.cell_options[c]['readonly']
         else:
             for c in columns_:
                 if c not in self.cell_options:
                     self.cell_options[c] = {}
                 self.cell_options[c]['readonly'] = True
 
-    def highlight_cells(self, c = 0, cells = tuple(), bg = None, fg = None, redraw = False, overwrite = True):
-        if bg is None and fg is None:
-            return
-        if cells and not isinstance(cells, int):
-            iterable = cells
-        elif isinstance(cells, int):
-            iterable = (cells, )
-        else:
-            iterable = (c, )
-        for c_ in iterable:
-            if c_ not in self.cell_options:
-                self.cell_options[c_] = {}
-            if 'highlight' in self.cell_options[c_] and not overwrite:
-                self.cell_options[c_]['highlight'] = (self.cell_options[c_]['highlight'][0] if bg is None else bg,
-                                                      self.cell_options[c_]['highlight'][1] if fg is None else fg)
-            else:
-                self.cell_options[c_]['highlight'] = (bg, fg)
-        if redraw:
-            self.MT.main_table_redraw_grid_and_text(True, False)
-
     def select_col(self, c, redraw = False, keep_other_selections = False):
-        ignore_keep = False
-        if keep_other_selections:
-            if self.MT.col_selected(c):
-                self.MT.create_current(0, c, type_ = "column", inside = True)
-            else:
-                ignore_keep = True
-        if ignore_keep or not keep_other_selections:
+        if not keep_other_selections:
             self.MT.delete_selection_rects()
-            self.MT.create_current(0, c, type_ = "column", inside = True)
-            self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
+        self.MT.create_current(0, c, type_ = "column", inside = True)
+        self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None:
             self.selection_binding_func(SelectColumnEvent("select_column", int(c)))
 
     def toggle_select_col(self, column, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
         if add_selection:
@@ -668,38 +719,95 @@
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(("select_column", int(c)))
             
     def get_cell_dimensions(self, datacn):
         txt = self.get_valid_cell_data_as_str(datacn, fix = False)
         if txt:
-            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text = txt, font = self.MT._hdr_font)
+            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text = txt, font = self.MT.header_font)
             b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
             w = b[2] - b[0] + 7
             h = b[3] - b[1] + 5
         else:
-            w = self.MT.min_cw
-            h = self.MT.hdr_min_rh
-        if datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 'checkbox' in self.cell_options[datacn]):
-            return w + self.MT.hdr_txt_h, h
+            w = self.MT.min_column_width
+            h = self.MT.min_header_height
+        if datacn in self.cell_options and (self.get_cell_kwargs(datacn, key = 'dropdown') or self.get_cell_kwargs(datacn, key = 'checkbox')):
+            return w + self.MT.header_txt_h, h
         return w, h
+    
+    def set_height_of_header_to_text(self, text = None):
+        if (text is None and not self.MT._headers and isinstance(self.MT._headers, list) or 
+            isinstance(self.MT._headers, int) and self.MT._headers >= len(self.MT.data)
+            ):
+            return
+        qconf = self.MT.txt_measure_canvas.itemconfig
+        qbbox = self.MT.txt_measure_canvas.bbox
+        qtxtm = self.MT.txt_measure_canvas_text
+        new_height = self.MT.min_header_height
+        self.fix_header()
+        if text is not None:
+            if text:
+                qconf(qtxtm, text = text)
+                b = qbbox(qtxtm)
+                h = b[3] - b[1] + 5
+                if h > new_height:
+                    new_height = h
+        else:
+            if self.MT.all_columns_displayed:
+                if isinstance(self.MT._headers, list):
+                    iterable = range(len(self.MT._headers))
+                else:
+                    iterable = range(len(self.MT.data[self.MT._headers]))
+            else:
+                iterable = self.MT.displayed_columns
+            if isinstance(self.MT._headers, list):
+                for datacn in iterable:
+                    w_, h = self.get_cell_dimensions(datacn)
+                    if h < self.MT.min_header_height:
+                        h = int(self.MT.min_header_height)
+                    elif h > self.MT.max_header_height:
+                        h = int(self.MT.max_header_height)
+                    if h > new_height:
+                        new_height = h
+            elif isinstance(self.MT._headers, int):
+                datarn = self.MT._headers
+                for datacn in iterable:
+                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
+                    if txt:
+                        qconf(qtxtm, text = txt)
+                        b = qbbox(qtxtm)
+                        h = b[3] - b[1] + 5
+                    else:
+                        h = self.default_header_height
+                    if h < self.MT.min_header_height:
+                        h = int(self.MT.min_header_height)
+                    elif h > self.MT.max_header_height:
+                        h = int(self.MT.max_header_height)
+                    if h > new_height:
+                        new_height = h
+        space_bot = self.MT.get_space_bot(0)
+        if new_height > space_bot:
+            new_height = space_bot
+        self.set_height(new_height, set_TL = True)
+        self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+        return new_height
 
     def set_col_width(self, col, width = None, only_set_if_too_small = False, displayed_only = False, recreate = True, return_new_width = False):
         if col < 0:
             return
         qconf = self.MT.txt_measure_canvas.itemconfig
         qbbox = self.MT.txt_measure_canvas.bbox
         qtxtm = self.MT.txt_measure_canvas_text
         qtxth = self.MT.txt_h
         qclop = self.MT.cell_options
-        qfont = self.MT._font
+        qfont = self.MT.table_font
         self.fix_header()
         if width is None:
-            w = self.MT.min_cw
-            hw = self.MT.min_cw
+            w = self.MT.min_column_width
+            hw = self.MT.min_column_width
             if self.MT.all_rows_displayed:
                 if displayed_only:
                     x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
                     start_row, end_row = self.MT.get_visible_rows(y1, y2)
                 else:
                     start_row, end_row = 0, len(self.MT.data)
                 iterable = range(start_row, end_row)
@@ -716,30 +824,30 @@
             # table
             if self.MT.data:
                 for datarn in iterable:
                     txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
                     if txt:
                         qconf(qtxtm, text = txt, font = qfont)
                         b = qbbox(qtxtm)
-                        if (datarn, datacn) in qclop and ('dropdown' in qclop[(datarn, datacn)] or 'checkbox' in qclop[(datarn, datacn)]):
+                        if self.MT.get_cell_kwargs(datarn, datacn, key = 'dropdown') or self.MT.get_cell_kwargs(datarn, datacn, key = 'checkbox'):
                             tw = b[2] - b[0] + qtxth + 7
                         else:
                             tw = b[2] - b[0] + 7
                         if tw > w:
                             w = tw
             if w > hw:
                 new_width = w
             else:
                 new_width = hw
         else:
             new_width = int(width)
-        if new_width <= self.MT.min_cw:
-            new_width = int(self.MT.min_cw)
-        elif new_width > self.max_cw:
-            new_width = int(self.max_cw)
+        if new_width <= self.MT.min_column_width:
+            new_width = int(self.MT.min_column_width)
+        elif new_width > self.MT.max_column_width:
+            new_width = int(self.MT.max_column_width)
         if only_set_if_too_small:
             if new_width <= self.MT.col_positions[col + 1] - self.MT.col_positions[col]:
                 return self.MT.col_positions[col + 1] - self.MT.col_positions[col]
         if not return_new_width:
             new_col_pos = self.MT.col_positions[col] + new_width
             increment = new_col_pos - self.MT.col_positions[col + 1]
             self.MT.col_positions[col + 2:] = [e + increment for e in islice(self.MT.col_positions, col + 2, len(self.MT.col_positions))]
@@ -774,59 +882,48 @@
                     del self.cell_options[c]['align']
         else:
             for c in cols:
                 if c not in self.cell_options:
                     self.cell_options[c] = {}
                 self.cell_options[c]['align'] = align
 
-    def redraw_highlight_get_text_fg(self, fc, sc, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, hlcol):
+    def redraw_highlight_get_text_fg(self, fc, sc, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, datacn):
         redrawn = False
-        if hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol] and c in actual_selected_cols:
-            if self.cell_options[hlcol]['highlight'][0] is not None:
-                c_1 = self.cell_options[hlcol]['highlight'][0] if self.cell_options[hlcol]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[hlcol]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1,
-                                                0,
-                                                sc,
-                                                self.current_height - 1,
-                                                fill = (f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}" +
-                                                        f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}" +
-                                                        f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"),
-                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "",
-                                                tag = "hi")
-            fill = self.header_selected_columns_fg if self.cell_options[hlcol]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[hlcol]['highlight'][1]
-        elif hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol] and (c in selected_cols or selected_rows):
-            if self.cell_options[hlcol]['highlight'][0] is not None:
-                c_1 = self.cell_options[hlcol]['highlight'][0] if self.cell_options[hlcol]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[hlcol]['highlight'][0]]
+        kwargs = self.get_cell_kwargs(datacn, key = 'highlight')
+        if kwargs:
+            if kwargs[0] is not None:
+                c_1 = kwargs[0] if kwargs[0].startswith("#") else Color_Map_[kwargs[0]]
+            if c in actual_selected_cols:
+                tf = self.header_selected_columns_fg if kwargs[1] is None or self.MT.display_selected_fg_over_highlights else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}" + f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}" + f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"
+            elif (c in selected_cols or selected_rows):
+                tf = self.header_selected_cells_fg if kwargs[1] is None or self.MT.display_selected_fg_over_highlights else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}" + f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}" + f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"
+            else:
+                tf = self.header_fg if kwargs[1] is None else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = kwargs[0]
+            if kwargs[0] is not None:
                 redrawn = self.redraw_highlight(fc + 1,
                                                 0,
                                                 sc,
                                                 self.current_height - 1,
-                                                fill = (f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}" +
-                                                        f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}" +
-                                                        f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"),
-                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "", 
-                                                tag = "hi")
-            fill = self.header_selected_cells_fg if self.cell_options[hlcol]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[hlcol]['highlight'][1]
-        elif c in actual_selected_cols:
-            fill = self.header_selected_columns_fg
-        elif c in selected_cols or selected_rows:
-            fill = self.header_selected_cells_fg
-        elif hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol]:
-            if self.cell_options[hlcol]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(fc + 1,
-                                                0, 
-                                                sc, 
-                                                self.current_height - 1, 
-                                                fill = self.cell_options[hlcol]['highlight'][0], 
-                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "", 
+                                                fill = fill,
+                                                outline = self.header_fg if self.get_cell_kwargs(datacn, key = 'dropdown') and self.MT.show_dropdown_borders else "",
                                                 tag = "hi")
-            fill = self.header_fg if self.cell_options[hlcol]['highlight'][1] is None else self.cell_options[hlcol]['highlight'][1]
-        else:
-            fill = self.header_fg
-        return fill, redrawn
+        elif not kwargs:
+            if c in actual_selected_cols:
+                tf = self.header_selected_columns_fg
+            elif c in selected_cols or selected_rows:
+                tf = self.header_selected_cells_fg
+            else:
+                tf = self.header_fg
+        return tf, redrawn
             
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         config = (fill, outline)
         coords = (x1 - 1 if outline else x1,
                   y1 - 1 if outline else y1,
                   x2, 
                   y2)
@@ -876,29 +973,29 @@
         else:
             self.disp_grid[self.create_line(points, fill = fill, width = width, tag = tag)] = True
             
     def redraw_dropdown(self, x1, y1, x2, y2, fill, outline, tag, draw_outline = True, draw_arrow = True, dd_is_open = False):
         if draw_outline and self.MT.show_dropdown_borders:
             self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill = "", outline = self.header_fg, tag = tag)
         if draw_arrow:
-            topysub = floor(self.MT.hdr_half_txt_h / 2)
-            mid_y = y1 + floor(self.MT.hdr_min_rh / 2)
-            if mid_y + topysub + 1 >= y1 + self.MT.hdr_txt_h - 1:
+            topysub = floor(self.MT.header_half_txt_h / 2)
+            mid_y = y1 + floor(self.MT.min_header_height / 2)
+            if mid_y + topysub + 1 >= y1 + self.MT.header_txt_h - 1:
                 mid_y -= 1
             if mid_y - topysub + 2 <= y1 + 4 + topysub:
                 mid_y -= 1
                 ty1 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
                 ty2 = mid_y - topysub + 3 if dd_is_open else mid_y + topysub + 1
                 ty3 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
             else:
                 ty1 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 2
                 ty2 = mid_y - topysub + 2 if dd_is_open else mid_y + topysub + 1
                 ty3 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 2
-            tx1 = x2 - self.MT.hdr_txt_h + 1
-            tx2 = x2 - self.MT.hdr_half_txt_h - 1
+            tx1 = x2 - self.MT.header_txt_h + 1
+            tx2 = x2 - self.MT.header_half_txt_h - 1
             tx3 = x2 - 3
             if tx2 - tx1 > tx3 - tx2:
                 tx1 += (tx2 - tx1) - (tx3 - tx2)
             elif tx2 - tx1 < tx3 - tx2:
                 tx1 -= (tx3 - tx2) - (tx2 - tx1)
             points = (tx1, ty1, tx2, ty2, tx3, ty3)
             if self.hidd_dropdown:
@@ -994,90 +1091,91 @@
                                    draw_x, -1,
                                    self.MT.col_positions[c + 1] if len(self.MT.col_positions) - 1 > c else draw_x, -1])
                 if points:
                     self.redraw_gridline(points = points, fill = self.header_grid_fg, width = 1, tag = "v")
         top = self.canvasy(0)
         c_2 = self.header_selected_cells_bg if self.header_selected_cells_bg.startswith("#") else Color_Map_[self.header_selected_cells_bg]
         c_3 = self.header_selected_columns_bg if self.header_selected_columns_bg.startswith("#") else Color_Map_[self.header_selected_columns_bg]
-        font = self.MT._hdr_font
+        font = self.MT.header_font
         for c in range(start_col, end_col - 1):
-            draw_y = self.MT.hdr_fl_ins
+            draw_y = self.MT.header_fl_ins
             cleftgridln = self.MT.col_positions[c]
             crightgridln = self.MT.col_positions[c + 1]
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             fill, dd_drawn = self.redraw_highlight_get_text_fg(cleftgridln, crightgridln, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, datacn)
 
             if datacn in self.cell_options and 'align' in self.cell_options[datacn]:
                 align = self.cell_options[datacn]['align']
             else:
                 align = self.align
-                
+            
+            kwargs = self.get_cell_kwargs(datacn, key = 'dropdown')
             if align == "w":
                 draw_x = cleftgridln + 3
-                if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
-                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
+                if kwargs:
+                    mw = crightgridln - cleftgridln - self.MT.header_txt_h - 2
                     self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[datacn]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = kwargs['window'] != "no dropdown open")
                 else:
                     mw = crightgridln - cleftgridln - 1
 
             elif align == "e":
-                if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
-                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
-                    draw_x = crightgridln - 5 - self.MT.hdr_txt_h
+                if kwargs:
+                    mw = crightgridln - cleftgridln - self.MT.header_txt_h - 2
+                    draw_x = crightgridln - 5 - self.MT.header_txt_h
                     self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1,
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[datacn]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = kwargs['window'] != "no dropdown open")
                 else:
                     mw = crightgridln - cleftgridln - 1
                     draw_x = crightgridln - 3
 
             elif align == "center":
                 #stop = cleftgridln + 5
-                if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
-                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
-                    draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.MT.hdr_txt_h) / 2)
+                if kwargs:
+                    mw = crightgridln - cleftgridln - self.MT.header_txt_h - 2
+                    draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.MT.header_txt_h) / 2)
                     self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[datacn]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = kwargs['window'] != "no dropdown open")
                 else:
                     mw = crightgridln - cleftgridln - 1
                     draw_x = cleftgridln + floor((crightgridln - cleftgridln) / 2)
-
-            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
-                if mw > self.MT.hdr_txt_h + 2:
-                    box_w = self.MT.hdr_txt_h + 1
+            kwargs = self.get_cell_kwargs(datacn, key = 'checkbox')
+            if kwargs:
+                if mw > self.MT.header_txt_h + 2:
+                    box_w = self.MT.header_txt_h + 1
                     mw -= box_w
                     if align == "w":
                         draw_x += box_w + 1
                     elif align == "center":
                         draw_x += ceil(box_w / 2) + 1
                         mw -= 1
                     else:
                         mw -= 3
                     try:
                         draw_check = self.MT._headers[datacn] if isinstance(self.MT._headers, (list, tuple)) else self.MT.data[self.MT._headers][datacn]
                     except:
                         draw_check = False
                     self.redraw_checkbox(cleftgridln + 2,
                                          2,
-                                         cleftgridln + self.MT.hdr_txt_h + 3,
-                                         self.MT.hdr_txt_h + 3,
-                                         fill = fill if self.cell_options[datacn]['checkbox']['state'] == "normal" else self.header_grid_fg,
+                                         cleftgridln + self.MT.header_txt_h + 3,
+                                         self.MT.header_txt_h + 3,
+                                         fill = fill if kwargs['state'] == "normal" else self.header_grid_fg,
                                          outline = "",
                                          tag = "cb", 
                                          draw_check = draw_check)
             lns = self.get_valid_cell_data_as_str(datacn, fix = False).split("\n")
             if lns == [""]:
                 if self.show_default_header_for_empty:
                     lns = (get_n2a(datacn, self.default_header), )
                 else:
                     continue
-            if mw > self.MT.hdr_txt_w and not ((align == "w" and (draw_x > x_stop)) or
+            if mw > self.MT.header_txt_w and not ((align == "w" and (draw_x > x_stop)) or
                                                (align == "e" and (draw_x > x_stop)) or
                                                (align == "center" and (cleftgridln + 5 > x_stop))):
                 for txt in islice(lns, self.lines_start_at if self.lines_start_at < len(lns) else len(lns) - 1, None):
                     if draw_y > top:
                         config = TextCfg(txt, fill, font, align)
                         k = None
                         if config in self.hidd_text:
@@ -1138,15 +1236,15 @@
                                     txt = txt[next(self.c_align_cyc)]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
                                 self.coords(iid, draw_x, draw_y)
                             self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = True))
                         else:
                             self.disp_text[config].add(DrawnItem(iid = iid, showing = True))
-                    draw_y += self.MT.hdr_xtra_lines_increment
+                    draw_y += self.MT.header_xtra_lines_increment
                     if draw_y - 1 > self.current_height:
                         break
         self.tag_raise("t")
         for cfg, set_ in self.hidd_text.items():
             for namedtup in tuple(set_):
                 if namedtup.showing:
                     self.itemconfig(namedtup.iid, state = "hidden")
@@ -1175,37 +1273,54 @@
         if not self.MT.anything_selected()  or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.MT.currently_selected()
         if not currently_selected:
             return
         x1 = int(currently_selected[1])
         datacn = x1 if self.MT.all_columns_displayed else self.MT.displayed_columns[x1]
-        if datacn in self.cell_options and 'readonly' in self.cell_options[datacn]:
+        if self.get_cell_kwargs(datacn, key = 'readonly'):
             return
-        elif datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 'checkbox' in self.cell_options[datacn]):
+        elif self.get_cell_kwargs(datacn, key = 'dropdown') or self.get_cell_kwargs(datacn, key = 'checkbox'):
             if self.MT.event_opens_dropdown_or_checkbox(event):
-                if 'dropdown' in self.cell_options[datacn]:
+                if self.get_cell_kwargs(datacn, key = 'dropdown'):
                     self.open_dropdown_window(x1, event = event)
-                elif 'checkbox' in self.cell_options[datacn]:
-                    self._click_checkbox(x1, datacn)
+                elif self.get_cell_kwargs(datacn, key = 'checkbox'):
+                    self.click_checkbox(x1, datacn)
         elif self.edit_cell_enabled:
-            self.edit_cell_(event, c = x1, dropdown = False)
+            self.open_text_editor(event = event, c = x1, dropdown = False)
+    
+    # displayed indexes
+    def get_cell_align(self, c):
+        datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+        if datacn in self.cell_options and 'align' in self.cell_options[datacn]:
+            align = self.cell_options[datacn]['align']
+        else:
+            align = self.align
+        return align
 
     # c is displayed col
-    def edit_cell_(self, event = None, c = None, dropdown = False):
+    def open_text_editor(self,
+                         event = None,
+                         c = 0,
+                         text = None,
+                         state = "normal",
+                         see = True,
+                         set_data_on_close = True,
+                         binding = None,
+                         dropdown = False):
         text = None
         extra_func_key = "??"
         if event is None or self.MT.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, 'keysym') and event.keysym == 'Return':
                     extra_func_key = "Return"
                 elif hasattr(event, 'keysym') and event.keysym == 'F2':
                     extra_func_key = "F2"
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            text = self.get_cell_data(datacn, redirect_int = True)
+            text = self.get_cell_data(datacn, none_to_empty_str = True, redirect_int = True)
         elif event is not None and ((hasattr(event, 'keysym') and event.keysym == 'BackSpace') or
                                     event.keycode in (8, 855638143)):
             extra_func_key = "BackSpace"
             text = ""
         elif event is not None and ((hasattr(event, "char") and event.char.isalpha()) or
                                     (hasattr(event, "char") and event.char.isdigit()) or
                                     (hasattr(event, "char") and event.char in symbols_set)):
@@ -1222,38 +1337,18 @@
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
-                self.set_current_height_to_text(text, datacn)
+                self.set_height_of_header_to_text(text)
             self.set_col_width_run_binding(c)
         self.select_col(c = c, keep_other_selections = True)
-        self.create_text_editor(c = c, text = text, set_data_on_close = True, dropdown = dropdown)
-        return True
-    
-    # displayed indexes
-    def get_cell_align(self, c):
-        datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-        if datacn in self.cell_options and 'align' in self.cell_options[datacn]:
-            align = self.cell_options[datacn]['align']
-        else:
-            align = self.align
-        return align
-
-    # c is displayed col
-    def create_text_editor(self,
-                           c = 0,
-                           text = None,
-                           state = "normal",
-                           see = True,
-                           set_data_on_close = False,
-                           binding = None,
-                           dropdown = False):
+        
         if c == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
             has_redrawn = self.MT.see(r = 0, c = c, keep_yscroll = True, check_cell_visibility = True)
@@ -1262,19 +1357,19 @@
         self.text_editor_loc = c
         x = self.MT.col_positions[c] + 1
         y = 0
         w = self.MT.col_positions[c + 1] - x
         h = self.current_height + 1
         datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         if text is None:
-            text = self.get_cell_data(datacn)
+            text = self.get_cell_data(datacn, none_to_empty_str = True, redirect_int = True)
         bg, fg = self.header_bg, self.header_fg
         self.text_editor = TextEditor(self,
                                       text = text,
-                                      font = self.MT._hdr_font,
+                                      font = self.MT.header_font,
                                       state = state,
                                       width = w,
                                       height = h,
                                       border_color = self.MT.table_selected_cells_border_fg,
                                       show_border = False,
                                       bg = bg,
                                       fg = fg,
@@ -1306,49 +1401,52 @@
             self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((c, "Tab")))
             self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((c, "Return")))
             if not dropdown:
                 self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((c, "FocusOut")))
             self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((c, "Escape")))
         else:
             self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
+        return True
     
     # displayed indexes                             #just here to receive text editor arg
     def text_editor_has_wrapped(self, r = 0, c = 0, check_lines = None):
         if self.width_resizing_enabled:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             curr_width = self.text_editor.winfo_width()
-            new_width = curr_width + (self.MT.hdr_txt_h * 2)
+            new_width = curr_width + (self.MT.header_txt_h * 2)
             if new_width != curr_width:
                 self.text_editor.config(width = new_width)
                 self.set_col_width_run_binding(c, width = new_width, only_set_if_too_small = False)
-                if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
-                    self.itemconfig(self.cell_options[datacn]['dropdown']['canvas_id'],
+                kwargs = self.get_cell_kwargs(datacn, key = 'dropdown')
+                if kwargs:
+                    self.itemconfig(kwargs['canvas_id'],
                                     width = new_width)
-                    self.cell_options[datacn]['dropdown']['window'].update_idletasks()
-                    self.cell_options[datacn]['dropdown']['window']._reselect()
+                    kwargs['window'].update_idletasks()
+                    kwargs['window']._reselect()
                 self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False, redraw_table = True)
     
     # displayed indexes
     def text_editor_newline_binding(self, r = 0, c = 0, event = None, check_lines = True):
         if self.height_resizing_enabled:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             curr_height = self.text_editor.winfo_height()
-            if not check_lines or self.MT.GetHdrLinesHeight(self.text_editor.get_num_lines() + 1) > curr_height:
-                new_height = curr_height + self.MT.hdr_xtra_lines_increment
+            if not check_lines or self.MT.get_lines_cell_height(self.text_editor.get_num_lines() + 1, font = self.MT.header_font) > curr_height:
+                new_height = curr_height + self.MT.header_xtra_lines_increment
                 space_bot = self.MT.get_space_bot(0)
                 if new_height > space_bot:
                     new_height = space_bot
                 if new_height != curr_height:
                     self.text_editor.config(height = new_height)
                     self.set_height(new_height, set_TL = True)
-                    if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
+                    kwargs = self.get_cell_kwargs(datacn, key = 'dropdown')
+                    if kwargs:
                         win_h, anchor = self.get_dropdown_height_anchor(datacn, new_height)
-                        self.coords(self.cell_options[datacn]['dropdown']['canvas_id'],
+                        self.coords(kwargs['canvas_id'],
                                     self.MT.col_positions[c], new_height - 1)
-                        self.itemconfig(self.cell_options[datacn]['dropdown']['canvas_id'],
+                        self.itemconfig(kwargs['canvas_id'],
                                         anchor = anchor, height = win_h)
             
     def bind_cell_edit(self, enable = True):
         if enable:
             self.edit_cell_enabled = True
         else:
             self.edit_cell_enabled = False
@@ -1427,269 +1525,282 @@
         if isinstance(self.MT._headers, int):
             self.MT.set_cell_data_undo(r = self.MT._headers, c = c, datacn = datacn, value = value, undo = True)
         else:
             self.fix_header(datacn)
             if not check_input_valid or self.input_valid_for_cell(datacn, value):
                 if self.MT.undo_enabled and undo:
                     self.MT.undo_storage.append(zlib.compress(pickle.dumps(("edit_header",
-                                                                            {datacn: self.MT._headers[datacn]},
-                                                                            (((0, c, len(self.MT.row_positions) - 1, c + 1), "columns"), ),
-                                                                            self.MT.currently_selected()))))
+                                                                           {datacn: self.MT._headers[datacn]},
+                                                                           self.MT.get_boxes(include_current = False),
+                                                                           self.MT.currently_selected()))))
                 self.set_cell_data(datacn = datacn, value = value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
-                self.set_current_height_to_text(value, datacn)
+                self.set_height_of_header_to_text(self.get_valid_cell_data_as_str(datacn, fix = False))
             self.set_col_width_run_binding(c)
         if redraw:
             self.MT.refresh()
-        self.event_generate("<<SheetDataChangeEvent>>")
+        self.parentframe.emit_modified_event()
     
     def set_cell_data(self, datacn = None, value = ""):
         if isinstance(self.MT._headers, int):
             self.MT.set_cell_data(datarn = self.MT._headers, datacn = datacn, value = value)
         else:
             self.fix_header(datacn)
-            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
+            if self.get_cell_kwargs(datacn, key = 'checkbox'):
                 self.MT._headers[datacn] = try_to_bool(value)
             else:
                 self.MT._headers[datacn] = value
     
     def input_valid_for_cell(self, datacn, value):
-        if datacn in self.cell_options:
-            if 'readonly' in self.cell_options[datacn]:
-                return False
-            if 'checkbox' in self.cell_options[datacn]:
-                return is_bool_like(value)
+        if self.get_cell_kwargs(datacn, key = 'readonly'):
+            return False
+        if self.get_cell_kwargs(datacn, key = 'checkbox'):
+            return is_bool_like(value)
         if self.cell_equal_to(datacn, value):
             return False
-        if (datacn in self.cell_options and 
-            'dropdown' in self.cell_options[datacn] and 
-            self.cell_options[datacn]['dropdown']['validate_input'] and 
-            value not in self.cell_options[datacn]['dropdown']['values']):
+        kwargs = self.get_cell_kwargs(datacn, key = 'dropdown')
+        if (kwargs and kwargs['validate_input'] and 
+            value not in kwargs['values']):
             return False
         return True
     
     def cell_equal_to(self, datacn, value):
         self.fix_header(datacn)
         if isinstance(self.MT._headers, list):
             return self.MT._headers[datacn] == value
         elif isinstance(self.MT._headers, int):
             return self.MT.cell_equal_to(self.MT._headers, datacn, value)
             
-    def get_cell_data(self, datacn, get_displayed = False, redirect_int = False):
-        if get_displayed and datacn in self.cell_options:
-            if 'dropdown' in self.cell_options[datacn] and self.cell_options[datacn]['dropdown']['text'] is not None:
-                return self.cell_options[datacn]['dropdown']['text']
-            if 'checkbox' in self.cell_options[datacn]:
-                return self.cell_options[datacn]['checkbox']['text']
-        if redirect_int and isinstance(self.MT._headers, int):
+    def get_cell_data(self, datacn, get_displayed = False, none_to_empty_str = False, redirect_int = False):
+        if get_displayed:
+            return self.get_valid_cell_data_as_str(datacn, fix = False)
+        if redirect_int and isinstance(self.MT._headers, int): # internal use
             return self.MT.get_cell_data(self.MT._headers, datacn, none_to_empty_str = True)
-        if isinstance(self.MT._headers, int) or not self.MT._headers or datacn >= len(self.MT._headers) or not self.MT._headers[datacn]:
-            if get_displayed and self.show_default_header_for_empty:
-                return get_n2a(datacn, self.default_header)
-            else:
-                return ""
-        return "" if self.MT._headers[datacn] is None and get_displayed else self.MT._headers[datacn]
+        if (isinstance(self.MT._headers, int) or
+            not self.MT._headers or 
+            datacn >= len(self.MT._headers) or 
+            (self.MT._headers[datacn] is None and none_to_empty_str)):
+            return ""
+        return self.MT._headers[datacn]
             
     def get_valid_cell_data_as_str(self, datacn, fix = True) -> str:
-        if datacn in self.cell_options:
-            if 'dropdown' in self.cell_options[datacn] and self.cell_options[datacn]['dropdown']['text'] is not None:
-                return f"{self.cell_options[datacn]['dropdown']['text']}"
-            if 'checkbox' in self.cell_options[datacn]:
-                return f"{self.cell_options[datacn]['checkbox']['text']}"
+        kwargs = self.get_cell_kwargs(datacn, key = 'dropdown')
+        if kwargs and kwargs['text'] is not None:
+            return f"{kwargs['text']}"
+        kwargs = self.get_cell_kwargs(datacn, key = 'checkbox')
+        if kwargs:
+            return f"{kwargs['text']}"
         if isinstance(self.MT._headers, int):
             return self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True)
         if fix:
             self.fix_header(datacn)
         try:
             return "" if self.MT._headers[datacn] is None else f"{self.MT._headers[datacn]}"
         except:
             return ""
-            
-    def fix_header(self, datacn = None):
+        
+    def get_value_for_empty_cell(self, datacn, c_ops = True):
+        if self.get_cell_kwargs(datacn, key = 'checkbox', cell = c_ops):
+            return False
+        kwargs = self.get_cell_kwargs(datacn, key = 'dropdown', cell = c_ops)
+        if kwargs and kwargs['validate_input'] and kwargs['values']:
+            return kwargs['values'][0]
+        return ""
+    
+    def get_empty_header_seq(self, end, start = 0, c_ops = True):
+        return [self.get_value_for_empty_cell(datacn, c_ops = c_ops) for datacn in range(start, end)]
+
+    def fix_header(self, datacn = None, fix_values = tuple()):
         if isinstance(self.MT._headers, int):
             return
         if isinstance(self.MT._headers, float):
             self.MT._headers = int(self.MT._headers)
             return
         if not isinstance(self.MT._headers, list):
             try:
                 self.MT._headers = list(self.MT._headers)
             except:
                 self.MT._headers = []
         if isinstance(datacn, int) and datacn >= len(self.MT._headers):
-            self.MT._headers.extend(list(repeat("", datacn - len(self.MT._headers) + 1)))
+            self.MT._headers.extend(self.get_empty_header_seq(end = datacn + 1, start = len(self.MT._headers)))
+        if fix_values:
+            for cn, v in enumerate(islice(self.MT._headers, fix_values[0], fix_values[1])):
+                if not self.input_valid_for_cell(cn, v):
+                    self.MT._headers[cn] = self.get_value_for_empty_cell(cn)
     
     # displayed indexes
     def set_col_width_run_binding(self, c, width = None, only_set_if_too_small = True):
         old_width = self.MT.col_positions[c + 1] - self.MT.col_positions[c]
         new_width = self.set_col_width(c, width = width, only_set_if_too_small = only_set_if_too_small)
         if self.column_width_resize_func is not None and old_width != new_width:
             self.column_width_resize_func(ResizeEvent("column_width_resize", c, old_width, new_width))
 
     #internal event use
-    def _click_checkbox(self, c, datacn = None, undo = True, redraw = True):
+    def click_checkbox(self, c, datacn = None, undo = True, redraw = True):
         if datacn is None:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-        if self.cell_options[datacn]['checkbox']['state'] == "normal":
+        kwargs = self.get_cell_kwargs(datacn, key = 'checkbox')
+        if kwargs['state'] == "normal":
             if isinstance(self.MT._headers, list):
                 value = not self.MT._headers[datacn] if type(self.MT._headers[datacn]) == bool else False
             elif isinstance(self.MT._headers, int):
                 value = not self.MT.data[self.MT._headers][datacn] if type(self.MT.data[self.MT._headers][datacn]) == bool else False
             else:
                 value = False
             self.set_cell_data_undo(c,
                                     datacn = datacn, 
                                     value = value, 
                                     cell_resize = False)
-            if self.cell_options[datacn]['checkbox']['check_function'] is not None:
-                self.cell_options[datacn]['checkbox']['check_function']((0,
-                                                                         c, 
-                                                                         "HeaderCheckboxClicked", 
-                                                                         self.MT._headers[datacn] if isinstance(self.MT._headers, list) else self.MT.get_cell_data(self.MT._headers, datacn)))
+            if kwargs['check_function'] is not None:
+                kwargs['check_function']((0,
+                                          c, 
+                                          "HeaderCheckboxClicked", 
+                                          self.MT._headers[datacn] if isinstance(self.MT._headers, list) else self.MT.get_cell_data(self.MT._headers, datacn)))
             if self.extra_end_edit_cell_func is not None:
                 self.extra_end_edit_cell_func(EditHeaderEvent(c, 
                                                               "Return",
                                                               self.MT._headers[datacn] if isinstance(self.MT._headers, list) else self.MT.get_cell_data(self.MT._headers, datacn), 
                                                               "end_edit_header"))
         if redraw:
             self.MT.refresh()
-
-    def create_checkbox(self, datacn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
+            
+    def checkbox_header(self, **kwargs):
+        self.destroy_opened_dropdown_window()
+        if 'dropdown' in self.options or 'checkbox' in self.options:
+            self.delete_options_dropdown_and_checkbox()
+        if 'checkbox' not in self.options:
+            self.options['checkbox'] = {}
+        self.options['checkbox'] = get_checkbox_dict(**kwargs)
+        total_cols = self.MT.total_data_cols()
+        if isinstance(self.MT._headers, int):
+            for datacn in total_cols:
+                self.MT.set_cell_data(datarn = self.MT._headers, datacn = datacn, value = kwargs['checked'])
+        else:
+            for datacn in total_cols:
+                self.set_cell_data(datacn = datacn, value = kwargs['checked'])
+                
+    def dropdown_header(self, **kwargs):
+        self.destroy_opened_dropdown_window()
+        if 'dropdown' in self.options or 'checkbox' in self.options:
+            self.delete_options_dropdown_and_checkbox()
+        if 'dropdown' not in self.options:
+            self.options['dropdown'] = {}
+        self.options['dropdown'] = get_dropdown_dict(**kwargs)
+        total_cols = self.MT.total_data_cols()
+        value = kwargs['set_value'] if kwargs['set_value'] is not None else kwargs['values'][0] if kwargs['values'] else ""
+        if isinstance(self.MT._headers, int):
+            for datacn in total_cols:
+                self.MT.set_cell_data(datarn = self.MT._headers, datacn = datacn, value = value)
+        else:
+            for datacn in total_cols:
+                self.set_cell_data(datacn = datacn, value = value)
+            
+    def create_checkbox(self, datacn = 0, **kwargs):
         if datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 
                                             'checkbox' in self.cell_options[datacn]):
-            self.delete_dropdown_and_checkbox(datacn)
+            self.delete_cell_options_dropdown_and_checkbox(datacn)
         if datacn not in self.cell_options:
             self.cell_options[datacn] = {}
-        self.cell_options[datacn]['checkbox'] = {'check_function': check_function,
-                                                 'state': state,
-                                                 'text': text}
-        self.set_cell_data(datacn = datacn, value = checked)
-        if redraw:
-            self.MT.refresh()
+        self.cell_options[datacn]['checkbox'] = get_checkbox_dict(**kwargs)
+        self.set_cell_data(datacn = datacn, value = kwargs['checked'])
 
-    def create_dropdown(self, 
-                        datacn = 0, 
-                        values = [], set_value = None, 
-                        state = "normal", redraw = True, 
-                        selection_function = None, modified_function = None,
-                        search_function = dropdown_search_function, validate_input = True, text = None):
+    def create_dropdown(self, datacn = 0, **kwargs):
         if datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 
                                             'checkbox' in self.cell_options[datacn]):
-            self.delete_dropdown_and_checkbox(datacn)
+            self.delete_cell_options_dropdown_and_checkbox(datacn)
         if datacn not in self.cell_options:
             self.cell_options[datacn] = {}
-        self.cell_options[datacn]['dropdown'] = {'values': values,
-                                                 'window': "no dropdown open",
-                                                 'canvas_id': "no dropdown open",
-                                                 'select_function': selection_function,
-                                                 'modified_function': modified_function,
-                                                 'search_function': search_function,
-                                                 'validate_input': validate_input,
-                                                 'text': text,
-                                                 'state': state}
+        self.cell_options[datacn]['dropdown'] = get_dropdown_dict(**kwargs)
         self.set_cell_data(datacn = datacn, 
-                           value = set_value if set_value is not None else values[0] if values else "")
-        if redraw:
-            self.MT.refresh()
+                           value = kwargs['set_value'] if kwargs['set_value'] is not None else kwargs['values'][0] if kwargs['values'] else "")
 
     def get_dropdown_height_anchor(self, datacn, text_editor_h = None):
         win_h = 5
-        for i, v in enumerate(self.cell_options[datacn]['dropdown']['values']):
+        for i, v in enumerate(self.get_cell_kwargs(datacn, key = 'dropdown')['values']):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
-                win_h += self.MT.hdr_fl_ins + (v_numlines * self.MT.hdr_xtra_lines_increment) + 5 # end of cell
+                win_h += self.MT.header_fl_ins + (v_numlines * self.MT.header_xtra_lines_increment) + 5 # end of cell
             else:
-                win_h += self.MT.hdr_min_rh
+                win_h += self.MT.min_header_height
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
         space_bot = self.MT.get_space_bot(0, text_editor_h)
         win_h2 = int(win_h)
         if win_h > space_bot:
             win_h = space_bot - 1
-        if win_h < self.MT.hdr_txt_h + 5:
-            win_h = self.MT.hdr_txt_h + 5
+        if win_h < self.MT.header_txt_h + 5:
+            win_h = self.MT.header_txt_h + 5
         elif win_h > win_h2:
             win_h = win_h2
         return win_h, "nw"
 
-    def set_current_height_to_text(self, text, datacn):
-        x = self.MT.txt_measure_canvas.create_text(0,
-                                                   0,
-                                                   text = self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True) if isinstance(self.MT._headers, int) else text,
-                                                   font = self.MT._hdr_font)
-        b = self.MT.txt_measure_canvas.bbox(x)
-        self.MT.txt_measure_canvas.delete(x)
-        new_height = b[3] - b[1] + 5
-        space_bot = self.MT.get_space_bot(0)
-        if new_height > space_bot:
-            new_height = space_bot
-        self.set_height(new_height, set_TL = True)
-
     def open_dropdown_window(self, c, datacn = None, event = None):
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window()
         if datacn is None:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-        if self.cell_options[datacn]['dropdown']['state'] == "normal":
-            if not self.edit_cell_(c = c, dropdown = True, event = event):
+        kwargs = self.get_cell_kwargs(datacn, key = 'dropdown')
+        if kwargs['state'] == "normal":
+            if not self.open_text_editor(event = event, c = c, dropdown = True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(datacn)
         window = self.MT.parentframe.dropdown_class(self.MT.winfo_toplevel(),
                                                     0,
                                                     c,
                                                     width = self.MT.col_positions[c + 1] - self.MT.col_positions[c] + 1,
                                                     height = win_h,
-                                                    font = self.MT._hdr_font,
+                                                    font = self.MT.header_font,
                                                     colors = {'bg': self.MT.popup_menu_bg, 
                                                               'fg': self.MT.popup_menu_fg, 
                                                               'highlight_bg': self.MT.popup_menu_highlight_bg,
                                                               'highlight_fg': self.MT.popup_menu_highlight_fg},
                                                     outline_color = self.MT.popup_menu_fg,
-                                                    values = self.cell_options[datacn]['dropdown']['values'],
+                                                    values = kwargs['values'],
                                                     close_dropdown_window = self.close_dropdown_window,
-                                                    search_function = self.cell_options[datacn]['dropdown']['search_function'],
+                                                    search_function = kwargs['search_function'],
                                                     arrowkey_RIGHT = self.MT.arrowkey_RIGHT,
                                                     arrowkey_LEFT = self.MT.arrowkey_LEFT,
                                                     align = "w",
                                                     single_index = "c")
         ypos = self.current_height - 1
-        self.cell_options[datacn]['dropdown']['canvas_id'] = self.create_window((self.MT.col_positions[c], ypos),
-                                                                                window = window,
-                                                                                anchor = anchor)
-        if self.cell_options[datacn]['dropdown']['state'] == "normal":
+        kwargs['canvas_id'] = self.create_window((self.MT.col_positions[c], ypos),
+                                                 window = window,
+                                                 anchor = anchor)
+        if kwargs['state'] == "normal":
             self.text_editor.textedit.bind("<<TextModified>>", 
                                            lambda x: window.search_and_see(DropDownModifiedEvent("HeaderComboboxModified", 0, c, self.text_editor.get())))
-            if self.cell_options[datacn]['dropdown']['modified_function'] is not None:
-                window.modified_function = self.cell_options[datacn]['dropdown']['modified_function']
+            if kwargs['modified_function'] is not None:
+                window.modified_function = kwargs['modified_function']
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
                 self.after(2, self.text_editor.scroll_to_bottom())
             except:
                 return
             redraw = False
         else:
             window.bind("<FocusOut>", lambda x: self.close_dropdown_window(c))
             self.update_idletasks()
             window.focus_set()
             redraw = True
         self.existing_dropdown_window = window
-        self.cell_options[datacn]['dropdown']['window'] = window
-        self.existing_dropdown_canvas_id = self.cell_options[datacn]['dropdown']['canvas_id']
+        kwargs['window'] = window
+        self.existing_dropdown_canvas_id = kwargs['canvas_id']
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False, redraw_table = False)
 
     def close_dropdown_window(self, c = None, selection = None, redraw = True):
         if c is not None and selection is not None:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            if self.cell_options[datacn]['dropdown']['select_function'] is not None: # user has specified a selection function
-                self.cell_options[datacn]['dropdown']['select_function'](EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
+            kwargs = self.get_cell_kwargs(datacn, key = 'dropdown')
+            if kwargs['select_function'] is not None: # user has specified a selection function
+                kwargs['select_function'](EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
             if self.extra_end_edit_cell_func is None:
                 self.set_cell_data_undo(c, datacn = datacn, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
                 if validation is not None:
                     selection = validation
                 self.set_cell_data_undo(c, datacn = datacn, value = selection, redraw = not redraw)
@@ -1739,28 +1850,49 @@
         except:
             pass
         self.existing_dropdown_canvas_id = None
         try:
             self.existing_dropdown_window.destroy()
         except:
             pass
-        if datacn_ in self.cell_options and 'dropdown' in self.cell_options[datacn_]:
-            self.cell_options[datacn_]['dropdown']['canvas_id'] = "no dropdown open"
-            self.cell_options[datacn_]['dropdown']['window'] = "no dropdown open"
+        kwargs = self.get_cell_kwargs(datacn_, key = 'dropdown')
+        if kwargs:
+            kwargs['canvas_id'] = "no dropdown open"
+            kwargs['window'] = "no dropdown open"
             try:
-                self.delete(self.cell_options[datacn_]['dropdown']['canvas_id'])
+                self.delete(kwargs['canvas_id'])
             except:
                 pass
         self.existing_dropdown_window = None
+        
+    def get_cell_kwargs(self, datacn, key = 'dropdown', cell = True, entire = True):
+        if cell and datacn in self.cell_options and key in self.cell_options[datacn]:
+            return self.cell_options[datacn][key]
+        if entire and key in self.options:
+            return self.options[key]
+        return {}
+        
+    def delete_options_dropdown(self):
+        self.destroy_opened_dropdown_window()
+        if 'dropdown' in self.options:
+            del self.options['dropdown']
+        
+    def delete_options_checkbox(self):
+        if 'checkbox' in self.options:
+            del self.options['checkbox']
+            
+    def delete_options_dropdown_and_checkbox(self):
+        self.delete_options_dropdown()
+        self.delete_options_checkbox()
 
-    def delete_dropdown(self, datacn):
+    def delete_cell_options_dropdown(self, datacn):
         self.destroy_opened_dropdown_window(datacn = datacn)
         if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
             del self.cell_options[datacn]['dropdown']
 
-    def delete_checkbox(self, datacn):
+    def delete_cell_options_checkbox(self, datacn):
         if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
             del self.cell_options[datacn]['checkbox']
 
-    def delete_dropdown_and_checkbox(self, datacn):
-        self.delete_dropdown(datacn)
-        self.delete_checkbox(datacn)
+    def delete_cell_options_dropdown_and_checkbox(self, datacn):
+        self.delete_cell_options_dropdown(datacn)
+        self.delete_cell_options_checkbox(datacn)
```

### Comparing `tksheet-6.0.2/tksheet/_tksheet_formatters.py` & `tksheet-6.0.3/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.2/tksheet/_tksheet_main_table.py` & `tksheet-6.0.3/tksheet/_tksheet_main_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.hidd_resize_lines = {}
         self.hidd_dropdown = {}
         self.hidd_checkbox = {}
 
         self.cell_options = {}
         self.col_options = {}
         self.row_options = {}
-        self.sheet_options = {}
+        self.options = {}
 
         """
         cell options dict looks like:
         {(row int, column int): {'dropdown': {'values': values,
                                               'window': "no dropdown open",
                                               'select_function': selection_function,
                                               'keypress_function': keypress_function,
@@ -103,16 +103,16 @@
         self.selected_rows_to_end_of_window = kwargs['selected_rows_to_end_of_window']
         self.horizontal_grid_to_end_of_window = kwargs['horizontal_grid_to_end_of_window']
         self.vertical_grid_to_end_of_window = kwargs['vertical_grid_to_end_of_window']
         self.empty_horizontal = kwargs['empty_horizontal']
         self.empty_vertical = kwargs['empty_vertical']
         self.show_vertical_grid = kwargs['show_vertical_grid']
         self.show_horizontal_grid = kwargs['show_horizontal_grid']
-        self.min_rh = 0
-        self.hdr_min_rh = 0
+        self.min_row_height = 0
+        self.min_header_height = 0
         self.being_drawn_rect = None
         self.extra_motion_func = None
         self.extra_b1_press_func = None
         self.extra_b1_motion_func = None
         self.extra_b1_release_func = None
         self.extra_double_b1_func = None
         self.extra_rc_func = None
@@ -149,27 +149,29 @@
 
         self.text_editor_user_bound_keys = {}
 
         self.selection_binding_func = None
         self.deselection_binding_func = None
         self.drag_selection_binding_func = None
         self.shift_selection_binding_func = None
+        self.ctrl_selection_binding_func = None
         self.select_all_binding_func = None
 
         self.single_selection_enabled = False
         self.toggle_selection_enabled = False # with this mode every left click adds the cell to selected cells
         self.show_dropdown_borders = kwargs['show_dropdown_borders']
         self.drag_selection_enabled = False
         self.select_all_enabled = False
         self.undo_enabled = False
         self.cut_enabled = False
         self.copy_enabled = False
         self.paste_enabled = False
         self.delete_key_enabled = False
         self.rc_select_enabled = False
+        self.ctrl_select_enabled = False
         self.rc_delete_column_enabled = False
         self.rc_insert_column_enabled = False
         self.rc_delete_row_enabled = False
         self.rc_insert_row_enabled = False
         self.rc_popup_menus_enabled = False
         self.edit_cell_enabled = False
         self.text_editor_loc = None
@@ -184,38 +186,49 @@
         self.RI = kwargs['row_index_canvas']
         self.RI.MT = self
         self.RI.CH = kwargs['column_headers_canvas']
         self.TL = None                # is set from within TopLeftRectangle() __init__
         self.all_columns_displayed = True
         self.all_rows_displayed = True
         self.align = kwargs['align']
-        self._font = kwargs['font']
-        self.fnt_fam = kwargs['font'][0]
-        self.fnt_sze = kwargs['font'][1]
-        self.fnt_wgt = kwargs['font'][2]
-        self._index_font = kwargs['index_font']
-        self.index_fnt_fam = kwargs['index_font'][0]
-        self.index_fnt_sze = kwargs['index_font'][1]
-        self.index_fnt_wgt = kwargs['index_font'][2]
-        self._hdr_font = kwargs['header_font']
-        self.hdr_fnt_fam = kwargs['header_font'][0]
-        self.hdr_fnt_sze = kwargs['header_font'][1]
-        self.hdr_fnt_wgt = kwargs['header_font'][2]
+        self.table_font = kwargs['font']
+        self.font_fam = kwargs['font'][0]
+        self.font_sze = kwargs['font'][1]
+        self.font_wgt = kwargs['font'][2]
+        self.index_font = kwargs['index_font']
+        self.index_font_fam = kwargs['index_font'][0]
+        self.index_font_sze = kwargs['index_font'][1]
+        self.index_font_wgt = kwargs['index_font'][2]
+        self.header_font = kwargs['header_font']
+        self.header_font_fam = kwargs['header_font'][0]
+        self.header_font_sze = kwargs['header_font'][1]
+        self.header_font_wgt = kwargs['header_font'][2]
         self.txt_measure_canvas = tk.Canvas(self)
-        self.txt_measure_canvas_text = self.txt_measure_canvas.create_text(0, 0, text = "", font = self._font)
+        self.txt_measure_canvas_text = self.txt_measure_canvas.create_text(0, 0, text = "", font = self.table_font)
         self.text_editor = None
         self.text_editor_id = None
-        self.default_cw = kwargs['column_width']
-        self.default_rh = (kwargs['row_height'] if isinstance(kwargs['row_height'], str) else "pixels",
-                           kwargs['row_height'] if isinstance(kwargs['row_height'], int) else self.GetLinesHeight(int(kwargs['row_height'])))
-        self.default_hh = (kwargs['header_height'] if isinstance(kwargs['header_height'], str) else "pixels",
-                           kwargs['header_height'] if isinstance(kwargs['header_height'], int) else self.GetHdrLinesHeight(int(kwargs['header_height'])))
-        self.set_fnt_help()
-        self.set_hdr_fnt_help()
-        self.set_index_fnt_help()
+        
+        self.max_row_height = float(kwargs['max_row_height'])
+        self.max_index_width = float(kwargs['max_index_width'])
+        self.max_column_width = float(kwargs['max_column_width'])
+        self.max_header_height = float(kwargs['max_header_height'])
+        if kwargs['row_index_width'] is None:
+            self.RI.set_width(70)
+            self.default_index_width = 70
+        else:
+            self.RI.set_width(kwargs['row_index_width'])
+            self.default_index_width = kwargs['row_index_width']
+        self.default_header_height = (kwargs['header_height'] if isinstance(kwargs['header_height'], str) else "pixels",
+                                      kwargs['header_height'] if isinstance(kwargs['header_height'], int) else self.get_lines_cell_height(int(kwargs['header_height']), font = self.header_font))
+        self.default_column_width = kwargs['column_width']
+        self.default_row_height = (kwargs['row_height'] if isinstance(kwargs['row_height'], str) else "pixels",
+                                   kwargs['row_height'] if isinstance(kwargs['row_height'], int) else self.get_lines_cell_height(int(kwargs['row_height'])))
+        self.set_font_help()
+        self.set_header_font_help()
+        self.set_index_font_help()
         self.data = kwargs['data_reference']
         if isinstance(self.data, (list, tuple)):
             self.data = kwargs['data_reference']
         else:
             self.data = []
         if not self.data:
             if isinstance(kwargs['total_rows'], int) and isinstance(kwargs['total_cols'], int) and kwargs['total_rows'] > 0 and kwargs['total_cols'] > 0:
@@ -293,15 +306,24 @@
                     canvas.bind("<Shift-Button-5>", self.shift_mousewheel)
             self.bind("<Shift-MouseWheel>", self.shift_mousewheel)
             self.bind("<Shift-ButtonPress-1>", self.shift_b1_press)
             self.CH.bind("<Shift-ButtonPress-1>", self.CH.shift_b1_press)
             self.RI.bind("<Shift-ButtonPress-1>", self.RI.shift_b1_press)
             self.CH.bind("<Shift-MouseWheel>", self.shift_mousewheel)
             self.RI.bind("<MouseWheel>", self.mousewheel)
-            self.bind(get_rc_binding(), self.rc)
+            self.bind(rc_binding, self.rc)
+            self.bind(f"<{ctrl_key}-ButtonPress-1>", self.ctrl_b1_press)
+            self.CH.bind(f"<{ctrl_key}-ButtonPress-1>", self.CH.ctrl_b1_press)
+            self.RI.bind(f"<{ctrl_key}-ButtonPress-1>", self.RI.ctrl_b1_press)
+            self.bind(f"<{ctrl_key}-Shift-ButtonPress-1>", self.ctrl_shift_b1_press)
+            self.CH.bind(f"<{ctrl_key}-Shift-ButtonPress-1>", self.CH.ctrl_shift_b1_press)
+            self.RI.bind(f"<{ctrl_key}-Shift-ButtonPress-1>", self.RI.ctrl_shift_b1_press)
+            self.bind(f"<{ctrl_key}-B1-Motion>", self.ctrl_b1_motion)
+            self.CH.bind(f"<{ctrl_key}-B1-Motion>", self.CH.ctrl_b1_motion)
+            self.RI.bind(f"<{ctrl_key}-B1-Motion>", self.RI.ctrl_b1_motion)
         else:
             self.unbind("<Configure>")
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
@@ -315,27 +337,38 @@
                     canvas.unbind("<Shift-Button-5>")
             self.unbind("<Shift-ButtonPress-1>")
             self.CH.unbind("<Shift-ButtonPress-1>")
             self.RI.unbind("<Shift-ButtonPress-1>")
             self.unbind("<Shift-MouseWheel>")
             self.CH.unbind("<Shift-MouseWheel>")
             self.RI.unbind("<MouseWheel>")
-            self.unbind(get_rc_binding())
-
-    def show_ctrl_outline(self, canvas = "table", start_cell = (0, 0), end_cell = (0, 0)):
-        self.create_ctrl_outline(self.col_positions[start_cell[0]] + 2,
-                                 self.row_positions[start_cell[1]] + 2,
-                                 self.col_positions[end_cell[0]] - 2,
-                                 self.row_positions[end_cell[1]] - 2,
+            self.unbind(rc_binding)
+            self.unbind(f"<{ctrl_key}-ButtonPress-1>")
+            self.CH.unbind(f"<{ctrl_key}-ButtonPress-1>")
+            self.RI.unbind(f"<{ctrl_key}-ButtonPress-1>")
+            self.unbind(f"<{ctrl_key}-Shift-ButtonPress-1>")
+            self.CH.unbind(f"<{ctrl_key}-Shift-ButtonPress-1>")
+            self.RI.unbind(f"<{ctrl_key}-Shift-ButtonPress-1>")
+            self.unbind(f"<{ctrl_key}-B1-Motion>")
+            self.CH.unbind(f"<{ctrl_key}-B1-Motion>")
+            self.RI.unbind(f"<{ctrl_key}-B1-Motion>")
+
+    def show_ctrl_outline(self, canvas = "table", start_cell = (0, 0), end_cell = (0, 0), dash = (20, 20), 
+                                outline = None, delete_on_timer = True):
+        self.create_ctrl_outline(self.col_positions[start_cell[0]] + 1,
+                                 self.row_positions[start_cell[1]] + 1,
+                                 self.col_positions[end_cell[0]] - 1,
+                                 self.row_positions[end_cell[1]] - 1,
                                  fill = "",
-                                 dash = (10, 15),
-                                 width = 3 if end_cell[0] - start_cell[0] == 1 and end_cell[1] - start_cell[1] == 1 else 2,
-                                 outline = self.table_selected_cells_border_fg,
+                                 dash = dash,
+                                 width = 3,
+                                 outline = self.RI.resizing_line_fg if outline is None else outline,
                                  tag = "ctrl")
-        self.after(1500, self.delete_ctrl_outlines)
+        if delete_on_timer:
+            self.after(1500, self.delete_ctrl_outlines)
 
     def create_ctrl_outline(self, x1, y1, x2, y2, fill, dash, width, outline, tag):
         if self.hidd_ctrl_outline:
             t, sh = self.hidd_ctrl_outline.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
                 self.itemconfig(t, fill = fill, dash = dash, width = width, outline = outline, tag = tag)
@@ -364,17 +397,18 @@
                     boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "cells"
                 elif alltags[0] == "ColSelectFill":
                     boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "columns"
             maxrows = 0
             for r1, c1, r2, c2 in boxes:
                 if r2 - r1 > maxrows:
                     maxrows = r2 - r1
-            for r1, c1, r2, c2 in tuple(boxes):
-                if r2 - r1 < maxrows:
-                    del boxes[(r1, c1, r2, c2)]
+            curr_box = self.find_last_selected_box_with_current_from_boxes(currently_selected, boxes)
+            for box in tuple(boxes):
+                if box[2] - box[0] < maxrows and box != curr_box:
+                    del boxes[box]
             return boxes, maxrows
         else:
             for item in self.find_withtag("RowSelectFill"):
                 boxes[tuple(int(e) for e in self.gettags(item)[1].split("_") if e)] = "rows"
             return boxes
 
     def ctrl_c(self, event = None):
@@ -495,30 +529,33 @@
                         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                         if self.input_valid_for_cell(datarn, datacn, ""):
                             if self.undo_enabled:
                                 undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
                             self.set_cell_data(datarn, datacn, "")
                             changes += 1
         if changes and self.undo_enabled:
-            self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, tuple(boxes.items()), currently_selected))))
+            self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, boxes, currently_selected))))
         self.clipboard_clear()
         self.clipboard_append(s.getvalue())
         self.update_idletasks()
         self.refresh()
         for r1, c1, r2, c2 in boxes:
             self.show_ctrl_outline(canvas = "table", start_cell = (c1, r1), end_cell = (c2, r2))
         if self.extra_end_ctrl_x_func is not None:
             self.extra_end_ctrl_x_func(CtrlKeyEvent("end_ctrl_x", boxes, currently_selected, rows))
-        self.event_generate("<<SheetDataChangeEvent>>")
+        self.parentframe.emit_modified_event()
 
     def find_last_selected_box_with_current(self, currently_selected):
         if currently_selected.type_ in ("cell", "column"):
             boxes, maxrows = self.get_ctrl_x_c_boxes()
         else:
             boxes = self.get_ctrl_x_c_boxes()
+        return self.find_last_selected_box_with_current_from_boxes(currently_selected, boxes)
+        
+    def find_last_selected_box_with_current_from_boxes(self, currently_selected, boxes):
         for (r1, c1, r2, c2), type_ in boxes.items():
             if (type_[:2] == currently_selected.type_[:2] and
                 currently_selected.row >= r1 and
                 currently_selected.row <= r2 and
                 currently_selected.column >= c1 and
                 currently_selected.column <= c2):
                 if (self.last_selected and self.last_selected == (r1, c1, r2, c2, type_)) or not self.last_selected:
@@ -624,106 +661,97 @@
                     changes += 1
         if self.expand_sheet_if_paste_too_big and self.undo_enabled:
             self.equalize_data_row_lengths()
         self.deselect("all")
         if changes and self.undo_enabled:
             self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells_paste",
                                                                  undo_storage,
-                                                                 (((selected_r, selected_c, selected_r + numrows, selected_c + numcols), "cells"), ), # boxes
+                                                                 {(selected_r, selected_c, selected_r + numrows, selected_c + numcols): "cells"}, # boxes
                                                                  currently_selected,
                                                                  added_rows_cols))))
         self.create_selected(selected_r, selected_c, selected_r + numrows, selected_c + numcols, "cells")
         self.create_current(selected_r, selected_c, type_ = "cell", inside = True if numrows > 1 or numcols > 1 else False)
         self.see(r = selected_r, c = selected_c, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
         self.refresh()
         if self.extra_end_ctrl_v_func is not None:
             self.extra_end_ctrl_v_func(PasteEvent("end_ctrl_v", currently_selected, rows))
-        self.event_generate("<<SheetDataChangeEvent>>")
+        self.parentframe.emit_modified_event()
 
     def delete_key(self, event = None):
-        if self.anything_selected():
-            currently_selected = self.currently_selected()
-            undo_storage = {}
-            boxes = {}
-            for item in chain(self.find_withtag("CellSelectFill"), self.find_withtag("RowSelectFill"), self.find_withtag("ColSelectFill"), self.find_withtag("Current_Outside")):
-                alltags = self.gettags(item)
-                box = tuple(int(e) for e in alltags[1].split("_") if e)
-                if alltags[0] in ("CellSelectFill", "Current_Outside"):
-                    boxes[box] = "cells"
-                elif alltags[0] == "ColSelectFill":
-                    boxes[box] = "columns"
-                elif alltags[0] == "RowSelectFill":
-                    boxes[box] = "rows"
-            if self.extra_begin_delete_key_func is not None:
-                try:
-                    self.extra_begin_delete_key_func(CtrlKeyEvent("begin_delete_key", boxes, currently_selected, tuple()))
-                except:
-                    return
-            changes = 0
-            for r1, c1, r2, c2 in boxes:
-                for r in range(r1, r2):
-                    datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-                    for c in range(c1, c2):
-                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                        if self.input_valid_for_cell(datarn, datacn, ""):
-                            if self.undo_enabled:
-                                undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
-                            self.set_cell_data(datarn, datacn, "")
-                            changes += 1
-            if self.extra_end_delete_key_func is not None:
-                self.extra_end_delete_key_func(CtrlKeyEvent("end_delete_key", boxes, currently_selected, undo_storage))
-            if changes and self.undo_enabled:
-                self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, tuple(boxes.items()), currently_selected))))
-            self.refresh()
-            self.event_generate("<<SheetDataChangeEvent>>")
+        if not self.anything_selected():
+            return
+        currently_selected = self.currently_selected()
+        undo_storage = {}
+        boxes = {}
+        for item in chain(self.find_withtag("CellSelectFill"), self.find_withtag("RowSelectFill"), self.find_withtag("ColSelectFill"), self.find_withtag("Current_Outside")):
+            alltags = self.gettags(item)
+            box = tuple(int(e) for e in alltags[1].split("_") if e)
+            if alltags[0] in ("CellSelectFill", "Current_Outside"):
+                boxes[box] = "cells"
+            elif alltags[0] == "ColSelectFill":
+                boxes[box] = "columns"
+            elif alltags[0] == "RowSelectFill":
+                boxes[box] = "rows"
+        if self.extra_begin_delete_key_func is not None:
+            try:
+                self.extra_begin_delete_key_func(CtrlKeyEvent("begin_delete_key", boxes, currently_selected, tuple()))
+            except:
+                return
+        changes = 0
+        for r1, c1, r2, c2 in boxes:
+            for r in range(r1, r2):
+                datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+                for c in range(c1, c2):
+                    datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                    if self.input_valid_for_cell(datarn, datacn, ""):
+                        if self.undo_enabled:
+                            undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
+                        self.set_cell_data(datarn, datacn, "")
+                        changes += 1
+        if self.extra_end_delete_key_func is not None:
+            self.extra_end_delete_key_func(CtrlKeyEvent("end_delete_key", boxes, currently_selected, undo_storage))
+        if changes and self.undo_enabled:
+            self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, boxes, currently_selected))))
+        self.refresh()
+        self.parentframe.emit_modified_event()
             
-    def move_columns_adjust_options_dict(self, col, to_move_min, num_cols, move_data = True, create_selections = True):
+    def move_columns_adjust_options_dict(self, col, to_move_min, num_cols, move_data = True, create_selections = True, index_type = "displayed"):
         c = int(col)
         to_move_max = to_move_min + num_cols
         to_del = to_move_max + num_cols
         orig_selected = list(range(to_move_min, to_move_min + num_cols))
-        self.deselect("all", redraw = False)
-        cws = [int(b - a) for a, b in zip(self.col_positions, islice(self.col_positions, 1, len(self.col_positions)))]
-        if to_move_min > c:
-            cws[c:c] = cws[to_move_min:to_move_max]
-            cws[to_move_max:to_del] = []
-        else:
-            cws[c + 1:c + 1] = cws[to_move_min:to_move_max]
-            cws[to_move_min:to_move_max] = []
-        self.col_positions = list(accumulate(chain([0], (width for width in cws))))
+        if index_type == "displayed":
+            self.deselect("all", redraw = False)
+            cws = [int(b - a) for a, b in zip(self.col_positions, islice(self.col_positions, 1, len(self.col_positions)))]
+            if to_move_min > c:
+                cws[c:c] = cws[to_move_min:to_move_max]
+                cws[to_move_max:to_del] = []
+            else:
+                cws[c + 1:c + 1] = cws[to_move_min:to_move_max]
+                cws[to_move_min:to_move_max] = []
+            self.col_positions = list(accumulate(chain([0], (width for width in cws))))
         if c + num_cols > len(self.col_positions):
             new_selected = tuple(range(len(self.col_positions) - 1 - num_cols, len(self.col_positions) - 1))
-            if create_selections:
+            if create_selections and index_type == "displayed":
                 self.create_selected(0, len(self.col_positions) - 1 - num_cols, len(self.row_positions) - 1, len(self.col_positions) - 1, "columns")
         else:
             if to_move_min > c:
                 new_selected = tuple(range(c, c + num_cols))
-                if create_selections:
+                if create_selections and index_type == "displayed":
                     self.create_selected(0, c, len(self.row_positions) - 1, c + num_cols, "columns")
             else:
                 new_selected = tuple(range(c + 1 - num_cols, c + 1))
-                if create_selections:
+                if create_selections and index_type == "displayed":
                     self.create_selected(0, c + 1 - num_cols, len(self.row_positions) - 1, c + 1, "columns")
-        if create_selections:
+        if create_selections and index_type == "displayed":
             self.create_current(0, int(new_selected[0]), type_ = "column", inside = True)
         newcolsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
-        if self.all_columns_displayed:
+        if self.all_columns_displayed or index_type != "displayed":
             dispset = {}
             if to_move_min > c:
-                if move_data:
-                    for rn in range(len(self.data)):
-                        if len(self.data[rn]) < to_move_max:
-                            self.data[rn].extend(list(repeat("", to_move_max - len(self.data[rn]) + 1)))
-                        self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
-                        self.data[rn][to_move_max:to_del] = []
-                    if isinstance(self._headers, list) and self._headers:
-                        if len(self._headers) < to_move_max:
-                            self._headers.extend(list(repeat("", to_move_max - len(self._headers) + 1)))
-                        self._headers[c:c] = self._headers[to_move_min:to_move_max]
-                        self._headers[to_move_max:to_del] = []
                 self.CH.cell_options = {
                     newcolsdct[k] if k in newcolsdct else
                     k + num_cols if k < to_move_min and k >= c else
                     k: v for k, v in self.CH.cell_options.items()
                 }
                 self.cell_options = {
                     (k[0], newcolsdct[k[1]]) if k[1] in newcolsdct else
@@ -731,27 +759,28 @@
                     k: v for k, v in self.cell_options.items()
                 }
                 self.col_options = {
                     newcolsdct[k] if k in newcolsdct else
                     k + num_cols if k < to_move_min and k >= c else
                     k: v for k, v in self.col_options.items()
                 }
-            else:
-                c += 1
                 if move_data:
                     for rn in range(len(self.data)):
-                        if len(self.data[rn]) < c - 1:
-                            self.data[rn].extend(list(repeat("", c - len(self.data[rn]))))
+                        if to_move_max >= len(self.data[rn]):
+                            self.fix_row_len(rn, to_move_max)
                         self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
-                        self.data[rn][to_move_min:to_move_max] = []
+                        self.data[rn][to_move_max:to_del] = []
+                    self.CH.fix_header(to_move_max)
                     if isinstance(self._headers, list) and self._headers:
-                        if len(self._headers) < c:
-                            self._headers.extend(list(repeat("", c - len(self._headers))))
                         self._headers[c:c] = self._headers[to_move_min:to_move_max]
-                        self._headers[to_move_min:to_move_max] = []
+                        self._headers[to_move_max:to_del] = []
+                if index_type != "displayed":
+                    self.displayed_columns = sorted(int(newcolsdct[k]) if k in newcolsdct else k + totalcols if k < to_move_min and k >= c else int(k) for k in self.displayed_columns)
+            else:
+                c += 1
                 self.CH.cell_options = {
                     newcolsdct[k] if k in newcolsdct else
                     k - num_cols if k < c and k > to_move_min else
                     k: v for k, v in self.CH.cell_options.items()
                 }
                 self.cell_options = {
                     (k[0], newcolsdct[k[1]]) if k[1] in newcolsdct else 
@@ -759,110 +788,115 @@
                     k: v for k, v in self.cell_options.items()
                 }
                 self.col_options = {
                     newcolsdct[k] if k in newcolsdct else
                     k - num_cols if k < c and k > to_move_min else
                     k: v for k, v in self.col_options.items()
                 }
+                if move_data:
+                    for rn in range(len(self.data)):
+                        if c >= len(self.data[rn]):
+                            self.fix_row_len(rn, c)
+                        self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
+                        self.data[rn][to_move_min:to_move_max] = []
+                    self.CH.fix_header(c)
+                    if isinstance(self._headers, list) and self._headers:
+                        self._headers[c:c] = self._headers[to_move_min:to_move_max]
+                        self._headers[to_move_min:to_move_max] = []
+                if index_type != "displayed":
+                    self.displayed_columns = sorted(int(newcolsdct[k]) if k in newcolsdct else k - totalcols if k < c and k > to_move_min else int(k) for k in self.displayed_columns)
         else:
             # moves data around, not displayed columns indexes
             # which remain sorted and the same after drop and drop
             if to_move_min > c:
-                dispset = {a: b for a, b in zip(self.displayed_columns, (self.displayed_columns[:c] +
+                dispset = {b: a for a, b in zip(self.displayed_columns, (self.displayed_columns[:c] +
                                                                          self.displayed_columns[to_move_min:to_move_min + num_cols] +
                                                                          self.displayed_columns[c:to_move_min] +
                                                                          self.displayed_columns[to_move_min + num_cols:]))}
             else:
-                dispset = {a: b for a, b in zip(self.displayed_columns, (self.displayed_columns[:to_move_min] +
+                dispset = {b: a for a, b in zip(self.displayed_columns, (self.displayed_columns[:to_move_min] +
                                                                          self.displayed_columns[to_move_min + num_cols:c + 1] +
                                                                          self.displayed_columns[to_move_min:to_move_min + num_cols] +
                                                                          self.displayed_columns[c + 1:]))}
             # has to pick up elements from all over the place in the original row
             # building an entirely new row is best due to permutations of hidden columns
+            self.CH.cell_options = {dispset[k] if k in dispset else k: v for k, v in self.CH.cell_options.items()}
+            self.cell_options = {(k[0], dispset[k[1]]) if k[1] in dispset else k: v for k, v in self.cell_options.items()}
+            self.col_options = {dispset[k] if k in dispset else k: v for k, v in self.col_options.items()}
+            dispset = {b: a for a, b in dispset.items()}
             if move_data:
-                max_idx = max(chain(dispset, dispset.values())) + 1
+                max_len = max(chain(dispset, dispset.values())) + 1
+                max_idx = max_len - 1
                 for rn in range(len(self.data)):
-                    if len(self.data[rn]) < max_idx:
-                        self.data[rn][:] = self.data[rn] + list(repeat("", max_idx - len(self.data[rn])))
+                    if max_len > len(self.data[rn]):
+                        self.fix_row_len(rn, max_idx)
                     new = []
                     idx = 0
                     done = set()
                     while len(new) < len(self.data[rn]):
                         if idx in dispset and idx not in done:
                             new.append(self.data[rn][dispset[idx]])
                             done.add(idx)
                         elif idx not in done:
                             new.append(self.data[rn][idx])
                             idx += 1
                         else:
                             idx += 1
                     self.data[rn] = new
+                self.CH.fix_header(max_idx)
                 if isinstance(self._headers, list) and self._headers:
-                    if len(self._headers) < max_idx:
-                        self._headers[:] = self._headers + list(repeat("", max_idx - len(self._headers)))
                     new = []
                     idx = 0
                     done = set()
                     while len(new) < len(self._headers):
                         if idx in dispset and idx not in done:
                             new.append(self._headers[dispset[idx]])
                             done.add(idx)
                         elif idx not in done:
                             new.append(self._headers[idx])
                             idx += 1
                         else:
                             idx += 1
                     self._headers = new
-            dispset = {b: a for a, b in dispset.items()}
-            self.CH.cell_options = {dispset[k] if k in dispset else k: v for k, v in self.CH.cell_options.items()}
-            self.cell_options = {(k[0], dispset[k[1]]) if k[1] in dispset else k: v for k, v in self.cell_options.items()}
-            self.col_options = {dispset[k] if k in dispset else k: v for k, v in self.col_options.items()}
-        return new_selected, dispset
+        return new_selected, {b: a for a, b in dispset.items()}
     
-    def move_rows_adjust_options_dict(self, row, to_move_min, num_rows, move_data = True, create_selections = True):
+    def move_rows_adjust_options_dict(self, row, to_move_min, num_rows, move_data = True, create_selections = True, index_type = "displayed"):
         r = int(row)
         to_move_max = to_move_min + num_rows
         to_del = to_move_max + num_rows
         orig_selected = list(range(to_move_min, to_move_min + num_rows))
-        self.deselect("all", redraw = False)
-        rhs = [int(b - a) for a, b in zip(self.row_positions, islice(self.row_positions, 1, len(self.row_positions)))]
-        if to_move_min > r:
-            rhs[r:r] = rhs[to_move_min:to_move_max]
-            rhs[to_move_max:to_del] = []
-        else:
-            rhs[r + 1:r + 1] = rhs[to_move_min:to_move_max]
-            rhs[to_move_min:to_move_max] = []
-        self.row_positions = list(accumulate(chain([0], (height for height in rhs))))       
+        if index_type == "displayed":
+            self.deselect("all", redraw = False)
+            rhs = [int(b - a) for a, b in zip(self.row_positions, islice(self.row_positions, 1, len(self.row_positions)))]
+            if to_move_min > r:
+                rhs[r:r] = rhs[to_move_min:to_move_max]
+                rhs[to_move_max:to_del] = []
+            else:
+                rhs[r + 1:r + 1] = rhs[to_move_min:to_move_max]
+                rhs[to_move_min:to_move_max] = []
+            self.row_positions = list(accumulate(chain([0], (height for height in rhs))))      
         if r + num_rows > len(self.row_positions):
             new_selected = tuple(range(len(self.row_positions) - 1 - num_rows, len(self.row_positions) - 1))
-            if create_selections:
+            if create_selections and index_type == "displayed":
                 self.create_selected(len(self.row_positions) - 1 - num_rows, 0, len(self.row_positions) - 1, len(self.col_positions) - 1, "rows")
         else:
             if to_move_min > r:
                 new_selected = tuple(range(r, r + num_rows))
-                if create_selections:
+                if create_selections and index_type == "displayed":
                     self.create_selected(r, 0, r + num_rows, len(self.col_positions) - 1, "rows")
             else:
                 new_selected = tuple(range(r + 1 - num_rows, r + 1))
-                if create_selections:
+                if create_selections and index_type == "displayed":
                     self.create_selected(r + 1 - num_rows, 0, r + 1, len(self.col_positions) - 1, "rows")
-        if create_selections:
+        if create_selections and index_type == "displayed":
             self.create_current(int(new_selected[0]), 0, type_ = "row", inside = True)
         newrowsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
-        if self.all_rows_displayed:
+        if self.all_rows_displayed or index_type != "displayed":
             dispset = {}
             if to_move_min > r:
-                if move_data:
-                    self.data[r:r] = self.data[to_move_min:to_move_max]
-                    self.data[to_move_max:to_del] = []
-                    if isinstance(self._row_index, list) and self._row_index:
-                        if len(self._row_index) < to_move_max:
-                            self._row_index.extend(list(repeat("", to_move_max - len(self._row_index) + 1)))
-                        self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
-                        self._row_index[to_move_max:to_del] = []
                 self.RI.cell_options = {
                     newrowsdct[k] if k in newrowsdct else
                     k + num_rows if k < to_move_min and k >= r else
                     k: v for k, v in self.RI.cell_options.items()
                 }
                 self.cell_options = {
                     (newrowsdct[k[0]], k[1]) if k[0] in newrowsdct else
@@ -870,24 +904,25 @@
                     k: v for k, v in self.cell_options.items()
                 }
                 self.row_options = {
                     newrowsdct[k] if k in newrowsdct else
                     k + num_rows if k < to_move_min and k >= r else
                     k: v for k, v in self.row_options.items()
                 }
-            else:
-                r += 1
                 if move_data:
                     self.data[r:r] = self.data[to_move_min:to_move_max]
-                    self.data[to_move_min:to_move_max] = []
+                    self.data[to_move_max:to_del] = []
+                    self.RI.fix_index(to_move_max)
                     if isinstance(self._row_index, list) and self._row_index:
-                        if len(self._row_index) < r:
-                            self._row_index.extend(list(repeat("", r - len(self._row_index))))
                         self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
-                        self._row_index[to_move_min:to_move_max] = []
+                        self._row_index[to_move_max:to_del] = []
+                if index_type != "displayed":
+                    self.displayed_rows = sorted(int(newrowsdct[k]) if k in newrowsdct else k + totalrows if k < to_move_min and k >= r else int(k) for k in self.displayed_rows)
+            else:
+                r += 1
                 self.RI.cell_options = {
                     newrowsdct[k] if k in newrowsdct else
                     k - num_rows if k < r and k > to_move_min else
                     k: v for k, v in self.RI.cell_options.items()
                 }
                 self.cell_options = {
                     (newrowsdct[k[0]], k[1]) if k[0] in newrowsdct else 
@@ -895,67 +930,75 @@
                     k: v for k, v in self.cell_options.items()
                 }
                 self.row_options = {
                     newrowsdct[k] if k in newrowsdct else
                     k - num_rows if k < r and k > to_move_min else
                     k: v for k, v in self.row_options.items()
                 }
+                if move_data:
+                    self.data[r:r] = self.data[to_move_min:to_move_max]
+                    self.data[to_move_min:to_move_max] = []
+                    self.RI.fix_index(r)
+                    if isinstance(self._row_index, list) and self._row_index:
+                        self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
+                        self._row_index[to_move_min:to_move_max] = []
+                if index_type != "displayed":
+                    self.displayed_rows = sorted(int(newrowsdct[k]) if k in newrowsdct else k - totalrows if k < r and k > to_move_min else int(k) for k in self.displayed_rows)
         else:
             # moves data around, not displayed rows indexes
             # which remain sorted and the same after drop and drop
             if to_move_min > r:
-                dispset = {a: b for a, b in zip(self.displayed_rows, (self.displayed_rows[:r] +
+                dispset = {b: a for a, b in zip(self.displayed_rows, (self.displayed_rows[:r] +
                                                                       self.displayed_rows[to_move_min:to_move_min + num_rows] +
                                                                       self.displayed_rows[r:to_move_min] +
                                                                       self.displayed_rows[to_move_min + num_rows:]))}
             else:
-                dispset = {a: b for a, b in zip(self.displayed_rows, (self.displayed_rows[:to_move_min] +
+                dispset = {b: a for a, b in zip(self.displayed_rows, (self.displayed_rows[:to_move_min] +
                                                                       self.displayed_rows[to_move_min + num_rows:r + 1] +
                                                                       self.displayed_rows[to_move_min:to_move_min + num_rows] +
                                                                       self.displayed_rows[r + 1:]))}
             # has to pick up rows from all over the place in the original sheet
             # building an entirely new sheet is best due to permutations of hidden rows
+            self.RI.cell_options = {dispset[k] if k in dispset else k: v for k, v in self.RI.cell_options.items()}
+            self.cell_options = {(dispset[k[0]], k[1]) if k[0] in dispset else k: v for k, v in self.cell_options.items()}
+            self.row_options = {dispset[k] if k in dispset else k: v for k, v in self.row_options.items()}
+            dispset = {b: a for a, b in dispset.items()}
             if move_data:
-                max_idx = max(chain(dispset, dispset.values())) + 1
-                if len(self.data) < max_idx:
-                    self.data[:] = self.data + list(repeat("", max_idx - len(self.data)))
+                max_len = max(chain(dispset, dispset.values())) + 1
+                if len(self.data) < max_len:
+                    self.fix_data_len(max_len - 1)
                 new = []
                 idx = 0
                 done = set()
                 while len(new) < len(self.data):
                     if idx in dispset and idx not in done:
                         new.append(self.data[dispset[idx]])
                         done.add(idx)
                     elif idx not in done:
                         new.append(self.data[idx])
                         idx += 1
                     else:
                         idx += 1
                 self.data = new
+                self.RI.fix_index(max_len - 1)
                 if isinstance(self._row_index, list) and self._row_index:
-                    if len(self._row_index) < max_idx:
-                        self._row_index[:] = self._row_index + list(repeat("", max_idx - len(self._row_index)))
                     new = []
                     idx = 0
                     done = set()
                     while len(new) < len(self._row_index):
                         if idx in dispset and idx not in done:
                             new.append(self._row_index[dispset[idx]])
                             done.add(idx)
                         elif idx not in done:
                             new.append(self._row_index[idx])
                             idx += 1
                         else:
                             idx += 1
                     self._row_index = new
-            dispset = {b: a for a, b in dispset.items()}
-            self.RI.cell_options = {dispset[k] if k in dispset else k: v for k, v in self.RI.cell_options.items()}
-            self.cell_options = {(dispset[k[0]], k[1]) if k[0] in dispset else k: v for k, v in self.cell_options.items()}
-            self.row_options = {dispset[k] if k in dispset else k: v for k, v in self.row_options.items()}
-        return new_selected, dispset
+        return new_selected, {b: a for a, b in dispset.items()}
 
     def ctrl_z(self, event = None):
         if not self.undo_storage:
             return
         if not isinstance(self.undo_storage[-1], (tuple, dict)):
             undo_storage = pickle.loads(zlib.decompress(self.undo_storage[-1]))
         else:
@@ -966,83 +1009,70 @@
                 self.extra_begin_ctrl_z_func(UndoEvent("begin_ctrl_z", undo_storage[0], undo_storage))
             except:
                 return
         self.undo_storage.pop()
         if undo_storage[0] in ("edit_header", ):
             for c, v in undo_storage[1].items():
                 self._headers[c] = v
-            for box in undo_storage[2]:
-                r1, c1, r2, c2 = box[0]
-                if not self.expand_sheet_if_paste_too_big:
-                    self.create_selected(r1, c1, r2, c2, box[1])
+            self.reselect_from_get_boxes(undo_storage[2])
             self.create_current(0, undo_storage[3][1], type_ = "column", inside = True)
             
         if undo_storage[0] in ("edit_index", ):
             for r, v in undo_storage[1].items():
                 self._row_index[r] = v
-            for box in undo_storage[2]:
-                r1, c1, r2, c2 = box[0]
-                if not self.expand_sheet_if_paste_too_big:
-                    self.create_selected(r1, c1, r2, c2, box[1])
+            self.reselect_from_get_boxes(undo_storage[2])
             self.create_current(0, undo_storage[3][1], type_ = "row", inside = True)
                         
         if undo_storage[0] in ("edit_cells", "edit_cells_paste"):
             for (datarn, datacn), v in undo_storage[1].items():
                 self.set_cell_data(datarn, datacn, v)
             start_row = float("inf")
             start_col = float("inf")
-            for box in undo_storage[2]:
-                r1, c1, r2, c2 = box[0]
-                if not self.expand_sheet_if_paste_too_big:
-                    self.create_selected(r1, c1, r2, c2, box[1])
-                if r1 < start_row:
-                    start_row = r1
-                if c1 < start_col:
-                    start_col = c1
             if undo_storage[0] == "edit_cells_paste" and self.expand_sheet_if_paste_too_big:
                 if undo_storage[4][0] > 0:
                     self.del_row_positions(len(self.row_positions) - 1 - undo_storage[4][0], undo_storage[4][0])
                     self.data[:] = self.data[:-undo_storage[4][0]]
+                    if not self.all_rows_displayed:
+                        self.displayed_rows[:] = self.displayed_rows[:-undo_storage[4][0]]
                 if undo_storage[4][1] > 0:
                     quick_added_cols = undo_storage[4][1]
                     self.del_col_positions(len(self.col_positions) - 1 - quick_added_cols, quick_added_cols)
                     for rn in range(len(self.data)):
                         self.data[rn][:] = self.data[rn][:-quick_added_cols]
                     if not self.all_columns_displayed:
                         self.displayed_columns[:] = self.displayed_columns[:-quick_added_cols]
+            self.reselect_from_get_boxes(undo_storage[2])
             if undo_storage[3]:
-                if isinstance(undo_storage[3][0], int):
-                    self.create_current(undo_storage[3][0], undo_storage[3][1], type_ = "cell", inside = True if self.cell_selected(undo_storage[3][0], undo_storage[3][1]) else False)
-                elif undo_storage[3][0] == "column":
-                    self.create_current(0, undo_storage[3][1], type_ = "column", inside = True)
-                elif undo_storage[3][0] == "row":
-                    self.create_current(undo_storage[3][1], 0, type_ = "row", inside = True)
+                self.create_current(undo_storage[3].row,
+                                    undo_storage[3].column, 
+                                    type_ = undo_storage[3].type_, 
+                                    inside = True if self.cell_selected(undo_storage[3].row, undo_storage[3].column) else False)
             elif start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
                 self.create_current(start_row, start_col, type_ = "cell", inside = True if self.cell_selected(start_row, start_col) else False)
             if start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
                 self.see(r = start_row, c = start_col, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
         
         elif undo_storage[0] == "move_cols":
-            c = undo_storage[1]
-            to_move_min = undo_storage[2]
-            totalcols = len(undo_storage[4])
+            c = undo_storage[1][0]
+            to_move_min = undo_storage[2][0]
+            totalcols = len(undo_storage[2])
             if to_move_min < c:
                 c += totalcols - 1
             self.move_columns_adjust_options_dict(c, to_move_min, totalcols)
         
         elif undo_storage[0] == "move_rows":
             rhs = [int(b - a) for a, b in zip(self.row_positions, islice(self.row_positions, 1, len(self.row_positions)))]
-            r = undo_storage[1]
-            to_move_min = undo_storage[2]
-            totalrows = len(undo_storage[4])
+            r = undo_storage[1][0]
+            to_move_min = undo_storage[2][0]
+            totalrows = len(undo_storage[2])
             if to_move_min < r:
                 r += totalrows - 1
             self.move_rows_adjust_options_dict(r, to_move_min, totalrows)
                     
-        elif undo_storage[0] == "insert_row":
+        elif undo_storage[0] == "insert_rows":
             self.displayed_rows = undo_storage[1]['displayed_rows']
             self.data[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
             try:
                 self._row_index[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
             except:
                 pass
             self.del_row_positions(undo_storage[1]['sheet_row_num'],
@@ -1060,29 +1090,29 @@
             self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items()}
             self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items()}
             if len(self.row_positions) > 1:
                 start_row = undo_storage[1]['sheet_row_num'] if undo_storage[1]['sheet_row_num'] < len(self.row_positions) - 1 else undo_storage[1]['sheet_row_num'] - 1
                 self.RI.select_row(start_row)
                 self.see(r = start_row, c = 0, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
                 
-        elif undo_storage[0] == "insert_col":
+        elif undo_storage[0] == "insert_cols":
             self.displayed_columns = undo_storage[1]['displayed_columns']
             qx = undo_storage[1]['data_col_num']
             qnum = undo_storage[1]['numcols']
             for rn in range(len(self.data)):
                 self.data[rn][qx:qx + qnum] = []
             try:
                 self._headers[qx:qx + qnum] = []
             except:
                 pass
             self.del_col_positions(undo_storage[1]['sheet_col_num'],
                                     undo_storage[1]['numcols'],
                                     deselect_all = False)
             for c in range(undo_storage[1]['sheet_col_num'],
-                            undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']):
+                           undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']):
                 if c in self.col_options:
                     del self.col_options[c]
                 if c in self.CH.cell_options:
                     del self.CH.cell_options[c]
             numcols = undo_storage[1]['numcols']
             idx = undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']
             self.cell_options = {(rn, cn if cn < idx else cn - numcols): t2 for (rn, cn), t2 in self.cell_options.items()}
@@ -1118,24 +1148,24 @@
                 self.insert_col_position(idx = cn, width = w)
             for cn, rowdict in reversed(tuple(undo_storage[1]['deleted_cols'].items())):
                 for rn, v in rowdict.items():
                     try:
                         self.data[rn].insert(cn, v)
                     except:
                         continue
-            for cn, v in reversed(tuple(undo_storage[1]['deleted_hdr_values'].items())):
+            for cn, v in reversed(tuple(undo_storage[1]['deleted_header_values'].items())):
                 try:
                     self._headers.insert(cn, v)
                 except:
                     continue
             self.reselect_from_get_boxes(undo_storage[1]['selection_boxes'])
         self.refresh()
         if self.extra_end_ctrl_z_func is not None:
             self.extra_end_ctrl_z_func(UndoEvent("end_ctrl_z", undo_storage[0], undo_storage))
-        self.event_generate("<<SheetDataChangeEvent>>")
+        self.parentframe.emit_modified_event()
 
     def bind_arrowkeys(self, keys: dict = {}):
         for canvas in (self, self.parentframe, self.CH, self.RI, self.TL):
             for k, func in keys.items():
                 canvas.bind(f"<{arrowkey_bindings_helper[k.lower()]}>", func)
 
     def unbind_arrowkeys(self, keys: dict = {}):
@@ -1229,35 +1259,36 @@
         cx1, cy1, cx2, cy2 = self.get_canvas_visible_area()
         x1, y1, x2, y2 = self.get_cell_coords(r, c)
         if x1 <= cx2 or y1 <= cy2 or x2 >= cx1 or y2 >= cy1:
             return True
         return False
 
     def select_all(self, redraw = True, run_binding_func = True):
+        currently_selected = self.currently_selected()
         self.deselect("all")
         if len(self.row_positions) > 1 and len(self.col_positions) > 1:
-            self.create_current(0, 0, type_ = "cell", inside = True)
+            if currently_selected:
+                self.create_current(currently_selected.row, currently_selected.column, type_ = "cell", inside = True)
+            else:
+                self.create_current(0, 0, type_ = "cell", inside = True)
             self.create_selected(0, 0, len(self.row_positions) - 1, len(self.col_positions) - 1)
             if redraw:
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
             if self.select_all_binding_func is not None and run_binding_func:
                 self.select_all_binding_func(SelectionBoxEvent("select_all_cells", (0, 0, len(self.row_positions) - 1, len(self.col_positions) - 1)))
 
     def select_cell(self, r, c, redraw = False, keep_other_selections = False):
         r = int(r)
         c = int(c)
-        ignore_keep = False
         if keep_other_selections:
-            if self.cell_selected(r, c):
-                self.create_current(r, c, type_ = "cell", inside = True)
-            else:
-                ignore_keep = True
-        if ignore_keep or not keep_other_selections:
+            inside = self.cell_selected(r, c)
+        else:
+            inside = False
             self.delete_selection_rects()
-            self.create_current(r, c, type_ = "cell", inside = False)
+        self.create_current(r, c, type_ = "cell", inside = inside)
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None:
             self.selection_binding_func(SelectCellEvent("select_cell", r, c))
 
     def add_selection(self, r, c, redraw = False, run_binding_func = True, set_as_current = False):
         r = int(r)
@@ -1269,15 +1300,15 @@
                 if alltags[2] == "cell":
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     add_sel = (r1, c1)
                 else:
                     add_sel = tuple()
             else:
                 add_sel = tuple()
-            self.create_current(r, c, type_ = "cell", inside = True if self.cell_selected(r, c) else False)
+            self.create_current(r, c, type_ = "cell", inside = self.cell_selected(r, c))
             if add_sel:
                 self.add_selection(add_sel[0], add_sel[1], redraw = False, run_binding_func = False, set_as_current = False)
         else:
             self.create_selected(r, c, r + 1, c + 1)
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
@@ -1380,131 +1411,14 @@
                         self.cell_options[(r, c)] = {}
                     self.cell_options[(r, c)]['align'] = align
             else:
                 if (row, column) not in self.cell_options:
                     self.cell_options[(row, column)] = {}
                 self.cell_options[(row, column)]['align'] = align
 
-    def readonly_rows(self, rows = [], readonly = True):
-        if isinstance(rows, int):
-            rows_ = [rows]
-        else:
-            rows_ = rows
-        if not readonly:
-            for r in rows_:
-                if r in self.row_options and 'readonly' in self.row_options[r]:
-                    del self.row_options[r]['readonly']
-        else:
-            for r in rows_:
-                if r not in self.row_options:
-                    self.row_options[r] = {}
-                self.row_options[r]['readonly'] = True
-
-    def readonly_columns(self, columns = [], readonly = True):
-        if isinstance(columns, int):
-            cols_ = [columns]
-        else:
-            cols_ = columns
-        if not readonly:
-            for c in cols_:
-                if c in self.col_options and 'readonly' in self.col_options[c]:
-                    del self.col_options[c]['readonly']
-        else:
-            for c in cols_:
-                if c not in self.col_options:
-                    self.col_options[c] = {}
-                self.col_options[c]['readonly'] = True
-
-    def readonly_cells(self, row = 0, column = 0, cells = [], readonly = True):
-        if not readonly:
-            if cells:
-                for r, c in cells:
-                    if (r, c) in self.cell_options and 'readonly' in self.cell_options[(r, c)]:
-                        del self.cell_options[(r, c)]['readonly']
-            else:
-                if (row, column) in self.cell_options and 'readonly' in self.cell_options[(row, column)]:
-                    del self.cell_options[(row, column)]['readonly']
-        else:
-            if cells:
-                for (r, c) in cells:
-                    if (r, c) not in self.cell_options:
-                        self.cell_options[(r, c)] = {}
-                    self.cell_options[(r, c)]['readonly'] = True
-            else:
-                if (row, column) not in self.cell_options:
-                    self.cell_options[(row, column)] = {}
-                self.cell_options[(row, column)]['readonly'] = True
-
-    def highlight_cells(self, r = 0, c = 0, cells = tuple(), bg = None, fg = None, redraw = False, overwrite = True):
-        if bg is None and fg is None:
-            return
-        if cells:
-            for r_, c_ in cells:
-                if (r_, c_) not in self.cell_options:
-                    self.cell_options[(r_, c_)] = {}
-                if 'highlight' in self.cell_options[(r_, c_)] and not overwrite:
-                    self.cell_options[(r_, c_)]['highlight'] = (self.cell_options[(r_, c_)]['highlight'][0] if bg is None else bg,
-                                                                self.cell_options[(r_, c_)]['highlight'][1] if fg is None else fg)
-                else:
-                    self.cell_options[(r_, c_)]['highlight'] = (bg, fg)
-        else:
-            if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
-                riter = range(self.total_data_rows())
-                citer = (c, )
-            elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
-                riter = (r, )
-                citer = range(self.total_data_cols())
-            elif isinstance(r, int) and isinstance(c, int):
-                riter = (r, )
-                citer = (c, )
-            for r_ in riter:
-                for c_ in citer:
-                    if (r_, c_) not in self.cell_options:
-                        self.cell_options[(r_, c_)] = {}
-                    if 'highlight' in self.cell_options[(r_, c_)] and not overwrite:
-                        self.cell_options[(r_, c_)]['highlight'] = (self.cell_options[(r_, c_)]['highlight'][0] if bg is None else bg,
-                                                                    self.cell_options[(r_, c_)]['highlight'][1] if fg is None else fg)
-                    else:
-                        self.cell_options[(r_, c_)]['highlight'] = (bg, fg)
-        if redraw:
-            self.main_table_redraw_grid_and_text()
-
-    def highlight_cols(self, cols = [], bg = None, fg = None, highlight_header = False, redraw = False, overwrite = True):
-        if bg is None and fg is None:
-            return
-        for c in (cols, ) if isinstance(cols, int) else cols:
-            if c not in self.col_options:
-                self.col_options[c] = {}
-            if 'highlight' in self.col_options[c] and not overwrite:
-                self.col_options[c]['highlight'] = (self.col_options[c]['highlight'][0] if bg is None else bg,
-                                                    self.col_options[c]['highlight'][1] if fg is None else fg)
-            else:
-                self.col_options[c]['highlight'] = (bg, fg)
-        if highlight_header:
-            self.CH.highlight_cells(cells = cols, bg = bg, fg = fg)
-        if redraw:
-            self.main_table_redraw_grid_and_text(redraw_header = highlight_header)
-
-    def highlight_rows(self, rows = [], bg = None, fg = None, highlight_index = False, redraw = False, end_of_screen = False, overwrite = True):
-        if bg is None and fg is None:
-            return
-        for r in (rows, ) if isinstance(rows, int) else rows:
-            if r not in self.row_options:
-                self.row_options[r] = {}
-            if 'highlight' in self.row_options[r] and not overwrite:
-                self.row_options[r]['highlight'] = (self.row_options[r]['highlight'][0] if bg is None else bg,
-                                                    self.row_options[r]['highlight'][1] if fg is None else fg,
-                                                    self.row_options[r]['highlight'][2] if self.row_options[r]['highlight'][2] != end_of_screen else end_of_screen)
-            else:
-                self.row_options[r]['highlight'] = (bg, fg, end_of_screen)
-        if highlight_index:
-            self.RI.highlight_cells(cells = rows, bg = bg, fg = fg)
-        if redraw:
-            self.main_table_redraw_grid_and_text(redraw_row_index = highlight_index)
-
     def deselect(self, r = None, c = None, cell = None, redraw = True):
         deselected = tuple()
         deleted_boxes = {}
         if r == "all":
             deselected = ("deselect_all", self.delete_selection_rects())
         elif r == "allrows":
             for item in self.find_withtag("RowSelectFill"):
@@ -1857,20 +1771,20 @@
                 self.bind_cell_edit(True)
             else:
                 self.bind_cell_edit(False)
         # edit header with text editor (dropdowns and checkboxes not included)
         # this will not by enabled by using enable_bindings() to enable all bindings
         # must be enabled directly using enable_bindings("edit_header")
         # the same goes for "edit_index"
-        if key == "edit_header":
+        if key is None or key == "edit_header":
             if enable:
                 self.CH.bind_cell_edit(True)
             else:
                 self.CH.bind_cell_edit(False)
-        if key == "edit_index":
+        if key is None or key == "edit_index":
             if enable:
                 self.RI.bind_cell_edit(True)
             else:
                 self.RI.bind_cell_edit(False)
 
     def menu_add_command(self, menu: tk.Menu, **kwargs):
         if 'label' not in kwargs:
@@ -2058,31 +1972,31 @@
             self.menu_add_command(self.CH.ch_rc_popup_menu,
                                   label = "Insert columns left",
                                   font = self.popup_menu_font,
                                   foreground = self.popup_menu_fg,
                                   background = self.popup_menu_bg,
                                   activebackground = self.popup_menu_highlight_bg,
                                   activeforeground = self.popup_menu_highlight_fg,
-                                  command = lambda: self.insert_col_rc("left"))
+                                  command = lambda: self.insert_cols_rc("left"))
             self.menu_add_command(self.empty_rc_popup_menu, 
                                   label = "Insert column",
                                   font = self.popup_menu_font,
                                   foreground = self.popup_menu_fg,
                                   background = self.popup_menu_bg,
                                   activebackground = self.popup_menu_highlight_bg,
                                   activeforeground = self.popup_menu_highlight_fg,
-                                  command = lambda: self.insert_col_rc("left"))
+                                  command = lambda: self.insert_cols_rc("left"))
             self.menu_add_command(self.CH.ch_rc_popup_menu, 
                                   label = "Insert columns right",
                                   font = self.popup_menu_font,
                                   foreground = self.popup_menu_fg,
                                   background = self.popup_menu_bg,
                                   activebackground = self.popup_menu_highlight_bg,
                                   activeforeground = self.popup_menu_highlight_fg,
-                                  command = lambda: self.insert_col_rc("right"))
+                                  command = lambda: self.insert_cols_rc("right"))
         if self.rc_delete_row_enabled:
             self.menu_add_command(self.RI.ri_rc_popup_menu, 
                                   label = "Delete rows",
                                   font = self.popup_menu_font,
                                   foreground = self.popup_menu_fg,
                                   background = self.popup_menu_bg,
                                   activebackground = self.popup_menu_highlight_bg,
@@ -2092,31 +2006,31 @@
             self.menu_add_command(self.RI.ri_rc_popup_menu,
                                   label = "Insert rows above",
                                   font = self.popup_menu_font,
                                   foreground = self.popup_menu_fg,
                                   background = self.popup_menu_bg,
                                   activebackground = self.popup_menu_highlight_bg,
                                   activeforeground = self.popup_menu_highlight_fg,
-                                  command = lambda: self.insert_row_rc("above"))
+                                  command = lambda: self.insert_rows_rc("above"))
             self.menu_add_command(self.RI.ri_rc_popup_menu, 
                                   label = "Insert rows below",
                                   font = self.popup_menu_font,
                                   foreground = self.popup_menu_fg,
                                   background = self.popup_menu_bg,
                                   activebackground = self.popup_menu_highlight_bg,
                                   activeforeground = self.popup_menu_highlight_fg,
-                                  command = lambda: self.insert_row_rc("below"))
+                                  command = lambda: self.insert_rows_rc("below"))
             self.menu_add_command(self.empty_rc_popup_menu, 
                                   label = "Insert row",
                                   font = self.popup_menu_font,
                                   foreground = self.popup_menu_fg,
                                   background = self.popup_menu_bg,
                                   activebackground = self.popup_menu_highlight_bg,
                                   activeforeground = self.popup_menu_highlight_fg,
-                                  command = lambda: self.insert_row_rc("below"))
+                                  command = lambda: self.insert_rows_rc("below"))
         for label, func in self.extra_table_rc_menu_funcs.items():
             self.menu_add_command(self.rc_popup_menu, 
                                   label = label,
                                   font = self.popup_menu_font,
                                   foreground = self.popup_menu_fg,
                                   background = self.popup_menu_bg,
                                   activebackground = self.popup_menu_highlight_bg,
@@ -2216,14 +2130,15 @@
             self.edit_bindings(True)
             self.rc_delete_column_enabled = True
             self.rc_delete_row_enabled = True
             self.rc_insert_column_enabled = True
             self.rc_insert_row_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
+            self.ctrl_select_enabled = True
             self.TL.rh_state()
             self.TL.rw_state()
         elif binding in ("single", "single_selection_mode", "single_select"):
             self.single_selection_enabled = True
             self.toggle_selection_enabled = False
         elif binding in ("toggle", "toggle_selection_mode", "toggle_select"):
             self.toggle_selection_enabled = True
@@ -2285,14 +2200,16 @@
         elif binding == "delete":
             self.edit_bindings(True, "delete")
         elif binding in ("right_click_popup_menu", "rc_popup_menu"):
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
         elif binding in ("right_click_select", "rc_select"):
             self.rc_select_enabled = True
+        elif binding in ("ctrl_click_select", "ctrl_select"):
+            self.ctrl_select_enabled = True
         elif binding == "undo":
             self.edit_bindings(True, "undo")
         elif binding == "edit_cell":
             self.edit_bindings(True, "edit_cell")
         elif binding == "edit_header":
             self.edit_bindings(True, "edit_header")
         elif binding == "edit_index":
@@ -2319,14 +2236,15 @@
             self.edit_bindings(False)
             self.rc_delete_column_enabled = False
             self.rc_delete_row_enabled = False
             self.rc_insert_column_enabled = False
             self.rc_insert_row_enabled = False
             self.rc_popup_menus_enabled = False
             self.rc_select_enabled = False
+            self.ctrl_select_enabled = False
             self.TL.rh_state("hidden")
             self.TL.rw_state("hidden")
         elif binding in ("single", "single_selection_mode", "single_select"):
             self.single_selection_enabled = False
         elif binding in ("toggle", "toggle_selection_mode", "toggle_select"):
             self.toggle_selection_enabled = False
         elif binding == "drag_select":
@@ -2377,14 +2295,16 @@
             self.edit_bindings(False, "paste")
         elif binding == "delete":
             self.edit_bindings(False, "delete")
         elif binding in ("right_click_popup_menu", "rc_popup_menu"):
             self.rc_popup_menus_enabled = False
         elif binding in ("right_click_select", "rc_select"):
             self.rc_select_enabled = False
+        elif binding in ("ctrl_click_select", "ctrl_select"):
+            self.ctrl_select_enabled = False
         elif binding == "undo":
             self.edit_bindings(False, "undo")
         elif binding == "edit_cell":
             self.edit_bindings(False, "edit_cell")
         elif binding == "edit_header":
             self.edit_bindings(False, "edit_header")
         elif binding == "edit_index":
@@ -2530,14 +2450,57 @@
     def delete_resize_lines(self):
         self.hidd_resize_lines.update(self.disp_resize_lines)
         self.disp_resize_lines = {}
         for t, sh in self.hidd_resize_lines.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_resize_lines[t] = False
+                
+    def ctrl_b1_press(self, event = None):
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
+        self.focus_set()
+        if self.ctrl_select_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
+            self.b1_pressed_loc = None
+            rowsel = int(self.identify_row(y = event.y))
+            colsel = int(self.identify_col(x = event.x))
+            if rowsel < len(self.row_positions) - 1 and colsel < len(self.col_positions) - 1:
+                currently_selected = self.currently_selected()
+                if not currently_selected or currently_selected.row != rowsel or currently_selected.column != colsel:
+                    self.add_selection(rowsel, colsel, set_as_current = True)
+                self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
+                if self.ctrl_selection_binding_func is not None:
+                    self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_cells", (rowsel, colsel, rowsel + 1, colsel + 1)))
+                    
+    def ctrl_shift_b1_press(self, event = None):
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
+        self.focus_set()
+        if self.ctrl_select_enabled and self.drag_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
+            self.b1_pressed_loc = None
+            rowsel = int(self.identify_row(y = event.y))
+            colsel = int(self.identify_col(x = event.x))
+            if rowsel < len(self.row_positions) - 1 and colsel < len(self.col_positions) - 1:
+                currently_selected = self.currently_selected()
+                if currently_selected and currently_selected.type_ == "cell":
+                    min_r = currently_selected[0]
+                    min_c = currently_selected[1]
+                    if rowsel >= min_r and colsel >= min_c:
+                        last_selected = (min_r, min_c, rowsel + 1, colsel + 1)
+                    elif rowsel >= min_r and min_c >= colsel:
+                        last_selected = (min_r, colsel, rowsel + 1, min_c + 1)
+                    elif min_r >= rowsel and colsel >= min_c:
+                        last_selected = (rowsel, min_c, min_r + 1, colsel + 1)
+                    elif min_r >= rowsel and min_c >= colsel:
+                        last_selected = (rowsel, colsel, min_r + 1, min_c + 1)
+                    self.create_selected(*last_selected)
+                else:
+                    self.add_selection(rowsel, colsel, set_as_current = True)
+                    last_selected = (rowsel, colsel, rowsel + 1, colsel + 1)
+                self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
+                if self.shift_selection_binding_func is not None:
+                    self.shift_selection_binding_func(SelectionBoxEvent("shift_select_cells", last_selected))
 
     def shift_b1_press(self, event = None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if self.drag_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
             self.b1_pressed_loc = None
             rowsel = int(self.identify_row(y = event.y))
@@ -2559,119 +2522,116 @@
                     last_selected = tuple(int(e) for e in self.gettags(self.find_withtag("CellSelectFill"))[1].split("_") if e)
                 else:
                     self.select_cell(rowsel, colsel, redraw = False)
                     last_selected = tuple(int(e) for e in self.gettags(self.find_withtag("Current_Outside"))[1].split("_") if e)
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
                 if self.shift_selection_binding_func is not None:
                     self.shift_selection_binding_func(SelectionBoxEvent("shift_select_cells", last_selected))
+                    
+    def get_b1_motion_rect(self, start_row, start_col, end_row, end_col):
+        if (end_row >= start_row and 
+            end_col >= start_col and
+            (end_row - start_row or end_col - start_col)):
+            return (start_row, start_col, end_row + 1, end_col + 1, "cells")
+        elif (end_row >= start_row and 
+              end_col < start_col and
+              (end_row - start_row or start_col - end_col)):
+            return (start_row, end_col, end_row + 1, start_col + 1, "cells")
+        elif (end_row < start_row and
+              end_col >= start_col and
+              (start_row - end_row or end_col - start_col)):
+            return (end_row, start_col, start_row + 1, end_col + 1, "cells")
+        elif (end_row < start_row and 
+              end_col < start_col and
+              (start_row - end_row or start_col - end_col)):
+            return (end_row, end_col, start_row + 1, start_col + 1, "cells")
+        else:
+            return (start_row, start_col, start_row + 1, start_col + 1, "cells")
+        return None
         
     def b1_motion(self, event):
         x1, y1, x2, y2 = self.get_canvas_visible_area()
         if self.drag_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
             need_redraw = False
             end_row = self.identify_row(y = event.y)
             end_col = self.identify_col(x = event.x)
             currently_selected = self.currently_selected()
             if end_row < len(self.row_positions) - 1 and end_col < len(self.col_positions) - 1 and currently_selected and currently_selected.type_ == "cell":
-                start_row = currently_selected[0]
-                start_col = currently_selected[1]
-                rect = None
-                if (end_row >= start_row and 
-                    end_col >= start_col and
-                    (end_row - start_row or end_col - start_col)):
-                    rect = (start_row, start_col, end_row + 1, end_col + 1)
-                elif (end_row >= start_row and 
-                      end_col < start_col and
-                      (end_row - start_row or start_col - end_col)):
-                    rect = (start_row, end_col, end_row + 1, start_col + 1)
-                elif (end_row < start_row and
-                      end_col >= start_col and
-                      (start_row - end_row or end_col - start_col)):
-                    rect = (end_row, start_col, start_row + 1, end_col + 1)
-                elif (end_row < start_row and 
-                      end_col < start_col and
-                      (start_row - end_row or start_col - end_col)):
-                    rect = (end_row, end_col, start_row + 1, start_col + 1)
-                else:
-                    rect = (start_row, start_col, start_row + 1, start_col + 1)
+                rect = self.get_b1_motion_rect(*(currently_selected[0], currently_selected[1], end_row, end_col))
                 if rect is not None and self.being_drawn_rect != rect:
                     self.delete_selection_rects(delete_current = False)
                     if rect[2] - rect[0] == 1 and rect[3] - rect[1] == 1:
                         self.being_drawn_rect = rect
                     else:
                         self.being_drawn_rect = rect
                         self.create_selected(*rect)
                     if self.drag_selection_binding_func is not None:
-                        self.drag_selection_binding_func(SelectionBoxEvent("drag_select_cells", rect))
+                        self.drag_selection_binding_func(SelectionBoxEvent("drag_select_cells", rect[:-1]))
                     need_redraw = True
-            if self.data:
-                xcheck = self.xview()
-                ycheck = self.yview()
-                if len(xcheck) > 1 and xcheck[0] > 0 and event.x < 0:
-                    try:
-                        self.xview_scroll(-1, "units")
-                        self.CH.xview_scroll(-1, "units")
-                    except:
-                        pass
-                    need_redraw = True
-                if len(ycheck) > 1 and ycheck[0] > 0 and event.y < 0:
-                    try:
-                        self.yview_scroll(-1, "units")
-                        self.RI.yview_scroll(-1, "units")
-                    except:
-                        pass
-                    need_redraw = True
-                if len(xcheck) > 1 and xcheck[1] < 1 and event.x > self.winfo_width():
-                    try:
-                        self.xview_scroll(1, "units")
-                        self.CH.xview_scroll(1, "units")
-                    except:
-                        pass
-                    need_redraw = True
-                if len(ycheck) > 1 and ycheck[1] < 1 and event.y > self.winfo_height():
-                    try:
-                        self.yview_scroll(1, "units")
-                        self.RI.yview_scroll(1, "units")
-                    except:
-                        pass
-                    need_redraw = True
-            self.check_views()
+            if self.scroll_if_event_offscreen(event):
+                need_redraw = True
             if need_redraw:
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
         elif self.RI.width_resizing_enabled and self.RI.rsz_w is not None and self.RI.currently_resizing_width:
             self.RI.delete_resize_lines()
             self.delete_resize_lines()
             if event.x >= 0:
                 x = self.canvasx(event.x)
                 self.new_row_width = self.RI.current_width + event.x
                 self.create_resize_line(x, y1, x, y2, width = 1, fill = self.RI.resizing_line_fg, tag = "rwl")
             else:
                 x = self.RI.current_width + event.x
-                if x < self.min_cw:
-                    x = int(self.min_cw)
+                if x < self.min_column_width:
+                    x = int(self.min_column_width)
                 self.new_row_width = x
                 self.RI.create_resize_line(x, y1, x, y2, width = 1, fill = self.RI.resizing_line_fg, tag = "rwl")
         elif self.CH.height_resizing_enabled and self.CH.rsz_h is not None and self.CH.currently_resizing_height:
             self.CH.delete_resize_lines()
             self.delete_resize_lines()
             if event.y >= 0:
                 y = self.canvasy(event.y)
                 self.new_header_height = self.CH.current_height + event.y
                 self.create_resize_line(x1, y, x2, y, width = 1, fill = self.RI.resizing_line_fg, tag = "rhl")
             else:
                 y = self.CH.current_height + event.y
-                if y < self.hdr_min_rh:
-                    y = int(self.hdr_min_rh)
+                if y < self.min_header_height:
+                    y = int(self.min_header_height)
                 self.new_header_height = y
                 self.CH.create_resize_line(x1, y, x2, y, width = 1, fill = self.RI.resizing_line_fg, tag = "rhl")
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
+            
+    def ctrl_b1_motion(self, event):
+        x1, y1, x2, y2 = self.get_canvas_visible_area()
+        if self.ctrl_select_enabled and self.drag_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
+            need_redraw = False
+            end_row = self.identify_row(y = event.y)
+            end_col = self.identify_col(x = event.x)
+            currently_selected = self.currently_selected()
+            if end_row < len(self.row_positions) - 1 and end_col < len(self.col_positions) - 1 and currently_selected and currently_selected.type_ == "cell":
+                rect = self.get_b1_motion_rect(*(currently_selected[0], currently_selected[1], end_row, end_col))
+                if rect is not None and self.being_drawn_rect != rect:
+                    if rect[2] - rect[0] == 1 and rect[3] - rect[1] == 1:
+                        self.being_drawn_rect = rect
+                    else:
+                        if self.being_drawn_rect is not None:
+                            self.delete_selected(*self.being_drawn_rect)
+                        self.being_drawn_rect = rect
+                        self.create_selected(*rect)
+                    if self.drag_selection_binding_func is not None:
+                        self.drag_selection_binding_func(SelectionBoxEvent("drag_select_cells", rect[:-1]))
+                    need_redraw = True
+            if self.scroll_if_event_offscreen(event):
+                need_redraw = True
+            if need_redraw:
+                self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
 
     def b1_release(self, event = None):
         if self.being_drawn_rect is not None and (self.being_drawn_rect[2] - self.being_drawn_rect[0] > 1 or self.being_drawn_rect[3] - self.being_drawn_rect[1] > 1):
+            self.delete_selected(*self.being_drawn_rect)
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.create_selected(*to_sel)
         else:
             self.being_drawn_rect = None
         if self.RI.width_resizing_enabled and self.RI.rsz_w is not None and self.RI.currently_resizing_width:
             self.delete_resize_lines()
@@ -2691,25 +2651,25 @@
         self.CH.rsz_h = None
         if self.b1_pressed_loc is not None:
             r = self.identify_row(y = event.y, allow_end = False)
             c = self.identify_col(x = event.x, allow_end = False)
             if r is not None and c is not None and (r, c) == self.b1_pressed_loc:
                 datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                 datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 'checkbox' in self.cell_options[(datarn, datacn)]):
+                if self.get_cell_kwargs(datarn, datacn, key = 'dropdown') or self.get_cell_kwargs(datarn, datacn, key = 'checkbox'):
                     canvasx = self.canvasx(event.x)
                     if (
                         (self.closed_dropdown != self.b1_pressed_loc and
-                         'dropdown' in self.cell_options[(datarn, datacn)] and
-                         canvasx > self.col_positions[c + 1] - self.txt_h - 5 and
+                         self.get_cell_kwargs(datarn, datacn, key = 'dropdown') and
+                         canvasx > self.col_positions[c + 1] - self.txt_h - 4 and
                          canvasx < self.col_positions[c + 1] - 1) 
                         or
-                        ('checkbox' in self.cell_options[(datarn, datacn)] and 
-                         canvasx < self.col_positions[c] + self.txt_h + 5 and
-                         self.canvasy(event.y) < self.row_positions[r] + self.txt_h + 5)
+                        (self.get_cell_kwargs(datarn, datacn, key = 'checkbox') and 
+                         canvasx < self.col_positions[c] + self.txt_h + 4 and
+                         self.canvasy(event.y) < self.row_positions[r] + self.txt_h + 4)
                         ):
                         self.open_cell(event)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.b1_pressed_loc = None
         self.closed_dropdown = None
         if self.extra_b1_release_func is not None:
@@ -2758,58 +2718,93 @@
         c = bisect.bisect_left(self.col_positions, x2)
         if c != 0:
             c -= 1
         if not allow_end and c >= len(self.col_positions) - 1:
             return None
         return c
 
-    def check_views(self):
+    def fix_views(self):
         xcheck = self.xview()
         ycheck = self.yview()
         if xcheck and xcheck[0] <= 0:
             self.xview(*("moveto", 0))
             if self.show_header:
                 self.CH.xview(*("moveto", 0))
-
         elif len(xcheck) > 1 and xcheck[1] >= 1:
             self.xview(*("moveto", 1))
             if self.show_header:
                 self.CH.xview(*("moveto", 1))
-                
         if ycheck and ycheck[0] <= 0:
             self.yview(*("moveto", 0))
             if self.show_index:
                 self.RI.yview(*("moveto", 0))
         elif len(ycheck) > 1 and ycheck[1] >= 1:
             self.yview(*("moveto", 1))
             if self.show_index:
                 self.RI.yview(*("moveto", 1))
+                
+    def scroll_if_event_offscreen(self, event):
+        need_redraw = False
+        if self.data:
+            xcheck = self.xview()
+            ycheck = self.yview()
+            if len(xcheck) > 1 and xcheck[0] > 0 and event.x < 0:
+                try:
+                    self.xview_scroll(-1, "units")
+                    self.CH.xview_scroll(-1, "units")
+                except:
+                    pass
+                need_redraw = True
+            if len(ycheck) > 1 and ycheck[0] > 0 and event.y < 0:
+                try:
+                    self.yview_scroll(-1, "units")
+                    self.RI.yview_scroll(-1, "units")
+                except:
+                    pass
+                need_redraw = True
+            if len(xcheck) > 1 and xcheck[1] < 1 and event.x > self.winfo_width():
+                try:
+                    self.xview_scroll(1, "units")
+                    self.CH.xview_scroll(1, "units")
+                except:
+                    pass
+                need_redraw = True
+            if len(ycheck) > 1 and ycheck[1] < 1 and event.y > self.winfo_height():
+                try:
+                    self.yview_scroll(1, "units")
+                    self.RI.yview_scroll(1, "units")
+                except:
+                    pass
+                need_redraw = True
+        if need_redraw:
+            self.fix_views()
+        return need_redraw
 
     def set_xviews(self, *args):
         self.xview(*args)
         if self.show_header:
             self.CH.xview(*args)
-        self.check_views()
+        self.fix_views()
         self.main_table_redraw_grid_and_text(redraw_header = True if self.show_header else False)
 
     def set_yviews(self, *args):
         self.yview(*args)
         if self.show_index:
             self.RI.yview(*args)
-        self.check_views()
+        self.fix_views()
         self.main_table_redraw_grid_and_text(redraw_row_index = True if self.show_index else False)
 
     def set_view(self, x_args, y_args):
         self.xview(*x_args)
         if self.show_header:
             self.CH.xview(*x_args)
         self.yview(*y_args)
         if self.show_index:
             self.RI.yview(*y_args)
-        self.check_views()
+        self.fix_views()
         self.main_table_redraw_grid_and_text(redraw_row_index = True if self.show_index else False,
                                              redraw_header = True if self.show_header else False)
 
     def mousewheel(self, event = None):
         if event.delta < 0 or event.num == 5:
             self.yview_scroll(1, "units")
             self.RI.yview_scroll(1, "units")
@@ -2827,171 +2822,124 @@
         elif event.delta >= 0 or event.num == 4:
             if self.canvasx(0) <= 0:
                 return
             self.xview_scroll(-1, "units")
             self.CH.xview_scroll(-1, "units")
         self.main_table_redraw_grid_and_text(redraw_header = True)
 
-    def GetWidthChars(self, width):
-        char_w = self.GetTextWidth("_")
-        return int(width / char_w)
-
-    def GetTextWidth(self, txt):
-        self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self._font)
+    def get_txt_w(self, txt, font = None):
+        self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self.table_font if font is None else font)
         b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
         return b[2] - b[0]
 
-    def GetTextHeight(self, txt):
-        self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self._font)
+    def get_txt_h(self, txt, font = None):
+        self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self.table_font if font is None else font)
         b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
         return b[3] - b[1]
-
-    def GetHdrTextWidth(self, txt):
-        self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self._hdr_font)
-        b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
-        return b[2] - b[0]
-
-    def GetHdrTextHeight(self, txt):
-        self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self._hdr_font)
+    
+    def get_txt_dimensions(self, txt, font = None):
+        self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self.table_font if font is None else font)
         b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
-        return b[3] - b[1]
+        return b[2] - b[0], b[3] - b[1]
     
-    def GetLinesHeight(self, n, old_method = False):
-        if old_method:
-            if n == 1:
-                return int(self.min_rh)
-            else:
-                return int(self.fl_ins) + (self.xtra_lines_increment * n) - 2
-        else:
-            x = self.txt_measure_canvas.create_text(0, 0,
-                                                    text = "\n".join(["j^|" for lines in range(n)]) if n > 1 else "j^|",
-                                                    font = self._font)
-            b = self.txt_measure_canvas.bbox(x)
-            h = b[3] - b[1] + 5
-            self.txt_measure_canvas.delete(x)
-            return h
-
-    def GetHdrLinesHeight(self, n, old_method = False):
-        if old_method:
-            if n == 1:
-                return int(self.hdr_min_rh)
-            else:
-                return int(self.hdr_fl_ins) + (self.hdr_xtra_lines_increment * n) - 2
-        else:
-            x = self.txt_measure_canvas.create_text(0, 0,
-                                                    text = "\n".join(["j^|" for lines in range(n)]) if n > 1 else "j^|",
-                                                    font = self._hdr_font)
-            b = self.txt_measure_canvas.bbox(x)
-            h = b[3] - b[1] + 5
-            self.txt_measure_canvas.delete(x)
-            return h
+    def get_lines_cell_height(self, n, font = None):
+        return self.get_txt_h(txt = "\n".join(["j^|" for lines in range(n)]) if n > 1 else "j^|", font = self.table_font if font is None else font) + 5
 
-    def set_min_cw(self):
-        #w1 = self.GetHdrTextWidth("X") + 5
-        #w2 = self.GetTextWidth("X") + 5
-        #if w1 >= w2:
-        #    self.min_cw = w1
-        #else:
-        #    self.min_cw = w2
-        self.min_cw = 5
-        if self.min_cw > self.CH.max_cw:
-            self.CH.max_cw = self.min_cw + 20
-        if self.min_cw > self.default_cw:
-            self.default_cw = self.min_cw + 20
+    def set_min_column_width(self):
+        self.min_column_width = 5
+        if self.min_column_width > self.max_column_width:
+            self.max_column_width = self.min_column_width + 20
+        if self.min_column_width > self.default_column_width:
+            self.default_column_width = self.min_column_width + 20
 
     def font(self, newfont = None, reset_row_positions = False):
         if newfont:
             if not isinstance(newfont, tuple):
                 raise ValueError("Argument must be tuple e.g. ('Carlito',12,'normal')")
             if len(newfont) != 3:
                 raise ValueError("Argument must be three-tuple")
             if (
                 not isinstance(newfont[0], str) or
                 not isinstance(newfont[1], int) or
                 not isinstance(newfont[2], str)
                 ):
                 raise ValueError("Argument must be font, size and 'normal', 'bold' or 'italic' e.g. ('Carlito',12,'normal')")
-            else:
-                self._font = newfont
-            self.fnt_fam = newfont[0]
-            self.fnt_sze = newfont[1]
-            self.fnt_wgt = newfont[2]
-            self.set_fnt_help()
+            self.table_font = newfont
+            self.font_fam = newfont[0]
+            self.font_sze = newfont[1]
+            self.font_wgt = newfont[2]
+            self.set_font_help()
             if reset_row_positions:
                 self.reset_row_positions()
         else:
-            return self._font
+            return self.table_font
 
-    def set_fnt_help(self):
-        self.txt_h = self.GetTextHeight("|ZXjy*'^")
-        self.txt_w = self.GetTextWidth("|")
+    def set_font_help(self):
+        self.txt_h = self.get_txt_h("|ZXjy*'^")
+        self.txt_w = self.get_txt_w("|")
         self.half_txt_h = ceil(self.txt_h / 2)
         if self.half_txt_h % 2 == 0:
             self.fl_ins = self.half_txt_h + 2
         else:
             self.fl_ins = self.half_txt_h + 3
         self.xtra_lines_increment = int(self.txt_h)
-        self.min_rh = self.txt_h + 5
-        if self.min_rh < 12:
-            self.min_rh = 12
-        #self.min_rh = 5
-        if self.default_rh[0] != "pixels":
-            self.default_rh = (self.default_rh[0] if self.default_rh[0] != "pixels" else "pixels",
-                               self.GetLinesHeight(int(self.default_rh[0])) if self.default_rh[0] != "pixels" else self.default_rh[1])
-        self.set_min_cw()
+        self.min_row_height = self.txt_h + 5
+        if self.min_row_height < 12:
+            self.min_row_height = 12
+        if self.default_row_height[0] != "pixels":
+            self.default_row_height = (self.default_row_height[0] if self.default_row_height[0] != "pixels" else "pixels",
+                                       self.get_lines_cell_height(int(self.default_row_height[0])) if self.default_row_height[0] != "pixels" else self.default_row_height[1])
+        self.set_min_column_width()
         
     def header_font(self, newfont = None):
         if newfont:
             if not isinstance(newfont, tuple):
                 raise ValueError("Argument must be tuple e.g. ('Carlito', 12, 'normal')")
             if len(newfont) != 3:
                 raise ValueError("Argument must be three-tuple")
             if (
                 not isinstance(newfont[0], str) or
                 not isinstance(newfont[1], int) or
                 not isinstance(newfont[2], str)
                 ):
                 raise ValueError("Argument must be font, size and 'normal', 'bold' or 'italic' e.g. ('Carlito', 12, 'normal')")
-            else:
-                self._hdr_font = newfont
-            self.hdr_fnt_fam = newfont[0]
-            self.hdr_fnt_sze = newfont[1]
-            self.hdr_fnt_wgt = newfont[2]
-            self.set_hdr_fnt_help()
-        else:
-            return self._hdr_font
-
-    def set_hdr_fnt_help(self):
-        self.hdr_txt_h = self.GetHdrTextHeight("|ZXj*'^")
-        self.hdr_txt_w = self.GetHdrTextWidth("|")
-        self.hdr_half_txt_h = ceil(self.hdr_txt_h / 2)
-        if self.hdr_half_txt_h % 2 == 0:
-            self.hdr_fl_ins = self.hdr_half_txt_h + 2
-        else:
-            self.hdr_fl_ins = self.hdr_half_txt_h + 3
-        self.hdr_xtra_lines_increment = self.hdr_txt_h
-        self.hdr_min_rh = self.hdr_txt_h + 5
-        if self.default_hh[0] != "pixels":
-            self.default_hh = (self.default_hh[0] if self.default_hh[0] != "pixels" else "pixels",
-                               self.GetHdrLinesHeight(int(self.default_hh[0])) if self.default_hh[0] != "pixels" else self.default_hh[1])
-        self.set_min_cw()
-        self.CH.set_height(self.default_hh[1])
+            self.header_font = newfont
+            self.header_font_fam = newfont[0]
+            self.header_font_sze = newfont[1]
+            self.header_font_wgt = newfont[2]
+            self.set_header_font_help()
+        else:
+            return self.header_font
+
+    def set_header_font_help(self):
+        self.header_txt_w, self.header_txt_h = self.get_txt_dimensions("|", self.header_font)
+        self.header_half_txt_h = ceil(self.header_txt_h / 2)
+        if self.header_half_txt_h % 2 == 0:
+            self.header_fl_ins = self.header_half_txt_h + 2
+        else:
+            self.header_fl_ins = self.header_half_txt_h + 3
+        self.header_xtra_lines_increment = self.header_txt_h
+        self.min_header_height = self.header_txt_h + 5
+        if self.default_header_height[0] != "pixels":
+            self.default_header_height = (self.default_header_height[0] if self.default_header_height[0] != "pixels" else "pixels",
+                                          self.get_lines_cell_height(int(self.default_header_height[0]), font = self.header_font) if self.default_header_height[0] != "pixels" else self.default_header_height[1])
+        self.set_min_column_width()
+        self.CH.set_height(self.default_header_height[1])
         
-    def set_index_fnt_help(self):
+    def set_index_font_help(self):
         pass
 
     def data_reference(self,
                        newdataref = None, 
                        reset_col_positions = True, 
                        reset_row_positions = True,
                        redraw = False, 
                        return_id = True,
                        keep_formatting = True):
         if isinstance(newdataref, (list, tuple)):
-            newdataref = [["" if c is None else c for c in row] for row in newdataref]        
             self.data = newdataref
             if keep_formatting:
                 self.reapply_formatting()
             else:
                 self.delete_all_formatting(clear_values = False)
             self.undo_storage = deque(maxlen = self.max_undos)
             if reset_col_positions:
@@ -3004,44 +2952,43 @@
             return id(self.data)
         else:
             return self.data
         
     def get_cell_dimensions(self, datarn, datacn):
         txt = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
         if txt:
-            self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self._font)
+            self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text = txt, font = self.table_font)
             b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
             w = b[2] - b[0] + 7
             h = b[3] - b[1] + 5
         else:
-            w = self.min_cw
-            h = self.min_rh
-        if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
-                                                      'checkbox' in self.cell_options[(datarn, datacn)]):
+            w = self.min_column_width
+            h = self.min_row_height
+        if self.get_cell_kwargs(datarn, datacn, key = 'dropdown') or self.get_cell_kwargs(datarn, datacn, key = 'checkbox'):
             return w + self.txt_h, h
         return w, h
 
     def set_cell_size_to_text(self, r, c, only_set_if_too_small = False, redraw = True, run_binding = False):
-        min_cw = int(self.min_cw)
-        min_rh = int(self.min_rh)
-        w = min_cw
+        min_column_width = int(self.min_column_width)
+        min_rh = int(self.min_row_height)
+        w = min_column_width
         h = min_rh
         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         tw, h = self.get_cell_dimensions(datarn, datacn)
         if tw > w:
             w = tw
         if h < min_rh:
             h = int(min_rh)
-        elif h > self.RI.max_rh:
-            h = int(self.RI.max_rh)
-        if w < min_cw:
-            w = int(min_cw)
-        elif w > self.CH.max_cw:
-            w = int(self.CH.max_cw)
+        elif h > self.max_row_height:
+            h = int(self.max_row_height)
+        if w < min_column_width:
+            w = int(min_column_width)
+        elif w > self.max_column_width:
+            w = int(self.max_column_width)
         cell_needs_resize_w = False
         cell_needs_resize_h = False
         if only_set_if_too_small:
             if w > self.col_positions[c + 1] - self.col_positions[c]:
                 cell_needs_resize_w = True
             if h > self.row_positions[r + 1] - self.row_positions[r]:
                 cell_needs_resize_h = True
@@ -3073,22 +3020,22 @@
             if redraw:
                 self.refresh()
                 return True
             else:
                 return False
 
     def set_all_cell_sizes_to_text(self, include_index = False):
-        min_cw = int(self.min_cw)
-        min_rh = int(self.min_rh)
-        w = min_cw
+        min_column_width = int(self.min_column_width)
+        min_rh = int(self.min_row_height)
+        w = min_column_width
         h = min_rh
         rhs = defaultdict(lambda: int(min_rh))
         cws = []
-        x = self.txt_measure_canvas.create_text(0, 0, text = "", font = self._font)
-        x2 = self.txt_measure_canvas.create_text(0, 0, text = "", font = self._hdr_font)
+        x = self.txt_measure_canvas.create_text(0, 0, text = "", font = self.table_font)
+        x2 = self.txt_measure_canvas.create_text(0, 0, text = "", font = self.header_font)
         itmcon = self.txt_measure_canvas.itemconfig
         itmbbx = self.txt_measure_canvas.bbox
         if self.all_columns_displayed:
             itercols = range(self.total_data_cols())
         else:
             itercols = self.displayed_columns
         if self.all_rows_displayed:
@@ -3096,16 +3043,16 @@
         else:
             iterrows = self.displayed_rows
         if is_iterable(self._row_index):
             for datarn in iterrows:
                 w_, h = self.RI.get_cell_dimensions(datarn)
                 if h < min_rh:
                     h = int(min_rh)
-                elif h > self.RI.max_rh:
-                    h = int(self.RI.max_rh)
+                elif h > self.max_row_height:
+                    h = int(self.max_row_height)
                 if h > rhs[datarn]:
                     rhs[datarn] = h
         for datacn in itercols:
             w, h_ = self.CH.get_cell_dimensions(datacn)
             if self.all_rows_displayed:
                 # refresh range generator if needed
                 iterrows = range(self.total_data_rows())
@@ -3113,48 +3060,47 @@
                 txt = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
                 if txt:
                     itmcon(x, text = txt)
                     b = itmbbx(x)
                     tw = b[2] - b[0] + 7
                     h = b[3] - b[1] + 5
                 else:
-                    tw = min_cw
+                    tw = min_column_width
                     h = min_rh
-                if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
-                                                              'checkbox' in self.cell_options[(datarn, datacn)]):
+                if self.get_cell_kwargs(datarn, datacn, key = 'dropdown') or self.get_cell_kwargs(datarn, datacn, key = 'checkbox'):
                     tw += self.txt_h
                 if tw > w:
                     w = tw
                 if h < min_rh:
                     h = int(min_rh)
-                elif h > self.RI.max_rh:
-                    h = int(self.RI.max_rh)
+                elif h > self.max_row_height:
+                    h = int(self.max_row_height)
                 if h > rhs[datarn]:
                     rhs[datarn] = h
-            if w < min_cw:
-                w = int(min_cw)
-            elif w > self.CH.max_cw:
-                w = int(self.CH.max_cw)
+            if w < min_column_width:
+                w = int(min_column_width)
+            elif w > self.max_column_width:
+                w = int(self.max_column_width)
             cws.append(w)
         self.txt_measure_canvas.delete(x)
         self.txt_measure_canvas.delete(x2)
         self.row_positions = list(accumulate(chain([0], (height for height in rhs.values()))))
         self.col_positions = list(accumulate(chain([0], (width for width in cws))))
         self.recreate_all_selection_boxes()
         return self.row_positions, self.col_positions
 
     def reset_col_positions(self, ncols = None):
-        colpos = int(self.default_cw)
+        colpos = int(self.default_column_width)
         if self.all_columns_displayed:
             self.col_positions = list(accumulate(chain([0], (colpos for c in range(ncols if ncols is not None else self.total_data_cols())))))
         else:
             self.col_positions = list(accumulate(chain([0], (colpos for c in range(ncols if ncols is not None else len(self.displayed_columns))))))
             
     def reset_row_positions(self, nrows = None):
-        rowpos = self.default_rh[1]
+        rowpos = self.default_row_height[1]
         if self.all_rows_displayed:
             self.row_positions = list(accumulate(chain([0], (rowpos for r in range(nrows if nrows is not None else self.total_data_rows())))))
         else:
             self.row_positions = list(accumulate(chain([0], (rowpos for r in range(nrows if nrows is not None else len(self.displayed_rows))))))
 
     def del_col_position(self, idx, deselect_all = False):
         if deselect_all:
@@ -3198,47 +3144,47 @@
             rhs[idx:idx + numrows] = []
             self.row_positions = list(accumulate(chain([0], (height for height in rhs))))
 
     def insert_col_position(self, idx = "end", width = None, deselect_all = False):
         if deselect_all:
             self.deselect("all", redraw = False)
         if width is None:
-            w = self.default_cw
+            w = self.default_column_width
         else:
             w = width
         if idx == "end" or len(self.col_positions) == idx + 1:
             self.col_positions.append(self.col_positions[-1] + w)
         else:
             idx += 1
             self.col_positions.insert(idx, self.col_positions[idx - 1] + w)
             idx += 1
             self.col_positions[idx:] = [e + w for e in islice(self.col_positions, idx, len(self.col_positions))]
             
     def insert_row_position(self, idx, height = None, deselect_all = False):
         if deselect_all:
             self.deselect("all", redraw = False)
         if height is None:
-            h = self.default_rh[1]
+            h = self.default_row_height[1]
         else:
             h = height
         if idx == "end" or len(self.row_positions) == idx + 1:
             self.row_positions.append(self.row_positions[-1] + h)
         else:
             idx += 1
             self.row_positions.insert(idx, self.row_positions[idx - 1] + h)
             idx += 1
             self.row_positions[idx:] = [e + h for e in islice(self.row_positions, idx, len(self.row_positions))]
 
     def insert_col_positions(self, idx = "end", widths = None, deselect_all = False):
         if deselect_all:
             self.deselect("all", redraw = False)
         if widths is None:
-            w = [self.default_cw]
+            w = [self.default_column_width]
         elif isinstance(widths, int):
-            w = list(repeat(self.default_cw, widths))
+            w = list(repeat(self.default_column_width, widths))
         else:
             w = widths
         if idx == "end" or len(self.col_positions) == idx + 1:
             if len(w) > 1:
                 self.col_positions += list(accumulate(chain([self.col_positions[-1] + w[0]], islice(w, 1, None))))
             else:
                 self.col_positions.append(self.col_positions[-1] + w[0])
@@ -3256,17 +3202,17 @@
                 idx += 1
                 self.col_positions[idx:] = [e + w for e in islice(self.col_positions, idx, len(self.col_positions))]
 
     def insert_row_positions(self, idx = "end", heights = None, deselect_all = False):
         if deselect_all:
             self.deselect("all", redraw = False)
         if heights is None:
-            h = [self.default_rh[1]]
+            h = [self.default_row_height[1]]
         elif isinstance(heights, int):
-            h = list(repeat(self.default_rh[1], heights))
+            h = list(repeat(self.default_row_height[1], heights))
         else:
             h = heights
         if idx == "end" or len(self.row_positions) == idx + 1:
             if len(h) > 1:
                 self.row_positions += list(accumulate(chain([self.row_positions[-1] + h[0]], islice(h, 1, None))))
             else:
                 self.row_positions.append(self.row_positions[-1] + h[0])
@@ -3280,15 +3226,15 @@
             else:
                 h = h[0]
                 idx += 1
                 self.row_positions.insert(idx, self.row_positions[idx - 1] + h)
                 idx += 1
                 self.row_positions[idx:] = [e + h for e in islice(self.row_positions, idx, len(self.row_positions))]
 
-    def insert_col_rc(self, event = None):
+    def insert_cols_rc(self, event = None):
         if self.anything_selected(exclude_rows = True, exclude_cells = True):
             selcols = self.get_selected_cols()
             numcols = len(selcols)
             displayed_ins_col = min(selcols) if event == "left" else max(selcols) + 1
             if self.all_columns_displayed:
                 data_ins_col = int(displayed_ins_col)
             else:
@@ -3321,224 +3267,234 @@
                 if displayed_ins_col > len(self.displayed_columns) - 1:
                     adj_ins = displayed_ins_col - 1
                 else:
                     adj_ins = displayed_ins_col
                 part1 = self.displayed_columns[:adj_ins]
                 part2 = list(range(self.displayed_columns[adj_ins], self.displayed_columns[adj_ins] + numcols + 1))
                 part3 = [] if displayed_ins_col > len(self.displayed_columns) - 1 else [cn + numcols for cn in islice(self.displayed_columns, adj_ins + 1, None)]
-                self.displayed_columns = (part1 +
-                                          part2 +
-                                          part3)
+                self.displayed_columns = part1 + part2 + part3
         self.insert_col_positions(idx = displayed_ins_col,
                                   widths = numcols,
                                   deselect_all = True)
         self.cell_options = {(rn, cn if cn < data_ins_col else cn + numcols): t2 for (rn, cn), t2 in self.cell_options.items()}
         self.col_options = {cn if cn < data_ins_col else cn + numcols: t for cn, t in self.col_options.items()}
         self.CH.cell_options = {cn if cn < data_ins_col else cn + numcols: t for cn, t in self.CH.cell_options.items()}
+        self.CH.fix_header()
         if self._headers and isinstance(self._headers, list):
-            try:
-                self._headers[data_ins_col:data_ins_col] = list(repeat("", numcols))
-            except:
-                pass
+            if data_ins_col >= len(self._headers):
+                self.CH.fix_header(datacn = data_ins_col, fix_values = (data_ins_col, data_ins_col + numcols))
+            else:
+                self._headers[data_ins_col:data_ins_col] = self.CH.get_empty_header_seq(end = data_ins_col + numcols, start = data_ins_col, c_ops = False)
         if self.row_positions == [0] and not self.data:
             self.insert_row_position(idx = "end",
-                                     height = int(self.min_rh),
+                                     height = int(self.min_row_height),
                                      deselect_all = False)
-            self.data.append(list(repeat("", numcols)))
+            self.data.append(self.get_empty_row_seq(0, end = data_ins_col + numcols, start = data_ins_col, c_ops = False))
         else:
+            end = data_ins_col + numcols
             for rn in range(len(self.data)):
-                self.data[rn][data_ins_col:data_ins_col] = list(repeat("", numcols))
+                self.data[rn][data_ins_col:data_ins_col] = self.get_empty_row_seq(rn, end, data_ins_col, c_ops = False)
         self.create_selected(0, displayed_ins_col, len(self.row_positions) - 1, displayed_ins_col + numcols, "columns")
         self.create_current(0, displayed_ins_col, "column", inside = True)
         if self.undo_enabled:
-            self.undo_storage.append(zlib.compress(pickle.dumps(("insert_col", {"data_col_num": data_ins_col,
-                                                                                "displayed_columns": saved_displayed_columns,
-                                                                                "sheet_col_num": displayed_ins_col,
-                                                                                "numcols": numcols}))))
+            self.undo_storage.append(zlib.compress(pickle.dumps(("insert_cols", {"data_col_num": data_ins_col,
+                                                                                 "displayed_columns": saved_displayed_columns,
+                                                                                 "sheet_col_num": displayed_ins_col,
+                                                                                 "numcols": numcols}))))
         self.refresh()
         if self.extra_end_insert_cols_rc_func is not None:
             self.extra_end_insert_cols_rc_func(InsertEvent("end_insert_columns", data_ins_col, displayed_ins_col, numcols))
-        self.event_generate("<<SheetDataChangeEvent>>")
+        self.parentframe.emit_modified_event()
 
-    def insert_row_rc(self, event = None):
+    def insert_rows_rc(self, event = None):
         if self.anything_selected(exclude_columns = True, exclude_cells = True):
             selrows = self.get_selected_rows()
             numrows = len(selrows)
-            stidx = min(selrows) if event == "above" else max(selrows) + 1
-            posidx = int(stidx)
+            displayed_ins_row = min(selrows) if event == "above" else max(selrows) + 1
+            if self.all_rows_displayed:
+                data_ins_row = int(displayed_ins_row)
+            else:
+                if displayed_ins_row == len(self.row_positions) - 1:
+                    datalen = len(self.data)
+                    data_ins_row = datalen
+                else:
+                    try:
+                        data_ins_row = int(self.displayed_rows[displayed_ins_row])
+                    except:
+                        data_ins_row = int(self.displayed_rows[displayed_ins_row - 1])
         else:
-            selrows = [0]
             numrows = 1
-            stidx = self.total_data_rows()
-            posidx = len(self.row_positions) - 1
-        if isinstance(self.paste_insert_row_limit, int) and self.paste_insert_row_limit < posidx + numrows:
+            displayed_ins_row = len(self.row_positions) - 1
+            data_ins_row = int(displayed_ins_row)
+        if isinstance(self.paste_insert_row_limit, int) and self.paste_insert_row_limit < displayed_ins_row + numrows:
             numrows = self.paste_insert_row_limit - len(self.row_positions) - 1
             if numrows < 1:
                 return
         if self.extra_begin_insert_rows_rc_func is not None:
             try:
-                self.extra_begin_insert_rows_rc_func(InsertEvent("begin_insert_rows", stidx, posidx, numrows))
+                self.extra_begin_insert_rows_rc_func(InsertEvent("begin_insert_rows", data_ins_row, displayed_ins_row, numrows))
             except:
                 return
-        self.insert_row_positions(idx = posidx,
+        saved_displayed_rows = list(self.displayed_rows)
+        if not self.all_rows_displayed:
+            if displayed_ins_row == len(self.row_positions) - 1:
+                self.displayed_rows += list(range(datalen, datalen + numrows))
+            else:
+                if displayed_ins_row > len(self.displayed_rows) - 1:
+                    adj_ins = displayed_ins_row - 1
+                else:
+                    adj_ins = displayed_ins_row
+                part1 = self.displayed_rows[:adj_ins]
+                part2 = list(range(self.displayed_rows[adj_ins], self.displayed_rows[adj_ins] + numrows + 1))
+                part3 = [] if displayed_ins_row > len(self.displayed_rows) - 1 else [rn + numrows for rn in islice(self.displayed_rows, adj_ins + 1, None)]
+                self.displayed_rows = part1 + part2 + part3
+        self.insert_row_positions(idx = displayed_ins_row,
                                   heights = numrows,
                                   deselect_all = True)
-        self.cell_options = {(rn if rn < posidx else rn + numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items()}
-        self.row_options = {rn if rn < posidx else rn + numrows: t for rn, t in self.row_options.items()}
-        self.RI.cell_options = {rn if rn < posidx else rn + numrows: t for rn, t in self.RI.cell_options.items()}
+        self.cell_options = {(rn if rn < data_ins_row else rn + numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items()}
+        self.row_options = {rn if rn < data_ins_row else rn + numrows: t for rn, t in self.row_options.items()}
+        self.RI.cell_options = {rn if rn < data_ins_row else rn + numrows: t for rn, t in self.RI.cell_options.items()}
+        self.RI.fix_index()
         if self._row_index and isinstance(self._row_index, list):
-            try:
-                self._row_index[stidx:stidx] = list(repeat("", numrows))
-            except:
-                pass
+            if data_ins_row >= len(self._row_index):
+                self.RI.fix_index(datacn = data_ins_row, fix_values = (data_ins_row, data_ins_row + numrows))
+            else:
+                self._row_index[data_ins_row:data_ins_row] = self.RI.get_empty_index_seq(data_ins_row + numrows, data_ins_row, r_ops = False)
         if self.col_positions == [0] and not self.data:
             self.insert_col_position(idx = "end",
                                      width = None,
                                      deselect_all = False)
-            self.data.append([""])
+            self.data.append(self.get_empty_row_seq(0, end = data_ins_row + numrows, start = data_ins_row, r_ops = False))
         else:
             total_data_cols = self.total_data_cols()
-            self.data[stidx:stidx] = [list(repeat("", total_data_cols)) for rn in range(numrows)]
-        self.create_selected(posidx, 0, posidx + numrows, len(self.col_positions) - 1, "rows")
-        self.create_current(posidx, 0, "row", inside = True)
+            self.data[data_ins_row:data_ins_row] = [self.get_empty_row_seq(rn, total_data_cols, r_ops = False) for rn in range(data_ins_row, data_ins_row + numrows)]
+        self.create_selected(displayed_ins_row, 0, displayed_ins_row + numrows, len(self.col_positions) - 1, "rows")
+        self.create_current(displayed_ins_row, 0, "row", inside = True)
         if self.undo_enabled:
-            self.undo_storage.append(zlib.compress(pickle.dumps(("insert_row", {"data_row_num": stidx,
-                                                                                "sheet_row_num": posidx,
-                                                                                "numrows": numrows}))))
+            self.undo_storage.append(zlib.compress(pickle.dumps(("insert_rows", {"data_row_num": data_ins_row,
+                                                                                 "displayed_rows": saved_displayed_rows,
+                                                                                 "sheet_row_num": displayed_ins_row,
+                                                                                 "numrows": numrows}))))
         self.refresh()
         if self.extra_end_insert_rows_rc_func is not None:
-            self.extra_end_insert_rows_rc_func(InsertEvent("end_insert_rows", stidx, posidx, numrows))
-        self.event_generate("<<SheetDataChangeEvent>>")
-            
+            self.extra_end_insert_rows_rc_func(InsertEvent("end_insert_rows", data_ins_row, displayed_ins_row, numrows))
+        self.parentframe.emit_modified_event()
+
     def del_cols_rc(self, event = None):
         seld_cols = sorted(self.get_selected_cols())
-        if seld_cols:
-            if self.extra_begin_del_cols_rc_func is not None:
-                try:
-                    self.extra_begin_del_cols_rc_func(DeleteRowColumnEvent("begin_delete_columns", seld_cols))
-                except:
-                    return
-            seldset = set(seld_cols) if self.all_columns_displayed else set(self.displayed_columns[c] for c in seld_cols)
-            list_of_coords = tuple((r, c) for (r, c) in self.cell_options if c in seldset)
-            if self.undo_enabled:
-                undo_storage = {'deleted_cols': {},
-                                'colwidths': {},
-                                'deleted_hdr_values': {},
-                                'selection_boxes': self.get_boxes(),
-                                'displayed_columns': list(self.displayed_columns) if not isinstance(self.displayed_columns, int) else int(self.displayed_columns),
-                                'cell_options': {k: v.copy() for k, v in self.cell_options.items()},
-                                'col_options': {k: v.copy() for k, v in self.col_options.items()},
-                                'CH_cell_options': {k: v.copy() for k, v in self.CH.cell_options.items()}}
-                for c in reversed(seld_cols):
-                    undo_storage['colwidths'][c] = self.col_positions[c + 1] - self.col_positions[c]
-                    datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                    for rn in range(len(self.data)):
-                        if datacn not in undo_storage['deleted_cols']:
-                            undo_storage['deleted_cols'][datacn] = {}
-                        try:
-                            undo_storage['deleted_cols'][datacn][rn] = self.data[rn].pop(datacn)
-                        except:
-                            continue
-                    try:
-                        undo_storage['deleted_hdr_values'][datacn] = self._headers.pop(datacn)
-                    except:
-                        continue
-            else:
-                for c in reversed(seld_cols):
-                    datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                    for rn in range(len(self.data)):
-                        del self.data[rn][datacn]
+        if not seld_cols:
+            return
+        if self.extra_begin_del_cols_rc_func is not None:
+            try:
+                self.extra_begin_del_cols_rc_func(DeleteRowColumnEvent("begin_delete_columns", seld_cols))
+            except:
+                return
+        seldset = set(seld_cols) if self.all_columns_displayed else set(self.displayed_columns[c] for c in seld_cols)
+        if self.undo_enabled:
+            undo_storage = {'deleted_cols': {},
+                            'colwidths': {},
+                            'deleted_header_values': {},
+                            'selection_boxes': self.get_boxes(),
+                            'displayed_columns': list(self.displayed_columns) if not isinstance(self.displayed_columns, int) else int(self.displayed_columns),
+                            'cell_options': {k: v.copy() for k, v in self.cell_options.items()},
+                            'col_options': {k: v.copy() for k, v in self.col_options.items()},
+                            'CH_cell_options': {k: v.copy() for k, v in self.CH.cell_options.items()}}
+            for c in reversed(seld_cols):
+                undo_storage['colwidths'][c] = self.col_positions[c + 1] - self.col_positions[c]
+                datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                for rn in range(len(self.data)):
+                    if datacn not in undo_storage['deleted_cols']:
+                        undo_storage['deleted_cols'][datacn] = {}
                     try:
-                        del self._headers[datacn]
+                        undo_storage['deleted_cols'][datacn][rn] = self.data[rn].pop(datacn)
                     except:
                         continue
-            if self.undo_enabled:
-                self.undo_storage.append(("delete_cols", undo_storage))
-            self.del_cell_options(list_of_coords)
+                try:
+                    undo_storage['deleted_header_values'][datacn] = self._headers.pop(datacn)
+                except:
+                    continue
+        else:
             for c in reversed(seld_cols):
                 datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                self.del_col_position(c,
-                                      deselect_all = False)
-                if datacn in self.col_options:
-                    del self.col_options[datacn]
-                if datacn in self.CH.cell_options:
-                    del self.CH.cell_options[datacn]
-            numcols = len(seld_cols)
-            idx = seld_cols[-1]
-            self.cell_options = {(rn, cn if cn < idx else cn - numcols): t2 for (rn, cn), t2 in self.cell_options.items()}
-            self.col_options = {cn if cn < idx else cn - numcols: t for cn, t in self.col_options.items()}
-            self.CH.cell_options = {cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items()}
-            self.deselect("allcols", redraw = False)
-            self.set_current_to_last()
-            if not self.all_columns_displayed:
-                self.displayed_columns = [c for c in self.displayed_columns if c not in seldset]
-                for c in sorted(seldset):
-                    self.displayed_columns = [dc if c > dc else dc - 1 for dc in self.displayed_columns]
-            self.refresh()
-            if self.extra_end_del_cols_rc_func is not None:
-                self.extra_end_del_cols_rc_func(DeleteRowColumnEvent("end_delete_columns", seld_cols))
-            self.event_generate('<<SheetDataChangeEvent>>')
+                for rn in range(len(self.data)):
+                    del self.data[rn][datacn]
+                try:
+                    del self._headers[datacn]
+                except:
+                    continue
+        if self.undo_enabled:
+            self.undo_storage.append(("delete_cols", undo_storage))
+        for c in reversed(seld_cols):
+            self.del_col_position(c, deselect_all = False)
+        numcols = len(seld_cols)
+        idx = seld_cols[-1]
+        self.cell_options = {(rn, cn if cn < idx else cn - numcols): t2 for (rn, cn), t2 in self.cell_options.items() if cn not in seldset}
+        self.col_options = {cn if cn < idx else cn - numcols: t for cn, t in self.col_options.items() if cn not in seldset}
+        self.CH.cell_options = {cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items() if cn not in seldset}
+        self.deselect("allcols", redraw = False)
+        self.set_current_to_last()
+        if not self.all_columns_displayed:
+            self.displayed_columns = [c for c in self.displayed_columns if c not in seldset]
+            for c in sorted(seldset):
+                self.displayed_columns = [dc if c > dc else dc - 1 for dc in self.displayed_columns]
+        self.refresh()
+        if self.extra_end_del_cols_rc_func is not None:
+            self.extra_end_del_cols_rc_func(DeleteRowColumnEvent("end_delete_columns", seld_cols))
+        self.parentframe.emit_modified_event()
 
     def del_rows_rc(self, event = None):
         seld_rows = sorted(self.get_selected_rows())
-        if seld_rows:
-            if self.extra_begin_del_rows_rc_func is not None:
+        if not seld_rows:
+            return
+        if self.extra_begin_del_rows_rc_func is not None:
+            try:
+                self.extra_begin_del_rows_rc_func(DeleteRowColumnEvent("begin_delete_rows", seld_rows))
+            except:
+                return
+        seldset = set(seld_rows) if self.all_rows_displayed else set(self.displayed_rows[r] for r in seld_rows)
+        if self.undo_enabled:
+            undo_storage = {'deleted_rows': [],
+                            'rowheights': {},
+                            'deleted_index_values': [],
+                            'selection_boxes': self.get_boxes(),
+                            'displayed_rows': list(self.displayed_rows) if not isinstance(self.displayed_rows, int) else int(self.displayed_rows),
+                            'cell_options': {k: v.copy() for k, v in self.cell_options.items()},
+                            'row_options': {k: v.copy() for k, v in self.row_options.items()},
+                            'RI_cell_options': {k: v.copy() for k, v in self.RI.cell_options.items()}}
+            for r in reversed(seld_rows):
+                undo_storage['rowheights'][r] = self.row_positions[r + 1] - self.row_positions[r]
+                datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+                undo_storage['deleted_rows'].append((datarn, self.data.pop(datarn)))
                 try:
-                    self.extra_begin_del_rows_rc_func(DeleteRowColumnEvent("begin_delete_rows", seld_rows))
+                    undo_storage['deleted_index_values'].append((datarn, self._row_index.pop(datarn)))
                 except:
-                    return
-            seldset = set(seld_rows) if self.all_rows_displayed else set(self.displayed_rows[r] for r in seld_rows)
-            list_of_coords = tuple((r, c) for (r, c) in self.cell_options if r in seldset)
-            if self.undo_enabled:
-                undo_storage = {'deleted_rows': [],
-                                'rowheights': {},
-                                'deleted_index_values': [],
-                                'selection_boxes': self.get_boxes(),
-                                'displayed_rows': list(self.displayed_rows) if not isinstance(self.displayed_rows, int) else int(self.displayed_rows),
-                                'cell_options': {k: v.copy() for k, v in self.cell_options.items()},
-                                'row_options': {k: v.copy() for k, v in self.row_options.items()},
-                                'RI_cell_options': {k: v.copy() for k, v in self.RI.cell_options.items()}}
-                for r in reversed(seld_rows):
-                    undo_storage['rowheights'][r] = self.row_positions[r + 1] - self.row_positions[r]
-                    datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-                    undo_storage['deleted_rows'].append((datarn, self.data.pop(datarn)))
-                    try:
-                        undo_storage['deleted_index_values'].append((datarn, self._row_index.pop(datarn)))
-                    except:
-                        continue
-            else:
-                for r in reversed(seld_rows):
-                    datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-                    del self.data[datarn]
-                    try:
-                        del self._row_index[datarn]
-                    except:
-                        continue
-            if self.undo_enabled:
-                self.undo_storage.append(("delete_rows", undo_storage))
-            self.del_cell_options(list_of_coords)
+                    continue
+        else:
             for r in reversed(seld_rows):
                 datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-                self.del_row_position(r,
-                                      deselect_all = False)
-                if datarn in self.row_options:
-                    del self.row_options[datarn]
-                if datarn in self.RI.cell_options:
-                    del self.RI.cell_options[datarn]
-            numrows = len(seld_rows)
-            idx = seld_rows[-1] if self.all_rows_displayed else self.displayed_rows[seld_rows[-1]]
-            self.cell_options = {(rn if rn < idx else rn - numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items()}
-            self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items()}
-            self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items()}
-            self.deselect("allrows", redraw = False)
-            self.set_current_to_last()
-            self.refresh()
-            if self.extra_end_del_rows_rc_func is not None:
-                self.extra_end_del_rows_rc_func(DeleteRowColumnEvent("end_delete_rows", seld_rows))
-            self.event_generate('<<SheetDataChangeEvent>>')
+                del self.data[datarn]
+                try:
+                    del self._row_index[datarn]
+                except:
+                    continue
+        if self.undo_enabled:
+            self.undo_storage.append(("delete_rows", undo_storage))
+        for r in reversed(seld_rows):
+            self.del_row_position(r, deselect_all = False)
+        numrows = len(seld_rows)
+        idx = seld_rows[-1] if self.all_rows_displayed else self.displayed_rows[seld_rows[-1]]
+        self.cell_options = {(rn if rn < idx else rn - numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items() if rn not in seldset}
+        self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items() if rn not in seldset}
+        self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items() if rn not in seldset}
+        self.deselect("allrows", redraw = False)
+        self.set_current_to_last()
+        self.refresh()
+        if self.extra_end_del_rows_rc_func is not None:
+            self.extra_end_del_rows_rc_func(DeleteRowColumnEvent("end_delete_rows", seld_rows))
+        self.parentframe.emit_modified_event()
 
     def move_row_position(self, idx1, idx2):
         if not len(self.row_positions) <= 2:
             if idx1 < idx2:
                 height = self.row_positions[idx1 + 1] - self.row_positions[idx1]
                 self.row_positions.insert(idx2 + 1, self.row_positions.pop(idx1 + 1))
                 for i in range(idx1 + 1, idx2 + 1):
@@ -3615,26 +3571,26 @@
     def headers(self, newheaders = None, index = None, reset_col_positions = False, show_headers_if_not_sheet = True, redraw = False):
         if newheaders is not None:
             if isinstance(newheaders, (list, tuple)):
                 self._headers = list(newheaders) if isinstance(newheaders, tuple) else newheaders
             elif isinstance(newheaders, int):
                 self._headers = int(newheaders)
             elif isinstance(self._headers, list) and isinstance(index, int):
-                if len(self._headers) <= index:
-                    self._headers.extend(list(repeat("", index - len(self._headers) + 1)))
+                if index >= len(self._headers):
+                    self.CH.fix_header(index)
                 self._headers[index] = f"{newheaders}"
             elif not isinstance(newheaders, (list, tuple, int)) and index is None:
                 try:
                     self._headers = list(newheaders)
                 except:
                     raise ValueError("New header must be iterable or int (use int to use a row as the header")
             if reset_col_positions:
                 self.reset_col_positions()
             elif show_headers_if_not_sheet and isinstance(self._headers, list) and (self.col_positions == [0] or not self.col_positions):
-                colpos = int(self.default_cw)
+                colpos = int(self.default_column_width)
                 if self.all_columns_displayed:
                     self.col_positions = list(accumulate(chain([0], (colpos for c in range(len(self._headers))))))
                 else:
                     self.col_positions = list(accumulate(chain([0], (colpos for c in range(len(self.displayed_columns))))))
             if redraw:
                 self.refresh()
         else:
@@ -3642,32 +3598,32 @@
                 return self._headers[index]
             else:
                 return self._headers
 
     def row_index(self, newindex = None, index = None, reset_row_positions = False, show_index_if_not_sheet = True, redraw = False):
         if newindex is not None:
             if not self._row_index and not isinstance(self._row_index, int):
-                self.RI.set_width(self.RI.default_width, set_TL = True)
+                self.RI.set_width(self.default_index_width, set_TL = True)
             if isinstance(newindex, (list, tuple)):
                 self._row_index = list(newindex) if isinstance(newindex, tuple) else newindex
             elif isinstance(newindex, int):
                 self._row_index = int(newindex)
             elif isinstance(index, int):
-                if len(self._row_index) <= index:
-                    self._row_index.extend(list(repeat("", index - len(self._row_index) + 1)))
+                if index >= len(self._row_index):
+                    self.RI.fix_index(index)
                 self._row_index[index] = f"{newindex}"
             elif not isinstance(newindex, (list, tuple, int)) and index is None:
                 try:
                     self._row_index = list(newindex)
                 except:
                     raise ValueError("New index must be iterable or int (use int to use a column as the index")
             if reset_row_positions:
                 self.reset_row_positions()
             elif show_index_if_not_sheet and isinstance(self._row_index, list) and (self.row_positions == [0] or not self.row_positions):
-                rowpos = self.default_rh[1]
+                rowpos = self.default_row_height[1]
                 if self.all_rows_displayed:
                     self.row_positions = list(accumulate(chain([0], (rowpos for r in range(len(self._row_index))))))
                 else:
                     self.row_positions = list(accumulate(chain([0], (rowpos for r in range(len(self.displayed_rows))))))
                 
             if redraw:
                 self.refresh()
@@ -3699,29 +3655,26 @@
         return i_total if i_total > d_total else d_total
 
     def data_dimensions(self, total_rows = None, total_columns = None):
         if total_rows is None and total_columns is None:
             return self.total_data_rows(), self.total_data_cols()
         if total_rows is not None:
             if len(self.data) < total_rows:
-                if total_columns is None:
-                    total_data_cols = self.total_data_cols()
-                    self.data.extend([list(repeat("", total_data_cols)) for r in range(total_rows - len(self.data))])
-                else:
-                    self.data.extend([list(repeat("", total_columns)) for r in range(total_rows - len(self.data))])
+                ncols = self.total_data_cols() if total_columns is None else total_columns
+                self.data.extend([self.get_empty_row_seq(r, ncols) for r in range(total_rows - len(self.data))])
             else:
                 self.data[total_rows:] = []
         if total_columns is not None:
-            self.data[:] = [r[:total_columns] if len(r) > total_columns else r + list(repeat("", total_columns - len(r))) for r in self.data]
+            self.data[:] = [r[:total_columns] if len(r) > total_columns else r + self.get_empty_row_seq(rn, end = len(r) + total_columns, start = len(r)) for rn, r in enumerate(self.data)]
 
-    def equalize_data_row_lengths(self, include_header = False):
-        total_columns = self.total_data_cols()
+    def equalize_data_row_lengths(self, include_header = False, total_columns = None):
+        total_columns = self.total_data_cols() if total_columns is None else total_columns
         if include_header and total_columns > len(self._headers):
-            self._headers[:] = self._headers + list(repeat("", total_columns - len(self._headers)))
-        self.data[:] = [r + list(repeat("", total_columns - len(r))) if total_columns > len(r) else r for r in self.data]
+            self.CH.fix_header(total_columns)
+        self.data[:] = [(r + self.get_empty_row_seq(rn, end = len(r) + total_columns, start = len(r))) if total_columns > len(r) else r for rn, r in enumerate(self.data)]
         return total_columns
 
     def get_canvas_visible_area(self):
         return self.canvasx(0), self.canvasy(0), self.canvasx(self.winfo_width()), self.canvasy(self.winfo_height())
 
     def get_visible_rows(self, y1, y2):
         start_row = bisect.bisect_left(self.row_positions, y1)
@@ -3735,144 +3688,48 @@
         end_col = bisect.bisect_right(self.col_positions, x2)
         if not x2 >= self.col_positions[-1]:
             end_col += 1
         return start_col, end_col
 
     def redraw_highlight_get_text_fg(self, r, c, fc, fr, sc, sr, c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, datarn, datacn, can_width):
         redrawn = False
-        # ________________________ CELL IS HIGHLIGHTED AND IN SELECTED CELLS ________________________
-        if (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and (r, c) in selected_cells:
-            tf = self.table_selected_cells_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(datarn, datacn)]['highlight'][1]
-            if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
-                c_1 = self.cell_options[(datarn, datacn)]['highlight'][0] if self.cell_options[(datarn, datacn)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(datarn, datacn)]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"), 
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
-                                                tag = "hi")
-            
-        elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and (r, c) in selected_cells:
-            tf = self.table_selected_cells_fg if self.row_options[datarn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[datarn]['highlight'][1]
-            if self.row_options[datarn]['highlight'][0] is not None:
-                c_1 = self.row_options[datarn]['highlight'][0] if self.row_options[datarn]['highlight'][0].startswith("#") else Color_Map_[self.row_options[datarn]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
-                                                tag = "hi",
-                                                can_width = can_width if self.row_options[datarn]['highlight'][2] else None)
-            
-        elif datacn in self.col_options and 'highlight' in self.col_options[datacn] and (r, c) in selected_cells:
-            tf = self.table_selected_cells_fg if self.col_options[datacn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[datacn]['highlight'][1]
-            if self.col_options[datacn]['highlight'][0] is not None:
-                c_1 = self.col_options[datacn]['highlight'][0] if self.col_options[datacn]['highlight'][0].startswith("#") else Color_Map_[self.col_options[datacn]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
-                                                tag = "hi")
-            
-        # ________________________ CELL IS HIGHLIGHTED AND IN SELECTED ROWS ________________________
-        elif (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and r in actual_selected_rows:
-            tf = self.table_selected_rows_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(datarn, datacn)]['highlight'][1]
-            if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
-                c_1 = self.cell_options[(datarn, datacn)]['highlight'][0] if self.cell_options[(datarn, datacn)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(datarn, datacn)]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_4_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
-                                                tag = "hi")
-            
-        elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and r in actual_selected_rows:
-            tf = self.table_selected_rows_fg if self.row_options[datarn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[datarn]['highlight'][1]
-            if self.row_options[datarn]['highlight'][0] is not None:
-                c_1 = self.row_options[datarn]['highlight'][0] if self.row_options[datarn]['highlight'][0].startswith("#") else Color_Map_[self.row_options[datarn]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_4_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
-                                                tag = "hi",
-                                                can_width = can_width if self.row_options[r]['highlight'][2] else None)
-            
-        elif datacn in self.col_options and 'highlight' in self.col_options[datacn] and r in actual_selected_rows:
-            tf = self.table_selected_rows_fg if self.col_options[datacn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[datacn]['highlight'][1]
-            if self.col_options[datacn]['highlight'][0] is not None:
-                c_1 = self.col_options[datacn]['highlight'][0] if self.col_options[datacn]['highlight'][0].startswith("#") else Color_Map_[self.col_options[datacn]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_4_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "",
-                                                tag = "hi")
-            
-        # ________________________ CELL IS HIGHLIGHTED AND IN SELECTED COLUMNS ________________________
-        elif (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and c in actual_selected_cols:
-            tf = self.table_selected_columns_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(datarn, datacn)]['highlight'][1]
-            if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
-                c_1 = self.cell_options[(datarn, datacn)]['highlight'][0] if self.cell_options[(datarn, datacn)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(datarn, datacn)]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_3_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "",
-                                                tag = "hi")
-            
-        elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and c in actual_selected_cols:
-            tf = self.table_selected_columns_fg if self.row_options[datarn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[datarn]['highlight'][1]
-            if self.row_options[datarn]['highlight'][0] is not None:
-                c_1 = self.row_options[datarn]['highlight'][0] if self.row_options[datarn]['highlight'][0].startswith("#") else Color_Map_[self.row_options[datarn]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_3_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
-                                                tag = "hi",
-                                                can_width = can_width if self.row_options[datarn]['highlight'][2] else None)
-            
-        elif datacn in self.col_options and 'highlight' in self.col_options[datacn] and c in actual_selected_cols:
-            tf = self.table_selected_columns_fg if self.col_options[datacn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[datacn]['highlight'][1]
-            if self.col_options[datacn]['highlight'][0] is not None:
-                c_1 = self.col_options[datacn]['highlight'][0] if self.col_options[datacn]['highlight'][0].startswith("#") else Color_Map_[self.col_options[datacn]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_3_[0]) / 2):02X}" +
-                                                                                f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
-                                                                                f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "",
-                                                tag = "hi")
-
-        # ________________________ CELL IS HIGHLIGHTED AND NOT SELECTED ________________________
-        elif (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
-            tf = self.table_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None else self.cell_options[(datarn, datacn)]['highlight'][1]
-            if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.cell_options[(datarn, datacn)]['highlight'][0],
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
-                                                tag = "hi")
-            
-        elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
-            tf = self.table_fg if self.row_options[datarn]['highlight'][1] is None else self.row_options[datarn]['highlight'][1]
-            if self.row_options[datarn]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.row_options[datarn]['highlight'][0],
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'highlight')
+        if kwargs:
+            if kwargs[0] is not None:
+                c_1 = kwargs[0] if kwargs[0].startswith("#") else Color_Map_[kwargs[0]]
+            if (r, c) in selected_cells:
+                tf = self.table_selected_cells_fg if kwargs[1] is None or self.display_selected_fg_over_highlights else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" + f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" + f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"
+            elif r in actual_selected_rows:
+                tf = self.table_selected_rows_fg if kwargs[1] is None or self.display_selected_fg_over_highlights else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = f"#{int((int(c_1[1:3], 16) + c_4_[0]) / 2):02X}" + f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" + f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"
+            elif c in actual_selected_cols:
+                tf = self.table_selected_columns_fg if kwargs[1] is None or self.display_selected_fg_over_highlights else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = f"#{int((int(c_1[1:3], 16) + c_3_[0]) / 2):02X}" + f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" + f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"
+            else:
+                tf = self.table_fg if kwargs[1] is None else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = kwargs[0]
+            if kwargs[0] is not None:
+                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = fill, 
+                                                outline = self.table_fg if self.get_cell_kwargs(datarn, datacn, key = 'dropdown') and self.show_dropdown_borders else "", 
                                                 tag = "hi",
-                                                can_width = can_width if self.row_options[datarn]['highlight'][2] else None)
-            
-        elif datacn in self.col_options and 'highlight' in self.col_options[datacn] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
-            tf = self.table_fg if self.col_options[datacn]['highlight'][1] is None else self.col_options[datacn]['highlight'][1]
-            if self.col_options[datacn]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.col_options[datacn]['highlight'][0],
-                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "",
-                                                tag = "hi")
-        
-        # ________________________ CELL IS JUST SELECTED ________________________
-        elif (r, c) in selected_cells:
-            tf = self.table_selected_cells_fg
-        elif r in actual_selected_rows:
-            tf = self.table_selected_rows_fg
-        elif c in actual_selected_cols:
-            tf = self.table_selected_columns_fg
-
-        # ________________________ CELL IS NOT SELECTED ________________________
-        else:
-            tf = self.table_fg
+                                                can_width = can_width if (len(kwargs) > 2 and kwargs[2]) else None)
+        elif not kwargs:
+            if (r, c) in selected_cells:
+                tf = self.table_selected_cells_fg
+            elif r in actual_selected_rows:
+                tf = self.table_selected_rows_fg
+            elif c in actual_selected_cols:
+                tf = self.table_selected_columns_fg
+            else:
+                tf = self.table_fg
         return tf, redrawn
 
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag, can_width = None, pc = None):
         config = (fill, outline)
         if type(pc) != int or pc >= 100 or pc <= 0:
             coords = (x1 - 1 if outline else x1,
                       y1 - 1 if outline else y1,
@@ -3887,46 +3744,41 @@
         if config in self.hidd_high:
             k = config
             iid, showing = self.hidd_high[k].pop()
             if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 0 if showing else 2
             else:
                 option = 1 if showing else 3
-
         elif self.hidd_high:
             k = next(iter(self.hidd_high))
             iid, showing = self.hidd_high[k].pop()
             if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 2 if showing else 3
             else:
                 option = 3
-            
         else:
             iid, showing, option = self.create_rectangle(coords, fill = fill, outline = outline, tag = tag), 1, 4
-
         if option in (1, 3):
             self.coords(iid, coords)
         if option in (2, 3):
             if showing:
                 self.itemconfig(iid, fill = fill, outline = outline)
             else:
                 self.itemconfig(iid, fill = fill, outline = outline, tag = tag, state = "normal")
-        
         if k is not None and not self.hidd_high[k]:
             del self.hidd_high[k]
-
         self.disp_high[config].add(DrawnItem(iid = iid, showing = 1))
         return True
 
     def redraw_dropdown(self, x1, y1, x2, y2, fill, outline, tag, draw_outline = True, draw_arrow = True, dd_is_open = False):
         if draw_outline and self.show_dropdown_borders:
             self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill = "", outline = self.table_fg, tag = tag)
         if draw_arrow:
             topysub = floor(self.half_txt_h / 2)
-            mid_y = y1 + floor(self.min_rh / 2)
+            mid_y = y1 + floor(self.min_row_height / 2)
             if mid_y + topysub + 1 >= y1 + self.txt_h - 1:
                 mid_y -= 1
             if mid_y - topysub + 2 <= y1 + 4 + topysub:
                 mid_y -= 1
                 ty1 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
                 ty2 = mid_y - topysub + 3 if dd_is_open else mid_y + topysub + 1
                 ty3 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
@@ -3986,15 +3838,14 @@
             else:
                 self.itemconfig(t, fill = outline, outline = fill, tag = tag, state = "normal")
             self.lift(t)
         else:
             t = self.create_polygon(points, fill = outline, outline = fill, tag = tag, smooth = True)
         self.disp_checkbox[t] = True
         if draw_check:
-            # draw filled box
             x1 = x1 + 4
             y1 = y1 + 4
             x2 = x2 - 3
             y2 = y2 - 3
             points = self.get_checkbox_points(x1, y1, x2, y2, radius = 4)
             if self.hidd_checkbox:
                 t, sh = self.hidd_checkbox.popitem()
@@ -4149,15 +4000,15 @@
         c_2_ = (int(c_2[1:3], 16), int(c_2[3:5], 16), int(c_2[5:], 16))
         c_3 = self.table_selected_columns_bg if self.table_selected_columns_bg.startswith("#") else Color_Map_[self.table_selected_columns_bg]
         c_3_ = (int(c_3[1:3], 16), int(c_3[3:5], 16), int(c_3[5:], 16))
         c_4 = self.table_selected_rows_bg if self.table_selected_rows_bg.startswith("#") else Color_Map_[self.table_selected_rows_bg]
         c_4_ = (int(c_4[1:3], 16), int(c_4[3:5], 16), int(c_4[5:], 16))
         rows_ = tuple(range(start_row, end_row))
         selected_cells, selected_rows, selected_cols, actual_selected_rows, actual_selected_cols = self.get_redraw_selections((start_row, start_col, end_row, end_col - 1))
-        font = self._font
+        font = self.table_font
         if redraw_table:
             for c in range(start_col, end_col - 1):
                 for r in rows_:
                     rtopgridln = self.row_positions[r]
                     rbotgridln = self.row_positions[r + 1]
                     if rbotgridln - rtopgridln < self.txt_h:
                         continue
@@ -4166,58 +4017,52 @@
                     
                     datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                     datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                     
                     fill, dd_drawn = self.redraw_highlight_get_text_fg(r, c, cleftgridln, rtopgridln, crightgridln, rbotgridln,
                                                                        c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, 
                                                                        datarn, datacn, can_width)
-                        
-                    if (datarn, datacn) in self.cell_options and 'align' in self.cell_options[(datarn, datacn)]:
-                        align = self.cell_options[(datarn, datacn)]['align']
-                    elif datarn in self.row_options and 'align' in self.row_options[datarn]:
-                        align = self.row_options[datarn]['align']
-                    elif datacn in self.col_options and 'align' in self.col_options[datacn]:
-                        align = self.col_options[datacn]['align']
+                    align = self.get_cell_kwargs(datarn, datacn, key = 'align')
+                    if align:
+                        align = align
                     else:
                         align = self.align
-                    
+                    kwargs = self.get_cell_kwargs(datarn, datacn, key = 'dropdown')
                     if align == "w":
                         draw_x = cleftgridln + 3
-                        if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)]:
+                        if kwargs:
                             mw = crightgridln - cleftgridln - self.txt_h - 2
                             self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
                                                 fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                                dd_is_open = self.cell_options[(datarn, datacn)]['dropdown']['window'] != "no dropdown open")
+                                                dd_is_open = kwargs['window'] != "no dropdown open")
                         else:
                             mw = crightgridln - cleftgridln - 1
-
                     elif align == "e":
-                        if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)]:
+                        if kwargs:
                             mw = crightgridln - cleftgridln - self.txt_h - 2
                             draw_x = crightgridln - 5 - self.txt_h
                             self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
                                                 fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                                dd_is_open = self.cell_options[(datarn, datacn)]['dropdown']['window'] != "no dropdown open")
+                                                dd_is_open = kwargs['window'] != "no dropdown open")
                         else:
                             mw = crightgridln - cleftgridln - 1
                             draw_x = crightgridln - 3
-
                     elif align == "center":
                         stop = cleftgridln + 5
-                        if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)]:
+                        if kwargs:
                             mw = crightgridln - cleftgridln - self.txt_h - 2
                             draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.txt_h) / 2)
                             self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
                                                 fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                                dd_is_open = self.cell_options[(datarn, datacn)]['dropdown']['window'] != "no dropdown open")
+                                                dd_is_open = kwargs['window'] != "no dropdown open")
                         else:
                             mw = crightgridln - cleftgridln - 1
                             draw_x = cleftgridln + floor((crightgridln - cleftgridln) / 2)
-
-                    if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
+                    kwargs = self.get_cell_kwargs(datarn, datacn, key = 'checkbox')
+                    if kwargs:
                         if mw > self.txt_h + 2:
                             box_w = self.txt_h + 1
                             mw -= box_w
                             if align == "w":
                                 draw_x += box_w + 1
                             elif align == "center":
                                 draw_x += ceil(box_w / 2) + 1
@@ -4228,15 +4073,15 @@
                                 draw_check = self.data[datarn][datacn]
                             except:
                                 draw_check = False
                             self.redraw_checkbox(cleftgridln + 2,
                                                  rtopgridln + 2,
                                                  cleftgridln + self.txt_h + 3,
                                                  rtopgridln + self.txt_h + 3,
-                                                 fill = fill if self.cell_options[(datarn, datacn)]['checkbox']['state'] == "normal" else self.table_grid_fg,
+                                                 fill = fill if kwargs['state'] == "normal" else self.table_grid_fg,
                                                  outline = "", tag = "cb", draw_check = draw_check)
                     lns = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True).split("\n")
                     if lns != [''] and mw > self.txt_w and not ((align == "w" and draw_x > scrollpos_right) or
                                                                 (align == "e" and cleftgridln + 5 > scrollpos_right) or
                                                                 (align == "center" and stop > scrollpos_right)):
                         draw_y = rtopgridln + self.fl_ins
                         start_ln = int((scrollpos_top - rtopgridln) / self.xtra_lines_increment)
@@ -4355,41 +4200,70 @@
         if redraw_row_index and self.show_index:
             self.RI.redraw_grid_and_text(last_row_line_pos, scrollpos_top, y_stop, start_row, end_row + 1, scrollpos_bot, selected_rows, actual_selected_cols, actual_selected_rows, row_pos_exists)
         return True
 
     def get_all_selection_items(self):
         return sorted(self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill") + self.find_withtag("Current_Inside") + self.find_withtag("Current_Outside"))
 
-    def get_boxes(self):
+    def get_boxes(self, include_current = True):
         boxes = {}
         for item in self.get_all_selection_items():
             alltags = self.gettags(item)
             if alltags[0] == "CellSelectFill":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "cells"
             elif alltags[0] == "RowSelectFill":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "rows"
             elif alltags[0] == "ColSelectFill":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "columns"
-            elif alltags[0] == "Current_Inside":
+            elif include_current and alltags[0] == "Current_Inside":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = f"{alltags[2]}_inside"
-            elif alltags[0] == "Current_Outside":
+            elif include_current and alltags[0] == "Current_Outside":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = f"{alltags[2]}_outside"
         return boxes
 
     def reselect_from_get_boxes(self, boxes):
-        for k, v in boxes.items():
-            if v == "cells":
-                self.create_selected(k[0], k[1], k[2], k[3], "cells")
-            elif v == "rows":
-                self.create_selected(k[0], k[1], k[2], k[3], "rows")
-            elif v == "columns":
-                self.create_selected(k[0], k[1], k[2], k[3], "columns")
-            elif v in ("cell_inside", "cell_outside", "row_inside", "row_outside", "col_outside", "col_inside"): #currently selected
-                x = v.split("_")
-                self.create_current(k[0], k[1], type_ = x[0], inside = True if x[1] == "inside" else False)
+        for (r1, c1, r2, c2), v in boxes.items():
+            if r2 < len(self.row_positions) and c2 < len(self.col_positions):
+                if v == "cells":
+                    self.create_selected(r1, c1, r2, c2, "cells")
+                elif v == "rows":
+                    self.create_selected(r1, c1, r2, c2, "rows")
+                elif v == "columns":
+                    self.create_selected(r1, c1, r2, c2, "columns")
+                elif v in ("cell_inside", "cell_outside", "row_inside", "row_outside", "col_outside", "col_inside"): #currently selected
+                    x = v.split("_")
+                    self.create_current(r1, c1, type_ = x[0], inside = True if x[1] == "inside" else False)
+                
+    def delete_selected(self, r1 = None, c1 = None, r2 = None, c2 = None, type_ = None):
+        deleted_boxes = {}
+        tags_to_del = set()
+        box1 = (r1, c1, r2, c2)
+        for s in self.get_selection_tags_from_type(type_):
+            for item in self.find_withtag(s):
+                alltags = self.gettags(item)
+                if alltags:
+                    box2 = tuple(int(e) for e in alltags[1].split("_") if e)
+                    if box1 == box2:
+                        tags_to_del.add(alltags)
+                        deleted_boxes[box2] = "cells" if alltags[0].startswith("Cell") else "rows" if alltags[0].startswith("Row") else "columns"
+                        self.delete(item)
+        for canvas in (self.RI, self.CH):
+            for item in canvas.find_withtag(s):
+                if canvas.gettags(item) in tags_to_del:
+                    canvas.delete(item)
+
+    def get_selection_tags_from_type(self, type_):
+        if type_ == "cells":
+            return {"CellSelectFill", "CellSelectBorder"}
+        if type_ == "rows":
+            return {"RowSelectFill", "RowSelectBorder"}
+        elif type_ == "columns":
+            return {"ColSelectFill", "ColSelectBorder"}
+        else:
+            return {"CellSelectFill", "CellSelectBorder", "RowSelectFill", "RowSelectBorder", "ColSelectFill", "ColSelectBorder"}             
 
     def delete_selection_rects(self, cells = True, rows = True, cols = True, delete_current = True):
         deleted_boxes = {}
         if cells:
             for item in self.find_withtag("CellSelectFill"):
                 alltags = self.gettags(item)
                 if alltags:
@@ -4548,15 +4422,15 @@
         self.CH.create_rectangle(self.col_positions[c1],
                                  0,
                                  self.col_positions[c2],
                                  self.CH.current_height - 1,
                                  fill = self.CH.header_selected_columns_bg if type_ == "columns" else self.CH.header_selected_cells_bg,
                                  outline = "",
                                  tags = tagr)
-        if self.show_selected_cells_border and self.being_drawn_rect is None and self.RI.being_drawn_rect is None and self.CH.being_drawn_rect is None:
+        if self.show_selected_cells_border and ((self.being_drawn_rect is None and self.RI.being_drawn_rect is None and self.CH.being_drawn_rect is None) or len(self.anything_selected()) > 1):
             b = self.create_rectangle(self.col_positions[c1], self.row_positions[r1], self.col_positions[c2], self.row_positions[r2],
                                       fill = "",
                                       outline = mt_border_col,
                                       tags = tagb)
         else:
             b = None
         if taglower:
@@ -4948,37 +4822,31 @@
             r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if r1 <= r and r2 > r:
                 return True
         return False
 
     def anything_selected(self, exclude_columns = False, exclude_rows = False, exclude_cells = False):
         if exclude_columns and exclude_rows and not exclude_cells:
-            if self.find_withtag("CellSelectFill") or self.find_withtag("Current_Outside"):
-                return True
+            return self.find_withtag("CellSelectFill") + self.find_withtag("Current_Outside")
         elif exclude_columns and exclude_cells and not exclude_rows:
-            if self.find_withtag("RowSelectFill"):
-                return True
+            return self.find_withtag("RowSelectFill")
         elif exclude_rows and exclude_cells and not exclude_columns:
-            if self.find_withtag("ColSelectFill"):
-                return True
+            return self.find_withtag("ColSelectFill")
             
         elif exclude_columns and not exclude_rows and not exclude_cells:
-            if self.find_withtag("CellSelectFill") or self.find_withtag("RowSelectFill") or self.find_withtag("Current_Outside"):
-                return True
+            return self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("Current_Outside")
         elif exclude_rows and not exclude_columns and not exclude_cells:
-            if self.find_withtag("CellSelectFill") or self.find_withtag("ColSelectFill") or self.find_withtag("Current_Outside"):
-                return True
+            return self.find_withtag("CellSelectFill") + self.find_withtag("ColSelectFill") + self.find_withtag("Current_Outside")
+
         elif exclude_cells and not exclude_columns and not exclude_rows:
-            if self.find_withtag("RowSelectFill") or self.find_withtag("ColSelectFill"):
-                return True
+            return self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill")
             
         elif not exclude_columns and not exclude_rows and not exclude_cells:
-            if self.find_withtag("CellSelectFill") or self.find_withtag("RowSelectFill") or self.find_withtag("ColSelectFill") or self.find_withtag("Current_Outside"):
-                return True
-        return False
+            return self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill") + self.find_withtag("Current_Outside")
+        return tuple()
 
     def hide_current(self):
         for item in chain(self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside")):
             self.itemconfig(item, state = "hidden")
 
     def show_current(self):
         for item in chain(self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside")):
@@ -4989,44 +4857,58 @@
             return
         currently_selected = self.currently_selected()
         if not currently_selected:
             return
         r, c = int(currently_selected[0]), int(currently_selected[1])
         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-        if (
-            ((datarn, datacn) in self.cell_options and 'readonly' in self.cell_options[(datarn, datacn)]) or
-            (datacn in self.col_options and 'readonly' in self.col_options[datacn]) or
-            (datarn in self.row_options and 'readonly' in self.row_options[datarn])
-            ):
+        if self.get_cell_kwargs(datarn, datacn, key = 'readonly'):
             return
-        elif (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 'checkbox' in self.cell_options[(datarn, datacn)]):
+        elif self.get_cell_kwargs(datarn, datacn, key = 'dropdown') or self.get_cell_kwargs(datarn, datacn, key = 'checkbox'):
             if self.event_opens_dropdown_or_checkbox(event):
-                if 'dropdown' in self.cell_options[(datarn, datacn)]:
+                if self.get_cell_kwargs(datarn, datacn, key = 'dropdown'):
                     self.open_dropdown_window(r, c, event = event)
-                elif 'checkbox' in self.cell_options[(datarn, datacn)]:
-                    self._click_checkbox(r = r, c = c, datarn = datarn, datacn = datacn)
+                elif self.get_cell_kwargs(datarn, datacn, key = 'checkbox'):
+                    self.click_checkbox(r = r, c = c, datarn = datarn, datacn = datacn)
         else:
-            self.edit_cell_(event, r = r, c = c, dropdown = False)
+            self.open_text_editor(event = event, r = r, c = c, dropdown = False)
             
     def event_opens_dropdown_or_checkbox(self, event = None):
         if event is None:
             return False
         elif event == "rc":
             return True
         elif ((hasattr(event, 'keysym') and event.keysym == 'Return') or  # enter or f2
               (hasattr(event, 'keysym') and event.keysym == 'F2') or
               (event is not None and hasattr(event, 'keycode') and event.keycode == "??" and hasattr(event, 'num') and event.num == 1) or
               (hasattr(event, 'keysym') and event.keysym == 'BackSpace')):
             return True
         else:
             return False
+    
+    # displayed indexes
+    def get_cell_align(self, r, c):
+        datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+        cell_alignment = self.get_cell_kwargs(datarn, datacn, key = 'align')
+        if cell_alignment:
+            return cell_alignment
+        return self.align
 
-    # c is displayed col
-    def edit_cell_(self, event = None, r = None, c = None, dropdown = False):
+    # displayed indexes
+    def open_text_editor(self,
+                         event = None,
+                         r = 0,
+                         c = 0,
+                         text = None,
+                         state = "normal",
+                         see = True,
+                         set_data_on_close = True,
+                         binding = None,
+                         dropdown = False):
         text = None
         extra_func_key = "??"
         if event is None or self.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, 'keysym') and event.keysym == 'Return':
                     extra_func_key = "Return"
                 elif hasattr(event, 'keysym') and event.keysym == 'F2':
@@ -5056,41 +4938,15 @@
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.cell_auto_resize_enabled:
             self.set_cell_size_to_text(r, c, only_set_if_too_small = True, redraw = True, run_binding = True)
         if not self.currently_selected():
             self.select_cell(r = r, c = c, keep_other_selections = True)
-        self.create_text_editor(r = r, c = c, text = text, set_data_on_close = True, dropdown = dropdown)
-        return True
-    
-    # displayed indexes
-    def get_cell_align(self, r, c):
-        datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-        if (datarn, datacn) in self.cell_options and 'align' in self.cell_options[(datarn, datacn)]:
-            cell_alignment = self.cell_options[(datarn, datacn)]['align']
-        elif datarn in self.row_options and 'align' in self.row_options[datarn]:
-            cell_alignment = self.row_options[datarn]['align']
-        elif datacn in self.col_options and 'align' in self.col_options[datacn]:
-            cell_alignment = self.col_options[datacn]['align']
-        else:
-            cell_alignment = self.align
-        return cell_alignment
-
-    # displayed indexes
-    def create_text_editor(self,
-                           r = 0,
-                           c = 0,
-                           text = None,
-                           state = "normal",
-                           see = True,
-                           set_data_on_close = False,
-                           binding = None,
-                           dropdown = False):
+            
         if (r, c) == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
             has_redrawn = self.see(r = r, c = c, check_cell_visibility = True)
@@ -5100,20 +4956,20 @@
         x = self.col_positions[c]
         y = self.row_positions[r]
         w = self.col_positions[c + 1] - x + 1
         h = self.row_positions[r + 1] - y + 1
         if text is None:
             text = f"""{self.get_cell_data(r if self.all_rows_displayed else self.displayed_rows[r],
                                            c if self.all_columns_displayed else self.displayed_columns[c],
-                                           none_to_empty_str=True)}"""
+                                           none_to_empty_str = True)}"""
         self.hide_current()
         bg, fg = self.table_bg, self.table_fg
         self.text_editor = TextEditor(self, 
                                       text = text, 
-                                      font = self._font, 
+                                      font = self.table_font, 
                                       state = state, 
                                       width = w, 
                                       height = h, 
                                       border_color = self.table_selected_cells_border_fg, 
                                       show_border = self.show_selected_cells_border,
                                       bg = bg, 
                                       fg = fg,
@@ -5146,40 +5002,41 @@
             self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((r, c, "Tab")))
             self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((r, c, "Return")))
             if not dropdown:
                 self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((r, c, "FocusOut")))
             self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((r, c, "Escape")))
         else:
             self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
+        return True
     
     # displayed indexes
     def text_editor_newline_binding(self, r = 0, c = 0, event = None, check_lines = True):
         datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         curr_height = self.text_editor.winfo_height()
-        if not check_lines or self.GetLinesHeight(self.text_editor.get_num_lines() + 1) > curr_height:
+        if not check_lines or self.get_lines_cell_height(self.text_editor.get_num_lines() + 1) > curr_height:
             new_height = curr_height + self.xtra_lines_increment
             space_bot = self.get_space_bot(r)
             if new_height > space_bot:
                 new_height = space_bot
             if new_height != curr_height:
                 self.text_editor.config(height = new_height)
-                if ((r, datacn) in self.cell_options and
-                    'dropdown' in self.cell_options[(r, datacn)]):
+                kwargs = self.get_cell_kwargs(datarn, datacn, key = 'dropdown')
+                if kwargs:
                     text_editor_h = self.text_editor.winfo_height()
                     win_h, anchor = self.get_dropdown_height_anchor(datarn, datacn, text_editor_h)
                     if anchor == "nw":
-                        self.coords(self.cell_options[(r, datacn)]['dropdown']['canvas_id'],
+                        self.coords(kwargs['canvas_id'],
                                     self.col_positions[c], self.row_positions[r] + text_editor_h - 1)
-                        self.itemconfig(self.cell_options[(r, datacn)]['dropdown']['canvas_id'],
+                        self.itemconfig(kwargs['canvas_id'],
                                         anchor = anchor, height = win_h)
                     elif anchor == "sw":
-                        self.coords(self.cell_options[(r, datacn)]['dropdown']['canvas_id'],
+                        self.coords(kwargs['canvas_id'],
                                     self.col_positions[c], self.row_positions[r])
-                        self.itemconfig(self.cell_options[(r, datacn)]['dropdown']['canvas_id'],
+                        self.itemconfig(kwargs['canvas_id'],
                                         anchor = anchor, height = win_h)
 
     def destroy_text_editor(self, event = None):
         if event is not None and self.extra_end_edit_cell_func is not None and self.text_editor_loc is not None:
             self.extra_end_edit_cell_func(EditCellEvent(int(self.text_editor_loc[0]), int(self.text_editor_loc[1]), "Escape", None, "escape_edit_cell"))
         self.text_editor_loc = None
         try:
@@ -5323,150 +5180,214 @@
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         if datarn is None:
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         if not check_input_valid or self.input_valid_for_cell(datarn, datacn, value):
             if self.undo_enabled and undo:
                 self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells",
                                                                     {(datarn, datacn): self.get_cell_data(datarn, datacn)},
-                                                                    (((r, c, r + 1, c + 1), "cells"), ),
+                                                                    self.get_boxes(include_current = False),
                                                                     self.currently_selected()))))
             self.set_cell_data(datarn, datacn, value)
         if cell_resize and self.cell_auto_resize_enabled:
             self.set_cell_size_to_text(r, c, only_set_if_too_small = True, redraw = redraw, run_binding = True)
-        self.event_generate('<<SheetDataChangeEvent>>')
+        self.parentframe.emit_modified_event()
         return True
     
     def set_cell_data(self, datarn, datacn, value, kwargs = {}, expand_sheet = True):
-        if value is None:
-            value = ""
         if expand_sheet:
             if datarn >= len(self.data):
-                self.data.extend([list(repeat("", datacn + 1)) for i in range((datarn + 1) - len(self.data))])
+                self.fix_data_len(datarn, datacn)
             elif datacn >= len(self.data[datarn]):
-                self.data[datarn].extend(list(repeat("", (datacn + 1) - len(self.data[datarn]))))
+                self.data[datarn].extend(self.get_empty_row_seq(datarn, end = datacn + 1, start = len(self.data[datarn])))
         if expand_sheet or (len(self.data) > datarn and len(self.data[datarn]) > datacn):
             if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
                 self.data[datarn][datacn] = try_to_bool(value)
             else:
                 if not kwargs:
-                    kwargs = self.get_format_kwargs(datarn, datacn)
+                    kwargs = self.get_cell_kwargs(datarn, datacn, key = 'format')
                 if kwargs:
                     if kwargs['formatter'] is None:
                         self.data[datarn][datacn] = format_data(value = value, **kwargs)
                     else:
                         self.data[datarn][datacn] = kwargs['formatter'](value, **kwargs)
                 else:
                     self.data[datarn][datacn] = value
+                    
+    def get_value_for_empty_cell(self, datarn, datacn, r_ops = True, c_ops = True):
+        if self.get_cell_kwargs(datarn, datacn, key = 'checkbox', cell = r_ops and c_ops, row = r_ops, column = c_ops):
+            return False
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'dropdown', cell = r_ops and c_ops, row = r_ops, column = c_ops)
+        if kwargs and kwargs['validate_input'] and kwargs['values']:
+            return kwargs['values'][0]
+        return ""
+    
+    def get_empty_row_seq(self, datarn, end, start = 0, r_ops = True, c_ops = True):
+        return [self.get_value_for_empty_cell(datarn, datacn, r_ops = r_ops, c_ops = c_ops) for datacn in range(start, end)]
+    
+    def fix_row_len(self, datarn, datacn):
+        self.data[datarn].extend([self.get_value_for_empty_cell(datarn, cn) for cn in range(datacn + 1 - len(self.data[datarn]))])
+        
+    def fix_row_values(self, datarn, start = None, end = None):
+        if datarn < len(self.data):
+            for datacn, v in enumerate(islice(self.data[rn], start, end)):
+                if not self.input_valid_for_cell(datarn, datacn, v):
+                    self.data[datarn][datacn] = self.get_value_for_empty_cell(datarn, datacn)
+    
+    def fix_data_len(self, datarn, datacn):
+        ncols = self.total_data_cols() if datacn is None else datacn + 1
+        self.data.extend([[self.get_value_for_empty_cell(rn, cn) for cn in range(ncols)] for rn in range(datarn + 1 - len(self.data))])
 
     #internal event use
-    def _click_checkbox(self, r, c, datarn = None, datacn = None, undo = True, redraw = True):
+    def click_checkbox(self, r, c, datarn = None, datacn = None, undo = True, redraw = True):
         if datarn is None:
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         if datacn is None:
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-        if self.cell_options[(datarn, datacn)]['checkbox']['state'] == "normal":
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'checkbox')
+        if kwargs['state'] == "normal":
             self.set_cell_data_undo(r, c, 
                                     value = not self.data[datarn][datacn] if type(self.data[datarn][datacn]) == bool else False, 
                                     undo = undo, cell_resize = False, check_input_valid = False)
-            if self.cell_options[(datarn, datacn)]['checkbox']['check_function'] is not None:
-                self.cell_options[(datarn, datacn)]['checkbox']['check_function']((r, c, "CheckboxClicked", self.data[datarn][datacn]))
+            if kwargs['check_function'] is not None:
+                kwargs['check_function']((r, c, "CheckboxClicked", self.data[datarn][datacn]))
             if self.extra_end_edit_cell_func is not None:
                 self.extra_end_edit_cell_func(EditCellEvent(r, c, "Return", self.data[datarn][datacn], "end_edit_cell"))
         if redraw:
             self.refresh()
-
-    def create_checkbox(self, datarn = 0, datacn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
-        self.delete_cell_format(datarn, datacn, clear_values = True)
+            
+    def create_checkbox(self, datarn = 0, datacn = 0, **kwargs):
+        self.delete_cell_format(datarn, datacn, clear_values = False)
         if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
                                                       'checkbox' in self.cell_options[(datarn, datacn)]):
-            self.delete_dropdown_and_checkbox(datarn, datacn)
+            self.delete_cell_options_dropdown_and_checkbox(datarn, datacn)
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
-        self.cell_options[(datarn, datacn)]['checkbox'] = {'check_function': check_function,
-                                                           'state': state,
-                                                           'text': text}
-        self.set_cell_data(datarn, datacn, checked)
-        if redraw:
-            self.refresh()
-
-    def create_dropdown(self, 
-                        datarn = 0, datacn = 0, 
-                        values = [], set_value = None,
-                        state = "normal", redraw = True, 
-                        selection_function = None, modified_function = None,
-                        search_function = dropdown_search_function, validate_input = True, text = None):
+        self.cell_options[(datarn, datacn)]['checkbox'] = get_checkbox_dict(**kwargs)
+        self.set_cell_data(datarn, datacn, kwargs['checked'])
+            
+    def checkbox_row(self, datarn = 0, **kwargs):
+        self.delete_row_format(datarn, clear_values = False)
+        if datarn in self.row_options and ('dropdown' in self.row_options[datarn] or 
+                                           'checkbox' in self.row_options[datarn]):
+            self.delete_row_options_dropdown_and_checkbox(datarn)
+        if datarn not in self.row_options:
+            self.row_options[datarn] = {}
+        self.row_options[datarn]['checkbox'] = get_checkbox_dict(**kwargs)
+        for datacn in range(self.total_data_cols()):
+            self.set_cell_data(datarn, datacn, kwargs['checked'])
+            
+    def checkbox_column(self, datacn = 0, **kwargs):
+        self.delete_column_format(datacn, clear_values = False)
+        if datacn in self.col_options and ('dropdown' in self.col_options[datacn] or 
+                                           'checkbox' in self.col_options[datacn]):
+            self.delete_column_options_dropdown_and_checkbox(datacn)
+        if datacn not in self.col_options:
+            self.col_options[datacn] = {}
+        self.col_options[datacn]['checkbox'] = get_checkbox_dict(**kwargs)
+        for datarn in range(self.total_data_rows()):
+            self.set_cell_data(datarn, datacn, kwargs['checked'])
+            
+    def checkbox_sheet(self, **kwargs):
+        self.delete_sheet_format(clear_values = False)
+        if 'dropdown' in self.options or 'checkbox' in self.options:
+            self.delete_options_dropdown_and_checkbox()
+        self.options['checkbox'] = get_checkbox_dict(**kwargs)
+        total_cols = self.total_data_cols()
+        for datarn in range(self.total_data_rows()):
+            for datacn in range(total_cols):
+                self.set_cell_data(datarn, datacn, kwargs['checked'])
+                
+    def create_dropdown(self, datarn = 0, datacn = 0, **kwargs):
         if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
                                                       'checkbox' in self.cell_options[(datarn, datacn)]):
-            self.delete_dropdown_and_checkbox(datarn, datacn)
+            self.delete_cell_options_dropdown_and_checkbox(datarn, datacn)
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
-        self.cell_options[(datarn, datacn)]['dropdown'] = {'values': values,
-                                                           'window': "no dropdown open",
-                                                           'canvas_id': "no dropdown open",
-                                                           'select_function': selection_function,
-                                                           'modified_function': modified_function,
-                                                           'search_function': search_function,
-                                                           'validate_input': validate_input,
-                                                           'text': text,
-                                                           'state': state}
-        self.set_cell_data(datarn, datacn, set_value if set_value is not None else values[0] if values else "")
-        if redraw:
-            self.refresh()
+        self.cell_options[(datarn, datacn)]['dropdown'] = get_dropdown_dict(**kwargs)
+        self.set_cell_data(datarn, datacn, 
+                           kwargs['set_value'] if kwargs['set_value'] is not None else kwargs['values'][0] if kwargs['values'] else "")
+            
+    def dropdown_row(self, datarn = 0, **kwargs):
+        if datarn in self.row_options and ('dropdown' in self.row_options[datarn] or 
+                                           'checkbox' in self.row_options[datarn]):
+            self.delete_row_options_dropdown_and_checkbox(datarn)
+        if datarn not in self.row_options:
+            self.row_options[datarn] = {}
+        self.row_options[datarn]['dropdown'] = get_dropdown_dict(**kwargs)
+        value = kwargs['set_value'] if kwargs['set_value'] is not None else kwargs['values'][0] if kwargs['values'] else ""
+        for datacn in range(self.total_data_cols()):
+            self.set_cell_data(datarn, datacn, value)
 
-    def format_cell(self,
-                    datarn, 
-                    datacn,
-                    **kwargs):
+    def dropdown_column(self, datacn = 0, **kwargs):
+        if datacn in self.col_options and ('dropdown' in self.col_options[datacn] or 
+                                           'checkbox' in self.col_options[datacn]):
+            self.delete_column_options_dropdown_and_checkbox(datacn)
+        if datacn not in self.col_options:
+            self.col_options[datacn] = {}
+        self.col_options[datacn]['dropdown'] = get_dropdown_dict(**kwargs)
+        value = kwargs['set_value'] if kwargs['set_value'] is not None else kwargs['values'][0] if kwargs['values'] else ""
+        for datarn in range(self.total_data_rows()):
+            self.set_cell_data(datarn, datacn, value)
+
+    def dropdown_sheet(self, **kwargs):
+        if 'dropdown' in self.options or 'checkbox' in self.options:
+            self.delete_cell_options_dropdown_and_checkbox(datarn, datacn)
+        self.options['dropdown'] = get_dropdown_dict(**kwargs)
+        value = kwargs['set_value'] if kwargs['set_value'] is not None else kwargs['values'][0] if kwargs['values'] else ""
+        total_cols = self.total_data_cols()
+        for datarn in range(self.total_data_rows()):
+            for datacn in range(total_cols):
+                self.set_cell_data(datarn, datacn, value)
+
+    def format_cell(self, datarn, datacn, **kwargs):
         if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
             return
-        if 'value' in kwargs:
-            v = kwargs['value']
-        else:
-            v = self.get_cell_data(datarn, datacn)
         kwargs = self.format_fix_kwargs(kwargs)
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
         self.cell_options[(datarn, datacn)]['format'] = kwargs
-        self.set_cell_data(datarn, datacn, value = v, kwargs = kwargs)
-        self.event_generate('<<SheetDataChangeEvent>>')
+        self.set_cell_data(datarn, datacn, 
+                           value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn), 
+                           kwargs = kwargs)
         
     def format_row(self, datarn, **kwargs):
+        if datarn in self.row_options and 'checkbox' in self.row_options[datarn]:
+            return
         kwargs = self.format_fix_kwargs(kwargs)
         if datarn not in self.row_options:
             self.row_options[datarn] = {}
         self.row_options[datarn]['format'] = kwargs
         for datacn in range(self.total_data_cols()):
             self.set_cell_data(datarn, 
                                datacn,
                                value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
                                kwargs = kwargs)
-        self.event_generate('<<SheetDataChangeEvent>>')
             
     def format_column(self, datacn, **kwargs):
+        if datacn in self.col_options and 'checkbox' in self.col_options[datacn]:
+            return
         kwargs = self.format_fix_kwargs(kwargs)
         if datacn not in self.col_options:
             self.col_options[datacn] = {}
         self.col_options[datacn]['format'] = kwargs
         for datarn in range(self.total_data_rows()):
             self.set_cell_data(datarn, 
                                datacn,
                                value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
                                kwargs = kwargs)
-        self.event_generate('<<SheetDataChangeEvent>>')
             
     def format_sheet(self, **kwargs):
         kwargs = self.format_fix_kwargs(kwargs)
-        self.sheet_options['format'] = kwargs
+        self.options['format'] = kwargs
         for datarn in range(self.total_data_rows()):
             for datacn in range(self.total_data_cols()):
                 self.set_cell_data(datarn, 
                                    datacn,
                                    value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
                                    kwargs = kwargs)
-        self.event_generate('<<SheetDataChangeEvent>>')
 
     def format_fix_kwargs(self, kwargs):
         if kwargs['formatter'] is None:
             if kwargs['nullable']:
                 if isinstance(kwargs['datatypes'], (list, tuple)):
                     kwargs['datatypes'] = tuple(kwargs['datatypes']) + (type(None), )
                 else:
@@ -5474,15 +5395,15 @@
             elif (isinstance(kwargs['datatypes'], (list, tuple)) and type(None) in kwargs['datatypes']) or kwargs['datatypes'] is type(None):
                 raise TypeError("Non-nullable cells cannot have NoneType as a datatype.")
         if not isinstance(kwargs['invalid_value'], str):
             kwargs['invalid_value'] = f"{kwargs['invalid_value']}"
         return kwargs
     
     def reapply_formatting(self):
-        if 'format' in self.sheet_options:
+        if 'format' in self.options:
             for r in range(len(self.data)):
                 if r not in self.row_options:
                     for c in range(len(self.data[r])):
                         if not ((r, c) in self.cell_options and 'format' in self.cell_options[(r, c)] or
                                 c in self.col_options and 'format' in self.col_options[c]):
                             self.set_cell_data(r, c, value = self.data[r][c])
         for c in self.yield_formatted_columns():
@@ -5541,102 +5462,83 @@
             if datacn in self.col_options and 'format' in self.col_options[datacn]:
                 del self.col_options[datacn]['format']
                 if clear_values:
                     for datarn in range(len(self.data)):
                         self.set_cell_data(datarn, datacn, "", expand_sheet = False)
     
     def delete_sheet_format(self, clear_values = False):
-        if 'format' in self.sheet_options:
-            del self.sheet_options['format']
+        if 'format' in self.options:
+            del self.options['format']
             if clear_values:
                 total_cols = self.total_data_cols()
-                self.data = [list(repeat("", total_cols)) for i in range(len(self.data))]
-                
-    def del_cell_options(self, list_of_coords):
-        for r, datacn in list_of_coords:
-            if (r, datacn) in self.cell_options and 'dropdown' in self.cell_options[(r, datacn)]:
-                self.delete_dropdown(r, datacn)
-            del self.cell_options[(r, datacn)]
+                self.data = [[self.get_value_for_empty_cell(r, c) for c in range(total_cols)] for r in range(self.total_data_rows())]
 
     # deals with possibility of formatter class being in self.data cell
     # if cell is formatted - possibly returns invalid_value kwarg if cell value is not in datatypes kwarg
     # if get displayed is true then Nones are replaced by ""
     def get_valid_cell_data_as_str(self, datarn, datacn, get_displayed = False, **kwargs) -> str:
-        if get_displayed and (datarn, datacn) in self.cell_options:
-            if 'dropdown' in self.cell_options[(datarn, datacn)] and self.cell_options[(datarn, datacn)]['dropdown']['text'] is not None:
-                return f"{self.cell_options[(datarn, datacn)]['dropdown']['text']}"
-            if 'checkbox' in self.cell_options[(datarn, datacn)]:
-                return f"{self.cell_options[(datarn, datacn)]['checkbox']['text']}"
+        if get_displayed:
+            kwargs = self.get_cell_kwargs(datarn, datacn, key = 'dropdown')
+            if kwargs and kwargs['text'] is not None:
+                return f"{kwargs['text']}"
+            kwargs = self.get_cell_kwargs(datarn, datacn, key = 'checkbox')
+            if kwargs:
+                return f"{kwargs['text']}"
         value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
-        kwargs = self.get_format_kwargs(datarn, datacn)
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'format')
         if kwargs:
             if kwargs['formatter'] is None:
                 if get_displayed:
                     return data_to_str(value, **kwargs)
                 else:
                     return f"{get_data_with_valid_check(value, **kwargs)}"
             else:
                 if get_displayed:
                     return f"{value}" # assumed given formatter class has __str__() function
                 else:
                     return f"{value.get_data_with_valid_check()}" # assumed given formatter class has get_data_with_valid_check() function
         return "" if value is None else f"{value}"
 
     def get_cell_data(self, datarn, datacn, get_displayed = False, none_to_empty_str = False, **kwargs) -> Any:
-        if get_displayed and (datarn, datacn) in self.cell_options:
-            if 'dropdown' in self.cell_options[(datarn, datacn)] and self.cell_options[(datarn, datacn)]['dropdown']['text'] is not None:
-                return self.cell_options[(datarn, datacn)]['dropdown']['text']
-            if 'checkbox' in self.cell_options[(datarn, datacn)] and self.cell_options[(datarn, datacn)]['checkbox']['text'] is not None:
-                return self.cell_options[(datarn, datacn)]['checkbox']['text']
+        if get_displayed:
+            return self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
         value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
-        kwargs = self.get_format_kwargs(datarn, datacn)
-        if kwargs:
-            if kwargs['formatter'] is None:
-                if get_displayed:
-                    return data_to_str(value, **kwargs)
-            else:
-                if get_displayed:
-                    return f"{value}" # assumed given formatter class has __str__() function
-                else:
-                    value = value.value # assumed given formatter class has value attribute
-        return "" if (value is None and (none_to_empty_str or get_displayed)) else value
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'format')
+        if kwargs and kwargs['formatter'] is not None:
+            value = value.value # assumed given formatter class has value attribute
+        return "" if (value is None and none_to_empty_str) else value
     
     def input_valid_for_cell(self, datarn, datacn, value):
-        if (datarn, datacn) in self.cell_options and 'readonly' in self.cell_options[(datarn, datacn)]:
-            return False
-        if datarn in self.row_options and 'readonly' in self.row_options[datarn]:
-            return False
-        if datacn in self.col_options and 'readonly' in self.col_options[datacn]:
+        if self.get_cell_kwargs(datarn, datacn, key = 'readonly'):
             return False
         if self.cell_equal_to(datarn, datacn, value):
             return False
-        if self.get_format_kwargs(datarn, datacn):
+        if self.get_cell_kwargs(datarn, datacn, key = 'format'):
             return True
-        if (datarn, datacn) in self.cell_options:
-            if 'checkbox' in self.cell_options[(datarn, datacn)]:
-                return is_bool_like(value)
-            if ('dropdown' in self.cell_options[(datarn, datacn)] and 
-                self.cell_options[(datarn, datacn)]['dropdown']['validate_input'] and 
-                value not in self.cell_options[(datarn, datacn)]['dropdown']['values']):
-                return False
+        if self.get_cell_kwargs(datarn, datacn, key = 'checkbox'):
+            return is_bool_like(value)
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'dropdown')
+        if (kwargs and kwargs['validate_input'] and 
+            value not in kwargs['values']):
+            return False
         return True
 
     def cell_equal_to(self, datarn, datacn, value, **kwargs):
         v = self.get_cell_data(datarn, datacn)
-        kwargs = self.get_format_kwargs(datarn, datacn)
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'format')
         if kwargs and kwargs['formatter'] is None:
             return v == format_data(value = value, **kwargs)
         # assumed if there is a formatter class in cell then it has a __eq__() function anyway
         # else if there is not a formatter class in cell and cell is not formatted
         # then compare value as is
         return v == value
 
     def get_cell_clipboard(self, datarn, datacn) -> Union[str, int, float, bool]:
         value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
-        kwargs = self.get_format_kwargs(datarn, datacn)
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'format')
         if kwargs:
             if kwargs['formatter'] is None:
                 return get_clipboard_data(value, **kwargs)
             else:
                 return value.get_clipboard_data() # assumed given formatter class has get_clipboard_data() function and it returns one of above type hints
         return f"{value}"
 
@@ -5654,23 +5556,23 @@
 
     def yield_formatted_columns(self, formatter = None):
         if formatter is None:
             yield from (c for c, options in self.col_options.items() if 'format' in options)
         else:
             yield from (c for c, options in self.col_options.items() if 'format' in options and options['format']['formatter'] == formatter)
 
-    def get_format_kwargs(self, datarn, datacn):
-        if (datarn, datacn) in self.cell_options and 'format' in self.cell_options[(datarn, datacn)]:
-            return self.cell_options[(datarn, datacn)]['format']
-        elif datarn in self.row_options and 'format' in self.row_options[datarn]:
-            return self.row_options[datarn]['format']
-        elif datacn in self.col_options and 'format' in self.col_options[datacn]:
-            return self.col_options[datacn]['format']
-        elif 'format' in self.sheet_options:
-            return self.sheet_options['format']
+    def get_cell_kwargs(self, datarn, datacn, key = 'format', cell = True, row = True, column = True, entire = True):
+        if cell and (datarn, datacn) in self.cell_options and key in self.cell_options[(datarn, datacn)]:
+            return self.cell_options[(datarn, datacn)][key]
+        if row and datarn in self.row_options and key in self.row_options[datarn]:
+            return self.row_options[datarn][key]
+        if column and datacn in self.col_options and key in self.col_options[datacn]:
+            return self.col_options[datacn][key]
+        if entire and key in self.options:
+            return self.options[key]
         return {}
 
     def get_space_bot(self, r, text_editor_h = None):
         if len(self.row_positions) <= 1:
             if text_editor_h is None:
                 win_h = int(self.winfo_height())
                 sheet_h = int(1 + self.empty_vertical)
@@ -5688,20 +5590,20 @@
             win_h -= 1
         if sheet_h > 0:
             sheet_h -= 1
         return win_h if win_h >= sheet_h else sheet_h
 
     def get_dropdown_height_anchor(self, datarn, datacn, text_editor_h = None):
         win_h = 5
-        for i, v in enumerate(self.cell_options[(datarn, datacn)]['dropdown']['values']):
+        for i, v in enumerate(self.get_cell_kwargs(datarn, datacn, key = 'dropdown')['values']):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
                 win_h += self.fl_ins + (v_numlines * self.xtra_lines_increment) + 5 # end of cell
             else:
-                win_h += self.min_rh
+                win_h += self.min_row_height
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
         space_bot = self.get_space_bot(datarn, text_editor_h)
         space_top = int(self.row_positions[datarn])
         anchor = "nw"
@@ -5721,80 +5623,82 @@
 
     # c is displayed col
     def open_dropdown_window(self, r, c, event = None):
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window()
         datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-        if self.cell_options[(r, datacn)]['dropdown']['state'] == "normal":
-            if not self.edit_cell_(r = r, c = c, dropdown = True, event = event):
+        kwargs = self.get_cell_kwargs(datarn, datacn, key = 'dropdown')
+        if kwargs['state'] == "normal":
+            if not self.open_text_editor(event = event, r = r, c = c, dropdown = True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(datarn, datacn)
         window = self.parentframe.dropdown_class(self.winfo_toplevel(),
                                                  r,
                                                  c,
                                                  width = self.col_positions[c + 1] - self.col_positions[c] + 1,
                                                  height = win_h,
-                                                 font = self._font,
+                                                 font = self.table_font,
                                                  colors = {'bg': self.popup_menu_bg, 
                                                            'fg': self.popup_menu_fg, 
                                                            'highlight_bg': self.popup_menu_highlight_bg,
                                                            'highlight_fg': self.popup_menu_highlight_fg},
                                                  outline_color = self.table_selected_cells_border_fg,
                                                  outline_thickness = 2,
-                                                 values = self.cell_options[(datarn, datacn)]['dropdown']['values'],
+                                                 values = kwargs['values'],
                                                  close_dropdown_window = self.close_dropdown_window,
-                                                 search_function = self.cell_options[(datarn, datacn)]['dropdown']['search_function'],
+                                                 search_function = kwargs['search_function'],
                                                  arrowkey_RIGHT = self.arrowkey_RIGHT,
                                                  arrowkey_LEFT = self.arrowkey_LEFT,
                                                  align = "w")#self.get_cell_align(r, c)
-        if self.cell_options[(datarn, datacn)]['dropdown']['state'] == "normal":
+        if kwargs['state'] == "normal":
             if anchor == "nw":
                 ypos = self.row_positions[r] + self.text_editor.h_ - 1
             else:
                 ypos = self.row_positions[r]
-            self.cell_options[(datarn, datacn)]['dropdown']['canvas_id'] = self.create_window((self.col_positions[c], ypos),
-                                                                                              window = window,
-                                                                                              anchor = anchor)
+            kwargs['canvas_id'] = self.create_window((self.col_positions[c], ypos),
+                                                     window = window,
+                                                     anchor = anchor)
             self.text_editor.textedit.bind("<<TextModified>>", 
                                            lambda x: window.search_and_see(DropDownModifiedEvent("ComboboxModified", r, c, self.text_editor.get())))
-            if self.cell_options[(datarn, datacn)]['dropdown']['modified_function'] is not None:
-                window.modified_function = self.cell_options[(datarn, datacn)]['dropdown']['modified_function']
+            if kwargs['modified_function'] is not None:
+                window.modified_function = kwargs['modified_function']
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
                 self.after(2, self.text_editor.scroll_to_bottom())
             except:
                 return
             redraw = False
         else:
             if anchor == "nw":
                 ypos = self.row_positions[r + 1]
             else:
                 ypos = self.row_positions[r]
-            self.cell_options[(datarn, datacn)]['dropdown']['canvas_id'] = self.create_window((self.col_positions[c], ypos),
-                                                                                              window = window,
-                                                                                              anchor = anchor)
+            kwargs['canvas_id'] = self.create_window((self.col_positions[c], ypos),
+                                                     window = window,
+                                                     anchor = anchor)
             self.update_idletasks()
             window.bind("<FocusOut>", lambda x: self.close_dropdown_window(r, c))
             window.focus()
             redraw = True
         self.existing_dropdown_window = window
-        self.cell_options[(datarn, datacn)]['dropdown']['window'] = window
-        self.existing_dropdown_canvas_id = self.cell_options[(datarn, datacn)]['dropdown']['canvas_id']
+        kwargs['window'] = window
+        self.existing_dropdown_canvas_id = kwargs['canvas_id']
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = False)
 
     # displayed indexes, not data
     def close_dropdown_window(self, r = None, c = None, selection = None, redraw = True):
         if r is not None and c is not None and selection is not None:
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-            if self.cell_options[(datarn, datacn)]['dropdown']['select_function'] is not None: # user has specified a selection function
-                self.cell_options[(datarn, datacn)]['dropdown']['select_function'](EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
+            kwargs = self.get_cell_kwargs(datarn, datacn, key = 'dropdown')
+            if kwargs['select_function'] is not None: # user has specified a selection function
+                kwargs['select_function'](EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
             if self.extra_end_edit_cell_func is None:
                 self.set_cell_data_undo(r, c, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and self.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
                 if validation is not None:
                     selection = validation
                 self.set_cell_data_undo(r, c, value = selection, redraw = not redraw)
@@ -5851,34 +5755,74 @@
         except:
             pass
         self.existing_dropdown_canvas_id = None
         try:
             self.existing_dropdown_window.destroy()
         except:
             pass
-        if (datarn_, datacn_) in self.cell_options and 'dropdown' in self.cell_options[(datarn_, datacn_)]:
-            self.cell_options[(datarn_, datacn_)]['dropdown']['canvas_id'] = "no dropdown open"
-            self.cell_options[(datarn_, datacn_)]['dropdown']['window'] = "no dropdown open"
+        kwargs = self.get_cell_kwargs(datarn_, datacn_, key = 'dropdown')
+        if kwargs:
+            kwargs['canvas_id'] = "no dropdown open"
+            kwargs['window'] = "no dropdown open"
             try:
-                self.delete(self.cell_options[(datarn_, datacn_)]['dropdown']['canvas_id'])
+                self.delete(kwargs['canvas_id'])
             except:
                 pass
         self.existing_dropdown_window = None
 
     def get_displayed_col_from_datacn(self, datacn):
         try:
             return self.displayed_columns.index(datacn)
         except:
             return None
     
-    def delete_dropdown(self, datarn, datacn):
-        self.destroy_opened_dropdown_window(datarn = datarn, datacn = datacn)
+    def delete_cell_options_dropdown(self, datarn, datacn):
+        self.destroy_opened_dropdown_window()
         if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)]:
             del self.cell_options[(datarn, datacn)]['dropdown']
 
-    def delete_checkbox(self, datarn, datacn):
+    def delete_cell_options_checkbox(self, datarn, datacn):
         if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
             del self.cell_options[(datarn, datacn)]['checkbox']
 
-    def delete_dropdown_and_checkbox(self, datarn, datacn):
-        self.delete_dropdown(datarn, datacn)
-        self.delete_checkbox(datarn, datacn)
+    def delete_cell_options_dropdown_and_checkbox(self, datarn, datacn):
+        self.delete_cell_options_dropdown(datarn, datacn)
+        self.delete_cell_options_checkbox(datarn, datacn)
+        
+    def delete_row_options_dropdown(self, datarn):
+        self.destroy_opened_dropdown_window()
+        if datarn in self.row_options and 'dropdown' in self.row_options[datarn]:
+            del self.row_options[datarn]['dropdown']
+
+    def delete_row_options_checkbox(self, datarn):
+        if datarn in self.row_options and 'checkbox' in self.row_options[datarn]:
+            del self.row_options[datarn]['checkbox']
+
+    def delete_row_options_dropdown_and_checkbox(self, datarn):
+        self.delete_row_options_dropdown(datarn)
+        self.delete_row_options_checkbox(datarn)
+        
+    def delete_column_options_dropdown(self, datacn):
+        self.destroy_opened_dropdown_window()
+        if datacn in self.col_options and 'dropdown' in self.col_options[datacn]:
+            del self.col_options[datacn]['dropdown']
+
+    def delete_column_options_checkbox(self, datacn):
+        if datacn in self.col_options and 'checkbox' in self.col_options[datacn]:
+            del self.col_options[datacn]['checkbox']
+
+    def delete_column_options_dropdown_and_checkbox(self, datacn):
+        self.delete_column_options_dropdown(datacn)
+        self.delete_column_options_checkbox(datacn)
+        
+    def delete_options_dropdown(self):
+        self.destroy_opened_dropdown_window()
+        if 'dropdown' in self.options:
+            del self.options['dropdown']
+
+    def delete_options_checkbox(self):
+        if 'checkbox' in self.options:
+            del self.options['checkbox']
+
+    def delete_options_dropdown_and_checkbox(self):
+        self.delete_options_dropdown()
+        self.delete_options_checkbox()
```

### Comparing `tksheet-6.0.2/tksheet/_tksheet_other_classes.py` & `tksheet-6.0.3/tksheet/_tksheet_other_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ._tksheet_vars import *
+import bisect
 from collections import namedtuple
 from itertools import islice
 import tkinter as tk
 
 
 CurrentlySelectedClass = namedtuple("CurrentlySelectedClass", "row column type_")
 CtrlKeyEvent = namedtuple("CtrlKeyEvent", "eventname selectionboxes currentlyselected rows")
@@ -20,15 +21,16 @@
 EditIndexEvent = namedtuple("EditIndexEvent", "row key text eventname")
 BeginDragDropEvent = namedtuple("BeginDragDropEvent", "eventname columnstomove movedto")
 EndDragDropEvent = namedtuple("EndDragDropEvent", "eventname oldindexes newindexes movedto")
 ResizeEvent = namedtuple("ResizeEvent", "eventname index oldsize newsize")
 DropDownModifiedEvent = namedtuple("DropDownModifiedEvent", "eventname row column value")
 DrawnItem = namedtuple("DrawnItem", "iid showing")
 TextCfg = namedtuple("TextCfg", "txt tf font align")
-ProgressBar = namedtuple("ProgressBar", "bg fg pc name")
+DraggedRowColumn = namedtuple("DraggedRowColumn", "dragged to_move")
+_ProgBar = namedtuple("_ProgBar", "bg fg pc name")
 
 
 class TextEditor_(tk.Text):
     def __init__(self,
                  parent,
                  font = get_font(),
                  text = None,
@@ -107,18 +109,15 @@
                                        font = popup_menu_font,
                                        foreground = popup_menu_fg,
                                        background = popup_menu_bg,
                                        activebackground = popup_menu_highlight_bg,
                                        activeforeground = popup_menu_highlight_fg,
                                        command = self.undo)
         self.bind("<1>", lambda event: self.focus_set())
-        if USER_OS == "darwin":
-            self.bind("<2>", self.rc)
-        else:
-            self.bind("<3>", self.rc)
+        self.bind(rc_binding, self.rc)
         self._orig = self._w + "_orig"
         self.tk.call("rename", self._w, self._orig)
         self.tk.createcommand(self._w, self._proxy)
 
     def _proxy(self, command, *args):
         cmd = (self._orig, command) + args
         try:
@@ -135,31 +134,31 @@
         return result
     
     def rc(self,event):
         self.focus_set()
         self.rc_popup_menu.tk_popup(event.x_root, event.y_root)
         
     def select_all(self, event = None):
-        self.event_generate("<Command-a>" if on_mac() else "<Control-a>")
+        self.event_generate(f"<{ctrl_key}-a>")
         return "break"
     
     def cut(self, event = None):
-        self.event_generate("<Command-x>" if on_mac() else "<Control-x>")
+        self.event_generate(f"<{ctrl_key}-x>")
         return "break"
     
     def copy(self, event = None):
-        self.event_generate("<Command-c>" if on_mac() else "<Control-c>")
+        self.event_generate(f"<{ctrl_key}-c>")
         return "break"
     
     def paste(self, event = None):
-        self.event_generate("<Command-v>" if on_mac() else "<Control-v>")
+        self.event_generate(f"<{ctrl_key}-v>")
         return "break"
 
     def undo(self, event = None):
-        self.event_generate("<Command-z>" if on_mac() else "<Control-z>")
+        self.event_generate(f"<{ctrl_key}-z>")
         return "break"
 
 
 class TextEditor(tk.Frame):
     def __init__(self,
                  parent,
                  font = get_font(),
@@ -256,15 +255,52 @@
                 best_match['rn'] = rn
                 best_match['st'] = st
                 best_match['len_diff'] = len_diff
     if best_match['rn'] != float("inf"):
         return best_match['rn']
     return None
 
+def get_dropdown_kwargs(values = [],
+                        set_value = None,
+                        state = "normal",
+                        redraw = True,
+                        selection_function = None,
+                        modified_function = None,
+                        search_function = dropdown_search_function,
+                        validate_input = True,
+                        text = None,
+                        **kwargs):
+    return {'values': values, 'set_value': set_value, 'state': state, 'redraw': redraw, 'selection_function': selection_function,
+            'modified_function': modified_function, 'search_function': search_function, 'validate_input': validate_input, 'text': text}
+    
+def get_dropdown_dict(**kwargs):
+    return {'values': kwargs['values'],
+            'window': "no dropdown open",
+            'canvas_id': "no dropdown open",
+            'select_function': kwargs['selection_function'],
+            'modified_function': kwargs['modified_function'],
+            'search_function': kwargs['search_function'],
+            'validate_input': kwargs['validate_input'],
+            'text': kwargs['text'],
+            'state': kwargs['state']}
+    
+def get_checkbox_kwargs(checked = False,
+                        state = "normal",
+                        redraw = True,
+                        check_function = None,
+                        text = "",
+                        **kwargs):
+    return {'checked': checked, 'state': state, 'redraw': redraw, 'check_function': check_function, 'text': text}
+
+def get_checkbox_dict(**kwargs):
+    return {'check_function': kwargs['check_function'], 'state': kwargs['state'], 'text': kwargs['text']}
+
 def is_iterable(o):
+    if isinstance(o, str):
+        return False
     try:
         iter(o)
         return True
     except:
         return False
 
 def num2alpha(n):
@@ -295,19 +331,17 @@
     prevn = seq[start]
     for idx, n in zip(range(start, -1, -1), reversed(seq[:start])):
         if n != prevn - 1:
             return idx
         prevn = n
     return None
 
-def on_mac():
-    if USER_OS == "darwin":
-        return True
-    else:
-        return False
-
-def get_rc_binding():
-    if USER_OS == "darwin":
-        return "<2>"
-    else:
-        return "<3>"
+def get_seq_without_gaps_at_index(seq, position):
+    start_idx = bisect.bisect_left(seq, position)
+    forward_gap = get_index_of_gap_in_sorted_integer_seq_forward(seq, start_idx)
+    reverse_gap = get_index_of_gap_in_sorted_integer_seq_reverse(seq, start_idx)
+    if forward_gap is not None:
+        seq[:] = seq[:forward_gap]
+    if reverse_gap is not None:
+        seq[:] = seq[reverse_gap:]
+    return seq
```

### Comparing `tksheet-6.0.2/tksheet/_tksheet_row_index.py` & `tksheet-6.0.3/tksheet/_tksheet_row_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,21 +40,23 @@
         self.extra_motion_func = None
         self.extra_b1_press_func = None
         self.extra_b1_motion_func = None
         self.extra_b1_release_func = None
         self.extra_rc_func = None
         self.selection_binding_func = None
         self.shift_selection_binding_func = None
+        self.ctrl_selection_binding_func = None
         self.drag_selection_binding_func = None
         self.ri_extra_begin_drag_drop_func = None
         self.ri_extra_end_drag_drop_func = None
         self.extra_double_b1_func = None
         self.row_height_resize_func = None
         self.new_row_width = 0
         self.cell_options = {}
+        self.options = {}
         self.drag_and_drop_enabled = False
         self.dragged_row = None
         self.width_resizing_enabled = False
         self.height_resizing_enabled = False
         self.double_click_resizing_enabled = False
         self.row_selection_enabled = False
         self.rc_insert_row_enabled = False
@@ -82,22 +84,14 @@
         self.hidd_fill_sels = {}
         self.hidd_bord_sels = {}
         self.hidd_resize_lines = {}
         self.hidd_dropdown = {}
         self.hidd_checkbox = {}
         
         self.row_drag_and_drop_perform = kwargs['row_drag_and_drop_perform']
-        if kwargs['row_index_width'] is None:
-            self.set_width(70)
-            self.default_width = 70
-        else:
-            self.set_width(kwargs['row_index_width'])
-            self.default_width = kwargs['row_index_width']
-        self.max_rh = float(kwargs['max_rh'])
-        self.max_row_width = float(kwargs['max_row_width'])
         self.index_fg = kwargs['index_fg']
         self.index_grid_fg = kwargs['index_grid_fg']
         self.index_border_fg = kwargs['index_border_fg']
         self.index_selected_cells_bg = kwargs['index_selected_cells_bg']
         self.index_selected_cells_fg = kwargs['index_selected_cells_fg']
         self.index_selected_rows_bg = kwargs['index_selected_rows_bg']
         self.index_selected_rows_fg = kwargs['index_selected_rows_fg']
@@ -114,22 +108,22 @@
     def basic_bindings(self, enable = True):
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
-            self.bind(get_rc_binding(), self.rc)
+            self.bind(rc_binding, self.rc)
         else:
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
-            self.unbind(get_rc_binding())
+            self.unbind(rc_binding)
 
     def set_width(self, new_width, set_TL = False):
         self.current_width = new_width
         try:
             self.config(width = new_width)
         except:
             return
@@ -189,20 +183,61 @@
                         self.toggle_select_row(r, redraw = True)
                     if self.MT.rc_popup_menus_enabled:
                         popup_menu = self.ri_rc_popup_menu
         if self.extra_rc_func is not None:
             self.extra_rc_func(event)
         if popup_menu is not None:
             popup_menu.tk_popup(event.x_root, event.y_root)
+            
+    def ctrl_b1_press(self, event = None):
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
+        if (self.drag_and_drop_enabled or self.row_selection_enabled) and self.MT.ctrl_select_enabled and self.rsz_h is None and self.rsz_w is None:
+            r = self.MT.identify_row(y = event.y)
+            if r < len(self.MT.row_positions) - 1:
+                r_selected = self.MT.row_selected(r)
+                if not r_selected and self.row_selection_enabled:
+                    self.add_selection(r, set_as_current = True)
+                    self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+                    if self.ctrl_selection_binding_func is not None:
+                        self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_rows", (r, r + 1)))
+                elif r_selected:
+                    self.dragged_row = DraggedRowColumn(dragged = r, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r))
+                    
+    def ctrl_shift_b1_press(self, event):
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
+        y = event.y
+        r = self.MT.identify_row(y = y)
+        if (self.drag_and_drop_enabled or self.row_selection_enabled) and self.MT.ctrl_select_enabled and self.rsz_h is None and self.rsz_w is None:
+            if r < len(self.MT.row_positions) - 1:
+                r_selected = self.MT.row_selected(r)
+                if not r_selected and self.row_selection_enabled:
+                    r = int(r)
+                    currently_selected = self.MT.currently_selected()
+                    if currently_selected and currently_selected.type_ == "row":
+                        min_r = int(currently_selected.row)
+                        if r > min_r:
+                            self.MT.create_selected(min_r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
+                            func_event = tuple(range(min_r, r + 1))
+                        elif r < min_r:
+                            self.MT.create_selected(r, 0, min_r + 1, len(self.MT.col_positions) - 1, "rows")
+                            func_event = tuple(range(r, min_r + 1))
+                    else:
+                        self.add_selection(r, set_as_current = True)
+                        func_event = (r, )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+                    if self.ctrl_selection_binding_func is not None:
+                        self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_rows", func_event))
+                elif r_selected:
+                    self.dragged_row = DraggedRowColumn(dragged = r, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r))
 
     def shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         y = event.y
         r = self.MT.identify_row(y = y)
-        if self.drag_and_drop_enabled or self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+        if (self.drag_and_drop_enabled or self.row_selection_enabled) and self.rsz_h is None and self.rsz_w is None:
             if r < len(self.MT.row_positions) - 1:
                 r_selected = self.MT.row_selected(r)
                 if not r_selected and self.row_selection_enabled:
                     r = int(r)
                     currently_selected = self.MT.currently_selected()
                     if currently_selected and currently_selected.type_ == "row":
                         min_r = int(currently_selected.row)
@@ -216,15 +251,15 @@
                     else:
                         self.select_row(r)
                         func_event = (r, )
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.shift_selection_binding_func is not None:
                         self.shift_selection_binding_func(SelectionBoxEvent("shift_select_rows", func_event))
                 elif r_selected:
-                    self.dragged_row = r
+                    self.dragged_row = DraggedRowColumn(dragged = r, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r))
 
     def create_resize_line(self, x1, y1, x2, y2, width, fill, tag):
         if self.hidd_resize_lines:
             t, sh = self.hidd_resize_lines.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
                 self.itemconfig(t, width = width, fill = fill, tag = tag)
@@ -293,16 +328,16 @@
             r = self.MT.identify_row(y = event.y)
             if r < len(self.MT.row_positions) - 1:
                 if self.MT.single_selection_enabled:
                     self.select_row(r, redraw = True)
                 elif self.MT.toggle_selection_enabled:
                     self.toggle_select_row(r, redraw = True)
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-                if ((datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]) or
-                    (datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]) or
+                if (self.get_cell_kwargs(datarn, key = 'dropdown') or
+                    self.get_cell_kwargs(datarn, key = 'checkbox') or
                     self.edit_cell_enabled):
                     self.open_cell(event)
         self.rsz_h = None
         self.mouse_motion(event)
         if self.extra_double_b1_func is not None:
             self.extra_double_b1_func(event)
         
@@ -327,107 +362,67 @@
             self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
             self.create_resize_line(0, line2y, self.current_width, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
             self.MT.create_resize_line(x1, line2y, x2, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
         elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w == True:
             self.currently_resizing_width = True
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
             x = int(event.x)
-            if x < self.MT.min_cw:
-                x = int(self.MT.min_cw)
+            if x < self.MT.min_column_width:
+                x = int(self.MT.min_column_width)
             self.new_row_width = x
             self.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
         elif self.MT.identify_row(y = event.y, allow_end = False) is None:
             self.MT.deselect("all")
         elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             r = self.MT.identify_row(y = event.y)
             if r < len(self.MT.row_positions) - 1:
-                if self.MT.row_selected(r):
-                    datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-                    if ((datarn in self.cell_options and 'dropdown' in self.cell_options[datarn] and event.x < self.current_width and event.x > self.current_width - self.MT.txt_h - 4) or
-                        (datarn in self.cell_options and 'checkbox' in self.cell_options[datarn] and event.x < self.current_width + self.MT.txt_h + 5)) and y < self.MT.row_positions[r] + self.MT.txt_h + 5:
-                        pass
-                    else:
-                        self.dragged_row = r
+                datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+                if self.MT.row_selected(r) and not self.event_over_dropdown(r, datarn, event, y) and not self.event_over_checkbox(r, datarn, event, y):
+                    self.dragged_row = DraggedRowColumn(dragged = r, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r))
                 else:
                     self.being_drawn_rect = (r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
                     if self.MT.single_selection_enabled:
                         self.select_row(r, redraw = True)
                     elif self.MT.toggle_selection_enabled:
                         self.toggle_select_row(r, redraw = True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
     
     def b1_motion(self, event):
         x1,y1,x2,y2 = self.MT.get_canvas_visible_area()
         if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             y = self.canvasy(event.y)
             size = y - self.MT.row_positions[self.rsz_h - 1]
-            if size >= self.MT.min_rh and size < self.max_rh:
-                self.delete_resize_lines()
-                self.MT.delete_resize_lines()
+            if size >= self.MT.min_row_height and size < self.MT.max_row_height:
+                self.delete_all_resize_and_ctrl_lines(ctrl_lines = False)
                 line2y = self.MT.row_positions[self.rsz_h - 1]
                 self.create_resize_line(0, y, self.current_width, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
                 self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
                 self.create_resize_line(0, line2y, self.current_width, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
                 self.MT.create_resize_line(x1, line2y, x2, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
         elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             evx = event.x
-            self.delete_resize_lines()
-            self.MT.delete_resize_lines()
+            self.delete_all_resize_and_ctrl_lines(ctrl_lines = False)
             if evx > self.current_width:
                 x = self.MT.canvasx(evx - self.current_width)
-                if evx > self.max_row_width:
-                    evx = int(self.max_row_width)
+                if evx > self.MT.max_index_width:
+                    evx = int(self.MT.max_index_width)
                     x = self.MT.canvasx(evx - self.current_width)
                 self.new_row_width = evx
                 self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
             else:
                 x = evx
-                if x < self.MT.min_cw:
-                    x = int(self.MT.min_cw)
+                if x < self.MT.min_column_width:
+                    x = int(self.MT.min_column_width)
                 self.new_row_width = x
                 self.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
         if self.drag_and_drop_enabled and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None and self.dragged_row is not None and self.MT.anything_selected(exclude_cells = True, exclude_columns = True):
             y = self.canvasy(event.y)
             if y > 0 and y < self.MT.row_positions[-1]:
-                y = event.y
-                hend = self.winfo_height()
-                ycheck = self.yview()
-                if y >= hend - 0 and len(ycheck) > 1 and ycheck[1] < 1:
-                    if y >= hend + 15:
-                        self.MT.yview_scroll(2, "units")
-                        self.yview_scroll(2, "units")
-                    else:
-                        self.MT.yview_scroll(1, "units")
-                        self.yview_scroll(1, "units")
-                    self.check_yview()
-                    self.MT.main_table_redraw_grid_and_text(redraw_row_index = True)
-                elif y <= 0 and len(ycheck) > 1 and ycheck[0] > 0:
-                    if y >= -15:
-                        self.MT.yview_scroll(-1, "units")
-                        self.yview_scroll(-1, "units")
-                    else:
-                        self.MT.yview_scroll(-2, "units")
-                        self.yview_scroll(-2, "units")
-                    self.check_yview()
-                    self.MT.main_table_redraw_grid_and_text(redraw_row_index = True)
-                row = self.MT.identify_row(y = event.y)
-                sels = self.MT.get_selected_rows()
-                selsmin = min(sels)
-                if row in sels:
-                    ypos = self.MT.row_positions[selsmin]
-                else:
-                    if row < selsmin:
-                        ypos = self.MT.row_positions[row]
-                    else:
-                        ypos = self.MT.row_positions[row + 1]
-                self.delete_resize_lines()
-                self.MT.delete_resize_lines()
-                self.create_resize_line(0, ypos, self.current_width, ypos, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
-                self.MT.create_resize_line(x1, ypos, x2, ypos, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+                self.show_drag_and_drop_indicators(self.drag_and_drop_motion(event), x1, x2, self.dragged_row.to_move[0], self.dragged_row.to_move[-1])
         elif self.MT.drag_selection_enabled and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             need_redraw = False
             end_row = self.MT.identify_row(y = event.y)
             currently_selected = self.MT.currently_selected()
             if end_row < len(self.MT.row_positions) - 1 and currently_selected:
                 if currently_selected.type_ == "row":
                     start_row = currently_selected.row
@@ -440,132 +435,208 @@
                     if self.being_drawn_rect != rect:
                         need_redraw = True
                         self.MT.delete_selection_rects(delete_current = False)
                         self.MT.create_selected(*rect)
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
                             self.drag_selection_binding_func(SelectionBoxEvent("drag_select_rows", func_event))
-            ycheck = self.yview()
-            if event.y > self.winfo_height() and len(ycheck) > 1 and ycheck[1] < 1:
-                try:
-                    self.MT.yview_scroll(1, "units")
-                    self.yview_scroll(1, "units")
-                except:
-                    pass
-                self.check_yview()
-                need_redraw = True
-            elif event.y < 0 and self.canvasy(self.winfo_height()) > 0 and ycheck and ycheck[0] > 0:
-                try:
-                    self.yview_scroll(-1, "units")
-                    self.MT.yview_scroll(-1, "units")
-                except:
-                    pass
-                self.check_yview()
+            if self.scroll_if_event_offscreen(event):
                 need_redraw = True
             if need_redraw:
                 self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
+            
+    def ctrl_b1_motion(self, event):
+        x1,y1,x2,y2 = self.MT.get_canvas_visible_area()
+        if self.drag_and_drop_enabled and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None and self.dragged_row is not None and self.MT.anything_selected(exclude_cells = True, exclude_columns = True):
+            y = self.canvasy(event.y)
+            if y > 0 and y < self.MT.row_positions[-1]:
+                self.show_drag_and_drop_indicators(self.drag_and_drop_motion(event), x1, x2, self.dragged_row.to_move[0], self.dragged_row.to_move[-1])
+        elif self.MT.ctrl_select_enabled and self.row_selection_enabled and self.MT.drag_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+            need_redraw = False
+            end_row = self.MT.identify_row(y = event.y)
+            currently_selected = self.MT.currently_selected()
+            if end_row < len(self.MT.row_positions) - 1 and currently_selected:
+                if currently_selected.type_ == "row":
+                    start_row = currently_selected.row
+                    if end_row >= start_row:
+                        rect = (start_row, 0, end_row + 1, len(self.MT.col_positions) - 1, "rows")
+                        func_event = tuple(range(start_row, end_row + 1))
+                    elif end_row < start_row:
+                        rect = (end_row, 0, start_row + 1, len(self.MT.col_positions) - 1, "rows")
+                        func_event = tuple(range(end_row, start_row + 1))
+                    if self.being_drawn_rect != rect:
+                        need_redraw = True
+                        if self.being_drawn_rect is not None:
+                            self.MT.delete_selected(*self.being_drawn_rect)
+                        self.MT.create_selected(*rect)
+                        self.being_drawn_rect = rect
+                        if self.drag_selection_binding_func is not None:
+                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_rows", func_event))
+            if self.scroll_if_event_offscreen(event):
+                need_redraw = True
+            if need_redraw:
+                self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
+                
+    def drag_and_drop_motion(self, event):
+        y = event.y
+        hend = self.winfo_height()
+        ycheck = self.yview()
+        if y >= hend - 0 and len(ycheck) > 1 and ycheck[1] < 1:
+            if y >= hend + 15:
+                self.MT.yview_scroll(2, "units")
+                self.yview_scroll(2, "units")
+            else:
+                self.MT.yview_scroll(1, "units")
+                self.yview_scroll(1, "units")
+            self.fix_yview()
+            self.MT.main_table_redraw_grid_and_text(redraw_row_index = True)
+        elif y <= 0 and len(ycheck) > 1 and ycheck[0] > 0:
+            if y >= -15:
+                self.MT.yview_scroll(-1, "units")
+                self.yview_scroll(-1, "units")
+            else:
+                self.MT.yview_scroll(-2, "units")
+                self.yview_scroll(-2, "units")
+            self.fix_yview()
+            self.MT.main_table_redraw_grid_and_text(redraw_row_index = True)
+        row = self.MT.identify_row(y = event.y)
+        if row >= self.dragged_row.to_move[0] and row <= self.dragged_row.to_move[-1]:
+            ypos = self.MT.row_positions[self.dragged_row.to_move[0]]
+        else:
+            if row < self.dragged_row.to_move[0]:
+                ypos = self.MT.row_positions[row]
+            else:
+                ypos = self.MT.row_positions[row + 1]
+        return ypos
+                
+    def show_drag_and_drop_indicators(self, ypos, x1, x2, start_row, end_row):
+        self.delete_all_resize_and_ctrl_lines()
+        self.create_resize_line(0, ypos, self.current_width, ypos, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+        self.MT.create_resize_line(x1, ypos, x2, ypos, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+        self.MT.show_ctrl_outline(start_cell = (0, start_row),
+                                  end_cell = (len(self.MT.col_positions) - 1, end_row + 1),
+                                  dash = (),
+                                  outline = self.drag_and_drop_bg,
+                                  delete_on_timer = False)
+        
+    def delete_all_resize_and_ctrl_lines(self, ctrl_lines = True):
+        self.delete_resize_lines()
+        self.MT.delete_resize_lines()
+        if ctrl_lines:
+            self.MT.delete_ctrl_outlines()
+            
+    def scroll_if_event_offscreen(self, event):
+        ycheck = self.yview()
+        need_redraw = False
+        if event.y > self.winfo_height() and len(ycheck) > 1 and ycheck[1] < 1:
+            try:
+                self.MT.yview_scroll(1, "units")
+                self.yview_scroll(1, "units")
+            except:
+                pass
+            self.fix_yview()
+            need_redraw = True
+        elif event.y < 0 and self.canvasy(self.winfo_height()) > 0 and ycheck and ycheck[0] > 0:
+            try:
+                self.yview_scroll(-1, "units")
+                self.MT.yview_scroll(-1, "units")
+            except:
+                pass
+            self.fix_yview()
+            need_redraw = True
+        return need_redraw
 
-    def check_yview(self):
+    def fix_yview(self):
         ycheck = self.yview()
         if ycheck and ycheck[0] < 0:
             self.MT.set_yviews("moveto", 0)
         if len(ycheck) > 1 and ycheck[1] > 1:
             self.MT.set_yviews("moveto", 1)
             
+    def event_over_dropdown(self, r, datarn, event, canvasy):
+        if (canvasy < self.MT.row_positions[r] + self.MT.txt_h and
+            self.get_cell_kwargs(datarn, key = 'dropdown') and 
+            event.x > self.current_width - self.MT.txt_h - 4):
+            return True
+        return False
+  
+    def event_over_checkbox(self, r, datarn, event, canvasy):
+        if (canvasy < self.MT.row_positions[r] + self.MT.txt_h and
+            self.get_cell_kwargs(datarn, key = 'checkbox') and
+            event.x < self.MT.txt_h + 4):
+            return True
+        return False
+            
     def b1_release(self, event = None):
         if self.being_drawn_rect is not None:
+            self.MT.delete_selected(*self.being_drawn_rect)
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.MT.create_selected(*to_sel)
         self.MT.bind("<MouseWheel>", self.MT.mousewheel)
         if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             self.currently_resizing_height = False
             new_row_pos = int(self.coords("rhl")[1])
-            self.delete_resize_lines()
-            self.MT.delete_resize_lines()
+            self.delete_all_resize_and_ctrl_lines(ctrl_lines = False)
             old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             size = new_row_pos - self.MT.row_positions[self.rsz_h - 1]
-            if size < self.MT.min_rh:
-                new_row_pos = ceil(self.MT.row_positions[self.rsz_h - 1] + self.MT.min_rh)
-            elif size > self.max_rh:
-                new_row_pos = floor(self.MT.row_positions[self.rsz_h - 1] + self.max_rh)
+            if size < self.MT.min_row_height:
+                new_row_pos = ceil(self.MT.row_positions[self.rsz_h - 1] + self.MT.min_row_height)
+            elif size > self.MT.max_row_height:
+                new_row_pos = floor(self.MT.row_positions[self.rsz_h - 1] + self.MT.max_row_height)
             increment = new_row_pos - self.MT.row_positions[self.rsz_h]
             self.MT.row_positions[self.rsz_h + 1:] = [e + increment for e in islice(self.MT.row_positions, self.rsz_h + 1, len(self.MT.row_positions))]
             self.MT.row_positions[self.rsz_h] = new_row_pos
             new_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             self.MT.recreate_all_selection_boxes()
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
             if self.row_height_resize_func is not None and old_height != new_height:
                 self.row_height_resize_func(ResizeEvent("row_height_resize", self.rsz_h - 1, old_height, new_height))
         elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             self.currently_resizing_width = False
-            self.delete_resize_lines()
-            self.MT.delete_resize_lines()
+            self.delete_all_resize_and_ctrl_lines(ctrl_lines = False)
             self.set_width(self.new_row_width, set_TL = True)
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.drag_and_drop_enabled and self.MT.anything_selected(exclude_cells = True, exclude_columns = True) and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None and self.dragged_row is not None:
-            self.delete_resize_lines()
-            self.MT.delete_resize_lines()
+            self.delete_all_resize_and_ctrl_lines()
             y = event.y
             r = self.MT.identify_row(y = y)
-            orig_selected = self.MT.get_selected_rows()
-            if r != self.dragged_row and r is not None and r not in orig_selected and len(orig_selected) != (len(self.MT.row_positions) - 1):
-                orig_selected = sorted(orig_selected)
-                if len(orig_selected) > 1:
-                    orig_min = orig_selected[0]
-                    orig_max = orig_selected[1]
-                    start_idx = bisect.bisect_left(orig_selected, self.dragged_row)
-                    forward_gap = get_index_of_gap_in_sorted_integer_seq_forward(orig_selected, start_idx)
-                    reverse_gap = get_index_of_gap_in_sorted_integer_seq_reverse(orig_selected, start_idx)
-                    if forward_gap is not None:
-                        orig_selected[:] = orig_selected[:forward_gap]
-                    if reverse_gap is not None:
-                        orig_selected[:] = orig_selected[reverse_gap:]
+            orig_selected = self.dragged_row.to_move
+            if r != self.dragged_row and r is not None and (r < self.dragged_row.to_move[0] or r > self.dragged_row.to_move[-1]) and len(orig_selected) != (len(self.MT.row_positions) - 1):
                 rm1start = orig_selected[0]
                 totalrows = len(orig_selected)
                 extra_func_success = True
                 if r >= len(self.MT.row_positions) - 1:
                     r -= 1
                 if self.ri_extra_begin_drag_drop_func is not None:
                     try:
                         self.ri_extra_begin_drag_drop_func(BeginDragDropEvent("begin_row_index_drag_drop", tuple(orig_selected), int(r)))
                     except:
                         extra_func_success = False
                 if extra_func_success:
                     new_selected, dispset = self.MT.move_rows_adjust_options_dict(r, 
-                                                                                  rm1start, totalrows, move_data = self.row_drag_and_drop_perform)
+                                                                                  rm1start, 
+                                                                                  totalrows, 
+                                                                                  move_data = self.row_drag_and_drop_perform)
                     if self.MT.undo_enabled:
                         self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_rows",
-                                                                                min(orig_selected),
-                                                                                new_selected[0],
-                                                                                new_selected[-1],
-                                                                                sorted(orig_selected)))))
+                                                                                orig_selected,
+                                                                                new_selected))))
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ri_extra_end_drag_drop_func is not None:
-                        self.ri_extra_end_drag_drop_func(EndDragDropEvent("end_row_index_drag_drop", tuple(orig_selected), new_selected, int(r)))
-                    self.event_generate("<<SheetDataChangeEvent>>")
-                        
+                        self.ri_extra_end_drag_drop_func(EndDragDropEvent("end_row_index_drag_drop", orig_selected, new_selected, int(r)))
+                    self.parentframe.emit_modified_event()
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             r = self.MT.identify_row(y = event.y)
             if r is not None and r < len(self.MT.row_positions) - 1 and r == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-                if (self.canvasy(event.y) < self.MT.row_positions[r] + self.MT.txt_h and
-                    (
-                     (datarn in self.cell_options and 
-                      'dropdown' in self.cell_options[datarn] and 
-                      event.x < self.current_width and 
-                      event.x > self.current_width - self.MT.txt_h - 4) 
-                    or
-                     (datarn in self.cell_options and 
-                      'checkbox' in self.cell_options[datarn] and
-                      event.x < self.MT.txt_h + 5)
-                     )
-                ):
+                canvasy = self.canvasy(event.y)
+                if self.event_over_dropdown(r, datarn, event, canvasy) or self.event_over_checkbox(r, datarn, event, canvasy):
                     self.open_cell(event)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases()
             self.b1_pressed_loc = None
             self.closed_dropdown = None    
         self.dragged_row = None
         self.currently_resizing_width = False
@@ -587,45 +658,19 @@
                     del self.cell_options[r]['readonly']
         else:
             for r in rows_:
                 if r not in self.cell_options:
                     self.cell_options[r] = {}
                 self.cell_options[r]['readonly'] = True
 
-    def highlight_cells(self, r = 0, cells = tuple(), bg = None, fg = None, redraw = False, overwrite = True):
-        if bg is None and fg is None:
-            return
-        if cells and not isinstance(cells, int):
-            iterable = cells
-        elif isinstance(cells, int):
-            iterable = (cells, )
-        else:
-            iterable = (r, )
-        for r_ in iterable:
-            if r_ not in self.cell_options:
-                self.cell_options[r_] = {}
-            if 'highlight' in self.cell_options[r_] and not overwrite:
-                self.cell_options[r_]['highlight'] = (self.cell_options[r_]['highlight'][0] if bg is None else bg,
-                                                        self.cell_options[r_]['highlight'][1] if fg is None else fg)
-            else:
-                self.cell_options[r_]['highlight'] = (bg, fg)
-        if redraw:
-            self.MT.main_table_redraw_grid_and_text(False, True)
-
     def select_row(self, r, redraw = False, keep_other_selections = False):
-        ignore_keep = False
-        if keep_other_selections:
-            if self.MT.row_selected(r):
-                self.MT.create_current(r, 0, type_ = "row", inside = True)
-            else:
-                ignore_keep = True
-        if ignore_keep or not keep_other_selections:
+        if not keep_other_selections:
             self.MT.delete_selection_rects()
-            self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
-            self.MT.create_current(r, 0, type_ = "row", inside = True)
+        self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
+        self.MT.create_current(r, 0, type_ = "row", inside = True)
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None:
             self.selection_binding_func(SelectRowEvent("select_row", int(r)))
 
     def toggle_select_row(self, row, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
         if add_selection:
@@ -656,29 +701,29 @@
             self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(("select_row", int(r)))
             
     def get_cell_dimensions(self, datarn):
         txt = self.get_valid_cell_data_as_str(datarn, fix = False)
         if txt:
-            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text = txt, font = self.MT._font)
+            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text = txt, font = self.MT.index_font)
             b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
             w = b[2] - b[0] + 7
             h = b[3] - b[1] + 5
         else:
-            w = self.default_width
-            h = self.MT.min_rh
-        if datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 'checkbox' in self.cell_options[datarn]):
+            w = self.MT.default_index_width
+            h = self.MT.min_row_height
+        if self.get_cell_kwargs(datarn, key = 'dropdown') or self.get_cell_kwargs(datarn, key = 'checkbox'):
             return w + self.MT.txt_h, h
         return w, h
 
     def set_row_height(self, row, height = None, only_set_if_too_small = False, recreate = True, return_new_height = False, displayed_only = False):
         r_norm = row + 1
         r_extra = row + 2
-        min_rh = self.MT.min_rh
+        min_rh = self.MT.min_row_height
         datarn = row if self.MT.all_rows_displayed else self.MT.displayed_rows[row]
         if height is None:
             if self.MT.all_columns_displayed:
                 if displayed_only:
                     x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
                     start_col, end_col = self.MT.get_visible_columns(x1, x2)
                 else:
@@ -691,97 +736,107 @@
                 else:
                     start_col, end_col = 0, len(self.MT.displayed_columns)
                 iterable = self.MT.displayed_columns[start_col:end_col]
             new_height = int(min_rh)
             w_, h = self.get_cell_dimensions(datarn)
             if h < min_rh:
                 h = int(min_rh)
-            elif h > self.max_rh:
-                h = int(self.max_rh)
+            elif h > self.MT.max_row_height:
+                h = int(self.MT.max_row_height)
             if h > new_height:
                 new_height = h
             if self.MT.data:
                 for datacn in iterable:
                     txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
                     if txt:
-                        h = self.MT.GetTextHeight(txt) + 5
+                        h = self.MT.get_txt_h(txt) + 5
                     else:
                         h = min_rh
                     if h < min_rh:
                         h = int(min_rh)
-                    elif h > self.max_rh:
-                        h = int(self.max_rh)
+                    elif h > self.MT.max_row_height:
+                        h = int(self.MT.max_row_height)
                     if h > new_height:
                         new_height = h
         else:
             new_height = int(height)
         if new_height < min_rh:
             new_height = int(min_rh)
-        elif new_height > self.max_rh:
-            new_height = int(self.max_rh)
+        elif new_height > self.MT.max_row_height:
+            new_height = int(self.MT.max_row_height)
         if only_set_if_too_small and new_height <= self.MT.row_positions[row + 1] - self.MT.row_positions[row]:
             return self.MT.row_positions[row + 1] - self.MT.row_positions[row]
         if not return_new_height:
             new_row_pos = self.MT.row_positions[row] + new_height
             increment = new_row_pos - self.MT.row_positions[r_norm]
             self.MT.row_positions[r_extra:] = [e + increment for e in islice(self.MT.row_positions, r_extra, len(self.MT.row_positions))]
             self.MT.row_positions[r_norm] = new_row_pos
             if recreate:
                 self.MT.recreate_all_selection_boxes()
         return new_height
 
-    def set_width_of_index_to_text(self, recreate = True):
-        if not self.MT._row_index and isinstance(self.MT._row_index, list):
+    def set_width_of_index_to_text(self, text = None):
+        if (text is None and not self.MT._row_index and isinstance(self.MT._row_index, list) or
+            isinstance(self.MT._row_index, int) and self.MT._row_index >= len(self.MT.data)
+            ):
             return
         qconf = self.MT.txt_measure_canvas.itemconfig
         qbbox = self.MT.txt_measure_canvas.bbox
         qtxtm = self.MT.txt_measure_canvas_text
-        new_width = int(self.MT.min_cw)
+        new_width = int(self.MT.min_column_width)
         self.fix_index()
-        if self.MT.all_rows_displayed:
-            if isinstance(self.MT._row_index, list):
-                iterable = range(len(self.MT._row_index))
-            else:
-                iterable = range(len(self.MT.data))
-        else:
-            iterable = self.MT.displayed_rows
-        if isinstance(self.MT._row_index, list):
-            for datarn in iterable:
-                w, h_ = self.get_cell_dimensions(datarn)
-                if w < self.MT.min_cw:
-                    w = int(self.MT.min_cw)
-                elif w > self.max_row_width:
-                    w = int(self.max_row_width)
-                if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
-                    w += self.MT.txt_h + 6
-                elif datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
-                    w += self.MT.txt_h + 4
+        if text is not None:
+            if text:
+                qconf(qtxtm, text = text)
+                b = qbbox(qtxtm)
+                w = b[2] - b[0] + 10
                 if w > new_width:
                     new_width = w
-        elif isinstance(self.MT._row_index, int):
-            datacn = self.MT._row_index
-            for datarn in iterable:
-                txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
-                if txt:
-                    qconf(qtxtm, text = txt)
-                    b = qbbox(qtxtm)
-                    w = b[2] - b[0] + 10
+            else:
+                w = self.MT.default_index_width
+        else:
+            if self.MT.all_rows_displayed:
+                if isinstance(self.MT._row_index, list):
+                    iterable = range(len(self.MT._row_index))
                 else:
-                    w = self.default_width
-                if w < self.MT.min_cw:
-                    w = int(self.MT.min_cw)
-                elif w > self.max_row_width:
-                    w = int(self.max_row_width)
-                if w > new_width:
-                    new_width = w
-        if new_width == self.MT.min_cw:
-            new_width = self.MT.min_cw + 10
+                    iterable = range(len(self.MT.data))
+            else:
+                iterable = self.MT.displayed_rows
+            if isinstance(self.MT._row_index, list):
+                for datarn in iterable:
+                    w, h_ = self.get_cell_dimensions(datarn)
+                    if w < self.MT.min_column_width:
+                        w = int(self.MT.min_column_width)
+                    elif w > self.MT.max_index_width:
+                        w = int(self.MT.max_index_width)
+                    if self.get_cell_kwargs(datarn, key = 'checkbox'):
+                        w += self.MT.txt_h + 6
+                    elif self.get_cell_kwargs(datarn, key = 'dropdown'):
+                        w += self.MT.txt_h + 4
+                    if w > new_width:
+                        new_width = w
+            elif isinstance(self.MT._row_index, int):
+                datacn = self.MT._row_index
+                for datarn in iterable:
+                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
+                    if txt:
+                        qconf(qtxtm, text = txt)
+                        b = qbbox(qtxtm)
+                        w = b[2] - b[0] + 10
+                    else:
+                        w = self.MT.default_index_width
+                    if w < self.MT.min_column_width:
+                        w = int(self.MT.min_column_width)
+                    elif w > self.MT.max_index_width:
+                        w = int(self.MT.max_index_width)
+                    if w > new_width:
+                        new_width = w
+        if new_width == self.MT.min_column_width:
+            new_width = self.MT.min_column_width + 10
         self.set_width(new_width, set_TL = True)
-        if recreate:
-            self.MT.recreate_all_selection_boxes()
         self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
 
     def set_height_of_all_rows(self, height = None, only_set_if_too_small = False, recreate = True):
         if height is None:
             self.MT.row_positions = list(accumulate(chain([0], (self.set_row_height(rn, only_set_if_too_small = only_set_if_too_small, recreate = False, return_new_height = True) for rn in range(len(self.MT.data))))))
         else:
             self.MT.row_positions = list(accumulate(chain([0], (height for r in range(len(self.MT.data))))))
@@ -802,75 +857,64 @@
                 if r not in self.cell_options:
                     self.cell_options[r] = {}
                 self.cell_options[r]['align'] = align
 
     def auto_set_index_width(self, end_row):
         if not self.MT._row_index and not isinstance(self.MT._row_index, int) and self.auto_resize_width:
             if self.default_index == "letters":
-                new_w = self.MT.GetTextWidth(f"{num2alpha(end_row)}") + 20
+                new_w = self.MT.get_txt_w(f"{num2alpha(end_row)}") + 20
                 if self.current_width - new_w > 15 or new_w - self.current_width > 5:
                     self.set_width(new_w, set_TL = True)
                     return True
             elif self.default_index == "numbers":
-                new_w = self.MT.GetTextWidth(f"{end_row}") + 20
+                new_w = self.MT.get_txt_w(f"{end_row}") + 20
                 if self.current_width - new_w > 15 or new_w - self.current_width > 5:
                     self.set_width(new_w, set_TL = True)
                     return True
             elif self.default_index == "both":
-                new_w = self.MT.GetTextWidth(f"{end_row + 1} {num2alpha(end_row)}") + 20
+                new_w = self.MT.get_txt_w(f"{end_row + 1} {num2alpha(end_row)}") + 20
                 if self.current_width - new_w > 15 or new_w - self.current_width > 5:
                     self.set_width(new_w, set_TL = True)
                     return True
         return False
 
-    def redraw_highlight_get_text_fg(self, fr, sr, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, hlrow):
+    def redraw_highlight_get_text_fg(self, fr, sr, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, datarn):
         redrawn = False
-        if r in self.cell_options and 'highlight' in self.cell_options[r] and r in actual_selected_rows:
-            if self.cell_options[r]['highlight'][0] is not None:
-                c_1 = self.cell_options[r]['highlight'][0] if self.cell_options[r]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[r]['highlight'][0]]
-                redrawn = self.redraw_highlight(0,
-                                                fr + 1,
-                                                self.current_width - 1,
-                                                sr,
-                                                fill = (f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}" +
-                                                        f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}" +
-                                                        f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"),
-                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "",
-                                                tag = "s")
-            fill = self.index_selected_rows_fg if self.cell_options[r]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[r]['highlight'][1]
-        elif r in self.cell_options and 'highlight' in self.cell_options[r] and (r in selected_rows or selected_cols):
-            if self.cell_options[r]['highlight'][0] is not None:
-                c_1 = self.cell_options[r]['highlight'][0] if self.cell_options[r]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[r]['highlight'][0]]
+        kwargs = self.get_cell_kwargs(datarn, key = 'highlight')
+        if kwargs:
+            if kwargs[0] is not None:
+                c_1 = kwargs[0] if kwargs[0].startswith("#") else Color_Map_[kwargs[0]]
+            if r in actual_selected_rows:
+                tf = self.index_selected_rows_fg if kwargs[1] is None or self.MT.display_selected_fg_over_highlights else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}" + f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}" + f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"
+            elif r in selected_rows or selected_cols:
+                tf = self.index_selected_cells_fg if kwargs[1] is None or self.MT.display_selected_fg_over_highlights else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}" + f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}" + f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"
+            else:
+                tf = self.index_fg if kwargs[1] is None else kwargs[1]
+                if kwargs[0] is not None:
+                    fill = kwargs[0]
+            if kwargs[0] is not None:
                 redrawn = self.redraw_highlight(0,
                                                 fr + 1,
                                                 self.current_width - 1,
                                                 sr,
-                                                fill = (f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}" +
-                                                        f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}" +
-                                                        f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"),
-                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "",
+                                                fill = fill,
+                                                outline = self.index_fg if self.get_cell_kwargs(datarn, key = 'dropdown') and self.MT.show_dropdown_borders else "",
                                                 tag = "s")
-            fill = self.index_selected_cells_fg if self.cell_options[r]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[r]['highlight'][1]
-        elif r in actual_selected_rows:
-            fill = self.index_selected_rows_fg
-        elif r in selected_rows or selected_cols:
-            fill = self.index_selected_cells_fg
-        elif r in self.cell_options and 'highlight' in self.cell_options[r]:
-            if self.cell_options[r]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(0, 
-                                                fr + 1, 
-                                                self.current_width - 1, 
-                                                sr,
-                                                fill = self.cell_options[r]['highlight'][0], 
-                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "", 
-                                                tag = "s")
-            fill = self.index_fg if self.cell_options[r]['highlight'][1] is None else self.cell_options[r]['highlight'][1]
-        else:
-            fill = self.index_fg
-        return fill, redrawn
+        elif not kwargs:
+            if r in actual_selected_rows:
+                tf = self.index_selected_rows_fg
+            elif r in selected_rows or selected_cols:
+                tf = self.index_selected_cells_fg
+            else:
+                tf = self.index_fg
+        return tf, redrawn
 
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         config = (fill, outline)
         coords = (x1, y1, x2, y2)
         k = None
         if config in self.hidd_high:
             k = config
@@ -918,15 +962,15 @@
             self.disp_grid[self.create_line(points, fill = fill, width = width, tag = tag)] = True
             
     def redraw_dropdown(self, x1, y1, x2, y2, fill, outline, tag, draw_outline = True, draw_arrow = True, dd_is_open = False):
         if draw_outline and self.MT.show_dropdown_borders:
             self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill = "", outline = self.index_fg, tag = tag)
         if draw_arrow:
             topysub = floor(self.MT.half_txt_h / 2)
-            mid_y = y1 + floor(self.MT.min_rh / 2)
+            mid_y = y1 + floor(self.MT.min_row_height / 2)
             if mid_y + topysub + 1 >= y1 + self.MT.txt_h - 1:
                 mid_y -= 1
             if mid_y - topysub + 2 <= y1 + 4 + topysub:
                 mid_y -= 1
                 ty1 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
                 ty2 = mid_y - topysub + 3 if dd_is_open else mid_y + topysub + 1
                 ty3 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
@@ -1034,61 +1078,61 @@
                     points.extend([self.current_width, draw_y,
                                    -1, draw_y,
                                    -1, self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y])
                 if points:
                     self.redraw_gridline(points = points, fill = self.index_grid_fg, width = 1, tag = "h")
         c_2 = self.index_selected_cells_bg if self.index_selected_cells_bg.startswith("#") else Color_Map_[self.index_selected_cells_bg]
         c_3 = self.index_selected_rows_bg if self.index_selected_rows_bg.startswith("#") else Color_Map_[self.index_selected_rows_bg]
-        font = self.MT._font
+        font = self.MT.index_font
         for r in range(start_row, end_row - 1):
             rtopgridln = self.MT.row_positions[r]
             rbotgridln = self.MT.row_positions[r + 1]
             if rbotgridln - rtopgridln < self.MT.txt_h:
                 continue
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             fill, dd_drawn = self.redraw_highlight_get_text_fg(rtopgridln, rbotgridln, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, datarn)
             
             if datarn in self.cell_options and 'align' in self.cell_options[datarn]:
                 align = self.cell_options[datarn]['align']
             else:
                 align = self.align
-                
+            dropdown_kwargs = self.get_cell_kwargs(datarn, key = 'dropdown')
             if align == "w":
                 draw_x = 3
-                if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
+                if dropdown_kwargs:
                     mw = self.current_width - self.MT.txt_h - 2
                     self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[datarn]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = dropdown_kwargs['window'] != "no dropdown open")
                 else:
                     mw = self.current_width - 2
 
             elif align == "e":
-                if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
+                if dropdown_kwargs:
                     mw = self.current_width - self.MT.txt_h - 2
                     draw_x = self.current_width - 5 - self.MT.txt_h
                     self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[datarn]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = dropdown_kwargs['window'] != "no dropdown open")
                 else:
                     mw = self.current_width - 2
                     draw_x = self.current_width - 3
 
             elif align == "center":
-                if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
+                if dropdown_kwargs:
                     mw = self.current_width - self.MT.txt_h - 2
                     draw_x = ceil((self.current_width - self.MT.txt_h) / 2)
                     self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[datarn]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = dropdown_kwargs['window'] != "no dropdown open")
                 else:
                     mw = self.current_width - 1
                     draw_x = floor(self.current_width / 2)
-
-            if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
+            checkbox_kwargs = self.get_cell_kwargs(datarn, key = 'checkbox')
+            if checkbox_kwargs:
                 if mw > + 2:
                     box_w = self.MT.txt_h + 1
                     mw -= box_w
                     if align == "w":
                         draw_x += box_w + 1
                     elif align == "center":
                         draw_x += ceil(box_w / 2) + 1
@@ -1099,15 +1143,15 @@
                         draw_check = self.MT._row_index[datarn] if isinstance(self.MT._row_index, (list, tuple)) else self.MT.data[datarn][self.MT._row_index]
                     except:
                         draw_check = False
                     self.redraw_checkbox(2,
                                          rtopgridln + 2,
                                          self.MT.txt_h + 3,
                                          rtopgridln + self.MT.txt_h + 3,
-                                         fill = fill if self.cell_options[datarn]['checkbox']['state'] == "normal" else self.index_grid_fg,
+                                         fill = fill if checkbox_kwargs['state'] == "normal" else self.index_grid_fg,
                                          outline = "",
                                          tag = "cb",
                                          draw_check = draw_check)
             lns = self.get_valid_cell_data_as_str(datarn, fix = False).split("\n")
             if lns == [""]:
                 if self.show_default_index_for_empty:
                     lns = (get_n2a(r, self.default_index), )
@@ -1152,31 +1196,31 @@
                             else:
                                 self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align, state = "normal")
                         if k is not None and not self.hidd_text[k]:
                             del self.hidd_text[k]
                         wd = self.bbox(iid)
                         wd = wd[2] - wd[0]
                         if wd > mw:
-                            if align == "w" and datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
+                            if align == "w" and dropdown_kwargs:
                                 txt = txt[:int(len(txt) * (mw / wd))]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[:-1]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
-                            elif align == "e" and datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
+                            elif align == "e" and dropdown_kwargs:
                                 txt = txt[len(txt) - int(len(txt) * (mw / wd)):]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[1:]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
-                            elif align == "center" and ((datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]) or (datarn in self.cell_options and 'dropdown' in self.cell_options[datarn])):
+                            elif align == "center" and (dropdown_kwargs or checkbox_kwargs):
                                 tmod = ceil((len(txt) - int(len(txt) * (mw / wd))) / 2)
                                 txt = txt[tmod - 1:-tmod]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
                                 self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[next(self.c_align_cyc)]
@@ -1219,37 +1263,54 @@
         if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.MT.currently_selected()
         if not currently_selected:
             return
         r = int(currently_selected[0])
         datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if datarn in self.cell_options and 'readonly' in self.cell_options[datarn]:
+        if self.get_cell_kwargs(datarn, key = 'readonly'):
             return
-        elif datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 'checkbox' in self.cell_options[datarn]):
+        elif self.get_cell_kwargs(datarn, key = 'dropdown') or self.get_cell_kwargs(datarn, key = 'checkbox'):
             if self.MT.event_opens_dropdown_or_checkbox(event):
-                if 'dropdown' in self.cell_options[datarn]:
+                if self.get_cell_kwargs(datarn, key = 'dropdown'):
                     self.open_dropdown_window(r, event = event)
-                elif 'checkbox' in self.cell_options[datarn]:
-                    self._click_checkbox(r, datarn)
+                elif self.get_cell_kwargs(datarn, key = 'checkbox'):
+                    self.click_checkbox(r, datarn)
         elif self.edit_cell_enabled:
-            self.edit_cell_(event, r = r, dropdown = False)
+            self.open_text_editor(event = event, r = r, dropdown = False)
+    
+    # displayed indexes
+    def get_cell_align(self, r):
+        datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+        if datarn in self.cell_options and 'align' in self.cell_options[datarn]:
+            align = self.cell_options[datarn]['align']
+        else:
+            align = self.align
+        return align
 
     # r is displayed row
-    def edit_cell_(self, event = None, r = None, dropdown = False):
+    def open_text_editor(self,
+                         event = None,
+                         r = 0,
+                         text = None,
+                         state = "normal",
+                         see = True,
+                         set_data_on_close = True,
+                         binding = None,
+                         dropdown = False):
         text = None
         extra_func_key = "??"
         if event is None or self.MT.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, 'keysym') and event.keysym == 'Return':
                     extra_func_key = "Return"
                 elif hasattr(event, 'keysym') and event.keysym == 'F2':
                     extra_func_key = "F2"
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            text = self.get_cell_data(datarn, redirect_int = True)
+            text = self.get_cell_data(datarn, none_to_empty_str = True, redirect_int = True)
         elif event is not None and ((hasattr(event, 'keysym') and event.keysym == 'BackSpace') or
                                     event.keycode in (8, 855638143)):
             extra_func_key = "BackSpace"
             text = ""
         elif event is not None and ((hasattr(event, "char") and event.char.isalpha()) or
                                     (hasattr(event, "char") and event.char.isdigit()) or
                                     (hasattr(event, "char") and event.char in symbols_set)):
@@ -1267,35 +1328,15 @@
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
             self.set_row_height_run_binding(r)
         self.select_row(r = r, keep_other_selections = True, redraw = not dropdown)
-        self.create_text_editor(r = r, text = text, set_data_on_close = True, dropdown = dropdown)
-        return True
-    
-    # displayed indexes
-    def get_cell_align(self, r):
-        datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if datarn in self.cell_options and 'align' in self.cell_options[datarn]:
-            align = self.cell_options[datarn]['align']
-        else:
-            align = self.align
-        return align
-
-    # r is displayed row
-    def create_text_editor(self,
-                           r = 0,
-                           text = None,
-                           state = "normal",
-                           see = True,
-                           set_data_on_close = False,
-                           binding = None,
-                           dropdown = False):
+        
         if r == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
             has_redrawn = self.MT.see(r = r, c = 0, keep_yscroll = True, check_cell_visibility = True)
@@ -1304,19 +1345,19 @@
         self.text_editor_loc = r
         x = 0
         y = self.MT.row_positions[r] + 1
         w = self.current_width + 1
         h = self.MT.row_positions[r + 1] - y
         datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if text is None:
-            text = self.get_cell_data(datarn)
+            text = self.get_cell_data(datarn, none_to_empty_str = True, redirect_int = True)
         bg, fg = self.index_bg, self.index_fg
         self.text_editor = TextEditor(self,
                                       text = text,
-                                      font = self.MT._font,
+                                      font = self.MT.index_font,
                                       state = state,
                                       width = w,
                                       height = h,
                                       border_color = self.MT.table_selected_cells_border_fg,
                                       show_border = False,
                                       bg = bg,
                                       fg = fg,
@@ -1348,40 +1389,42 @@
             self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((r, "Tab")))
             self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((r, "Return")))
             if not dropdown:
                 self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((r, "FocusOut")))
             self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((r, "Escape")))
         else:
             self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
+        return True
             
     def text_editor_newline_binding(self, r = 0, c = 0, event = None, check_lines = True):
         if self.height_resizing_enabled:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             curr_height = self.text_editor.winfo_height()
-            if not check_lines or self.MT.GetLinesHeight(self.text_editor.get_num_lines() + 1) > curr_height:
+            if not check_lines or self.MT.get_lines_cell_height(self.text_editor.get_num_lines() + 1, font = self.MT.index_font) > curr_height:
                 new_height = curr_height + self.MT.xtra_lines_increment
                 space_bot = self.MT.get_space_bot(r)
                 if new_height > space_bot:
                     new_height = space_bot
                 if new_height != curr_height:
                     self.set_row_height(datarn, new_height)
                     self.MT.refresh()
                     self.text_editor.config(height = new_height)
-                    if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
+                    kwargs = self.get_cell_kwargs(datarn, key = 'dropdown')
+                    if kwargs:
                         text_editor_h = self.text_editor.winfo_height()
                         win_h, anchor = self.get_dropdown_height_anchor(datarn, text_editor_h)
                         if anchor == "nw":
-                            self.coords(self.cell_options[datarn]['dropdown']['canvas_id'],
+                            self.coords(kwargs['canvas_id'],
                                         self.MT.col_positions[c], self.MT.row_positions[r] + text_editor_h - 1)
-                            self.itemconfig(self.cell_options[datarn]['dropdown']['canvas_id'],
+                            self.itemconfig(kwargs['canvas_id'],
                                             anchor = anchor, height = win_h)
                         elif anchor == "sw":
-                            self.coords(self.cell_options[datarn]['dropdown']['canvas_id'],
+                            self.coords(kwargs['canvas_id'],
                                         self.MT.col_positions[c], self.MT.row_positions[r])
-                            self.itemconfig(self.cell_options[datarn]['dropdown']['canvas_id'],
+                            self.itemconfig(kwargs['canvas_id'],
                                             anchor = anchor, height = win_h)
             
     def bind_cell_edit(self, enable = True):
         if enable:
             self.edit_cell_enabled = True
         else:
             self.edit_cell_enabled = False
@@ -1461,179 +1504,203 @@
             self.MT.set_cell_data_undo(r = r, c = self.MT._row_index, datarn = datarn, value = value, undo = True)
         else:
             self.fix_index(datarn)
             if not check_input_valid or self.input_valid_for_cell(datarn, value):
                 if self.MT.undo_enabled and undo:
                     self.MT.undo_storage.append(zlib.compress(pickle.dumps(("edit_index",
                                                                             {datarn: self.MT._row_index[datarn]},
-                                                                            (((r, 0, r + 1, len(self.MT.col_positions) - 1), "rows"), ),
+                                                                            self.MT.get_boxes(include_current = False),
                                                                             self.MT.currently_selected()))))
                 self.set_cell_data(datarn = datarn, value = value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
             self.set_row_height_run_binding(r, only_set_if_too_small = False)
         if redraw:
             self.MT.refresh()
-        self.event_generate('<<SheetDataChangeEvent>>')
+        self.parentframe.emit_modified_event()
 
     def set_cell_data(self, datarn = None, value = ""):
         if isinstance(self.MT._row_index, int):
             self.MT.set_cell_data(datarn = datarn, datacn = self.MT._row_index, value = value)
         else:
             self.fix_index(datarn)
-            if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
+            if self.get_cell_kwargs(datarn, key = 'checkbox'):
                 self.MT._row_index[datarn] = try_to_bool(value)
             else:
                 self.MT._row_index[datarn] = value
             
     def input_valid_for_cell(self, datarn, value):
-        if datarn in self.cell_options:
-            if 'readonly' in self.cell_options[datarn]:
-                return False
-            if 'checkbox' in self.cell_options[datarn]:
-                return is_bool_like(value)
+        if self.get_cell_kwargs(datarn, key = 'readonly'):
+            return False
+        if self.get_cell_kwargs(datarn, key = 'checkbox'):
+            return is_bool_like(value)
         if self.cell_equal_to(datarn, value):
             return False
-        if (datarn in self.cell_options and 
-            'dropdown' in self.cell_options[datarn] and 
-            self.cell_options[datarn]['dropdown']['validate_input'] and 
-            value not in self.cell_options[datarn]['dropdown']['values']):
+        kwargs = self.get_cell_kwargs(datarn, key = 'dropdown')
+        if (kwargs and kwargs['validate_input'] and 
+            value not in kwargs['values']):
             return False
         return True
     
     def cell_equal_to(self, datarn, value):
         self.fix_index(datarn)
         if isinstance(self.MT._row_index, list):
             return self.MT._row_index[datarn] == value
         elif isinstance(self.MT._row_index, int):
             return self.MT.cell_equal_to(datarn, self.MT._row_index, value)
             
-    def get_cell_data(self, datarn, get_displayed = False, redirect_int = False):
-        if get_displayed and datarn in self.cell_options:
-            if 'dropdown' in self.cell_options[datarn] and self.cell_options[datarn]['dropdown']['text'] is not None:
-                return self.cell_options[datarn]['dropdown']['text']
-            if 'checkbox' in self.cell_options[datarn]:
-                return self.cell_options[datarn]['checkbox']['text']
-        if redirect_int and isinstance(self.MT._row_index, int):
+    def get_cell_data(self, datarn, get_displayed = False, none_to_empty_str = False, redirect_int = False):
+        if get_displayed:
+            return self.get_valid_cell_data_as_str(datarn, fix = False)
+        if redirect_int and isinstance(self.MT._row_index, int): #internal use
             return self.MT.get_cell_data(datarn, self.MT._row_index, none_to_empty_str = True)
-        if isinstance(self.MT._row_index, int) or not self.MT._row_index or datarn >= len(self.MT._row_index) or not self.MT._row_index[datarn]:
-            if get_displayed and self.show_default_index_for_empty:
-                return get_n2a(datarn, self.default_index)
-            else:
-                return ""
-        return "" if self.MT._row_index[datarn] is None and get_displayed else self.MT._row_index[datarn]
+        if (isinstance(self.MT._row_index, int) or
+            not self.MT._row_index or 
+            datarn >= len(self.MT._row_index) or 
+            (self.MT._row_index[datarn] is None and none_to_empty_str)):
+            return ""
+        return self.MT._row_index[datarn]
             
     def get_valid_cell_data_as_str(self, datarn, fix = True) -> str:
-        if datarn in self.cell_options:
-            if 'dropdown' in self.cell_options[datarn] and self.cell_options[datarn]['dropdown']['text'] is not None:
-                return f"{self.cell_options[datarn]['dropdown']['text']}"
-            if 'checkbox' in self.cell_options[datarn]:
-                return f"{self.cell_options[datarn]['checkbox']['text']}"
+        kwargs = self.get_cell_kwargs(datarn, key = 'dropdown')
+        if kwargs and kwargs['text'] is not None:
+            return f"{kwargs['text']}"
+        kwargs = self.get_cell_kwargs(datarn, key = 'checkbox')
+        if kwargs:
+            return f"{kwargs['text']}"
         if isinstance(self.MT._row_index, int):
             return self.MT.get_valid_cell_data_as_str(datarn, self.MT._row_index, get_displayed = True)
         if fix:
             self.fix_index(datarn)
         try:
             return "" if self.MT._row_index[datarn] is None else f"{self.MT._row_index[datarn]}"
         except:
             return ""
-            
-    def fix_index(self, datarn = None):
+        
+    def get_value_for_empty_cell(self, datarn, r_ops = True):
+        if self.get_cell_kwargs(datarn, key = 'checkbox', cell = r_ops):
+            return False
+        kwargs = self.get_cell_kwargs(datarn, key = 'dropdown', cell = r_ops)
+        if kwargs and kwargs['validate_input'] and kwargs['values']:
+            return kwargs['values'][0]
+        return ""
+    
+    def get_empty_index_seq(self, end, start = 0, r_ops = True):
+        return [self.get_value_for_empty_cell(datarn, r_ops = r_ops) for datarn in range(start, end)]
+
+    def fix_index(self, datarn = None, fix_values = tuple()):
         if isinstance(self.MT._row_index, int):
             return
         if isinstance(self.MT._row_index, float):
             self.MT._row_index = int(self.MT._row_index)
             return
         if not isinstance(self.MT._row_index, list):
             try:
                 self.MT._row_index = list(self.MT._row_index)
             except:
                 self.MT._row_index = []
         if isinstance(datarn, int) and datarn >= len(self.MT._row_index):
-            self.MT._row_index.extend(list(repeat("", datarn - len(self.MT._row_index) + 1)))
-            
+            self.MT._row_index.extend(self.get_empty_index_seq(end = datarn + 1, start = len(self.MT._row_index)))
+        if fix_values:
+            for rn, v in enumerate(islice(self.MT._row_index, fix_values[0], fix_values[1])):
+                if not self.input_valid_for_cell(rn, v):
+                    self.MT._row_index[rn] = self.get_value_for_empty_cell(rn)
+
     def set_row_height_run_binding(self, r, only_set_if_too_small = True):
         old_height = self.MT.row_positions[r + 1] - self.MT.row_positions[r]
         new_height = self.set_row_height(r, only_set_if_too_small = only_set_if_too_small)
         if self.row_height_resize_func is not None and old_height != new_height:
             self.row_height_resize_func(ResizeEvent("row_height_resize", r, old_height, new_height))
 
     #internal event use
-    def _click_checkbox(self, r, datarn = None, undo = True, redraw = True):
+    def click_checkbox(self, r, datarn = None, undo = True, redraw = True):
         if datarn is None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if self.cell_options[datarn]['checkbox']['state'] == "normal":
+        kwargs = self.get_cell_kwargs(datarn, key = 'checkbox')
+        if kwargs['state'] == "normal":
             if isinstance(self.MT._row_index, list):
                 value = not self.MT._row_index[datarn] if type(self.MT._row_index[datarn]) == bool else False
             elif isinstance(self.MT._row_index, int):
                 value = not self.MT.data[datarn][self.MT._row_index] if type(self.MT.data[datarn][self.MT._row_index]) == bool else False
             else:
                 value = False
             self.set_cell_data_undo(r, 
                                     datarn = datarn, 
                                     value = value, 
                                     cell_resize = False)
-            if self.cell_options[datarn]['checkbox']['check_function'] is not None:
-                self.cell_options[datarn]['checkbox']['check_function']((r,
-                                                                         0, 
-                                                                         "IndexCheckboxClicked",
-                                                                         self.MT._row_index[datarn] if isinstance(self.MT._row_index, list) else self.MT.get_cell_data(datarn, self.MT._row_index)))
+            if kwargs['check_function'] is not None:
+                kwargs['check_function']((r,
+                                          0, 
+                                          "IndexCheckboxClicked",
+                                          self.MT._row_index[datarn] if isinstance(self.MT._row_index, list) else self.MT.get_cell_data(datarn, self.MT._row_index)))
             if self.extra_end_edit_cell_func is not None:
                 self.extra_end_edit_cell_func(EditIndexEvent(r, 
                                                              "Return",
                                                              self.MT._row_index[datarn] if isinstance(self.MT._row_index, list) else self.MT.get_cell_data(datarn, self.MT._row_index), 
                                                              "end_edit_index"))
         if redraw:
             self.MT.refresh()
+            
+    def checkbox_index(self, **kwargs):
+        self.destroy_opened_dropdown_window()
+        if 'dropdown' in self.options or 'checkbox' in self.options:
+            self.delete_options_dropdown_and_checkbox()
+        if 'checkbox' not in self.options:
+            self.options['checkbox'] = {}
+        self.options['checkbox'] = get_checkbox_dict(**kwargs)
+        total_rows = self.MT.total_data_rows()
+        if isinstance(self.MT._row_index, int):
+            for datarn in total_rows:
+                self.MT.set_cell_data(datarn = datarn, datacn = self.MT._row_index, value = kwargs['checked'])
+        else:
+            for datarn in total_rows:
+                self.set_cell_data(datarn = datarn, value = kwargs['checked'])
+                
+    def dropdown_index(self, **kwargs):
+        self.destroy_opened_dropdown_window()
+        if 'dropdown' in self.options or 'checkbox' in self.options:
+            self.delete_options_dropdown_and_checkbox()
+        if 'dropdown' not in self.options:
+            self.options['dropdown'] = {}
+        self.options['dropdown'] = get_dropdown_dict(**kwargs)
+        total_rows = self.MT.total_data_rows()
+        value = kwargs['set_value'] if kwargs['set_value'] is not None else kwargs['values'][0] if kwargs['values'] else ""
+        if isinstance(self.MT._row_index, int):
+            for datarn in total_rows:
+                self.MT.set_cell_data(datarn = datarn, datacn = self.MT._row_index, value = value)
+        else:
+            for datarn in total_rows:
+                self.set_cell_data(datarn = datarn, datacn = self.MT._row_index, value = value)
 
-    def create_checkbox(self, datarn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
+    def create_checkbox(self, datarn = 0, **kwargs):
         if datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 
                                             'checkbox' in self.cell_options[datarn]):
-            self.delete_dropdown_and_checkbox(datarn)
+            self.delete_cell_options_dropdown_and_checkbox(datarn)
         if datarn not in self.cell_options:
             self.cell_options[datarn] = {}
-        self.cell_options[datarn]['checkbox'] = {'check_function': check_function,
-                                                 'state': state,
-                                                 'text': text}
-        self.set_cell_data(datarn = datarn, value = checked)
-        if redraw:
-            self.MT.refresh()
+        self.cell_options[datarn]['checkbox'] = get_checkbox_dict(**kwargs)
+        self.set_cell_data(datarn = datarn, value = kwargs['checked'])
 
-    def create_dropdown(self, 
-                        datarn = 0, 
-                        values = [], set_value = None, 
-                        state = "normal", redraw = True, 
-                        selection_function = None, modified_function = None,
-                        search_function = dropdown_search_function, validate_input = True, text = None):
+    def create_dropdown(self, **kwargs):
         if datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 
                                             'checkbox' in self.cell_options[datarn]):
-            self.delete_dropdown_and_checkbox(datarn)
+            self.delete_cell_options_dropdown_and_checkbox(datarn)
         if datarn not in self.cell_options:
             self.cell_options[datarn] = {}
-        self.cell_options[datarn]['dropdown'] = {'values': values,
-                                                 'window': "no dropdown open",
-                                                 'canvas_id': "no dropdown open",
-                                                 'select_function': selection_function,
-                                                 'modified_function': modified_function,
-                                                 'search_function': search_function,
-                                                 'validate_input': validate_input,
-                                                 'text': text,
-                                                 'state': state}
+        self.cell_options[datarn]['dropdown'] = get_dropdown_dict(**kwargs)
         self.set_cell_data(datarn = datarn, 
-                           value = set_value if set_value is not None else values[0] if values else "")
-        if redraw:
-            self.MT.refresh()
+                           value = kwargs['set_value'] if kwargs['set_value'] is not None else kwargs['values'][0] if kwargs['values'] else "")
     
     def get_dropdown_height_anchor(self, datarn, text_editor_h = None):
         win_h = 5
-        for i, v in enumerate(self.cell_options[datarn]['dropdown']['values']):
+        for i, v in enumerate(self.get_cell_kwargs(datacn, key = 'dropdown')['values']):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
                 win_h += self.MT.fl_ins + (v_numlines * self.MT.xtra_lines_increment) + 5 # end of cell
             else:
-                win_h += self.MT.min_rh
+                win_h += self.MT.min_row_height
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
         space_bot = self.MT.get_space_bot(0, text_editor_h)
         win_h2 = int(win_h)
         if win_h > space_bot:
@@ -1646,69 +1713,71 @@
             
     # r is displayed row
     def open_dropdown_window(self, r, datarn = None, event = None):
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window()
         if datarn is None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if self.cell_options[datarn]['dropdown']['state'] == "normal":
-            if not self.edit_cell_(r = r, dropdown = True, event = event):
+        kwargs = self.get_cell_kwargs(datarn, key = 'dropdown')
+        if kwargs['state'] == "normal":
+            if not self.open_text_editor(event = event, r = r, dropdown = True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(datarn)
         window = self.MT.parentframe.dropdown_class(self.MT.winfo_toplevel(),
                                                     r,
                                                     0,
                                                     width = self.current_width,
                                                     height = win_h,
-                                                    font = self.MT._font,
+                                                    font = self.MT.index_font,
                                                     colors = {'bg': self.MT.popup_menu_bg, 
                                                               'fg': self.MT.popup_menu_fg, 
                                                               'highlight_bg': self.MT.popup_menu_highlight_bg,
                                                               'highlight_fg': self.MT.popup_menu_highlight_fg},
                                                     outline_color = self.MT.popup_menu_fg,
-                                                    values = self.cell_options[datarn]['dropdown']['values'],
+                                                    values = kwargs['values'],
                                                     close_dropdown_window = self.close_dropdown_window,
-                                                    search_function = self.cell_options[datarn]['dropdown']['search_function'],
+                                                    search_function = kwargs['search_function'],
                                                     arrowkey_RIGHT = self.MT.arrowkey_RIGHT,
                                                     arrowkey_LEFT = self.MT.arrowkey_LEFT,
                                                     align = "w",
                                                     single_index = "r")
         ypos = self.MT.row_positions[r + 1]
-        self.cell_options[datarn]['dropdown']['canvas_id'] = self.create_window((0, ypos),
-                                                                               window = window,
-                                                                               anchor = anchor)
-        if self.cell_options[datarn]['dropdown']['state'] == "normal":
+        kwargs['canvas_id'] = self.create_window((0, ypos),
+                                                 window = window,
+                                                 anchor = anchor)
+        if kwargs['state'] == "normal":
             self.text_editor.textedit.bind("<<TextModified>>", 
                                            lambda x: window.search_and_see(DropDownModifiedEvent("IndexComboboxModified", r, 0, self.text_editor.get())))
-            if self.cell_options[datarn]['dropdown']['modified_function'] is not None:
-                window.modified_function = self.cell_options[datarn]['dropdown']['modified_function']
+            if kwargs['modified_function'] is not None:
+                window.modified_function = kwargs['modified_function']
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
                 self.after(2, self.text_editor.scroll_to_bottom())
             except:
                 return
             redraw = False
         else:
             window.bind("<FocusOut>", lambda x: self.close_dropdown_window(r))
             self.update_idletasks()
             window.focus_set()
             redraw = True
         self.existing_dropdown_window = window
-        self.cell_options[datarn]['dropdown']['window'] = window
-        self.existing_dropdown_canvas_id = self.cell_options[datarn]['dropdown']['canvas_id']
+        kwargs['window'] = window
+        self.existing_dropdown_canvas_id = kwargs['canvas_id']
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True, redraw_table = False)
             
     # r is displayed row
     def close_dropdown_window(self, r = None, selection = None, redraw = True):
         if r is not None and selection is not None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            if self.cell_options[datarn]['dropdown']['select_function'] is not None: # user has specified a selection function
-                self.cell_options[datarn]['dropdown']['select_function'](EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
+            kwargs = self.get_cell_kwargs(datarn, key = 'dropdown')
+            if kwargs['select_function'] is not None: # user has specified a selection function
+                kwargs['select_function'](EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
             if self.extra_end_edit_cell_func is None:
                 self.set_cell_data_undo(r, datarn = datarn, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
                 if validation is not None:
                     selection = validation
                 self.set_cell_data_undo(r, datarn = datarn, value = selection, redraw = not redraw)
@@ -1758,28 +1827,49 @@
         except:
             pass
         self.existing_dropdown_canvas_id = None
         try:
             self.existing_dropdown_window.destroy()
         except:
             pass
-        if datarn_ in self.cell_options and 'dropdown' in self.cell_options[datarn_]:
-            self.cell_options[datarn_]['dropdown']['canvas_id'] = "no dropdown open"
-            self.cell_options[datarn_]['dropdown']['window'] = "no dropdown open"
+        kwargs = self.get_cell_kwargs(datarn_, key = 'dropdown')
+        if kwargs:
+            kwargs['canvas_id'] = "no dropdown open"
+            kwargs['window'] = "no dropdown open"
             try:
-                self.delete(self.cell_options[datarn_]['dropdown']['canvas_id'])
+                self.delete(kwargs['canvas_id'])
             except:
                 pass
         self.existing_dropdown_window = None
+    
+    def get_cell_kwargs(self, datarn, key = 'dropdown', cell = True, entire = True):
+        if cell and datarn in self.cell_options and key in self.cell_options[datarn]:
+            return self.cell_options[datarn][key]
+        if entire and key in self.options:
+            return self.options[key]
+        return {}
+        
+    def delete_options_dropdown(self):
+        self.destroy_opened_dropdown_window()
+        if 'dropdown' in self.options:
+            del self.options['dropdown']
+        
+    def delete_options_checkbox(self):
+        if 'checkbox' in self.options:
+            del self.options['checkbox']
+            
+    def delete_options_dropdown_and_checkbox(self):
+        self.delete_options_dropdown()
+        self.delete_options_checkbox()
 
-    def delete_dropdown(self, datarn):
+    def delete_cell_options_dropdown(self, datarn):
         self.destroy_opened_dropdown_window(datarn = datarn)
         if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
             del self.cell_options[datarn]['dropdown']
 
-    def delete_checkbox(self, datarn):
+    def delete_cell_options_checkbox(self, datarn):
         if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
             del self.cell_options[datarn]['checkbox']
 
-    def delete_dropdown_and_checkbox(self, datarn):
-        self.delete_dropdown(datarn)
-        self.delete_checkbox(datarn)
+    def delete_cell_options_dropdown_and_checkbox(self, datarn):
+        self.delete_cell_options_dropdown(datarn)
+        self.delete_cell_options_checkbox(datarn)
```

### Comparing `tksheet-6.0.2/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.0.3/tksheet/_tksheet_top_left_rectangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.tag_bind("rw", "<Leave>", self.rw_leave)
         self.tag_bind("rh", "<Leave>", self.rh_leave)
         self.bind("<Motion>", self.mouse_motion)
         self.bind("<ButtonPress-1>", self.b1_press)
         self.bind("<B1-Motion>", self.b1_motion)
         self.bind("<ButtonRelease-1>", self.b1_release)
         self.bind("<Double-Button-1>", self.double_b1)
-        self.bind(get_rc_binding(), self.rc)
+        self.bind(rc_binding, self.rc)
 
     def rw_state(self, state = "normal"):
         self.itemconfig("rw", state = state)
 
     def rh_state(self, state = "normal"):
         self.itemconfig("rh", state = state)
 
@@ -69,22 +69,22 @@
     def basic_bindings(self, enable = True):
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
-            self.bind(get_rc_binding(), self.rc)
+            self.bind(rc_binding, self.rc)
         else:
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
-            self.unbind(get_rc_binding())
+            self.unbind(rc_binding)
 
     def set_dimensions(self, new_w = None, new_h = None):
         try:
             if new_w:
                 self.config(width = new_w)
                 w = new_w
                 h = self.winfo_height()
@@ -103,24 +103,25 @@
         if self.extra_motion_func is not None:
             self.extra_motion_func(event)
 
     def b1_press(self, event = None):
         self.focus_set()
         rect = self.find_overlapping(event.x, event.y, event.x, event.y)
         if not rect:
-            if self.MT.select_all_enabled and not self.MT.all_selected():
+            if self.MT.select_all_enabled:
+                self.MT.deselect("all")
                 self.MT.select_all()
             else:
                 self.MT.deselect("all")
         elif rect[0] == 1:
             if self.RI.width_resizing_enabled:
-                self.RI.set_width(self.RI.default_width, set_TL = True)
+                self.RI.set_width(self.RI.default_index_width, set_TL = True)
         elif rect[0] == 2:
             if self.CH.height_resizing_enabled:
-                self.CH.set_height(self.MT.default_hh[1], set_TL = True)
+                self.CH.set_height(self.MT.default_header_h[1], set_TL = True)
         self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
 
     def b1_motion(self, event = None):
         self.focus_set()
         if self.extra_b1_motion_func is not None:
```

### Comparing `tksheet-6.0.2/tksheet/_tksheet_vars.py` & `tksheet-6.0.3/tksheet/_tksheet_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # for mac bindings
 from platform import system as get_os
 
 USER_OS = f"{get_os()}".lower()
 ctrl_key = "Command" if USER_OS == "darwin" else "Control"
+rc_binding = "<2>" if USER_OS == "darwin" else "<3>"
 symbols_set = set("""!#\$%&'()*+,-./:;"@[]^_`{|}~>?= """)
 nonelike = {None, 'none', ''}
 truthy = {True, "true", "t", "yes", "y", "on", "1", 1, 1.0}
 falsy = {False, "false", "f", "no", "n", "off", "0", 0, 0.0}
 
 arrowkey_bindings_helper = {"tab": "Tab",
                             "up": "Up",
                             "right": "Right",
                             "left": "Left",
                             "down": "Down",
                             "prior": "Prior",
                             "next": "Next"}
+emitted_events = {"<<SheetModified>>", }
 
 def get_font():
     return ("Calibri", 13 if USER_OS == "darwin" else 11, "normal")
 
 def get_index_font():
     return ('Calibri', 13 if USER_OS == "darwin" else 11, "normal")
```

### Comparing `tksheet-6.0.2/tksheet.egg-info/PKG-INFO` & `tksheet-6.0.3/tksheet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.0.2
+Version: 6.0.3
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.0.2.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.3.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

