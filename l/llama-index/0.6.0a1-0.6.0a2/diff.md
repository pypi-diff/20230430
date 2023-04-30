# Comparing `tmp/llama_index-0.6.0a1.tar.gz` & `tmp/llama_index-0.6.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.6.0a1.tar", last modified: Fri Apr 28 21:55:20 2023, max compression
+gzip compressed data, was "llama_index-0.6.0a2.tar", last modified: Sat Apr 29 16:25:25 2023, max compression
```

## Comparing `llama_index-0.6.0a1.tar` & `llama_index-0.6.0a2.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.258896 llama_index-0.6.0a1/
--rw-r--r--   0 suo        (501) staff       (20)     1064 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/LICENSE
--rw-r--r--   0 suo        (501) staff       (20)       73 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/MANIFEST.in
--rw-r--r--   0 suo        (501) staff       (20)     4270 2023-04-28 21:55:20.258535 llama_index-0.6.0a1/PKG-INFO
--rw-r--r--   0 suo        (501) staff       (20)     4040 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/README.md
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.160961 llama_index-0.6.0a1/llama_index/
--rw-r--r--   0 suo        (501) staff       (20)       13 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/VERSION
--rw-r--r--   0 suo        (501) staff       (20)     4500 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      322 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/async_utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.164407 llama_index-0.6.0a1/llama_index/composability/
--rw-r--r--   0 suo        (501) staff       (20)      220 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/composability/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      171 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/composability/base.py
--rw-r--r--   0 suo        (501) staff       (20)     2739 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 suo        (501) staff       (20)      345 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/constants.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.168073 llama_index-0.6.0a1/llama_index/data_structs/
--rw-r--r--   0 suo        (501) staff       (20)      373 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    12377 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/data_structs.py
--rw-r--r--   0 suo        (501) staff       (20)     9476 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/data_structs_v2.py
--rw-r--r--   0 suo        (501) staff       (20)     6221 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/node_v2.py
--rw-r--r--   0 suo        (501) staff       (20)      779 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/registry.py
--rw-r--r--   0 suo        (501) staff       (20)     3256 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/struct_type.py
--rw-r--r--   0 suo        (501) staff       (20)      908 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/table.py
--rw-r--r--   0 suo        (501) staff       (20)     1032 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/table_v2.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.170420 llama_index-0.6.0a1/llama_index/embeddings/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     7721 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/base.py
--rw-r--r--   0 suo        (501) staff       (20)     1109 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/langchain.py
--rw-r--r--   0 suo        (501) staff       (20)    10103 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/openai.py
--rw-r--r--   0 suo        (501) staff       (20)      559 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.171742 llama_index-0.6.0a1/llama_index/evaluation/
--rw-r--r--   0 suo        (501) staff       (20)      259 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/evaluation/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    11972 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/evaluation/base.py
--rw-r--r--   0 suo        (501) staff       (20)     5344 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 suo        (501) staff       (20)      544 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/img_utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.174801 llama_index-0.6.0a1/llama_index/indices/
--rw-r--r--   0 suo        (501) staff       (20)      542 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     9024 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/base.py
--rw-r--r--   0 suo        (501) staff       (20)      897 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.175185 llama_index-0.6.0a1/llama_index/indices/common/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.176561 llama_index-0.6.0a1/llama_index/indices/common/struct_store/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     8114 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 suo        (501) staff       (20)      776 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 suo        (501) staff       (20)     2629 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.177215 llama_index-0.6.0a1/llama_index/indices/common_tree/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     7244 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.177978 llama_index-0.6.0a1/llama_index/indices/composability/
--rw-r--r--   0 suo        (501) staff       (20)      180 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/composability/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     3962 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.179065 llama_index-0.6.0a1/llama_index/indices/empty/
--rw-r--r--   0 suo        (501) staff       (20)      198 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/empty/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2151 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/empty/base.py
--rw-r--r--   0 suo        (501) staff       (20)     1176 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.180992 llama_index-0.6.0a1/llama_index/indices/keyword_table/
--rw-r--r--   0 suo        (501) staff       (20)      656 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     7652 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 suo        (501) staff       (20)      650 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 suo        (501) staff       (20)     5991 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 suo        (501) staff       (20)      844 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 suo        (501) staff       (20)     2264 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.181949 llama_index-0.6.0a1/llama_index/indices/knowledge_graph/
--rw-r--r--   0 suo        (501) staff       (20)      254 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     7816 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 suo        (501) staff       (20)     9543 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.183183 llama_index-0.6.0a1/llama_index/indices/list/
--rw-r--r--   0 suo        (501) staff       (20)      295 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/list/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     3305 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/list/base.py
--rw-r--r--   0 suo        (501) staff       (20)     3455 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/list/retrievers.py
--rw-r--r--   0 suo        (501) staff       (20)     3608 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/loading.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.185401 llama_index-0.6.0a1/llama_index/indices/postprocessor/
--rw-r--r--   0 suo        (501) staff       (20)      888 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)       83 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/base.py
--rw-r--r--   0 suo        (501) staff       (20)    11695 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 suo        (501) staff       (20)     8778 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 suo        (501) staff       (20)     4896 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 suo        (501) staff       (20)     8492 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.187738 llama_index-0.6.0a1/llama_index/indices/query/
--rw-r--r--   0 suo        (501) staff       (20)      137 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     1975 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/base.py
--rw-r--r--   0 suo        (501) staff       (20)     3386 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.189097 llama_index-0.6.0a1/llama_index/indices/query/query_transform/
--rw-r--r--   0 suo        (501) staff       (20)      281 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     8928 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 suo        (501) staff       (20)     5920 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 suo        (501) staff       (20)     8098 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 suo        (501) staff       (20)     1203 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/schema.py
--rw-r--r--   0 suo        (501) staff       (20)     1811 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/registry.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.190938 llama_index-0.6.0a1/llama_index/indices/response/
--rw-r--r--   0 suo        (501) staff       (20)      419 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/response/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    22075 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/response/response_builder.py
--rw-r--r--   0 suo        (501) staff       (20)      264 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/response/type.py
--rw-r--r--   0 suo        (501) staff       (20)     3310 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/service_context.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.195220 llama_index-0.6.0a1/llama_index/indices/struct_store/
--rw-r--r--   0 suo        (501) staff       (20)      622 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2115 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/base.py
--rw-r--r--   0 suo        (501) staff       (20)     5802 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 suo        (501) staff       (20)     2214 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 suo        (501) staff       (20)     4688 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 suo        (501) staff       (20)     5904 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 suo        (501) staff       (20)     5887 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.197948 llama_index-0.6.0a1/llama_index/indices/tree/
--rw-r--r--   0 suo        (501) staff       (20)      616 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     1612 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 suo        (501) staff       (20)     5834 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/base.py
--rw-r--r--   0 suo        (501) staff       (20)     7181 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/inserter.py
--rw-r--r--   0 suo        (501) staff       (20)     4663 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 suo        (501) staff       (20)    15299 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 suo        (501) staff       (20)     1402 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 suo        (501) staff       (20)     2005 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.198966 llama_index-0.6.0a1/llama_index/indices/vector_store/
--rw-r--r--   0 suo        (501) staff       (20)      260 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     8183 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/vector_store/base.py
--rw-r--r--   0 suo        (501) staff       (20)     3905 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.200969 llama_index-0.6.0a1/llama_index/langchain_helpers/
--rw-r--r--   0 suo        (501) staff       (20)       39 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.202399 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/
--rw-r--r--   0 suo        (501) staff       (20)      514 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2989 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 suo        (501) staff       (20)      837 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 suo        (501) staff       (20)     2211 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 suo        (501) staff       (20)      252 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)     7675 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)     3299 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)    17463 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.204454 llama_index-0.6.0a1/llama_index/llm_predictor/
--rw-r--r--   0 suo        (501) staff       (20)      330 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    10593 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/base.py
--rw-r--r--   0 suo        (501) staff       (20)     4275 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 suo        (501) staff       (20)     4732 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/stable_lm.py
--rw-r--r--   0 suo        (501) staff       (20)     2274 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.205141 llama_index-0.6.0a1/llama_index/logger/
--rw-r--r--   0 suo        (501) staff       (20)       95 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/logger/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      995 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/logger/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.206830 llama_index-0.6.0a1/llama_index/node_parser/
--rw-r--r--   0 suo        (501) staff       (20)      184 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/node_parser/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      530 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/node_parser/interface.py
--rw-r--r--   0 suo        (501) staff       (20)     3585 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/node_parser/node_utils.py
--rw-r--r--   0 suo        (501) staff       (20)     1821 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/node_parser/simple.py
--rw-r--r--   0 suo        (501) staff       (20)     4900 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/old_docstore.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.207639 llama_index-0.6.0a1/llama_index/optimization/
--rw-r--r--   0 suo        (501) staff       (20)      144 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/optimization/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     4301 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.209038 llama_index-0.6.0a1/llama_index/output_parsers/
--rw-r--r--   0 suo        (501) staff       (20)      230 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/output_parsers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      611 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/output_parsers/base.py
--rw-r--r--   0 suo        (501) staff       (20)     2742 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 suo        (501) staff       (20)     1828 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/output_parsers/langchain.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.209838 llama_index-0.6.0a1/llama_index/playground/
--rw-r--r--   0 suo        (501) staff       (20)      202 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/playground/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     6471 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/playground/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.212629 llama_index-0.6.0a1/llama_index/prompts/
--rw-r--r--   0 suo        (501) staff       (20)       87 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     6626 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/base.py
--rw-r--r--   0 suo        (501) staff       (20)     1969 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 suo        (501) staff       (20)     1134 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 suo        (501) staff       (20)    10843 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/default_prompts.py
--rw-r--r--   0 suo        (501) staff       (20)      992 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/prompt_type.py
--rw-r--r--   0 suo        (501) staff       (20)     7685 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/prompts.py
--rw-r--r--   0 suo        (501) staff       (20)        0 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/py.typed
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.214307 llama_index-0.6.0a1/llama_index/query_engine/
--rw-r--r--   0 suo        (501) staff       (20)      460 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     3572 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 suo        (501) staff       (20)     5814 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 suo        (501) staff       (20)     5322 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 suo        (501) staff       (20)     2967 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.222505 llama_index-0.6.0a1/llama_index/readers/
--rw-r--r--   0 suo        (501) staff       (20)     2974 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      659 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.223301 llama_index-0.6.0a1/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 suo        (501) staff       (20)      145 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2111 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 suo        (501) staff       (20)     3755 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/chroma.py
--rw-r--r--   0 suo        (501) staff       (20)     3328 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/database.py
--rw-r--r--   0 suo        (501) staff       (20)     3457 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/deeplake.py
--rw-r--r--   0 suo        (501) staff       (20)     4981 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/discord_reader.py
--rw-r--r--   0 suo        (501) staff       (20)     7775 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/download.py
--rw-r--r--   0 suo        (501) staff       (20)     2392 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/elasticsearch.py
--rw-r--r--   0 suo        (501) staff       (20)     2510 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/faiss.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.228542 llama_index-0.6.0a1/llama_index/readers/file/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     8527 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/base.py
--rw-r--r--   0 suo        (501) staff       (20)     1342 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/base_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     1629 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     1318 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3180 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     4106 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/image_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3222 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     1027 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3616 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3162 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3945 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3357 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     1770 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.230107 llama_index-0.6.0a1/llama_index/readers/github_readers/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    11730 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 suo        (501) staff       (20)    15928 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 suo        (501) staff       (20)     5473 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.231307 llama_index-0.6.0a1/llama_index/readers/google_readers/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     5659 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 suo        (501) staff       (20)     4989 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 suo        (501) staff       (20)     3708 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/json.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.231973 llama_index-0.6.0a1/llama_index/readers/make_com/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     1696 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)     1261 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/mbox.py
--rw-r--r--   0 suo        (501) staff       (20)     4588 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/milvus.py
--rw-r--r--   0 suo        (501) staff       (20)     2608 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/mongo.py
--rw-r--r--   0 suo        (501) staff       (20)     5541 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/myscale.py
--rw-r--r--   0 suo        (501) staff       (20)     5679 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/notion.py
--rw-r--r--   0 suo        (501) staff       (20)     1601 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/obsidian.py
--rw-r--r--   0 suo        (501) staff       (20)     2766 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/pinecone.py
--rw-r--r--   0 suo        (501) staff       (20)     3909 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/qdrant.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.233084 llama_index-0.6.0a1/llama_index/readers/schema/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/schema/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     1214 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/schema/base.py
--rw-r--r--   0 suo        (501) staff       (20)     7892 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/slack.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.234210 llama_index-0.6.0a1/llama_index/readers/steamship/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     3498 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 suo        (501) staff       (20)     1042 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/string_iterable.py
--rw-r--r--   0 suo        (501) staff       (20)     1918 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/twitter.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.236345 llama_index-0.6.0a1/llama_index/readers/weaviate/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     7766 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/weaviate/client.py
--rw-r--r--   0 suo        (501) staff       (20)     3986 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 suo        (501) staff       (20)     1867 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 suo        (501) staff       (20)     7987 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/web.py
--rw-r--r--   0 suo        (501) staff       (20)      981 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/wikipedia.py
--rw-r--r--   0 suo        (501) staff       (20)     1255 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.238506 llama_index-0.6.0a1/llama_index/response/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/response/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2039 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/response/notebook_utils.py
--rw-r--r--   0 suo        (501) staff       (20)     3071 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/response/schema.py
--rw-r--r--   0 suo        (501) staff       (20)      262 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/response/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.239630 llama_index-0.6.0a1/llama_index/retrievers/
--rw-r--r--   0 suo        (501) staff       (20)     1056 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/retrievers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     1066 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 suo        (501) staff       (20)     2768 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/schema.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.240739 llama_index-0.6.0a1/llama_index/storage/
--rw-r--r--   0 suo        (501) staff       (20)      124 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/__init__.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.245147 llama_index-0.6.0a1/llama_index/storage/docstore/
--rw-r--r--   0 suo        (501) staff       (20)      536 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     4825 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 suo        (501) staff       (20)     1408 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 suo        (501) staff       (20)      762 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/registry.py
--rw-r--r--   0 suo        (501) staff       (20)     2294 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 suo        (501) staff       (20)     2532 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/types.py
--rw-r--r--   0 suo        (501) staff       (20)      918 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.248036 llama_index-0.6.0a1/llama_index/storage/index_store/
--rw-r--r--   0 suo        (501) staff       (20)      301 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2224 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 suo        (501) staff       (20)     1341 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 suo        (501) staff       (20)     1508 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 suo        (501) staff       (20)      884 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/types.py
--rw-r--r--   0 suo        (501) staff       (20)      644 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.249673 llama_index-0.6.0a1/llama_index/storage/kvstore/
--rw-r--r--   0 suo        (501) staff       (20)      187 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     4061 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 suo        (501) staff       (20)     2330 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 suo        (501) staff       (20)      973 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/kvstore/types.py
--rw-r--r--   0 suo        (501) staff       (20)     3114 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/storage_context.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.251707 llama_index-0.6.0a1/llama_index/token_counter/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     4664 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)      722 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 suo        (501) staff       (20)     2874 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/token_counter.py
--rw-r--r--   0 suo        (501) staff       (20)      908 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.252495 llama_index-0.6.0a1/llama_index/tools/
--rw-r--r--   0 suo        (501) staff       (20)       13 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/tools/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      723 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/tools/file_utils.py
--rw-r--r--   0 suo        (501) staff       (20)       81 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/types.py
--rw-r--r--   0 suo        (501) staff       (20)     5847 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.258006 llama_index-0.6.0a1/llama_index/vector_stores/
--rw-r--r--   0 suo        (501) staff       (20)     1132 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     5240 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 suo        (501) staff       (20)     3947 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/chroma.py
--rw-r--r--   0 suo        (501) staff       (20)     8631 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 suo        (501) staff       (20)     4365 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/faiss.py
--rw-r--r--   0 suo        (501) staff       (20)    15768 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/milvus.py
--rw-r--r--   0 suo        (501) staff       (20)     8344 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/myscale.py
--rw-r--r--   0 suo        (501) staff       (20)     7186 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 suo        (501) staff       (20)    11419 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 suo        (501) staff       (20)     6505 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 suo        (501) staff       (20)     1973 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/registry.py
--rw-r--r--   0 suo        (501) staff       (20)     5084 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/simple.py
--rw-r--r--   0 suo        (501) staff       (20)     2210 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/types.py
--rw-r--r--   0 suo        (501) staff       (20)     3385 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/weaviate.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.163209 llama_index-0.6.0a1/llama_index.egg-info/
--rw-r--r--   0 suo        (501) staff       (20)     4270 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 suo        (501) staff       (20)     9542 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 suo        (501) staff       (20)        1 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 suo        (501) staff       (20)       96 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/requires.txt
--rw-r--r--   0 suo        (501) staff       (20)       12 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/top_level.txt
--rw-r--r--   0 suo        (501) staff       (20)       38 2023-04-28 21:55:20.258999 llama_index-0.6.0a1/setup.cfg
--rw-r--r--   0 suo        (501) staff       (20)     1130 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/setup.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.174981 llama_index-0.6.0a2/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1064 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/LICENSE
+-rw-r--r--   0 jerryliu   (501) staff       (20)       73 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/MANIFEST.in
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-04-29 16:25:25.174866 llama_index-0.6.0a2/PKG-INFO
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4124 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/README.md
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.149320 llama_index-0.6.0a2/llama_index/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       13 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/VERSION
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4719 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      322 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/async_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.150040 llama_index-0.6.0a2/llama_index/composability/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      220 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/composability/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      171 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/composability/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2739 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      219 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/constants.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.150864 llama_index-0.6.0a2/llama_index/data_structs/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      409 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    12377 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9476 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/data_structs_v2.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      264 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/node_mapping.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6221 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/node_v2.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      779 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3256 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/table.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1032 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/data_structs/table_v2.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.151315 llama_index-0.6.0a2/llama_index/embeddings/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/embeddings/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7721 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/embeddings/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1109 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/embeddings/langchain.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10103 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/embeddings/openai.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      559 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/embeddings/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.151604 llama_index-0.6.0a2/llama_index/evaluation/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/evaluation/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11972 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/evaluation/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5344 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      544 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/img_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.152468 llama_index-0.6.0a2/llama_index/indices/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      542 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9024 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      897 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.152585 llama_index-0.6.0a2/llama_index/indices/common/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.153032 llama_index-0.6.0a2/llama_index/indices/common/struct_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8114 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      776 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2629 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.153279 llama_index-0.6.0a2/llama_index/indices/common_tree/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7244 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.153626 llama_index-0.6.0a2/llama_index/indices/composability/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      180 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3962 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.154080 llama_index-0.6.0a2/llama_index/indices/empty/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      198 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2151 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/empty/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1176 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.154949 llama_index-0.6.0a2/llama_index/indices/keyword_table/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      656 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7652 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      650 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5891 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      844 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2264 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.155352 llama_index-0.6.0a2/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      254 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7816 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9543 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.155770 llama_index-0.6.0a2/llama_index/indices/list/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      295 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/list/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3305 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/list/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3455 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3608 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/loading.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.156504 llama_index-0.6.0a2/llama_index/indices/postprocessor/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      888 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)       83 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/postprocessor/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11695 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8778 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4896 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8492 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.157147 llama_index-0.6.0a2/llama_index/indices/query/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      137 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/query/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1975 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/query/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3386 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.157506 llama_index-0.6.0a2/llama_index/indices/query/query_transform/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      281 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8928 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5920 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8098 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1203 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/query/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1811 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/registry.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.157932 llama_index-0.6.0a2/llama_index/indices/response/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      419 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/response/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    22074 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/response/type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3296 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/service_context.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.158814 llama_index-0.6.0a2/llama_index/indices/struct_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      622 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2115 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5802 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2214 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4688 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5904 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5887 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.159588 llama_index-0.6.0a2/llama_index/indices/tree/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      616 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1612 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5834 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/tree/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7181 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4663 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15299 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1402 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2005 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.159909 llama_index-0.6.0a2/llama_index/indices/vector_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      260 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8183 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/vector_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3987 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.160471 llama_index-0.6.0a2/llama_index/langchain_helpers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       39 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.160957 llama_index-0.6.0a2/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      514 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2989 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      837 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2211 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      252 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7675 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3299 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    17585 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.161518 llama_index-0.6.0a2/llama_index/llm_predictor/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      330 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10593 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/llm_predictor/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4275 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4732 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/llm_predictor/stable_lm.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2274 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.161718 llama_index-0.6.0a2/llama_index/logger/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       95 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/logger/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      995 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/logger/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.162086 llama_index-0.6.0a2/llama_index/node_parser/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      184 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/node_parser/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      530 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/node_parser/interface.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3585 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1821 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/node_parser/simple.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.162296 llama_index-0.6.0a2/llama_index/optimization/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      144 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/optimization/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4301 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.162717 llama_index-0.6.0a2/llama_index/output_parsers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      230 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      611 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/output_parsers/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2742 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1828 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/output_parsers/langchain.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.162892 llama_index-0.6.0a2/llama_index/playground/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      202 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/playground/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6471 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/playground/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.163540 llama_index-0.6.0a2/llama_index/prompts/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       87 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/prompts/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6626 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/prompts/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1969 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1134 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10843 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      992 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7685 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/prompts/prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/py.typed
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.164000 llama_index-0.6.0a2/llama_index/query_engine/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      460 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/query_engine/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3572 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5814 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5322 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2967 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.166664 llama_index-0.6.0a2/llama_index/readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2974 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      659 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.166874 llama_index-0.6.0a2/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      145 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2111 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3755 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/chroma.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3328 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/database.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3457 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/deeplake.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4981 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/discord_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7775 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/download.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2392 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2510 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/faiss.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.168363 llama_index-0.6.0a2/llama_index/readers/file/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8527 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1342 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1629 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1318 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3180 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4106 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3222 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1027 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3616 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3162 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3945 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3357 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1770 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.168792 llama_index-0.6.0a2/llama_index/readers/github_readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11730 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15928 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5473 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.169097 llama_index-0.6.0a2/llama_index/readers/google_readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5659 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4989 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3708 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/json.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.169309 llama_index-0.6.0a2/llama_index/readers/make_com/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1696 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1261 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/mbox.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4588 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/milvus.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2608 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/mongo.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5541 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/myscale.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5679 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/notion.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1601 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/obsidian.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2766 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/pinecone.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3909 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/qdrant.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.169502 llama_index-0.6.0a2/llama_index/readers/schema/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1214 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/schema/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7892 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/slack.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.169690 llama_index-0.6.0a2/llama_index/readers/steamship/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3498 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1042 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/string_iterable.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1918 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/twitter.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.170079 llama_index-0.6.0a2/llama_index/readers/weaviate/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7766 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3986 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1867 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7987 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/web.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      981 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/wikipedia.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1255 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.170443 llama_index-0.6.0a2/llama_index/response/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/response/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2039 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/response/notebook_utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3071 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/response/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/response/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.170631 llama_index-0.6.0a2/llama_index/retrievers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1258 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/retrievers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1066 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2768 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/schema.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.170822 llama_index-0.6.0a2/llama_index/storage/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      124 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.171518 llama_index-0.6.0a2/llama_index/storage/docstore/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      536 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4825 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1408 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      762 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2294 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2532 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/docstore/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      918 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.172120 llama_index-0.6.0a2/llama_index/storage/index_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      301 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2224 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1341 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1508 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      884 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/index_store/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      644 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.172504 llama_index-0.6.0a2/llama_index/storage/kvstore/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      187 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4061 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2330 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      973 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3114 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/storage/storage_context.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.173084 llama_index-0.6.0a2/llama_index/token_counter/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/token_counter/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4664 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      722 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2874 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/token_counter/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.173292 llama_index-0.6.0a2/llama_index/tools/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       13 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/tools/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      723 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/tools/file_utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)       81 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5847 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.174710 llama_index-0.6.0a2/llama_index/vector_stores/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1132 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5240 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3947 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8631 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4365 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15768 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8344 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7186 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11419 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6505 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1973 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5084 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/simple.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2210 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3385 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/llama_index/vector_stores/weaviate.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-04-29 16:25:25.149765 llama_index-0.6.0a2/llama_index.egg-info/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-04-29 16:25:25.000000 llama_index-0.6.0a2/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9555 2023-04-29 16:25:25.000000 llama_index-0.6.0a2/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)        1 2023-04-29 16:25:25.000000 llama_index-0.6.0a2/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       96 2023-04-29 16:25:25.000000 llama_index-0.6.0a2/llama_index.egg-info/requires.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       12 2023-04-29 16:25:25.000000 llama_index-0.6.0a2/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       38 2023-04-29 16:25:25.175011 llama_index-0.6.0a2/setup.cfg
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1130 2023-04-29 16:25:24.000000 llama_index-0.6.0a2/setup.py
```

### Comparing `llama_index-0.6.0a1/LICENSE` & `llama_index-0.6.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/PKG-INFO` & `llama_index-0.6.0a2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: llama_index
-Version: 0.6.0a1
+Version: 0.6.0a2
 Summary: Interface between LLMs and your data.
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
 PyPi: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
