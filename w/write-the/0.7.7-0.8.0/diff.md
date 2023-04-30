# Comparing `tmp/write_the-0.7.7.tar.gz` & `tmp/write_the-0.8.0.tar.gz`

## Comparing `write_the-0.7.7.tar` & `write_the-0.8.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.7.7/mkdocs.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.7.7/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.7.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.7.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/CNAME
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/index.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/cli.md
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/commands.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/cst.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/llm.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.7/docs/reference/utils.md
--rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.7.7/images/docs-help.png
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.7.7/images/logo-black.svg
--rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.7.7/images/logo.png
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.7.7/images/mkdocs-help.png
--rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.7.7/images/multiply-docs-tests.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.7.7/images/tests-help.png
--rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.7.7/images/untitled.blend
--rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.7.7/images/untitled.blend1
--rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.7.7/images/write-the-docs.gif
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.7.7/images/write-the-icon.svg
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.7.7/images/write-the.svg
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cli_main.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_cst_utils.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/test_utils.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/data/calculate.py
--rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/data/expected.dat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/data/multiply.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.7.7/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/__main__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/llm.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cli/__init__.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cli/main.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cli/tasks.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/docs/__init__.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/docs/docs.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/docs/prompts.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/docs/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/mkdocs/__init__.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/mkdocs/mkdocs.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/mkdocs/templates.py
--rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/tests/prompts.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/commands/tests/tests.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.7.7/write_the/cst/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 write_the-0.7.7/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.7.7/LICENSE.txt
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 write_the-0.7.7/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 write_the-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 write_the-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.8.0/mkdocs.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.8.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.8.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.8.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/CNAME
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/index.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/cli.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/commands.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/cst.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/llm.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/utils.md
+-rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.8.0/images/docs-help.png
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.8.0/images/logo-black.svg
+-rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.8.0/images/logo.png
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.8.0/images/mkdocs-help.png
+-rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.8.0/images/multiply-docs-tests.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.8.0/images/tests-help.png
+-rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.8.0/images/untitled.blend
+-rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.8.0/images/untitled.blend1
+-rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.8.0/images/write-the-docs.gif
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.8.0/images/write-the-icon.svg
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.8.0/images/write-the.svg
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cli_main.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_utils.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_utils.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/data/calculate.py
+-rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/data/expected.dat
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/data/multiply.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/__main__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/llm.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cli/main.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cli/tasks.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/docs/__init__.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/docs/docs.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/docs/prompts.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/docs/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/mkdocs/__init__.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/mkdocs/mkdocs.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/mkdocs/templates.py
+-rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/tests/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/tests/prompts.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/tests/tests.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/node_batcher.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 write_the-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 write_the-0.8.0/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 write_the-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 write_the-0.8.0/PKG-INFO
```

### Comparing `write_the-0.7.7/mkdocs.yml` & `write_the-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/.github/workflows/publish.yml` & `write_the-0.8.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/.github/workflows/tests.yml` & `write_the-0.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/docs/index.md` & `write_the-0.8.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/docs-help.png` & `write_the-0.8.0/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/logo-black.svg` & `write_the-0.8.0/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/logo.png` & `write_the-0.8.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/mkdocs-help.png` & `write_the-0.8.0/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/multiply-docs-tests.png` & `write_the-0.8.0/images/multiply-docs-tests.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/tests-help.png` & `write_the-0.8.0/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/untitled.blend` & `write_the-0.8.0/images/untitled.blend`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/untitled.blend1` & `write_the-0.8.0/images/untitled.blend1`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/write-the-docs.gif` & `write_the-0.8.0/images/write-the-docs.gif`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/write-the-icon.svg` & `write_the-0.8.0/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/images/write-the.svg` & `write_the-0.8.0/images/write-the.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/tests/test_cli_main.py` & `write_the-0.8.0/tests/test_cli_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from write_the.cli.main import app
 from write_the.llm import LLM
 from typer.testing import CliRunner
 import unittest.mock as mock
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def file_path(tmp_path) -> Path:
     temp_file = tmp_path / "test_add.py"
     temp_file.write_text("def add(a, b):\n  return a + b")
     return temp_file
 
 
 @pytest.fixture
@@ -32,15 +32,18 @@
         (True, True, True, True),
         (True, True, True, False),
         (True, True, False, True),
         (True, False, True, True),
         (False, True, True, True),
     ],
 )
-@mock.patch('write_the.llm.LLM.run', return_value="\n\nadd:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n")
+@mock.patch(
+    "write_the.llm.LLM.run",
+    return_value="\n\nadd:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n",
+)
 def test_docs_mocked(mocked_run, file_path: Path, nodes, save, context, pretty, force):
     runner = CliRunner()
     args = ["docs", str(file_path)]
 
     if nodes:
         for node in nodes:
             args.append("--node")
@@ -71,37 +74,40 @@
 def test_mkdocs(tmp_path: Path):
     runner = CliRunner()
     args = ["mkdocs", "tests/data", "--readme", "README.md", "--out", tmp_path]
     result = runner.invoke(app, args)
     print(result.stdout)
     assert result.exit_code == 0
     files = [f.name for f in tmp_path.glob("*")]
-    assert 'mkdocs.yml' in files
-    assert '.github' in files
-    assert 'docs' in files
+    assert "mkdocs.yml" in files
+    assert ".github" in files
+    assert "docs" in files
 
 
 @pytest.mark.parametrize(
     "save, pretty, force",
     [
         (True, True, True),
         (True, True, True),
         (True, True, False),
         (True, False, True),
         (False, True, True),
     ],
 )
-@mock.patch('write_the.llm.LLM.run', return_value="""@pytest.mark.parametrize(
+@mock.patch(
+    "write_the.llm.LLM.run",
+    return_value="""@pytest.mark.parametrize(
     "a, b, expected", [(2, 3, 5), (0, 5, 5), (-2, -3, -5), (2.5, 3, 5.5), (2, -3, -1)]
 )
 def test_add(a, b, expected):
-    assert add(a, b) == expected""")
+    assert add(a, b) == expected""",
+)
 def test_tests_mocked(mocked_run, file_path: Path, save, pretty, force):
     runner = CliRunner()
-    test_dir = file_path.parent / 'docs'
+    test_dir = file_path.parent / "docs"
     args = ["tests", str(file_path), "--out", test_dir]
 
     if save:
         args.append("--save")
 
     if pretty:
         args.append("--pretty")
@@ -113,8 +119,8 @@
     assert result.exit_code == 0
     mocked_run.assert_called_once()
     if save:
         test_file = next(test_dir.glob("*test_add.py"))
         assert "assert add(a, b) == expected" in test_file.read_text()
         assert str(file_path) in result.stdout
     else:
-        assert "assert add(a, b) == expected" in result.stdout
+        assert "assert add(a, b) == expected" in result.stdout
```

