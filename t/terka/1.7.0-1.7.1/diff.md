# Comparing `tmp/terka-1.7.0.tar.gz` & `tmp/terka-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.7.0.tar", last modified: Wed Apr 26 19:54:36 2023, max compression
+gzip compressed data, was "terka-1.7.1.tar", last modified: Sun Apr 30 19:50:32 2023, max compression
```

## Comparing `terka-1.7.0.tar` & `terka-1.7.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/
--rw-r--r--   0 am        (1000) am        (1000)      292 2023-04-26 19:54:36.686519 terka-1.7.0/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-26 19:54:36.686519 terka-1.7.0/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      903 2023-04-26 19:51:31.000000 terka-1.7.0/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.682520 terka-1.7.0/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.0/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.0/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41931 2023-04-26 19:48:32.000000 terka-1.7.0/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)     1556 2023-04-26 19:48:32.000000 terka-1.7.0/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.0/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.0/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)     1538 2023-04-26 19:48:32.000000 terka-1.7.0/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.0/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-26 19:47:22.000000 terka-1.7.0/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    26315 2023-04-26 19:48:32.000000 terka-1.7.0/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     1427 2023-04-26 19:47:22.000000 terka-1.7.0/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7747 2023-04-26 19:47:22.000000 terka-1.7.0/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-26 19:54:36.686519 terka-1.7.0/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      292 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-26 19:54:36.000000 terka-1.7.0/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-30 19:50:32.984289 terka-1.7.1/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-04-30 19:50:32.980288 terka-1.7.1/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-30 19:50:32.984289 terka-1.7.1/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      903 2023-04-30 19:50:24.000000 terka-1.7.1/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-30 19:50:32.976288 terka-1.7.1/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-30 19:50:32.980288 terka-1.7.1/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.1/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.1/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-30 19:50:32.980288 terka-1.7.1/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41987 2023-04-30 09:58:41.000000 terka-1.7.1/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1556 2023-04-26 19:48:32.000000 terka-1.7.1/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-30 19:50:32.980288 terka-1.7.1/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.1/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.1/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1538 2023-04-26 19:48:32.000000 terka-1.7.1/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.1/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-30 19:50:32.980288 terka-1.7.1/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.7.1/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-30 19:50:32.980288 terka-1.7.1/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.1/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    29368 2023-04-30 19:47:46.000000 terka-1.7.1/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.1/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.1/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.1/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.7.1/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7860 2023-04-30 11:10:05.000000 terka-1.7.1/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-30 19:50:32.976288 terka-1.7.1/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-04-30 19:50:32.000000 terka-1.7.1/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-30 19:50:32.000000 terka-1.7.1/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-30 19:50:32.000000 terka-1.7.1/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-04-30 19:50:32.000000 terka-1.7.1/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-30 19:50:32.000000 terka-1.7.1/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-30 19:50:32.000000 terka-1.7.1/terka.egg-info/top_level.txt
```

### Comparing `terka-1.7.0/setup.py` & `terka-1.7.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.7.0",
+    version="1.7.1",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.7.0/terka/adapters/orm.py` & `terka-1.7.1/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/adapters/repository.py` & `terka-1.7.1/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/collaborators.py` & `terka-1.7.1/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/commands.py` & `terka-1.7.1/terka/domain/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -861,15 +861,16 @@
         elif command == "show":
             if len(kwargs) == 1 and "project" in kwargs:
                 kwargs["id"] = kwargs["project"]
                 del kwargs["project"]
             print_options = printer.PrintOptions(
                 show_history=bool(kwargs.pop("show_history", False)),
                 show_commentaries=bool(kwargs.pop("show_commentaries", False)),
-                show_completed=bool(kwargs.pop("show_completed", False)))
+                show_completed=bool(kwargs.pop("show_completed", False)),
+                show_viz=kwargs.pop("show_viz", False))
             if kwargs.pop("partial_project_view", False):
                 print_options.show_epics = bool(kwargs.pop("epics", False))
                 print_options.show_tasks = bool(kwargs.pop("tasks", False))
                 print_options.show_stories = bool(kwargs.pop("stories", False))
             if entity_type == "tasks":
                 print_options.show_completed = True
             if not (task_id := kwargs.get("id")):
```

### Comparing `terka-1.7.0/terka/domain/commentary.py` & `terka-1.7.1/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/epic.py` & `terka-1.7.1/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/event_history.py` & `terka-1.7.1/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/project.py` & `terka-1.7.1/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/sprint.py` & `terka-1.7.1/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/story.py` & `terka-1.7.1/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/tag.py` & `terka-1.7.1/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/task.py` & `terka-1.7.1/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/domain/time_tracker.py` & `terka-1.7.1/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/entrypoints/cli.py` & `terka-1.7.1/terka/entrypoints/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,14 +92,33 @@
             logger.warning(f"Current focus is {focus_type}: {task_id or project_name}")
 
         task_dict = format_task_dict(config, args, kwargs)
         task_dict = update_task_dict(task_dict, repo)
         logger.debug(task_dict)
 
         command, entity = args.command, args.entity
