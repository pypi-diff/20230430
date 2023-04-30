# Comparing `tmp/hhoppe-tools-1.2.9.tar.gz` & `tmp/hhoppe-tools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhoppe-tools-1.2.9.tar", last modified: Sun Apr 16 23:57:55 2023, max compression
+gzip compressed data, was "hhoppe-tools-1.3.0.tar", last modified: Sun Apr 30 04:11:56 2023, max compression
```

## Comparing `hhoppe-tools-1.2.9.tar` & `hhoppe-tools-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/LICENSE
--rw-r--r--   0        0        0      147 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/README.md
--rw-r--r--   0        0        0    75696 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/hhoppe_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/hhoppe_tools/py.typed
--rw-r--r--   0        0        0     2569 2023-04-16 23:57:47.691275 hhoppe-tools-1.2.9/pyproject.toml
--rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 hhoppe-tools-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-30 04:11:48.934039 hhoppe-tools-1.3.0/LICENSE
+-rw-r--r--   0        0        0      147 2023-04-30 04:11:48.934039 hhoppe-tools-1.3.0/README.md
+-rw-r--r--   0        0        0    75774 2023-04-30 04:11:48.934039 hhoppe-tools-1.3.0/hhoppe_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 04:11:48.934039 hhoppe-tools-1.3.0/hhoppe_tools/py.typed
+-rw-r--r--   0        0        0     2545 2023-04-30 04:11:48.934039 hhoppe-tools-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 hhoppe-tools-1.3.0/PKG-INFO
```

### Comparing `hhoppe-tools-1.2.9/LICENSE` & `hhoppe-tools-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hhoppe-tools-1.2.9/hhoppe_tools/__init__.py` & `hhoppe-tools-1.3.0/hhoppe_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 env python3 -m doctest -v __init__.py | perl -ne 'print if /had no tests/../passed all/' | tail -n +2 | head -n -1
 ```
 """
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.2.9'
+__version__ = '1.3.0'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 import ast
 import collections.abc
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 import contextlib
 import cProfile
@@ -205,37 +205,37 @@
   '[3, 4, 5][1] = 4'
   """
 
   def matching_parenthesis(text: str) -> int:
     """Return the index of ')' matching '(' in text[0]."""
     check_eq(text[0], '(')
     num_open = 0
-    for i, c in enumerate(text):
-      if c == '(':
+    for i, ch in enumerate(text):
+      if ch == '(':
         num_open += 1
-      elif c == ')':
+      elif ch == ')':
         num_open -= 1
         if num_open == 0:
           return i
-    raise RuntimeError(f'No matching right parenthesis in "{text}"')
+    raise RuntimeError(f'No matching right parenthesis in "{text}".')
 
   # Adapted from make_dict() in https://stackoverflow.com/a/2553524 .
   stack = traceback.extract_stack()
   this_function_name = stack[-1][2]  # i.e. initially '_dump_vars'.
   for stackframe in stack[-2::-1]:
     filename, unused_line_number, function_name, text = stackframe  # Caller.
     # https://docs.python.org/3/tutorial/errors.html:
     # "however, it will not display lines read from standard input."
     if filename == '<stdin>':
       check_eq(text, '')
       return ', '.join(str(e) for e in args)  # Unfortunate fallback.
     prefix = this_function_name + '('
     begin = text.find(prefix)
     if begin < 0:
-      raise AssertionError(f'_dump_vars: cannot find "{prefix}" in line "{text}"')
+      raise RuntimeError(f'_dump_vars: cannot find "{prefix}" in line "{text}".')
     begin += len(this_function_name)
     end = begin + matching_parenthesis(text[begin:])
     parameter_string = text[begin + 1 : end].strip()
     if re.fullmatch(r'\*[\w]+', parameter_string):
       this_function_name = function_name
       # Because the call is made using a *args, we continue to
       # the earlier caller in the stack trace.
@@ -253,14 +253,15 @@
           return '?' if text is None else text
 
         expressions = [get_text(element) for element in elements]
       l = []
       for expr, value in zip(expressions, args):
         l.append(f'{expr} = {value}' if expr[0] not in '"\'' else str(value))
       return ', '.join(l)
+
   raise AssertionError
 
 
 def show(*args: Any) -> None:
   r"""Prints expressions and their values on stdout.
 
   Args:
@@ -482,26 +483,28 @@
           {% block content %}{% endblock %}
           {% filter minify_css %}
                   <style>{% include "syntax-highlighting.css" %}</style>
                   <style>{% include "theme.css" %}</style>
                   <style>{% include "content.css" %}</style>
           {% endfilter %}
       </div>
-      """
+      """,
+        encoding='utf-8',
     )
     (template_dir / 'module.html.jinja2').write_text(
         """\
       {% extends "default/module.html.jinja2" %}
       {% macro is_public(doc) %}
           {% if should_show(doc.qualname) %}
               {{ default_is_public(doc) }}
           {% endif %}
       {% endmacro %}
       {% block module_info %}{% endblock %}
-      """
+      """,
+        encoding='utf-8',
     )
     module = inspect.getmodule(thing)
     if module is None:
       raise ValueError(f'Cannot identify module for {thing=}.')
     doc = pdoc.doc.Module(module)
     pdoc.render.configure(
         docformat=docformat, math=True, show_source=True, template_directory=template_dir
@@ -1017,19 +1020,19 @@
     ValueError if `pattern` is not found in `string`.
 
   >>> re_groups(r'object (\d+).*loc (\w+)', 'The object 13 at loc ABC.')
   ('13', 'ABC')
   >>> re_groups(r'(\d+)', 'Some text.')
   Traceback (most recent call last):
   ...
-  ValueError: Did not locate pattern "(\d+)" in "Some text."
+  ValueError: Did not locate pattern "(\d+)" in "Some text.".
   """
   match = re.search(pattern, string)
   if not match:
-    raise ValueError(f'Did not locate pattern "{pattern}" in "{string}"')
+    raise ValueError(f'Did not locate pattern "{pattern}" in "{string}".')
   return match.groups()
 
 
 # ** Mathematics
 
 
 def as_float(a: _ArrayLike, /) -> _NDArray:
@@ -2392,15 +2395,15 @@
 
 def is_executable(path: _Path, /) -> bool:
   """Return True if the file `path` is executable.
 
   >>> import tempfile
   >>> with tempfile.TemporaryDirectory() as dir:
   ...   path = pathlib.Path(dir) / 'file'
-  ...   _ = path.write_text('test')
+  ...   _ = path.write_text('test', encoding='utf-8')
   ...   check_eq(is_executable(path), False)
   ...   if sys.platform != 'cygwin':
   ...     # Copy R bits to X bits:
   ...     path.chmod(path.stat().st_mode | ((path.stat().st_mode & 0o444) >> 2))
   ...     check_eq(is_executable(path), True)
   """
   return bool(pathlib.Path(path).stat().st_mode & stat.S_IEXEC)
```

### Comparing `hhoppe-tools-1.2.9/pyproject.toml` & `hhoppe-tools-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 pyink-use-majority-quotes = true
 # quiet = true
 # verbose = true
 extend-exclude = "^/Other/|/old_setup\\.py/"
 
 [tool.pylint.main]
 disable = [
-    "unspecified-encoding", "fixme", "redefined-builtin", "cell-var-from-loop",
+    "fixme", "redefined-builtin", "cell-var-from-loop",
     "using-constant-test", "simplifiable-condition", "import-outside-toplevel", "line-too-long",
     "too-many-lines", "too-few-public-methods", "too-many-arguments", "too-many-locals", "use-dict-literal",
 ]
 reports = false
 score = false
 recursive = true
 ignore-paths = [".ipynb_checkpoints"]
```

### Comparing `hhoppe-tools-1.2.9/PKG-INFO` & `hhoppe-tools-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhoppe-tools
-Version: 1.2.9
+Version: 1.3.0
 Summary: Library of Python tools by Hugues Hoppe
 Keywords: 
 Author-email: Hugues Hoppe <hhoppe@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

