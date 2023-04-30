# Comparing `tmp/absl_extra-0.0.5.tar.gz` & `tmp/absl_extra-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.5.tar", last modified: Sat Apr 29 00:40:11 2023, max compression
+gzip compressed data, was "absl_extra-0.0.6.tar", last modified: Sun Apr 30 09:23:30 2023, max compression
```

## Comparing `absl_extra-0.0.5.tar` & `absl_extra-0.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1266 2023-04-29 00:39:56.816630 absl_extra-0.0.5/Readme.md
--rw-r--r--   0        0        0     5481 2023-04-29 00:39:56.816630 absl_extra-0.0.5/absl_extra.py
--rw-r--r--   0        0        0     6066 2023-04-29 00:39:56.816630 absl_extra-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 absl_extra-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1400 2023-04-30 09:23:17.613395 absl_extra-0.0.6/Readme.md
+-rw-r--r--   0        0        0     5550 2023-04-30 09:23:17.613395 absl_extra-0.0.6/absl_extra.py
+-rw-r--r--   0        0        0     6066 2023-04-30 09:23:17.613395 absl_extra-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 absl_extra-0.0.6/PKG-INFO
```

### Comparing `absl_extra-0.0.5/Readme.md` & `absl_extra-0.0.6/Readme.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 It will:
 - Notify on execution start, finish or failed.
   - By default, Notifier will just log those out to `stdout`.
   - I prefer receiving those in Slack, though (see example below).
 - Log parsed CLI flags from `absl.flags.FLAGS` and config values from `config_file:get_config()`
 - Inject `ml_collections.ConfigDict` from `config_file`, if kwarg provided.
 - Inject `pymongo.collection.Collection` if `mongo_config` kwarg provided.
+- `log_after` and `log_before` decorators, which proved extremely usefully for print-debugging.
 
 Minimal example
 ```python
 import os
 import functools
 from pymongo.collection import Collection
 from absl import flags, app
@@ -29,12 +30,14 @@
     mongo_config=MongoConfig(
         uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
     ),
     notifier=SlackNotifier(
         slack_token=os.environ["SLACK_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
     ),
 )
-def main(cmd: str, config: ConfigDict, db: Collection) -> None: ...
+def main(cmd: str, config: ConfigDict, db: Collection) -> None:
+    # Do all the heavy lifting. 
+    pass
 
 if __name__ == "__main__":
     app.run(main)
 ```
```

### Comparing `absl_extra-0.0.5/absl_extra.py` & `absl_extra-0.0.6/absl_extra.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 import json
 from importlib import util
-from typing import Callable, NamedTuple
+from typing import Callable, NamedTuple, TypeVar
 from functools import partial, wraps
 from absl import app, flags, logging
 import inspect
 
+T = TypeVar("T", bound=Callable, covariant=True)
+
 
 if util.find_spec("pymongo"):
     from pymongo import MongoClient
 else:
     logging.warning("pymongo not installed.")
 
 
@@ -41,84 +43,83 @@
     import slack_sdk
 
     class SlackNotifier(Notifier):
         def __init__(self, slack_token: str, channel_id: str):
             self.slack_token = slack_token
             self.channel_id = channel_id
 
-        def notify_job_started(self, cmd: str):
+        def notify_job_started(self, name: str):
             slack_client = slack_sdk.WebClient(token=self.slack_token)
             slack_client.chat_postMessage(
                 channel=self.channel_id,
                 blocks=[
                     {
                         "type": "section",
                         "text": {
                             "type": "mrkdwn",
-                            "text": f" :ballot_box_with_check: Job {cmd} started.",
+                            "text": f" :ballot_box_with_check: Job {name} started.",
                         },
                     }
                 ],
                 text="Job Started!",
             )
 
-        def notify_job_finished(self, cmd: str):
+        def notify_job_finished(self, name: str):
             slack_client = slack_sdk.WebClient(token=self.slack_token)
             slack_client.chat_postMessage(
                 channel=self.channel_id,
                 blocks=[
                     {
                         "type": "section",
                         "text": {
                             "type": "mrkdwn",
-                            "text": f":white_check_mark: Job {cmd} finished execution.",
+                            "text": f":white_check_mark: Job {name} finished execution.",
                         },
                     }
                 ],
                 text="Job Finished!",
             )
 
