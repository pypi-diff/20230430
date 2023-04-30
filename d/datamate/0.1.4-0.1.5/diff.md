# Comparing `tmp/datamate-0.1.4.tar.gz` & `tmp/datamate-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamate-0.1.4.tar", last modified: Tue Apr  4 14:27:02 2023, max compression
+gzip compressed data, was "datamate-0.1.5.tar", last modified: Sun Apr 30 17:33:14 2023, max compression
```

## Comparing `datamate-0.1.4.tar` & `datamate-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-04-04 14:27:02.342611 datamate-0.1.4/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-04-04 14:27:02.341996 datamate-0.1.4/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3642 2023-03-06 13:58:32.000000 datamate-0.1.4/README.md
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-04-04 14:27:02.334900 datamate-0.1.4/datamate/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      612 2023-03-15 22:43:05.000000 datamate-0.1.4/datamate/__init__.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968    46384 2023-03-28 09:59:41.000000 datamate-0.1.4/datamate/directory.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968    10264 2023-04-04 14:26:02.000000 datamate-0.1.4/datamate/namespaces.py
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-04-04 14:27:02.338465 datamate-0.1.4/datamate.egg-info/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-04-04 14:27:02.000000 datamate-0.1.4/datamate.egg-info/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      292 2023-04-04 14:27:02.000000 datamate-0.1.4/datamate.egg-info/SOURCES.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968        1 2023-04-04 14:27:02.000000 datamate-0.1.4/datamate.egg-info/dependency_links.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      109 2023-04-04 14:27:02.000000 datamate-0.1.4/datamate.egg-info/requires.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968        9 2023-04-04 14:27:02.000000 datamate-0.1.4/datamate.egg-info/top_level.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968       38 2023-04-04 14:27:02.342755 datamate-0.1.4/setup.cfg
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      715 2023-04-04 14:26:56.000000 datamate-0.1.4/setup.py
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-04-04 14:27:02.340934 datamate-0.1.4/tests/
--rwxr-xr-x   0 lappalainenj (1483866292) 1899195968    17040 2023-03-28 10:03:49.000000 datamate-0.1.4/tests/test_directory.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3747 2023-04-04 14:23:09.000000 datamate-0.1.4/tests/test_namespaces.py
+drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-04-30 17:33:14.398858 datamate-0.1.5/
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3829 2023-04-30 17:33:14.398000 datamate-0.1.5/PKG-INFO
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3642 2023-03-06 13:58:32.000000 datamate-0.1.5/README.md
+drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-04-30 17:33:14.393271 datamate-0.1.5/datamate/
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      612 2023-03-15 22:43:05.000000 datamate-0.1.5/datamate/__init__.py
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    50945 2023-04-30 17:25:37.000000 datamate-0.1.5/datamate/directory.py
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    10441 2023-04-24 19:52:52.000000 datamate-0.1.5/datamate/namespaces.py
+drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-04-30 17:33:14.396179 datamate-0.1.5/datamate.egg-info/
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3829 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/PKG-INFO
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      292 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/SOURCES.txt
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        1 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/dependency_links.txt
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      109 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/requires.txt
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        9 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/top_level.txt
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)       38 2023-04-30 17:33:14.399105 datamate-0.1.5/setup.cfg
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      715 2023-04-24 21:33:17.000000 datamate-0.1.5/setup.py
+drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-04-30 17:33:14.397348 datamate-0.1.5/tests/
+-rwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    21665 2023-04-30 17:00:43.000000 datamate-0.1.5/tests/test_directory.py
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3747 2023-04-04 14:23:09.000000 datamate-0.1.5/tests/test_namespaces.py
```

### Comparing `datamate-0.1.4/PKG-INFO` & `datamate-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.1.4
+Version: 0.1.5
 Summary: A data organization and compilation system.
 Author: Janne Lappalainen & Mason McGill
 Description-Content-Type: text/markdown
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
```

### Comparing `datamate-0.1.4/README.md` & `datamate-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `datamate-0.1.4/datamate/__init__.py` & `datamate-0.1.5/datamate/__init__.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.4/datamate/directory.py` & `datamate-0.1.5/datamate/directory.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import json
 from pathlib import Path
 import shutil
 import functools
 import threading
 from time import sleep
 import inspect
+from numbers import Number
 from typing import (
     Any,
     Iterator,
     List,
     Mapping,
     MutableMapping,
     Optional,
@@ -59,17 +60,23 @@
     pass
 
 
 class ModifiedError(Exception):
     pass
 
 
-# -- Static type definitions ---------------------------------------------------
+class ImplementationWarning(Warning):
+    pass
+
+
+class ImplementationError(Exception):
+    pass
+
 
-from pathlib import Path as Path
+# -- Static type definitions ---------------------------------------------------
 
 
 class ArrayFile(Protocol):
     """
     A property that corresponds to a single-array HDF5 file
     """
 
@@ -342,39 +349,50 @@
         pass
 
     path: Path
     config: Config
 
     def __new__(cls, *args: object, **kwargs: object) -> Any:
         path, config = _parse_directory_args(args, kwargs)
-        if path is None and config is None:
-            return _directory(cls)
-        elif path is not None and config is None:
-            return _check_size(_directory_from_path(cls, _resolve_path(path)))
+        cls = _directory(cls)
+        _check_implementation(cls)
+        if config is None and has_defaults_for_init(cls) and _implements_init(cls):
+            config = get_defaults(cls)
+        # breakpoint()
+        if path is not None and config is None:
+            cls = _check_size(_directory_from_path(cls, _resolve_path(path)))
         elif path is None and config is not None:
-            return _check_size(_directory_from_config(cls, config))
+            cls = _check_size(_directory_from_config(cls, config))
         elif path is not None and config is not None:
-            return _check_size(
+            cls = _check_size(
                 _directory_from_path_and_config(cls, _resolve_path(path), config)
             )
+        elif path is None and config is None:
+            if _implements_init(cls):
+                # raise ValueError("no configuration provided")
+                pass
+
+        cls.__doc__ = _update_doc(cls)
+
+        return cls
 
     def __init__(self, config: Config):
         """Implement to compile data at runtime from a configuration."""
         pass
 
     @property
     def meta(self) -> Namespace:
         """
         The metadata stored in `{self.path}/_meta.yaml`
         """
         return read_meta(self.path)
 
     @property
     def config(self):
-        return self.meta.config
+        return self.meta.config or self._config
 
     @property
     def status(self):
         return self.meta.status
 
     # -- MutableMapping methods ----------------------------
 
@@ -788,14 +806,32 @@
             if file.is_file() and file.suffix == suffix:
                 file.unlink()
 
 
 # -- Directory construction -----------------------------------------------------
 
 
+def get_defaults(cls):
+    if "Config" in cls.__dict__:
+        defaults = {
+            k: v
+            for k, v in cls.Config.__dict__.items()
+            if not (k.startswith("_") or (k.startswith("__") and k.endswith("__")))
+        }
+        return Namespace(defaults)
+    return Namespace({})
+
+
+def get_annotations(cls):
+    if "Config" in cls.__dict__:
+        annotations = getattr(cls.Config, "__annotations__", {})
+        return Namespace(annotations)
+    return Namespace({})
+
+
 def _parse_directory_args(
     args: Tuple[object, ...], kwargs: Mapping[str, object]
 ) -> Tuple[Optional[Path], Optional[Mapping[str, object]]]:
     """
     Return `(path, conf)` or raise an error.
     """
     # ()
@@ -863,67 +899,119 @@
             "    - Directory(path: Path|str)\n"
             "    - Directory(path: Path|str, conf: Mapping[str, object])\n"
             "    - Directory(name: str)\n"
             "    - Directory(name: str, conf: Mapping[str, object])"
         )
 
 
+def _implements_init(cls: type) -> bool:
+    """True if the class implements `__init__`."""
+    return inspect.getsource(cls.__init__).split("\n")[-2].replace(" ", "") != "pass"
+
+
+def has_defaults_for_init(cls):
+    """Directory subclasses that specify
+
+    class Config:
+        foo = 1
+        bar = 2
+
+    and are constructed without arguments will be initialized with
+    `foo=1` and `bar=2`.
+    """
+    return (
+        "Config" in cls.__class__.__dict__
+        # and len(inspect.signature(cls.__init__).parameters) == 1
+        and get_defaults(cls.__class__)
+    )
+
+
+def _check_implementation(cls):
+    defaults = get_defaults(cls.__class__)
+
+    if not defaults:
+        # check if Config only has annotations, no defaults
+        defaults = get_annotations(cls.__class__)
+
+    if _implements_init(cls) and not defaults:
+        with warnings.catch_warnings():
+            warnings.simplefilter("always")
+            warnings.warn(
+                (f"The Directory {type(cls)} implements __init__ but not Config."),
+                ImplementationWarning,
+                stacklevel=2,
+            )
+
+
 def _directory(cls: type) -> Directory:
     """
     Return a new Directory corresponding to the file tree at root_dir / cls.__name___ *
     """
     directory = _forward_subclass(cls, {})
     path = _new_directory_path(type(directory))
     object.__setattr__(directory, "_cached_keys", set())
     object.__setattr__(directory, "path", path)
     return directory
 
 
-def _check_for_init(cls: type) -> bool:
-    # import pdb; pdb.set_trace()
-    return inspect.getsource(cls.__init__).split("\n")[-2].replace(" ", "") != "pass"
-
-
 def _directory_from_path(cls: type, path: Path) -> Directory:
     """
     Return a Directory corresponding to the file tree at `path`.
 
     An error is raised if the type recorded in `_meta.yaml`, if any, is not a
     subtype of `cls`.
     """
+
+    def _has_defaults_for_init(cls):
+        """True if cls implements Config and __init__(self, config)"""
+        return (
+            "Config" in cls.__dict__
+            and len(inspect.signature(cls.__init__).parameters) == 2
+        )
+
     config = read_meta(path).config or {}
     written_type = get_scope().get(config.get("type", None), None)
 
     if path.is_file():
         raise FileExistsError(f"{path} is a file.")
 
-    if context.enforce_config_match:
-        if _check_for_init(cls) and not path.is_dir():
-            raise FileNotFoundError(f"{path} does not exist.")
-
-        if written_type is not None and not issubclass(written_type, cls):
-            raise FileExistsError(
-                f"{path} is a {written_type.__module__}.{written_type.__qualname__}"
-                f", not a {cls.__module__}.{cls.__qualname__}."
-            )
+    # if context.enforce_config_match:
 
-    if context.enforce_config_match:
-        directory = _forward_subclass(cls, config)
+    # if directory is constructed from path that does not exist,
+    # but that does implement an init function method and has no defaults
+    # for the config, raise an error
+    if _implements_init(cls) and not _has_defaults_for_init(cls) and not path.is_dir():
+        raise FileNotFoundError(f"{path} does not exist.")
+
+    # otherwise pass which is important for the case where the directory
+    # is constructed from a path that does not exist
     else:
-        directory = _forward_subclass(cls, {})
+        pass
+
+    if written_type is not None and not issubclass(written_type, type(cls)):
+        raise FileExistsError(
+            f"{path} is a {written_type.__module__}.{written_type.__qualname__}"
+            f", not a {cls.__module__}.{cls.__qualname__}."
+        )
+
+    # if context.enforce_config_match:
+    directory = _forward_subclass(type(cls), config)
+    # else:
+    #     directory = _forward_subclass(type(cls), {})
+
     object.__setattr__(directory, "_cached_keys", set())
     object.__setattr__(directory, "path", path)
     return directory
 
 
 def _directory_from_config(cls: type, conf: Mapping[str, object]) -> Directory:
     """
     Find or build a Directory with the given type and Namespace.
     """
-    directory = _forward_subclass(cls, conf)
+    directory = _forward_subclass(type(cls), conf)
     new_dir_path = _new_directory_path(type(directory))
     object.__setattr__(directory, "_cached_keys", set())
     config = Namespace(**directory._config)
 
     def _new_directory():
         object.__setattr__(directory, "path", new_dir_path)
         # return empty path cause only the type field is populated
@@ -976,15 +1064,15 @@
 
 def _directory_from_path_and_config(
     cls: type, path: Path, conf: Mapping[str, object]
 ) -> Directory:
     """
     Find or build a Directory with the given type, path, and Namespace.
     """
-    directory = _forward_subclass(cls, conf)
+    directory = _forward_subclass(type(cls), conf)
     object.__setattr__(directory, "_cached_keys", set())
     object.__setattr__(directory, "path", path)
 
     if path.exists():
         meta = read_meta(path)
         config = Namespace({"type": _identify(type(directory)), **directory._config})
         if meta.config != config:
@@ -1021,14 +1109,20 @@
 
 def _build(directory: Directory) -> None:
     """
     Create parent directories, invoke `Directory.__init__`, and store metadata.
     """
     # TODO: Fix YAML generation.
 
+    if directory.path.exists() and directory.status == "done":
+        return
+    elif directory.path.exists() and directory.status == "running":
+        sleep(0.01)
+        return _build(directory)
+
     directory.path.mkdir(parents=True)
 
     meta_path = directory.path / "_meta.yaml"
     config = Namespace(**directory._config)
     write_meta = lambda **kwargs: meta_path.write_text(
         json.dumps(_identify_elements(kwargs))
     )
@@ -1042,14 +1136,46 @@
             directory.__init__(*build_args)
         write_meta(config=config, status="done")
     except BaseException as e:
         write_meta(config=config, status="stopped")
         raise e
 
 
+def _update_doc(cls):
+    if "Config" not in cls.__class__.__dict__ or not get_defaults(cls.__class__):
+        return cls.__doc__
+    Config = cls.__class__.__dict__["Config"]
+
+    def clsstrip(string):
+        string = string[string.find("'") + 1 : string.rfind("'")]
+        return string.replace("__main__.", "")
+
+    doc = cls.__doc__
+    if doc is None:
+        doc = ""
+    else:
+        doc += "\n\n"
+    doc += "Initialize from config or leave default:\n"
+    doc += "{}(dict(\n{}))"
+    attributes = ""
+    for k, v in Config.__dict__.items():
+        if not k.startswith("__"):
+            if (
+                hasattr(Config, "__annotations__")
+                and Config.__annotations__.get(k, None) is not None
+            ):
+                annotation = Config.__annotations__.get(k)
+                attributes += f"{k}: {clsstrip(repr(annotation))} = {v},\n"
+            else:
+                attributes += f"{k} = {v},\n"
+
+    name = clsstrip(repr(Config)).replace(".Config", "")
+    return doc.format(name, attributes)
+
+
 def _resolve_path(path: Path) -> Path:
     """
     Dereference ".", "..", "~", and "@".
     """
     if path.parts[0] == "@":
         path = get_root_dir() / "/".join(path.parts[1:])
     return path.expanduser().resolve()
@@ -1123,24 +1249,26 @@
         cls = cls_override
     elif isinstance(cls_override, str):
         try:
             cls = get_scope()[cls_override]
         except KeyError as e:
             raise KeyError(
                 f'"{cls_override}" can\'t be resolved because it is not found'
-                + f" inside the scope of Directory subclasses. Typo?"
-                + " If this happens in the context of autoreload enabled in"
+                + f" inside the current scope of Directory subclasses."
+                + " If this happens unexpectedly with autoreload enabled in"
                 + " a notebook/IPython session, run `datamate.reset_scope(datamate.Directory)`"
                 + " as a workaround or restart the kernel"
                 + f" (background: https://github.com/ipython/ipython/issues/12399)."
             ) from e
 
-    # Construct and return a `Configurable` instance.
+    # Construct and return a Directory instance
     obj = object.__new__(cls)
-    config = Namespace(type=_identify(type(obj)), **config)
+    default_config = get_defaults(cls)
+    default_config.update(config)
+    config = Namespace(type=_identify(type(obj)), **default_config)
     object.__setattr__(obj, "_config", namespacify(config))
     return cast(Directory, obj)
 
 
 # -- I/O -----------------------------------------------------------------------
 
 
@@ -1185,15 +1313,17 @@
     val = np.asarray(val)
     path.parent.mkdir(parents=True, exist_ok=True)
     # mode='a' to read file, create otherwise
     try:
         f = h5.File(path, libver="latest", mode="a")
     except BlockingIOError as e:
         print(e)
-        if "errno = 11" in str(e):  # 11 := Reource temporarily unavailable
+        if "errno = 11" in str(e) or "errno = 35" in str(
+            e
+        ):  # 11, 35 := Reource temporarily unavailable
             sleep(0.1)
             if retry < max_retries:
                 _extend_h5(path, val, retry + 1, max_retries)
             else:
                 raise RecursionError(
                     "maximum retries to extend the dataset"
                     " exceeded, while the resource was unavailable. Because"
@@ -1273,48 +1403,42 @@
         for key in list(directory.keys())
         if isinstance(getattr(directory, key), h5.Dataset)
     }
     return dw_dict
 
 
 def directory_to_df(directory: Directory, dtypes: dict = None) -> DataFrame:
-    def convert(_arr):
-        if isinstance(_arr, np.ndarray):
-            if isinstance(_arr.item(0), (np.character, bytes)):
-                return _arr.astype(str)
-        return _arr
-
+    """Convert a directory to a pandas DataFrame."""
     df_dict = {
         key: getattr(directory, key)[...]
         for key in list(directory.keys())
         if isinstance(getattr(directory, key), h5.Dataset)
     }
 
     # Get the lengths of all datasets.
-    _lengths = {k: len(v) or 1 for k, v in df_dict.items()}
+    nelements = {k: len(v) or 1 for k, v in df_dict.items()}
 
-    lengths, counts = np.unique([val for val in _lengths.values()], return_counts=True)
+    lengths, counts = np.unique([val for val in nelements.values()], return_counts=True)
     most_frequent_length = lengths[np.argmax(counts)]
 
     # If there are single element datasets, just create a new column of most_frequent_length and put the value in each row.
     if lengths.min() == 1:
-        for k, v in _lengths.items():
+        for k, v in nelements.items():
             if v == 1:
                 df_dict[k] = df_dict[k].repeat(most_frequent_length)
 
-    df_dict = valmap(
-        convert,
-        {key: val for key, val in df_dict.items() if len(val) == most_frequent_length},
-    )
+    df_dict = byte_to_str(df_dict)
+
     if dtypes is not None:
         df_dict = {
             k: np.array(v).astype(dtypes[k]) for k, v in df_dict.items() if k in dtypes
         }
-
-    return DataFrame.from_dict(df_dict)
+    return DataFrame.from_dict(
+        {k: v.tolist() if v.ndim > 1 else v for k, v in df_dict.items()}
+    )
 
 
 def tree(
     dir_path: Path,
     level: int = -1,
     limit_to_directories: bool = False,
     length_limit: int = 1000,
@@ -1379,14 +1503,40 @@
             + (f", {files} files" if files else "")
             + (f", {level} levels." if level >= 1 else "")
         )
 
     return tree_string
 
 
+def byte_to_str(obj):
+    """Cast byte elements to string types.
+
+    Note, this function is recursive and will cast all byte elements in a nested
+    list or tuple.
+    """
+    if isinstance(obj, Mapping):
+        return type(obj)({k: byte_to_str(v) for k, v in obj.items()})
+    elif isinstance(obj, np.ndarray):
+        if np.issubdtype(obj.dtype, np.dtype("S")):
+            return obj.astype("U")
+        return obj
+    elif isinstance(obj, list):
+        obj = [byte_to_str(item) for item in obj]
+        return obj
+    elif isinstance(obj, tuple):
+        obj = tuple([byte_to_str(item) for item in obj])
+        return obj
+    elif isinstance(obj, bytes):
+        return obj.decode()
+    elif isinstance(obj, (str, Number)):
+        return obj
+    else:
+        raise TypeError(f"can't cast {obj} of type {type(obj)} to str")
+
+
 # -- Scope search --------------------------------------------------------------
 
 
 def _identify(type_: type) -> str:
     for sym, t in get_scope().items():
         # comparing t == type_ can yield false in combination with
         # ipython autoreload, therefore relying on comparing the __qualname__
```