### Comparing `write_the-0.7.7/tests/test_cst_docstring_adder.py` & `write_the-0.8.0/tests/test_cst_docstring_adder.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,36 +18,36 @@
 
 
 @pytest.fixture
 def function_def_node():
     return cst.FunctionDef(
         name=cst.Name("function_name"),
         params=cst.Parameters(),
-        body=cst.IndentedBlock(
-            body=[cst.SimpleStatementLine(body=[cst.Pass()])]),
+        body=cst.IndentedBlock(body=[cst.SimpleStatementLine(body=[cst.Pass()])]),
     )
 
 
 @pytest.fixture
 def class_def_node():
-    return cst.ClassDef(name=cst.Name("ClassName"), body=cst.IndentedBlock(body=[cst.SimpleStatementLine(body=[cst.Pass()])]))
+    return cst.ClassDef(
+        name=cst.Name("ClassName"),
+        body=cst.IndentedBlock(body=[cst.SimpleStatementLine(body=[cst.Pass()])]),
+    )
 
 
 @pytest.fixture
 def method_def_node():
     method_def = cst.FunctionDef(
         name=cst.Name("method_name"),
         params=cst.Parameters(params=[cst.Param(name=cst.Name("cls"))]),
-        body=cst.IndentedBlock(
-            body=[cst.SimpleStatementLine(body=[cst.Pass()])]),
+        body=cst.IndentedBlock(body=[cst.SimpleStatementLine(body=[cst.Pass()])]),
     )
     return cst.ClassDef(
         name=cst.Name("ClassName"),
-        body=cst.IndentedBlock(
-            body=[cst.SimpleStatementLine(body=[method_def])]),
+        body=cst.IndentedBlock(body=[cst.SimpleStatementLine(body=[method_def])]),
     )
 
 
 def test_leave_function_def_with_docstring(docstrings, force, function_def_node):
     docstring_adder = DocstringAdder(docstrings, force)
     updated_node = docstring_adder.leave_FunctionDef(
         function_def_node, function_def_node
@@ -62,36 +62,32 @@
         function_def_node, function_def_node
     )
     assert not has_docstring(updated_node)
 
 
 def test_leave_class_def_with_docstring(docstrings, force, class_def_node):
     docstring_adder = DocstringAdder(docstrings, force)
-    updated_node = docstring_adder.leave_ClassDef(
-        class_def_node, class_def_node)
+    updated_node = docstring_adder.leave_ClassDef(class_def_node, class_def_node)
     assert has_docstring(updated_node) is False
 
 
 def test_leave_class_def_without_docstring(docstrings, force, class_def_node):
     docstrings.pop("ClassName.method_name")
     docstring_adder = DocstringAdder(docstrings, force)
-    updated_node = docstring_adder.leave_ClassDef(
-        class_def_node, class_def_node)
+    updated_node = docstring_adder.leave_ClassDef(class_def_node, class_def_node)
     assert not has_docstring(updated_node)
 
 
 def test_leave_method_def_without_docstring(
     docstrings, force, class_def_node, method_def_node
 ):
     docstrings.pop("ClassName.method_name")
     docstring_adder = DocstringAdder(docstrings, force)
-    updated_node = docstring_adder.leave_ClassDef(
-        class_def_node, class_def_node)
-    updated_node = docstring_adder.leave_FunctionDef(
-        method_def_node, method_def_node)
+    updated_node = docstring_adder.leave_ClassDef(class_def_node, class_def_node)
+    updated_node = docstring_adder.leave_FunctionDef(method_def_node, method_def_node)
     assert not has_docstring(updated_node)
 
 
 def test_add_docstring_with_docstring(docstrings, force, function_def_node):
     docstring_adder = DocstringAdder(docstrings, force)
     updated_node = docstring_adder.add_docstring(function_def_node)
     assert has_docstring(updated_node)
@@ -106,14 +102,18 @@
 
 def test_add_docstring_with_force(docstrings, function_def_node):
     force = True
     docstring_adder = DocstringAdder(docstrings, force)
     updated_node = docstring_adder.add_docstring(function_def_node)
     assert has_docstring(updated_node)
 
+
 def test_add_docstring_escape_newline(docstrings, function_def_node):
     force = True
-    docstrings['function_name'] = """\\ntest\ntest\\\\n\\n"""
+    docstrings["function_name"] = """\\ntest\ntest\\\\n\\n"""
     docstring_adder = DocstringAdder(docstrings, force)
     updated_node = docstring_adder.add_docstring(function_def_node)
     assert has_docstring(updated_node)
-    assert get_docstring(updated_node).strip('"""').strip() == """\\\\ntest\n    test\\\\n\\\\n"""
+    assert (
+        get_docstring(updated_node).strip('"""').strip()
+        == """\\\\ntest\n    test\\\\n\\\\n"""
+    )
```

### Comparing `write_the-0.7.7/tests/test_cst_docstring_remover.py` & `write_the-0.8.0/tests/test_cst_docstring_remover.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import libcst as cst
 from write_the.cst.docstring_remover import DocstringRemover, remove_docstrings
 from write_the.cst.utils import get_docstring
 
