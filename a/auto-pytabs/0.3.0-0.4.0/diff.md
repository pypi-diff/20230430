# Comparing `tmp/auto_pytabs-0.3.0.tar.gz` & `tmp/auto_pytabs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_pytabs-0.3.0.tar", max compression
+gzip compressed data, was "auto_pytabs-0.4.0.tar", max compression
```

## Comparing `auto_pytabs-0.3.0.tar` & `auto_pytabs-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/LICENSE
--rw-r--r--   0        0        0    12172 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/__init__.py
--rw-r--r--   0        0        0     5391 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/core.py
--rw-r--r--   0        0        0     6364 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/markdown_ext.py
--rw-r--r--   0        0        0     1556 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/mkdocs_plugin.py
--rw-r--r--   0        0        0     6915 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/sphinx_ext.py
--rw-r--r--   0        0        0     2089 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 auto_pytabs-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-30 11:35:49.082567 auto_pytabs-0.4.0/LICENSE
+-rw-r--r--   0        0        0    13940 2023-04-30 11:35:49.082567 auto_pytabs-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 11:35:49.082567 auto_pytabs-0.4.0/auto_pytabs/__init__.py
+-rw-r--r--   0        0        0     5391 2023-04-30 11:35:49.082567 auto_pytabs-0.4.0/auto_pytabs/core.py
+-rw-r--r--   0        0        0     7740 2023-04-30 11:35:49.082567 auto_pytabs-0.4.0/auto_pytabs/markdown_ext.py
+-rw-r--r--   0        0        0     1823 2023-04-30 11:35:49.082567 auto_pytabs-0.4.0/auto_pytabs/mkdocs_plugin.py
+-rw-r--r--   0        0        0     8275 2023-04-30 11:35:49.082567 auto_pytabs-0.4.0/auto_pytabs/sphinx_ext.py
+-rw-r--r--   0        0        0     2094 2023-04-30 11:35:49.082567 auto_pytabs-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    14756 1970-01-01 00:00:00.000000 auto_pytabs-0.4.0/PKG-INFO
```

### Comparing `auto_pytabs-0.3.0/LICENSE` & `auto_pytabs-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_pytabs-0.3.0/README.md` & `auto_pytabs-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -73,49 +73,57 @@
   - pymdownx.tabbed:
 plugins:
   - auto_pytabs:
       min_version: "3.7"  # optional
       max_version: "3.11" # optional
       tab_title_template: "Python {min_version}+"  # optional
       no_cache: false  # optional
+      default_tab: "highest"  # optional
+      reverse_order: false  # optional
 ```
 
 *Available configuration options*
 
-| Name                 | Default                   | Description                 |
-| -------------------- | ------------------------- | --------------------------- |
-| `min_version`        | `(3, 7)`                  | Minimum python version      |
-| `max_version`        | `(3, 7)`                  | Maximum python version      |
-| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles     |
-| `no_cache`           | `False`                   | Disable file system caching |
+| Name                 | Default                   | Description                                                                |
+| -------------------- | ------------------------- | -------------------------------------------------------------------------- |
+| `min_version`        | `(3, 7)`                  | Minimum python version                                                     |
+| `max_version`        | `(3, 7)`                  | Maximum python version                                                     |
+| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles                                                    |
+| `no_cache`           | `False`                   | Disable file system caching                                                |
+| `default_tab`        | `highest`                 | (`highest` or `lowest`) Version tab to preselect                           |
+| `reverse_order`      | `False`                   | Reverse the order of tabs. Default is to go from lowest to highest version |
 
 #### Markdown extension
 
 ```python
 import markdown
 
 md = markdown.Markdown(
     extensions=["auto_pytabs"],
     extension_configs={
         "auto_pytabs": {
             "min_version": "3.7",  # optional
             "max_version": "3.11",  # optional
             "tab_title_template": "Python {min_version}+",  # optional
+            "default_tab": "highest",  # optional
+            "reverse_order": False,  # optional
         }
     },
 )
 ```
 
 *Available configuration options*
 
-| Name                 | Default                   | Description                                 |
-| -------------------- | ------------------------- | ------------------------------------------- |
-| `min_version`        | `(3, 7)`                  | Minimum python version to generate code for |
-| `max_version`        | `(3, 7)`                  | Maximum python version to generate code for |
-| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles                     |
+| Name                 | Default                   | Description                                                                |
+| -------------------- | ------------------------- | -------------------------------------------------------------------------- |
+| `min_version`        | `(3, 7)`                  | Minimum python version to generate code for                                |
+| `max_version`        | `(3, 7)`                  | Maximum python version to generate code for                                |
+| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles                                                    |
+| `default_tab`        | `highest`                 | (`highest` or `lowest`) Version tab to preselect                           |
+| `reverse_order`      | `False`                   | Reverse the order of tabs. Default is to go from lowest to highest version |
 
 ### Differences between the mkdocs plugin and markdown extension
 
 AutoPyTabs ships as a markdown extension and an mkdocs plugin, both of which can be used in mkdocs. The only difference
 between them is that the mkdocs plugin supports caching, which can make subsequent builds faster (i.e. when using `mkdocs serve`).
 The reason why the markdown extension does not support caching is that `markdown` does not have clearly defined build
 steps with wich an extension could interact (like mkdocs [plugin events](https://www.mkdocs.org/dev-guide/plugins/#events)),
@@ -281,25 +289,29 @@
 extensions = ["auto_pytabs.sphinx_ext", "sphinx_design"]
 
 auto_pytabs_min_version = (3, 7)  # optional
 auto_pytabs_max_version = (3, 11)  # optional
 auto_pytabs_tab_title_template = "Python {min_version}+"  # optional 
 # auto_pytabs_no_cache = True  # disabled file system caching
 # auto_pytabs_compat_mode = True  # enable compatibility mode
+# auto_pytabs_default_tab = "lowest"  # Pre-select the tab with the lowest version
+# auto_pytabs_reverse_order = True  # reverse the order of tabs to highest > lowest
 ```
 
 #### Available configuration options
 