-        def notify_job_failed(self, cmd: str, ex: Exception):
+        def notify_job_failed(self, name: str, exception: Exception):
             slack_client = slack_sdk.WebClient(token=self.slack_token)
             slack_client.chat_postMessage(
                 channel=self.channel_id,
                 blocks=[
                     {
                         "type": "section",
                         "text": {
                             "type": "mrkdwn",
-                            "text": f":x: Job {cmd} failed, reason:\n ```{ex}```",
+                            "text": f":x: Job {name} failed, reason:\n ```{exception}```",
                         },
                     }
                 ],
                 text="Job Finished!",
             )
-            raise ex
 
 else:
     logging.warning("slack_sdk not installed.")
 
 
 class ExceptionHandlerImpl(app.ExceptionHandler):
-    def __init__(self, cmd: str, notifier: Notifier):
-        self.cmd = cmd
+    def __init__(self, name: str, notifier: Notifier):
+        self.cmd = name
         self.notifier = notifier
 
-    def handle(self, exc: Exception):
-        self.notifier.notify_job_failed(self.cmd, exc)
-        raise exc
+    def handle(self, exception: Exception):
+        self.notifier.notify_job_failed(self.cmd, exception)
 
 
 def hook_main(
     main: Callable,
+    *,
     app_name: str | None = None,
     notifier: Notifier | None = None,
     config_file: str | None = None,
     mongo_config: MongoConfig | None = None,
-):
+) -> Callable:
     if notifier is None:
         notifier = Notifier()
     if util.find_spec("ml_collections") and config_file is not None:
         config = config_flags.DEFINE_config_file("config")
     else:
         config = None
     if util.find_spec("pymongo") and mongo_config is not None:
@@ -156,28 +157,28 @@
         notifier.notify_job_started(app_name)
         app.run(partial(main, **kwargs))
         notifier.notify_job_finished(app_name)
 
     return wrapper
 
 
-def log_before(func, logger=logging.debug):
+def log_before(func: T, logger=logging.debug) -> T:
     @wraps(func)
     def wrapper(*args, **kwargs):
         func_args = inspect.signature(func).bind(*args, **kwargs).arguments
         func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
         logger(
             f"Entered {func.__module__}.{func.__qualname__} with args ( {func_args_str} )"
         )
         return func(*args, **kwargs)
 
     return wrapper
 
 
-def log_after(func, logger=logging.debug):
+def log_after(func: T, logger=logging.debug) -> T:
     @wraps(func)
-    def wrapper(*func_args, **func_kwargs):
-        retval = func(*func_args, **func_kwargs)
+    def wrapper(*args, **kwargs):
+        retval = func(*args, **kwargs)
         logger("Exited " + func.__name__ + "() with value: " + repr(retval))
         return retval
 
     return wrapper
```

### Comparing `absl_extra-0.0.5/pyproject.toml` & `absl_extra-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "absl_extra"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.5"  # Required
+version = "0.0.6"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A wrapper to run and monitor absl app."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `absl_extra-0.0.5/PKG-INFO` & `absl_extra-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.5
+Version: 0.0.6
 Summary: A wrapper to run and monitor absl app.
 Keywords: 
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,15 @@
 It will:
 - Notify on execution start, finish or failed.
   - By default, Notifier will just log those out to `stdout`.
   - I prefer receiving those in Slack, though (see example below).
 - Log parsed CLI flags from `absl.flags.FLAGS` and config values from `config_file:get_config()`
 - Inject `ml_collections.ConfigDict` from `config_file`, if kwarg provided.
 - Inject `pymongo.collection.Collection` if `mongo_config` kwarg provided.
+- `log_after` and `log_before` decorators, which proved extremely usefully for print-debugging.
 
 Minimal example
 ```python
 import os
 import functools
 from pymongo.collection import Collection
 from absl import flags, app
@@ -51,13 +52,15 @@
     mongo_config=MongoConfig(
         uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
     ),
     notifier=SlackNotifier(
         slack_token=os.environ["SLACK_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
     ),
 )
-def main(cmd: str, config: ConfigDict, db: Collection) -> None: ...
+def main(cmd: str, config: ConfigDict, db: Collection) -> None:
+    # Do all the heavy lifting. 
+    pass
 
 if __name__ == "__main__":
     app.run(main)
 ```
```

