# Comparing `tmp/debater_python_api-4.3.1.tar.gz` & `tmp/debater_python_api-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debater_python_api-4.3.1.tar", last modified: Sun Apr  2 14:32:15 2023, max compression
+gzip compressed data, was "debater_python_api-4.3.2.tar", last modified: Sun Apr 30 13:43:43 2023, max compression
```

## Comparing `debater_python_api-4.3.1.tar` & `debater_python_api-4.3.2.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.580056 debater_python_api-4.3.1/
--rw-r--r--   0 lilache    (501) staff       (20)    11358 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/LICENSE
--rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-04-02 14:32:15.579828 debater_python_api-4.3.1/PKG-INFO
--rw-r--r--   0 lilache    (501) staff       (20)      169 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/README.md
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.565736 debater_python_api-4.3.1/debater_python_api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.566763 debater_python_api-4.3.1/debater_python_api/api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.569477 debater_python_api-4.3.1/debater_python_api/api/clients/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     4503 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/abstract_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1147 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/argument_quality_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1548 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/claim_and_evidence_detection_client.py
--rw-r--r--   0 lilache    (501) staff       (20)      934 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/claim_boundaries_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     6203 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/clustering_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3034 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/embedding_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1999 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/index_searcher_client.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.570397 debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/
--rw-r--r--   0 lilache    (501) staff       (20)    28620 2023-04-02 13:19:13.000000 debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/KpAnalysisUtils.py
--rw-r--r--   0 lilache    (501) staff       (20)      136 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/KpaExceptions.py
--rw-r--r--   0 lilache    (501) staff       (20)    17249 2023-04-02 14:02:37.000000 debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/KpaResult.py
--rw-r--r--   0 lilache    (501) staff       (20)    12256 2023-04-02 08:06:05.000000 debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/docx_generator.py
--rw-r--r--   0 lilache    (501) staff       (20)     1711 2023-01-30 15:29:08.000000 debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/utils.py
--rw-r--r--   0 lilache    (501) staff       (20)     6234 2023-01-30 15:29:08.000000 debater_python_api-4.3.1/debater_python_api/api/clients/keypoints_admin_client.py
--rw-r--r--   0 lilache    (501) staff       (20)    27847 2023-04-02 13:47:03.000000 debater_python_api-4.3.1/debater_python_api/api/clients/keypoints_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1894 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/keypoints_pairs_infer_client.py
--rw-r--r--   0 lilache    (501) staff       (20)    13830 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/narrative_generation_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1230 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/pro_con_client.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.570721 debater_python_api-4.3.1/debater_python_api/api/clients/response_data/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/response_data/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     1597 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/response_data/speech_response.py
--rw-r--r--   0 lilache    (501) staff       (20)     1790 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/term_relater_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1563 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/term_wikifier_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3394 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/clients/theme_extraction_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3270 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/debater_api.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.570898 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.573639 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      142 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
--rw-r--r--   0 lilache    (501) staff       (20)     5079 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/elastic_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1001 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
--rw-r--r--   0 lilache    (501) staff       (20)     1314 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
--rw-r--r--   0 lilache    (501) staff       (20)     3576 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
--rw-r--r--   0 lilache    (501) staff       (20)     1516 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.576811 debater_python_api-4.3.1/debater_python_api/examples/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      803 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/argument_quality_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      854 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/claim_boundaries_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1002 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/claim_detection_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      932 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/clustering_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      860 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/embedding_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1014 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/evidence_detection_example.py
--rw-r--r--   0 lilache    (501) staff       (20)    85859 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/example_of_sc_args.py
--rw-r--r--   0 lilache    (501) staff       (20)     1480 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/index_searcher_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1173 2023-04-02 11:19:29.000000 debater_python_api-4.3.1/debater_python_api/examples/keypoints_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1428 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/pro_con_example.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.577270 debater_python_api-4.3.1/debater_python_api/examples/resources/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/resources/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)    23817 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/resources/arguments.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.577419 debater_python_api-4.3.1/debater_python_api/examples/resources/filters_output/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/resources/filters_output/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     2530 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/resources/pro_con_scores.py
--rw-r--r--   0 lilache    (501) staff       (20)     9581 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/run_all_services.py
--rw-r--r--   0 lilache    (501) staff       (20)      870 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/speech_construction_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      480 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/term_relater_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      907 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/term_wikifier_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1154 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/theme_extraction_example.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.577835 debater_python_api-4.3.1/debater_python_api/examples/usecases/
--rw-r--r--   0 lilache    (501) staff       (20)     4943 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/usecases/kp_based_survey.py
--rw-r--r--   0 lilache    (501) staff       (20)     6036 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/usecases/mining_to_narrative.py
--rw-r--r--   0 lilache    (501) staff       (20)    10191 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/examples/usecases/survey.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.577983 debater_python_api-4.3.1/debater_python_api/integration_tests/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/integration_tests/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.578102 debater_python_api-4.3.1/debater_python_api/integration_tests/api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/integration_tests/api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.578903 debater_python_api-4.3.1/debater_python_api/integration_tests/api/clients/
--rw-r--r--   0 lilache    (501) staff       (20)     2708 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
--rw-r--r--   0 lilache    (501) staff       (20)    11539 2023-04-02 08:34:25.000000 debater_python_api-4.3.1/debater_python_api/integration_tests/api/clients/ServicesIT.py
--rw-r--r--   0 lilache    (501) staff       (20)     4630 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/integration_tests/api/clients/ServicesLoad.py
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/integration_tests/api/clients/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.579590 debater_python_api-4.3.1/debater_python_api/utils/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/utils/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      992 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/utils/clusters_refiner.py
--rw-r--r--   0 lilache    (501) staff       (20)     1574 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/utils/general_utils.py
--rw-r--r--   0 lilache    (501) staff       (20)      604 2022-12-12 10:25:59.000000 debater_python_api-4.3.1/debater_python_api/utils/kp_analysis_conf.py
--rw-r--r--   0 lilache    (501) staff       (20)     1816 2023-01-30 15:29:08.000000 debater_python_api-4.3.1/debater_python_api/utils/kp_analysis_utils.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-04-02 14:32:15.566458 debater_python_api-4.3.1/debater_python_api.egg-info/
--rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-04-02 14:32:15.000000 debater_python_api-4.3.1/debater_python_api.egg-info/PKG-INFO
--rw-r--r--   0 lilache    (501) staff       (20)     4062 2023-04-02 14:32:15.000000 debater_python_api-4.3.1/debater_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 lilache    (501) staff       (20)        1 2023-04-02 14:32:15.000000 debater_python_api-4.3.1/debater_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 lilache    (501) staff       (20)       87 2023-04-02 14:32:15.000000 debater_python_api-4.3.1/debater_python_api.egg-info/requires.txt
--rw-r--r--   0 lilache    (501) staff       (20)       19 2023-04-02 14:32:15.000000 debater_python_api-4.3.1/debater_python_api.egg-info/top_level.txt
--rw-r--r--   0 lilache    (501) staff       (20)      879 2023-04-02 14:18:59.000000 debater_python_api-4.3.1/pyproject.toml
--rw-r--r--   0 lilache    (501) staff       (20)       38 2023-04-02 14:32:15.580104 debater_python_api-4.3.1/setup.cfg
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.831185 debater_python_api-4.3.2/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    11358 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/LICENSE
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-04-30 13:43:43.831010 debater_python_api-4.3.2/PKG-INFO
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      169 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/README.md
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.820064 debater_python_api-4.3.2/debater_python_api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.821190 debater_python_api-4.3.2/debater_python_api/api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.824154 debater_python_api-4.3.2/debater_python_api/api/clients/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4503 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/abstract_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1147 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/argument_quality_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1548 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/claim_and_evidence_detection_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      934 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/claim_boundaries_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6203 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/clustering_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3034 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/embedding_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1999 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/index_searcher_client.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.825239 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    28620 2023-04-18 08:38:46.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/KpAnalysisUtils.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      136 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/KpaExceptions.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    17249 2023-04-18 07:19:29.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/KpaResult.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    12256 2023-04-18 07:19:29.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/docx_generator.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     2121 2023-01-23 14:28:56.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/try_things.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1711 2023-01-18 11:06:06.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/utils.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6234 2022-12-27 12:16:15.000000 debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_admin_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    28126 2023-04-30 13:39:08.000000 debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1894 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_pairs_infer_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13830 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/narrative_generation_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1230 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/pro_con_client.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.825508 debater_python_api-4.3.2/debater_python_api/api/clients/response_data/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/response_data/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1597 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/response_data/speech_response.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1790 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/term_relater_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1563 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/term_wikifier_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3394 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/theme_extraction_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3270 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/debater_api.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.825641 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.826556 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      142 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     5079 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1001 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1314 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3576 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1516 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.828623 debater_python_api-4.3.2/debater_python_api/examples/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      803 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/argument_quality_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      854 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/claim_boundaries_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1002 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/claim_detection_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      932 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/clustering_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      860 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/embedding_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1014 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/evidence_detection_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    85859 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/example_of_sc_args.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1480 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/index_searcher_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1173 2023-04-18 07:19:29.000000 debater_python_api-4.3.2/debater_python_api/examples/keypoints_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1428 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/pro_con_example.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.828987 debater_python_api-4.3.2/debater_python_api/examples/resources/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/resources/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    23817 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/resources/arguments.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.829122 debater_python_api-4.3.2/debater_python_api/examples/resources/filters_output/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/resources/filters_output/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     2530 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/resources/pro_con_scores.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     9581 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/run_all_services.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      870 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/speech_construction_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      480 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/term_relater_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      907 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/term_wikifier_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1154 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/theme_extraction_example.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.829476 debater_python_api-4.3.2/debater_python_api/examples/usecases/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4943 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/usecases/kp_based_survey.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6036 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/usecases/mining_to_narrative.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    10191 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/usecases/survey.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.829611 debater_python_api-4.3.2/debater_python_api/integration_tests/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.829718 debater_python_api-4.3.2/debater_python_api/integration_tests/api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.830205 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     2708 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    11539 2023-04-18 07:19:29.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/ServicesIT.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4630 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/ServicesLoad.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.830793 debater_python_api-4.3.2/debater_python_api/utils/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/utils/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      992 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/utils/clusters_refiner.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1574 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/utils/general_utils.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      604 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/utils/kp_analysis_conf.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1816 2023-01-18 09:21:46.000000 debater_python_api-4.3.2/debater_python_api/utils/kp_analysis_utils.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.820855 debater_python_api-4.3.2/debater_python_api.egg-info/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4126 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        1 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       87 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/requires.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       19 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      879 2023-04-30 13:43:21.000000 debater_python_api-4.3.2/pyproject.toml
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       38 2023-04-30 13:43:43.831222 debater_python_api-4.3.2/setup.cfg
```

### Comparing `debater_python_api-4.3.1/LICENSE` & `debater_python_api-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/PKG-INFO` & `debater_python_api-4.3.2/debater_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: debater_python_api
-Version: 4.3.1
+Name: debater-python-api
+Version: 4.3.2
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/abstract_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/abstract_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/argument_quality_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/argument_quality_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/claim_and_evidence_detection_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/claim_and_evidence_detection_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/claim_boundaries_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/claim_boundaries_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/clustering_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/clustering_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/embedding_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/embedding_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/index_searcher_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/index_searcher_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/KpAnalysisUtils.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/KpAnalysisUtils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/KpaResult.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/KpaResult.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/docx_generator.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/docx_generator.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/key_point_analysis/utils.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/keypoints_admin_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_admin_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/keypoints_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 self_check_endpoint = '/self_check'
 
 
 class KpAnalysisClient(AbstractClient):
     '''
     A client for the Key Point Analysis (KPA) service.
     '''