+
 @pytest.fixture
 def tree():
     return cst.parse_module(
         """
 def foo():
     '''This is a docstring.'''
     pass
@@ -30,15 +31,15 @@
 def nodes():
     return ["foo", "Bar"]
 
 
 def test_leave_FunctionDef(tree, nodes):
     remover = DocstringRemover(nodes)
     updated_tree = tree.visit(remover)
-    assert get_docstring(updated_tree.body[0]) is None 
+    assert get_docstring(updated_tree.body[0]) is None
     assert get_docstring(updated_tree.body[1]) == "'''This is another docstring.'''"
 
 
 def test_leave_ClassDef(tree, nodes):
     remover = DocstringRemover(nodes)
     updated_tree = tree.visit(remover)
     assert get_docstring(updated_tree.body[2]) == "'''This is a class docstring.'''"
```

### Comparing `write_the-0.7.7/tests/test_cst_function_and_class_collector.py` & `write_the-0.8.0/tests/test_cst_function_and_class_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,12 +37,12 @@
 def test_visit_ClassDef_with_docstring(tree):
     collector = FunctionAndClassCollector(force=True)
     tree.visit(collector)
     assert collector.classes == ["Bar"]
 
 
 def test_get_node_names(tree, force):
-    assert get_node_names(tree, force) == ["foo", "Bar"]
+    assert get_node_names(tree, force) == ["Bar", "foo"]
 
 
 def test_get_node_names_with_force_true(tree, force):
-    assert get_node_names(tree, True) == ["foo", "Bar"]
+    assert get_node_names(tree, True) == ["Bar", "foo"]
```

### Comparing `write_the-0.7.7/tests/test_cst_node_extractor.py` & `write_the-0.8.0/tests/test_cst_node_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 import libcst as cst
 from write_the.cst.node_extractor import NodeExtractor, extract_nodes_from_tree
 
+
 @pytest.fixture
 def tree():
     return cst.parse_module(
         """
 def foo():
     pass
```

### Comparing `write_the-0.7.7/tests/test_cst_node_remover.py` & `write_the-0.8.0/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/tests/test_cst_utils.py` & `write_the-0.8.0/tests/test_cst_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 import libcst as cst
 from write_the.cst.utils import has_docstring, nodes_to_tree
 import pytest
 
+
 @pytest.fixture
 def cst_function_def():
     return cst.FunctionDef(
-    name=cst.Name("function_name"),
-    params=cst.Parameters(),
-    body=cst.IndentedBlock(
-        body=[
-            cst.SimpleStatementLine(body=[cst.Expr(value=cst.SimpleString('"""This is a docstring."""'))]),
-            cst.SimpleStatementLine(body=[cst.Pass()]),
-        ]
-    ),
-)
+        name=cst.Name("function_name"),
+        params=cst.Parameters(),
+        body=cst.IndentedBlock(
+            body=[
+                cst.SimpleStatementLine(
+                    body=[
+                        cst.Expr(value=cst.SimpleString('"""This is a docstring."""'))
+                    ]
+                ),
+                cst.SimpleStatementLine(body=[cst.Pass()]),
+            ]
+        ),
+    )
 
 
 @pytest.fixture
 def cst_class_def():
     return cst.ClassDef(
-    name=cst.Name("ClassName"),
-    body=cst.IndentedBlock(
-        body=[
-            cst.SimpleStatementLine(body=[cst.Expr(value=cst.SimpleString('"""This is a class docstring."""'))]),
-            cst.SimpleStatementLine(body=[cst.Pass()]),
-        ]
-    ),
-)
+        name=cst.Name("ClassName"),
+        body=cst.IndentedBlock(
+            body=[
+                cst.SimpleStatementLine(
+                    body=[
+                        cst.Expr(
+                            value=cst.SimpleString('"""This is a class docstring."""')
+                        )
+                    ]
+                ),
+                cst.SimpleStatementLine(body=[cst.Pass()]),
+            ]
+        ),
+    )
 
 
 def test_has_docstring_function_def(cst_function_def):
     assert has_docstring(cst_function_def)
 
 
 def test_has_docstring_class_def(cst_class_def):
```

### Comparing `write_the-0.7.7/tests/test_utils.py` & `write_the-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/tests/data/expected.dat` & `write_the-0.8.0/tests/data/expected.dat`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/write_the/llm.py` & `write_the-0.8.0/write_the/llm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.llms import OpenAI
+import tiktoken
+
 
 class LLM:
-    def __init__(self, prompt: PromptTemplate, temperature=0, max_tokens=-1, gpt_4=False):
+    def __init__(self, prompt: PromptTemplate, temperature=0, gpt_4=False):
         self.prompt = prompt
+        self.prompt_size = self.number_of_tokens(prompt.template)
         self.temperature = temperature
-        self.max_tokens = max_tokens
         self.gpt_4 = gpt_4
         self.model_name = "gpt-4" if self.gpt_4 else "text-davinci-003"
+        self.max_tokens = 4097 * 2 if self.gpt_4 else 4097
 
     async def run(self, code, **kwargs):
         llm = OpenAI(
-            temperature=self.temperature, 
-            max_tokens=self.max_tokens, 
-            model_name=self.model_name
+            temperature=self.temperature, max_tokens=-1, model_name=self.model_name
         )
         chain = LLMChain(llm=llm, prompt=self.prompt)
-        return await chain.apredict(code=code, **kwargs)
+        return await chain.apredict(code=code, **kwargs)
+
+    def number_of_tokens(self, text):
+        encoding = tiktoken.encoding_for_model("gpt-4")
+        return len(encoding.encode(text))
```

### Comparing `write_the-0.7.7/write_the/utils.py` & `write_the-0.8.0/write_the/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,15 @@
         python_files.append(file)
     return python_files
 
 
 def load_source_code(file: Path):
     with open(file, "r") as file:
         return file.read()
