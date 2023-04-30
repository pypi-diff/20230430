# Comparing `tmp/patent_client-3.2.3.tar.gz` & `tmp/patent_client-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-3.2.3.tar", max compression
+gzip compressed data, was "patent_client-3.2.4.tar", max compression
```

## Comparing `patent_client-3.2.3.tar` & `patent_client-3.2.4.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0      593 2023-04-30 00:17:13.630604 patent_client-3.2.3/LICENSE
--rw-r--r--   0        0        0     4414 2023-04-30 00:17:13.630604 patent_client-3.2.3/README.md
--rw-r--r--   0        0        0     3485 2023-04-30 00:17:13.670605 patent_client-3.2.3/pyproject.toml
--rw-r--r--   0        0        0     2590 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/__init__.py
--rw-r--r--   0        0        0      215 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/default_settings.yml
--rw-r--r--   0        0        0        0 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/epo/__init__.py
--rw-r--r--   0        0        0      271 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      350 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/api.py
--rw-r--r--   0        0        0      406 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     8854 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/examples/example.xml
--rw-r--r--   0        0        0     7248 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/expected/example.json
--rw-r--r--   0        0        0     8853 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/expected/example.xml
--rw-r--r--   0        0        0      304 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1180 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/model.py
--rw-r--r--   0        0        0     1603 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/schema.py
--rw-r--r--   0        0        0      594 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0       77 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      355 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/api.py
--rw-r--r--   0        0        0      380 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0   285423 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx
--rw-r--r--   0        0        0      323 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2117 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/model.py
--rw-r--r--   0        0        0     4163 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      283 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4041 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/schema.py
--rw-r--r--   0        0        0      904 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0    76105 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/example.xml
--rw-r--r--   0        0        0    44095 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/example.json
--rw-r--r--   0        0        0    76104 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/example.xml
--rw-r--r--   0        0        0    11924 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/us_example.json
--rw-r--r--   0        0        0    22970 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/us_example.xml
--rw-r--r--   0        0        0      114 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1269 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1102 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      600 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      972 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5024 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/api.py
--rw-r--r--   0        0        0     1884 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/cql.py
--rw-r--r--   0        0        0     3127 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2043 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      399 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2633 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1095 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     1610 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      776 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      306 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3943 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      891 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1652 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      668 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3099 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     3973 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0     5916 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     9015 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34663 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     2318 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/session.py
--rw-r--r--   0        0        0     1613 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/util.py
--rw-r--r--   0        0        0     5991 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/parser.py
--rw-r--r--   0        0        0     1129 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/session.py
--rw-r--r--   0        0        0     1300 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/test_parser.py
--rw-r--r--   0        0        0      278 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/uspto/__init__.py
--rw-r--r--   0        0        0      105 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     3822 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4269 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     3404 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/model.py
--rw-r--r--   0        0        0     3473 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/schema.py
--rw-r--r--   0        0        0     2234 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/schema_test.py
--rw-r--r--   0        0        0    13274 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_1.xml
--rw-r--r--   0        0        0    11638 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_2.xml
--rw-r--r--   0        0        0   277704 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_3.xml
--rw-r--r--   0        0        0       76 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     1161 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     2983 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1979 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     5405 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3705 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     5062 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5146 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     2094 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/schema.py
--rw-r--r--   0        0        0      983 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/schema_test.py
--rw-r--r--   0        0        0      271 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/session.py
--rw-r--r--   0        0        0     4134 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      117 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/peds/__init__.py
--rw-r--r--   0        0        0     7525 2023-04-30 00:17:13.722605 patent_client-3.2.3/src/patent_client/uspto/peds/manager.py
--rw-r--r--   0        0        0     9017 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    19234 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/model.py
--rw-r--r--   0        0        0     8250 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/schema.py
--rw-r--r--   0        0        0      529 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/schema_test.py
--rw-r--r--   0        0        0    94546 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/test/app_12721698.json
--rw-r--r--   0        0        0    15274 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/test/expected.json
--rw-r--r--   0        0        0      331 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/__init__.py
--rw-r--r--   0        0        0     5774 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/developer.uspto.gov.crt
--rw-r--r--   0        0        0     3207 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2135 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     7387 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/model.py
--rw-r--r--   0        0        0    69917 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/ptabApiV2.json
--rw-r--r--   0        0        0     3597 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/schema.py
--rw-r--r--   0        0        0      282 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/session.py
--rw-r--r--   0        0        0      159 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/util.py
--rw-r--r--   0        0        0       72 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     4943 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/public_search/api.py
--rw-r--r--   0        0        0     3891 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/manager.py
--rw-r--r--   0        0        0    12219 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/model.py
--rw-r--r--   0        0        0     7277 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4331 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     3689 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/query_test.py
--rw-r--r--   0        0        0    10290 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/schema.py
--rw-r--r--   0        0        0     1254 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/schema_test.py
--rw-r--r--   0        0        0   387227 2023-04-30 00:17:13.822605 patent_client-3.2.3/src/patent_client/uspto/public_search/test/biblio.json
--rw-r--r--   0        0        0   213101 2023-04-30 00:17:13.822605 patent_client-3.2.3/src/patent_client/uspto/public_search/test/biblio_expected.json
--rw-r--r--   0        0        0  2431829 2023-04-30 00:17:13.826605 patent_client-3.2.3/src/patent_client/uspto/public_search/test/docs.json
--rw-r--r--   0        0        0  1880230 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/uspto/public_search/test/docs_expected.json
--rw-r--r--   0        0        0      565 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/__init__.py
--rw-r--r--   0        0        0     5030 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/manager.py
--rw-r--r--   0        0        0     1696 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/model.py
--rw-r--r--   0        0        0      775 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/model_test.py
--rw-r--r--   0        0        0     3148 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/related.py
--rw-r--r--   0        0        0        0 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/test_manager.py
--rw-r--r--   0        0        0     1913 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/util.py
--rw-r--r--   0        0        0        0 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4263 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6204 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      834 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3565 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      931 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      204 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/__init__.py
--rw-r--r--   0        0        0     5774 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/date_parse.py
--rw-r--r--   0        0        0     9054 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/date_parse_test.py
--rw-r--r--   0        0        0    15027 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/functional.py
--rw-r--r--   0        0        0    12808 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/regex_helper.py
--rw-r--r--   0        0        0      611 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/format.py
--rw-r--r--   0        0        0     2699 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/version.py
--rw-r--r--   0        0        0     6965 1970-01-01 00:00:00.000000 patent_client-3.2.3/PKG-INFO
+-rw-r--r--   0        0        0      593 2023-04-30 00:25:43.167737 patent_client-3.2.4/LICENSE
+-rw-r--r--   0        0        0     4414 2023-04-30 00:25:43.167737 patent_client-3.2.4/README.md
+-rw-r--r--   0        0        0     3485 2023-04-30 00:25:43.207737 patent_client-3.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2590 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/default_settings.yml
+-rw-r--r--   0        0        0        0 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      350 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/api.py
+-rw-r--r--   0        0        0      406 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     8854 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/examples/example.xml
+-rw-r--r--   0        0        0     7248 2023-04-30 00:25:43.207737 patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/expected/example.json
+-rw-r--r--   0        0        0     8853 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/expected/example.xml
+-rw-r--r--   0        0        0      304 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1180 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/model.py
+-rw-r--r--   0        0        0     1603 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      594 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0       77 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      355 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      380 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0   285423 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx
+-rw-r--r--   0        0        0      323 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2117 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     4163 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      283 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4041 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0      904 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0    76105 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/example.xml
+-rw-r--r--   0        0        0    44095 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.json
+-rw-r--r--   0        0        0    76104 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.xml
+-rw-r--r--   0        0        0    11924 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/us_example.json
+-rw-r--r--   0        0        0    22970 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/test/us_example.xml
+-rw-r--r--   0        0        0      114 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1239 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1269 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1102 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2023-04-30 00:25:43.211737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      600 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      972 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5024 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/api.py
+-rw-r--r--   0        0        0     1884 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     3127 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2043 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      399 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2633 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1095 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     1610 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      776 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      306 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3943 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      891 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1652 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      668 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3099 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2023-04-30 00:25:43.215737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     3973 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0     5916 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     9015 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34663 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     2318 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/session.py
+-rw-r--r--   0        0        0     1613 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/epo/ops/util.py
+-rw-r--r--   0        0        0     5991 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/parser.py
+-rw-r--r--   0        0        0     1129 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/session.py
+-rw-r--r--   0        0        0     1300 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/test_parser.py
+-rw-r--r--   0        0        0      278 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/uspto/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-30 00:25:43.219737 patent_client-3.2.4/src/patent_client/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     3822 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4269 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     3404 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/model.py
+-rw-r--r--   0        0        0     3473 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/schema.py
+-rw-r--r--   0        0        0     2234 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/schema_test.py
+-rw-r--r--   0        0        0    13274 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_1.xml
+-rw-r--r--   0        0        0    11638 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_2.xml
+-rw-r--r--   0        0        0   277704 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_3.xml
+-rw-r--r--   0        0        0       76 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     1161 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     2983 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1979 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     5405 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3705 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     5062 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5146 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     2094 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/schema.py
+-rw-r--r--   0        0        0      983 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/schema_test.py
+-rw-r--r--   0        0        0      271 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/session.py
+-rw-r--r--   0        0        0     4134 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      117 2023-04-30 00:25:43.231737 patent_client-3.2.4/src/patent_client/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     7525 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9017 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    19255 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/model.py
+-rw-r--r--   0        0        0     8585 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/schema.py
+-rw-r--r--   0        0        0      529 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/schema_test.py
+-rw-r--r--   0        0        0    94546 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/test/app_12721698.json
+-rw-r--r--   0        0        0    15274 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/peds/test/expected.json
+-rw-r--r--   0        0        0      331 2023-04-30 00:25:43.255737 patent_client-3.2.4/src/patent_client/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0     5774 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/developer.uspto.gov.crt
+-rw-r--r--   0        0        0     3207 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2135 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     7387 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/model.py
+-rw-r--r--   0        0        0    69917 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/ptabApiV2.json
+-rw-r--r--   0        0        0     3597 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/schema.py
+-rw-r--r--   0        0        0      282 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/session.py
+-rw-r--r--   0        0        0      159 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/ptab/util.py
+-rw-r--r--   0        0        0       72 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     4943 2023-04-30 00:25:43.259737 patent_client-3.2.4/src/patent_client/uspto/public_search/api.py
+-rw-r--r--   0        0        0     3891 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/manager.py
+-rw-r--r--   0        0        0    12219 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/model.py
+-rw-r--r--   0        0        0     7277 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4331 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     3689 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0    10290 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/schema.py
+-rw-r--r--   0        0        0     1254 2023-04-30 00:25:43.331738 patent_client-3.2.4/src/patent_client/uspto/public_search/schema_test.py
+-rw-r--r--   0        0        0   387227 2023-04-30 00:25:43.339738 patent_client-3.2.4/src/patent_client/uspto/public_search/test/biblio.json
+-rw-r--r--   0        0        0   213101 2023-04-30 00:25:43.339738 patent_client-3.2.4/src/patent_client/uspto/public_search/test/biblio_expected.json
+-rw-r--r--   0        0        0  2431829 2023-04-30 00:25:43.343738 patent_client-3.2.4/src/patent_client/uspto/public_search/test/docs.json
+-rw-r--r--   0        0        0  1880230 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/uspto/public_search/test/docs_expected.json
+-rw-r--r--   0        0        0      565 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/__init__.py
+-rw-r--r--   0        0        0     5030 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/manager.py
+-rw-r--r--   0        0        0     1696 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/model.py
+-rw-r--r--   0        0        0      775 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/model_test.py
+-rw-r--r--   0        0        0     3148 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/related.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/test_manager.py
+-rw-r--r--   0        0        0     1913 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/base/util.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4263 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6204 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      834 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3565 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      931 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      204 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/__init__.py
+-rw-r--r--   0        0        0     5774 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/date_parse.py
+-rw-r--r--   0        0        0     9054 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/date_parse_test.py
+-rw-r--r--   0        0        0    15027 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/functional.py
+-rw-r--r--   0        0        0    12808 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/datetime/regex_helper.py
+-rw-r--r--   0        0        0      611 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/format.py
+-rw-r--r--   0        0        0     2699 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2023-04-30 00:25:43.347738 patent_client-3.2.4/src/patent_client/version.py
+-rw-r--r--   0        0        0     6965 1970-01-01 00:00:00.000000 patent_client-3.2.4/PKG-INFO
```

### Comparing `patent_client-3.2.3/LICENSE` & `patent_client-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/README.md` & `patent_client-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/pyproject.toml` & `patent_client-3.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent_client"
-version = "3.2.3"
+version = "3.2.4"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
```

### Comparing `patent_client-3.2.3/src/patent_client/__init__.py` & `patent_client-3.2.4/src/patent_client/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/examples/example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/examples/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/expected/example.json` & `patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/expected/example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/expected/example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/family/fixtures/expected/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/family/model.py` & `patent_client-3.2.4/src/patent_client/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/family/schema.py` & `patent_client-3.2.4/src/patent_client/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/family/schema_test.py` & `patent_client-3.2.4/src/patent_client/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/model.py` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/national_codes.py` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/national_codes.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/schema.py` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/schema_test.py` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/example.json` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/us_example.json` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/expected/us_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/us_example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/legal/test/us_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/number_service/api.py` & `patent_client-3.2.4/src/patent_client/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/number_service/api_test.py` & `patent_client-3.2.4/src/patent_client/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/number_service/errors.py` & `patent_client-3.2.4/src/patent_client/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/number_service/errors.txt` & `patent_client-3.2.4/src/patent_client/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/number_service/messages.txt` & `patent_client-3.2.4/src/patent_client/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/number_service/model.py` & `patent_client-3.2.4/src/patent_client/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/number_service/schema.py` & `patent_client-3.2.4/src/patent_client/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/api.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/api_test.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/cql.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/manager.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/manager_test.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/model/biblio.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/model/fulltext.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/model/images.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/model/search.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/schema/biblio.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/schema/fulltext.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/schema/images.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/schema/search.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/schema_test.py` & `patent_client-3.2.4/src/patent_client/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_2.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_3.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_4.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/claims_example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/claims_example_2.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/description_example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/claims_example.json` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/image_example.json` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/search_result.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/full_cycle_example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/image_example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/published/test/search_example.xml` & `patent_client-3.2.4/src/patent_client/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/session.py` & `patent_client-3.2.4/src/patent_client/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/epo/ops/util.py` & `patent_client-3.2.4/src/patent_client/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/parser.py` & `patent_client-3.2.4/src/patent_client/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/session.py` & `patent_client-3.2.4/src/patent_client/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/settings.py` & `patent_client-3.2.4/src/patent_client/settings.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/test_parser.py` & `patent_client-3.2.4/src/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/assignment/manager.py` & `patent_client-3.2.4/src/patent_client/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/assignment/manager_test.py` & `patent_client-3.2.4/src/patent_client/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/assignment/model.py` & `patent_client-3.2.4/src/patent_client/uspto/assignment/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/assignment/schema.py` & `patent_client-3.2.4/src/patent_client/uspto/assignment/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/assignment/schema_test.py` & `patent_client-3.2.4/src/patent_client/uspto/assignment/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_1.xml` & `patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_2.xml` & `patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_3.xml` & `patent_client-3.2.4/src/patent_client/uspto/assignment/test/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/api.py` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/gd_input.csv` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/manager.py` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/model.py` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/model_test.py` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/query.py` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/query_test.py` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/schema.py` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/schema_test.py` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/app.json` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/app_expected.json` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/doc_list.json` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-3.2.4/src/patent_client/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/peds/manager.py` & `patent_client-3.2.4/src/patent_client/uspto/peds/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/peds/manager_test.py` & `patent_client-3.2.4/src/patent_client/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/peds/model.py` & `patent_client-3.2.4/src/patent_client/uspto/peds/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,19 +343,19 @@
 
     def __hash__(self):
         return hash((self.parent_appl_id, self.child_appl_id, self.relationship))
 
 
 @dataclass
 class ForeignPriority(Model):
