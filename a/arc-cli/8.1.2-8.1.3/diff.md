# Comparing `tmp/arc_cli-8.1.2.tar.gz` & `tmp/arc_cli-8.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arc_cli-8.1.2.tar", max compression
+gzip compressed data, was "arc_cli-8.1.3.tar", max compression
```

## Comparing `arc_cli-8.1.2.tar` & `arc_cli-8.1.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      944 2023-04-24 02:20:30.375199 arc_cli-8.1.2/README.md
--rw-r--r--   0        0        0      719 2023-04-30 19:26:36.120254 arc_cli-8.1.2/arc/__init__.py
--rw-r--r--   0        0        0     1449 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/api.py
--rw-r--r--   0        0        0     6902 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/autocompletions.py
--rw-r--r--   0        0        0     2189 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/autoload.py
--rw-r--r--   0        0        0      114 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/color.py
--rw-r--r--   0        0        0     5732 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/config.py
--rw-r--r--   0        0        0      385 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/constants.py
--rw-r--r--   0        0        0      121 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/define/__init__.py
--rw-r--r--   0        0        0     1379 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/define/alias.py
--rw-r--r--   0        0        0     1768 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/define/classful.py
--rw-r--r--   0        0        0    17181 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/define/command.py
--rw-r--r--   0        0        0     3118 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/define/documentation.py
--rw-r--r--   0        0        0      219 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/define/param/__init__.py
--rw-r--r--   0        0        0     8036 2023-04-24 02:18:25.036233 arc_cli-8.1.2/arc/define/param/constructors.py
--rw-r--r--   0        0        0     3499 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/define/param/groups.py
--rw-r--r--   0        0        0     8706 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/define/param/param.py
--rw-r--r--   0        0        0     8549 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/define/param/param_definition.py
--rw-r--r--   0        0        0     3388 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/define/param/param_mixin.py
--rw-r--r--   0        0        0     1889 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/define/param/param_tree.py
--rw-r--r--   0        0        0     6314 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/errors.py
--rw-r--r--   0        0        0     1070 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/logging.py
--rw-r--r--   0        0        0    16336 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/parser.py
--rw-r--r--   0        0        0      402 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/__init__.py
--rw-r--r--   0        0        0     6168 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/ansi.py
--rw-r--r--   0        0        0     4681 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/box.py
--rw-r--r--   0        0        0     5101 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/console.py
--rw-r--r--   0        0        0      187 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/data.py
--rw-r--r--   0        0        0     2126 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/drawing.py
--rw-r--r--   0        0        0     2748 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/formatters.py
--rw-r--r--   0        0        0     9078 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/help_formatter.py
--rw-r--r--   0        0        0     3024 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/joiner.py
--rw-r--r--   0        0        0       54 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/markdown/__init__.py
--rw-r--r--   0        0        0     6473 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/markdown/markdown_parser.py
--rw-r--r--   0        0        0     3754 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/markdown/nodes.py
--rw-r--r--   0        0        0     1632 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/out.py
--rw-r--r--   0        0        0      987 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/pager.py
--rw-r--r--   0        0        0     9825 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/table.py
--rw-r--r--   0        0        0     5182 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/present/wrap.py
--rw-r--r--   0        0        0      288 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/prompt/__init__.py
--rw-r--r--   0        0        0     3686 2023-04-30 19:15:57.867568 arc_cli-8.1.2/arc/prompt/helpers.py
--rw-r--r--   0        0        0     5926 2023-04-24 02:18:25.039567 arc_cli-8.1.2/arc/prompt/prompt.py
--rw-r--r--   0        0        0      812 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/prompt/prompts.py
--rw-r--r--   0        0        0     7019 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/prompt/questions.py
--rw-r--r--   0        0        0        0 2023-03-18 01:38:52.879777 arc_cli-8.1.2/arc/py.typed
--rw-r--r--   0        0        0      306 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/runtime/__init__.py
--rw-r--r--   0        0        0     2970 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/runtime/app.py
--rw-r--r--   0        0        0     2678 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/runtime/context.py
--rw-r--r--   0        0        0    12517 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/runtime/exec.py
--rw-r--r--   0        0        0     8240 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/runtime/init.py
--rw-r--r--   0        0        0     7402 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/runtime/middleware.py
--rw-r--r--   0        0        0      382 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/safe.py
--rw-r--r--   0        0        0     1866 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/suggest.py
--rw-r--r--   0        0        0      335 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/__init__.py
--rw-r--r--   0        0        0    13898 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/aliases.py
--rw-r--r--   0        0        0      670 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/convert.py
--rw-r--r--   0        0        0      545 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/default.py
--rw-r--r--   0        0        0     4422 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/file.py
--rw-r--r--   0        0        0       79 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/middleware/__init__.py
--rw-r--r--   0        0        0     1403 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/middleware/observers.py
--rw-r--r--   0        0        0     2630 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/middleware/transformers.py
--rw-r--r--   0        0        0     4042 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/middleware/validators.py
--rw-r--r--   0        0        0     3486 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/network.py
--rw-r--r--   0        0        0      854 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/numbers.py
--rw-r--r--   0        0        0      860 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/path.py
--rw-r--r--   0        0        0     6881 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/semver.py
--rw-r--r--   0        0        0      877 2023-04-24 02:18:25.042900 arc_cli-8.1.2/arc/types/state.py
--rw-r--r--   0        0        0     1921 2023-04-24 02:18:25.046233 arc_cli-8.1.2/arc/types/strings.py
--rw-r--r--   0        0        0     2155 2023-04-24 02:18:25.046233 arc_cli-8.1.2/arc/types/type_arg.py
--rw-r--r--   0        0        0     2718 2023-04-24 02:18:25.046233 arc_cli-8.1.2/arc/types/type_info.py
--rw-r--r--   0        0        0     3176 2023-04-24 02:18:25.046233 arc_cli-8.1.2/arc/types/users.py
--rw-r--r--   0        0        0     2257 2023-04-24 02:18:25.046233 arc_cli-8.1.2/arc/typing.py
--rw-r--r--   0        0        0     1043 2023-04-30 19:26:36.570252 arc_cli-8.1.2/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 arc_cli-8.1.2/setup.py
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 arc_cli-8.1.2/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-04-24 02:20:30.375199 arc_cli-8.1.3/README.md
+-rw-r--r--   0        0        0      719 2023-04-30 19:31:59.521654 arc_cli-8.1.3/arc/__init__.py
+-rw-r--r--   0        0        0     1449 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/api.py
+-rw-r--r--   0        0        0     6902 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/autocompletions.py
+-rw-r--r--   0        0        0     2189 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/autoload.py
+-rw-r--r--   0        0        0      114 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/color.py
+-rw-r--r--   0        0        0     5732 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/config.py
+-rw-r--r--   0        0        0      385 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/constants.py
+-rw-r--r--   0        0        0      121 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/define/__init__.py
+-rw-r--r--   0        0        0     1379 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/define/alias.py
+-rw-r--r--   0        0        0     1768 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/define/classful.py
+-rw-r--r--   0        0        0    17181 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/define/command.py
+-rw-r--r--   0        0        0     3118 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/define/documentation.py
+-rw-r--r--   0        0        0      219 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/define/param/__init__.py
+-rw-r--r--   0        0        0     8036 2023-04-24 02:18:25.036233 arc_cli-8.1.3/arc/define/param/constructors.py
+-rw-r--r--   0        0        0     3499 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/define/param/groups.py
+-rw-r--r--   0        0        0     8706 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/define/param/param.py
+-rw-r--r--   0        0        0     8549 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/define/param/param_definition.py
+-rw-r--r--   0        0        0     3388 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/define/param/param_mixin.py
+-rw-r--r--   0        0        0     1889 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/define/param/param_tree.py
+-rw-r--r--   0        0        0     6314 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/errors.py
+-rw-r--r--   0        0        0     1070 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/logging.py
+-rw-r--r--   0        0        0    16336 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/parser.py
+-rw-r--r--   0        0        0      402 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/__init__.py
+-rw-r--r--   0        0        0     6168 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/ansi.py
+-rw-r--r--   0        0        0     4681 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/box.py
+-rw-r--r--   0        0        0     5101 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/console.py
+-rw-r--r--   0        0        0      187 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/data.py
+-rw-r--r--   0        0        0     2126 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/drawing.py
+-rw-r--r--   0        0        0     2748 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/formatters.py
+-rw-r--r--   0        0        0     9078 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/help_formatter.py
+-rw-r--r--   0        0        0     3024 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/joiner.py
+-rw-r--r--   0        0        0       54 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/markdown/__init__.py
+-rw-r--r--   0        0        0     6473 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/markdown/markdown_parser.py
+-rw-r--r--   0        0        0     3754 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/markdown/nodes.py
+-rw-r--r--   0        0        0     1632 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/out.py
+-rw-r--r--   0        0        0      987 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/pager.py
+-rw-r--r--   0        0        0     9825 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/table.py
+-rw-r--r--   0        0        0     5182 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/present/wrap.py
+-rw-r--r--   0        0        0      288 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/prompt/__init__.py
+-rw-r--r--   0        0        0     3722 2023-04-30 19:31:15.828580 arc_cli-8.1.3/arc/prompt/helpers.py
+-rw-r--r--   0        0        0     5926 2023-04-24 02:18:25.039567 arc_cli-8.1.3/arc/prompt/prompt.py
+-rw-r--r--   0        0        0      812 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/prompt/prompts.py
+-rw-r--r--   0        0        0     7019 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/prompt/questions.py
+-rw-r--r--   0        0        0        0 2023-03-18 01:38:52.879777 arc_cli-8.1.3/arc/py.typed
+-rw-r--r--   0        0        0      306 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/runtime/__init__.py
+-rw-r--r--   0        0        0     2970 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/runtime/app.py
+-rw-r--r--   0        0        0     2678 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/runtime/context.py
+-rw-r--r--   0        0        0    12517 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/runtime/exec.py
+-rw-r--r--   0        0        0     8240 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/runtime/init.py
+-rw-r--r--   0        0        0     7402 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/runtime/middleware.py
+-rw-r--r--   0        0        0      382 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/safe.py
+-rw-r--r--   0        0        0     1866 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/suggest.py
+-rw-r--r--   0        0        0      335 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/__init__.py
+-rw-r--r--   0        0        0    13898 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/aliases.py
+-rw-r--r--   0        0        0      670 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/convert.py
+-rw-r--r--   0        0        0      545 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/default.py
+-rw-r--r--   0        0        0     4422 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/file.py
+-rw-r--r--   0        0        0       79 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/middleware/__init__.py
+-rw-r--r--   0        0        0     1403 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/middleware/observers.py
+-rw-r--r--   0        0        0     2630 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/middleware/transformers.py
+-rw-r--r--   0        0        0     4042 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/middleware/validators.py
+-rw-r--r--   0        0        0     3486 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/network.py
+-rw-r--r--   0        0        0      854 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/numbers.py
+-rw-r--r--   0        0        0      860 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/path.py
+-rw-r--r--   0        0        0     6881 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/semver.py
+-rw-r--r--   0        0        0      877 2023-04-24 02:18:25.042900 arc_cli-8.1.3/arc/types/state.py
+-rw-r--r--   0        0        0     1921 2023-04-24 02:18:25.046233 arc_cli-8.1.3/arc/types/strings.py
+-rw-r--r--   0        0        0     2155 2023-04-24 02:18:25.046233 arc_cli-8.1.3/arc/types/type_arg.py
+-rw-r--r--   0        0        0     2718 2023-04-24 02:18:25.046233 arc_cli-8.1.3/arc/types/type_info.py
+-rw-r--r--   0        0        0     3176 2023-04-24 02:18:25.046233 arc_cli-8.1.3/arc/types/users.py
+-rw-r--r--   0        0        0     2257 2023-04-24 02:18:25.046233 arc_cli-8.1.3/arc/typing.py
+-rw-r--r--   0        0        0     1043 2023-04-30 19:32:00.194983 arc_cli-8.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 arc_cli-8.1.3/setup.py
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 arc_cli-8.1.3/PKG-INFO
```

### Comparing `arc_cli-8.1.2/README.md` & `arc_cli-8.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/__init__.py` & `arc_cli-8.1.3/arc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "8.1.2"
+__version__ = "8.1.3"
 
 from arc import types, prompt, present, errors
 from arc.config import (
     ColorConfig,
     Config,
     LinksConfig,
     SuggestionConfig,
```

### Comparing `arc_cli-8.1.2/arc/api.py` & `arc_cli-8.1.3/arc/api.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/autocompletions.py` & `arc_cli-8.1.3/arc/autocompletions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/autoload.py` & `arc_cli-8.1.3/arc/autoload.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/config.py` & `arc_cli-8.1.3/arc/config.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/alias.py` & `arc_cli-8.1.3/arc/define/alias.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/classful.py` & `arc_cli-8.1.3/arc/define/classful.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/command.py` & `arc_cli-8.1.3/arc/define/command.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/documentation.py` & `arc_cli-8.1.3/arc/define/documentation.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/param/constructors.py` & `arc_cli-8.1.3/arc/define/param/constructors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/param/groups.py` & `arc_cli-8.1.3/arc/define/param/groups.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/param/param.py` & `arc_cli-8.1.3/arc/define/param/param.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/param/param_definition.py` & `arc_cli-8.1.3/arc/define/param/param_definition.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/param/param_mixin.py` & `arc_cli-8.1.3/arc/define/param/param_mixin.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/define/param/param_tree.py` & `arc_cli-8.1.3/arc/define/param/param_tree.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/errors.py` & `arc_cli-8.1.3/arc/errors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/logging.py` & `arc_cli-8.1.3/arc/logging.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/parser.py` & `arc_cli-8.1.3/arc/parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/ansi.py` & `arc_cli-8.1.3/arc/present/ansi.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/box.py` & `arc_cli-8.1.3/arc/present/box.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/console.py` & `arc_cli-8.1.3/arc/present/console.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/drawing.py` & `arc_cli-8.1.3/arc/present/drawing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/formatters.py` & `arc_cli-8.1.3/arc/present/formatters.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/help_formatter.py` & `arc_cli-8.1.3/arc/present/help_formatter.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/joiner.py` & `arc_cli-8.1.3/arc/present/joiner.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/markdown/markdown_parser.py` & `arc_cli-8.1.3/arc/present/markdown/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/markdown/nodes.py` & `arc_cli-8.1.3/arc/present/markdown/nodes.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/out.py` & `arc_cli-8.1.3/arc/present/out.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/pager.py` & `arc_cli-8.1.3/arc/present/pager.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/table.py` & `arc_cli-8.1.3/arc/present/table.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/present/wrap.py` & `arc_cli-8.1.3/arc/present/wrap.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/prompt/helpers.py` & `arc_cli-8.1.3/arc/prompt/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 import re
 import sys
-import tty
 import typing as t
 from contextlib import contextmanager
 
 T = t.TypeVar("T")
 
 
 def clear_line(amount: t.Literal["all", "before", "after"] = "all") -> str:
@@ -22,21 +21,23 @@
 class RawTerminal:
     __raw: bool = False
     __old_settings: list[t.Any]
 
     def __init__(self) -> None:
         # Moved into here to support pyodide
         import termios
+        import tty
 
         self.termios = termios
+        self.tty = tty
 
     def __enter__(self) -> RawTerminal:
         fd = sys.stdin.fileno()
         self.__old_settings = self.termios.tcgetattr(fd)
-        tty.setraw(sys.stdin.fileno())
+        self.tty.setraw(sys.stdin.fileno())
         self.__raw = True
         return self
 
     def __exit__(self, *args: t.Any) -> None:
         fd = sys.stdin.fileno()
         self.__raw = False
         self.termios.tcsetattr(fd, self.termios.TCSADRAIN, self.__old_settings)
```

### Comparing `arc_cli-8.1.2/arc/prompt/prompt.py` & `arc_cli-8.1.3/arc/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/prompt/prompts.py` & `arc_cli-8.1.3/arc/prompt/prompts.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/prompt/questions.py` & `arc_cli-8.1.3/arc/prompt/questions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/runtime/app.py` & `arc_cli-8.1.3/arc/runtime/app.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/runtime/context.py` & `arc_cli-8.1.3/arc/runtime/context.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/runtime/exec.py` & `arc_cli-8.1.3/arc/runtime/exec.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/runtime/init.py` & `arc_cli-8.1.3/arc/runtime/init.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/runtime/middleware.py` & `arc_cli-8.1.3/arc/runtime/middleware.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/suggest.py` & `arc_cli-8.1.3/arc/suggest.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/aliases.py` & `arc_cli-8.1.3/arc/types/aliases.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/convert.py` & `arc_cli-8.1.3/arc/types/convert.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/default.py` & `arc_cli-8.1.3/arc/types/default.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/file.py` & `arc_cli-8.1.3/arc/types/file.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/middleware/observers.py` & `arc_cli-8.1.3/arc/types/middleware/observers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/middleware/transformers.py` & `arc_cli-8.1.3/arc/types/middleware/transformers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/middleware/validators.py` & `arc_cli-8.1.3/arc/types/middleware/validators.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/network.py` & `arc_cli-8.1.3/arc/types/network.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/numbers.py` & `arc_cli-8.1.3/arc/types/numbers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/path.py` & `arc_cli-8.1.3/arc/types/path.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/semver.py` & `arc_cli-8.1.3/arc/types/semver.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/state.py` & `arc_cli-8.1.3/arc/types/state.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/strings.py` & `arc_cli-8.1.3/arc/types/strings.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/type_arg.py` & `arc_cli-8.1.3/arc/types/type_arg.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/type_info.py` & `arc_cli-8.1.3/arc/types/type_info.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/types/users.py` & `arc_cli-8.1.3/arc/types/users.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/arc/typing.py` & `arc_cli-8.1.3/arc/typing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.2/pyproject.toml` & `arc_cli-8.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arc-cli"
-version = "8.1.2"
+version = "8.1.3"
 description = "A Regular CLI"
 authors = ["Sean Collings <seanrcollings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/arc"
 documentation = "https://arc.seanrcollings.com"
 keywords = ["CLI", "extendable", "easy", "arc"]
```

### Comparing `arc_cli-8.1.2/setup.py` & `arc_cli-8.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['cli = cli:command']}
 
 setup_kwargs = {
     'name': 'arc-cli',
-    'version': '8.1.2',
+    'version': '8.1.3',
     'description': 'A Regular CLI',
     'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# [Docs](http://arc.seanrcollings.com)\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
     'author': 'Sean Collings',
     'author_email': 'seanrcollings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/arc',
```

### Comparing `arc_cli-8.1.2/PKG-INFO` & `arc_cli-8.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arc-cli
-Version: 8.1.2
+Version: 8.1.3
 Summary: A Regular CLI
 Home-page: https://github.com/seanrcollings/arc
 License: MIT
 Keywords: CLI,extendable,easy,arc
 Author: Sean Collings
 Author-email: seanrcollings@gmail.com
 Requires-Python: >=3.10,<4.0
```