-    
+
+
 def format_source_code(source_code):
-  return format_str(source_code, mode=FileMode())
+    return format_str(source_code, mode=FileMode())
+
 
 def create_tree(source_code):
-    return cst.parse_module(source_code)
+    return cst.parse_module(source_code)
```

### Comparing `write_the-0.7.7/write_the/cli/main.py` & `write_the-0.8.0/write_the/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import List, Optional
 from black import InvalidInput
 from asyncio import run, gather
 from functools import wraps
 
 from .tasks import async_cli_task
 
+
 class AsyncTyper(typer.Typer):
     def async_command(self, *args, **kwargs):
         def decorator(async_func):
             @wraps(async_func)
             def sync_func(*_args, **_kwargs):
                 return run(async_func(*_args, **_kwargs))
 
@@ -25,24 +26,33 @@
             return async_func
 
         return decorator
 
 
 app = AsyncTyper()
 
+
 def _print_version(ctx: typer.Context, value: bool):
     if value:
         typer.echo(__version__)
         raise typer.Exit()
 
 
 @app.callback(context_settings={"help_option_names": ["-h", "--help"]})
 def callback(
-        version: Optional[bool] = typer.Option(None, '-v', '--version', help="Show the pipeline version.", is_eager=True, callback=_print_version, show_default=False)
-    ):
+    version: Optional[bool] = typer.Option(
+        None,
+        "-v",
+        "--version",
+        help="Show the pipeline version.",
+        is_eager=True,
+        callback=_print_version,
+        show_default=False,
+    )
+):
     """
     AI-powered Code Generation and Refactoring Tool
     """
 
 
 @app.async_command()
 async def docs(
@@ -50,24 +60,39 @@
     nodes: List[str] = typer.Option(
         None,
         "--node",
         "-n",
         help="Generate docs for specific nodes (functions and classes).",
     ),
     save: bool = typer.Option(
-        False, "--save/--print", "-s", help="Save the docstrings to file or print to stdout."
+        False,
+        "--save/--print",
+        "-s",
+        help="Save the docstrings to file or print to stdout.",
     ),
     pretty: bool = typer.Option(
         False, "--pretty/--plain", "-p", help="Syntax highlight and format the output."
     ),
     context: bool = typer.Option(
-        False, "--context/--no-context", "-c", help="Send context with nodes."
+        False,
+        "--context/--no-context",
+        "-c",
+        help="Send context (other nodes) with nodes.",
+    ),
+    background: bool = typer.Option(
+        True,
+        "--background/--no-background",
+        "-g",
+        help="Send background (other code) with nodes.",
     ),
     force: bool = typer.Option(
-        False, "--force/--no-force", "-f", help="Generate docstings even if they already exist."
+        False,
+        "--force/--no-force",
+        "-f",
+        help="Generate docstings even if they already exist.",
     ),
     batch: bool = typer.Option(
         False, "--batch/--no-batch", "-b", help="Send each node as a separate request."
     ),
 ):
     """
     Document your code with AI.
@@ -80,96 +105,116 @@
     with Progress(
         SpinnerColumn(),
         TextColumn("{task.description}"),
         transient=True,
         auto_refresh=True,
     ) as progress:
         tasks = []
-        print_status=len(files)>1
+        print_status = len(files) > 1
         for file in files:
             tasks.append(
                 async_cli_task(
                     file,
-                    nodes=nodes, 
-                    force=force, 
-                    save=save, 
-                    context=context, 
+                    nodes=nodes,
+                    force=force,
+                    save=save,
+                    context=context,
+                    background=background,
                     pretty=pretty,
                     batch=batch,
                     print_status=print_status,
-                    progress=progress
+                    progress=progress,
                 )
             )
         await gather(*tasks)
 
+
 @app.command()
 def mkdocs(
     code_dir: Path = typer.Argument(
         ...,
         help="Path to the projects code. Uses docstings to build API reference.",
         file_okay=False,
     ),
     readme: Optional[Path] = typer.Option(
         None, help="Path to projects README (used to create index.md).", dir_okay=False
     ),
     out_dir: Path = typer.Option(
-        Path('.'), "--out", "-o", help="Path to save output (docs/ and yaml). Defaults to current directory."
+        Path("."),
+        "--out",
+        "-o",
+        help="Path to save output (docs/ and yaml). Defaults to current directory.",
     ),
 ):
     """
     Generate a mkdocs website for a project including the API reference.
     """
     write_the_mkdocs(code_dir=code_dir, readme=readme, out_dir=out_dir)
 
 
 @app.async_command()
 async def tests(
     file: Path = typer.Argument(..., help="Path to the code file/folder."),
     tests_dir: Path = typer.Option(
-        'tests', "--out", "-o", help="Path to save the docs."
+        "tests", "--out", "-o", help="Path to save the docs."
     ),
     save: bool = typer.Option(
-        False, "--save/--print", "-s", help="Save the tests to the tests directory or print to stdout."
+        False,
+        "--save/--print",
+        "-s",
+        help="Save the tests to the tests directory or print to stdout.",
     ),
-       pretty: bool = typer.Option(
+    pretty: bool = typer.Option(
         False, "--pretty/--plain", "-p", help="Syntax highlight the output."
     ),
     group: bool = typer.Option(
-        False, "--group/--flat", "-g", help="Group the tests into folder or keep them flat."
+        False,
+        "--group/--flat",
+        "-g",
+        help="Group the tests into folder or keep them flat.",
     ),
     force: bool = typer.Option(
         False, "--force", "-f", help="Generate tests even if they already exist."
     ),
     empty: bool = typer.Option(
-        False, "--empty", "-e", help="Save empty files if a test creation fails. This will prevent write-the from regenerating failed test creations."
+        False,
+        "--empty",
+        "-e",
+        help="Save empty files if a test creation fails. This will prevent write-the from regenerating failed test creations.",
     ),
     gpt_4: bool = typer.Option(
-        False, "--gpt-4", help="Use GPT-4 to generate the tests (requires API will access)."
+        False,
+        "--gpt-4",
+        help="Use GPT-4 to generate the tests (requires API will access).",
     ),
 ):
     """
