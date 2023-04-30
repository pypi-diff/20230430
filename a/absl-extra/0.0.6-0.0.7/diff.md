# Comparing `tmp/absl_extra-0.0.6.tar.gz` & `tmp/absl_extra-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.6.tar", last modified: Sun Apr 30 09:23:30 2023, max compression
+gzip compressed data, was "absl_extra-0.0.7.tar", last modified: Sun Apr 30 14:03:04 2023, max compression
```

## Comparing `absl_extra-0.0.6.tar` & `absl_extra-0.0.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1400 2023-04-30 09:23:17.613395 absl_extra-0.0.6/Readme.md
--rw-r--r--   0        0        0     5550 2023-04-30 09:23:17.613395 absl_extra-0.0.6/absl_extra.py
--rw-r--r--   0        0        0     6066 2023-04-30 09:23:17.613395 absl_extra-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 absl_extra-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1404 2023-04-30 14:02:55.689952 absl_extra-0.0.7/Readme.md
+-rw-r--r--   0        0        0     5647 2023-04-30 14:02:55.689952 absl_extra-0.0.7/absl_extra.py
+-rw-r--r--   0        0        0     6066 2023-04-30 14:02:55.689952 absl_extra-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2140 1970-01-01 00:00:00.000000 absl_extra-0.0.7/PKG-INFO
```

### Comparing `absl_extra-0.0.6/Readme.md` & `absl_extra-0.0.7/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     hook_main,
     app_name="some_name",
     config_file="config.py",
     mongo_config=MongoConfig(
         uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
     ),
     notifier=SlackNotifier(
-        slack_token=os.environ["SLACK_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
+        slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
     ),
 )
 def main(cmd: str, config: ConfigDict, db: Collection) -> None:
     # Do all the heavy lifting. 
     pass
 
 if __name__ == "__main__":
```

### Comparing `absl_extra-0.0.6/absl_extra.py` & `absl_extra-0.0.7/absl_extra.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
+import functools
 import json
 from importlib import util
-from typing import Callable, NamedTuple, TypeVar
-from functools import partial, wraps
+from typing import Callable, NamedTuple, TypeVar, Mapping
+from functools import wraps
 from absl import app, flags, logging
 import inspect
 
 T = TypeVar("T", bound=Callable, covariant=True)
 
 
 if util.find_spec("pymongo"):
@@ -25,22 +26,22 @@
 class MongoConfig(NamedTuple):
     uri: str
     db_name: str
     collection: str | None = None
 
 
 class Notifier:
-    def notify_job_started(self, cmd: str):
-        logging.info(f"Job {cmd} started.")
+    def notify_job_started(self, name: str):
+        logging.info(f"Job {name} started.")
 
-    def notify_job_finished(self, cmd: str):
-        logging.info(f"Job {cmd} finished.")
+    def notify_job_finished(self, name: str):
+        logging.info(f"Job {name} finished.")
 
-    def notify_job_failed(self, cmd: str, ex: Exception):
-        logging.fatal(f"Job {cmd} failed", exc_info=ex)
+    def notify_job_failed(self, name: str, exception: Exception):
+        logging.fatal(f"Job {name} failed", exc_info=exception)
 
 
 if util.find_spec("slack_sdk"):
     import slack_sdk
 
     class SlackNotifier(Notifier):
         def __init__(self, slack_token: str, channel_id: str):
@@ -97,72 +98,70 @@
 
 else:
     logging.warning("slack_sdk not installed.")
 
 
 class ExceptionHandlerImpl(app.ExceptionHandler):
     def __init__(self, name: str, notifier: Notifier):
-        self.cmd = name
+        self.name = name
         self.notifier = notifier
 
     def handle(self, exception: Exception):
-        self.notifier.notify_job_failed(self.cmd, exception)
+        self.notifier.notify_job_failed(self.name, exception)
 
 
 def hook_main(
     main: Callable,
     *,
-    app_name: str | None = None,
+    app_name: str = "absl_app",
     notifier: Notifier | None = None,
     config_file: str | None = None,
-    mongo_config: MongoConfig | None = None,
+    mongo_config: MongoConfig | Mapping[str, ...] | None = None,
 ) -> Callable:
+    main_kwargs = {}
+
     if notifier is None:
         notifier = Notifier()
     if util.find_spec("ml_collections") and config_file is not None:
         config = config_flags.DEFINE_config_file("config")
+        main_kwargs["config"] = config.value
     else:
         config = None
+
     if util.find_spec("pymongo") and mongo_config is not None:
+        if isinstance(mongo_config, Mapping):
+            mongo_config = MongoConfig(**mongo_config)
         db = MongoClient(mongo_config.uri).get_database(mongo_config.db_name)
         if mongo_config.collection is not None:
             db = db.get_collection(mongo_config.collection)
-    else:
-        db = None
-
-    @wraps(main)
-    def wrapper(cmd: str):
-        if app_name is None:
-            _app_name = cmd
-        else:
-            _app_name = app_name
-
-        app.install_exception_handler(ExceptionHandlerImpl(cmd, notifier))
-
-        kwargs = {}
-        if config is not None:
-            logging.info(
-                f"Config: {json.dumps(config.value, sort_keys=True, indent=4)}"
-            )
-            logging.info("-" * 50)
-            kwargs["config"] = config.value
-        if db is not None:
-            kwargs["db"] = db
+        main_kwargs["db"] = db
 
+    def init_callback():
         logging.info("-" * 50)
         logging.info(
             f"Flags: {json.dumps(flags.FLAGS.flag_values_dict(), sort_keys=True, indent=4)}"
         )
+        if config is not None:
+            logging.info(
+                f"Config: {json.dumps(config.value, sort_keys=True, indent=4)}"
+            )
         logging.info("-" * 50)
 
         notifier.notify_job_started(app_name)
-        app.run(partial(main, **kwargs))
+
+    app.install_exception_handler(ExceptionHandlerImpl(app_name, notifier))
+    app.call_after_init(init_callback)
+
+    @wraps(main)
+    def wrapper(*args, **kwargs):
+        ret_val = main(*args, **kwargs)
         notifier.notify_job_finished(app_name)
+        return ret_val
 
-    return wrapper
+    return functools.partial(wrapper, **main_kwargs)
 
 
 def log_before(func: T, logger=logging.debug) -> T:
     @wraps(func)
     def wrapper(*args, **kwargs):
         func_args = inspect.signature(func).bind(*args, **kwargs).arguments
         func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
```

### Comparing `absl_extra-0.0.6/pyproject.toml` & `absl_extra-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "absl_extra"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.6"  # Required
+version = "0.0.7"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A wrapper to run and monitor absl app."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `absl_extra-0.0.6/PKG-INFO` & `absl_extra-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper to run and monitor absl app.
 Keywords: 
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -49,15 +49,15 @@
     hook_main,
     app_name="some_name",
     config_file="config.py",
     mongo_config=MongoConfig(
         uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
     ),
     notifier=SlackNotifier(
-        slack_token=os.environ["SLACK_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
+        slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
     ),
 )
 def main(cmd: str, config: ConfigDict, db: Collection) -> None:
     # Do all the heavy lifting. 
     pass
 
 if __name__ == "__main__":
```