-Documentation: https://gpt-index.readthedocs.io/en/latest/.
+Documentation:
+- v0.6 (pre-release): https://gpt-index.readthedocs.io/en/latest/.
+- v0.5 (stable): https://gpt-index.readthedocs.io/en/v0.5.27/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
 ### Ecosystem
 
 - LlamaHub (community library of data loaders): https://llamahub.ai
-- Llama Lab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
+- LlamaLab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
 
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
```

### Comparing `llama_index-0.6.0a1/README.md` & `llama_index-0.6.0a2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
 PyPi: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
-Documentation: https://gpt-index.readthedocs.io/en/latest/.
+Documentation:
+- v0.6 (pre-release): https://gpt-index.readthedocs.io/en/latest/.
+- v0.5 (stable): https://gpt-index.readthedocs.io/en/v0.5.27/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
 ### Ecosystem
 
 - LlamaHub (community library of data loaders): https://llamahub.ai
-- Llama Lab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
+- LlamaLab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
 
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
```

### Comparing `llama_index-0.6.0a1/llama_index/__init__.py` & `llama_index-0.6.0a2/llama_index/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,14 +97,20 @@
 # loading
 from llama_index.indices.loading import (
     load_graph_from_storage,
     load_index_from_storage,
     load_indices_from_storage,
 )
 