-    Generate tests for your code. 
+    Generate tests for your code.
     """
     current_tests = list_python_files(tests_dir)
     if file.is_dir():
         files = list_python_files(file)
     else:
         assert file.suffix == ".py"
         files = [file]
     for file in files:
-        if file.stem.startswith('_'):
+        if file.stem.startswith("_"):
             continue
         parts = list(file.parts[1:-1])
-        parts = ['test'] + parts
+        parts = ["test"] + parts
         test_file = f"{'_'.join(parts)}_{file.stem}.py"
         if group:
             parts.append(test_file)
             test_file = Path(os.path.join(*parts))
         test_file_path = tests_dir / test_file
-        if test_file_path.exists() and (not force and save) or (test_file in current_tests):
+        if (
+            test_file_path.exists()
+            and (not force and save)
+            or (test_file in current_tests)
+        ):
             continue
         with Progress(
             SpinnerColumn(),
             TextColumn("[progress.description]{task.description}"),
             transient=True,
         ) as progress:
             failed = False
@@ -194,15 +239,20 @@
                     f.writelines(result)
             elif pretty:
                 syntax = Syntax(result, "python")
                 console = Console()
                 console.print(syntax)
             else:
                 typer.echo(result)
-            
+
+
+@app.command()
+def models():
+    raise NotImplementedError()
+
 
 @app.command()
 def refactor():
     raise NotImplementedError()
 
 
 @app.command()
```

### Comparing `write_the-0.7.7/write_the/cli/tasks.py` & `write_the-0.8.0/write_the/cli/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from write_the.commands import write_the_docs
 from write_the.utils import create_tree, format_source_code, load_source_code
 from rich.syntax import Syntax
 from rich.progress import Progress
 from typing import List
 from pathlib import Path
+from openai.error import InvalidRequestError
 
 
 async def async_cli_task(
     file: Path,
     nodes: List,
     force: bool,
     save: bool,
     context: bool,
+    background: bool,
     pretty: bool,
     batch: bool,
     print_status: bool,
     progress: Progress,
 ) -> None:
     """
     Executes a task asynchronously.
@@ -41,34 +43,42 @@
     """
     task_id = progress.add_task(description=f"{file}", total=None)
     failed = False
     source_code = load_source_code(file=file)
     if pretty:
         source_code = format_source_code(source_code)
     tree = create_tree(source_code)
+    max_batch_size = None
+    msg = ""
+    if batch:
+        max_batch_size = 1
     try:
         result = await write_the_docs(
             tree,
-            nodes=nodes,
+            node_names=nodes,
             force=force,
             save=save,
             context=context,
+            background=background,
             pretty=pretty,
-            batch=batch,
+            max_batch_size=max_batch_size,
         )
-    except Exception as e:
-        print(e)
+    except ValueError as e:
+        msg = f" - {e}"
+        failed = True
+    except InvalidRequestError as e:
+        msg = f" - {e}"
         failed = True
     progress.remove_task(task_id)
     progress.refresh()
     if print_status or save or failed:
         icon = "❌" if failed else "✅"
         colour = "red" if failed else "green"
         progress.print(
-            f"[not underline]{icon} [/not underline]{file}",
+            f"[not underline]{icon} [/not underline]{file}{msg}",
             style=f"bold {colour} underline",
         )
     if failed:
         return None
     if save:
         with open(file, "w") as f:
             f.writelines(result)
```

### Comparing `write_the-0.7.7/write_the/commands/docs/docs.py` & `write_the-0.8.0/write_the/commands/docs/docs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,41 @@
+import asyncio
 import libcst as cst
 from black import format_str, FileMode
 
 from write_the.cst import nodes_to_tree
 from write_the.cst.docstring_adder import add_docstrings_to_tree
-from write_the.cst.docstring_remover import remove_docstrings
 from write_the.cst.function_and_class_collector import get_node_names
 from write_the.cst.node_extractor import extract_nodes_from_tree
-from write_the.commands.docs.utils import extract_block, process_nodes
+from write_the.cst.node_batcher import create_batches
+from write_the.commands.docs.utils import extract_block
 from write_the.llm import LLM
 from .prompts import write_docstings_for_nodes_prompt
 
 
 async def write_the_docs(
     tree: cst.Module,
-    nodes=[],
+    node_names=[],
     force=False,
     save=False,
-    context=True,
+    context=False,
+    background=True,
     pretty=False,
-    batch=False,
+    max_batch_size=False,
 ) -> str:
     """
     Generates docstrings for a given tree of nodes.
     Args:
       tree (cst.Module): The tree of nodes to write docs for.
-      nodes (list): The list of nodes to write docs for.
+      node_names (list): The list of nodes names to write docs for.
       force (bool): Whether to force writing of docs.
       save (bool): Whether to save the docs.
       context (bool): Whether to include context nodes.
       pretty (bool): Whether to format the code.
-      batch (bool): Whether to run in batch mode.
+      max_batch_size (bool): Max number of nodes in each batch.
     Returns:
       str: The source code with the generated docstrings.
     Notes:
       If `nodes` is provided, `force` is set to `True` and `context` is set to `False`.
     Examples:
       >>> write_the_docs("example.py")
       "def add(a, b):
