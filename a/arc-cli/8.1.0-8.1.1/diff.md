# Comparing `tmp/arc_cli-8.1.0.tar.gz` & `tmp/arc_cli-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arc_cli-8.1.0.tar", max compression
+gzip compressed data, was "arc_cli-8.1.1.tar", max compression
```

## Comparing `arc_cli-8.1.0.tar` & `arc_cli-8.1.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      948 2023-04-03 06:10:36.617549 arc_cli-8.1.0/README.md
--rw-r--r--   0        0        0      719 2023-04-24 02:17:23.823406 arc_cli-8.1.0/arc/__init__.py
--rw-r--r--   0        0        0     1449 2023-04-02 19:49:22.490290 arc_cli-8.1.0/arc/api.py
--rw-r--r--   0        0        0     6902 2023-04-02 19:50:04.610035 arc_cli-8.1.0/arc/autocompletions.py
--rw-r--r--   0        0        0     2189 2023-04-24 02:12:55.892295 arc_cli-8.1.0/arc/autoload.py
--rw-r--r--   0        0        0      114 2023-03-18 01:38:52.866444 arc_cli-8.1.0/arc/color.py
--rw-r--r--   0        0        0     5732 2023-04-02 19:50:49.346437 arc_cli-8.1.0/arc/config.py
--rw-r--r--   0        0        0      385 2023-04-02 19:50:56.469728 arc_cli-8.1.0/arc/constants.py
--rw-r--r--   0        0        0      121 2023-03-18 01:38:52.869777 arc_cli-8.1.0/arc/define/__init__.py
--rw-r--r--   0        0        0     1379 2023-04-02 17:43:44.931222 arc_cli-8.1.0/arc/define/alias.py
--rw-r--r--   0        0        0     1768 2023-04-02 18:33:44.151939 arc_cli-8.1.0/arc/define/classful.py
--rw-r--r--   0        0        0    17181 2023-04-05 15:50:39.351207 arc_cli-8.1.0/arc/define/command.py
--rw-r--r--   0        0        0     3118 2023-04-02 18:42:11.444896 arc_cli-8.1.0/arc/define/documentation.py
--rw-r--r--   0        0        0      219 2023-03-18 01:38:52.869777 arc_cli-8.1.0/arc/define/param/__init__.py
--rw-r--r--   0        0        0     8036 2023-04-02 17:56:17.764120 arc_cli-8.1.0/arc/define/param/constructors.py
--rw-r--r--   0        0        0     3499 2023-04-02 20:00:29.589991 arc_cli-8.1.0/arc/define/param/groups.py
--rw-r--r--   0        0        0     8706 2023-04-02 18:33:06.022072 arc_cli-8.1.0/arc/define/param/param.py
--rw-r--r--   0        0        0     8549 2023-04-02 19:59:52.323512 arc_cli-8.1.0/arc/define/param/param_definition.py
--rw-r--r--   0        0        0     3388 2023-04-02 18:24:36.069969 arc_cli-8.1.0/arc/define/param/param_mixin.py
--rw-r--r--   0        0        0     1889 2023-04-02 18:14:05.651853 arc_cli-8.1.0/arc/define/param/param_tree.py
--rw-r--r--   0        0        0     6314 2023-04-02 19:59:32.173614 arc_cli-8.1.0/arc/errors.py
--rw-r--r--   0        0        0     1070 2023-04-02 19:53:55.292050 arc_cli-8.1.0/arc/logging.py
--rw-r--r--   0        0        0    16336 2023-04-03 06:34:53.306993 arc_cli-8.1.0/arc/parser.py
--rw-r--r--   0        0        0      402 2023-04-02 18:55:17.768463 arc_cli-8.1.0/arc/present/__init__.py
--rw-r--r--   0        0        0     6168 2023-04-02 18:49:02.832312 arc_cli-8.1.0/arc/present/ansi.py
--rw-r--r--   0        0        0     4681 2023-04-02 18:50:13.529156 arc_cli-8.1.0/arc/present/box.py
--rw-r--r--   0        0        0     5101 2023-04-02 01:35:30.112194 arc_cli-8.1.0/arc/present/console.py
--rw-r--r--   0        0        0      187 2023-03-18 01:38:52.873111 arc_cli-8.1.0/arc/present/data.py
--rw-r--r--   0        0        0     2126 2023-03-18 01:38:52.873111 arc_cli-8.1.0/arc/present/drawing.py
--rw-r--r--   0        0        0     2748 2023-04-02 18:50:56.742602 arc_cli-8.1.0/arc/present/formatters.py
--rw-r--r--   0        0        0     9078 2023-04-05 14:25:08.363048 arc_cli-8.1.0/arc/present/help_formatter.py
--rw-r--r--   0        0        0     3024 2023-04-02 18:54:21.520831 arc_cli-8.1.0/arc/present/joiner.py
--rw-r--r--   0        0        0       54 2023-04-02 01:35:30.112194 arc_cli-8.1.0/arc/present/markdown/__init__.py
--rw-r--r--   0        0        0     6473 2023-04-02 01:35:30.112194 arc_cli-8.1.0/arc/present/markdown/markdown_parser.py
--rw-r--r--   0        0        0     3754 2023-04-02 18:42:43.214931 arc_cli-8.1.0/arc/present/markdown/nodes.py
--rw-r--r--   0        0        0     1632 2023-04-02 01:35:30.115527 arc_cli-8.1.0/arc/present/out.py
--rw-r--r--   0        0        0      987 2023-04-02 18:55:42.314170 arc_cli-8.1.0/arc/present/pager.py
--rw-r--r--   0        0        0     9825 2023-04-02 18:58:32.921906 arc_cli-8.1.0/arc/present/table.py
--rw-r--r--   0        0        0     5182 2023-04-02 18:58:53.471341 arc_cli-8.1.0/arc/present/wrap.py
--rw-r--r--   0        0        0      288 2023-03-18 01:38:52.876444 arc_cli-8.1.0/arc/prompt/__init__.py
--rw-r--r--   0        0        0     3553 2023-04-02 19:01:30.097653 arc_cli-8.1.0/arc/prompt/helpers.py
--rw-r--r--   0        0        0     5926 2023-04-02 19:10:04.010602 arc_cli-8.1.0/arc/prompt/prompt.py
--rw-r--r--   0        0        0      812 2023-04-02 19:06:08.453122 arc_cli-8.1.0/arc/prompt/prompts.py
--rw-r--r--   0        0        0     7019 2023-04-02 19:05:25.083697 arc_cli-8.1.0/arc/prompt/questions.py
--rw-r--r--   0        0        0        0 2023-03-18 01:38:52.879777 arc_cli-8.1.0/arc/py.typed
--rw-r--r--   0        0        0      306 2023-03-18 01:38:52.879777 arc_cli-8.1.0/arc/runtime/__init__.py
--rw-r--r--   0        0        0     2970 2023-04-02 19:11:35.999835 arc_cli-8.1.0/arc/runtime/app.py
--rw-r--r--   0        0        0     2678 2023-04-02 19:12:32.056081 arc_cli-8.1.0/arc/runtime/context.py
--rw-r--r--   0        0        0    12517 2023-04-05 16:07:36.763616 arc_cli-8.1.0/arc/runtime/exec.py
--rw-r--r--   0        0        0     8240 2023-04-03 06:32:50.920598 arc_cli-8.1.0/arc/runtime/init.py
--rw-r--r--   0        0        0     7402 2023-04-10 14:24:59.927180 arc_cli-8.1.0/arc/runtime/middleware.py
--rw-r--r--   0        0        0      382 2023-04-02 19:57:53.277453 arc_cli-8.1.0/arc/safe.py
--rw-r--r--   0        0        0     1866 2023-04-02 19:58:09.647368 arc_cli-8.1.0/arc/suggest.py
--rw-r--r--   0        0        0      335 2023-03-18 01:38:52.883111 arc_cli-8.1.0/arc/types/__init__.py
--rw-r--r--   0        0        0    13898 2023-04-02 20:01:19.976406 arc_cli-8.1.0/arc/types/aliases.py
--rw-r--r--   0        0        0      670 2023-04-02 19:44:25.002266 arc_cli-8.1.0/arc/types/convert.py
--rw-r--r--   0        0        0      545 2023-04-02 19:36:55.892931 arc_cli-8.1.0/arc/types/default.py
--rw-r--r--   0        0        0     4422 2023-04-02 19:37:41.742437 arc_cli-8.1.0/arc/types/file.py
--rw-r--r--   0        0        0       79 2023-03-18 01:38:52.883111 arc_cli-8.1.0/arc/types/middleware/__init__.py
--rw-r--r--   0        0        0     1403 2023-04-02 19:23:23.836123 arc_cli-8.1.0/arc/types/middleware/observers.py
--rw-r--r--   0        0        0     2630 2023-04-02 19:24:57.642461 arc_cli-8.1.0/arc/types/middleware/transformers.py
--rw-r--r--   0        0        0     4042 2023-04-02 19:25:31.049016 arc_cli-8.1.0/arc/types/middleware/validators.py
--rw-r--r--   0        0        0     3486 2023-04-02 19:38:15.415422 arc_cli-8.1.0/arc/types/network.py
--rw-r--r--   0        0        0      854 2023-03-18 01:38:52.883111 arc_cli-8.1.0/arc/types/numbers.py
--rw-r--r--   0        0        0      860 2023-04-02 19:38:33.971903 arc_cli-8.1.0/arc/types/path.py
--rw-r--r--   0        0        0     6881 2023-04-02 19:41:26.780325 arc_cli-8.1.0/arc/types/semver.py
--rw-r--r--   0        0        0      877 2023-04-02 19:42:04.026684 arc_cli-8.1.0/arc/types/state.py
--rw-r--r--   0        0        0     1921 2023-04-02 19:42:33.143116 arc_cli-8.1.0/arc/types/strings.py
--rw-r--r--   0        0        0     2155 2023-04-02 20:00:43.369922 arc_cli-8.1.0/arc/types/type_arg.py
--rw-r--r--   0        0        0     2718 2023-04-02 20:01:36.192993 arc_cli-8.1.0/arc/types/type_info.py
--rw-r--r--   0        0        0     3176 2023-04-02 19:47:49.397539 arc_cli-8.1.0/arc/types/users.py
--rw-r--r--   0        0        0     2257 2023-04-02 19:36:17.910027 arc_cli-8.1.0/arc/typing.py
--rw-r--r--   0        0        0     1043 2023-04-24 02:17:24.306735 arc_cli-8.1.0/pyproject.toml
--rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 arc_cli-8.1.0/setup.py
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 arc_cli-8.1.0/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-04-24 02:20:30.375199 arc_cli-8.1.1/README.md
+-rw-r--r--   0        0        0      719 2023-04-30 19:17:22.940349 arc_cli-8.1.1/arc/__init__.py
+-rw-r--r--   0        0        0     1449 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/api.py
+-rw-r--r--   0        0        0     6902 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/autocompletions.py
+-rw-r--r--   0        0        0     2189 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/autoload.py
+-rw-r--r--   0        0        0      114 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/color.py
+-rw-r--r--   0        0        0     5732 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/config.py
+-rw-r--r--   0        0        0      385 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/constants.py
+-rw-r--r--   0        0        0      121 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/define/__init__.py
+-rw-r--r--   0        0        0     1379 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/define/alias.py
+-rw-r--r--   0        0        0     1768 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/define/classful.py
+-rw-r--r--   0        0        0    17181 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/define/command.py
+-rw-r--r--   0        0        0     3118 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/define/documentation.py
+-rw-r--r--   0        0        0      219 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/define/param/__init__.py
+-rw-r--r--   0        0        0     8036 2023-04-24 02:18:25.036233 arc_cli-8.1.1/arc/define/param/constructors.py
+-rw-r--r--   0        0        0     3499 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/define/param/groups.py
+-rw-r--r--   0        0        0     8706 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/define/param/param.py
+-rw-r--r--   0        0        0     8549 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/define/param/param_definition.py
+-rw-r--r--   0        0        0     3388 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/define/param/param_mixin.py
+-rw-r--r--   0        0        0     1889 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/define/param/param_tree.py
+-rw-r--r--   0        0        0     6314 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/errors.py
+-rw-r--r--   0        0        0     1070 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/logging.py
+-rw-r--r--   0        0        0    16336 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/parser.py
+-rw-r--r--   0        0        0      402 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/__init__.py
+-rw-r--r--   0        0        0     6168 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/ansi.py
+-rw-r--r--   0        0        0     4681 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/box.py
+-rw-r--r--   0        0        0     5101 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/console.py
+-rw-r--r--   0        0        0      187 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/data.py
+-rw-r--r--   0        0        0     2126 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/drawing.py
+-rw-r--r--   0        0        0     2748 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/formatters.py
+-rw-r--r--   0        0        0     9078 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/help_formatter.py
+-rw-r--r--   0        0        0     3024 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/joiner.py
+-rw-r--r--   0        0        0       54 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/markdown/__init__.py
+-rw-r--r--   0        0        0     6473 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/markdown/markdown_parser.py
+-rw-r--r--   0        0        0     3754 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/markdown/nodes.py
+-rw-r--r--   0        0        0     1632 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/out.py
+-rw-r--r--   0        0        0      987 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/pager.py
+-rw-r--r--   0        0        0     9825 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/table.py
+-rw-r--r--   0        0        0     5182 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/present/wrap.py
+-rw-r--r--   0        0        0      288 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/prompt/__init__.py
+-rw-r--r--   0        0        0     3686 2023-04-30 19:15:57.867568 arc_cli-8.1.1/arc/prompt/helpers.py
+-rw-r--r--   0        0        0     5926 2023-04-24 02:18:25.039567 arc_cli-8.1.1/arc/prompt/prompt.py
+-rw-r--r--   0        0        0      812 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/prompt/prompts.py
+-rw-r--r--   0        0        0     7019 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/prompt/questions.py
+-rw-r--r--   0        0        0        0 2023-03-18 01:38:52.879777 arc_cli-8.1.1/arc/py.typed
+-rw-r--r--   0        0        0      306 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/runtime/__init__.py
+-rw-r--r--   0        0        0     2970 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/runtime/app.py
+-rw-r--r--   0        0        0     2678 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/runtime/context.py
+-rw-r--r--   0        0        0    12517 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/runtime/exec.py
+-rw-r--r--   0        0        0     8240 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/runtime/init.py
+-rw-r--r--   0        0        0     7402 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/runtime/middleware.py
+-rw-r--r--   0        0        0      382 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/safe.py
+-rw-r--r--   0        0        0     1866 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/suggest.py
+-rw-r--r--   0        0        0      335 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/__init__.py
+-rw-r--r--   0        0        0    13898 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/aliases.py
+-rw-r--r--   0        0        0      670 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/convert.py
+-rw-r--r--   0        0        0      545 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/default.py
+-rw-r--r--   0        0        0     4422 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/file.py
+-rw-r--r--   0        0        0       79 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/middleware/__init__.py
+-rw-r--r--   0        0        0     1403 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/middleware/observers.py
+-rw-r--r--   0        0        0     2630 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/middleware/transformers.py
+-rw-r--r--   0        0        0     4042 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/middleware/validators.py
+-rw-r--r--   0        0        0     3486 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/network.py
+-rw-r--r--   0        0        0      854 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/numbers.py
+-rw-r--r--   0        0        0      860 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/path.py
+-rw-r--r--   0        0        0     6881 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/semver.py
+-rw-r--r--   0        0        0      877 2023-04-24 02:18:25.042900 arc_cli-8.1.1/arc/types/state.py
+-rw-r--r--   0        0        0     1921 2023-04-24 02:18:25.046233 arc_cli-8.1.1/arc/types/strings.py
+-rw-r--r--   0        0        0     2155 2023-04-24 02:18:25.046233 arc_cli-8.1.1/arc/types/type_arg.py
+-rw-r--r--   0        0        0     2718 2023-04-24 02:18:25.046233 arc_cli-8.1.1/arc/types/type_info.py
+-rw-r--r--   0        0        0     3176 2023-04-24 02:18:25.046233 arc_cli-8.1.1/arc/types/users.py
+-rw-r--r--   0        0        0     2257 2023-04-24 02:18:25.046233 arc_cli-8.1.1/arc/typing.py
+-rw-r--r--   0        0        0     1043 2023-04-30 19:17:23.583678 arc_cli-8.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1886 1970-01-01 00:00:00.000000 arc_cli-8.1.1/setup.py
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 arc_cli-8.1.1/PKG-INFO
```

### Comparing `arc_cli-8.1.0/README.md` & `arc_cli-8.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ```py
 import arc
 
 @arc.command
 def hello(name: str):
     """My first arc program!"""
-    arc.arc.print(f"Hello {name}!")
+    arc.print(f"Hello {name}!")
 
 hello()
 ```
 
 ```
 $ python hello.py Sean
 Hello, Sean!
```

