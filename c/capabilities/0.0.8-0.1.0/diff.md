# Comparing `tmp/capabilities-0.0.8.tar.gz` & `tmp/capabilities-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capabilities-0.0.8.tar", last modified: Wed Apr 12 17:12:25 2023, max compression
+gzip compressed data, was "capabilities-0.1.0.tar", last modified: Sun Apr 30 16:48:22 2023, max compression
```

## Comparing `capabilities-0.0.8.tar` & `capabilities-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:12:25.540668 capabilities-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 17:12:15.000000 capabilities-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-04-12 17:12:25.540668 capabilities-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 17:12:15.000000 capabilities-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:12:25.540668 capabilities-0.0.8/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 17:12:15.000000 capabilities-0.0.8/capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-12 17:12:15.000000 capabilities-0.0.8/capabilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-12 17:12:15.000000 capabilities-0.0.8/capabilities/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-12 17:12:15.000000 capabilities-0.0.8/capabilities/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-12 17:12:15.000000 capabilities-0.0.8/capabilities/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:12:25.540668 capabilities-0.0.8/capabilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-04-12 17:12:25.000000 capabilities-0.0.8/capabilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 17:12:25.000000 capabilities-0.0.8/capabilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:12:25.000000 capabilities-0.0.8/capabilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 17:12:25.000000 capabilities-0.0.8/capabilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 17:12:25.000000 capabilities-0.0.8/capabilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-12 17:12:15.000000 capabilities-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:12:25.544668 capabilities-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 17:12:15.000000 capabilities-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:48:22.954115 capabilities-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 16:48:11.000000 capabilities-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-04-30 16:48:22.954115 capabilities-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-30 16:48:11.000000 capabilities-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:48:22.950114 capabilities-0.1.0/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12737 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:48:22.954115 capabilities-0.1.0/capabilities/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/nomic_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/search_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/simple_vector_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:48:22.954115 capabilities-0.1.0/capabilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-30 16:48:11.000000 capabilities-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:48:22.954115 capabilities-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-30 16:48:11.000000 capabilities-0.1.0/setup.py
```

### Comparing `capabilities-0.0.8/LICENSE` & `capabilities-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.0.8/PKG-INFO` & `capabilities-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.0.8
+Version: 0.1.0
+Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -202,14 +203,17 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: search
+Provides-Extra: nomic
+Provides-Extra: sentence-transformers
 License-File: LICENSE
 
 # capabilities
 
 Blazon Capabilities SDK
 
 # Install and run example
```

### Comparing `capabilities-0.0.8/capabilities/core.py` & `capabilities-0.1.0/capabilities/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import dataclasses
 import dacite
 from dataclasses import dataclass, field, is_dataclass
-from typing import Dict, Any, List, Union
+from typing import Dict, Any, List, Union, Literal
 from typing import Optional
 import requests
 import aiohttp
 import asyncio
 import time
 from capabilities.config import CONFIG
 from pydantic import BaseModel
@@ -179,15 +179,15 @@
                 sleep_duration = 2.0**count
                 print(f"retrying after sleeping for {sleep_duration:.2f}")
                 count += 1
                 time.sleep(sleep_duration)
         raise Exception("[Summarize] failed after hitting max retries")
 
 
-def flatten_model(m: Union[ModelMetaclass, str, bool, float, int]):
+def flatten_model(m: Union[ModelMetaclass, str, bool, float, int]) -> Dict[Any, Any]:
     if hasattr(m, "__dict__"):
         if m.__dict__.get("_name") == "List":
             return [flatten_model(m.__args__[0])]
     if isinstance(m, ModelMetaclass) or is_dataclass(m):
         return {k: flatten_model(v) for k, v in m.__annotations__.items()}
     elif m == str:
         return "string"
@@ -230,14 +230,15 @@
         payload = dict(
             input_spec=flatten_model(input_spec),
             output_spec=flatten_model(output_spec),
             instructions=instructions,
             input=dataclasses.asdict(input) if is_dataclass(input) else input.dict(),
         )
         r = requests.post(self.url, headers=self.headers, json=payload)
+        print("R: ", r)
         result = r.json()["output"]
         return (
             output_spec.parse_obj(result)
             if isinstance(output_spec, ModelMetaclass)
             else dacite.from_dict(output_spec, result)
         )
