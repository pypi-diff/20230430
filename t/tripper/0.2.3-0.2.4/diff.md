# Comparing `tmp/tripper-0.2.3.tar.gz` & `tmp/tripper-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tripper-0.2.3.tar", last modified: Sun Feb  5 16:13:09 2023, max compression
+gzip compressed data, was "tripper-0.2.4.tar", last modified: Sun Apr 30 20:08:04 2023, max compression
```

## Comparing `tripper-0.2.3.tar` & `tripper-0.2.4.tar`

### file list

```diff
@@ -1,61 +1,71 @@
--rw-r--r--   0        0        0      205 2023-02-05 16:12:19.986171 tripper-0.2.3/.github/dependabot.yml
--rw-r--r--   0        0        0      637 2023-02-05 16:12:19.986171 tripper-0.2.3/.github/pull_request_template.md
--rw-r--r--   0        0        0      916 2023-02-05 16:12:19.986171 tripper-0.2.3/.github/workflows/cd_release.yml
--rw-r--r--   0        0        0      545 2023-02-05 16:12:19.986171 tripper-0.2.3/.github/workflows/ci_automerge_dependency_prs.yml
--rw-r--r--   0        0        0      656 2023-02-05 16:12:19.986171 tripper-0.2.3/.github/workflows/ci_cd_updated_main.yml
--rw-r--r--   0        0        0      602 2023-02-05 16:12:19.986171 tripper-0.2.3/.github/workflows/ci_check_dependencies.yml
--rw-r--r--   0        0        0     3297 2023-02-05 16:12:19.986171 tripper-0.2.3/.github/workflows/ci_tests.yml
--rw-r--r--   0        0        0      838 2023-02-05 16:12:19.986171 tripper-0.2.3/.github/workflows/ci_update_dependencies.yml
--rw-r--r--   0        0        0      137 2023-02-05 16:12:19.986171 tripper-0.2.3/.gitignore
--rw-r--r--   0        0        0     1819 2023-02-05 16:12:19.986171 tripper-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8369 2023-02-05 16:13:07.049901 tripper-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-02-05 16:12:19.990171 tripper-0.2.3/LICENSE
--rw-r--r--   0        0        0     2460 2023-02-05 16:12:19.990171 tripper-0.2.3/README.md
-lrwxr-xr-x   0        0        0        0 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/CHANGELOG.md -> ../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/LICENSE.md -> ../LICENSE
--rw-r--r--   0        0        0       23 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/.pages
--rw-r--r--   0        0        0       18 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/backends/.pages
--rw-r--r--   0        0        0       46 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/backends/collection.md
--rw-r--r--   0        0        0       38 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/backends/ontopy.md
--rw-r--r--   0        0        0       38 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/backends/rdflib.md
--rw-r--r--   0        0        0       52 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/backends/sparqlwrapper.md
--rw-r--r--   0        0        0       29 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/errors.md
--rw-r--r--   0        0        0       35 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/interface.md
--rw-r--r--   0        0        0       31 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/literal.md
--rw-r--r--   0        0        0       18 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/mappings/.pages
--rw-r--r--   0        0        0       42 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/mappings/mappings.md
--rw-r--r--   0        0        0       35 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/namespace.md
--rw-r--r--   0        0        0       39 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/triplestore.md
--rw-r--r--   0        0        0       27 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/api_reference/utils.md
--rw-r--r--   0        0        0      183 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/css/reference.css
--rw-r--r--   0        0        0     2458 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/index.md
--rw-r--r--   0        0        0    12710 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/mappings/figs/function_emmo.svg
--rw-r--r--   0        0        0      311 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/planned-backends.md
--rw-r--r--   0        0        0     3775 2023-02-05 16:12:19.990171 tripper-0.2.3/docs/tutorial.md
--rw-r--r--   0        0        0     1943 2023-02-05 16:12:19.990171 tripper-0.2.3/mkdocs.yml
--rw-r--r--   0        0        0     2805 2023-02-05 16:12:19.990171 tripper-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3444 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     1455 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/mappings/test_mappings.py
--rw-r--r--   0        0        0     5701 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/ontologies/family.ttl
--rw-r--r--   0        0        0     6753 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/ontologies/food.ttl
--rw-r--r--   0        0        0     3166 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/test_add_function.py
--rw-r--r--   0        0        0      959 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/test_collection.py
--rw-r--r--   0        0        0     3943 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/test_literals.py
--rw-r--r--   0        0        0     1993 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/test_namespace.py
--rw-r--r--   0        0        0     7576 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/test_triplestore.py
--rw-r--r--   0        0        0     5665 2023-02-05 16:12:19.990171 tripper-0.2.3/tests/test_utils.py
--rw-r--r--   0        0        0      663 2023-02-05 16:13:07.577898 tripper-0.2.3/tripper/__init__.py
--rw-r--r--   0        0        0     1330 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/backends/__init__.py
--rw-r--r--   0        0        0     2482 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/backends/collection.py
--rw-r--r--   0        0        0     9100 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/backends/ontopy.py
--rw-r--r--   0        0        0     7249 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/backends/rdflib.py
--rw-r--r--   0        0        0     4112 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/backends/sparqlwrapper.py
--rw-r--r--   0        0        0      362 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/errors.py
--rw-r--r--   0        0        0     5379 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/interface.py
--rw-r--r--   0        0        0     5509 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/literal.py
--rw-r--r--   0        0        0      102 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/mappings/__init__.py
--rw-r--r--   0        0        0    32048 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/mappings/mappings.py
--rw-r--r--   0        0        0     6901 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/namespace.py
--rw-r--r--   0        0        0    29200 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/triplestore.py
--rw-r--r--   0        0        0     7244 2023-02-05 16:12:19.990171 tripper-0.2.3/tripper/utils.py
--rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 tripper-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      205 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      637 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/pull_request_template.md
+-rw-r--r--   0        0        0      916 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/cd_release.yml
+-rw-r--r--   0        0        0      545 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_automerge_dependency_prs.yml
+-rw-r--r--   0        0        0      656 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_cd_updated_main.yml
+-rw-r--r--   0        0        0      602 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_check_dependencies.yml
+-rw-r--r--   0        0        0     2420 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_tests.yml
+-rw-r--r--   0        0        0      838 2023-04-30 20:07:11.412130 tripper-0.2.4/.github/workflows/ci_update_dependencies.yml
+-rw-r--r--   0        0        0      137 2023-04-30 20:07:11.412130 tripper-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1819 2023-04-30 20:07:11.412130 tripper-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       42 2023-04-30 20:07:11.412130 tripper-0.2.4/.pylintrc
+-rw-r--r--   0        0        0     9917 2023-04-30 20:08:01.428129 tripper-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-04-30 20:07:11.412130 tripper-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2496 2023-04-30 20:07:11.412130 tripper-0.2.4/README.md
+lrwxr-xr-x   0        0        0        0 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/CHANGELOG.md -> ../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/LICENSE.md -> ../LICENSE
+-rw-r--r--   0        0        0       23 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/.pages
+-rw-r--r--   0        0        0       18 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/.pages
+-rw-r--r--   0        0        0       46 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/collection.md
+-rw-r--r--   0        0        0       38 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/ontopy.md
+-rw-r--r--   0        0        0       38 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/rdflib.md
+-rw-r--r--   0        0        0       52 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/backends/sparqlwrapper.md
+-rw-r--r--   0        0        0       29 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/errors.md
+-rw-r--r--   0        0        0       35 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/interface.md
+-rw-r--r--   0        0        0       31 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/literal.md
+-rw-r--r--   0        0        0       18 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/mappings/.pages
+-rw-r--r--   0        0        0       42 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/mappings/mappings.md
+-rw-r--r--   0        0        0       35 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/namespace.md
+-rw-r--r--   0        0        0       39 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/triplestore.md
+-rw-r--r--   0        0        0       27 2023-04-30 20:07:11.412130 tripper-0.2.4/docs/api_reference/utils.md
+-rw-r--r--   0        0        0     2909 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/backend_discovery.md
+-rw-r--r--   0        0        0      183 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/css/reference.css
+-rw-r--r--   0        0        0     2489 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/index.md
+-rw-r--r--   0        0        0    12710 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/mappings/figs/function_emmo.svg
+-rw-r--r--   0        0        0      228 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/planned-backends.md
+-rw-r--r--   0        0        0     3963 2023-04-30 20:07:11.416130 tripper-0.2.4/docs/tutorial.md
+-rw-r--r--   0        0        0     1188 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/README.md
+-rw-r--r--   0        0        0    18333 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/knowledge-base.svg
+-rw-r--r--   0        0        0     8546 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/route.svg
+-rw-r--r--   0        0        0     7117 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/workflow.svg
+-rw-r--r--   0        0        0      894 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/workflow_mappings.py
+-rw-r--r--   0        0        0    14169 2023-04-30 20:07:11.416130 tripper-0.2.4/examples/workflow-mappings/workflow_w_pipes.svg
+-rw-r--r--   0        0        0     1943 2023-04-30 20:07:11.416130 tripper-0.2.4/mkdocs.yml
+-rw-r--r--   0        0        0     2713 2023-04-30 20:07:11.416130 tripper-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3444 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0      959 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/mappings/test_function.py
+-rw-r--r--   0        0        0     1455 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/mappings/test_mappings.py
+-rw-r--r--   0        0        0     5701 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/ontologies/family.ttl
+-rw-r--r--   0        0        0     6753 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/ontologies/food.ttl
+-rw-r--r--   0        0        0     3166 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_add_function.py
+-rw-r--r--   0        0        0      880 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_collection.py
+-rw-r--r--   0        0        0     2451 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_get_data.py
+-rw-r--r--   0        0        0     3943 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_literals.py
+-rw-r--r--   0        0        0     1993 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_namespace.py
+-rw-r--r--   0        0        0     7802 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_triplestore.py
+-rw-r--r--   0        0        0     6062 2023-04-30 20:07:11.416130 tripper-0.2.4/tests/test_utils.py
+-rw-r--r--   0        0        0      705 2023-04-30 20:08:01.744129 tripper-0.2.4/tripper/__init__.py
+-rw-r--r--   0        0        0     1330 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/collection.py
+-rw-r--r--   0        0        0     9100 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/ontopy.py
+-rw-r--r--   0        0        0     7363 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/rdflib.py
+-rw-r--r--   0        0        0     4112 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/backends/sparqlwrapper.py
+-rw-r--r--   0        0        0      362 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/errors.py
+-rw-r--r--   0        0        0     5379 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/interface.py
+-rw-r--r--   0        0        0     5510 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/literal.py
+-rw-r--r--   0        0        0      102 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/mappings/__init__.py
+-rw-r--r--   0        0        0    35281 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/mappings/mappings.py
+-rw-r--r--   0        0        0     6901 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/namespace.py
+-rw-r--r--   0        0        0    43718 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/triplestore.py
+-rw-r--r--   0        0        0     8237 2023-04-30 20:07:11.416130 tripper-0.2.4/tripper/utils.py
+-rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 tripper-0.2.4/PKG-INFO
```

### Comparing `tripper-0.2.3/.github/pull_request_template.md` & `tripper-0.2.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/.github/workflows/cd_release.yml` & `tripper-0.2.4/.github/workflows/cd_release.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/.github/workflows/ci_automerge_dependency_prs.yml` & `tripper-0.2.4/.github/workflows/ci_automerge_dependency_prs.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/.github/workflows/ci_cd_updated_main.yml` & `tripper-0.2.4/.github/workflows/ci_cd_updated_main.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/.github/workflows/ci_check_dependencies.yml` & `tripper-0.2.4/.github/workflows/ci_check_dependencies.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/.github/workflows/ci_tests.yml` & `tripper-0.2.4/.github/workflows/ci_tests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -53,62 +53,35 @@
 
   pytest:
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        # -- Uncomment when tripper this version of tripper has been released
-        #    such that we can import tripper with Python 3.11
-        # python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
         python-version: ["3.7", "3.8", "3.9", "3.10"]
 
     steps:
     - name: Checkout tripper
       uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