-    priority_claim: str
+    priority_claim: str = None
     """The application number of the foreign priority application"""
-    country_name: str
+    country_name: str = None
     """The country in which the foreign priorty application was filed"""
-    filing_date: datetime.date
+    filing_date: datetime.date = None
     """The filing date of the foreign priority application"""
 
 
 @dataclass
 class PtaPteHistory(Model):
     number: float
     date: datetime.date
```

### Comparing `patent_client-3.2.3/src/patent_client/uspto/peds/schema.py` & `patent_client-3.2.4/src/patent_client/uspto/peds/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+import datetime
 from collections import defaultdict
 from typing import *
 
+from dateutil.parser import ParserError
 from patent_client.util.format import clean_whitespace
 from yankee.json.schema import fields as f
 from yankee.json.schema import Schema
 
 
+class UsptoDate(f.Date):
+    def deserialize(self, elem) -> "Optional[datetime.date]":
+        try:
+            return super().deserialize(elem)
+        except ParserError:
+            return datetime.datetime(1900, 1, 1).date()
+
+
 class InventorNameField(f.Combine):
     name_line_one = f.Str()
     name_line_two = f.Str()
     suffix = f.Str()
 
     def combine_func(self, obj):
         return clean_whitespace(
@@ -43,36 +53,36 @@
 
 
 class ApplicantSchema(PersonSchema):
     cust_no = f.Str()
 
 
 class TransactionSchema(Schema):
-    date = f.Date("recordDate")
+    date = UsptoDate("recordDate")
     code = f.Str()
     description = f.Str()
 
 
 class ChildSchema(Schema):
     __model_name__ = "Relationship"
     parent_appl_id = f.Str("applicationNumberText")
-    child_app_filing_date = f.Date("filingDate")
+    child_app_filing_date = UsptoDate("filingDate")
     child_app_status = f.Str("applicationStatus")
     child_appl_id = f.Str("claimApplicationNumberText")
     relationship = f.Str(
         "applicationStatusDescription",
         formatter=lambda x: x.replace("This application ", ""),
     )
 
 
 class ParentSchema(Schema):
     __model_name__ = "Relationship"
     parent_appl_id = f.Str("claimApplicationNumberText")
     child_appl_id = f.Str("applicationNumberText")
-    parent_app_filing_date = f.Date("filingDate")
+    parent_app_filing_date = UsptoDate("filingDate")
     parent_app_status = f.Str("applicationStatus")
     relationship = f.Str(
         "applicationStatusDescription",
         formatter=lambda x: x.replace("This application ", ""),
     )
 
 
@@ -81,15 +91,15 @@
         try:
             return super().deserialize(elem)
         except ValueError:
             return None
 
 
 class PtaPteHistorySchema(Schema):
-    date = f.Date("ptaOrPteDate")
+    date = UsptoDate("ptaOrPteDate")
     description = f.String("contentsDescription")
     number = f.Float()
     pto_days = OptionalFloat()
     applicant_days = OptionalFloat()
     start = f.Float()
 
 
@@ -142,25 +152,25 @@
     phone_num = f.Str()
     reg_status = f.Str()
 
 
 class ForeignPrioritySchema(Schema):
     priority_claim = f.Str()
     country_name = f.Str()
-    filing_date = f.Date(dt_format="%m-%d-%Y")
+    filing_date = UsptoDate(dt_format="%m-%d-%Y")
 
 
 class DocumentSchema(Schema):
     access_level_category = f.Str()
     appl_id = f.Str("applicationNumberText")
     category = f.Str("documentCategory")
     code = f.Str(data_key="documentCode")
     description = f.Str("documentDescription")
     identifier = f.Str("documentIdentifier")
-    mail_room_date = f.Date()
+    mail_room_date = UsptoDate()
     page_count = f.Int()
     url = f.Str(data_key="pdf_url")
 
 
 class ReelFrameField(f.Combine):
     reel_number = f.Str()
     frame_number = f.Str()
@@ -180,15 +190,15 @@
             f"{obj.get('line_1', '')}\n{obj.get('line_2', '')}\n{obj.get('line_3', '')}\n{obj.get('line_4', '')}".strip(),
             preserve_newlines=True,
         )
 
 
 class AssignorSchema(Schema):
     name = f.Str("assignorName")