@@ -43,26 +45,45 @@
               b (int): The second number to add.
           Returns:
               int: The sum of `a` and `b`.
           \"\"\"
           return a + b"
     """
     extract_specific_nodes = False
-    if nodes:
+    if node_names:
         extract_specific_nodes = True
         force = True
     else:
-        nodes = get_node_names(tree, force)
-    if not nodes:
+        node_names = get_node_names(tree, force)
+    if not node_names:
         return tree.code
-    tree_without_docstrings = remove_docstrings(tree, nodes)
-    code = process_nodes(tree_without_docstrings, nodes, context, extract_specific_nodes)
+    # batch
     llm = LLM(write_docstings_for_nodes_prompt)
-    result = await llm.run(code=code, nodes=nodes)
-    docstring_dict = extract_block(result, nodes)
+    batches = create_batches(
+        tree=tree,
+        node_names=node_names,
+        max_tokens=llm.max_tokens,
+        prompt_size=llm.prompt_size,
+        response_size_per_node=250,  # a guess... TODO: smarter
+        max_batch_size=max_batch_size,
+        send_background_context=background,
+        send_node_context=context,
+    )
+    promises = []
+    node_names_list = []
+    for batch in batches:
+        node_names = batch.node_names
+        code = batch.code
+        promises.append((llm.run(code=code, nodes=node_names)))
+        node_names_list.append(node_names)
+    # Can i yield here so batches can be logged?
+    results = await asyncio.gather(*promises)
+    docstring_dict = {}
+    for node_names, result in zip(node_names_list, results):
+        docstring_dict.update(extract_block(result, node_names))
     modified_tree = add_docstrings_to_tree(tree, docstring_dict, force=force)
     if not save and extract_specific_nodes:
-        extracted_nodes = extract_nodes_from_tree(modified_tree, nodes)
+        extracted_nodes = extract_nodes_from_tree(modified_tree, node_names)
         modified_tree = nodes_to_tree(extracted_nodes)
     if pretty:
         return format_str(modified_tree.code, mode=FileMode())
     return modified_tree.code
```

### Comparing `write_the-0.7.7/write_the/commands/docs/utils.py` & `write_the-0.8.0/write_the/commands/docs/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import libcst as cst
-import re 
+import re
 
 from write_the.cst import nodes_to_tree
 from write_the.cst.function_and_class_collector import get_node_names
 from write_the.cst.node_extractor import extract_nodes_from_tree
 from write_the.cst.node_remover import remove_nodes_from_tree
 
+
 def pad_with_newline_if_needed(s):
-    if not s.startswith('\n'):
-        s = '\n' + s
-    if not s.endswith('\n'):
-        s = s + '\n'
+    if not s.startswith("\n"):
+        s = "\n" + s
+    if not s.endswith("\n"):
+        s = s + "\n"
     return s
 
+
 def extract_block(text, class_function_names):
     results = {}
     for name in class_function_names:
-        pattern = rf'({name}:[\s\S]*?)(?=(\n\w|\Z))'
+        pattern = rf"({name}:[\s\S]*?)(?=(\n\w|\Z))"
         match = re.search(pattern, text)
         if match:
             block = match.group(1).lstrip(f"{name}:")
             results[name] = pad_with_newline_if_needed(block)
     return results
 
 
@@ -39,18 +41,15 @@
       "Processed tree as a string"
     """
     if not context:
         if extract_specific_nodes:
             extracted_nodes = extract_nodes_from_tree(tree, nodes)
             processed_tree = nodes_to_tree(extracted_nodes)
         else:
-            all_nodes = get_node_names(tree, False)
+            all_nodes = get_node_names(tree, True)
             nodes_to_remove = [n for n in all_nodes if n not in nodes]
-            processed_tree = remove_nodes_from_tree(
-                tree, nodes_to_remove
-            )
+            processed_tree = remove_nodes_from_tree(tree, nodes_to_remove)
         code = processed_tree.code
     else:
         code = tree.code
 
     return code
-
```

### Comparing `write_the-0.7.7/write_the/commands/mkdocs/mkdocs.py` & `write_the-0.8.0/write_the/commands/mkdocs/mkdocs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from pathlib import Path
 from collections import defaultdict
 from write_the.utils import list_python_files
 
 from .templates import action_template, mkdocs_template
 
-def write_the_mkdocs(code_dir: Path, readme: Path = None, out_dir: Path = Path('.'), project_name=None):
+
+def write_the_mkdocs(
+    code_dir: Path, readme: Path = None, out_dir: Path = Path("."), project_name=None
+):
     """
     Generates a mkdocs project from a directory of python files.
     Args:
       code_dir (Path): The directory containing the python files.
       readme (Path, optional): The readme file to include in the project. Defaults to None.
       out_dir (Path, optional): The directory to write the project to. Defaults to the current directory.
       project_name (str, optional): The name of the project. Defaults to the name of the code_dir.
@@ -29,20 +32,22 @@
     mkdocs = mkdocs_template.format(project_name=project_name)
     references = defaultdict(list)
     for file in files:
         if file.name.startswith("_"):
             continue
         key = "index"
         for group in groups:
-            if f"{code_dir.name}/{group}/" in str(file) or f"{code_dir.name}/{group}." in str(file):
+            if f"{code_dir.name}/{group}/" in str(
+                file
+            ) or f"{code_dir.name}/{group}." in str(file):
                 key = group
                 break
         module = str(file).rstrip(".py").replace("/", ".")  # breaks on windows?
         references[key].append(f"::: {module}")
-    docs_dir = out_dir / 'docs'
+    docs_dir = out_dir / "docs"
     reference_path = docs_dir / "reference"
     reference_path.mkdir(parents=True, exist_ok=True)
     for doc in references:
         with open(f"{reference_path}/{doc}.md", "w") as f:
             for ref in references[doc]:
                 f.write(ref + "\n\n")
     if readme:
```

### Comparing `write_the-0.7.7/write_the/commands/mkdocs/templates.py` & `write_the-0.8.0/write_the/commands/mkdocs/templates.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,8 @@
           python-version: 3.x
       - uses: actions/cache@v2
         with:
           key: ${{ github.ref }}
           path: .cache
       - run: pip install "mkdocstrings[python]" "mkdocs-material"
       - run: mkdocs gh-deploy --force
-"""
+"""
```

### Comparing `write_the-0.7.7/write_the/commands/tests/tests.py` & `write_the-0.8.0/write_the/commands/tests/tests.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from pathlib import Path
 from black import format_str, FileMode
 from .prompts import write_tests_for_file_prompt
 from write_the.llm import LLM
 
-async def write_the_tests(
-    filename: Path,
-    gpt_4: bool = False
-) -> str:
+
+async def write_the_tests(filename: Path, gpt_4: bool = False) -> str:
     """
     Formats and runs the tests for a given file.
     Args:
       filename (Path): The path to the file to be tested.
       gpt_4 (bool, optional): Whether to use GPT-4 for testing. Defaults to False.
     Returns:
       str: The formatted and tested code.