+# QueryBundle
+from llama_index.indices.query.schema import QueryBundle
+
+# Response Synthesizer
+from llama_index.indices.query.response_synthesis import ResponseSynthesizer
+
 # best practices for library logging:
 # https://docs.python.org/3/howto/logging.html#configuring-logging-for-a-library
 logging.getLogger(__name__).addHandler(NullHandler())
 
 
 __all__ = [
     "StorageContext",
@@ -164,11 +170,13 @@
     "IndexStructType",
     "TwitterTweetReader",
     "download_loader",
     "GithubRepositoryReader",
     "load_graph_from_storage",
     "load_index_from_storage",
     "load_indices_from_storage",
+    "QueryBundle",
+    "ResponseSynthesizer",
 ]
 
 # NOTE: keep for backwards compatibility
 SQLContextBuilder = SQLDocumentContextBuilder
```

### Comparing `llama_index-0.6.0a1/llama_index/composability/joint_qa_summary.py` & `llama_index-0.6.0a2/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/data_structs/data_structs.py` & `llama_index-0.6.0a2/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/data_structs/data_structs_v2.py` & `llama_index-0.6.0a2/llama_index/data_structs/data_structs_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/data_structs/node_v2.py` & `llama_index-0.6.0a2/llama_index/data_structs/node_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/data_structs/registry.py` & `llama_index-0.6.0a2/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/data_structs/struct_type.py` & `llama_index-0.6.0a2/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/data_structs/table.py` & `llama_index-0.6.0a2/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/data_structs/table_v2.py` & `llama_index-0.6.0a2/llama_index/data_structs/table_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/embeddings/base.py` & `llama_index-0.6.0a2/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/embeddings/langchain.py` & `llama_index-0.6.0a2/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/embeddings/openai.py` & `llama_index-0.6.0a2/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/embeddings/utils.py` & `llama_index-0.6.0a2/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/evaluation/base.py` & `llama_index-0.6.0a2/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/evaluation/dataset_generation.py` & `llama_index-0.6.0a2/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/img_utils.py` & `llama_index-0.6.0a2/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/__init__.py` & `llama_index-0.6.0a2/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/base.py` & `llama_index-0.6.0a2/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/base_retriever.py` & `llama_index-0.6.0a2/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/common/struct_store/base.py` & `llama_index-0.6.0a2/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.6.0a2/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.6.0a2/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/common_tree/base.py` & `llama_index-0.6.0a2/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/composability/graph.py` & `llama_index-0.6.0a2/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/empty/base.py` & `llama_index-0.6.0a2/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/empty/retrievers.py` & `llama_index-0.6.0a2/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.6.0a2/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/keyword_table/base.py` & `llama_index-0.6.0a2/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.6.0a2/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.6.0a2/llama_index/indices/keyword_table/retrievers.py`

 * *Files 12% similar despite different names*

```diff
@@ -108,16 +108,15 @@
 
         return sorted_nodes_with_scores
 
 
 class KeywordTableGPTRetriever(BaseKeywordTableRetriever):
     """Keyword Table Index GPT Retriever.
 
-    Extracts keywords using GPT. Set when `mode="default"` in `query` method of
-    `GPTKeywordTableIndex`.
+    Extracts keywords using GPT. Set when using `retriever_mode="default"`.
 
     See BaseGPTKeywordTableQuery for arguments.
 
     """
 
     def _get_keywords(self, query_str: str) -> List[str]:
         """Extract keywords."""
