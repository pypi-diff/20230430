# Comparing `tmp/docchain-0.0.3.tar.gz` & `tmp/docchain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docchain-0.0.3.tar", max compression
+gzip compressed data, was "docchain-0.0.4.tar", max compression
```

## Comparing `docchain-0.0.3.tar` & `docchain-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1079 2023-04-28 14:04:53.107245 docchain-0.0.3/README.md
--rw-r--r--   0        0        0      107 2023-04-28 14:04:53.107245 docchain-0.0.3/docchain/__init__.py
--rw-r--r--   0        0        0      754 2023-04-28 14:04:53.107245 docchain-0.0.3/docchain/documents.py
--rw-r--r--   0        0        0       51 2023-04-28 14:04:53.107245 docchain-0.0.3/docchain/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-28 14:04:53.107245 docchain-0.0.3/docchain/generators/__init__.py
--rw-r--r--   0        0        0     1905 2023-04-28 14:04:53.107245 docchain-0.0.3/docchain/generators/base.py
--rw-r--r--   0        0        0     2302 2023-04-28 14:04:53.107245 docchain-0.0.3/docchain/generators/pydantic.py
--rw-r--r--   0        0        0     2648 2023-04-28 14:04:53.107245 docchain-0.0.3/docchain/generators/text.py
--rw-r--r--   0        0        0        0 2023-04-28 14:04:53.107245 docchain-0.0.3/docchain/models/__init__.py
--rw-r--r--   0        0        0      155 2023-04-28 14:04:53.111245 docchain-0.0.3/docchain/models/gpt.py
--rw-r--r--   0        0        0     1023 2023-04-28 14:04:53.111245 docchain-0.0.3/docchain/settings.py
--rw-r--r--   0        0        0     1902 2023-04-28 14:04:53.111245 docchain-0.0.3/docchain/specs.py
--rw-r--r--   0        0        0      674 2023-04-28 14:04:53.111245 docchain-0.0.3/docchain/steps/__init__.py
--rw-r--r--   0        0        0      730 2023-04-28 14:04:53.111245 docchain-0.0.3/docchain/steps/base.py
--rw-r--r--   0        0        0      915 2023-04-28 14:04:53.111245 docchain-0.0.3/docchain/steps/collect_openai_stats.py
--rw-r--r--   0        0        0      394 2023-04-28 14:04:53.111245 docchain-0.0.3/docchain/steps/save_document.py
--rw-r--r--   0        0        0      648 2023-04-28 14:04:53.111245 docchain-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1641 1970-01-01 00:00:00.000000 docchain-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-30 12:46:59.618177 docchain-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/__init__.py
+-rw-r--r--   0        0        0      758 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/documents.py
+-rw-r--r--   0        0        0       51 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/generators/__init__.py
+-rw-r--r--   0        0        0     1905 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/generators/base.py
+-rw-r--r--   0        0        0     3446 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/generators/pydantic.py
+-rw-r--r--   0        0        0     2648 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/generators/text.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/models/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/models/gpt.py
+-rw-r--r--   0        0        0     1707 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/output_parsers/json_schema.py
+-rw-r--r--   0        0        0     1023 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/settings.py
+-rw-r--r--   0        0        0     2044 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/specs.py
+-rw-r--r--   0        0        0      574 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/steps/__init__.py
+-rw-r--r--   0        0        0      730 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/steps/base.py
+-rw-r--r--   0        0        0      921 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/steps/collect_openai_stats.py
+-rw-r--r--   0        0        0      394 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/steps/save_document.py
+-rw-r--r--   0        0        0      288 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/utils.py
+-rw-r--r--   0        0        0      605 2023-04-30 12:46:59.618177 docchain-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 docchain-0.0.4/PKG-INFO
```

### Comparing `docchain-0.0.3/README.md` & `docchain-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,7 @@
 
 `Step` is a callable that can modify Spec or generated Document. It could be thought as middleware
 in an HTTP framework and cna be used for variety of tasks.
 
 ## TODO
 
 - [ ] Implement checkpoints and resume generation from checkpoint on failure.