-    def __init__(self, apikey: str, host: Optional[str]=None):
+    def __init__(self, apikey: str, host: Optional[str] = None, verify_certificate: bool = True):
         '''
         :param apikey: user's api-key, should be retreived from the early-access-program site.
         :param host: optional, enable switching to alternative services.
         '''
         AbstractClient.__init__(self, apikey)
         self.host = host if host is not None else 'https://keypoint-matching-backend.debater.res.ibm.com'
+        self.verify_certificate = verify_certificate
 
     def _delete(self, url, params, use_cache=True, timeout=300, retries=10, headers=None):
         return self._run_request_with_retry(requests.delete, url, params, use_cache, timeout, retries, headers)
 
     def _get(self, url, params, use_cache=True, timeout=300, retries=10, headers=None):
         return self._run_request_with_retry(requests.get, url, params, use_cache, timeout, retries, headers)
 
@@ -48,17 +49,17 @@
         logging.info('client calls service (%s): %s' % (func.__name__, url))
         if not use_cache:
             headers['cache-control'] = 'no-cache'
 
         while True:
             try:
                 if func.__name__ == 'post':
-                    resp = func(url, json=params, headers=headers, timeout=timeout)
+                    resp = func(url, json=params, headers=headers, timeout=timeout, verify=self.verify_certificate)
                 else:
-                    resp = func(url, params=params, headers=headers, timeout=timeout)
+                    resp = func(url, params=params, headers=headers, timeout=timeout, verify=self.verify_certificate)
                 if resp.status_code == 200:
                     return resp.json()
                 if resp.status_code == 422:
                     msg = 'There is a problem with the request (%d): %s' % (resp.status_code, resp.reason)
                     logging.error(msg)
                     raise KpaIllegalInputException(msg)
                 msg = 'Failed calling server at %s: (%d) %s' % (url, resp.status_code, resp.reason)
@@ -113,14 +114,15 @@
         :param batch_size: the number of comments that will be uploaded in every REST-API call.
         '''
         assert len(comments_ids) == len(comments_texts), 'comments_texts and comments_ids must be the same length'
         assert len(comments_ids) == len(set(comments_ids)), 'comment_ids must be unique'
         assert self._is_list_of_strings(comments_texts), 'comment_texts must be a list of strings'
         assert self._is_list_of_strings(comments_ids), 'comment_ids must be a list of strings'
         assert len([c for c in comments_texts if c is None or c == '' or len(c) == 0 or c.isspace()]) == 0, 'comment_texts must not have an empty string in it'
+        assert len([c for c in comments_texts if len(c) > 3000]) == 0, 'comment_texts must be shorter than 3000 charachters'
         logging.info('uploading %d comments in batches' % len(comments_ids))
 
         ids_texts = list(zip(comments_ids, comments_texts))
         uploaded = 0
         batches = [ids_texts[i:i + batch_size] for i in range(0, len(ids_texts), batch_size)]
         for batch in batches:
             comments_ids = [t[0] for t in batch]
@@ -153,16 +155,16 @@
         '''
         while True:
             res = self.get_comments_status(domain)
             if res['pending_comments'] == 0:
                 break
             time.sleep(polling_timout_secs if polling_timout_secs is not None else 10)
 