+        if file_path := task_dict.get("file"):
+            with open(file_path, "r") as f:
+                lines = [line.rstrip() for line in f if line.rstrip()]
+                for line in lines:
+                    entry = line.strip().split("::")
+                    if not entry:
+                        continue
+                    match entry:
+                        case [project, name, description]:
+                            task_dict = {"name": name, "project": project, "description": description}
+                        case [project, name]:
+                            task_dict = {"name": name, "project": project}
+                        case [name]:
+                            task_dict = {"name": name}
+                        case _:
+                            raise Exception("Unknown format")
+                    task_dict = update_task_dict(task_dict, repo)
+                    command_handler.execute(command, entity, task_dict)
+            exit()
         is_interactive = False
         if not command and not entity:
             is_interactive = True
             interactive_message = f"[green]>>> Running terka in an interactive mode[/green]"
             if task_id:
                 interactive_message = f"{interactive_message} (focus task {task_id})"
             elif project_name:
```

### Comparing `terka-1.7.0/terka/service_layer/printer.py` & `terka-1.7.1/terka/service_layer/printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import Any, Dict, List, Optional, Tuple
 from dataclasses import dataclass
 from operator import attrgetter
 import inspect
 from copy import deepcopy
 
 from collections import defaultdict
+import itertools
 from datetime import datetime, date, timedelta
 import plotext as plt
 import rich
+import pandas as pd
+import numpy as np
+import matplotlib.pyplot
 from rich.console import Console
 from rich.table import Table
 from statistics import mean, median
 
 from terka.service_layer import services, views
 from terka.service_layer.ui import TerkaTask
 
@@ -20,14 +24,15 @@
 class PrintOptions:
     show_tasks: bool = True
     show_history: bool = False
     show_commentaries: bool = False
     show_completed: bool = False
     show_epics: bool = True
     show_stories: bool = True
+    show_viz: bool = False
 
 
 class Printer:
 
     def __init__(self, repo, box=rich.box.SIMPLE) -> None:
         self.console = Console()
         self.box = box
@@ -75,15 +80,16 @@
         if entity_type == "sprints":
             if entities:
                 self.print_sprint(entities, repo, print_options, kwargs)
             else:
                 exit(f"No sprint with id '{task}' found!")
         if entity_type in ("epics", "stories"):
             if entities:
-                self.print_composite(entities, repo, print_options, entity_type)
+                self.print_composite(entities, repo, print_options,
+                                     entity_type)
             else:
                 exit(f"No {entity_type} with id '{task}' found!")
         if entity_type == "projects":
             if entities:
                 self.print_project(entities, print_options, kwargs)
             else:
                 exit(f"No project '{task}' found!")
@@ -116,17 +122,17 @@
             self.print_user(entities=entities)
         elif type == "sprints":
             self.print_sprint(entities=entities,
                               repo=repo,
                               print_options=print_options)
         elif type in ("epics", "stories"):
             self.print_composite(entities=entities,
-                            repo=repo,
-                            print_options=print_options,
-                            composite_type=type)
+                                 repo=repo,
+                                 print_options=print_options,
+                                 composite_type=type)
         else:
             self.print_default_entity(self, entities)
 
     def print_user(self, entities):
         table = Table(box=self.box)
         for column in ("id", "name"):
             table.add_column(column)
@@ -253,23 +259,49 @@
                             print_options=task_print_options,
                             story_points=story_points,
                             kwargs=kwargs,
                             show_window=False)
         if i == 0 and print_options.show_commentaries and (
                 commentaries := entities[0].commentaries):
             self.print_commentaries(commentaries)
