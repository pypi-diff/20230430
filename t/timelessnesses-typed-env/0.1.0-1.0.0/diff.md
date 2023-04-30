# Comparing `tmp/timelessnesses_typed_env-0.1.0.tar.gz` & `tmp/timelessnesses_typed_env-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelessnesses_typed_env-0.1.0.tar", max compression
+gzip compressed data, was "timelessnesses_typed_env-1.0.0.tar", max compression
```

## Comparing `timelessnesses_typed_env-0.1.0.tar` & `timelessnesses_typed_env-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1097 2023-04-29 06:54:03.098295 timelessnesses_typed_env-0.1.0/LICENSE
--rw-r--r--   0        0        0      519 2023-04-29 08:28:25.328240 timelessnesses_typed_env-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1202 2023-04-29 08:39:37.782078 timelessnesses_typed_env-0.1.0/README.md
--rw-r--r--   0        0        0     6394 2023-04-29 08:35:36.485960 timelessnesses_typed_env-0.1.0/timelessnesses/typed_env.py
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 timelessnesses_typed_env-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-04-29 06:54:03.098295 timelessnesses_typed_env-1.0.0/LICENSE
+-rw-r--r--   0        0        0      519 2023-04-30 07:09:19.050393 timelessnesses_typed_env-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1852 2023-04-30 07:20:58.468969 timelessnesses_typed_env-1.0.0/README.md
+-rw-r--r--   0        0        0     8591 2023-04-30 07:22:58.594773 timelessnesses_typed_env-1.0.0/timelessnesses/typed_env.py
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 timelessnesses_typed_env-1.0.0/PKG-INFO
```

### Comparing `timelessnesses_typed_env-0.1.0/LICENSE` & `timelessnesses_typed_env-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timelessnesses_typed_env-0.1.0/pyproject.toml` & `timelessnesses_typed_env-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timelessnesses-typed-env"
-version = "0.1.0"
+version = "1.0.0"
 description = "A python module that help you have a type safety on enviroment variable"
 authors = ["timelessnesses <mooping3roblox@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "timelessnesses"}]
 homepage = "https://github.com/timelessnesses/typed_env"
```

### Comparing `timelessnesses_typed_env-0.1.0/timelessnesses/typed_env.py` & `timelessnesses_typed_env-1.0.0/timelessnesses/typed_env.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from enum import Enum
 from json import loads
 from typing import Any, Callable, Optional
-
+import os
 from dotenv import dotenv_values
-
+import warnings
 
 def int_validator(value: Optional[str]) -> int:
     if value is None:
         raise ValueError("Value is None")
     return int(value)
 
 
@@ -115,14 +115,18 @@
     Optional[dict]: optional_dict_validator,
     bool: bool_validator,
     Optional[bool]: optional_bool_validator,
     list: list_validator,
     Optional[list]: optional_list_validator
 }
 
+class Method(Enum):
+    dotenv = 0
+    env = 1
+    all = 2
 
 class TypedEnv:
     """
     This class consists of methods to load environment variables from .env file.
     You should subclass this class then add your own types and default values.
     Only supported types are\n
     int\n
@@ -132,27 +136,60 @@
     bool\n
     But you can extend it with your own type converters by using add_validator method with a type and a function that takes string (optionally).
     Or you can overwrite the validators dict to your own!
     """
 
     types: dict[str, object] = {}
     validators: dict[object, Callable[[Optional[str]], object]] = {}
+    envs: dict[str, Optional[str]] = {}
+    raise_error_on_unknown_env_op: bool = True
 
     def __init_subclass__(cls) -> None:
         cls.types = {}
 
         for key, value in cls.__annotations__.items():
             cls.types[key] = value
         cls.validators.update(default_validators)
 
-    def load(self, dotenv: Optional[str] = None, **kwargs) -> None:
-        envs = dotenv_values(dotenv_path=dotenv, **kwargs)
+    def get_env(self,method: Method=Method.dotenv,dotenv:Optional[str] = None,**kwargs):
+        """
+        This method loads environment variables from .env file or os.environ or both.
+        Default way to get enviroment variable is from .env file currently. You can change it with Method Enum.
+        You HAVE to call this method before load method.
+        """
+        
+        if method == Method.env and dotenv is not None:
+            raise ValueError("dotenv argument is not needed when method is Method.env")
+        elif method in (Method.dotenv, Method.all) and dotenv is None:
+            raise ValueError("dotenv argument is required when method is Method.dotenv or Method.all")
+        if method == Method.dotenv:
+            self.envs = dotenv_values(dotenv,**kwargs)
+        elif method == Method.env:
+            self.envs = dict(os.environ)
+        elif method == Method.all:
+            self.envs = {**dict(os.environ),**dotenv_values(dotenv,**kwargs)}
+        else:
+            raise ValueError("Unknown method")
+        
+    def raise_error_on_unknown_env(self, enable: bool):
+        """
+        When this is enabled, if there is an environment variable that is not defined in the class, it will raise an error, else it will raise a warning.
+        """
+        self.raise_error_on_unknown_env_op = enable
+
+    def load(self) -> None:
+        """
+        Load environment variables from .env file or os.environ or both based on get_env method.
+        """
+        envs = self.envs
+        if not envs:
+            raise ValueError("No environment variables were loaded!")
         successful = {}
         for key, value in envs.items():
-            if key in self.types:
+            if key in self.types.keys():
                 try:
                     value = self.validators[self.types[key]](value)
                 except ValueError as e:
                     raise ValueError(f"Error while parsing {key} (type {self.types[key]}).") from e
                 except KeyError as e:
                     raise ValueError(f"Unknown type {self.types[key]}") from e
                 if value is not None:
@@ -160,26 +197,39 @@
                     successful[key] = value
                 else:
                     if not hasattr(self, key) and self.types[key] is not Optional:
                         raise ValueError(f"Variable {key} was not set!")
                     elif not hasattr(self, key) and self.types[key] is Optional:
                         setattr(self, key, None)
                 continue
-            raise ValueError(f"Unknown type {self.types[key]}")
+            if self.raise_error_on_unknown_env_op:
+                raise ValueError(f"Unknown variable {key}")
+            else:
+                warnings.warn(f"Unknown variable {key}")
         # now we check if any enviroment variable were not used and any variable that we didn't set
         for key, value in self.types.items():
             if key not in successful:
                 if value is not Optional:
                     raise ValueError(f"Variable {key} was not set!")
                 else:
                     if hasattr(self, key):
                         continue
                     else:
                         setattr(self, key, None)
 
     def add_validator(
         self, type_: object, validator: Callable[[Optional[str]], object]
     ) -> None:
+        """
+        Add a validator for a type.
+        This is important if you have custom type like a class or an enum.
+        NOTE: If there's same type it will get overwritten.
+        """
         self.validators[type_] = validator
     
     def export_as_dict(self) -> dict:
+        
+        """
+        Exporting all variables as a dict.
+        NOTE: This will not export variables that are not set. So you had to call load method before this.
+        """
         return {key: getattr(self, key) for key in self.types.keys()}
```

