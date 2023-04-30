# Comparing `tmp/thinkgpt-0.0.5.tar.gz` & `tmp/thinkgpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinkgpt-0.0.5.tar", max compression
+gzip compressed data, was "thinkgpt-0.0.6.tar", max compression
```

## Comparing `thinkgpt-0.0.5.tar` & `thinkgpt-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.5/LICENSE
--rw-r--r--   0        0        0     8095 2023-04-25 15:24:53.616328 thinkgpt-0.0.5/README.md
--rw-r--r--   0        0        0      562 2023-04-25 15:38:13.266488 thinkgpt-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.5/thinkgpt/__init__.py
--rw-r--r--   0        0        0     3906 2023-04-24 17:17:15.104859 thinkgpt-0.0.5/thinkgpt/abstract.py
--rw-r--r--   0        0        0     2190 2023-04-24 17:17:15.101408 thinkgpt-0.0.5/thinkgpt/condition.py
--rw-r--r--   0        0        0     3650 2023-04-24 17:17:15.093655 thinkgpt-0.0.5/thinkgpt/gpt_select.py
--rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.5/thinkgpt/helper.py
--rw-r--r--   0        0        0     2779 2023-04-24 17:17:15.108158 thinkgpt-0.0.5/thinkgpt/infer.py
--rw-r--r--   0        0        0     4426 2023-04-25 15:26:36.146838 thinkgpt-0.0.5/thinkgpt/llm.py
--rw-r--r--   0        0        0     2393 2023-04-24 17:17:15.111894 thinkgpt-0.0.5/thinkgpt/memory.py
--rw-r--r--   0        0        0     1587 2023-04-24 17:17:15.115188 thinkgpt-0.0.5/thinkgpt/refine.py
--rw-r--r--   0        0        0     2890 2023-04-24 17:17:15.097660 thinkgpt-0.0.5/thinkgpt/summarize.py
--rw-r--r--   0        0        0     8996 1970-01-01 00:00:00.000000 thinkgpt-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.6/LICENSE
+-rw-r--r--   0        0        0     8688 2023-04-30 11:57:54.059196 thinkgpt-0.0.6/README.md
+-rw-r--r--   0        0        0      562 2023-04-30 15:23:17.123338 thinkgpt-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.6/thinkgpt/__init__.py
+-rw-r--r--   0        0        0     3906 2023-04-24 17:17:15.104859 thinkgpt-0.0.6/thinkgpt/abstract.py
+-rw-r--r--   0        0        0     2190 2023-04-24 17:17:15.101408 thinkgpt-0.0.6/thinkgpt/condition.py
+-rw-r--r--   0        0        0     3650 2023-04-24 17:17:15.093655 thinkgpt-0.0.6/thinkgpt/gpt_select.py
+-rw-r--r--   0        0        0     1656 2023-04-30 11:32:02.536883 thinkgpt-0.0.6/thinkgpt/helper.py
+-rw-r--r--   0        0        0     2779 2023-04-24 17:17:15.108158 thinkgpt-0.0.6/thinkgpt/infer.py
+-rw-r--r--   0        0        0     4426 2023-04-25 15:26:36.146838 thinkgpt-0.0.6/thinkgpt/llm.py
+-rw-r--r--   0        0        0     2615 2023-04-30 11:32:02.539652 thinkgpt-0.0.6/thinkgpt/memory.py
+-rw-r--r--   0        0        0     1587 2023-04-24 17:17:15.115188 thinkgpt-0.0.6/thinkgpt/refine.py
+-rw-r--r--   0        0        0     2890 2023-04-24 17:17:15.097660 thinkgpt-0.0.6/thinkgpt/summarize.py
+-rw-r--r--   0        0        0     9589 1970-01-01 00:00:00.000000 thinkgpt-0.0.6/PKG-INFO
```

### Comparing `thinkgpt-0.0.5/LICENSE` & `thinkgpt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.5/README.md` & `thinkgpt-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 ## Key Features ✨
 * Thinking building blocks 🧱:
     * Memory 🧠: GPTs that can remember experience
     * Self-refinement 🔧: Improve model-generated content by addressing critics
     * Compress knowledge 🌐: Compress knowledge and fit it in LLM's context either by anstracring rules out of observations or summarize large content
     * Inference 💡️: Make educated guesses based on available information
     * Natural Language Conditions 📝: Easily express choices and conditions in natural language
