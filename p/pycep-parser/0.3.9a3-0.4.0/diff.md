# Comparing `tmp/pycep-parser-0.3.9a3.tar.gz` & `tmp/pycep_parser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycep-parser-0.3.9a3.tar", max compression
+gzip compressed data, was "pycep_parser-0.4.0.tar", max compression
```

## Comparing `pycep-parser-0.3.9a3.tar` & `pycep_parser-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    10834 2022-08-30 20:23:05.548242 pycep-parser-0.3.9a3/LICENSE
--rw-r--r--   0        0        0     1315 2022-08-30 20:23:05.548242 pycep-parser-0.3.9a3/README.md
--rw-r--r--   0        0        0       57 2022-08-30 20:23:05.552242 pycep-parser-0.3.9a3/pycep/__init__.py
--rw-r--r--   0        0        0    12165 2022-08-30 20:23:05.552242 pycep-parser-0.3.9a3/pycep/bicep.lark
--rw-r--r--   0        0        0     1854 2022-08-30 20:23:05.552242 pycep-parser-0.3.9a3/pycep/main.py
--rw-r--r--   0        0        0        0 2022-08-30 20:23:05.552242 pycep-parser-0.3.9a3/pycep/py.typed
--rw-r--r--   0        0        0    54908 2022-08-30 20:23:05.552242 pycep-parser-0.3.9a3/pycep/transformer.py
--rw-r--r--   0        0        0    23529 2022-08-30 20:23:05.552242 pycep-parser-0.3.9a3/pycep/typing.py
--rw-r--r--   0        0        0      274 2022-08-30 20:23:05.552242 pycep-parser-0.3.9a3/pycep/validator.py
--rw-r--r--   0        0        0     1648 2022-08-30 20:23:22.136511 pycep-parser-0.3.9a3/pyproject.toml
--rw-r--r--   0        0        0     2176 2022-08-30 20:23:23.913016 pycep-parser-0.3.9a3/setup.py
--rw-r--r--   0        0        0     2315 2022-08-30 20:23:23.913381 pycep-parser-0.3.9a3/PKG-INFO
+-rw-r--r--   0        0        0    10834 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1511 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/README.md
+-rw-r--r--   0        0        0       57 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/__init__.py
+-rw-r--r--   0        0        0    12350 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/bicep.lark
+-rw-r--r--   0        0        0     1854 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/main.py
+-rw-r--r--   0        0        0        0 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/py.typed
+-rw-r--r--   0        0        0    55529 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/transformer.py
+-rw-r--r--   0        0        0    23875 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/typing.py
+-rw-r--r--   0        0        0      274 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/validator.py
+-rw-r--r--   0        0        0     1459 2023-04-30 03:43:08.180629 pycep_parser-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 pycep_parser-0.4.0/PKG-INFO
```

### Comparing `pycep-parser-0.3.9a3/LICENSE` & `pycep_parser-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycep-parser-0.3.9a3/README.md` & `pycep_parser-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pycep
 
 [![Build Status](https://github.com/gruebel/pycep/workflows/CI/badge.svg)](https://github.com/gruebel/pycep/actions)
 [![codecov](https://codecov.io/gh/gruebel/pycep/branch/master/graph/badge.svg?token=49WHVYGE1D)](https://codecov.io/gh/gruebel/pycep)
 [![PyPI](https://img.shields.io/pypi/v/pycep-parser)](https://pypi.org/project/pycep-parser/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pycep-parser)](https://github.com/gruebel/pycep)
 ![CodeQL](https://github.com/gruebel/pycep/workflows/CodeQL/badge.svg)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/gruebel/pycep/badge)](https://api.securityscorecards.dev/projects/github.com/gruebel/pycep)
 
 A parser for [Azure Bicep](https://github.com/Azure/bicep) files leveraging [Lark](https://github.com/lark-parser/lark).
 
 ## Getting Started
 
 ### Requirements
 
@@ -29,14 +30,15 @@
 
 ### Functions
 - [x] Any
 - [ ] Array (in progress)
 - [x] Date
 - [x] Deployment
 - [x] File
+- [ ] Lambda (in progress)
 - [x] Logical
 - [x] Numeric
 - [x] Object
 - [x] Resource
 - [x] Scope
 - [x] String
```

### Comparing `pycep-parser-0.3.9a3/pycep/bicep.lark` & `pycep_parser-0.4.0/pycep/bicep.lark`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
       | INDEXED                     -> string
       | MULTI_LINE_STRING           -> multi_line_string
       | array
       | object
       | function
       | operator
 
-?value_brackets: value
-               | "(" value ")"
+?value_brackets: (value | "(" value ")") "!"?
 
 // element values
 
 ?var_value: value_brackets | loop
 
 ?output_value: value_brackets | loop
 
@@ -69,21 +68,21 @@
 
 pair: key ":" (value_brackets | loop)
 
 !key: "resource" | quoted_string
 
 // decorators
 
-decorator: ("@" (deco_allowed | deco_batch | deco_description | deco_min_len | deco_max_len | deco_min_val | deco_max_val | deco_metadata | deco_secure) _CPP_COMMENT_NL)+
+decorator: ("@" "sys."? (deco_allowed | deco_batch | deco_description | deco_min_len | deco_max_len | deco_min_val | deco_max_val | deco_metadata | deco_secure) _CPP_COMMENT_NL~0..5)+
 
 deco_allowed: "allowed" "(" array ")"
 
 deco_batch: "batchSize" "(" /\d+/ ")"
 
-deco_description: "description" "(" QUOTED_INTERPOLATION ")"
+deco_description: "description" "(" (QUOTED_INTERPOLATION | MULTI_LINE_STRING) ")"
 
 deco_min_len: "minLength" "(" /\d+/ ")"
 
 deco_max_len: "maxLength" "(" /\d+/ ")"
 
 deco_min_val: "minValue" "(" /-?\d+/ ")"
 
@@ -91,16 +90,16 @@
 
 deco_metadata: "metadata" "(" object ")"
 
 deco_secure: "secure" "(" ")"
 
 // functions
 
-function: function_any | function_array | function_date | function_deployment | function_file | function_logical
-        | function_numeric | function_object | function_resource | function_scope | function_string
+function: function_any | function_array | function_date | function_deployment | function_file | function_lambda
+        | function_logical | function_numeric | function_object | function_resource | function_scope | function_string
 
 // functions - any
 
 ?function_any: any_func
 
 any_func: ("any" | "sys.any") "(" value_brackets ")" ["." STRING]
 
@@ -167,14 +166,20 @@
 
 load_file_as_base64: ("loadFileAsBase64" | "sys.loadFileAsBase64") "(" value_brackets ")"
 
 load_json_content: ("loadJsonContent" | "sys.loadJsonContent") "(" value_brackets ["," value_brackets ["," value_brackets]] ")" [["[" STRING "]"] "." (STRING | INDEXED)]
 
 load_text_content: ("loadTextContent" | "sys.loadTextContent") "(" value_brackets ["," value_brackets] ")"
 
+// functions - lambda
+
+?function_lambda: filter
+
+filter: ("filter" | "sys.filter") "(" value_brackets "," STRING "=>" value_brackets ")"
+
 // functions - logical
 
 ?function_logical: bool_func
 
 bool_func: ("bool" | "sys.bool") "(" value_brackets ")"
 
 // functions - numeric
@@ -342,15 +347,15 @@
 
 // Terms
 
 EXISTING: "existing"
 
 STRING: /[a-zA-Z_](::|[\w_.])*/
 QUOTED_STRING: "'" STRING "'"
-INDEXED: /(?=[\w][\w_.]+(.(get|list)[a-zA-Z]*\(('[\w-]+'|[\w.]+)?\)|[\[\]])+)(.(get|list)[a-zA-Z]*\(('[\w-]+'|[\w.]+)?\)|\[[\w\[\]_().']+\]|[\w_\-\/.,'= ])+/
+INDEXED: /(?=[\w][\w_.]+(.(get|list)[a-zA-Z]*\(('[\w-]+'|[\w.]+)?\)|[\[\]])+)(.(get|list)[a-zA-Z]*\(('[\w-]+'|[\w.]+)?\)|\[[\w\[\]_().']+\]!?|[\w_\-\/.,'= ])+/
 QUOTED_INTERPOLATION: /(?!.*''')'(\${(?:[^}'{]+|(?R))*+}|\\'|[^'])*'/
 
 MULTI_LINE_STRING: "'''" (/.*?/ | NEWLINE)+ "'''"
 
 _NEWLINE: NEWLINE
 _CPP_COMMENT_NL: [CPP_COMMENT] NEWLINE
```

### Comparing `pycep-parser-0.3.9a3/pycep/main.py` & `pycep_parser-0.4.0/pycep/main.py`

 * *Files identical despite different names*

### Comparing `pycep-parser-0.3.9a3/pycep/transformer.py` & `pycep_parser-0.4.0/pycep/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 from lark import Token, Transformer, v_args
 from lark.tree import Meta
 from typing_extensions import Literal
 
 from pycep import typing as pycep_typing
 
-BICEP_REGISTRY_ALIAS_PATTERN = re.compile(r"br/(?P<alias>[\w]+):(?P<path>[\w/\-]+):(?P<tag>[\w.\-]+)")
+BICEP_REGISTRY_ALIAS_PATTERN = re.compile(r"br/(?P<alias>[\w]+):(?P<path>[\w/\-.]+):(?P<tag>[\w.\-]+)")
 PUBLIC_BICEP_REGISTRY_PATTERN = re.compile(r"br:mcr\.microsoft\.com/(?P<path>[\w/\-]+):(?P<tag>[\w.\-]+)")
 PRIVATE_BICEP_REGISTRY_PATTERN = re.compile(
-    r"br:(?P<registry_name>\w+)\.azurecr\.io/(?P<path>[\w/\-]+):(?P<tag>[\w.\-]+)"
+    r"br:(?P<registry_name>\w+)\.azurecr\.io/(?P<path>[\w/\-.]+):(?P<tag>[\w.\-]+)"
 )
 TEMPLATE_SPEC_ALIAS_PATTERN = re.compile(r"ts/(?P<alias>[\w]+):(?P<path>[\w/\-]+):(?P<tag>[\w.\-]+)")
 TEMPLATE_SPEC_PATTERN = re.compile(
     r"ts:(?P<sub_id>[\d\-]+)/(?P<rg_id>[\w._\-()]+)/(?P<name>[\w.\-]+):(?P<version>[\w.\-]+)"
 )
 
 VALID_TARGET_SCOPES = {"resourceGroup", "subscription", "managementGroup", "tenant"}
@@ -371,21 +371,21 @@
                 "item_name": str(item_name) if item_name else None,
                 "index_name": str(idx_name),
                 "start_index": start_idx,
                 "count": count,
             },
         }
 
-    def loop_array(self, args: tuple[Token, Token]) -> pycep_typing.LoopArray:
+    def loop_array(self, args: tuple[Token, pycep_typing.PossibleValue]) -> pycep_typing.LoopArray:
         item_name, array_name = args
         return {
             "type": "array",
             "detail": {
                 "item_name": str(item_name),
-                "array_name": str(array_name),
+                "array_name": array_name,
             },
         }
 
     def loop_array_index(self, args: tuple[Token, Token, Token]) -> pycep_typing.LoopArrayIndex:
         item_name, idx_name, array_name = args
         return {
             "type": "array_index",
@@ -792,14 +792,32 @@
             "parameters": {
                 "file_path": args[0],
             },
         }
 
     ####################
     #
+    # functions - lambda
+    #
+    ####################
+
+    def filter(self, args: tuple[pycep_typing.PossibleValue, Token, pycep_typing.PossibleValue]) -> pycep_typing.Filter:
+        input_array, input_element, expression = args
+
+        return {
+            "type": "filter",
+            "parameters": {
+                "input_array": input_array,
+                "input_element": str(input_element),
+                "expression": expression,
+            },
+        }
+
+    ####################
+    #
     # functions - logical
     #
     ####################
 
     def bool_func(self, args: tuple[pycep_typing.PossibleValue]) -> pycep_typing.BoolFunc:
         return {
             "type": "bool",
@@ -1713,11 +1731,14 @@
             )
 
     def transform_string_token(self, value: Token) -> str | BicepElement:
         """Transforms string typed Token to a `str` or `BicepElement`.
 
         Additionally, removes surrounding single quotes.
         """
+        if value.type == "MULTI_LINE_STRING":
+            return self.multi_line_string((value,))
+
         if value.type not in ("QUOTED_STRING", "QUOTED_INTERPOLATION"):
             return BicepElement(value)
 
         return str(value)[1:-1]
```

### Comparing `pycep-parser-0.3.9a3/pycep/typing.py` & `pycep_parser-0.4.0/pycep/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 AnyFunctions: TypeAlias = "AnyFunc"
 ArrayFunctions: TypeAlias = (
     "Array | Concat | Contains | Empty | First | Intersection | Last | Length | Max | Min | Skip | Take | UnionFunc"
 )
 DateFunctions: TypeAlias = "DateTimeAdd | DateTimeFromEpoch | DateTimeToEpoch | UtcNow"
 DeploymentFunctions: TypeAlias = "Deployment | Environment"
 FileFunctions: TypeAlias = "LoadFileAsBase64 | LoadJsonContent | LoadTextContent"
+LambdaFunctions: TypeAlias = "Filter"
 LogicalFunctions: TypeAlias = "BoolFunc"
 NumericFunctions: TypeAlias = "IntFunc"
 ObjectFunctions: TypeAlias = "Json"
 ResourceFunctions: TypeAlias = "ExtensionResourceId | ListKeys | ManagementGroupResourceId | PickZones | Reference | ResourceId | SubscriptionResourceId | TenantResourceId"
 ScopeFunctions: TypeAlias = "ManagementGroup | ResourceGroup | Subscription | Tenant"
 StringFunctions: TypeAlias = "Base64 | Base64ToJson | Base64ToString | DataUri | DataUriToString | EndsWith | Format | Guid | IndexOf | LastIndexOf | NewGuid | Split | StartsWith | String | Substring | ToLower | ToUpper | Trim | UniqueString | Uri | UriComponent | UriComponentToString"
-Functions: TypeAlias = "AnyFunctions | ArrayFunctions | DateFunctions | DeploymentFunctions | FileFunctions | LogicalFunctions | NumericFunctions | ObjectFunctions | ResourceFunctions | ScopeFunctions | StringFunctions"
+Functions: TypeAlias = "AnyFunctions | ArrayFunctions | DateFunctions | DeploymentFunctions | FileFunctions | LambdaFunctions | LogicalFunctions | NumericFunctions | ObjectFunctions | ResourceFunctions | ScopeFunctions | StringFunctions"
 
 
 ####################
 #
 # Elements
 #
 ####################
@@ -242,15 +243,15 @@
 class LoopRange(TypedDict):
     type: Literal["range"]
     detail: _LoopRangeDetail
 
 
 class _LoopArrayDetail(TypedDict):
     item_name: str
-    array_name: str
+    array_name: PossibleValue
 
 
 class LoopArray(TypedDict):
     type: Literal["array"]
     detail: _LoopArrayDetail
 
 
@@ -578,14 +579,32 @@
 class LoadTextContent(TypedDict):
     type: Literal["load_text_content"]
     parameters: _LoadTextContentParameters
 
 
 ####################
 #
+# functions - lambda
+#
+####################
+
+
+class _FilterParameters(TypedDict):
+    input_array: PossibleValue
+    input_element: str
+    expression: PossibleValue
+
+
+class Filter(TypedDict):
+    type: Literal["filter"]
+    parameters: _FilterParameters
+
+
+####################
+#
 # functions - logical
 #
 ####################
 
 
 class BoolFunc(TypedDict):
     type: Literal["bool"]
```

### Comparing `pycep-parser-0.3.9a3/pyproject.toml` & `pycep_parser-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycep-parser"
-version = "0.3.9-alpha.3"
+version = "0.4.0"
 description = "A Python based Bicep parser"
 authors = ["Anton Grübel <anton.gruebel@gmail.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 
 packages = [
@@ -20,39 +20,30 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 lark = ">=1.1.2"
 regex = ">=2022.1.18"
 typing-extensions = ">=3.10.0"
 importlib-resources = {version = ">=2.0.0", python = "<3.9"}
 
 [tool.poetry.dev-dependencies]
 assertpy = "^1.1"
-bandit = "^1.7.4"
-black = "^22.6.0"
-flake8 = "^5.0.4"
-flake8-bugbear = "^22.8.23"
-flake8-builtins = "^1.5.3"
-flake8-comprehensions = "^3.10.0"
-flake8-pytest-style = "^1.6.0"
-flake8-typing-imports = "^1.13.0"
-isort = "^5.10.1"
-mypy = "^0.971"
-pep8-naming = "^0.13.2"
-pre-commit = "^2.20.0"
-pytest = "^7.1.2"
+mypy = "^1.2.0"
+pre-commit = "^2.21.0"  # v3 needs Python 3.8
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 recursive = true
```

### Comparing `pycep-parser-0.3.9a3/PKG-INFO` & `pycep_parser-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 Metadata-Version: 2.1
 Name: pycep-parser
-Version: 0.3.9a3
+Version: 0.4.0
 Summary: A Python based Bicep parser
 Home-page: https://github.com/gruebel/pycep
 License: Apache-2.0
 Keywords: bicep,parser,lark
 Author: Anton Grübel
 Author-email: anton.gruebel@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
-Requires-Dist: importlib-resources (>=2.0.0); python_version < "3.9"
+Requires-Dist: importlib-resources (>=2.0.0) ; python_version < "3.9"
 Requires-Dist: lark (>=1.1.2)
 Requires-Dist: regex (>=2022.1.18)
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Repository, https://github.com/gruebel/pycep
 Description-Content-Type: text/markdown
 
 # pycep
 
 [![Build Status](https://github.com/gruebel/pycep/workflows/CI/badge.svg)](https://github.com/gruebel/pycep/actions)
 [![codecov](https://codecov.io/gh/gruebel/pycep/branch/master/graph/badge.svg?token=49WHVYGE1D)](https://codecov.io/gh/gruebel/pycep)
 [![PyPI](https://img.shields.io/pypi/v/pycep-parser)](https://pypi.org/project/pycep-parser/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pycep-parser)](https://github.com/gruebel/pycep)
 ![CodeQL](https://github.com/gruebel/pycep/workflows/CodeQL/badge.svg)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/gruebel/pycep/badge)](https://api.securityscorecards.dev/projects/github.com/gruebel/pycep)
 
 A parser for [Azure Bicep](https://github.com/Azure/bicep) files leveraging [Lark](https://github.com/lark-parser/lark).
 
 ## Getting Started
 
 ### Requirements
 
@@ -55,14 +62,15 @@
 
 ### Functions
 - [x] Any
 - [ ] Array (in progress)
 - [x] Date
 - [x] Deployment
 - [x] File
+- [ ] Lambda (in progress)
 - [x] Logical
 - [x] Numeric
 - [x] Object
 - [x] Resource
 - [x] Scope
 - [x] String
```