@@ -130,15 +129,15 @@
         return list(keywords)
 
 
 class KeywordTableSimpleRetriever(BaseKeywordTableRetriever):
     """Keyword Table Index Simple Retriever.
 
     Extracts keywords using simple regex-based keyword extractor.
-    Set when `mode="simple"` in `query` method of `GPTKeywordTableIndex`.
+    Set when `retriever_mode="simple"`.
 
     See BaseGPTKeywordTableQuery for arguments.
 
     """
 
     def _get_keywords(self, query_str: str) -> List[str]:
         """Extract keywords."""
@@ -147,15 +146,15 @@
         )
 
 
 class KeywordTableRAKERetriever(BaseKeywordTableRetriever):
     """Keyword Table Index RAKE Retriever.
 
     Extracts keywords using RAKE keyword extractor.
-    Set when `mode="rake"` in `query` method of `GPTKeywordTableIndex`.
+    Set when `retriever_mode="rake"`.
 
     See BaseGPTKeywordTableQuery for arguments.
 
     """
 
     def _get_keywords(self, query_str: str) -> List[str]:
         """Extract keywords."""
```

### Comparing `llama_index-0.6.0a1/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.6.0a2/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/keyword_table/utils.py` & `llama_index-0.6.0a2/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.6.0a2/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/knowledge_graph/retrievers.py` & `llama_index-0.6.0a2/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/list/base.py` & `llama_index-0.6.0a2/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/list/retrievers.py` & `llama_index-0.6.0a2/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/loading.py` & `llama_index-0.6.0a2/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.6.0a2/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/postprocessor/node.py` & `llama_index-0.6.0a2/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.6.0a2/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/postprocessor/pii.py` & `llama_index-0.6.0a2/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/prompt_helper.py` & `llama_index-0.6.0a2/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/query/base.py` & `llama_index-0.6.0a2/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/query/embedding_utils.py` & `llama_index-0.6.0a2/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/query/query_transform/base.py` & `llama_index-0.6.0a2/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.6.0a2/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/query/response_synthesis.py` & `llama_index-0.6.0a2/llama_index/indices/query/response_synthesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         cls,
         service_context: Optional[ServiceContext] = None,
         streaming: bool = False,
         use_async: bool = False,
         text_qa_template: Optional[QuestionAnswerPrompt] = None,
         refine_template: Optional[RefinePrompt] = None,
         simple_template: Optional[SimpleInputPrompt] = None,