+        sudo apt install graphviz
         python -m pip install -U pip
         pip install -U setuptools wheel flit
         pip install -e .[testing]
 
     - name: Test with pytest
-      run: pytest -vvv --cov-report=xml
+      run: pytest -vvv --cov-report=xml --doctest-modules
 
     - name: Upload coverage to Codecov
       if: matrix.python-version == '3.9' && github.repository == 'EMMC-ASBL/tripper'
       uses: codecov/codecov-action@v3
 
-  # -- Uncomment when tripper this version of tripper has been released
-  #    such that we can import tripper with Python 3.6
-  # pytest-36:
-  #   runs-on: ubuntu-20.04
-  #
-  #   strategy:
-  #     fail-fast: false
-  #     matrix:
-  #       python-version: ["3.6.8"]
-  #
-  #   steps:
-  #   - name: Checkout tripper
-  #     uses: actions/checkout@v3
-  #
-  #   - name: Set up Python ${{ matrix.python-version }}
-  #     uses: actions/setup-python@v4
-  #     with:
-  #       python-version: ${{ matrix.python-version }}
-  #
-  #   - name: Install dependencies
-  #     run: |
-  #       python -m pip install -U pip
-  #       pip install -U setuptools wheel flit
-  #       pip install -e .
-  #       pip install pytest EMMOntoPy rdflib SPARQLWrapper DLite-Python
-  #
-  #   - name: Test with pytest
-  #     run: pytest -vvv
+    - name: Run doctest on tutorial
+      run: |
+        python -m doctest docs/tutorial.md
```

### Comparing `tripper-0.2.3/.github/workflows/ci_update_dependencies.yml` & `tripper-0.2.4/.github/workflows/ci_update_dependencies.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/.pre-commit-config.yaml` & `tripper-0.2.4/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -22,36 +22,36 @@
     - id: isort
       args:
       - --profile=black
       - --filter-files
       - --skip-gitignore
 
   - repo: https://github.com/ambv/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     - id: black
 
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
     - id: bandit
       args: ["-r"]
       files: ^tripper/.*$
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.1.1
     hooks:
     - id: mypy
       exclude: ^tests/.*$
       additional_dependencies:
         - "types-requests"
         - "pydantic"
 
   - repo: https://github.com/SINTEF/ci-cd
-    rev: v2.0.0
+    rev: v2.3.0
     hooks:
     - id: docs-api-reference
       args:
       - --package-dir=tripper
     - id: docs-landing-page
 
   - repo: local
```

### Comparing `tripper-0.2.3/CHANGELOG.md` & `tripper-0.2.4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Changelog
 
