# Comparing `tmp/balcony-0.0.86.tar.gz` & `tmp/balcony-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.0.86.tar", max compression
+gzip compressed data, was "balcony-0.0.9.tar", max compression
```

## Comparing `balcony-0.0.86.tar` & `balcony-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,29 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.0.86/LICENSE
--rw-r--r--   0        0        0     1865 2023-04-30 19:22:24.440612 balcony-0.0.86/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.0.86/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.0.86/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.0.86/balcony/aws.py
--rw-r--r--   0        0        0    11892 2023-04-21 17:50:16.401554 balcony-0.0.86/balcony/botocore_utils.py
--rw-r--r--   0        0        0    14182 2023-04-30 21:17:49.283350 balcony-0.0.86/balcony/cli.py
--rw-r--r--   0        0        0     2978 2023-04-30 21:07:33.646010 balcony-0.0.86/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.0.86/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.0.86/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.0.86/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.0.86/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.0.86/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.0.86/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.0.86/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.0.86/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.0.86/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.0.86/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.0.86/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.0.86/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.0.86/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.0.86/balcony/errors.py
--rw-r--r--   0        0        0    48117 2023-04-29 22:05:26.837497 balcony-0.0.86/balcony/nodes.py
--rw-r--r--   0        0        0    17071 2023-04-16 19:18:28.505235 balcony-0.0.86/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.0.86/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.0.86/balcony/relations.py
--rw-r--r--   0        0        0     2533 2023-04-21 19:19:57.046512 balcony-0.0.86/balcony/test.py
--rw-r--r--   0        0        0     4224 2023-04-21 17:54:28.473417 balcony-0.0.86/balcony/utils.py
--rw-r--r--   0        0        0     2735 2023-04-15 19:57:02.419610 balcony-0.0.86/balcony/yaml_config.py
--rw-r--r--   0        0        0     2049 2023-04-29 22:16:26.774034 balcony-0.0.86/balcony/yaml_validators.py
--rw-r--r--   0        0        0      664 2023-04-30 21:19:14.586509 balcony-0.0.86/pyproject.toml
--rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 balcony-0.0.86/setup.py
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 balcony-0.0.86/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.0.9/LICENSE
+-rw-r--r--   0        0        0      353 2022-09-26 12:41:48.924073 balcony-0.0.9/README.md
+-rw-r--r--   0        0        0      286 2022-10-09 10:37:47.142816 balcony-0.0.9/balcony/__init__.py
+-rw-r--r--   0        0        0       53 2022-10-04 08:01:49.289224 balcony-0.0.9/balcony/__main__.py
+-rw-r--r--   0        0        0     1432 2022-10-09 09:50:45.143185 balcony-0.0.9/balcony/app.py
+-rw-r--r--   0        0        0    10347 2022-10-08 07:04:48.840377 balcony-0.0.9/balcony/botocore_utils.py
+-rw-r--r--   0        0        0     7724 2022-10-09 10:41:41.880849 balcony-0.0.9/balcony/cli.py
+-rw-r--r--   0        0        0      264 2022-09-30 20:25:42.597791 balcony-0.0.9/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0     1444 2022-09-29 13:15:21.107762 balcony-0.0.9/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     1095 2022-10-09 17:51:42.748364 balcony-0.0.9/balcony/custom_nodes/ec2.py
+-rw-r--r--   0        0        0     2530 2022-09-29 13:15:21.126367 balcony-0.0.9/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     3140 2022-10-10 07:22:17.872579 balcony-0.0.9/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0     1018 2022-09-29 19:23:48.871446 balcony-0.0.9/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1410 2022-10-01 08:48:13.809464 balcony-0.0.9/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0     2214 2022-09-30 20:31:15.045592 balcony-0.0.9/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0       26 2022-10-04 07:57:08.884233 balcony-0.0.9/balcony/exceptions.py
+-rw-r--r--   0        0        0     2011 2022-10-09 10:37:09.474616 balcony-0.0.9/balcony/factories.py
+-rw-r--r--   0        0        0     1261 2022-09-26 08:05:59.761176 balcony-0.0.9/balcony/logs.py
+-rw-r--r--   0        0        0     4012 2022-10-09 11:11:51.901472 balcony-0.0.9/balcony/main.py
+-rw-r--r--   0        0        0    33760 2022-10-09 10:52:29.206820 balcony-0.0.9/balcony/nodes.py
+-rw-r--r--   0        0        0    20844 2022-10-11 20:37:36.250496 balcony-0.0.9/balcony/reader.py
+-rw-r--r--   0        0        0     6560 2022-10-09 10:03:48.761239 balcony-0.0.9/balcony/registries.py
+-rw-r--r--   0        0        0     9472 2022-10-09 17:45:39.425216 balcony-0.0.9/balcony/relations.py
+-rw-r--r--   0        0        0      386 2022-10-13 07:07:22.872196 balcony-0.0.9/balcony/rrr.py
+-rw-r--r--   0        0        0      377 2022-10-09 17:48:27.201727 balcony-0.0.9/balcony/settings.py
+-rw-r--r--   0        0        0     3231 2022-10-08 07:24:30.953384 balcony-0.0.9/balcony/utils.py
+-rw-r--r--   0        0        0      521 2022-10-13 07:16:58.915722 balcony-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 balcony-0.0.9/setup.py
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 balcony-0.0.9/PKG-INFO
```

### Comparing `balcony-0.0.86/LICENSE` & `balcony-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.0.86/balcony/botocore_utils.py` & `balcony-0.0.9/balcony/botocore_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,39 @@
-from utils import icompare_two_camel_case_words
-from config import get_rich_console
-
+from functools import lru_cache
 from typing import List, Union
 from botocore.model import Shape, DenormalizedStructureBuilder, OperationModel