-        response_mode: ResponseMode = ResponseMode.DEFAULT,
+        response_mode: ResponseMode = ResponseMode.COMPACT,
         response_kwargs: Optional[Dict] = None,
         node_postprocessors: Optional[List[BaseNodePostprocessor]] = None,
         optimizer: Optional[BaseTokenUsageOptimizer] = None,
         verbose: bool = False,
     ) -> "ResponseSynthesizer":
         """Initialize response synthesizer from args.
```

### Comparing `llama_index-0.6.0a1/llama_index/indices/query/schema.py` & `llama_index-0.6.0a2/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/registry.py` & `llama_index-0.6.0a2/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/response/response_builder.py` & `llama_index-0.6.0a2/llama_index/indices/response/response_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,22 +572,22 @@
 
 
 def get_response_builder(
     service_context: ServiceContext,
     text_qa_template: Optional[QuestionAnswerPrompt] = None,
     refine_template: Optional[RefinePrompt] = None,
     simple_template: Optional[SimpleInputPrompt] = None,
-    mode: ResponseMode = ResponseMode.DEFAULT,
+    mode: ResponseMode = ResponseMode.COMPACT,
     use_async: bool = False,
     streaming: bool = False,
 ) -> BaseResponseBuilder:
     text_qa_template = text_qa_template or DEFAULT_TEXT_QA_PROMPT
     refine_template = refine_template or DEFAULT_REFINE_PROMPT_SEL
     simple_template = simple_template or DEFAULT_SIMPLE_INPUT_PROMPT
-    if mode == ResponseMode.DEFAULT:
+    if mode == ResponseMode.REFINE:
         return Refine(
             service_context=service_context,
             text_qa_template=text_qa_template,
             refine_template=refine_template,
             streaming=streaming,
         )
     elif mode == ResponseMode.COMPACT:
```

### Comparing `llama_index-0.6.0a1/llama_index/indices/service_context.py` & `llama_index-0.6.0a2/llama_index/indices/service_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from llama_index.node_parser.interface import NodeParser
 from llama_index.node_parser.simple import SimpleNodeParser
 
 
 def _get_default_node_parser(chunk_size_limit: Optional[int] = None) -> NodeParser:
     """Get default node parser."""
     if chunk_size_limit is None:
-        # use default chunk size (3900)
-        token_text_splitter = TokenTextSplitter()
+        token_text_splitter = TokenTextSplitter()  # use default chunk size
     else:
         token_text_splitter = TokenTextSplitter(chunk_size=chunk_size_limit)
     return SimpleNodeParser(text_splitter=token_text_splitter)
 
 
 @dataclass
 class ServiceContext:
```

### Comparing `llama_index-0.6.0a1/llama_index/indices/struct_store/__init__.py` & `llama_index-0.6.0a2/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/struct_store/base.py` & `llama_index-0.6.0a2/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.6.0a2/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/struct_store/pandas.py` & `llama_index-0.6.0a2/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/struct_store/pandas_query.py` & `llama_index-0.6.0a2/llama_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/struct_store/sql.py` & `llama_index-0.6.0a2/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.6.0a2/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/tree/__init__.py` & `llama_index-0.6.0a2/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.6.0a2/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/tree/base.py` & `llama_index-0.6.0a2/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/tree/inserter.py` & `llama_index-0.6.0a2/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.6.0a2/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.6.0a2/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.6.0a2/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/utils.py` & `llama_index-0.6.0a2/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/vector_store/base.py` & `llama_index-0.6.0a2/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/indices/vector_store/retrievers.py` & `llama_index-0.6.0a2/llama_index/indices/vector_store/retrievers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Base vector store index query."""
 
 
 from typing import Any, List, Optional