-| Name                             | Default                   | Description                                      |
-| -------------------------------- | ------------------------- | ------------------------------------------------ |
-| `auto_pytabs_min_version`        | `(3, 7)`                  | Minimum python version to generate code for      |
-| `auto_pytabs_max_version`        | `(3, 7)`                  | Maximum python version to generate code for      |
-| `auto_pytabs_tab_title_template` | `"Python {min_version}+"` | Template for tab titles                          |
-| `auto_pytabs_no_cache`           | `False`                   | Disable file system caching                      |
-| `auto_pytabs_compat_mode`        | `False`                   | Enable [compatibility mode](#compatibility-mode) |
+| Name                             | Default                   | Description                                                                |
+| -------------------------------- | ------------------------- | -------------------------------------------------------------------------- |
+| `auto_pytabs_min_version`        | `(3, 7)`                  | Minimum python version to generate code for                                |
+| `auto_pytabs_max_version`        | `(3, 7)`                  | Maximum python version to generate code for                                |
+| `auto_pytabs_tab_title_template` | `"Python {min_version}+"` | Template for tab titles                                                    |
+| `auto_pytabs_no_cache`           | `False`                   | Disable file system caching                                                |
+| `auto_pytabs_compat_mode`        | `False`                   | Enable [compatibility mode](#compatibility-mode)                           |
+| `auto_pytabs_default_tab`        | `highest`                 | Either `highest` or `lowest`. Version tab to preselect                     |
+| `auto_pytabs_reverse_order`      | `False`                   | Reverse the order of tabs. Default is to go from lowest to highest version |
 
 <h3 id="sphinx-examples">Examples</h3>
 
 **Input**
 
 ```rst
 .. code-block:: python
```

### Comparing `auto_pytabs-0.3.0/auto_pytabs/core.py` & `auto_pytabs-0.4.0/auto_pytabs/core.py`

 * *Files identical despite different names*

### Comparing `auto_pytabs-0.3.0/auto_pytabs/mkdocs_plugin.py` & `auto_pytabs-0.4.0/auto_pytabs/mkdocs_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 
 class PluginConfig(Config):  # type: ignore[no-untyped-call]
     min_version = config_options.Type(str, default="3.7")
     max_version = config_options.Type(str, default="3.11")
     tab_title_template = config_options.Type(str, default="Python {min_version}+")
     no_cache = config_options.Type(bool, default=False)
+    default_tab = config_options.Choice(["highest", "lowest"], default="highest")
+    reverse_order = config_options.Type(bool, default=False)
 
 
 class AutoPyTabsPlugin(BasePlugin[PluginConfig]):  # type: ignore[no-untyped-call]
     def __init__(self) -> None:
         self.cache: Cache | None = None
 
     def on_config(self, config: MkDocsConfig) -> Config | None:
@@ -31,14 +33,16 @@
         config["mdx_configs"].update(
             {
                 "auto_pytabs": {
                     "min_version": self.config.min_version,
                     "max_version": self.config.max_version,
                     "tab_title_template": self.config.tab_title_template,
                     "cache": self.cache,
+                    "default_tab": self.config.default_tab,
+                    "reverse_order": self.config.reverse_order,
                 }
             }
         )
         return None
 
     def on_post_build(self, config: MkDocsConfig) -> None:
         if self.cache:
```

### Comparing `auto_pytabs-0.3.0/auto_pytabs/sphinx_ext.py` & `auto_pytabs-0.4.0/auto_pytabs/sphinx_ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import importlib
 import importlib.metadata
 from collections.abc import Iterable
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, Literal, cast
 
 from docutils.nodes import Node, container, section
 from docutils.parsers.rst import directives
 from docutils.statemachine import ViewList
 from sphinx.directives.code import CodeBlock, LiteralInclude
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util.nodes import nested_parse_with_titles
@@ -21,66 +21,106 @@
 
 if TYPE_CHECKING:
     from sphinx.application import Sphinx
     from sphinx.config import Config
     from sphinx.environment import BuildEnvironment
 
 
-def indent(string: str, indent_char: str = " ", level: int = 4) -> list[str]:
-    return list((indent_char * level) + line for line in string.splitlines())
+def indent(
+    text: str | Iterable[str], indent_char: str = " ", level: int = 4
+) -> list[str]:
+    lines = text.splitlines() if isinstance(text, str) else text
+    return list((indent_char * level) + line for line in lines)
+
+
+def _render_directive(
+    *,
+    name: str,
+    argument: str = "",
+    options: dict[str, Any] | None = None,
+    body: str | Iterable[str],
+) -> list[str]:
+    directive = [f".. {name}:: {argument}"]
+    if options:
+        rendered_options = [
+            f":{option}: {value if (value is not True and value) else ''}"
+            for option, value in options.items()
+            if value is not False
+        ]
+        directive.extend(indent(rendered_options))
+
+    directive.append("")
+    directive.extend(indent(body))
+
+    return directive
 
 
 class UpgradeMixin(SphinxDirective):
     compat: bool = False
 
-    def _render_directive_options(self) -> str:
-        ret = ""
-        options: dict[str, Any] = {
-            k: v for k, v in self.options.items() if k in CodeBlock.option_spec
-        }
+    def _get_directive_options(self) -> dict[str, Any]:
+        options: dict[str, Any] = {}
         if not self.compat:
             options["no-upgrade"] = True
-        for option, value in options.items():
+        for option, value in self.options.items():
+            if option not in CodeBlock.option_spec:
+                continue
             if self.option_spec[option] is directives.flag:
-                value = None
+                value = True
             if isinstance(value, Iterable) and not isinstance(value, str):
                 value = "\n".join(value)
-            ret += f":{option}: {value if value is not None else ''}\n"
-        return ret
+            options[option] = value
+        return options
 
     def _create_tabs(
         self,
         versioned_code: VersionedCode,
         tab_title_template: str,
     ) -> list[str]:
+        directive_options = self._get_directive_options()
         if len(versioned_code) == 1:
-            return [
-                ".. code-block:: python",
-                *indent(self._render_directive_options()),
-                "",
-                *indent(versioned_code.popitem()[1]),
-                "",
-            ]
+            return _render_directive(
+                name="code-block",
+                argument="python",
+                body=versioned_code.popitem()[1],
+                options=directive_options,
+            )
+
+        default_tab_strategy: Literal["highest", "lowest"] = self.config[
+            "auto_pytabs_default_tab"
+        ]
+        versions = list(versioned_code.keys())
+        default_selected_version = versions[
+            -1 if default_tab_strategy == "highest" else 0
+        ]
+
+        tab_set_body = []
+        if self.config["auto_pytabs_reverse_order"]:
+            versioned_code = dict(reversed(versioned_code.items()))
 
-        out = [".. tab-set::", ""]
         for version, code in versioned_code.items():
             version_string = f"{version[0]}.{version[1]}"
-            out.extend(
-                [
-                    f"    .. tab-item:: {tab_title_template.format(min_version=version_string)}",  # noqa: E501
-                    f"        :sync: {version_string}",
-                    "",
-                    "        .. code-block:: python",
-                    *indent(self._render_directive_options(), level=12),
-                    "",
-                    *indent(code, level=12),
-                    "",
-                ]
+            code_block = _render_directive(
+                name="code-block",
+                argument="python",
+                options=directive_options,
+                body=code,
+            )
+            tab_item = _render_directive(
+                name="tab-item",
+                argument=tab_title_template.format(min_version=version_string),
+                options={
+                    "sync": version_string,
+                    "selected": version == default_selected_version,
+                },
+                body=code_block,
             )
-        return out
+            tab_set_body.extend(tab_item)
+
+        return _render_directive(name="tab-set", body=tab_set_body)
 
     @property
     def cache(self) -> Cache | None:
         return getattr(self.env, "auto_pytabs_cache", None)
 
     def _create_py_tab_nodes(self, code: str) -> list[Node]:
         version_requirements = self.config["auto_pytabs_versions"]
@@ -188,14 +228,16 @@
         default="Python {min_version}+",
         rebuild="html",
     )
     app.add_config_value("auto_pytabs_min_version", default=(3, 7), rebuild="html")
     app.add_config_value("auto_pytabs_max_version", default=(3, 11), rebuild="html")
     app.add_config_value("auto_pytabs_no_cache", default=False, rebuild="html")
     app.add_config_value("auto_pytabs_compat_mode", default=False, rebuild="html")
+    app.add_config_value("auto_pytabs_default_tab", default="highest", rebuild="html")
+    app.add_config_value("auto_pytabs_reverse_order", default=False, rebuild="html")
 
     app.connect("config-inited", on_config_inited)
     app.connect("build-finished", on_build_finished)
     app.connect("env-before-read-docs", on_env_before_read_docs)
     app.connect("env-merge-info", on_env_merge_info)
 
     return {
```

### Comparing `auto_pytabs-0.3.0/pyproject.toml` & `auto_pytabs-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "auto-pytabs"
-version = "0.3.0"
+version = "0.4.0"
 description = "Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations"
 authors = ["Janek Nouvertné <provinzkraut@posteo.de>"]
 readme = "README.md"
 packages = [{ include = "auto_pytabs" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+ruff = ">=0.0.260"
 sphinx = { version = ">=4", optional = true }
 markdown = {version = ">=3.2.1", optional = true }
-mkdocs = {version = "^1.4.2", optional = true}
-ruff = "^0.0.260"
+mkdocs = {version = ">=1.4.2,<2", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 mypy = "^0.990"
 types-markdown = "^3.4.2.1"
 pytest = "^7.2.0"
 pymdown-extensions = "^9.9"
```

### Comparing `auto_pytabs-0.3.0/PKG-INFO` & `auto_pytabs-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: auto-pytabs
-Version: 0.3.0
+Version: 0.4.0
 Summary: Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations
 Author: Janek Nouvertné
 Author-email: provinzkraut@posteo.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: markdown
 Provides-Extra: mkdocs
 Provides-Extra: sphinx
 Requires-Dist: markdown (>=3.2.1) ; extra == "markdown"
-Requires-Dist: mkdocs (>=1.4.2,<2.0.0) ; extra == "mkdocs"
-Requires-Dist: ruff (>=0.0.260,<0.0.261)
+Requires-Dist: mkdocs (>=1.4.2,<2) ; extra == "mkdocs"
+Requires-Dist: ruff (>=0.0.260)
 Requires-Dist: sphinx (>=4) ; extra == "sphinx"
 Description-Content-Type: text/markdown
 
 # AutoPyTabs
 
 Automatically generate code examples for different Python versions in
 [mkdocs](https://www.mkdocs.org) or [Sphinx](https://www.sphinx-doc.org) based documentations, or a plain
@@ -94,49 +94,57 @@
   - pymdownx.tabbed:
 plugins:
   - auto_pytabs:
       min_version: "3.7"  # optional
       max_version: "3.11" # optional
       tab_title_template: "Python {min_version}+"  # optional
       no_cache: false  # optional
+      default_tab: "highest"  # optional
+      reverse_order: false  # optional
 ```
 
 *Available configuration options*
 
-| Name                 | Default                   | Description                 |
-| -------------------- | ------------------------- | --------------------------- |
-| `min_version`        | `(3, 7)`                  | Minimum python version      |
-| `max_version`        | `(3, 7)`                  | Maximum python version      |
-| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles     |
-| `no_cache`           | `False`                   | Disable file system caching |
+| Name                 | Default                   | Description                                                                |
+| -------------------- | ------------------------- | -------------------------------------------------------------------------- |
+| `min_version`        | `(3, 7)`                  | Minimum python version                                                     |
+| `max_version`        | `(3, 7)`                  | Maximum python version                                                     |
+| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles                                                    |
+| `no_cache`           | `False`                   | Disable file system caching                                                |
+| `default_tab`        | `highest`                 | (`highest` or `lowest`) Version tab to preselect                           |
+| `reverse_order`      | `False`                   | Reverse the order of tabs. Default is to go from lowest to highest version |
 
 #### Markdown extension
 
 ```python
 import markdown
 
 md = markdown.Markdown(
     extensions=["auto_pytabs"],
     extension_configs={
         "auto_pytabs": {
             "min_version": "3.7",  # optional
             "max_version": "3.11",  # optional
             "tab_title_template": "Python {min_version}+",  # optional
+            "default_tab": "highest",  # optional
+            "reverse_order": False,  # optional
         }
     },
 )
 ```
 
 *Available configuration options*
 
-| Name                 | Default                   | Description                                 |
-| -------------------- | ------------------------- | ------------------------------------------- |
-| `min_version`        | `(3, 7)`                  | Minimum python version to generate code for |
-| `max_version`        | `(3, 7)`                  | Maximum python version to generate code for |
-| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles                     |
+| Name                 | Default                   | Description                                                                |
+| -------------------- | ------------------------- | -------------------------------------------------------------------------- |
+| `min_version`        | `(3, 7)`                  | Minimum python version to generate code for                                |
+| `max_version`        | `(3, 7)`                  | Maximum python version to generate code for                                |
+| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles                                                    |
+| `default_tab`        | `highest`                 | (`highest` or `lowest`) Version tab to preselect                           |
+| `reverse_order`      | `False`                   | Reverse the order of tabs. Default is to go from lowest to highest version |
 
 ### Differences between the mkdocs plugin and markdown extension
 
 AutoPyTabs ships as a markdown extension and an mkdocs plugin, both of which can be used in mkdocs. The only difference
 between them is that the mkdocs plugin supports caching, which can make subsequent builds faster (i.e. when using `mkdocs serve`).
 The reason why the markdown extension does not support caching is that `markdown` does not have clearly defined build
 steps with wich an extension could interact (like mkdocs [plugin events](https://www.mkdocs.org/dev-guide/plugins/#events)),
@@ -302,25 +310,29 @@
 extensions = ["auto_pytabs.sphinx_ext", "sphinx_design"]
 
 auto_pytabs_min_version = (3, 7)  # optional
 auto_pytabs_max_version = (3, 11)  # optional
 auto_pytabs_tab_title_template = "Python {min_version}+"  # optional 
 # auto_pytabs_no_cache = True  # disabled file system caching
 # auto_pytabs_compat_mode = True  # enable compatibility mode
+# auto_pytabs_default_tab = "lowest"  # Pre-select the tab with the lowest version
+# auto_pytabs_reverse_order = True  # reverse the order of tabs to highest > lowest
 ```
 
 #### Available configuration options
 
-| Name                             | Default                   | Description                                      |
-| -------------------------------- | ------------------------- | ------------------------------------------------ |
-| `auto_pytabs_min_version`        | `(3, 7)`                  | Minimum python version to generate code for      |
-| `auto_pytabs_max_version`        | `(3, 7)`                  | Maximum python version to generate code for      |
-| `auto_pytabs_tab_title_template` | `"Python {min_version}+"` | Template for tab titles                          |
-| `auto_pytabs_no_cache`           | `False`                   | Disable file system caching                      |
-| `auto_pytabs_compat_mode`        | `False`                   | Enable [compatibility mode](#compatibility-mode) |
+| Name                             | Default                   | Description                                                                |
+| -------------------------------- | ------------------------- | -------------------------------------------------------------------------- |
+| `auto_pytabs_min_version`        | `(3, 7)`                  | Minimum python version to generate code for                                |
+| `auto_pytabs_max_version`        | `(3, 7)`                  | Maximum python version to generate code for                                |
+| `auto_pytabs_tab_title_template` | `"Python {min_version}+"` | Template for tab titles                                                    |
+| `auto_pytabs_no_cache`           | `False`                   | Disable file system caching                                                |
+| `auto_pytabs_compat_mode`        | `False`                   | Enable [compatibility mode](#compatibility-mode)                           |
+| `auto_pytabs_default_tab`        | `highest`                 | Either `highest` or `lowest`. Version tab to preselect                     |
+| `auto_pytabs_reverse_order`      | `False`                   | Reverse the order of tabs. Default is to go from lowest to highest version |
 
 <h3 id="sphinx-examples">Examples</h3>
 
 **Input**
 
 ```rst
 .. code-block:: python
```

