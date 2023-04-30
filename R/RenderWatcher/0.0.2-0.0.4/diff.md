# Comparing `tmp/RenderWatcher-0.0.2-py3-none-any.whl.zip` & `tmp/RenderWatcher-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4854 bytes, number of entries: 8
+Zip file size: 5160 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-20 18:46 render_watcher/__init__.py
--rw-rw-r--  2.0 unx     1957 b- defN 23-Jan-11 13:34 render_watcher/core.py
--rw-rw-r--  2.0 unx     5078 b- defN 22-Dec-28 11:40 render_watcher/ui.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jan-11 13:49 RenderWatcher-0.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      296 b- defN 23-Jan-11 13:49 RenderWatcher-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-11 13:49 RenderWatcher-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Jan-11 13:49 RenderWatcher-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 23-Jan-11 13:49 RenderWatcher-0.0.2.dist-info/RECORD
-8 files, 9165 bytes uncompressed, 3710 bytes compressed:  59.5%
+-rw-rw-r--  2.0 unx     1571 b- defN 23-Apr-13 12:17 render_watcher/core.py
+-rw-rw-r--  2.0 unx     6889 b- defN 23-Apr-30 14:13 render_watcher/ui.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-30 14:16 RenderWatcher-0.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      296 b- defN 23-Apr-30 14:16 RenderWatcher-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-30 14:16 RenderWatcher-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-30 14:15 RenderWatcher-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-30 14:16 RenderWatcher-0.0.4.dist-info/RECORD
+8 files, 10590 bytes uncompressed, 4016 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: render_watcher/core.py
 Comment: 
 
 Filename: render_watcher/ui.py
 Comment: 
 
-Filename: RenderWatcher-0.0.2.dist-info/LICENSE
+Filename: RenderWatcher-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: RenderWatcher-0.0.2.dist-info/METADATA
+Filename: RenderWatcher-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: RenderWatcher-0.0.2.dist-info/WHEEL
+Filename: RenderWatcher-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: RenderWatcher-0.0.2.dist-info/top_level.txt
+Filename: RenderWatcher-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: RenderWatcher-0.0.2.dist-info/RECORD
+Filename: RenderWatcher-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## render_watcher/core.py

```diff
@@ -1,58 +1,56 @@
 import json
 import os
 import subprocess
 import threading
 
 from katana_render_submitter import util
 
-
 PACKAGE_DIR = '/tlg/shows/{}/tmp'.format(util.get_shot_context())
 
 
-#TODO, want to inspect the job, create a dictionary of this, max the threads at 4?
-#e.g {job:{thread1:pass1, thread2:pass2, thread3:pass3, thread4:pass4}}
+def get_rendered_frames(render_path):
+    """"Gets the number of rendered frames"""
+    return len(os.listdir(render_path))
+
 
 def get_render_jobs():
-    jobs = [j for j in os.listdir(PACKAGE_DIR) if j.endswith('.json')]
+    jobs = {}
+    # get jobs
+    for job in os.listdir(PACKAGE_DIR):
+        if job.endswith('.json'):
+            full_path = f'{PACKAGE_DIR}/{job}'
+            jobs[job] = os.path.getmtime(full_path)
+    # sort into list by time
     if jobs:
-        return jobs
+        sorted_jobs = sorted(jobs.items(), key=lambda x: x[1], reverse=True)
+        return sorted_jobs
     else:
         return None
 
 
 def get_job_data(job_id):
     json_file = '{}/{}'.format(PACKAGE_DIR, job_id)
     f = open(json_file)
     job_data = json.load(f)
     f.close()
     return job_data
 
 
 def launch_render(main_widget, tree_widget, data):
+    #TODO dont need the extra arguments which arent being used
     threaded_dict = {}
     if tree_widget.topLevelItemCount() == 0:
         print ('need to load job first')
         return False
     for k, v in data.items():
         for pass_info in v:
             rndr_cmd = pass_info.get('batch_cmd')
-            # here we need to break this down into frame chunks
-            frames = pass_info.get('frame_range')
-            frame_range_split = frames.split('-')
+            #frames = pass_info.get('frame_range')
             pass_name = pass_info.get('pass_name')
-            frame_start = int(frame_range_split[0])
-            frame_end = int(frame_range_split[1])
             # run the threads
-            t = threading.Thread(target=render_thread_job, args=(main_widget, rndr_cmd, frame_start, frame_end, pass_name), daemon=False)
+            t = threading.Thread(target=render_thread_job, args=(main_widget, rndr_cmd, pass_name), daemon=False)
             t.start()
-            #NON THREADED RENDER
-            #render_thread_job(main_widget, rndr_cmd, frame_start, frame_end, pass_name)
 
 
-def render_thread_job(main_widget, rndr_cmd, frame_start, frame_end, pass_name):
+def render_thread_job(main_widget, rndr_cmd, pass_name):
     subprocess.run(rndr_cmd)
-    #TODO this will run slower and is more efficient, but does update the progress bars.
-    # for frame in range(frame_start, frame_end):
-    #     rndr_cmd[5] = '--t={}'.format(frame)
-    #     subprocess.run(rndr_cmd)
-    #     main_widget.update_progress(frame, pass_name)
```