-from rich.markup import escape
-import re
+
+try:
+    from .utils import icompare_two_camel_case_words
+    from .logs import get_rich_console
+except ImportError:
+    from utils import icompare_two_camel_case_words
+    from logs import get_rich_console
+
+
+
 from collections import namedtuple
+from rich.text import Text
 from rich.tree import Tree
+from rich.layout import Layout
+ShapeAndTargetPath = namedtuple('ShapeAndTargetPath', ['shape', 'target_path'])
 
-ShapeAndTargetPath = namedtuple("ShapeAndTargetPath", ["shape", "target_path"])
-
-UNWANTED_SHAPE_NAMES = ("String", "DateTime", "Name", "Id", "Arn", "__string")
+UNWANTED_SHAPE_NAMES = ('String', 'DateTime', 'Name', 'Id', 'Arn', '__string')
 UNWANTED_SHAPE_NAMES_LOWERED = [_.lower() for _ in UNWANTED_SHAPE_NAMES]
 SHAPE_SCALAR_TYPES = DenormalizedStructureBuilder.SCALAR_TYPES
-_MAX_ALLOWED_RECURSION = 10
-SHAPE_COLLECTION_TYPES = ("structure", "list", "map")
-READ_ONLY_VERBS = ("Describe", "List", "Get")
-IDENTIFIER_NAMES = (
-    "arn",
-    "id",
-    "name",
-    "arns",
-    "ids",
-    "names",
-    "identifier",
-    "identifiers",
-    "number",
-    "url",
-)
-
-# shape_resolver can't find the reference of BLACKLISTED_SHAPE_NAMES, so they're ignored
-BLACKLISTED_SHAPE_NAMES = (
-    "ComponentChildList",
-    "FirewallManagerRuleGroups",
-    "Rules",
-    "HeaderNames",  # noqa
-    "ExcludedRules",
-    "CountryCodes",
-    "CookieNames",
-    "TextTransformations",
-    "ComponentSummaryList",  # noqa
-    "AnomalyMonitors",
-    "ConfigurationList",
-    "HandshakeResources",
-    "JsonPointerPaths",  # noqa
-    "AdministrativeActions",
-    "DataValueList",
-    "ThemeValuesList",
-    "Expression",
-    "Expressions",
-    "CostCategoryRulesList",
-    "GetCostAndUsageRequest",
-    "GetCostAndUsageWithResourcesRequest",
-    "GetAnomaliesRequest",
-    "InventoryAggregator",
-    "OpsFilter",
-    "OpsAggregator",
-    "QueryStagePlanNodes",
-    "QueryStagePlanNode",
-    "QueryStage",
-    "ElicitSubSlot",
-    "DialogAction"
-)  # noqa
-# regex expr for removing html caret tags
-HTML_CLEANER_REGEX = re.compile("<.*?>|&([a-z0-9]+|#[0-9]{1,6}|#x[0-9a-f]{1,6});")
+SHAPE_COLLECTION_TYPES = ('structure', 'list','map')
+READ_ONLY_VERBS = ('Describe', 'List', 'Get')
+IDENTIFIER_NAMES = ('arn', 'id', 'name', 'arns', 'ids',
+                    'names', 'identifier', 'identifiers', 'number', 'url')
+BLACKLISTED_SHAPE_NAMES = ('ComponentChildList','FirewallManagerRuleGroups', 'Rules','HeaderNames', 'ExcludedRules', 'CountryCodes', 'CookieNames', 'TextTransformations', 'ComponentSummaryList','AnomalyMonitors','ConfigurationList','HandshakeResources','JsonPointerPaths','AdministrativeActions','DataValueList','ThemeValuesList','Expressions','CostCategoryRulesList')
 
 console = get_rich_console()
 