-- [ ] Publish to PyPI.
```

### Comparing `docchain-0.0.3/docchain/documents.py` & `docchain-0.0.4/docchain/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     summary: str | None = None
     text: str = Field(default="")
 
 
 class Document(Section):
     """
     Document consist of Sections.
-    It should support the same behaviour as section though so documents can be included in other documents.
+    It should support the same behaviour as section though so documents can be
+    included in other documents.
     """
 
     sections: list[Section] = Field(default=[])
     format: Format | PydanticFormat = Format.text
     filename: Path = Field(default=None)
     stats: dict[str, int | float] = Field(default={})
```

### Comparing `docchain-0.0.3/docchain/generators/base.py` & `docchain-0.0.4/docchain/generators/base.py`

 * *Files identical despite different names*

### Comparing `docchain-0.0.3/docchain/generators/pydantic.py` & `docchain-0.0.4/docchain/generators/pydantic.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,20 +3,28 @@
 from collections.abc import Iterable
 
 import yaml
 from langchain.chains import LLMChain
 
 from .base import BaseDocumentGenerator
 from ..documents import Document, Section, PydanticFormat
-from docchain.settings import conf
+from ..output_parsers.json_schema import JSONSchemaOutputParser
+from ..settings import conf
 from langchain.llms import BaseLLM
 from langchain.prompts import PromptTemplate
 from langchain.output_parsers import PydanticOutputParser
 
-from ..specs import PydanticDocumentSpec, PydanticSectionSpec
+
+from ..specs import (
+    PydanticDocumentSpec,
+    PydanticSectionSpec,
+    ModelSectionSpec,
+    JSONSchemaSectionSpec,
+)
+from ..utils import set_nested_key
 
 
 class PydanticGenerator(BaseDocumentGenerator):
     """
     Generates a document from a Pydantic model.
     """
 
@@ -32,44 +40,70 @@
             filename=spec.filename,
             format=spec.format,
             text="{}",
         )
 
         doc_dict = {}
         for section_spec in spec.sections:
-            section = self.build_section(section_spec)
+            section = self.gen_section(section_spec)
             doc.sections.append(section)
-            doc_dict[section_spec.key] = json.loads(section.text)
+            set_nested_key(doc_dict, section_spec.key, json.loads(section.text))
 
         match spec.format:
             case PydanticFormat.json:
                 doc.text = json.dumps(doc_dict, indent=4)
             case PydanticFormat.yaml:
                 doc.text = yaml.dump(doc_dict, indent=4)
 
         return doc
 
-    def build_section(self, spec: PydanticSectionSpec) -> Section:
+    def gen_section(self, spec: PydanticSectionSpec) -> Section:
         section = Section(
             title=spec.title,
         )
 
+        match spec:
+            case ModelSectionSpec():
+                section.text = self.generate_model_section(spec)
+            case JSONSchemaSectionSpec():
+                section.text = self.generate_json_schema_section(spec)
+
+        return section
+
+    def generate_model_section(self, spec: ModelSectionSpec) -> str:
         parser = PydanticOutputParser(pydantic_object=spec.document_schema)
         default_prompt = PromptTemplate(
             template="""
         Write {section_name} section of configuration file for {description}.
 
         {format_instructions}
         """,
             input_variables=["section_name", "description"],
             output_parser=parser,
             partial_variables={"format_instructions": parser.get_format_instructions()},
         )
+        llm_chain = LLMChain(prompt=default_prompt, llm=self.llm)
+        result = llm_chain.run(
+            section_name=spec.title,
+            description=spec.description,
+        )
 
+        return result
+
+    def generate_json_schema_section(self, spec: JSONSchemaSectionSpec) -> str:
+        parser = JSONSchemaOutputParser()
+        default_prompt = PromptTemplate(
+            template="""Give me JSON Schema for {section_name}.
+{description}
+{format_instructions}
+        """,
+            output_parser=parser,
+            input_variables=["section_name", "description"],
+            partial_variables={"format_instructions": parser.get_format_instructions()},
+        )
         llm_chain = LLMChain(prompt=default_prompt, llm=self.llm)
         result = llm_chain.run(
             section_name=spec.title,
             description=spec.description,
         )
-        section.text = result
 