@@ -19,9 +17,15 @@
       "Formatted and tested code"
     """
     with open(filename, "r") as file:
         source_code = file.read()
     source_code = format_str(source_code, mode=FileMode())
     llm = LLM(write_tests_for_file_prompt, gpt_4=gpt_4)
     result = await llm.run(code=source_code, path=filename)
-    code = result.strip().lstrip("Test Code:\n```python").lstrip("```python").lstrip("```").rstrip("```")
+    code = (
+        result.strip()
+        .lstrip("Test Code:\n```python")
+        .lstrip("```python")
+        .lstrip("```")
+        .rstrip("```")
+    )
     return format_str(code, mode=FileMode())
```

### Comparing `write_the-0.7.7/write_the/cst/docstring_adder.py` & `write_the-0.8.0/write_the/cst/docstring_adder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import libcst as cst
 from .utils import has_docstring, remove_docstring
 import textwrap
 import re
 
+
 class DocstringAdder(cst.CSTTransformer):
     def __init__(self, docstrings, force):
         self.docstrings = docstrings
-        self.current_class = None
         self.force = force
+        self.current_class = None
 
     def leave_FunctionDef(
         self, original_node: cst.FunctionDef, updated_node: cst.FunctionDef
     ) -> cst.FunctionDef:
         """
         Adds a docstring to a function definition.
         Args:
           original_node (cst.FunctionDef): The original CST node.
           updated_node (cst.FunctionDef): The updated CST node.
         Returns:
           cst.FunctionDef: The updated CST node with a docstring added.
         """
         return self.add_docstring(updated_node)
 
-    def visit_ClassDef(
-            self, original_node: cst.ClassDef
-    ) -> None:
+    def visit_ClassDef(self, original_node: cst.ClassDef) -> None:
         self.current_class = original_node.name.value
 
     def leave_ClassDef(
         self, original_node: cst.ClassDef, updated_node: cst.ClassDef
     ) -> cst.ClassDef:
         """
         Adds a docstring to a class definition.
@@ -55,19 +54,20 @@
             if self.current_class
             else node.name.value
         )
         docstring: str = self.docstrings.get(key, None)
         if docstring and (self.force or not has_docstring(node)):
             if self.force and has_docstring(node):
                 # Remove existing docstring
-                node = remove_docstring(node)            
-            escaped_docstring = re.sub(r'(?<!\\)\\n', '\\\\\\\\n', docstring) 
+                node = remove_docstring(node)
+            escaped_docstring = re.sub(r"(?<!\\)\\n", "\\\\\\\\n", docstring)
             dedented_docstring = textwrap.dedent(escaped_docstring)
-            indented_docstring = textwrap.indent(dedented_docstring, '    ')
+            indented_docstring = textwrap.indent(dedented_docstring, "    ")
             new_docstring = cst.parse_statement(f'"""{indented_docstring}    """')
             body = node.body.with_changes(body=[new_docstring] + list(node.body.body))
             return node.with_changes(body=body)
-        
+
         return node
 
+
 def add_docstrings_to_tree(tree, docstring_dict, force=False):
-    return tree.visit(DocstringAdder(docstring_dict, force))
+    return tree.visit(DocstringAdder(docstring_dict, force))
```

### Comparing `write_the-0.7.7/write_the/cst/function_and_class_collector.py` & `write_the-0.8.0/write_the/cst/function_and_class_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         """
         Initializes the FunctionAndClassCollector.
         Args:
           force (bool): Whether to force the collection of functions and classes even if they have docstrings.
         """
         self.functions = []
         self.classes = []
-        self.current_class = None
         self.force = force
+        self.current_class = None
 
     def visit_FunctionDef(self, node: cst.FunctionDef) -> None:
         """
         Visits a FunctionDef node and adds it to the list of functions if it does not have a docstring or if `force` is `True`.
         Args:
           node (cst.FunctionDef): The FunctionDef node to visit.
         """
@@ -50,8 +50,8 @@
       tree (cst.CSTNode): The CST tree to traverse.
       force (bool): Whether to force the collection of functions and classes even if they have docstrings.
     Returns:
       list[str]: A list of function and class names.
     """
     collector = FunctionAndClassCollector(force)
     tree.visit(collector)
-    return collector.functions + collector.classes
+    return collector.classes + collector.functions
```

### Comparing `write_the-0.7.7/write_the/cst/node_extractor.py` & `write_the-0.8.0/write_the/cst/node_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,48 @@
+from typing import Optional
 import libcst as cst
 
 
 class NodeExtractor(cst.CSTVisitor):
     def __init__(self, nodes):
         self.nodes = nodes
         self.extracted_nodes = []
+        self.current_class = None
 
     def visit_FunctionDef(self, node: cst.FunctionDef):
         """
         Visits a FunctionDef node and adds it to the extracted_nodes list if it is in the nodes list.
         Args:
           node (cst.FunctionDef): The FunctionDef node to visit.
         Side Effects:
           Adds the node to the extracted_nodes list if it is in the nodes list.
         """
-        if node.name.value in self.nodes:
+        name = (
+            f"{self.current_class}.{node.name.value}"
+            if self.current_class
+            else node.name.value
+        )
+        if name in self.nodes:
             self.extracted_nodes.append(node)
 
     def visit_ClassDef(self, node: cst.ClassDef):
         """
         Visits a ClassDef node and adds it to the extracted_nodes list if it is in the nodes list.
         Args:
           node (cst.ClassDef): The ClassDef node to visit.
         Side Effects:
           Adds the node to the extracted_nodes list if it is in the nodes list.
         """
+        self.current_class = node.name.value
         if node.name.value in self.nodes:
             self.extracted_nodes.append(node)
 
+    def leave_ClassDef(self, node: cst.ClassDef) -> None:
+        self.current_class = None
+
 
 def extract_nodes_from_tree(tree, nodes):
     """
     Extracts nodes from a CST tree.
     Args:
       tree (cst.CSTNode): The CST tree to extract nodes from.
       nodes (list): A list of nodes to extract.