### Comparing `arc_cli-8.1.0/arc/__init__.py` & `arc_cli-8.1.1/arc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "8.1.0"
+__version__ = "8.1.1"
 
 from arc import types, prompt, present, errors
 from arc.config import (
     ColorConfig,
     Config,
     LinksConfig,
     SuggestionConfig,
```

### Comparing `arc_cli-8.1.0/arc/api.py` & `arc_cli-8.1.1/arc/api.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/autocompletions.py` & `arc_cli-8.1.1/arc/autocompletions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/autoload.py` & `arc_cli-8.1.1/arc/autoload.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/config.py` & `arc_cli-8.1.1/arc/config.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/alias.py` & `arc_cli-8.1.1/arc/define/alias.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/classful.py` & `arc_cli-8.1.1/arc/define/classful.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/command.py` & `arc_cli-8.1.1/arc/define/command.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/documentation.py` & `arc_cli-8.1.1/arc/define/documentation.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/param/constructors.py` & `arc_cli-8.1.1/arc/define/param/constructors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/param/groups.py` & `arc_cli-8.1.1/arc/define/param/groups.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/param/param.py` & `arc_cli-8.1.1/arc/define/param/param.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/param/param_definition.py` & `arc_cli-8.1.1/arc/define/param/param_definition.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/param/param_mixin.py` & `arc_cli-8.1.1/arc/define/param/param_mixin.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/define/param/param_tree.py` & `arc_cli-8.1.1/arc/define/param/param_tree.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/errors.py` & `arc_cli-8.1.1/arc/errors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/logging.py` & `arc_cli-8.1.1/arc/logging.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/parser.py` & `arc_cli-8.1.1/arc/parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/ansi.py` & `arc_cli-8.1.1/arc/present/ansi.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/box.py` & `arc_cli-8.1.1/arc/present/box.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/console.py` & `arc_cli-8.1.1/arc/present/console.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/drawing.py` & `arc_cli-8.1.1/arc/present/drawing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/formatters.py` & `arc_cli-8.1.1/arc/present/formatters.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/help_formatter.py` & `arc_cli-8.1.1/arc/present/help_formatter.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/joiner.py` & `arc_cli-8.1.1/arc/present/joiner.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/markdown/markdown_parser.py` & `arc_cli-8.1.1/arc/present/markdown/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/markdown/nodes.py` & `arc_cli-8.1.1/arc/present/markdown/nodes.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/out.py` & `arc_cli-8.1.1/arc/present/out.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/pager.py` & `arc_cli-8.1.1/arc/present/pager.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/table.py` & `arc_cli-8.1.1/arc/present/table.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/present/wrap.py` & `arc_cli-8.1.1/arc/present/wrap.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/prompt/helpers.py` & `arc_cli-8.1.1/arc/prompt/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 import re
 import sys
-import termios
 import tty
 import typing as t
 from contextlib import contextmanager
 
 T = t.TypeVar("T")
 
 
@@ -20,25 +19,31 @@
     return f"\033[{num}K"
 
 
 class RawTerminal:
     __raw: bool = False
     __old_settings: list[t.Any]
 
+    def __init__(self) -> None:
+        # Moved into here to support pyodide
+        import termios
+
+        self.termios = termios
+
     def __enter__(self) -> RawTerminal:
         fd = sys.stdin.fileno()
-        self.__old_settings = termios.tcgetattr(fd)
+        self.__old_settings = self.termios.tcgetattr(fd)
         tty.setraw(sys.stdin.fileno())
         self.__raw = True
         return self
 
     def __exit__(self, *args: t.Any) -> None:
         fd = sys.stdin.fileno()
         self.__raw = False
-        termios.tcsetattr(fd, termios.TCSADRAIN, self.__old_settings)
+        self.termios.tcsetattr(fd, self.termios.TCSADRAIN, self.__old_settings)
 
     def getch(self) -> str:
         assert self.__raw, "Cannot getch() when not in raw mode"
         return sys.stdin.read(1)
 
 
 class Cursor:
```

### Comparing `arc_cli-8.1.0/arc/prompt/prompt.py` & `arc_cli-8.1.1/arc/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/prompt/prompts.py` & `arc_cli-8.1.1/arc/prompt/prompts.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/prompt/questions.py` & `arc_cli-8.1.1/arc/prompt/questions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/runtime/app.py` & `arc_cli-8.1.1/arc/runtime/app.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/runtime/context.py` & `arc_cli-8.1.1/arc/runtime/context.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/runtime/exec.py` & `arc_cli-8.1.1/arc/runtime/exec.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/runtime/init.py` & `arc_cli-8.1.1/arc/runtime/init.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/runtime/middleware.py` & `arc_cli-8.1.1/arc/runtime/middleware.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/suggest.py` & `arc_cli-8.1.1/arc/suggest.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/aliases.py` & `arc_cli-8.1.1/arc/types/aliases.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/convert.py` & `arc_cli-8.1.1/arc/types/convert.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/default.py` & `arc_cli-8.1.1/arc/types/default.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/file.py` & `arc_cli-8.1.1/arc/types/file.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/middleware/observers.py` & `arc_cli-8.1.1/arc/types/middleware/observers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/middleware/transformers.py` & `arc_cli-8.1.1/arc/types/middleware/transformers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/middleware/validators.py` & `arc_cli-8.1.1/arc/types/middleware/validators.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/network.py` & `arc_cli-8.1.1/arc/types/network.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/numbers.py` & `arc_cli-8.1.1/arc/types/numbers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/path.py` & `arc_cli-8.1.1/arc/types/path.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/semver.py` & `arc_cli-8.1.1/arc/types/semver.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/state.py` & `arc_cli-8.1.1/arc/types/state.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/strings.py` & `arc_cli-8.1.1/arc/types/strings.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/type_arg.py` & `arc_cli-8.1.1/arc/types/type_arg.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/type_info.py` & `arc_cli-8.1.1/arc/types/type_info.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/types/users.py` & `arc_cli-8.1.1/arc/types/users.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/arc/typing.py` & `arc_cli-8.1.1/arc/typing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.0/pyproject.toml` & `arc_cli-8.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arc-cli"
-version = "8.1.0"
+version = "8.1.1"
 description = "A Regular CLI"
 authors = ["Sean Collings <seanrcollings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/arc"
 documentation = "https://arc.seanrcollings.com"
 keywords = ["CLI", "extendable", "easy", "arc"]
```

### Comparing `arc_cli-8.1.0/setup.py` & `arc_cli-8.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 ['hypothesis>=6.68.2,<7.0.0']
 
 entry_points = \
 {'console_scripts': ['cli = cli:command']}
 
 setup_kwargs = {
     'name': 'arc-cli',
-    'version': '8.1.0',
+    'version': '8.1.1',
     'description': 'A Regular CLI',
-    'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# [Docs](http://arc.seanrcollings.com)\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
+    'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# [Docs](http://arc.seanrcollings.com)\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
     'author': 'Sean Collings',
     'author_email': 'seanrcollings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/arc',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `arc_cli-8.1.0/PKG-INFO` & `arc_cli-8.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arc-cli
-Version: 8.1.0
+Version: 8.1.1
 Summary: A Regular CLI
 Home-page: https://github.com/seanrcollings/arc
 License: MIT
 Keywords: CLI,extendable,easy,arc
 Author: Sean Collings
 Author-email: seanrcollings@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -34,15 +34,15 @@
 
 ```py
 import arc
 
 @arc.command
 def hello(name: str):
     """My first arc program!"""
-    arc.arc.print(f"Hello {name}!")
+    arc.print(f"Hello {name}!")
 
 hello()
 ```
 
 ```
 $ python hello.py Sean
 Hello, Sean!
```