-        return section
+        return result
```

### Comparing `docchain-0.0.3/docchain/generators/text.py` & `docchain-0.0.4/docchain/generators/text.py`

 * *Files identical despite different names*

### Comparing `docchain-0.0.3/docchain/settings.py` & `docchain-0.0.4/docchain/settings.py`

 * *Files identical despite different names*

### Comparing `docchain-0.0.3/docchain/specs.py` & `docchain-0.0.4/docchain/specs.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,37 +20,45 @@
         default="", description="The title of the section within the document."
     )
     description: str = Field(
         default="", description="A brief description of the section."
     )
 
 
-class PydanticSectionSpec(TextSectionSpec):
-    key: str = Field(
-        regex="[a-zA-Z0-9_-]{0,1000}",
-        description="A unique string key for the section. Follows slug format.",
-    )
-    document_schema: type[BaseModel] = Field(
-        description="A Pydantic BaseModel representing the schema for the section."
-    )
-
-
 class TextDocumentSpec(Spec):
     document_name: str = Field(default="", description="The name of the document.")
     document_description: str = Field(
         default="", description="A brief description of the document."
     )
     sections: list[TextSectionSpec] = Field(
         default=[],
-        description="A list of TextSectionSpec objects representing the sections within the document.",
+        description="A list of objects representing the sections within the document.",
+    )
+
+
+class PydanticSectionSpec(TextSectionSpec):
+    key: str = Field(
+        regex="[a-zA-Z0-9_\\-\\.]{1,100}",
+        description="A unique string key for the section. Must be unique within the document. "
+        "Dot in the key represents a nested section.",
+    )
+
+
+class JSONSchemaSectionSpec(PydanticSectionSpec):
+    pass
+
+
+class ModelSectionSpec(PydanticSectionSpec):
+    document_schema: type[BaseModel] = Field(
+        description="A Pydantic model representing the schema for the section."
     )
 
 
 class PydanticDocumentSpec(TextDocumentSpec):
     format: PydanticFormat = Field(
         default=PydanticFormat.json,
         description="The format of the document as a PydanticFormat object. Defaults to json.",
     )
     sections: list[PydanticSectionSpec] = Field(
         default=[],
-        description="A list of PydanticSectionSpec objects representing the sections within the document.",
+        description="A list of objects representing the sections within the document.",
     )
```

### Comparing `docchain-0.0.3/docchain/steps/__init__.py` & `docchain-0.0.4/docchain/steps/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,10 +18,7 @@
             # Modify Doc
             document.title += " (Draft)"
 
             return document
 
         return run
 """
-
-from .collect_openai_stats import collect_openai_stats
-from .save_document import SaveDocumentStep
```

### Comparing `docchain-0.0.3/docchain/steps/base.py` & `docchain-0.0.4/docchain/steps/base.py`

 * *Files identical despite different names*

### Comparing `docchain-0.0.3/docchain/steps/collect_openai_stats.py` & `docchain-0.0.4/docchain/steps/collect_openai_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from ..settings import conf
 
 from logging import getLogger
 
-from docchain import Spec
+from docchain.specs import Spec
 from langchain.callbacks import get_openai_callback
 
 logger = getLogger(__name__)
 
 
 def collect_openai_stats(build_document):
     def run(spec: Spec):
```

### Comparing `docchain-0.0.3/PKG-INFO` & `docchain-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: docchain
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: Artem Kolesnikov
 Author-email: tyomo4ka@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langchain (>=0.0.152,<0.0.153)
-Requires-Dist: openai (>=0.27.4,<0.28.0)
-Requires-Dist: pytest-dotenv (>=0.5.2,<0.6.0)
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Requires-Dist: langchain (>=0.0.153,<0.0.154)
+Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Doc Chain
 
 This package can be used to generate complex structured documents from specification using LLMm
 models.
 
@@ -35,9 +34,8 @@
 
 `Step` is a callable that can modify Spec or generated Document. It could be thought as middleware
 in an HTTP framework and cna be used for variety of tasks.
 
 ## TODO
 
 - [ ] Implement checkpoints and resume generation from checkpoint on failure.
-- [ ] Publish to PyPI.
```