-    exec_date = f.Date()
+    exec_date = UsptoDate()
 
 
 class AssigneeAddressField(f.Combine):
     line_1 = f.Str("streetLineOneText", null_value="null")
     line_2 = f.Str("streetLineTwoText", null_value="null")
     city = f.Str("cityName")
     country = f.Str("countryCode")
@@ -206,50 +216,50 @@
     address = AssigneeAddressField(data_key=False)
 
 
 class AssignmentSchema(Schema):
     id = ReelFrameField(data_key=False)
     correspondent = f.Str("addressNameText")
     correspondent_address = AddressField(data_key=False)
-    mail_date = f.Date(null_value="NONE")
-    received_date = f.Date(null_value="NONE")
-    recorded_date = f.Date(null_value="NONE")
+    mail_date = UsptoDate(null_value="NONE")
+    received_date = UsptoDate(null_value="NONE")
+    recorded_date = UsptoDate(null_value="NONE")
     pages = f.Int("pagesCount")
     conveyance_text = f.Str(
         "converyanceName",
         formatter=lambda x: x.replace(" (SEE DOCUMENT FOR DETAILS).", ""),
     )
     sequence_number = f.Int()
     assignors = f.List(AssignorSchema, "assignors")
     assignees = f.List(AssigneeSchema, "assignee")
 
 
 class USApplicationSchema(Schema):
     # Basic Bibliographic Data
     appl_id = f.Str()
     app_confr_number = f.Str()