+from llama_index.constants import DEFAULT_SIMILARITY_TOP_K
 
 from llama_index.data_structs.data_structs_v2 import IndexDict
 
 from llama_index.data_structs.node_v2 import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.utils import log_vector_store_query_result
@@ -26,15 +27,15 @@
         vector_store (Optional[VectorStore]): vector store
 
     """
 
     def __init__(
         self,
         index: GPTVectorStoreIndex,
-        similarity_top_k: int = 1,
+        similarity_top_k: int = DEFAULT_SIMILARITY_TOP_K,
         vector_store_query_mode: str = VectorStoreQueryMode.DEFAULT,
         alpha: Optional[float] = None,
         doc_ids: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
         self._index = index
```

### Comparing `llama_index-0.6.0a1/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.6.0a2/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.6.0a2/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.6.0a2/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.6.0a2/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.6.0a2/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.6.0a2/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.6.0a2/llama_index/langchain_helpers/text_splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Text splitter implementations."""
 from dataclasses import dataclass
 from typing import Callable, List, Optional
 
 from langchain.text_splitter import TextSplitter
+from llama_index.constants import DEFAULT_CHUNK_OVERLAP, DEFAULT_CHUNK_SIZE
 
 from llama_index.utils import globals_helper
 
 
 @dataclass
 class TextSplit:
     """Text split with overlap.
@@ -22,16 +23,16 @@
 
 class TokenTextSplitter(TextSplitter):
     """Implementation of splitting text that looks at word tokens."""
 
     def __init__(
         self,
         separator: str = " ",
-        chunk_size: int = 3900,
-        chunk_overlap: int = 200,
+        chunk_size: int = DEFAULT_CHUNK_SIZE,
+        chunk_overlap: int = DEFAULT_CHUNK_OVERLAP,
         tokenizer: Optional[Callable] = None,
         backup_separators: Optional[List[str]] = ["\n"],
     ):
         """Initialize with parameters."""
         if chunk_overlap > chunk_size:
             raise ValueError(
                 f"Got a larger chunk overlap ({chunk_overlap}) than chunk size "
@@ -243,15 +244,15 @@
     compared to the original TokenTextSplitter, there are less likely to be
     hanging sentences or parts of sentences at the end of the node chunk.
     """
 
     def __init__(
         self,
         separator: str = " ",
-        chunk_size: int = 4000,
+        chunk_size: int = DEFAULT_CHUNK_SIZE,
         chunk_overlap: int = 200,
         tokenizer: Optional[Callable] = None,
         backup_separators: Optional[List[str]] = ["\n"],
         paragraph_separator: Optional[str] = "\n\n\n",
         chunking_tokenizer_fn: Optional[Callable[[str], List[str]]] = None,
         secondary_chunking_regex: Optional[str] = "[^,.;。]+[,.;。]?",
     ):