-
-def find_key_in_dict_keys(key: str, dict_keys: Union[list, dict]) -> str:
-    """Case insensitive search for a `key` in a `list` or `dict.keys()`.
-    Returns the existing key.
+def find_key_in_dict_keys(key:str, dict_keys: Union[list, dict]) -> str:
+    """Case insensitive search for a `key` in a `list` or `dict.keys()`. 
 
     Args:
         key (str): Search case insensively for
         dict_keys (Union[list, dict]): In a list or keys of dictionary
 
     Returns:
         str: Found key that case insensively matches the given key.
@@ -83,17 +42,16 @@
     if type(dict_keys) == dict:
         dict_keys_list = dict_keys.keys()
     for dict_key in dict_keys_list:
         if key.lower() == dict_key.lower():
             return dict_key
     return False
 
-
-def ifind_key_in_dict_keys(key: str, dict_keys: Union[list, dict]) -> str:
-    """Case insensitive search for a `key` in a `list` or `dict.keys()`.
+def ifind_key_in_dict_keys(key:str, dict_keys: Union[list, dict]) -> str:
+    """Case insensitive search for a `key` in a `list` or `dict.keys()`. 
 
     Args:
         key (str): Search case insensively for
         dict_keys (Union[list, dict]): In a list or keys of dictionary
 
     Returns:
         str: Found key that case insensively matches the given key.
@@ -102,266 +60,211 @@
     if type(dict_keys) == dict:
         dict_keys_list = dict_keys.keys()
     for dict_key in dict_keys_list:
         if icompare_two_camel_case_words(key, dict_key):
             return dict_key
     return False
 
-
 def get_max_results_value_from_shape(input_shape: Shape) -> int:
     """Finds the `MaxResults` highest value for an input shape.
 
     Args:
         input_shape (Shape): Input shape of an operation. Generally postfixed with `Request`.
 
     Returns:
         int: `MaxResults` highest value if found in the Shape definition
     """
-    flat_shapes_and_target_paths = (
-        flatten_shape_to_its_non_collection_shape_and_target_paths(input_shape)
-    )
+    flat_shapes_and_target_paths = flatten_shape_to_its_non_collection_shape_and_target_paths(input_shape)
     flat_members = [_.shape for _ in flat_shapes_and_target_paths]
+    result = False
     for member_shape in flat_members:
-        shape_key_name = getattr(member_shape, "key_name", False)
-        is_key_name_maxresults = shape_key_name and (
-            shape_key_name.lower() == "maxresults"
-        )
+        shape_key_name = getattr(member_shape, 'key_name', False)
+        is_key_name_maxresults = shape_key_name and (shape_key_name.lower() == 'maxresults')
         shape_name = get_shape_name(member_shape)
-        if shape_name.lower() == "maxresults" or is_key_name_maxresults:
+        if shape_name.lower() == 'maxresults' or is_key_name_maxresults:
             member_shape
-            max_value = member_shape.metadata.get("max", False)
+            max_value = member_shape.metadata.get('max', False)
             if max_value:
                 return max_value
     return False
 
-
 def get_input_shape(operation_model: OperationModel) -> Shape:
     """Get the input shape of the operation model
 
     Args:
-        operation_model (OperationModel): botocore OperationModel
+        operation_model (OperationModel): botocore OperationModel 
 
     Returns:
         Shape: Input Shape of the OperationModel
     """
-    return getattr(operation_model, "input_shape", False)
+    return getattr(operation_model, 'input_shape', False)
+
 
 
-def get_members_shapes(shape: Shape, _recursion_count=0) -> List[Shape]:
+def get_members_shapes(shape: Shape) -> List[Shape]:
     """Get the member shapes of and input or output Shape.
 
     Args:
         shape (Shape): Shape to get members from
 
     Returns:
         List[Shape]: Member Shapes, added `key_name` and `parent_name` values to objects.
     """
-
     found_members_shapes = []
-
-    if _recursion_count >= _MAX_ALLOWED_RECURSION:
-        return found_members_shapes
-
     if not shape:
         return found_members_shapes
     if shape.name in BLACKLISTED_SHAPE_NAMES:
         return found_members_shapes
-
-    if shape.type_name == "structure":
+    if shape.type_name == 'structure':
         for shape_key, member in shape.members.items():
-            setattr(member, "key_name", shape_key)
-            setattr(member, "parent_name", shape.name)
+            setattr(member, 'key_name', shape_key)
+            setattr(member, 'parent_name', shape.name)
             found_members_shapes.append(member)
-    elif shape.type_name == "list":
+    elif shape.type_name == 'list':
         only_member = shape.member
         found_members_shapes.append(only_member)
-    elif shape.type_name == "map":
-        t = get_members_shapes(shape.value, _recursion_count+1)
+    elif shape.type_name == 'map':
+        t = get_members_shapes(shape.value)
         return t
     return found_members_shapes
 
 
-def is_shape_non_collection_type(shape_and_target_path: ShapeAndTargetPath) -> bool:
-    """Boolean function to check ShapeAndTargetPath Named Tuple
+def filter_non_collection_shape(shape_and_target_path: ShapeAndTargetPath) -> bool:
+    """Bool function to check ShapeAndTargetPath Named Tuple 
 
     Args:
-        shape_and_target_path (ShapeAndTargetPath): Named Tuple
+        shape_and_target_path (ShapeAndTargetPath): Named Tuple. 
 
     Returns:
         bool: _description_
     """
     shape = shape_and_target_path.shape
-    has_key_name = getattr(shape, "key_name", False)
+    has_key_name = getattr(shape, 'key_name', False)
     is_non_collection = shape.type_name not in SHAPE_COLLECTION_TYPES
     return has_key_name and is_non_collection
 
 
-def _flatten_shape_to_its_members_and_target_paths(
-    shape: Shape, target_str: str = ""
-) -> List[ShapeAndTargetPath]:
-    """Recursive function to get a shape's all members with targetpaths.
-    Generates target_str JMESPath selector for each member as it's located in the hierarchy.
-    Returns a flat list of (shape, target_path) namedtuples
-
-    Args:
-        shape (Shape): botocore shape, possibly output shape of an operation
-        target_str (str, optional): Used for keeping track of the target path in recursion.
-
-    Returns:
-        List[ShapeAndTargetPath]: List of ShapeAndTargetPath NamedTuple
-    """
+def _flatten_shape_to_its_members_and_target_paths(shape, target_str='', ):
     result = []
     members = get_members_shapes(shape)
     for member in members:
-        member_key_name = getattr(member, "key_name", False)
+        member_key_name = getattr(member, 'key_name', False)
         new_target_str = target_str
         if member_key_name:
-            if target_str == "":
+            if target_str == '':
                 new_target_str = f"{member_key_name}"
             else:
                 new_target_str = f"{target_str}[*].{member_key_name}"
-        if member.type_name in (
-            "structure",
-            "list",
-        ):  # TODO:SHAPE_COLLECTION_TYPES-('map',):
-            # if the member is a collection type, recurse into it
-            inner_list = _flatten_shape_to_its_members_and_target_paths(
-                member, new_target_str
-            )
+        if member.type_name in ('structure', 'list'):# TODO:SHAPE_COLLECTION_TYPES-('map',):
+            inner_list = _flatten_shape_to_its_members_and_target_paths(member, new_target_str)
             result.extend(inner_list)
         else:
             result.append(ShapeAndTargetPath(member, new_target_str))
     return result
 
-
-def flatten_shape_to_its_non_collection_shape_and_target_paths(
-    shape: Shape,
-) -> List[ShapeAndTargetPath]:
-    """Return a flat list of shapes all member shapes w/ their JMESPath selector `target_path`
-
-    Args:
-        shape (Shape): botocore shape to list its members
-
-    Returns:
-        List[ShapeAndTargetPath]: (shape, target_path) custom namedtuple
-    """
-    # generate all possible members and their target paths
-    all_flat_members_and_target_paths = _flatten_shape_to_its_members_and_target_paths(
-        shape
-    )
-    # filter out the collection types beacuse they are not supported by JMESPath
-    non_collection_shapes_and_target_paths = list(
-        filter(is_shape_non_collection_type, all_flat_members_and_target_paths)
-    )
+def flatten_shape_to_its_non_collection_shape_and_target_paths(shape):
+    all_flat_members_and_target_paths = _flatten_shape_to_its_members_and_target_paths(shape)
+    non_collection_shapes_and_target_paths = list(filter(filter_non_collection_shape, all_flat_members_and_target_paths))
     return non_collection_shapes_and_target_paths
 
+"""
+    root = Tree("🌲 [b green]Rich Tree", highlight=True, hide_root=True)
+    node = root.add(":file_folder: Renderables", guide_style="red")
+    simple_node = node.add(":file_folder: [bold yellow]Atomic", guide_style="uu green")
+    simple_node.add(Group("📄 Syntax", syntax))
+    simple_node.add(Group("📄 Markdown", Panel(markdown, border_style="green")))
+    containers_node = node.add(
+        ":file_folder: [bold magenta]Containers", guide_style="bold magenta"
+    )
+    containers_node.expanded = True
+    panel = Panel.fit("Just a panel", border_style="red")
+    containers_node.add(Group("📄 Panels", panel))
 
-def cleanhtml(raw_html: str) -> str:
-    """Removes the HTML tags from given raw_html
+therewillbebeloodthere
+        containers_node.add(Group("📄 [b magenta]Table", table))
 
-    Args:
-        raw_html (str): HTML string to clean the tags off of
+    console = Console()
 
-    Returns:
-        str: HTML with tags removed
-    """
-    cleantext = re.sub(HTML_CLEANER_REGEX, "", raw_html)
-    return cleantext
+    console.print(root)
+"""
 
 
 def rich_str_shape(shape: Shape) -> str:
     """Transforms a Shape to rich supported string.
 
     Args:
         shape (Shape): botocore.model.Shape object.
 
     Returns:
         str: Rich string for shape.
     """
-    key_name = getattr(shape, "key_name", "")
+    key_name = getattr(shape, 'key_name', '{')
     type_name = str(shape.type_name)
-    shape_documentation = cleanhtml(shape.documentation)
-
-    shape_str = (
-        f"[blue bold]{key_name}[/] [white]({type_name})[/]: {shape_documentation}"
-    )
-    if key_name == "":
-        lead = ""
-        if type_name == "list":
-            lead = "["
-        elif type_name == "structure":
-            lead = "{"
-        shape_str = f"[red]{escape(lead)}[/] — [white](({type_name}))[/]: [gray]{shape_documentation}[/]"
-
+    if key_name == '{' and type_name == 'structure':
+        type_name = ''
+    if type_name:
+        type_name = f"({type_name})"
+    shape_str = f"[blue]{key_name} [white]{type_name}"
     return shape_str
 
 
 def generate_rich_tree_from_shape(shape: Shape) -> Tree:
     """Genereate a rich Tree containing `shape` and it's members."""
     tree = Tree(rich_str_shape(shape), guide_style="red")