+## [v0.2.4](https://github.com/EMMC-ASBL/tripper/tree/v0.2.4) (2023-04-30)
+
+[Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.3...v0.2.4)
+
+**Implemented enhancements:**
+
+- Add entrypoint system to link external backend implementation [\#63](https://github.com/EMMC-ASBL/tripper/issues/63)
+
+**Closed issues:**
+
+- Transformations based on data sources [\#90](https://github.com/EMMC-ASBL/tripper/issues/90)
+- Add workflow example  [\#79](https://github.com/EMMC-ASBL/tripper/issues/79)
+
+**Merged pull requests:**
+
+- Added argument `lang` to triplestore.value\(\) [\#104](https://github.com/EMMC-ASBL/tripper/pull/104) ([jesper-friis](https://github.com/jesper-friis))
+- Run doctest from CI tests [\#101](https://github.com/EMMC-ASBL/tripper/pull/101) ([jesper-friis](https://github.com/jesper-friis))
+- Added add\_data\(\), get\_value\(\) and add\_interpolation\_source\(\) methods to Triplestore [\#91](https://github.com/EMMC-ASBL/tripper/pull/91) ([jesper-friis](https://github.com/jesper-friis))
+- Added tests for Python 3.11 and 3.6 [\#84](https://github.com/EMMC-ASBL/tripper/pull/84) ([jesper-friis](https://github.com/jesper-friis))
+- Remove some deprecation warnings [\#83](https://github.com/EMMC-ASBL/tripper/pull/83) ([jesper-friis](https://github.com/jesper-friis))
+- Workflow example [\#81](https://github.com/EMMC-ASBL/tripper/pull/81) ([jesper-friis](https://github.com/jesper-friis))
+- Support external backends [\#80](https://github.com/EMMC-ASBL/tripper/pull/80) ([jesper-friis](https://github.com/jesper-friis))
+
 ## [v0.2.3](https://github.com/EMMC-ASBL/tripper/tree/v0.2.3) (2023-02-05)
 
 [Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.2...v0.2.3)
 
 **Closed issues:**
 
 - Add a to\_yaml\(\) method to MappingStep [\#66](https://github.com/EMMC-ASBL/tripper/issues/66)
```

### Comparing `tripper-0.2.3/LICENSE` & `tripper-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/README.md` & `tripper-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
 A triplestore wrapper is created with the [`tripper.Triplestore`][Triplestore] class.
 
 
 
 Documentation
 -------------
-* Getting started: Take a look at the [tutorial](docs/tutorial.md).
-* Reference manual: [API Reference]
+* Getting started: See the [tutorial](docs/tutorial.md)
+* [Discovery of custom backends](docs/backend_discovery.md)
+* [Reference manual]
 
 
 Installation
 ------------
 Tripper has by itself no dependencies outside the standard library, but the triplestore backends may have specific dependencies.
 
 
@@ -55,11 +56,11 @@
 SINTEF.
 
 
 
 
 [rdflib]: https://rdflib.readthedocs.io/en/stable/
 [PyPI]: https://pypi.org/project/tripper
-[API Reference]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/
+[Reference manual]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/
 [Literal]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Literal
 [Namespace]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Namespace
 [Triplestore]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Triplestore
```

### Comparing `tripper-0.2.3/docs/index.md` & `tripper-0.2.4/docs/index.md`

 * *Files 17% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
 A triplestore wrapper is created with the [`tripper.Triplestore`][Triplestore] class.
 
 
 
 Documentation
 -------------
-* Getting started: Take a look at the [tutorial](tutorial.md).
-* Reference manual: [API Reference]
+* Getting started: See the [tutorial](tutorial.md)
+* [Discovery of custom backends](backend_discovery.md)
+* [Reference manual]
 
 
 Installation
 ------------
 Tripper has by itself no dependencies outside the standard library, but the triplestore backends may have specific dependencies.
 
 
@@ -55,11 +56,11 @@
 SINTEF.
 
 
 
 
 [rdflib]: https://rdflib.readthedocs.io/en/stable/
 [PyPI]: https://pypi.org/project/tripper
-[API Reference]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/
+[Reference manual]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/
 [Literal]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Literal
 [Namespace]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Namespace
 [Triplestore]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Triplestore
```

### Comparing `tripper-0.2.3/docs/mappings/figs/function_emmo.svg` & `tripper-0.2.4/docs/mappings/figs/function_emmo.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/docs/tutorial.md` & `tripper-0.2.4/docs/tutorial.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,101 @@
 Tutorial
 ========
 <!-- markdownlint-disable MD007 -->
 
 Create a triplestore instance using the `rdflib` backend:
 
 ```python
-from tripper import Triplestore
-ts = Triplestore(backend="rdflib")
+>>> from tripper import Triplestore
+>>> ts = Triplestore(backend="rdflib")
+
 ```
 
 The module already provides a set of pre-defined namespaces that simplifies writing IRIs.
 For example:
 
 ```python
-from tripper import RDFS, OWL
-RDFS.subClassOf
-# -> 'http://www.w3.org/2000/01/rdf-schema#subClassOf'
+>>> from tripper import RDFS, OWL
+>>> RDFS.subClassOf
+'http://www.w3.org/2000/01/rdf-schema#subClassOf'
+
 ```
 
 New namespaces can be created using the Namespace class, but are usually added with the `bind()` method:
 
 ```python
-ONTO = ts.bind("onto", "http://example.com/onto#")
-ONTO.MyConcept
-# -> 'http://example.com/onto#MyConcept'
+>>> ONTO = ts.bind("onto", "http://example.com/onto#")
+>>> ONTO.MyConcept
+'http://example.com/onto#MyConcept'
+
 ```
 
 Namespace also supports access by label and IRI checking.
 Both of these features requires loading an ontology.
 The following example shows how to create an EMMO namespace with IRI checking.
 The keyword argument `label_annotations=True` enables access by `skos:prefLabel`, `rdfs:label` or `skos:altLabel`.
 The `check=True` enables checking for existing IRIs.
 The `triplestore_url=...` is a resolvable URL that can be read by the 'rdflib' backend.
 It is needed, because the 'rdflib' backend is currently not able to load EMMO from the `http://emmo.info/emmo#` namespace.
 
 ```python
-EMMO = ts.bind(
-    "emmo", "http://emmo.info/emmo#",
-    label_annotations=True,
-    check=True,
-    triplestore_url="https://emmo-repo.github.io/versions/1.0.0-beta4/emmo-inferred.ttl",
-)
-EMMO.Atom
-# -> 'http://emmo.info/emmo#EMMO_eb77076b_a104_42ac_a065_798b2d2809ad'
-EMMO.invalid_name
-# -> NoSuchIRIError: http://emmo.info/emmo#invalid_name
+>>> EMMO = ts.bind(
+...     "emmo", "http://emmo.info/emmo#",
+...     label_annotations=True,
+...     check=True,
+...     triplestore_url="https://emmo-repo.github.io/versions/1.0.0-beta4/emmo-inferred.ttl",
+... )
+
+>>> EMMO.Atom
+'http://emmo.info/emmo#EMMO_eb77076b_a104_42ac_a065_798b2d2809ad'
+
+>>> EMMO.invalid_name
+Traceback (most recent call last):
+    ...
+tripper.errors.NoSuchIRIError: http://emmo.info/emmo#invalid_name
+
 ```
 
-New triples can be added either with the `parse()` method (for backends that support it) or the `add()` and `add_triples()` methods:
+New triples can be added with the `add()` and `add_triples()` methods:
 
 ```python
 # en(msg) is a convenient function for adding english literals.
 # It is equivalent to ``tripper.Literal(msg, lang="en")``.
-from tripper.utils import en
+>>> from tripper.utils import en
+>>> ts.add_triples([
+...     (ONTO.MyConcept, RDFS.subClassOf, OWL.Thing),
+...     (ONTO.MyConcept, RDFS.label, en("My briliant ontological concept.")),
+... ])
+
+```
+
+You can also load triples from a source using the `parse()` method (for backends that support it):
+
+```python
 ts.parse("onto.ttl", format="turtle")
-ts.add_triples([
-    (ONTO.MyConcept, RDFS.subClassOf, OWL.Thing),
-    (ONTO.MyConcept, RDFS.label, en("My briliant ontological concept.")),
-])
 ```
 
+
 For backends that support it the triplestore can be serialised using `serialize()`:
 
 ```python
 ts.serialize("onto2.ttl")
 ```
 
 A set of convenient functions exists for simple queries, including `triples()`, `subjects()`, `predicates()`, `objects()`, `subject_predicates()`, `subject_objects()`, `predicate_objects()` and `value()`.
 Except for `value()`, they return the result as generators.
 For example:
 
 ```python
-ts.objects(subject=ONTO.MyConcept, predicate=RDFS.subClassOf)
-# -> <generator object Triplestore.objects at 0x7fa502590200>
-list(ts.objects(subject=ONTO.MyConcept, predicate=RDFS.subClassOf))
-# -> ['http://www.w3.org/2002/07/owl#Thing']
+>>> ts.objects(subject=ONTO.MyConcept, predicate=RDFS.subClassOf)  # doctest: +ELLIPSIS
+<generator object Triplestore.objects at 0x...>
+
+>>> list(ts.objects(subject=ONTO.MyConcept, predicate=RDFS.subClassOf))
+['http://www.w3.org/2002/07/owl#Thing']
+
 ```
 
 The `query()` and `update()` methods can be used to query and update the triplestore using SPARQL.
 
 Finally Triplestore has two specialised methods `add_mapsTo()` and `add_function()` that simplify working with mappings.
 `add_mapsTo()` is convinient for defining new mappings:
```

### Comparing `tripper-0.2.3/mkdocs.yml` & `tripper-0.2.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/pyproject.toml` & `tripper-0.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,70 +10,68 @@
 description = "A triplestore wrapper for Python."
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Environment :: Plugins",
     "Natural Language :: English",
     "Operating System :: OS Independent",
 ]
 keywords = ["triplestore", "ontology", "RDF"]
 requires-python = "~=3.7"
 dynamic = ["version"]
 
 dependencies = [
-    "typing-extensions ~=4.4 ; python_version<'3.8'",
+    "typing-extensions ~=4.5; python_version<'3.8'",
 ]
 
 [project.optional-dependencies]
 docs = [
     "mike ~=1.1",
     "mkdocs ~=1.4",
     "mkdocs-awesome-pages-plugin ~=2.8",
-    "mkdocs-material ~=9.0",
+    "mkdocs-material ~=9.1",
     "mkdocstrings[python-legacy] ~=0.20.0",
-    "EMMOntoPy ~=0.4",
-    "rdflib ~=6.2",
+    "EMMOntoPy ~=0.5",
+    "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.16,<1",
+    "DLite-Python >=0.3.18,<1",
 ]
 pre-commit = [
     "pre-commit ~=2.21",
     "pylint ~=2.13",
 ]
 testing = [
     "pytest ~=7.2",
     "pytest-cov ~=4.0",
-    "EMMOntoPy ~=0.4",
-    "rdflib ~=6.2",
+    "EMMOntoPy ~=0.5",
+    "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.16,<1",
+    "DLite-Python >=0.3.18,<1",
 ]
 dev = [
     "mike ~=1.1",
     "mkdocs ~=1.4",
     "mkdocs-awesome-pages-plugin ~=2.8",
-    "mkdocs-material ~=9.0",
+    "mkdocs-material ~=9.1",
     "mkdocstrings[python-legacy] ~=0.20.0",
     "pre-commit ~=2.21",
     "pylint ~=2.13",
     "pytest ~=7.2",
     "pytest-cov ~=4.0",
-    "EMMOntoPy ~=0.4",
-    "rdflib ~=6.2",
+    "EMMOntoPy ~=0.5",
+    "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.16,<1",
+    "DLite-Python >=0.3.18,<1",
 ]
 
 [project.urls]
 Home = "https://github.com/EMMC-ASBL/tripper"
 Documentation = "https://EMMC-ASBL.github.io/tripper"
 Source = "https://github.com/EMMC-ASBL/tripper"
 "Issue Tracker" = "https://github.com/EMMC-ASBL/tripper/issues"
```

### Comparing `tripper-0.2.3/tests/conftest.py` & `tripper-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tests/mappings/test_mappings.py` & `tripper-0.2.4/tests/mappings/test_mappings.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tests/ontologies/family.ttl` & `tripper-0.2.4/tests/ontologies/family.ttl`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tests/ontologies/food.ttl` & `tripper-0.2.4/tests/ontologies/food.ttl`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tests/test_add_function.py` & `tripper-0.2.4/tests/test_add_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 @prefix dcterms: <http://purl.org/dc/terms/> .
 @prefix ex: <http://example.com/ex#> .
 @prefix fno: <https://w3id.org/function/ontology#> .
 @prefix map: <http://emmo.info/domain-mappings#> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
-<:func_f1a5429a> a fno:Function ;
+<:func_daa3fc91> a fno:Function ;
     rdfs:label "func"@en ;
     dcterms:description "Returns the sum of `a` and `b`."@en ;
-    fno:expects ( <:func_f1a5429a_parameter1_a> <:func_f1a5429a_parameter2_b> ) ;
-    fno:returns ( <:func_f1a5429a_output1> ) .
+    fno:expects ( <:func_daa3fc91_parameter1_a> <:func_daa3fc91_parameter2_b> ) ;
+    fno:returns ( <:func_daa3fc91_output1> ) .
 
-<:func_f1a5429a_output1> a fno:Output ;
+<:func_daa3fc91_output1> a fno:Output ;
     map:mapsTo ex:sum .
 
-<:func_f1a5429a_parameter1_a> a fno:Parameter ;
+<:func_daa3fc91_parameter1_a> a fno:Parameter ;
     rdfs:label "a"@en ;
     map:mapsTo ex:arg1 .
 
-<:func_f1a5429a_parameter2_b> a fno:Parameter ;
+<:func_daa3fc91_parameter2_b> a fno:Parameter ;
     rdfs:label "b"@en ;
     map:mapsTo ex:arg2 .
 """.strip()
 )
 
 
 ts2 = Triplestore(backend="rdflib")
@@ -58,15 +58,15 @@
     ts2.serialize().strip()
     == """
 @prefix dcterms: <http://purl.org/dc/terms/> .
 @prefix emmo: <http://emmo.info/emmo#> .
 @prefix ex: <http://example.com/ex#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
-<:func_f1a5429a> a emmo:EMMO_4299e344_a321_4ef2_a744_bacfcce80afc ;
+<:func_daa3fc91> a emmo:EMMO_4299e344_a321_4ef2_a744_bacfcce80afc ;
     rdfs:label "func"@en ;
     emmo:EMMO_36e69413_8c59_4799_946c_10b05d266e22 ex:arg1,
         ex:arg2 ;
     emmo:EMMO_c4bace1d_4db0_4cd3_87e9_18122bae2840 ex:sum ;
     dcterms:description "Returns the sum of `a` and `b`."@en .
 
 ex:arg1 a emmo:EMMO_194e367c_9783_4bf5_96d0_9ad597d48d9a ;
@@ -92,15 +92,15 @@
     ts3.serialize().strip()
     == """
 @prefix dcterms: <http://purl.org/dc/terms/> .
 @prefix emmo: <http://emmo.info/emmo#> .
 @prefix ex: <http://example.com/ex#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 
-<:func_f1a5429a> a emmo:EMMO_4299e344_a321_4ef2_a744_bacfcce80afc ;
+<:func_daa3fc91> a emmo:EMMO_4299e344_a321_4ef2_a744_bacfcce80afc ;
     rdfs:label "func"@en ;
     emmo:EMMO_36e69413_8c59_4799_946c_10b05d266e22 ex:arg1,
         ex:arg2 ;
     emmo:EMMO_c4bace1d_4db0_4cd3_87e9_18122bae2840 ex:sum ;
     dcterms:description "Returns the sum of `a` and `b`."@en .
 
 ex:arg1 a emmo:EMMO_194e367c_9783_4bf5_96d0_9ad597d48d9a ;
```

### Comparing `tripper-0.2.3/tests/test_literals.py` & `tripper-0.2.4/tests/test_literals.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tests/test_namespace.py` & `tripper-0.2.4/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tests/test_triplestore.py` & `tripper-0.2.4/tests/test_triplestore.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Test triplestore.
 
 If backend is given, only that backend will be tested.  Otherwise all
 installed backends are tested one by one.
 """
-# pylint: disable=duplicate-code,comparison-with-callable
+# pylint: disable=duplicate-code,comparison-with-callable,invalid-name
 from typing import TYPE_CHECKING
 
 import pytest
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Any, Callable
 
 
 # @pytest.mark.parametrize("backend", ["rdflib", "ontopy", "collection"])
 @pytest.mark.parametrize("backend", ["rdflib", "collection"])
-def test_triplestore(
+def test_triplestore(  # pylint: disable=too-many-locals
     backend: str,
     example_function: "Callable[[Any, Any], Any]",
     expected_function_triplestore: str,
 ) -> None:
     """Test the Triplestore class.
 
     Parameters:
@@ -27,47 +27,47 @@
         example_function: Fixture from `conftest.py` to return a function
             implementation example for use with Triplestore.
         expected_function_triplestore: Fixture from `conftest.py`, which returns a
             Turtle-serialized string of what is expected when serializing the
             Triplestore in this test.
 
     """
-    from tripper.triplestore import OWL, RDF, RDFS, XSD, Triplestore
+    from tripper.triplestore import DCTERMS, OWL, RDF, RDFS, XSD, Triplestore
 
-    store = Triplestore(backend)
-    assert store.expand_iri("xsd:integer") == XSD.integer
-    assert store.prefix_iri(RDF.type) == "rdf:type"
-    EX = store.bind("ex", "http://example.com/onto#")  # pylint: disable=invalid-name
+    ts = Triplestore(backend)
+    assert ts.expand_iri("xsd:integer") == XSD.integer
+    assert ts.prefix_iri(RDF.type) == "rdf:type"
+    EX = ts.bind("ex", "http://example.com/onto#")  # pylint: disable=invalid-name
     assert str(EX) == "http://example.com/onto#"
-    store.add_mapsTo(EX.MyConcept, "http://onto-ns.com/meta/0.1/MyEntity", "myprop")
-    store.add((EX.MyConcept, RDFS.subClassOf, OWL.Thing))
-    store.add((EX.AnotherConcept, RDFS.subClassOf, OWL.Thing))
-    store.add((EX.Sum, RDFS.subClassOf, OWL.Thing))
-    assert store.has(EX.Sum) is True
-    assert store.has(EX.Sum, RDFS.subClassOf, OWL.Thing) is True
-    assert store.has(object=EX.NotInOntology) is False
+    ts.add_mapsTo(EX.MyConcept, "http://onto-ns.com/meta/0.1/MyEntity", "myprop")
+    ts.add((EX.MyConcept, RDFS.subClassOf, OWL.Thing))
+    ts.add((EX.AnotherConcept, RDFS.subClassOf, OWL.Thing))
+    ts.add((EX.Sum, RDFS.subClassOf, OWL.Thing))
+    assert ts.has(EX.Sum) is True
+    assert ts.has(EX.Sum, RDFS.subClassOf, OWL.Thing) is True
+    assert ts.has(object=EX.NotInOntology) is False
 
-    store.add_function(
+    func_iri = ts.add_function(
         example_function,
         expects=(EX.MyConcept, EX.AnotherConcept),
         returns=EX.Sum,
         base_iri=EX,
         standard="fno",
     )
 
     try:
-        ts_as_turtle = store.serialize(format="turtle")
+        ts_as_turtle = ts.serialize(format="turtle")
     except NotImplementedError:
         pass
     else:
         assert ts_as_turtle == expected_function_triplestore
 
     # Test SPARQL query
     try:
-        rows = store.query("SELECT ?s ?o WHERE { ?s rdfs:subClassOf ?o }")
+        rows = ts.query("SELECT ?s ?o WHERE { ?s rdfs:subClassOf ?o }")
     except NotImplementedError:
         pass
     else:
         assert len(rows) == 3
         rows.sort()  # ensure consistent ordering of rows
         assert rows[0] == (
             "http://example.com/onto#AnotherConcept",
@@ -78,53 +78,60 @@
             "http://www.w3.org/2002/07/owl#Thing",
         )
         assert rows[2] == (
             "http://example.com/onto#Sum",
             "http://www.w3.org/2002/07/owl#Thing",
         )
 
+    # Test value() method
+    assert ts.value(func_iri, DCTERMS.description) == example_function.__doc__
+    assert (
+        ts.value(func_iri, DCTERMS.description, lang="en") == example_function.__doc__
+    )
+    assert ts.value(func_iri, DCTERMS.description, lang="de") is None
+
 
 def test_backend_rdflib(expected_function_triplestore: str) -> None:
     """Specifically test the rdflib backend Triplestore.
 
     Parameters:
         expected_function_triplestore: Fixture from `conftest.py`, which returns a
             Turtle-serialized string of what is expected when serializing the
             Triplestore in this test.
 
     """
     from tripper.triplestore import RDFS, Triplestore
 
-    store = Triplestore("rdflib")
-    EX = store.bind("ex", "http://example.com/onto#")  # pylint: disable=invalid-name
-    store.parse(format="turtle", data=expected_function_triplestore)
-    assert store.serialize(format="turtle") == expected_function_triplestore
-    store.set((EX.AnotherConcept, RDFS.subClassOf, EX.MyConcept))
+    ts = Triplestore("rdflib")
+    EX = ts.bind("ex", "http://example.com/onto#")  # pylint: disable=invalid-name
+    ts.parse(format="turtle", data=expected_function_triplestore)
+    assert ts.serialize(format="turtle") == expected_function_triplestore
+    ts.set((EX.AnotherConcept, RDFS.subClassOf, EX.MyConcept))
 
     def cost(parameter):
         return 2 * parameter
 
-    store.add_mapsTo(EX.Sum, "http://onto-ns.com/meta/0.1/MyEntity#sum", cost=cost)
-    assert list(store.function_repo.values())[0] == cost
+    ts.add_mapsTo(EX.Sum, "http://onto-ns.com/meta/0.1/MyEntity#sum", cost=cost)
+    assert list(ts.function_repo.values())[0] == cost
 
     def func(parameter):
         return parameter + 1
 
-    store.add_function(func, expects=EX.Sum, returns=EX.OneMore, cost=cost)
-    assert list(store.function_repo.values())[1] == func
-    assert len(store.function_repo) == 2  # cost is only added once
+    ts.add_function(func, expects=EX.Sum, returns=EX.OneMore, cost=cost)
+    assert list(ts.function_repo.values())[1] == func
+    assert len(ts.function_repo) == 2  # cost is only added once
 
     def func2(parameter):
         return parameter + 2
 
     def cost2(parameter):
         return 2 * parameter + 1
 
-    store.add_function(func2, expects=EX.Sum, returns=EX.EvenMore, cost=cost2)
-    assert len(store.function_repo) == 4
+    ts.add_function(func2, expects=EX.Sum, returns=EX.EvenMore, cost=cost2)
+    assert len(ts.function_repo) == 4
 
 
 def test_backend_rdflib_base_iri(
     get_ontology_path: "Callable[[str], Path]", tmp_path: "Path"
 ) -> None:
     """Test rdflib with `base_iri`.
 
@@ -139,26 +146,26 @@
 
     from tripper.triplestore import RDF, Triplestore
 
     ontopath_family = get_ontology_path("family")
     tmp_onto = tmp_path / "family.ttl"
     shutil.copy(ontopath_family, tmp_onto)
 
-    store = Triplestore(backend="rdflib", base_iri=f"file://{tmp_onto}")
-    FAM = store.bind(  # pylint: disable=invalid-name
+    ts = Triplestore(backend="rdflib", base_iri=f"file://{tmp_onto}")
+    FAM = ts.bind(  # pylint: disable=invalid-name
         "fam", "http://onto-ns.com/ontologies/examples/family#"
     )
-    store.add_triples(
+    ts.add_triples(
         [
             (":Nils", RDF.type, FAM.Father),
             (":Anna", RDF.type, FAM.Dauther),
             (":Nils", FAM.hasChild, ":Anna"),
         ]
     )
-    store.close()
+    ts.close()
 
 
 def test_backend_ontopy(get_ontology_path: "Callable[[str], Path]") -> None:
     """Specifically test the ontopy backend Triplestore.
 
     Parameters:
         get_ontology_path: Fixture from `conftest.py` to retrieve a `pathlib.Path`
@@ -172,59 +179,59 @@
     FOOD = Namespace(  # pylint: disable=invalid-name
         "http://onto-ns.com/ontologies/examples/food#",
         label_annotations=True,
         check=True,
         triplestore_url=ontopath_food,
     )
 
-    store = Triplestore(
+    ts = Triplestore(
         "ontopy",
         base_iri="http://onto-ns.com/ontologies/examples/food",
     )
-    store.parse(ontopath_food)
+    ts.parse(ontopath_food)
 
-    store = Triplestore(
+    ts = Triplestore(
         "ontopy",
         base_iri="http://onto-ns.com/ontologies/examples/food",
     )
-    store.bind("food", FOOD)
+    ts.bind("food", FOOD)
     with open(ontopath_food, "rt", encoding="utf8") as handle:
-        store.parse(data=handle.read())
+        ts.parse(data=handle.read())
 
 
 def test_backend_sparqlwrapper() -> None:
     """Specifically test the SPARQLWrapper backend Triplestore."""
     from tripper import SKOS, Triplestore
 
-    store = Triplestore(
+    ts = Triplestore(
         backend="sparqlwrapper",
         base_iri="http://vocabs.ardc.edu.au/repository/api/sparql/"
         "csiro_international-chronostratigraphic-chart_geologic-time-scale-2020",
     )
-    for s, p, o in store.triples((None, SKOS.notation, None)):
+    for s, p, o in ts.triples(predicate=SKOS.notation):
         assert s
         assert p
         assert o
 
 
 @pytest.mark.skip(
     "These will fail because we do not have credentials to modify the triplestore"
 )
 def test_backend_sparqlwrapper_methods() -> None:
     """Test SPARQLWrapper methods."""
     from tripper import RDFS, SKOS, Literal, Namespace, Triplestore
 
-    store = Triplestore(
+    ts = Triplestore(
         backend="sparqlwrapper",
         base_iri="http://vocabs.ardc.edu.au/repository/api/sparql/"
         "csiro_international-chronostratigraphic-chart_geologic-time-scale-2020",
     )
 
-    store.remove((None, SKOS.notation, None))
+    ts.remove((None, SKOS.notation, None))
 
     EX = Namespace("http://example.com#")  # pylint: disable=invalid-name
-    store.add_triples(
+    ts.add_triples(
         [
             (EX.a, RDFS.subClassOf, EX.base),
             (EX.a, SKOS.prefLabel, Literal("An a class.", lang="en")),
         ]
     )
```

### Comparing `tripper-0.2.3/tests/test_utils.py` & `tripper-0.2.4/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Test utils"""
 # pylint: disable=invalid-name,too-few-public-methods
 import dlite
 import pytest
 
 from tripper import DCTERMS, RDFS, XSD, Literal
 from tripper.utils import (
+    as_python,
     en,
     function_id,
     infer_iri,
     parse_literal,
     parse_object,
+    random_string,
     split_iri,
 )
 
 # Test infer_iri()
 assert infer_iri(RDFS.subClassOf) == RDFS.subClassOf
 
 coll = dlite.Collection()
@@ -156,7 +158,22 @@
 assert parse_object('"abc"@en') == Literal("abc", lang="en")
 assert parse_object(str(XSD)) == str(XSD)
 assert parse_object(XSD.int) == XSD.int
 assert parse_object(f'"42"^^{XSD.integer}') == Literal("42", datatype=XSD.integer)
 assert parse_object(f'"4.2"^^{XSD.double}') == Literal("4.2", datatype=XSD.double)
 assert parse_object(f'"42"^^{XSD.double}') == Literal("42.0", datatype=XSD.double)
 assert parse_object(f'"42"^^{XSD.int}') == Literal("42", datatype=XSD.int)
+
+
+# test as_python()
+assert as_python("abc") == "abc"
+assert as_python('"abc"@en') == "abc"
+assert as_python(f'"42"^^{XSD.double}') == 42
+assert as_python(Literal(32, datatype=XSD.integer)) == 32
+assert as_python(3.14) == 3.14
+
+
+# test random_string()
+rstring = random_string(16)
+assert isinstance(rstring, str)
+assert len(rstring) == 16
+assert rstring.isalnum()
```

### Comparing `tripper-0.2.3/tripper/__init__.py` & `tripper-0.2.4/tripper/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     RDF,
     RDFS,
     SKOS,
     XML,
     XSD,
     Namespace,
 )
-from .triplestore import Triplestore
+from .triplestore import Triplestore, backend_packages
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 __all__ = (
     "Literal",
     #
     "DC",
     "DCTERMS",
     "DM",
@@ -41,8 +41,9 @@
     "RDFS",
     "SKOS",
     "XML",
     "XSD",
     "Namespace",
     #
     "Triplestore",
+    "backend_packages",
 )
```

### Comparing `tripper-0.2.3/tripper/backends/__init__.py` & `tripper-0.2.4/tripper/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tripper/backends/collection.py` & `tripper-0.2.4/tripper/backends/collection.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tripper/backends/ontopy.py` & `tripper-0.2.4/tripper/backends/ontopy.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tripper/backends/rdflib.py` & `tripper-0.2.4/tripper/backends/rdflib.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,19 @@
         """Returns a generator over matching triples."""
         for s, p, o in self.graph.triples(  # pylint: disable=not-an-iterable
             astriple(triple)
         ):
             yield (
                 str(s),
                 str(p),
-                Literal(o.value, lang=o.language, datatype=o.datatype)
+                Literal(
+                    o.value,
+                    lang=o.language,
+                    datatype=str(o.datatype) if o.datatype else o.datatype,
+                )
                 if isinstance(o, rdflibLiteral)
                 else str(o),
             )
 
     def add_triples(self, triples: "Sequence[Triple]"):
         """Add a sequence of triples."""
         for triple in triples:
```

### Comparing `tripper-0.2.3/tripper/backends/sparqlwrapper.py` & `tripper-0.2.4/tripper/backends/sparqlwrapper.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tripper/interface.py` & `tripper-0.2.4/tripper/interface.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tripper/literal.py` & `tripper-0.2.4/tripper/literal.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
             value = float(self)
         elif self.datatype == XSD.hexBinary:
             value = self.encode()
         elif self.datatype == XSD.dateTime:
             value = datetime.fromisoformat(self)
         elif self.datatype and self.datatype not in self.datatypes[str]:
             warnings.warn(f"unknown datatype: {self.datatype} - assuming string")
+
         return value
 
     def n3(self) -> str:  # pylint: disable=invalid-name
         """Returns a representation in n3 format."""
         if self.lang:
             return f'"{self}"@{self.lang}'
         if self.datatype:
```

### Comparing `tripper-0.2.3/tripper/mappings/mappings.py` & `tripper-0.2.4/tripper/mappings/mappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from enum import Enum
 from typing import TYPE_CHECKING, Sequence
 
 import numpy as np
 from pint import Quantity  # remove
 
 from tripper import DM, EMMO, FNO, MAP, RDF, RDFS
+from tripper.triplestore import hasAccessFunction, hasDataValue
 from tripper.utils import parse_literal
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
     from tripper import Triplestore
 
@@ -88,25 +89,67 @@
         self,
         value: "Any" = None,
         unit: "Optional[str]" = None,
         iri: "Optional[str]" = None,
         property_iri: "Optional[str]" = None,
         cost: "Union[float, Callable]" = 0.0,
     ):
-        self.value = value
+        self._value = value
         self.unit = unit
         if iri:
             self.output_iri = iri
         elif hasattr(value, __name__):
             self.output_iri = value.__name__
         else:
             self.output_iri = f"_:value_{id(value)}"
         self.property_iri = property_iri
         self.cost = cost
 
+    value = property(
+        lambda self: self._value() if callable(self._value) else self._value,
+        doc="Value of property.",
+    )
+
+    def __repr__(self):
+        args = []
+        if self.unit:
+            args.append(", unit={self.unit}")
+        if self.output_iri:
+            args.append(", iri={self.output_iri}")
+        if self.property_iri:
+            args.append(", property_iri={self.property_iri}")
+        if self.cost:
+            args.append(", cost={self.cost}")
+        return f"Value({self._value}{''.join(args)})"
+
+    def get_value(self, unit=None, magnitude=False, quantity=None) -> "Any":
+        """Returns the evaluated value of given input route number.
+
+        Arguments:
+            unit: return the result in the given unit.
+                Implies `magnitude=True`.
+            magnitude: Whether to only return the magnitude of the evaluated
+                value (with no unit).
+            quantity: Quantity class to use for evaluation.  Defaults to pint.
+
+        Returns:
+            Value.
+        """
+        if quantity is None:
+            quantity = Quantity
+        value = self._value() if callable(self._value) else self._value
+        if not isinstance(value, Quantity) and not self.unit:
+            return value
+        q = quantity(value, self.unit)
+        if unit:
+            return q.m_as(unit)
+        if magnitude:
+            return q.m
+        return q
+
     def show(
         self,
         routeno: "Optional[int]" = None,
         name: "Optional[str]" = None,
         indent: int = 0,
     ) -> str:
         # pylint: disable=unused-argument
@@ -116,15 +159,14 @@
             routeno: Unused.  The argument exists for consistency with
                 the corresponding method in Step.
             name: Name of value.
             indent: Indentation level.
 
         Returns:
             String representation of the value.
-
         """
         strings = []
         ind = " " * indent
         strings.append(ind + f'{name if name else "Value"}:')
         strings.append(ind + f"  iri: {self.output_iri}")
         strings.append(ind + f"  property_iri: {self.property_iri}")
         strings.append(ind + f"  unit: {self.unit}")
@@ -208,15 +250,15 @@
         self.joined_input = {}
 
     def eval(
         self,
         routeno: "Optional[int]" = None,
         unit: "Optional[str]" = None,
         magnitude: bool = False,
-        quantity: "Type[Quantity]" = Quantity,
+        quantity: "Optional[Type[Quantity]]" = None,
     ) -> "Any":
         """Returns the evaluated value of given input route number.
 
         Arguments:
             routeno: The route number to evaluate.  If None (default)
                 the route with the lowest cost is evalueated.
             unit: return the result in the given unit.
@@ -224,29 +266,36 @@
             magnitude: Whether to only return the magnitude of the evaluated
                 value (with no unit).
             quantity: Quantity class to use for evaluation.  Defaults to pint.
 
         Returns:
             Evaluation result.
         """
+        if quantity is None:
+            quantity = Quantity
         if routeno is None:
             ((_, routeno),) = self.lowest_costs(nresults=1)
         inputs, idx = self.get_inputs(routeno)
         values = get_values(inputs, idx, quantity=quantity)
-        if self.function:
+
+        if len(inputs) == 1 and all(isinstance(v, Value) for v in inputs.values()):
+            (value,) = tuple(inputs.values())
+        elif self.function:
             value = self.function(**values)
         elif len(values) == 1:
             (value,) = values.values()
         else:
             raise TypeError(f"Expected inputs to be a single argument: {values}")
 
-        if isinstance(value, quantity) and unit:
+        if isinstance(value, Quantity) and unit:
             return value.m_as(unit)
-        if isinstance(value, quantity) and magnitude:
+        if isinstance(value, Quantity) and magnitude:
             return value.m
+        if isinstance(value, Value):
+            return value.get_value(unit=unit, magnitude=magnitude, quantity=quantity)
         return value
 
     def get_inputs(self, routeno: int) -> "Tuple[Inputs, int]":
         """Returns input and input index `(inputs, idx)` for route number
         `routeno`.
 
         Arguments:
@@ -575,15 +624,15 @@
             value = v.eval(routeno=routeno, quantity=quantity)
             values[k] = (
                 value.to(v.output_unit)
                 if v.output_unit and isinstance(v, quantity)
                 else value
             )
         elif isinstance(v, Value):
-            values[k] = quantity(v.value, v.unit)
+            values[k] = v.value if v.unit is None else quantity(v.value, v.unit)
         else:
             raise TypeError(
                 "Expected values in inputs to be either `MappingStep` or "
                 "`Value` objects."
             )
 
         if magnitudes:
@@ -667,15 +716,15 @@
                 d[ret].append((func, input_iris))
 
     return d
 
 
 def mapping_routes(
     target: str,
-    sources: "Dict[str, Value]",
+    sources: "Union[Dict[str, Union[Value, None]], Sequence[str]]",
     triplestore: "Triplestore",
     function_repo: "Optional[dict]" = None,
     function_mappers: "Union[str, Sequence[Callable]]" = (emmo_mapper, fno_mapper),
     default_costs: "Tuple" = (
         ("function", 10.0),
         ("mapsTo", 2.0),
         ("instanceOf", 1.0),
@@ -687,27 +736,28 @@
     mapsTo: str = MAP.mapsTo,
     instanceOf: str = DM.instanceOf,
     subClassOf: str = RDFS.subClassOf,
     # description: str = DCTERMS.description,
     label: str = RDFS.label,
     hasUnit: str = DM.hasUnit,
     hasCost: str = DM.hasCost,  # TODO - add hasCost to the DM ontology
+    hasAccessFunction: str = hasAccessFunction,  # pylint: disable=redefined-outer-name
+    hasDataValue: str = hasDataValue,  # pylint: disable=redefined-outer-name
 ) -> Input:
     """Find routes of mappings from any source in `sources` to `target`.
 
     This implementation supports functions (using FnO) and subclass
     relations.  It also correctly handles transitivity of `mapsTo` and
     `subClassOf` relations.
 
     Arguments:
         target: IRI of the target in `triplestore`.
         sources: Dict mapping source IRIs to source values or a sequence
             of source IRIs (with no explicit values).
-        triplestore: Triplestore instance.
-            It is safe to pass a generator expression too.
+        triplestore: Triplestore instance for the knowledge graph to traverse.
 
     Additional arguments for fine-grained tuning:
         function_repo: Dict mapping function IRIs to corresponding Python
             function.  Default is to use `triplestore.function_repo`.
         function_mappers: Name of mapping standard: "emmo" or "fno".
             Alternatively, a sequence of mapping functions that takes
             `triplestore` as argument and return a dict mapping output IRIs
@@ -722,19 +772,23 @@
             `MappingStep` when creating the returned mapping route.
         mapsTo: IRI of 'mapsTo' in `triplestore`.
         instanceOf: IRI of 'instanceOf' in `triplestore`.
         subClassOf: IRI of 'subClassOf' in `triples`.  Set it to None if
             subclasses should not be considered.
         label: IRI of 'label' in `triplestore`.  Used for naming function
             input parameters.  The default is to use rdfs:label.
-        hasUnit: IRI of 'hasUnit' in `triples`.  Can be used to explicit
+        hasUnit: IRI of 'hasUnit' in `triplestore`.  Can be used to explicit
             specify the unit of a quantity.
-        hasCost: IRI of 'hasCost' in `triples`.  Used for associating a
+        hasCost: IRI of 'hasCost' in `triplestore`.  Used for associating a
             user-defined cost or cost function with instantiation of a
             property.
+        hasAccessFunction: IRI of 'hasAccessFunction'.  Used to associate a
+            data source to a function that retrieves the data.
+        hasDataValue: IRI of 'hasDataValue'.  Used to associate a data source
+            with its literal value.
 
     Returns:
         A MappingStep instance.  This is a root of a nested tree of
         MappingStep instances providing an (efficient) internal description
         of all possible mapping routes from `sources` to `target`.
     """
     # pylint: disable=too-many-arguments,too-many-locals,too-many-statements
@@ -758,18 +812,18 @@
         value_class = Value
 
     if mappingstep_class is None:
         mappingstep_class = MappingStep
 
     # Create lookup tables for fast access to triplestore content
     soMaps = defaultdict(list)  # (s, mapsTo, o)     ==> soMaps[s]  -> [o, ..]
-    osMaps = defaultdict(list)  # (o, mapsTo, s)     ==> osMaps[o]  -> [s, ..]
-    osSubcl = defaultdict(list)  # (o, subClassOf, s) ==> osSubcl[o] -> [s, ..]
+    osMaps = defaultdict(list)  # (o, inv(mapsTo), s)     ==> osMaps[o]  -> [s, ..]
+    osSubcl = defaultdict(list)  # (o, inv(subClassOf), s) ==> osSubcl[o] -> [s, ..]
     soInst = {}  # (s, instanceOf, o) ==> soInst[s]  -> o
-    osInst = defaultdict(list)  # (o, instanceOf, s) ==> osInst[o]  -> [s, ..]
+    osInst = defaultdict(list)  # (o, inv(instanceOf), s) ==> osInst[o]  -> [s, ..]
     for s, o in triplestore.subject_objects(mapsTo):
         soMaps[s].append(o)
         osMaps[o].append(s)
     for s, o in triplestore.subject_objects(subClassOf):
         osSubcl[o].append(s)
     for s, o in triplestore.subject_objects(instanceOf):
         if s in soInst:
@@ -778,14 +832,16 @@
                 f"property via {instanceOf} relations."
             )
         soInst[s] = o
         osInst[o].append(s)
     soName = dict(triplestore.subject_objects(label))
     soUnit = dict(triplestore.subject_objects(hasUnit))
     soCost = dict(triplestore.subject_objects(hasCost))
+    soAFun = dict(triplestore.subject_objects(hasAccessFunction))
+    soDVal = dict(triplestore.subject_objects(hasDataValue))
 
     def getcost(target, stepname):
         """Returns the cost assigned to IRI `target` for a mapping step
         of type `stepname`."""
         cost = soCost.get(target, default_costs[stepname])
         if cost is None:
             return None
@@ -800,15 +856,34 @@
         visited.add(target)
 
         def addnode(node, steptype, stepname):
             if node in visited:
                 return
             step.steptype = steptype
             step.cost = getcost(target, stepname)
-            if node in sources:
+            if node in soAFun:
+                value = value_class(
+                    value=triplestore.function_repo[soAFun[node]],
+                    unit=soUnit.get(node),
+                    iri=node,
+                    property_iri=soInst.get(node),
+                    cost=getcost(node, "value"),
+                )
+                step.add_input(value, name=soName.get(node))
+            elif node in soDVal:
+                literal = parse_literal(soDVal[node])
+                value = value_class(
+                    value=literal.to_python(),
+                    unit=soUnit.get(node),
+                    iri=node,
+                    property_iri=soInst.get(node),
+                    cost=getcost(node, "value"),
+                )
+                step.add_input(value, name=soName.get(node))
+            elif node in sources:
                 value = value_class(
                     value=sources[node],
                     unit=soUnit.get(node),
                     iri=node,
                     property_iri=soInst.get(node),
                     cost=getcost(node, "value"),
                 )
@@ -868,12 +943,13 @@
             output_iri=source,
             output_unit=soUnit.get(source),
             triplestore=triplestore,
         )
         step.add_input(step0, name=soName.get(target))
         step = step0
         target = source
+
     if target not in soMaps:
         raise MissingRelationError(f'Missing "mapsTo" relation on: {target}')
     walk(target, visited, step)
 
     return step
```

### Comparing `tripper-0.2.3/tripper/namespace.py` & `tripper-0.2.4/tripper/namespace.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.3/tripper/triplestore.py` & `tripper-0.2.4/tripper/triplestore.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 
 This module has no dependencies outside the standard library, but the
 triplestore backends may have.
 
 For developers: The usage of `s`, `p`, and `o` represent the different parts of an
 RDF Triple: subject, predicate, and object.
 """
-# pylint: disable=invalid-name,too-many-public-methods
+# pylint: disable=invalid-name,too-many-public-methods,too-many-lines
 from __future__ import annotations  # Support Python 3.7 (PEP 585)
 
+import importlib
 import inspect
 import re
+import sys
+import uuid
 import warnings
 from collections.abc import Sequence
-from importlib import import_module
 from typing import TYPE_CHECKING
 
 from tripper.errors import NamespaceError, TriplestoreError, UniquenessError
 from tripper.literal import Literal
 from tripper.namespace import (
     DCTERMS,
     DM,
@@ -32,22 +34,49 @@
     OWL,
     RDF,
     RDFS,
     XML,
     XSD,
     Namespace,
 )
-from tripper.utils import en, function_id, infer_iri, split_iri
+from tripper.utils import (
+    en,
+    function_id,
+    infer_iri,
+    parse_literal,
+    random_string,
+    split_iri,
+)
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Mapping
-    from typing import Callable, Dict, Generator, List, Optional, Tuple, Union
+    from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
+    from tripper.mappings import Value
     from tripper.utils import OptionalTriple, Triple
 
+try:
+    from importlib.metadata import entry_points
+except ImportError:
+    # Use importlib_metadata backport for Python 3.6 and 3.7
+    from importlib_metadata import entry_points
+
+
+# Default packages in which to look for tripper backends
+backend_packages = ["tripper.backends"]
+
+
+# FIXME - add the following classes and properties to ontologies
+# These would be good to have in EMMO
+DataSource = EMMO.DataSource
+hasAccessFunction = EMMO.hasAccessFunction
+hasDataValue = RDF.value  # ??
+hasUnit = DM.hasUnit
+hasCost = DM.hasCost
+
 
 # Regular expression matching a prefixed IRI
 _MATCH_PREFIXED_IRI = re.compile(r"^([a-z]+):([^/]{2}.*)$")
 
 
 class Triplestore:
     """Provides a common frontend to a range of triplestore backends."""
@@ -70,41 +99,98 @@
     }
 
     def __init__(
         self,
         backend: str,
         base_iri: "Optional[str]" = None,
         database: "Optional[str]" = None,
+        package: "Optional[str]" = None,
         **kwargs,
     ) -> None:
         """Initialise triplestore using the backend with the given name.
 
         Parameters:
             backend: Name of the backend module.
+
+                For built-in backends or backends provided via a
+                backend package (using entrypoints), this should just
+                be the name of the backend with no dots (ex: "rdflib").
+
+                For a custom backend, you can provide the full module name,
+                including the dots (ex:"mypackage.mybackend").  If `package`
+                is given, `backend` is interpreted relative to `package`
+                (ex: ..mybackend).
             base_iri: Base IRI used by the add_function() method when adding
                 new triples. May also be used by the backend.
-            database: Name of database to connect to (for backends that supports it).
+            database: Name of database to connect to (for backends that
+                supports it).
+            package: Required when `backend` is a relative module.  In that
+                case, it is relative to `package`.
             kwargs: Keyword arguments passed to the backend's __init__()
                 method.
+
         """
-        module = import_module(
-            backend if "." in backend else f"tripper.backends.{backend}"
-        )
+        module = self._load_backend(backend, package)
         cls = getattr(module, f"{backend.title()}Strategy")
         self.base_iri = base_iri
         self.namespaces: "Dict[str, Namespace]" = {}
         self.closed = False
         self.backend_name = backend
         self.backend = cls(base_iri=base_iri, database=database, **kwargs)
+
         # Keep functions in the triplestore for convienence even though
         # they usually do not belong to the triplestore per se.
-        self.function_repo: "Dict[str, Union[float, Callable[[], float], None]]" = {}
+        self.function_repo: "Dict[str, Union[float, Callable, None]]" = {}
         for prefix, namespace in self.default_namespaces.items():
             self.bind(prefix, namespace)
 
+    @classmethod
+    def _load_backend(cls, backend: str, package: "Optional[str]" = None):
+        """Load and return backend module.  The arguments has the same meaning
+        as corresponding arguments to __init__().
+
+        If `backend` contains a dot or `package` is given, import `backend` using
+        `package` for relative imports.
+
+        Otherwise, if there in the "tripper.backends" entry point group exists
+        an entry point who's name matches `backend`, then the corresponding module
+        is loaded.
+
+        Otherwise, look for the `backend` in any of the (sub)packages listed
+        `backend_packages` module variable.
+        """
+        # Explicitly specified backend
+        if "." in backend or package:
+            return importlib.import_module(backend, package)
+
+        # Installed backend package
+        if (3, 8) <= sys.version_info < (3, 10):
+            # Fallback for Python 3.8 and 3.9
+            eps = entry_points().get("tripper.backends", ())
+        else:
+            # New entry_point interface from Python 3.10+, which is also
+            # implemented in the importlib_metadata backport for Python 3.6
+            # and 3.7.
+            eps = entry_points(group="tripper.backends")
+        for entry_point in eps:
+            if entry_point.name == backend:
+                return importlib.import_module(entry_point.module)
+
+        # Backend module
+        for pack in backend_packages:
+            try:
+                return importlib.import_module(f"{pack}.{backend}")
+            except ModuleNotFoundError:
+                pass
+
+        raise ModuleNotFoundError(
+            "No tripper backend named '{backend}'",
+            name=backend,
+        )
+
     # Methods implemented by backend
     # ------------------------------
     def triples(  # pylint: disable=redefined-builtin
         self,
         subject: "Optional[Union[str, Triple]]" = None,
         predicate: "Optional[str]" = None,
         object: "Optional[Union[str, Literal]]" = None,
@@ -347,19 +433,17 @@
     # Convenient methods
     # ------------------
     # These methods are modelled after rdflib and provide some convinient
     # interfaces to the triples(), add_triples() and remove() methods
     # implemented by all backends.
 
     @classmethod
-    def _get_backend(cls, backend: str):
+    def _get_backend(cls, backend: str, package: "Optional[str]" = None):
         """Returns the class implementing the given backend."""
-        module = import_module(
-            backend if "." in backend else f"tripper.backends.{backend}"
-        )
+        module = cls._load_backend(backend, package=package)
         return getattr(module, f"{backend.title()}Strategy")
 
     @classmethod
     def _check_backend_method(cls, backend: str, name: str):
         """Checks that `backend` has a method called `name`.
 
         Raises NotImplementedError if it hasn't.
@@ -375,48 +459,76 @@
         self._check_backend_method(self.backend_name, name)
 
     def add(self, triple: "Triple"):
         """Add `triple` to triplestore."""
         self.add_triples([triple])
 
     def value(  # pylint: disable=redefined-builtin
-        self, subject=None, predicate=None, object=None, default=None, any=False
-    ):
+        self,
+        subject=None,
+        predicate=None,
+        object=None,
+        default=None,
+        any=False,
+        lang=None,
+    ) -> "Union[str, Literal]":
         """Return the value for a pair of two criteria.
 
         Useful if one knows that there may only be one value.
 
         Parameters:
-            subject, predicate, object: Triple to match.
+            subject, predicate, object: Criteria to match. Two of these must
+                be provided.
             default: Value to return if no matches are found.
             any: If true, return any matching value, otherwise raise
                 UniquenessError.
+            lang: If provided, require that the value must be a localised
+                literal with the given language code.
+
+        Returns:
+            The value of the `subject`, `predicate` or `object` that is
+            None.
         """
         spo = (subject, predicate, object)
         if sum(iri is None for iri in spo) != 1:
             raise ValueError(
                 "Exactly one of `subject`, `predicate` or `object` must be None."
             )
 
-        triple = self.triples(spo)
-        try:
-            value = next(triple)
-        except StopIteration:
-            return default
-
         # Index of subject-predicate-object argument that is None
         (idx,) = [i for i, v in enumerate(spo) if v is None]
 
+        triples = self.triples(subject, predicate, object)
+        if lang:
+            first = None
+            if idx != 2:
+                raise ValueError("`object` must be None if `lang` is given")
+            for triple in triples:
+                value = triple[idx]
+                if isinstance(value, Literal) and value.lang == lang:
+                    if any:
+                        return value
+                    if first:
+                        raise UniquenessError("More than one match")
+                    first = value
+            if first is None:
+                return default
+        else:
+            try:
+                triple = next(triples)
+            except StopIteration:
+                return default
+
         try:
-            next(triple)
+            next(triples)
         except StopIteration:
-            return value[idx]
+            return triple[idx]
 
         if any:
-            return value[idx]
+            return triple[idx]
         raise UniquenessError("More than one match")
 
     def subjects(
         self, predicate=None, object=None  # pylint: disable=redefined-builtin
     ):
         """Returns a generator of subjects for given predicate and object."""
         for s, _, _ in self.triples(predicate=predicate, object=object):
@@ -455,15 +567,15 @@
     def set(self, triple):
         """Convenience method to update the value of object.
 
         Removes any existing triples for subject and predicate before adding
         the given `triple`.
         """
         s, p, _ = triple
-        self.remove((s, p, None))
+        self.remove(s, p)
         self.add(triple)
 
     def has(
         self, subject=None, predicate=None, object=None
     ):  # pylint: disable=redefined-builtin
         """Returns true if the triplestore has any triple matching
         the give subject, predicate and/or object."""
@@ -748,24 +860,283 @@
             self.add((func_iri, hasInput, iri))
         for iri in returns:
             self.add((iri, RDF.type, DataSet))
             self.add((func_iri, hasOutput, iri))
         if doc_string:
             self.add((func_iri, DCTERMS.description, en(doc_string)))
 
-        # self.add((func_iri, RDF.type, Task))
-        # self.add((func_iri, RDFS.label, en(name)))
-        # for parname, iri in pars:
-        #    par = f"{func_iri}_input_{parname}"
-        #    self.add((par, RDF.type, DataSet))
-        #    self.add((par, RDFS.label, en(parname)))
-        #    self.add((par, MAP.mapsTo, iri))
-        #    self.add((func_iri, hasInput, par))
-        # for i, iri in enumerate(returns):
-        #    val = f"{func_iri}_output{i+1}"
-        #    self.add((val, RDF.type, DataSet))
-        #    self.add((val, MAP.mapsTo, iri))
-        #    self.add((func_iri, hasOutput, val))
-        # if doc_string:
-        #    self.add((func_iri, DCTERMS.description, en(doc_string)))
-
         return func_iri
+
+    def add_interpolation_source(  # pylint: disable=too-many-arguments
+        self,
+        xcoord: str,
+        ycoord: str,
+        input_iri: str,
+        output_iri: str,
+        base_iri: "Optional[str]" = None,
+        standard: str = "emmo",
+        cost: "Optional[Union[float, Callable]]" = None,
+        left: "Optional[float]" = None,
+        right: "Optional[float]" = None,
+        period: "Optional[float]" = None,
+    ) -> str:
+        """Add data source to triplestore, such that it can be used to
+        transparently transform other data.
+
+        No data will be fetch before it is actually needed.
+
+        Parameters:
+            xcoord: IRI of data source with x-coordinates `xp`.  Must be
+                increasing if argument `period` is not specified. Otherwise,
+                `xp` is internally sorted after normalising the periodic
+                boundaries with ``xp = xp % period``.
+            ycoord: IRI of data source with y-coordinates `yp`.  Must have
+                the same length as `xp`.
+            input_iri: IRI of ontological concept that interpolation input-
+                data should be mapped to.
+            output_iri: IRI of ontological concept that interpolation output-
+                data should be mapped to.
+            base_iri: Base of the IRI representing the transformation in the
+                knowledge base.  Defaults to the base IRI of the triplestore.
+            standard: Name of ontology to use when describing the
+                transformation.  Valid values are:
+                - "emmo": Elementary Multiperspective Material Ontology (EMMO)
+                - "fno": Function Ontology (FnO)
+            cost: User-defined cost of following this mapping relation
+                represented as a float.  It may be given either as a
+                float or as a callable taking the same arguments as `func`
+                returning the cost as a float.
+            left: Value to return for `x < xp[0]`, default is `fp[0]`.
+            right: Value to return for `x > xp[-1]`, default is `fp[-1]`.
+            period: A period for the x-coordinates. This parameter allows the
+                proper interpolation of angular x-coordinates. Parameters
+                `left` and `right` are ignored if `period` is specified.
+
+        Returns:
+            transformation_iri: IRI of the added transformation.
+
+        Example:
+            Assume we have a data source that relates water temperature
+            (mapped to EX.Temp) to the amount of blue-green algae (mapped to
+            EX.AlgaeConc). By registering it with
+
+            >>> from tripper import Triplestore
+            >>> from tripper.mappings import Value
+
+            >>> ts = Triplestore(backend="rdflib")
+            >>> EX = ts.bind("ex", "http://example.com#")
+
+            # Add data source with temperatures
+            >>> temp = ts.add_data(
+            ...     lambda ret, conf, ts: Value([0., 20., 30., 37., 40.], unit="degC")
+            ... )
+
+            # Add data source with algae conc.
+            >>> conc = ts.add_data(
+            ...     lambda ret, conf, ts: Value([1e4, 1e6, 1e7, 1e8, 1e3], unit="")
+            ... )
+
+            >>> ts.add_interpolation_source(temp, conc, EX.Temp, EX.AlgaeConc)
+            ':func_3c61cfff'
+
+            we can now ask for the blue-green algae concentration in a fjord,
+            given we have a data source with the water temperature field in
+            the same fjord.
+            >>> ts.add_data(
+            ...     lambda ret, conf, ts: Value([10., 5., 0., 20.], unit="degC"),
+            ...     iri=EX.Temp,
+            ... )  # doctest: +ELLIPSIS
+            '_data_source_...'
+            >>> ts.map(EX.indv, EX.AlgaeConc)
+            >>> ts.get_value(EX.indv)  # should return the algae conc. field
+            array([ 505000.,  257500.,   10000., 1000000.])
+        """
+        try:
+            import numpy as np  # pylint: disable=import-outside-toplevel
+        except ImportError as exc:
+            raise RuntimeError(
+                "Triplestore.add_interpolation_source() requires numpy.\n"
+                "Install it with\n\n"
+                "    pip install numpy"
+            ) from exc
+
+        def func(x):
+            xp = self.get_value(xcoord)
+            fp = self.get_value(ycoord)
+            return np.interp(
+                x,
+                xp=xp,
+                fp=fp,
+                left=left,
+                right=right,
+                period=period,
+            )
+
+        return self.add_function(
+            func,
+            expects=input_iri,
+            returns=output_iri,
+            base_iri=base_iri,
+            standard=standard,
+            cost=cost,
+        )
+
+    def add_data(
+        self,
+        func: "Union[Callable, Literal]",
+        iri: "Optional[Union[str, Sequence]]" = None,
+        configurations: "Optional[dict]" = None,
+        base_iri: "Optional[str]" = None,
+        standard: str = "emmo",
+        cost: "Optional[Union[float, Callable]]" = None,
+    ) -> str:
+        """Register a data source to the triplestore.
+
+        Parameters:
+            func: A callable that should return the value of the registered
+                data source.  It is called with following protopype:
+
+                    func(returns, configurations, triplestore)
+
+                The returned value may in principle be of any type, but for
+                values with unit, it is recommended to return a
+                tripper.mappings.Value object.
+                Alternatively, `func` may also be a literal value.
+            iri: IRI of ontological concept or individual that the data
+                returned by `func` should be mapped to.  If `func` is a
+                callable and multiple values are returned, it may also be
+                given as a sequenceof IRIs.
+                If not given, it will default to a new blank node.
+            configurations: Configurations passed on to `func`.
+            base_iri: Base of the IRI representing the function in the
+                knowledge base.  Defaults to the base IRI of the triplestore.
+            standard: Name of ontological standard to use when describing the
+                function.  Valid values are:
+                - "emmo": Elementary Multiperspective Material Ontology (EMMO)
+                - "fno": Function Ontology (FnO)
+            cost: User-defined cost of following this mapping relation
+                represented as a float.  It may be given either as a
+                float or as a callable taking the same arguments as `func`
+                returning the cost as a float.
+
+        Returns:
+            IRI of data source.
+        """
+        if iri is None:
+            # pylint complains about uuid being unused if we make this an
+            # f-string
+            iri = "_bnode_" + str(uuid.uuid4())
+        data_source = "_data_source_" + random_string(8)
+        self.add((data_source, RDF.type, DataSource))
+
+        if isinstance(func, Literal):
+            self.add((data_source, hasDataValue, func))
+            if cost is not None:
+                self._add_cost(cost, data_source)
+            if isinstance(iri, str):
+                self.map(data_source, iri)
+            else:
+                raise TypeError("literal data can only have a single `iri`")
+
+        elif callable(func):
+
+            def fn():
+                return func(iri, configurations, self)
+
+            # Include data source IRI in documentation to ensure that the
+            # function_id of `fn()` will differ for different data sources...
+            fn.__doc__ = f"Function for data source: {data_source}.\n\n{func.__doc__}"
+            fn.__name__ = func.__name__
+
+            func_iri = self.add_function(
+                fn,
+                expects=(),
+                returns=iri,
+                base_iri=base_iri,
+                standard=standard,
+                cost=cost,
+            )
+            self.add((data_source, hasAccessFunction, func_iri))
+        else:
+            raise TypeError(f"`func` must be a callable or literal, got {type(func)}")
+
+        return data_source
+
+    def get_value(
+        self,
+        iri,
+        routeno=0,
+        unit: "Optional[str]" = None,
+        magnitude: bool = False,
+        quantity: "Optional[Any]" = None,
+        **kwargs,
+    ) -> "Value":
+        """Return the value of an individual.
+
+        Parameters:
+            iri: IRI of individual who's value we want to return.  IRI may
+                either refer to a data source or an individual mapped to
+                an ontological concept.
+            routeno: Number identifying the mapping route to apply for
+                retrieving the individual value in case IRI does not refer
+                to a data source.
+            unit: return the result in the given unit.
+                Implies `magnitude=True`.
+            magnitude: Whether to only return the magnitude of the evaluated
+                value (with no unit).
+            quantity: Quantity class to use for evaluation.  Defaults to pint.
+            kwargs: Additional arguments passed on to `mapping_routes()`.
+
+        Returns:
+            The value of the individual.
+        """
+        from tripper.mappings import (  # pylint: disable=import-outside-toplevel
+            Value,
+            mapping_routes,
+        )
+
+        if self.has(iri, RDF.type, DataSource):
+            # `iri` refer to a DataSource
+            if self.has(iri, hasDataValue):  # literal value
+                return Value(
+                    value=parse_literal(self.value(iri, hasDataValue)).to_python(),
+                    unit=parse_literal(self.value(iri, hasUnit)).to_python()
+                    if self.has(iri, hasUnit)
+                    else None,
+                    iri=self.value(iri, MAP.mapsTo),
+                    cost=parse_literal(self.value(iri, hasCost)).to_python()
+                    if self.has(iri, hasCost)
+                    else 0.0,
+                ).get_value(unit=unit, magnitude=magnitude, quantity=quantity)
+
+            if self.has(iri, hasAccessFunction):  # callable
+                func_iri = self.value(iri, hasAccessFunction)
+                func = self.function_repo[func_iri]
+                assert callable(func)  # nosec
+                retval = func()
+                if isinstance(retval, Value):
+                    return retval.get_value(
+                        unit=unit, magnitude=magnitude, quantity=quantity
+                    )
+                return retval
+
+            raise TriplestoreError(
+                f"data source {iri} has neither a 'hasDataValue' or a "
+                f"'hasAccessFunction' property"
+            )
+
+        # `iri` correspond to an individual mapped to an ontological concept.
+        # In this case we check if there exists a mapping route.
+        routes = mapping_routes(
+            target=iri,
+            sources=list(self.subjects(RDF.type, DataSource)),
+            triplestore=self,
+            **kwargs,
+        )
+        if isinstance(routes, Value):
+            return routes.get_value(unit=unit, magnitude=magnitude, quantity=quantity)
+        return routes.eval(
+            routeno=routeno,
+            unit=unit,
+            magnitude=magnitude,
+            quantity=quantity,
+        )
```

### Comparing `tripper-0.2.3/tripper/utils.py` & `tripper-0.2.4/tripper/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 """Utility functions."""
 # pylint: disable=invalid-name,redefined-builtin
 import datetime
 import hashlib
 import inspect
+import random
 import re
+import string
 from typing import TYPE_CHECKING
 
 from tripper.literal import Literal
 from tripper.namespace import XSD
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing import Any, Callable, Tuple, Union
 
     OptionalTriple = Tuple[
         Union[str, None], Union[str, None], Union[str, Literal, None]
     ]
     Triple = Tuple[str, str, Union[str, Literal]]
 
 
+__all__ = (
+    "infer_iri",
+    "split_iri",
+    "function_id",
+    "en",
+    "parse_literal",
+    "parse_object",
+    "as_python",
+    "check",
+    "random_string",
+)
+
+
 class UnusedArgumentWarning(Warning):
     """Argument is unused."""
 
 
 def infer_iri(obj):
     """Return IRI of the individual that stands for object `obj`."""
     if isinstance(obj, str):
@@ -78,16 +93,18 @@
 
     The returned object is a string of hexadecimal digits.
 
     `length` is the number of bytes in the returned checksum.  Since
     the current implementation is based on the shake_128 algorithm,
     it make no sense to set `length` larger than 32 bytes.
     """
+    source = inspect.getsource(func)
+    doc = func.__doc__ if func.__doc__ else ""
     return hashlib.shake_128(  # pylint: disable=too-many-function-args
-        inspect.getsource(func).encode()
+        (source + doc).encode()
     ).hexdigest(length)
 
 
 def en(value) -> "Literal":  # pylint: disable=invalid-name
     """Convenience function that returns value as a plain english literal.
 
     Equivalent to ``Literal(value, lang="en")``.
@@ -163,15 +180,15 @@
     """Applies heuristics to parse RDF object `obj` to an IRI or literal.
 
     The following heuristics is performed (in the given order):
     - If `obj` is a Literal, it is returned.
     - If `obj` is a string and
       - starts with "_:", it is assumed to be a blank node and returned.
       - starts with a scheme, it is asumed to be an IRI and returned.
-      - can be converted to a float, int or datetime, it is returned.
+      - can be converted to a float, int or datetime, it is returned
         converted to a literal of the corresponding type.
       - it is a valid n3 representation, return it as the given type.
       - otherwise, return it as a xsd:string literal.
     - Otherwise, raise an ValueError.
 
     Returns
         A string if `obj` is considered to be an IRI, otherwise a
@@ -191,20 +208,41 @@
             return Literal(obj, datatype=XSD.double)
         if check(datetime.datetime.fromisoformat, obj, ValueError):  #  datetime
             return Literal(obj, datatype=XSD.dateTime)
         return parse_literal(obj)
     raise ValueError("`obj` should be a literal or a string.")
 
 
+def as_python(value: "Any") -> "Any":
+    """Converts `value` to a native Python representation.
+
+    If `value` is a Literal, its Python representation will be returned.
+    If `value` is a string, it will first be converted to a Literal, before
+    its Python representation is returned.
+    Otherwise, `value` will be returned as-is.
+    """
+    if isinstance(value, Literal):
+        return value.to_python()
+    if isinstance(value, str):
+        return parse_literal(value).to_python()
+    return value
+
+
 def check(func: "Callable", s: str, exceptions) -> bool:
     """Help function that returns true if `func(s)` does not raise an exception.
 
     False is returned if `func(s)` raises an exception listed in `exceptions`.
     Otherwise the exception is propagated.
     """
-    # Note that the missing type hint on `exceptions` is deliberately, see
+    # Note that the missing type hint on `exceptions` is deliberate, see
     # https://peps.python.org/pep-0484/#exceptions
     try:
         func(s)
     except exceptions:
         return False
     return True
+
+
+def random_string(length=8):
+    """Return a random string of the given length."""
+    letters = string.ascii_letters + string.digits
+    return "".join(random.choice(letters) for i in range(length))  # nosec
```

### Comparing `tripper-0.2.3/PKG-INFO` & `tripper-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 Metadata-Version: 2.1
 Name: tripper
-Version: 0.2.3
+Version: 0.2.4
 Summary: A triplestore wrapper for Python.
 Keywords: triplestore,ontology,RDF
 Author-email: SINTEF <TEAM4.0@sintef.no>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Plugins
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Dist: typing-extensions ~=4.4 ; python_version<'3.8'
+Requires-Dist: typing-extensions ~=4.5; python_version<'3.8'
 Requires-Dist: mike ~=1.1 ; extra == "dev"
 Requires-Dist: mkdocs ~=1.4 ; extra == "dev"
 Requires-Dist: mkdocs-awesome-pages-plugin ~=2.8 ; extra == "dev"
-Requires-Dist: mkdocs-material ~=9.0 ; extra == "dev"
+Requires-Dist: mkdocs-material ~=9.1 ; extra == "dev"
 Requires-Dist: mkdocstrings[python-legacy] ~=0.20.0 ; extra == "dev"
 Requires-Dist: pre-commit ~=2.21 ; extra == "dev"
 Requires-Dist: pylint ~=2.13 ; extra == "dev"
 Requires-Dist: pytest ~=7.2 ; extra == "dev"
 Requires-Dist: pytest-cov ~=4.0 ; extra == "dev"
-Requires-Dist: EMMOntoPy ~=0.4 ; extra == "dev"
-Requires-Dist: rdflib ~=6.2 ; extra == "dev"
+Requires-Dist: EMMOntoPy ~=0.5 ; extra == "dev"
+Requires-Dist: rdflib ~=6.3 ; extra == "dev"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "dev"
-Requires-Dist: DLite-Python >=0.3.16,<1 ; extra == "dev"
+Requires-Dist: DLite-Python >=0.3.18,<1 ; extra == "dev"
 Requires-Dist: mike ~=1.1 ; extra == "docs"
 Requires-Dist: mkdocs ~=1.4 ; extra == "docs"
 Requires-Dist: mkdocs-awesome-pages-plugin ~=2.8 ; extra == "docs"
-Requires-Dist: mkdocs-material ~=9.0 ; extra == "docs"
+Requires-Dist: mkdocs-material ~=9.1 ; extra == "docs"
 Requires-Dist: mkdocstrings[python-legacy] ~=0.20.0 ; extra == "docs"
-Requires-Dist: EMMOntoPy ~=0.4 ; extra == "docs"
-Requires-Dist: rdflib ~=6.2 ; extra == "docs"
+Requires-Dist: EMMOntoPy ~=0.5 ; extra == "docs"
+Requires-Dist: rdflib ~=6.3 ; extra == "docs"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "docs"
-Requires-Dist: DLite-Python >=0.3.16,<1 ; extra == "docs"
+Requires-Dist: DLite-Python >=0.3.18,<1 ; extra == "docs"
 Requires-Dist: pre-commit ~=2.21 ; extra == "pre-commit"
 Requires-Dist: pylint ~=2.13 ; extra == "pre-commit"
 Requires-Dist: pytest ~=7.2 ; extra == "testing"
 Requires-Dist: pytest-cov ~=4.0 ; extra == "testing"
-Requires-Dist: EMMOntoPy ~=0.4 ; extra == "testing"
-Requires-Dist: rdflib ~=6.2 ; extra == "testing"
+Requires-Dist: EMMOntoPy ~=0.5 ; extra == "testing"
+Requires-Dist: rdflib ~=6.3 ; extra == "testing"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "testing"
-Requires-Dist: DLite-Python >=0.3.16,<1 ; extra == "testing"
+Requires-Dist: DLite-Python >=0.3.18,<1 ; extra == "testing"
 Project-URL: Changelog, https://github.com/EMMC-ASBL/tripper/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://EMMC-ASBL.github.io/tripper
 Project-URL: Home, https://github.com/EMMC-ASBL/tripper
 Project-URL: Issue Tracker, https://github.com/EMMC-ASBL/tripper/issues
 Project-URL: Package, https://pypi.org/project/tripper
 Project-URL: Source, https://github.com/EMMC-ASBL/tripper
 Provides-Extra: dev
@@ -91,16 +89,17 @@
 
 A triplestore wrapper is created with the [`tripper.Triplestore`][Triplestore] class.
 
 
 
 Documentation
 -------------
-* Getting started: Take a look at the [tutorial](docs/tutorial.md).
-* Reference manual: [API Reference]
+* Getting started: See the [tutorial](docs/tutorial.md)
+* [Discovery of custom backends](docs/backend_discovery.md)
+* [Reference manual]
 
 
 Installation
 ------------
 Tripper has by itself no dependencies outside the standard library, but the triplestore backends may have specific dependencies.
 
 
@@ -117,12 +116,12 @@
 SINTEF.
 
 
 
 
 [rdflib]: https://rdflib.readthedocs.io/en/stable/
 [PyPI]: https://pypi.org/project/tripper
-[API Reference]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/
+[Reference manual]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/
 [Literal]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Literal
 [Namespace]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Namespace
 [Triplestore]: https://emmc-asbl.github.io/tripper/latest/api_reference/triplestore/#tripper.triplestore.Triplestore
```