-    app_filing_date = f.Date()
+    app_filing_date = UsptoDate()
     app_location = f.Str()
     app_type = f.Str()
     app_entity_status = f.Str()
     app_cls_sub_cls = f.Str()
     app_grp_art_number = f.Str()
     app_exam_name = f.Str()
     first_inventor_file = f.Bool(true_value="Yes")
     patent_title = f.Str()
     # Status Information
     app_status = f.Str()
-    app_status_date = f.Date()
+    app_status_date = UsptoDate()
     # Publication Information
     app_early_pub_number = f.Str()
-    app_early_pub_date = f.Date()
+    app_early_pub_date = UsptoDate()
     patent_number = f.Str()
-    patent_issue_date = f.Date()
+    patent_issue_date = UsptoDate()
     wipo_early_pub_number = f.Str()
-    wipo_early_pub_date = f.Date()
+    wipo_early_pub_date = UsptoDate()
     # Correspondent / Attorney Information
     corr_addr_cust_no = f.Str()
     app_cust_number = f.Str()
     app_attr_dock_number = f.Str()
 
     # Assignments
     assignments = f.List(AssignmentSchema)
@@ -264,10 +274,10 @@
     pta_pte_summary = PtaPteSummarySchema(data_key=False)
     correspondent = CorrespondentSchema(data_key=False)
     attorneys = f.List(AttorneySchema, data_key="attrnyAddr")
     foreign_priority = f.List(ForeignPrioritySchema)
 
 
 class PedsPageSchema(Schema):