```

### Comparing `capabilities-0.0.8/capabilities/example.py` & `capabilities-0.1.0/capabilities/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import fire
 from capabilities import Capability
 from pydantic import BaseModel
 from typing import List
 
+
 EXAMPLE_PASSAGE = """\
 Wide-scale production is credited to Edward Goodrich Acheson in 1890.[11] Acheson was attempting to prepare artificial diamonds when he heated a mixture of clay (aluminium silicate) and powdered coke (carbon) in an iron bowl. He called the blue crystals that formed carborundum, believing it to be a new compound of carbon and aluminium, similar to corundum. Moissan also synthesized SiC by several routes, including dissolution of carbon in molten silicon, melting a mixture of calcium carbide and silica, and by reducing silica with carbon in an electric furnace. Acheson patented the method for making silicon carbide powder on February 28, 1893.[12] Acheson also developed the electric batch furnace by which SiC is still made today and formed the Carborundum Company to manufacture bulk SiC, initially for use as an abrasive.[13] In 1900 the company settled with the Electric Smelting and Aluminum Company when a judge's decision gave "priority broadly" to its founders "for reducing ores and other substances by the incandescent method".[14] It is said that Acheson was trying to dissolve carbon in molten corundum (alumina) and discovered the presence of hard, blue-black crystals which he believed to be a compound of carbon and corundum: hence carborundum. It may be that he named the material "carborundum" by analogy to corundum, which is another very hard substance (9 on the Mohs scale). The first use of SiC was as an abrasive. This was followed by electronic applications. In the beginning of the 20th century, silicon carbide was used as a detector in the first radios.[15] In 1907 Henry Joseph Round produced the first LED by applying a voltage to a SiC crystal and observing yellow, green and orange emission at the cathode. The effect was later rediscovered by O. V. Losev in the Soviet Union in 1923.[16]\
 """
 
 
 def example_structured():
     # structured synthesis capability
@@ -75,19 +76,14 @@
     print("Result: ", answer)
     print(
         "Formatted result: ",
         "- " + "\n- ".join(bp["bullet_point"] for bp in answer["answer"]["claims"]),
     )
 
 
-def example_search():
-    c = Capability("blazon/search")
-    print(c("Who discovered the useful properties of silicon carbide?"))
-
-
 def parse_table():
     class UnstructuredTable(BaseModel):
         unstructured_table: str
 
     class ParsedCell(BaseModel):
         cell_content: str
 
@@ -248,15 +244,14 @@
 
 
 class SortedIndices(BaseModel):
     sorted_indices: List[int]
 
 
 def example_link_permutations(topic: str, input: Links) -> SortedIndices:
-
     instructions = f"""\
 Given the input list of `links`, return a list of `sorted_indices` which reorders `links` from most relevant to least relevant for {topic}. `sorted_indices` must contain all integers from 0 to len(`links`) - 1, and `sorted_indices[0]` must be the most relevant link and `sorted_indices[-1]` must be the least relevant link.
     """
 
     indices = Capability("blazon/summarize")(
         Links, SortedIndices, instructions, input
     ).sorted_indices
@@ -290,14 +285,16 @@
 
     input: SynthesisRequest = SynthesisRequest(
         goal="Retrieve the first three paragraphs",
         url="https://en.wikipedia.org/wiki/Selenium_(software)",
         title="Google",
     )
 
+    
+
     print(
         Capability("blazon/structured")(
             SynthesisRequest, SynthesisResponse, instructions, input=input
         ).dict()
     )
 
 
@@ -315,9 +312,8 @@
         BulletPoints(bullet_points=bullet_points),
     ).summary
 
 
 # example usage: python -m capabilities.example example_translation
 if __name__ == "__main__":
     import sys
-
     fire.Fire(component=locals()[sys.argv[1]], command=sys.argv[2:])
```

### Comparing `capabilities-0.0.8/capabilities/util.py` & `capabilities-0.1.0/capabilities/util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.0.8/capabilities.egg-info/PKG-INFO` & `capabilities-0.1.0/capabilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.0.8
+Version: 0.1.0
+Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -202,14 +203,17 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: search
+Provides-Extra: nomic
+Provides-Extra: sentence-transformers
 License-File: LICENSE
 
 # capabilities
 
 Blazon Capabilities SDK
 
 # Install and run example
```