### Comparing `datamate-0.1.4/datamate/namespaces.py` & `datamate-0.1.5/datamate/namespaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,20 @@
 
     def __eq__(self, other):
         return all_true(compare(namespacify(self), namespacify(other)))
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
+    def without(self, key):
+        """Return a copy of the namespace without the specified key."""
+        _copy = self.deepcopy()
+        _copy.pop(key)
+        return _copy
+
     def is_superset(self, superset):
         _keys_subset = set(self)
         _keys_superset = set(superset)
         return _keys_subset.issubset(_keys_superset)
 
     def is_value_matching_superset(self, subset):
         """
```

### Comparing `datamate-0.1.4/datamate.egg-info/PKG-INFO` & `datamate-0.1.5/datamate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.1.4
+Version: 0.1.5
 Summary: A data organization and compilation system.
 Author: Janne Lappalainen & Mason McGill
 Description-Content-Type: text/markdown
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
```

### Comparing `datamate-0.1.4/setup.py` & `datamate-0.1.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="datamate",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         "pandas",
         "toolz",
         "numpy",
         "typing_extensions",
         "h5py>=3.6.0",
```

### Comparing `datamate-0.1.4/tests/test_directory.py` & `datamate-0.1.5/tests/test_directory.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,21 @@
     Directory,
     Namespace,
     set_root_dir,
     get_root_dir,
     root,
     set_root_context,
 )
-from datamate.directory import ModifiedError, ModifiedWarning, ConfigWarning
+from datamate.directory import (
+    ModifiedError,
+    ModifiedWarning,
+    ConfigWarning,
+    ImplementationWarning,
+    ImplementationError,
+)
 
 # -- Helper functions ----------------------------------------------------------
 
 
 def data_file(path: Path) -> Path:
     path.parent.mkdir(parents=True, exist_ok=True)
     path.write_bytes(np.random.rand(3).tobytes())
@@ -329,45 +335,47 @@
 
 # -- [Subclass tests] Construction ---------------------------------------------
 
 
 class CustomDirectory(Directory):
     n_calls = 0
 
+    class Config:
+        n_zeros: int
+        n_ones: int
+
     def __init__(self, conf) -> None:
         CustomDirectory.n_calls += 1
         self.zeros = np.zeros(conf.n_zeros)
         self.ones = np.ones(conf.n_ones)
 
 
 class AnotherDirectory(Directory):
-    n_calls = 0
-
     def __init__(self) -> None:
-        AnotherDirectory.n_calls += 1
+        AnotherDirectory.Config.n_calls += 1
 
 
 def test_construction_from_nothing(tmp_path: Path) -> None:
     # Setup
     set_root_dir(tmp_path)
-    AnotherDirectory.n_calls = 0
+    AnotherDirectory.Config.n_calls = 0
 
     # Case 1: (not exists)
     a0 = AnotherDirectory()
-    assert AnotherDirectory.n_calls == 0
+    assert AnotherDirectory.Config.n_calls == 0
 
     # Case 2: (exists, empty)
     path = a0.path
     a1 = AnotherDirectory()
     assert path == a1.path
 
     # Case 3: (exists, non-empty)
     a0.__init__()
     a1 = AnotherDirectory()
-    assert AnotherDirectory.n_calls == 1
+    assert AnotherDirectory.Config.n_calls == 1
 
     # Cleanup
     set_root_dir(Path("."))
 
 
 def test_construction_from_path(tmp_path: Path) -> None:
     # Setup
@@ -476,38 +484,50 @@
         CustomDirectory(n_zeros=2, n_ones=3)
 
 
 # -- [Subclass tests] Build customization --------------------------------------
 
 
 class DirectoryWithUnaryBuild(Directory):
+    class Config:
+        prop: int
+
     def __init__(self) -> None:
         self.field = self.config.prop
 
 
 class DirectoryWithBinaryBuild(Directory):
+    class Config:
+        prop: int
+
     def __init__(self, conf) -> None:
         self.field = conf.prop
 
 
 def test_build_customization(tmp_path: Path) -> None:
     a_unary = DirectoryWithUnaryBuild(tmp_path / "unary", prop=10)
-    a_binary = DirectoryWithUnaryBuild(tmp_path / "binary", prop=10)
+    a_binary = DirectoryWithBinaryBuild(tmp_path / "binary", prop=10)
     assert a_unary.field[()] == 10
     assert a_binary.field[()] == 10
 
 
 # -- Test root control ---------------------------------------------------------
 
 
 @pytest.fixture(scope="session")
 def rooted_dir(tmp_path_factory):
     path = tmp_path_factory.mktemp("rooted_dir")
+
     @root(path)
     class RootedDirectory(Directory):
+        class Config:
+            start: int
+            stop: int
+            step: int
+
         def __init__(self, config) -> None:
             self.array = np.arange(config.start, config.stop, config.step)
 
     return RootedDirectory, path
 
 
 def test_root_dir_provided(tmp_path, rooted_dir):
@@ -543,7 +563,162 @@
     dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
     assert dir.path.parent == tmp_path
 
     # case 5: root dir not provided and within context
     with set_root_context(tmp_path / "subdir"):
         dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
         assert dir.path.parent == tmp_path / "subdir"
+
+
+# -- test default config
+
+
+class DefaultConfigDir(Directory):
+    class Config:
+        x: int = 2
+
+    def __init__(self, config) -> None:
+        self.x = np.arange(config.x)
+
+
+class BadImplementation(Directory):
+    # Config has no attributes
+    class Config:
+        pass
+
+    # but has init
+    def __init__(self, config) -> None:
+        self.x = np.arange(config.x)
+
+
+def test_default_config(tmp_path):
+    set_root_dir(tmp_path)
+
+    # from default config
+    dir = DefaultConfigDir()
+    assert isinstance(dir, DefaultConfigDir)
+    assert (dir.x[()] == np.arange(2)).all()
+    assert dir.path.parent == tmp_path
+    _first = dir.path.name
+    assert "DefaultConfigDir" in _first
+
+    # again
+    dir = DefaultConfigDir()
+    assert isinstance(dir, DefaultConfigDir)
+    assert (dir.x[()] == np.arange(2)).all()
+    assert dir.path.parent == tmp_path
+    assert _first == dir.path.name
+
+    # from custom config
+    dir = DefaultConfigDir(x=3)
+    assert isinstance(dir, DefaultConfigDir)
+    assert (dir.x[()] == np.arange(3)).all()
+    assert dir.path.parent == tmp_path
+    assert "DefaultConfigDir" in dir.path.name
+    assert _first != dir.path.name
+
+    # with path from default config
+    dir = DefaultConfigDir(tmp_path / "test3")
+    assert isinstance(dir, DefaultConfigDir)
+    assert (dir.x[()] == np.arange(2)).all()
+    assert dir.path.parent == tmp_path
+    assert "test3" == dir.path.name
+
+    # with path and custom config
+    dir = DefaultConfigDir(tmp_path / "test4", dict(x=3))
+    assert isinstance(dir, DefaultConfigDir)
+    assert (dir.x[()] == np.arange(3)).all()
+    assert dir.path.parent == tmp_path
+    assert "test4" == dir.path.name
+
+    # with name/ path from custom config but directory exists
+    with pytest.raises(FileExistsError):
+        dir = DefaultConfigDir(tmp_path / "test3", dict(x=3))
+
+    # bad implementation warning
+    with pytest.warns(ImplementationWarning):
+        dir = BadImplementation()
+
+    with pytest.warns(ImplementationWarning):
+        with pytest.raises(FileNotFoundError):
+            dir = BadImplementation(tmp_path / "test8")
+
+    # config has no default attributes but directory has init, with custom config
+    with pytest.warns(ImplementationWarning):
+        dir = BadImplementation(dict(x=2))
+        assert (dir.x[()] == np.arange(2)).all()
+
+    with pytest.warns(ImplementationWarning):
+        dir = BadImplementation(tmp_path / "test10", dict(x=2))
+        assert (dir.x[()] == np.arange(2)).all()
+
+    # config has no default attributes but directory has init, with custom, wrong config
+    with pytest.raises(AttributeError):
+        with pytest.warns(ImplementationWarning):
+            dir = BadImplementation(dict(y=2))
+
+    with pytest.raises(AttributeError):
+        with pytest.warns(ImplementationWarning):
+            dir = BadImplementation(tmp_path / "test12", dict(y=2))
+
+
+# -- test auto docstring
+
+
+class AutoDocConfigDir(Directory):
+    """Dir to test auto docstring based on config."""
+
+    class Config:
+        x: int = 2
+        y: float = 2.0
+        q = Namespace(a=1, b=2)
+
+
+class SoloConfigDocDir(Directory):
+    class Config:
+        x: int = 2
+        y: float = 2.0
+        q = Namespace(a=1, b=2)
+
+
+class EmptyConfigDocDir(Directory):
+    """Dir to test auto docstring based on config."""
+
+    class Config:
+        pass
+
+
+class NoConfigDocDir(Directory):
+    """Dir to test auto docstring based on config."""
+
+    pass
+
+
+def test_auto_doc(tmp_path):
+    a = AutoDocConfigDir()
+
+    doc = "Dir to test auto docstring based on config."
+    doc += "\n\n"
+    doc += "Initialize from config or leave default:\n"
+    doc += "{}(dict(\n{}))"
+    doc = doc.format(
+        "test_directory.AutoDocConfigDir",
+        "x: int = 2,\ny: float = 2.0,\nq = Namespace(a=1, b=2),\n",
+    )
+    assert a.__doc__ == doc
+
+    b = SoloConfigDocDir()
+    doc = "Initialize from config or leave default:\n"
+    doc += "{}(dict(\n{}))"
+    doc = doc.format(
+        "test_directory.SoloConfigDocDir",
+        "x: int = 2,\ny: float = 2.0,\nq = Namespace(a=1, b=2),\n",
+    )
+    assert b.__doc__ == doc
+
+    c = EmptyConfigDocDir()
+    doc = "Dir to test auto docstring based on config."
+    assert c.__doc__ == doc
+
+    d = NoConfigDocDir()
+    doc = "Dir to test auto docstring based on config."
+    assert d.__doc__ == doc
```

### Comparing `datamate-0.1.4/tests/test_namespaces.py` & `datamate-0.1.5/tests/test_namespaces.py`

 * *Files identical despite different names*