## render_watcher/ui.py

```diff
@@ -1,134 +1,178 @@
 from PyQt5 import QtWidgets, QtCore
+from PyQt5.QtCore import QObject, QThread, pyqtSignal
 import sys
+import time
 
 from render_watcher import core
 
+RENDER_WATCHER = object()
 
 
-#TODO/NICE TO HAVES
+# TODO/NICE TO HAVES
 '''
-sort by latest jobs
-add latest job button
-update status when rendering and completed (with colour!) 
 do style sheets, probably look like katana
 add title for window
-centre text in columns, add
+centre text in columns, RESIZE APPROPRIATE
 '''
 
+class Worker(QObject):
+    finished = pyqtSignal()
+    progress = pyqtSignal(int)
+    def run(self):
+        rendering = True
+        render_status = dict()
+        tree_widget = RENDER_WATCHER.render_tree_widget
+        status_data = tree_widget.status_data
+        #TODO can prob do this in one line
+        for pass_name in status_data.keys():
+            render_status[pass_name] = True
+        # update the status column
+        job_item = tree_widget.topLevelItem(0)
+        for i in range(job_item.childCount()):
+            child_item = job_item.child(i)
+            child_item.setText(2, 'RUNNING')
+        while rendering:
+            # we only want to check each render passes progress every 30 secs
+            time.sleep(30)
+            for pass_name, data in status_data.items():
+                if render_status.get(pass_name) is True:
+                    output_path = data.get('output_path')
+                    widget_item = data.get('widget_item')
+                    progress_widget = tree_widget.itemWidget(widget_item, 5)
+                    num_frames = data.get('num_frames')
+                    #TODO this is overkill and should be set initally first
+                    widget_item.setText(2, 'RUNNING')
+                    current_frames = core.get_rendered_frames(output_path)
+                    #update progress bar
+                    progress_widget.setValue(current_frames)
+                    if current_frames == num_frames:
+                        widget_item.setText(2, 'COMPLETE')
+                        render_status[pass_name] = False
+                    #check to see if all passes have finished rendering
+                    if any(render_status.values()) is False:
+                        rendering = False
+        RENDER_WATCHER.launch_render_button.setEnabled(True)
+        self.finished.emit()
 
 class RenderWatcherTree(QtWidgets.QTreeWidget):
     def __init__(self, parent=None):
         super(RenderWatcherTree, self).__init__(parent)
         self.setColumnCount(5)
-        self.setHeaderLabels(['Job id', 'RenderPass', 'Status', 'FrameRange', 'Progress'])
+        self.setHeaderLabels(['Job id', 'RenderPass', 'Status', 'FrameRange', 'Version', 'Progress'])
+        self.status_data = dict()
         # TODO open in expanded state
 
-
     def populate_tree(self, data):
         for key, values in data.items():
             job_item = QtWidgets.QTreeWidgetItem([key])
             self.insertTopLevelItems(0, [job_item])
             for pass_info in values:
                 frame_range = pass_info.get('frame_range')
-                child_item = QtWidgets.QTreeWidgetItem(['', pass_info.get('pass_name'), 'WAITING', frame_range, ''])
+                version = pass_info.get('version')
+                child_item = QtWidgets.QTreeWidgetItem(['', pass_info.get('pass_name'), 'WAITING', frame_range, version, ''])
                 job_item.addChild(child_item)
+                self.status_data[pass_info.get('pass_name')] = {
+                    'widget_item': child_item,
+                    'output_path': pass_info.get('output_path'),
+                    'num_frames': int(pass_info.get('num_frames'))
+                }
                 progress_bar = QtWidgets.QProgressBar()
                 progress_bar.setTextVisible(True)
-                start_frame = int(frame_range.split('-')[0])
-                end_frame = int(frame_range.split('-')[1])
-                progress_bar.setMinimum(start_frame)
-                progress_bar.setMaximum(end_frame)
-                self.setItemWidget(child_item, 4, progress_bar)
+                progress_bar.setMinimum(0)
+                progress_bar.setMaximum(int(pass_info.get('num_frames')))
+                self.setItemWidget(child_item, 5, progress_bar)
+
+    def update_status(self):
+        pass
+
+    def update_progress(self):
+        pass
+
+
+class JobsTree(QtWidgets.QTreeWidget):
+    def __init__(self, parent=None):
+        super(JobsTree, self).__init__(parent)
+        self.setColumnCount(2)
+        self.setHeaderLabels(['Job Name', 'Submission Date'])
+
+    def populate_tree(self, jobs):
+        for job in jobs:
+            job_item = QtWidgets.QTreeWidgetItem([job[0], time.ctime(job[1])])
+            # Add the new item to the tree
+            self.addTopLevelItem(job_item)
 
 
 class RenderWatcher(QtWidgets.QWidget):
     def __init__(self):
         super().__init__()
         self.selected_job = None
+        self.arrange_layout()
+        self.populate_render_job_widget()
+        self.connect_signals()
+
+    def arrange_layout(self):
+        # self.showMaximized()
         layout_main = QtWidgets.QVBoxLayout()
-        self.showMaximized()
         self.setLayout(layout_main)
         view_widgets_hbox = QtWidgets.QHBoxLayout()
         layout_main.addLayout(view_widgets_hbox)
-        self.tree = RenderWatcherTree()
-        view_widgets_hbox.addWidget(self.tree)
-        self.render_job_window = QtWidgets.QListWidget()
-        view_widgets_hbox.addWidget(self.render_job_window)
+        self.render_tree_widget = RenderWatcherTree()
+        view_widgets_hbox.addWidget(self.render_tree_widget)
+        self.jobs_tree_widget = JobsTree()
+        view_widgets_hbox.addWidget(self.jobs_tree_widget)
         buttons_hbox = QtWidgets.QHBoxLayout()
         layout_main.addLayout(buttons_hbox)
         self.load_job_btn = QtWidgets.QPushButton('Load Job')
         self.launch_render_button = QtWidgets.QPushButton('Launch Render')
         buttons_hbox.addWidget(self.launch_render_button)
         buttons_hbox.addWidget(self.load_job_btn)
-        self.populate_render_job_widget()
-        self.connect_signals()
+
+
+    def run_check_render_status_task(self):
+        """"Initializes the threading work"""
+        self.thread = QThread()
+        self.worker = Worker()
+        self.worker.moveToThread(self.thread)
+        # Step 5: Connect signals and slots
+        # TODO move these to the signals connect_signals
+        self.thread.started.connect(self.worker.run)
+        self.worker.finished.connect(self.thread.quit)
+        self.worker.finished.connect(self.worker.deleteLater)
+        self.thread.finished.connect(self.thread.deleteLater)
+        self.launch_render_button.setEnabled(False)
+        self.thread.start()
 
     def connect_signals(self):
         self.load_job_btn.clicked.connect(self.load_job_btn_clicked)
         self.launch_render_button.clicked.connect(self.launch_render_btn_clicked)
 
     def load_job_btn_clicked(self):
-        curent_item = self.render_job_window.currentItem()
+        curent_item = self.jobs_tree_widget.currentItem()
         if not curent_item:
-            #TODO put a dialog here
-            pass
-        id_txt = curent_item.text()
+            return
+        id_txt = curent_item.text(0)
         self.selected_job = id_txt
         data = core.get_job_data(id_txt)
-        self.tree.populate_tree(data)
+        self.render_tree_widget.populate_tree(data)
 
     def launch_render_btn_clicked(self):
-        if self.tree.topLevelItemCount() == 0:
+        if self.render_tree_widget.topLevelItemCount() == 0:
             print('need to load job first')
             return False
         data = core.get_job_data(self.selected_job)
-        core.launch_render(self, self.tree, data)
-
+        core.launch_render(self, self.render_tree_widget, data)
+        self.run_check_render_status_task()
 
-    # def launch_render(self):
-    #     if self.tree.topLevelItemCount() == 0:
-    #         print ('need to load job first')
-    #         return False
-    #     print ('is this really running?')
-    #     for k, v in self.render_data.items():
-    #         for pass_info in v:
-    #             rndr_cmd = pass_info.get('batch_cmd')
-    #             # here we need to break this down into frame chunks
-    #             frames = pass_info.get('frame_range')
-    #             frame_range_split = frames.split('-')
-    #             frame_start = int(frame_range_split[0])
-    #             frame_end = int(frame_range_split[1])
-    #             frame_range_count = frame_end-frame_start
-    #             for frame in range(frame_start, frame_end):
-    #                 rndr_cmd[5] = str(frame)
-    #                 subprocess.run(rndr_cmd)
-    #                 self.update_progress(frame, pass_info.get('pass_name'))
-
-    def update_progress(self, frame_number, pass_name):
-        # get widget
-        #TODO revisit this if neededm current iterator method is not very efficient
-        #item = self.tree.findItems(pass_name, QtCore.Qt.MatchExactly, 2)
-        iterator = QtWidgets.QTreeWidgetItemIterator(
-            self.tree,
-            flags=QtWidgets.QTreeWidgetItemIterator.NoChildren
-        )
-        while iterator.value():
-            item = iterator.value()
-            if pass_name == item.text(1):
-                progress_widget = self.tree.itemWidget(item, 4)
-                progress_widget.setValue(frame_number + 1)
-                break
-            iterator += 1
 
     def populate_render_job_widget(self):
         jobs = core.get_render_jobs()
-        self.render_job_window.addItems(jobs)
-
+        if jobs:
+            self.jobs_tree_widget.populate_tree(jobs)
 
 
-def launch_render_watcher(arg):
-    # running from terminal
-    app = QtWidgets.QApplication(arg)
-    render_watcher = RenderWatcher()
-    render_watcher.show()
+def launch_render_watcher():
+    global RENDER_WATCHER
+    app = QtWidgets.QApplication(sys.argv)
+    RENDER_WATCHER = RenderWatcher()
+    RENDER_WATCHER.show()
     sys.exit(app.exec_())
```