@@ -40,7 +51,15 @@
     Examples:
       >>> extract_nodes_from_tree(tree, nodes)
       [cst.FunctionDef, cst.ClassDef]
     """
     extractor = NodeExtractor(nodes)
     tree.visit(extractor)
     return extractor.extracted_nodes
+
+
+def extract_node_from_tree(tree, node) -> Optional[cst.CSTNode]:
+    extractor = NodeExtractor([node])
+    tree.visit(extractor)
+    if not extractor.extracted_nodes:
+        raise ValueError(f"Could not find node: {node}!")
+    return extractor.extracted_nodes[0]
```

### Comparing `write_the-0.7.7/write_the/cst/node_remover.py` & `write_the-0.8.0/write_the/cst/node_remover.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,43 +5,54 @@
     def __init__(self, nodes):
         """
         Initializes a NodeRemover instance.
         Args:
           nodes (list): A list of nodes to remove.
         """
         self.nodes = nodes
+        self.current_class = None
 
     def leave_FunctionDef(
         self, original_node: cst.FunctionDef, updated_node: cst.FunctionDef
     ) -> cst.RemovalSentinel:
         """
         Removes a FunctionDef node from the tree if it is in the list of nodes.
         Args:
           original_node (cst.FunctionDef): The original FunctionDef node.
           updated_node (cst.FunctionDef): The updated FunctionDef node.
         Returns:
           cst.RemovalSentinel: A sentinel indicating whether the node should be removed.
         """
-        if original_node.name.value in self.nodes:
+        name = (
+            f"{self.current_class}.{original_node.name.value}"
+            if self.current_class
+            else original_node.name.value
+        )
+        if name in self.nodes:
             return cst.RemoveFromParent()
         return updated_node
 
+    def visit_ClassDef(self, original_node: cst.ClassDef) -> None:
+        self.current_class = original_node.name.value
+
     def leave_ClassDef(
         self, original_node: cst.ClassDef, updated_node: cst.ClassDef
     ) -> cst.RemovalSentinel:
         """
         Removes a ClassDef node from the tree if it is in the list of nodes.
         Args:
           original_node (cst.ClassDef): The original ClassDef node.
           updated_node (cst.ClassDef): The updated ClassDef node.
         Returns:
           cst.RemovalSentinel: A sentinel indicating whether the node should be removed.
         """
+        self.current_class = None
         if original_node.name.value in self.nodes:
             return cst.RemoveFromParent()
+
         return updated_node
 
 
 def remove_nodes_from_tree(tree, nodes):
     """
     Removes nodes from a CST tree.
     Args:
```

### Comparing `write_the-0.7.7/write_the/cst/utils.py` & `write_the-0.8.0/write_the/cst/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import libcst as cst
 from typing import Optional
 
+
 def has_docstring(node: cst.CSTNode) -> bool:
     """
     Checks if a CSTNode has a docstring.
     Args:
       node (cst.CSTNode): The node to check.
     Returns:
       bool: Whether or not the node has a docstring.
@@ -15,14 +16,15 @@
         body = node.body.body
         if body and isinstance(body[0], cst.SimpleStatementLine):
             stmt = body[0].body[0]
             if isinstance(stmt, cst.Expr) and isinstance(stmt.value, cst.SimpleString):
                 return True
     return False
 
+
 def remove_docstring(node):
     """
     Removes the docstring from a node.
     Args:
       node (cst.CSTNode): The node to remove the docstring from.
     Returns:
       cst.CSTNode: The node with the docstring removed.
@@ -33,14 +35,15 @@
     if isinstance(first_stmt, cst.SimpleStatementLine):
         stmt = first_stmt.body[0]
         if isinstance(stmt, cst.Expr) and isinstance(stmt.value, cst.SimpleString):
             new_body = node.body.with_changes(body=node.body.body[1:])
             return node.with_changes(body=new_body)
     return node
 
+
 def get_docstring(node: cst.CSTNode) -> Optional[str]:
     """
     Retrieves the docstring of a CSTNode if it has one.
     Args:
         node (cst.CSTNode): The node to check.
     Returns:
         Optional[str]: The docstring of the node if it exists, None otherwise.
@@ -49,17 +52,22 @@
     """
     if has_docstring(node):
         body = node.body.body
         stmt = body[0].body[0]
         return stmt.value.value
     return None
 
+
 def nodes_to_tree(nodes):
     """
     Converts a list of CSTNodes into a CSTModule.
     Args:
       nodes (list[cst.CSTNode]): The list of nodes to convert.
     Returns:
       cst.Module: The CSTModule containing the given nodes.
     """
     module = cst.Module(body=nodes)
     return module
+
+
+def get_code_from_node(node: cst.CSTNode):
+    return cst.Module(body=[node]).code
```

### Comparing `write_the-0.7.7/LICENSE.txt` & `write_the-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/README.md` & `write_the-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/pyproject.toml` & `write_the-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.7/PKG-INFO` & `write_the-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.7.7
+Version: 0.8.0
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