-        time_entries = views.time_spent(repo.session, entity.start_date,
-                                        entity.end_date)
-        dates = [entry.get("date") for entry in time_entries]
-        times = [entry.get("time_spent_hours") for entry in time_entries]
-        plt.date_form('Y-m-d')
-        plt.plot_size(100, 15)
-        plt.title("Time tracker")
-        plt.bar(dates, times)
-        plt.show()
+        if viz := print_options.show_viz:
+            if "cfd" in viz:
+                dates = [
+                    date.strftime("%Y-%m-%d")
+                    for date in pd.date_range(entity.start_date, entity.end_date).
+                    to_pydatetime().tolist()
+                ]
+                status_changes = views.status_changes(repo.session, 2)
+                placeholders = pd.DataFrame(data=list(
+                    itertools.product([task.id for task in tasks], dates)),
+                                            columns=["task", "date"])
+                history = self._restore_status_history(placeholders, status_changes)
+                # TODO: aggreggate history ty date and number of tasks within the state
+                # plt.date_form('Y-m-d')
+                # y = range(1, 10)
+                # y2 = range(2, 20, 2)
+                # y3 = range(3, 30, 3)
+                # y4 = range(4, 40, 4)
+                # y5 = range(5, 50, 5)
+                # plt.plot(dates, y2,  fillx=True, color="green", label="TODO")
+                # plt.plot(dates, y3,  fillx=False, color="blue", label="IN_PROGRESS")
+                # plt.plot(dates, y4,  fillx=False, color="red", label="REVIEW")
+                # plt.plot(dates, y5,  fillx=False, color="black", label="DONE")
+                # plt.plot_size(50, 15)
+                # plt.show()
+            if "time" in viz:
+                time_entries = views.time_spent(repo.session, entity.start_date,
+                                                entity.end_date)
+                dates = [entry.get("date") for entry in time_entries]
+                times = [entry.get("time_spent_hours") for entry in time_entries]
+                plt.date_form('Y-m-d')
+                plt.plot_size(100, 15)
+                plt.title("Time tracker")
+                plt.bar(dates, times)
+                plt.show()
 
     def print_project(self, entities, print_options, kwargs=None):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD, expand=True)
         non_active_projects = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "name", "description", "status", "open_tasks",
                        "overdue", "stale", "backlog", "todo", "in_progress",
                        "review", "done", "median_task_age"):
@@ -328,18 +360,20 @@
         if non_active_projects.row_count:
             self.console.print("[green]Inactive projects[/green]")
             self.console.print(non_active_projects)
         non_task_view_options = deepcopy(print_options)
         non_task_view_options.show_tasks = False
         if print_options.show_epics and (epics := entity.epics):
             self.console.print("")
-            self.print_composite(epics, self.repo, non_task_view_options, "epics")
+            self.print_composite(epics, self.repo, non_task_view_options,
+                                 "epics")
         if print_options.show_stories and (stories := entity.stories):
             self.console.print("")
-            self.print_composite(stories, self.repo, non_task_view_options, "stories")
+            self.print_composite(stories, self.repo, non_task_view_options,
+                                 "stories")
         if print_options.show_tasks and (tasks := entity.tasks):
             task_print_options = deepcopy(print_options)
             task_print_options.show_commentaries = False
             self.console.print("")
             self.print_task(entities=tasks,
                             repo=self.repo,
                             print_options=task_print_options,
@@ -588,7 +622,35 @@
         # if print_options.show_commentaries and (commentaries :=
         #                                         entity.commentaries):
         #     self.print_commentaries(commentaries)
         # # TODO: not working
         # if print_options.show_history and (history := entity.history):
         #     self.print_history(history)
         return table, completed_tasks, completed_story_points
+
+    def _restore_status_history(self, placeholders, status_history):
+        partial_history = status_history[status_history["last_status_for_date"].notnull()]
+        current_values = status_history[["task", "current_status"]].drop_duplicates()
+        if not partial_history.empty:
+            joined = pd.merge(placeholders,
+                              partial_history,
+                              on=["task", "date"],
+                              how="left")
+            joined = joined.replace({np.nan: None})
+            joined["filled_backward"] = joined.groupby(
+                "task")["first_status_for_date"].bfill()
+            joined["filled_forward"] = joined.groupby(
+                "task")["last_status_for_date"].ffill()
+            joined["filled_forward"] = joined.groupby(
+                "task")["filled_forward"].fillna(
+                    joined.pop("filled_backward"))
+            joined = pd.merge(joined,
+                              current_values,
+                              on="task",
+                              how="left")
+            joined["status"] = joined["filled_forward"]
+        else:
+            joined = pd.merge(placeholders,
+                              current_values,
+                              on="task",
+                              how="left")
+        return joined[["date", "task", "status"]]
```

### Comparing `terka-1.7.0/terka/service_layer/services.py` & `terka-1.7.1/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/service_layer/ui.py` & `terka-1.7.1/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/service_layer/vertical_layout.css` & `terka-1.7.1/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.7.0/terka/utils.py` & `terka-1.7.1/terka/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
             "show_history": new_dict.get("show-history"),
             "show_commentaries": new_dict.get("show-commentaries") or new_dict.get("show-comments"),
             "epics": new_dict.get("epics"),
             "stories": new_dict.get("stories"),
             "tasks": new_dict.get("tasks"),
             "external_project": new_dict.get("external-project"),
             "external_task": new_dict.get("external-task"),
+            "show_viz": new_dict.get("show-viz"),
+            "file": new_dict.get("file") or new_dict.get("f"),
         }
         if "--show-completed" in kwargs:
             task_dict.update({"show_completed": True})
         if "--sort" in kwargs:
             sort_statement = kwargs[kwargs.index("--sort"):]
             task_dict.update(create_task_dict(sort_statement))
     elif len(kwargs) == 1:
```

### Comparing `terka-1.7.0/terka.egg-info/SOURCES.txt` & `terka-1.7.1/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