## Comparing `RenderWatcher-0.0.2.dist-info/LICENSE` & `RenderWatcher-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `RenderWatcher-0.0.2.dist-info/RECORD` & `RenderWatcher-0.0.4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 render_watcher/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-render_watcher/core.py,sha256=dL5sknmLmuEG1tmdY_EqLcO7v5D9zTqKHKrteiAdXuQ,1957
-render_watcher/ui.py,sha256=J5A9AGNVGLejSZvyYfhtx6iFfNwfE8wPZy5xIWzHjhA,5078
-RenderWatcher-0.0.2.dist-info/LICENSE,sha256=1XA4KGQxKUlItNfQukbpovOFHE8ZKmtvPHbCNe2mO5M,1073
-RenderWatcher-0.0.2.dist-info/METADATA,sha256=LhKoopfzGQY3MbdRtCMLqbiRRBoiD54ZQIEGeMXieaQ,296
-RenderWatcher-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-RenderWatcher-0.0.2.dist-info/top_level.txt,sha256=ceKnBToGlQjvKbDbXiSJ1gFtrF0Lhak3mQwC6Idh_Fk,18
-RenderWatcher-0.0.2.dist-info/RECORD,,
+render_watcher/core.py,sha256=9b3MjGEewl9udXjaSti-IUsp5coNqg2tIkUiD6bdz5I,1571
+render_watcher/ui.py,sha256=pugG7d_3U1kkXK59haPDFIg38nMcanE7tfyFwIOY45s,6889
+RenderWatcher-0.0.4.dist-info/LICENSE,sha256=1XA4KGQxKUlItNfQukbpovOFHE8ZKmtvPHbCNe2mO5M,1073
+RenderWatcher-0.0.4.dist-info/METADATA,sha256=hBzgwW32MWfAOJgqzAiU4cxoslontW2lD76HcGNBWKM,296
+RenderWatcher-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+RenderWatcher-0.0.4.dist-info/top_level.txt,sha256=ceKnBToGlQjvKbDbXiSJ1gFtrF0Lhak3mQwC6Idh_Fk,18
+RenderWatcher-0.0.4.dist-info/RECORD,,
```