-    def start_kp_analysis_job(self, domain: str, comments_ids: Optional[List[str]]=None,
-                              run_params=None, description: Optional[str]=None, use_cache: bool = True) -> 'KpAnalysisTaskFuture':
+    def start_kp_analysis_job(self, domain: str, comments_ids: Optional[List[str]] = None,
+                              run_params = None, description: Optional[str] = None, use_cache: bool = True) -> 'KpAnalysisTaskFuture':
         '''
         Starts a Key Point Analysis (KPA) job in an async manner. Please make sure all comments had already been uploaded into a domain and processed before starting a new job (using the wait_till_all_comments_are_processed method).
           * By default it runs over all comments in the domain. In order to run only on a subset of the comments in the domain, pass their ids in the comment_ids param.
           * It is also possible to add a job description. This description will later be visible in the user-report.
           * Every domain has a cache. When running a new job, only the delta from previous jobs in the same domain is calculated.
           * Different parameters that affect the job and its result can be passed in the run_params parameter:
               * keypoints (List of strings, empty by default): When keypoints are provided the service matches the sentences to the given keypoints instead of extracting them automatically.
@@ -320,15 +322,15 @@
         Checks the connection to the service and if the service is UP and running.
         :return: a json with 'status': that have the value UP if all is well and DOWN otherwise.
         '''
         return self._get(self.host + self_check_endpoint, None, timeout=180)
 
     def get_sentences_for_domain(self, domain: str, job_id: Optional[str] = None):
         '''
-        Uploaded comments are cleaned and splitted into sentences. This method retrieves the sentences in a domain.
+        Uploaded comments are cleaned and split into sentences. This method retrieves the sentences in a domain.
         :param domain: the name of the domain.
         :param job_id: when provided, it will only return the sentences used in a specific key point analysis job.
         :return: a dictionary with all the sentences' details.
         '''
         res = self._get(self.host + data_endpoint, {'domain': domain, 'get_sentences': True, 'job_id': job_id})
         logging.info(res['msg'])
         return res['sentences_results']
@@ -413,8 +415,8 @@
         if 'total_stages' in progress:
             total_stages = progress['total_stages']
             for i in reversed(range(total_stages)):
                 stage = str(i + 1)
                 stage_i = 'stage_' + stage
                 if stage_i in progress and 'inferred_batches' in progress[stage_i] and 'total_batches' in progress[stage_i]:
                     print_progress_bar(progress[stage_i]['inferred_batches'], progress[stage_i]['total_batches'], prefix='Stage %s/%s:' % (stage, str(total_stages)), suffix='Complete', length=50)