-
-    def _recursive_stringify_shape(shape, node: Tree):
+    def _recursive_stringify_shape(shape, node):
 
         members = get_members_shapes(shape)
         for member in members:
-            member_str = rich_str_shape(member)
+            member_str = rich_str_shape(member) 
             if member.type_name in SHAPE_COLLECTION_TYPES:
                 new_node = node.add(member_str)
                 _recursive_stringify_shape(member, new_node)
             else:
                 node.add(member_str)
-
     _recursive_stringify_shape(shape, tree)
     return tree
-
-
+        
+    
 # @lru_cache(maxsize=500) # print(get_shape_name.cache_info())
 def get_shape_name(shape: Shape) -> str:
-    """Returns the shapes name, using custom set 'key_name' attr
-
-    Args:
-        shape (Shape): botocore Shape obj
-
-    Returns:
-        str: Name of the shape.
-    """
+    """Returns the shapes name, using custom set object values"""
     shape_name = shape.name
-    shape_key_name = getattr(shape, "key_name", False)
+    shape_key_name = getattr(shape, 'key_name', False)
     if shape_name.lower() in UNWANTED_SHAPE_NAMES_LOWERED:
         # check for name forgotten in shape.serialization if the name is a type name.
         if shape_key_name:
             return shape_key_name
-        elif shape.serialization and shape.serialization.get("name", False):
-            given_serialization_name = shape.serialization.get("name")
+        elif shape.serialization and shape.serialization.get('name', False):
+            given_serialization_name = shape.serialization.get('name')
             return given_serialization_name
-    if shape_key_name:
-        return shape_key_name
     return shape_name
-
-
-def get_required_parameter_shapes_from_operation_model(
-    operation_model: OperationModel,
-) -> List[Shape]:
-    """Finds required parameter shapes of the operation models input_shape.
-
-    Args:
-        operation_model (OperationModel): botocore OperationModel obj of the Operation
-
-    Returns:
-        List[Shape]: Required parameter shapes.
-    """
+   
+def get_required_parameter_shapes_from_operation_model(operation_model: OperationModel) -> List[Shape]:
     input_shape = get_input_shape(operation_model)
     if not input_shape:
-        return []  # there's no input shape
+        return [] # there's no input shape
     input_shape_members = get_members_shapes(input_shape)
     input_required_member_names = input_shape.required_members
     if input_required_member_names == []:
         return []
-
+    
     required_member_shapes = []
     for input_member in input_shape_members:
         input_member_name = get_shape_name(input_member)
         for required_name in input_required_member_names:
             if icompare_two_camel_case_words(required_name, input_member_name):
                 required_member_shapes.append(input_member)
-
+            
     return required_member_shapes