-    * Finetuning 📚: Agents that can learn by finetuning (coming soon!)
 * Efficient and Measurable GPT context length 📐
 * Extremely easy setup and pythonic API 🎯 thanks to [DocArray](https://github.com/docarray/docarray)
 
 ## Installation 💻
 You can install ThinkGPT using pip:
 
 ```shell
@@ -43,14 +42,31 @@
 
 print(llm.remember('Sending data with DocArray', limit=1))
 ```
 ```text
 ['DocArray allows you to send your data, in an ML-native way.']
 ```
 
+Use the `limit` parameter to specify the maximum number of documents to retrieve.
+In case you want to fit documents into a certain context size, you can also use the `max_tokens` parameter to specify the maximum number of tokens to retrieve.
+For instance:
+```python
+from examples.knowledge_base import knowledge
+from thinkgpt.helper import get_n_tokens
+
+llm.memorize(knowledge)
+results = llm.remember('hello', max_tokens=1000, limit=1000)
+print(get_n_tokens(''.join(results)))
+```
+```text
+1000
+```
+However, keep in mind that concatenating documents with a separator will add more tokens to the final result.
+The `remember` method does not account for those tokens.
+
 ### Predicting with context from long memory
 ```python
 from examples.knowledge_base import knowledge
 llm.memorize(knowledge)
 llm.predict('Implement a DocArray schema with 2 fields: image and TorchTensor', remember=llm.remember('DocArray schemas and types'))
 ```
 
@@ -88,14 +104,15 @@
 llm.summarize(
   large_content,
   max_tokens= 1000,
   instruction_hint= 'Pay attention to code snippets, links and scientific terms.'
 )
 ```
 Since this technique relies on summarizing using a single LLM call, you can only pass content that does not exceed the LLM's context length.
+
 2. Chunked summarization
 ```python
 llm.chunked_summarize(
   very_large_content,
   max_tokens= 4096,
   instruction_hint= 'Pay attention to code snippets, links and scientific terms.'
 )
```

### Comparing `thinkgpt-0.0.5/pyproject.toml` & `thinkgpt-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thinkgpt"
-version = "0.0.5"
+version = "0.0.6"
 description = "ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents."
 authors = ["Alaeddine Abdessalem <alaeddine-13@live.fr>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
```

### Comparing `thinkgpt-0.0.5/thinkgpt/abstract.py` & `thinkgpt-0.0.6/thinkgpt/abstract.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.5/thinkgpt/condition.py` & `thinkgpt-0.0.6/thinkgpt/condition.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.5/thinkgpt/gpt_select.py` & `thinkgpt-0.0.6/thinkgpt/gpt_select.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.5/thinkgpt/helper.py` & `thinkgpt-0.0.6/thinkgpt/helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,8 +29,27 @@
             sys.stdout = old_stdout
             output = mystdout.getvalue()
         except Exception as e:
             sys.stdout = old_stdout
             output = mystdout.getvalue()
             # TODO: need stack trace as well
             error = str(e)
-        return output, error
+        return output, error
+
+
+def get_n_tokens(input: str, model_name: str = 'gpt-3.5-turbo'):
+    import tiktoken
+    enc = tiktoken.encoding_for_model(model_name)
+    res = enc.encode(input)
+    return len(res)
+
+
+def fit_context(text_elememts: List[str], max_tokens: int):
+    results = []
+    total_tokens = 0
+    for element in text_elememts:
+        total_tokens += get_n_tokens(element)
+        if total_tokens <= max_tokens:
+            results.append(element)
+        else:
+            break
+    return results
```

### Comparing `thinkgpt-0.0.5/thinkgpt/infer.py` & `thinkgpt-0.0.6/thinkgpt/infer.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.5/thinkgpt/llm.py` & `thinkgpt-0.0.6/thinkgpt/llm.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.5/thinkgpt/memory.py` & `thinkgpt-0.0.6/thinkgpt/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Optional
 
 import numpy as np
 from langchain import PromptTemplate, LLMChain
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.llms import OpenAI, BaseLLM
 from docarray import Document, DocumentArray
 
+from thinkgpt.helper import get_n_tokens, fit_context
 
 EXECUTE_WITH_CONTEXT_PROMPT = PromptTemplate(template="""
 Given a context information, reply to the provided request
 Context: {context}
 User request: {prompt}
 """, input_variables=["prompt", "context"], )
 
@@ -38,15 +39,15 @@
             self.memory.append(concept)
         elif isinstance(concept, (DocumentArray, list)):
             for doc in concept:
                 self.memorize(doc)
         else:
             raise ValueError('wrong type, must be either str, Document, DocumentArray, List')
 
-    def remember(self, concept: Union[str, Document] = None, limit: int = 5, sort_by_order: bool = False) -> List[str]:
+    def remember(self, concept: Union[str, Document] = None, limit: int = 5, sort_by_order: bool = False, max_tokens: Optional[int] = None) -> List[str]:
         if len(self.memory) == 0:
             return []
         if concept is None:
             return [doc.text for doc in self.memory[-limit:]]
         elif isinstance(concept, str):
             query_input = Document(embedding=np.asarray(self.embeddings_model.embed_query(concept)))
         elif isinstance(concept, Document):
@@ -55,8 +56,11 @@
         else:
             raise ValueError('wrong type, must be either str or Document')
 
         docs = self.memory.find(query_input, limit=limit)[0]
         # memory needs to be sorted in chronological order
         if sort_by_order:
             docs = sorted(docs, key=lambda doc: doc.tags['mem_cnt'])
-        return [doc.text for doc in docs]
+        text_results = [doc.text for doc in docs]
+        if max_tokens:
+            text_results = fit_context(text_results, max_tokens)
+        return text_results
```

### Comparing `thinkgpt-0.0.5/thinkgpt/refine.py` & `thinkgpt-0.0.6/thinkgpt/refine.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.5/thinkgpt/summarize.py` & `thinkgpt-0.0.6/thinkgpt/summarize.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.5/PKG-INFO` & `thinkgpt-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinkgpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents.
 License: Apache 2.0
 Author: Alaeddine Abdessalem
 Author-email: alaeddine-13@live.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,14 @@
 ## Key Features ✨
 * Thinking building blocks 🧱:
     * Memory 🧠: GPTs that can remember experience
     * Self-refinement 🔧: Improve model-generated content by addressing critics
     * Compress knowledge 🌐: Compress knowledge and fit it in LLM's context either by anstracring rules out of observations or summarize large content
     * Inference 💡️: Make educated guesses based on available information
     * Natural Language Conditions 📝: Easily express choices and conditions in natural language
-    * Finetuning 📚: Agents that can learn by finetuning (coming soon!)
 * Efficient and Measurable GPT context length 📐
 * Extremely easy setup and pythonic API 🎯 thanks to [DocArray](https://github.com/docarray/docarray)
 
 ## Installation 💻
 You can install ThinkGPT using pip:
 
 ```shell
@@ -64,14 +63,31 @@
 
 print(llm.remember('Sending data with DocArray', limit=1))
 ```
 ```text
 ['DocArray allows you to send your data, in an ML-native way.']
 ```
 
+Use the `limit` parameter to specify the maximum number of documents to retrieve.
+In case you want to fit documents into a certain context size, you can also use the `max_tokens` parameter to specify the maximum number of tokens to retrieve.
+For instance:
+```python
+from examples.knowledge_base import knowledge
+from thinkgpt.helper import get_n_tokens
+
+llm.memorize(knowledge)
+results = llm.remember('hello', max_tokens=1000, limit=1000)
+print(get_n_tokens(''.join(results)))
+```
+```text
+1000
+```
+However, keep in mind that concatenating documents with a separator will add more tokens to the final result.
+The `remember` method does not account for those tokens.
+
 ### Predicting with context from long memory
 ```python
 from examples.knowledge_base import knowledge
 llm.memorize(knowledge)
 llm.predict('Implement a DocArray schema with 2 fields: image and TorchTensor', remember=llm.remember('DocArray schemas and types'))
 ```
 
@@ -109,14 +125,15 @@
 llm.summarize(
   large_content,
   max_tokens= 1000,
   instruction_hint= 'Pay attention to code snippets, links and scientific terms.'
 )
 ```
 Since this technique relies on summarizing using a single LLM call, you can only pass content that does not exceed the LLM's context length.
+
 2. Chunked summarization
 ```python
 llm.chunked_summarize(
   very_large_content,
   max_tokens= 4096,
   instruction_hint= 'Pay attention to code snippets, links and scientific terms.'
 )
```