```

### Comparing `llama_index-0.6.0a1/llama_index/llm_predictor/base.py` & `llama_index-0.6.0a2/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/llm_predictor/chatgpt.py` & `llama_index-0.6.0a2/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/llm_predictor/stable_lm.py` & `llama_index-0.6.0a2/llama_index/llm_predictor/stable_lm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/llm_predictor/structured.py` & `llama_index-0.6.0a2/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/logger/base.py` & `llama_index-0.6.0a2/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/node_parser/interface.py` & `llama_index-0.6.0a2/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/node_parser/node_utils.py` & `llama_index-0.6.0a2/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/node_parser/simple.py` & `llama_index-0.6.0a2/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/optimization/optimizer.py` & `llama_index-0.6.0a2/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/output_parsers/base.py` & `llama_index-0.6.0a2/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/output_parsers/guardrails.py` & `llama_index-0.6.0a2/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/output_parsers/langchain.py` & `llama_index-0.6.0a2/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/playground/base.py` & `llama_index-0.6.0a2/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/prompts/base.py` & `llama_index-0.6.0a2/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/prompts/chat_prompts.py` & `llama_index-0.6.0a2/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.6.0a2/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/prompts/default_prompts.py` & `llama_index-0.6.0a2/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/prompts/prompt_type.py` & `llama_index-0.6.0a2/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/prompts/prompts.py` & `llama_index-0.6.0a2/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.6.0a2/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.6.0a2/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.6.0a2/llama_index/query_engine/retriever_query_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def from_args(
         cls,
         retriever: BaseRetriever,
         service_context: Optional[ServiceContext] = None,
         node_postprocessors: Optional[List[BaseNodePostprocessor]] = None,
         verbose: bool = False,
         # response synthesizer args
-        response_mode: ResponseMode = ResponseMode.DEFAULT,
+        response_mode: ResponseMode = ResponseMode.COMPACT,
         text_qa_template: Optional[QuestionAnswerPrompt] = None,
         refine_template: Optional[RefinePrompt] = None,
         simple_template: Optional[SimpleInputPrompt] = None,
         response_kwargs: Optional[Dict] = None,
         use_async: bool = False,
         streaming: bool = False,
         optimizer: Optional[BaseTokenUsageOptimizer] = None,
```

### Comparing `llama_index-0.6.0a1/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.6.0a2/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/__init__.py` & `llama_index-0.6.0a2/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/base.py` & `llama_index-0.6.0a2/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.6.0a2/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/chroma.py` & `llama_index-0.6.0a2/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/database.py` & `llama_index-0.6.0a2/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/deeplake.py` & `llama_index-0.6.0a2/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/discord_reader.py` & `llama_index-0.6.0a2/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/download.py` & `llama_index-0.6.0a2/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/elasticsearch.py` & `llama_index-0.6.0a2/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/faiss.py` & `llama_index-0.6.0a2/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/base.py` & `llama_index-0.6.0a2/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/base_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/docs_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/epub_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/image_caption_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/image_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/image_vision_llm_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/ipynb_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/markdown_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/mbox_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/slides_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/tabular_parser.py` & `llama_index-0.6.0a2/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/file/video_audio.py` & `llama_index-0.6.0a2/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.6.0a2/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.6.0a2/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/github_readers/utils.py` & `llama_index-0.6.0a2/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.6.0a2/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.6.0a2/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/json.py` & `llama_index-0.6.0a2/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/make_com/wrapper.py` & `llama_index-0.6.0a2/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/mbox.py` & `llama_index-0.6.0a2/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/milvus.py` & `llama_index-0.6.0a2/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/mongo.py` & `llama_index-0.6.0a2/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/myscale.py` & `llama_index-0.6.0a2/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/notion.py` & `llama_index-0.6.0a2/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/obsidian.py` & `llama_index-0.6.0a2/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/pinecone.py` & `llama_index-0.6.0a2/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/qdrant.py` & `llama_index-0.6.0a2/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/schema/base.py` & `llama_index-0.6.0a2/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/slack.py` & `llama_index-0.6.0a2/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/steamship/file_reader.py` & `llama_index-0.6.0a2/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/string_iterable.py` & `llama_index-0.6.0a2/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/twitter.py` & `llama_index-0.6.0a2/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/weaviate/client.py` & `llama_index-0.6.0a2/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/weaviate/reader.py` & `llama_index-0.6.0a2/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/weaviate/utils.py` & `llama_index-0.6.0a2/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/web.py` & `llama_index-0.6.0a2/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/wikipedia.py` & `llama_index-0.6.0a2/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/readers/youtube_transcript.py` & `llama_index-0.6.0a2/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/response/notebook_utils.py` & `llama_index-0.6.0a2/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/response/schema.py` & `llama_index-0.6.0a2/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/retrievers/transform_retriever.py` & `llama_index-0.6.0a2/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/schema.py` & `llama_index-0.6.0a2/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/docstore/__init__.py` & `llama_index-0.6.0a2/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.6.0a2/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.6.0a2/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/docstore/registry.py` & `llama_index-0.6.0a2/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.6.0a2/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/docstore/types.py` & `llama_index-0.6.0a2/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/docstore/utils.py` & `llama_index-0.6.0a2/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.6.0a2/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.6.0a2/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.6.0a2/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/index_store/types.py` & `llama_index-0.6.0a2/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/index_store/utils.py` & `llama_index-0.6.0a2/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.6.0a2/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.6.0a2/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/kvstore/types.py` & `llama_index-0.6.0a2/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/storage/storage_context.py` & `llama_index-0.6.0a2/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index-0.6.0a2/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.6.0a2/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/token_counter/token_counter.py` & `llama_index-0.6.0a2/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/token_counter/utils.py` & `llama_index-0.6.0a2/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/tools/file_utils.py` & `llama_index-0.6.0a2/llama_index/tools/file_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/utils.py` & `llama_index-0.6.0a2/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/__init__.py` & `llama_index-0.6.0a2/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.6.0a2/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/chroma.py` & `llama_index-0.6.0a2/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/deeplake.py` & `llama_index-0.6.0a2/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/faiss.py` & `llama_index-0.6.0a2/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/milvus.py` & `llama_index-0.6.0a2/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/myscale.py` & `llama_index-0.6.0a2/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/opensearch.py` & `llama_index-0.6.0a2/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/pinecone.py` & `llama_index-0.6.0a2/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/qdrant.py` & `llama_index-0.6.0a2/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/registry.py` & `llama_index-0.6.0a2/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/simple.py` & `llama_index-0.6.0a2/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/types.py` & `llama_index-0.6.0a2/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index/vector_stores/weaviate.py` & `llama_index-0.6.0a2/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a1/llama_index.egg-info/PKG-INFO` & `llama_index-0.6.0a2/llama_index.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: llama-index
-Version: 0.6.0a1
+Version: 0.6.0a2
 Summary: Interface between LLMs and your data.
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
 PyPi: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
-Documentation: https://gpt-index.readthedocs.io/en/latest/.
+Documentation:
+- v0.6 (pre-release): https://gpt-index.readthedocs.io/en/latest/.
+- v0.5 (stable): https://gpt-index.readthedocs.io/en/v0.5.27/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
 ### Ecosystem
 
 - LlamaHub (community library of data loaders): https://llamahub.ai
-- Llama Lab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
+- LlamaLab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
 
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
```

### Comparing `llama_index-0.6.0a1/llama_index.egg-info/SOURCES.txt` & `llama_index-0.6.0a2/llama_index.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 setup.py
 llama_index/VERSION
 llama_index/__init__.py
 llama_index/async_utils.py
 llama_index/constants.py
 llama_index/img_utils.py
-llama_index/old_docstore.py
 llama_index/py.typed
 llama_index/schema.py
 llama_index/types.py
 llama_index/utils.py
 llama_index.egg-info/PKG-INFO
 llama_index.egg-info/SOURCES.txt
 llama_index.egg-info/dependency_links.txt
@@ -19,14 +18,15 @@
 llama_index.egg-info/top_level.txt
 llama_index/composability/__init__.py
 llama_index/composability/base.py
 llama_index/composability/joint_qa_summary.py
 llama_index/data_structs/__init__.py
 llama_index/data_structs/data_structs.py
 llama_index/data_structs/data_structs_v2.py
+llama_index/data_structs/node_mapping.py
 llama_index/data_structs/node_v2.py
 llama_index/data_structs/registry.py
 llama_index/data_structs/struct_type.py
 llama_index/data_structs/table.py
 llama_index/data_structs/table_v2.py
 llama_index/embeddings/__init__.py
 llama_index/embeddings/base.py
```

### Comparing `llama_index-0.6.0a1/setup.py` & `llama_index-0.6.0a2/setup.py`

 * *Files identical despite different names*