-                    break
+                    break
```

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/keypoints_pairs_infer_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_pairs_infer_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/narrative_generation_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/narrative_generation_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/pro_con_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/pro_con_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/response_data/speech_response.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/response_data/speech_response.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/term_relater_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/term_relater_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/term_wikifier_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/term_wikifier_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/clients/theme_extraction_client.py` & `debater_python_api-4.3.2/debater_python_api/api/clients/theme_extraction_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/debater_api.py` & `debater_python_api-4.3.2/debater_python_api/api/debater_api.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/elastic_client.py` & `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py` & `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py` & `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/sentence_query_base.py` & `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/sentence_query_base.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/api/sentence_level_index/client/sentence_query_request.py` & `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/sentence_query_request.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/argument_quality_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/argument_quality_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/claim_boundaries_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/claim_boundaries_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/claim_detection_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/claim_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/clustering_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/clustering_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/embedding_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/embedding_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/evidence_detection_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/evidence_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/example_of_sc_args.py` & `debater_python_api-4.3.2/debater_python_api/examples/example_of_sc_args.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/index_searcher_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/index_searcher_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/keypoints_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/keypoints_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/pro_con_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/pro_con_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/resources/arguments.py` & `debater_python_api-4.3.2/debater_python_api/examples/resources/arguments.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/resources/pro_con_scores.py` & `debater_python_api-4.3.2/debater_python_api/examples/resources/pro_con_scores.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/run_all_services.py` & `debater_python_api-4.3.2/debater_python_api/examples/run_all_services.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/speech_construction_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/speech_construction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/term_wikifier_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/term_wikifier_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/theme_extraction_example.py` & `debater_python_api-4.3.2/debater_python_api/examples/theme_extraction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/usecases/kp_based_survey.py` & `debater_python_api-4.3.2/debater_python_api/examples/usecases/kp_based_survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/usecases/mining_to_narrative.py` & `debater_python_api-4.3.2/debater_python_api/examples/usecases/mining_to_narrative.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/examples/usecases/survey.py` & `debater_python_api-4.3.2/debater_python_api/examples/usecases/survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py` & `debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/integration_tests/api/clients/ServicesIT.py` & `debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/ServicesIT.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/integration_tests/api/clients/ServicesLoad.py` & `debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/ServicesLoad.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/utils/clusters_refiner.py` & `debater_python_api-4.3.2/debater_python_api/utils/clusters_refiner.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/utils/general_utils.py` & `debater_python_api-4.3.2/debater_python_api/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/utils/kp_analysis_conf.py` & `debater_python_api-4.3.2/debater_python_api/utils/kp_analysis_conf.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api/utils/kp_analysis_utils.py` & `debater_python_api-4.3.2/debater_python_api/utils/kp_analysis_utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.1/debater_python_api.egg-info/PKG-INFO` & `debater_python_api-4.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: debater-python-api
-Version: 4.3.1
+Name: debater_python_api
+Version: 4.3.2
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-4.3.1/debater_python_api.egg-info/SOURCES.txt` & `debater_python_api-4.3.2/debater_python_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 debater_python_api/api/clients/term_relater_client.py
 debater_python_api/api/clients/term_wikifier_client.py
 debater_python_api/api/clients/theme_extraction_client.py
 debater_python_api/api/clients/key_point_analysis/KpAnalysisUtils.py
 debater_python_api/api/clients/key_point_analysis/KpaExceptions.py
 debater_python_api/api/clients/key_point_analysis/KpaResult.py
 debater_python_api/api/clients/key_point_analysis/docx_generator.py
+debater_python_api/api/clients/key_point_analysis/try_things.py
 debater_python_api/api/clients/key_point_analysis/utils.py
 debater_python_api/api/clients/response_data/__init__.py
 debater_python_api/api/clients/response_data/speech_response.py
 debater_python_api/api/sentence_level_index/__init__.py
 debater_python_api/api/sentence_level_index/client/__init__.py
 debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
 debater_python_api/api/sentence_level_index/client/elastic_client.py
```

### Comparing `debater_python_api-4.3.1/pyproject.toml` & `debater_python_api-4.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debater_python_api"
-version = "4.3.1"
+version = "4.3.2"
 description = "Project Debater Early Access Program API sdk for python"
 readme = "README.md"
 authors = [{ name = "Elad Venezian", email = "eladv@il.ibm.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