+
+# def get_required_parameters_for_operation(operation_model):
+#     required_parameter_shapes = get_required_parameters_for_operation(operation_model)
+#     required_parameter_names = [
+#         get_shape_name(r_param_shape)
+#         for r_param_shape in required_parameter_shapes
+#     ]
+#     return required_parameter_names
+
+def compare_shape_names(member, search_shape):
+    return get_shape_name(member) == get_shape_name(search_shape)
+
+
```

### Comparing `balcony-0.0.86/balcony/custom_nodes/lambda_functions.py` & `balcony-0.0.9/balcony/custom_nodes/lambda_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-# from ..nodes import ResourceNode
-# from ..config import get_logger
+try:
+    from ..nodes import ResourceNode
+    from ..registries import ResourceNodeRegistry
+    from ..logs import get_logger
+    from ..relations import FindRelationResultTypes
+except ImportError:
+    from nodes import ResourceNode
+    from registries import ResourceNodeRegistry
+    from logs import get_logger
+    from relations import FindRelationResultTypes
+logger = get_logger(__name__)
 
-# logger = get_logger(__name__)
-
-# class Function(ResourceNode, service_name="lambda", name="Function"):
-#     def __init__(self, *args, **kwargs):
-#         super().__init__(*args, **kwargs)
+class Lambda_Function(ResourceNode, ResourceNodeRegistry, service_name="lambda", name="Function"):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
     
-#     def define_extra_relations(self):
-#         r= super().define_extra_relations()
-#         return [{
-#             "service_name": "lambda",
-#             "resource_node_name": "Function",
-#             "operation_name": "ListFunctions",
-#             "required_shape_name": "FunctionName",
-#             "target_shape_name": "FunctionName",
-#             "target_shape_type": "string",
-#             "target_path": "Functions[*].FunctionName"
-#         }]
+    def define_extra_relations(self):
+        r= super().define_extra_relations()
+        return [{
+            "service_name": "lambda",
+            "resource_node_name": "Function",
+            "operation_name": "ListFunctions",
+            "search_shape_name": "FunctionName",
+            "target_shape_name": "FunctionName",
+            "target_shape_type": "string",
+            "target_path": "Functions[*].FunctionName"
+        }]
```

### Comparing `balcony-0.0.86/balcony/custom_nodes/s3.py` & `balcony-0.0.9/balcony/custom_nodes/s3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-from nodes import ResourceNode
-from config import get_logger
-
+try:
+    from ..nodes import ResourceNode
+    from ..registries import ResourceNodeRegistry
+    from ..logs import get_logger
+    from ..relations import FindRelationResultTypes
+except ImportError:
+    from nodes import ResourceNode
+    from registries import ResourceNodeRegistry
+    from logs import get_logger
+    from relations import FindRelationResultTypes
 logger = get_logger(__name__)
 
-class BucketLifecycleConfiguration(ResourceNode, service_name="s3", name="BucketLifecycleConfiguration"):
+class S3_BucketLifecycleConfiguration(ResourceNode, ResourceNodeRegistry, service_name="s3", name="BucketLifecycleConfiguration"):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
     
     def define_extra_relations(self):
         r= super().define_extra_relations()
         return [{
             "service_name": "s3",
             "resource_node_name": "Buckets",
-            "required_shape_name": "Bucket",
+            "search_shape_name": "Bucket",
             "target_shape_name": "Name",
             "target_shape_type": "string",
             "operation_name": "ListBuckets",
             "target_path": "Buckets[*].Name"
         }]
 
     # def find_best_relations_for_operation(self, operation_name, relation_map):
```

### Comparing `balcony-0.0.86/pyproject.toml` & `balcony-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 [tool.poetry]
 name = "balcony"
-version = "0.0.86"
+version = "0.0.9"
 description = "AWS API for humans"
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-typer = "^0.7.0"
-rich = "^13.3.4"
+typer = "^0.6.1"
+rich = "^12.5.1"
 boto3 = "^1.24.80"
 jmespath = "^1.0.1"
 inflect = "^6.0.0"
-mkdocstrings = {version = "^0.21.2", extras = ["python"]}
-mkdocs-material = ">=8.5.7,<10.0.0"
-mkdocs-autorefs = "^0.4.1"
-PyYAML = "^6.0"
-pydantic = "^1.10.7"
-
 
 [tool.poetry.group.dev.dependencies]
+nose3 = "^1.3.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