-    index_last_updated = f.Date("queryResults.indexLastUpdatedDate")
+    index_last_updated = UsptoDate("queryResults.indexLastUpdatedDate")
     num_found = f.Int("queryResults.searchResponse.response.numFound")
     applications = f.List(USApplicationSchema, "queryResults.searchResponse.response.docs")
```

### Comparing `patent_client-3.2.3/src/patent_client/uspto/peds/schema_test.py` & `patent_client-3.2.4/src/patent_client/uspto/peds/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/peds/test/app_12721698.json` & `patent_client-3.2.4/src/patent_client/uspto/peds/test/app_12721698.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/peds/test/expected.json` & `patent_client-3.2.4/src/patent_client/uspto/peds/test/expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/ptab/developer.uspto.gov.crt` & `patent_client-3.2.4/src/patent_client/uspto/ptab/developer.uspto.gov.crt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/ptab/manager.py` & `patent_client-3.2.4/src/patent_client/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/ptab/manager_test.py` & `patent_client-3.2.4/src/patent_client/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/ptab/model.py` & `patent_client-3.2.4/src/patent_client/uspto/ptab/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/ptab/ptabApiV2.json` & `patent_client-3.2.4/src/patent_client/uspto/ptab/ptabApiV2.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/ptab/schema.py` & `patent_client-3.2.4/src/patent_client/uspto/ptab/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/api.py` & `patent_client-3.2.4/src/patent_client/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/manager.py` & `patent_client-3.2.4/src/patent_client/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/model.py` & `patent_client-3.2.4/src/patent_client/uspto/public_search/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/model_test.py` & `patent_client-3.2.4/src/patent_client/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/query.py` & `patent_client-3.2.4/src/patent_client/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/query_config.csv` & `patent_client-3.2.4/src/patent_client/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/query_test.py` & `patent_client-3.2.4/src/patent_client/uspto/public_search/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/schema.py` & `patent_client-3.2.4/src/patent_client/uspto/public_search/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/schema_test.py` & `patent_client-3.2.4/src/patent_client/uspto/public_search/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/test/biblio.json` & `patent_client-3.2.4/src/patent_client/uspto/public_search/test/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/test/biblio_expected.json` & `patent_client-3.2.4/src/patent_client/uspto/public_search/test/biblio_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/test/docs.json` & `patent_client-3.2.4/src/patent_client/uspto/public_search/test/docs.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/uspto/public_search/test/docs_expected.json` & `patent_client-3.2.4/src/patent_client/uspto/public_search/test/docs_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/__init__.py` & `patent_client-3.2.4/src/patent_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/base/manager.py` & `patent_client-3.2.4/src/patent_client/util/base/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/base/model.py` & `patent_client-3.2.4/src/patent_client/util/base/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/base/model_test.py` & `patent_client-3.2.4/src/patent_client/util/base/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/base/related.py` & `patent_client-3.2.4/src/patent_client/util/base/related.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/base/util.py` & `patent_client-3.2.4/src/patent_client/util/base/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-3.2.4/src/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-3.2.4/src/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/claims/examples/published_claims.json` & `patent_client-3.2.4/src/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/claims/examples/published_claims.txt` & `patent_client-3.2.4/src/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/claims/model.py` & `patent_client-3.2.4/src/patent_client/util/claims/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/claims/parser.py` & `patent_client-3.2.4/src/patent_client/util/claims/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/claims/parser_test.py` & `patent_client-3.2.4/src/patent_client/util/claims/parser_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/datetime/date_parse.py` & `patent_client-3.2.4/src/patent_client/util/datetime/date_parse.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/datetime/date_parse_test.py` & `patent_client-3.2.4/src/patent_client/util/datetime/date_parse_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/datetime/functional.py` & `patent_client-3.2.4/src/patent_client/util/datetime/functional.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/datetime/regex_helper.py` & `patent_client-3.2.4/src/patent_client/util/datetime/regex_helper.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/format.py` & `patent_client-3.2.4/src/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/src/patent_client/util/test.py` & `patent_client-3.2.4/src/patent_client/util/test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.3/PKG-INFO` & `patent_client-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patent-client
-Version: 3.2.3
+Version: 3.2.4
 Summary: A set of ORM-style clients for publicly available intellectual property data
 Home-page: https://github.com/parkerhancock/patent_client
 License: Apache Software License 2.0
 Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
```

