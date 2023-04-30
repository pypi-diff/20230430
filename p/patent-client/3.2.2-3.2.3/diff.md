# Comparing `tmp/patent_client-3.2.2.tar.gz` & `tmp/patent_client-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-3.2.2.tar", max compression
+gzip compressed data, was "patent_client-3.2.3.tar", max compression
```

## Comparing `patent_client-3.2.2.tar` & `patent_client-3.2.3.tar`

### file list

```diff
@@ -1,166 +1,165 @@
--rw-r--r--   0        0        0      593 2023-01-20 21:05:24.412394 patent_client-3.2.2/LICENSE
--rw-r--r--   0        0        0     4739 2023-01-20 21:05:24.412394 patent_client-3.2.2/README.md
--rw-r--r--   0        0        0     3485 2023-01-20 21:05:24.456394 patent_client-3.2.2/pyproject.toml
--rw-r--r--   0        0        0     2590 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/__init__.py
--rw-r--r--   0        0        0      215 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/default_settings.yml
--rw-r--r--   0        0        0        0 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/__init__.py
--rw-r--r--   0        0        0      271 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      350 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/api.py
--rw-r--r--   0        0        0      406 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     8854 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/fixtures/examples/example.xml
--rw-r--r--   0        0        0     7248 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/fixtures/expected/example.json
--rw-r--r--   0        0        0     8853 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/fixtures/expected/example.xml
--rw-r--r--   0        0        0      304 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1180 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/model.py
--rw-r--r--   0        0        0     1603 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/schema.py
--rw-r--r--   0        0        0      594 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0       77 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      355 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/api.py
--rw-r--r--   0        0        0      380 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0   285423 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx
--rw-r--r--   0        0        0      323 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2117 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/model.py
--rw-r--r--   0        0        0     4045 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      283 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4041 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/schema.py
--rw-r--r--   0        0        0      904 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0    76105 2023-01-20 21:05:24.456394 patent_client-3.2.2/src/patent_client/epo/ops/legal/test/example.xml
--rw-r--r--   0        0        0    44095 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/legal/test/expected/example.json
--rw-r--r--   0        0        0    76104 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/legal/test/expected/example.xml
--rw-r--r--   0        0        0    11924 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/legal/test/expected/us_example.json
--rw-r--r--   0        0        0    22970 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/legal/test/us_example.xml
--rw-r--r--   0        0        0      114 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1239 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1269 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1102 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      600 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      972 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5024 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/published/api.py
--rw-r--r--   0        0        0     1794 2023-01-20 21:05:24.460394 patent_client-3.2.2/src/patent_client/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/cql.py
--rw-r--r--   0        0        0     3127 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2043 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      399 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2633 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1095 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     1610 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      776 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      306 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3943 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      891 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1652 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      668 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3099 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     3973 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0     5916 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     9015 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34663 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     2318 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/session.py
--rw-r--r--   0        0        0     1613 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/epo/ops/util.py
--rw-r--r--   0        0        0     5991 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/parser.py
--rw-r--r--   0        0        0     1129 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/session.py
--rw-r--r--   0        0        0     1300 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/test_parser.py
--rw-r--r--   0        0        0      278 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/uspto/__init__.py
--rw-r--r--   0        0        0      105 2023-01-20 21:05:24.464394 patent_client-3.2.2/src/patent_client/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     3822 2023-01-20 21:05:24.476394 patent_client-3.2.2/src/patent_client/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4269 2023-01-20 21:05:24.476394 patent_client-3.2.2/src/patent_client/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     3404 2023-01-20 21:05:24.476394 patent_client-3.2.2/src/patent_client/uspto/assignment/model.py
--rw-r--r--   0        0        0     3473 2023-01-20 21:05:24.476394 patent_client-3.2.2/src/patent_client/uspto/assignment/schema.py
--rw-r--r--   0        0        0     2234 2023-01-20 21:05:24.476394 patent_client-3.2.2/src/patent_client/uspto/assignment/schema_test.py
--rw-r--r--   0        0        0    13274 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/assignment/test/assignment_1.xml
--rw-r--r--   0        0        0    11638 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/assignment/test/assignment_2.xml
--rw-r--r--   0        0        0   277704 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/assignment/test/assignment_3.xml
--rw-r--r--   0        0        0       76 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     1161 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     2983 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1979 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     5333 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3383 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     5062 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5146 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     2093 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/schema.py
--rw-r--r--   0        0        0      983 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/schema_test.py
--rw-r--r--   0        0        0      271 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/session.py
--rw-r--r--   0        0        0     4134 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2023-01-20 21:05:24.480394 patent_client-3.2.2/src/patent_client/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      117 2023-01-20 21:05:24.484394 patent_client-3.2.2/src/patent_client/uspto/peds/__init__.py
--rw-r--r--   0        0        0     7525 2023-01-20 21:05:24.508394 patent_client-3.2.2/src/patent_client/uspto/peds/manager.py
--rw-r--r--   0        0        0     9017 2023-01-20 21:05:24.508394 patent_client-3.2.2/src/patent_client/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    19234 2023-01-20 21:05:24.508394 patent_client-3.2.2/src/patent_client/uspto/peds/model.py
--rw-r--r--   0        0        0     8250 2023-01-20 21:05:24.508394 patent_client-3.2.2/src/patent_client/uspto/peds/schema.py
--rw-r--r--   0        0        0      529 2023-01-20 21:05:24.508394 patent_client-3.2.2/src/patent_client/uspto/peds/schema_test.py
--rw-r--r--   0        0        0    94546 2023-01-20 21:05:24.508394 patent_client-3.2.2/src/patent_client/uspto/peds/test/app_12721698.json
--rw-r--r--   0        0        0    15274 2023-01-20 21:05:24.508394 patent_client-3.2.2/src/patent_client/uspto/peds/test/expected.json
--rw-r--r--   0        0        0      331 2023-01-20 21:05:24.508394 patent_client-3.2.2/src/patent_client/uspto/ptab/__init__.py
--rw-r--r--   0        0        0     5774 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/ptab/developer.uspto.gov.crt
--rw-r--r--   0        0        0     3207 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2135 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     7387 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/ptab/model.py
--rw-r--r--   0        0        0    69917 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/ptab/ptabApiV2.json
--rw-r--r--   0        0        0     3597 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/ptab/schema.py
--rw-r--r--   0        0        0      282 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/ptab/session.py
--rw-r--r--   0        0        0      159 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/ptab/util.py
--rw-r--r--   0        0        0       72 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     4943 2023-01-20 21:05:24.512394 patent_client-3.2.2/src/patent_client/uspto/public_search/api.py
--rw-r--r--   0        0        0     3891 2023-01-20 21:05:24.596393 patent_client-3.2.2/src/patent_client/uspto/public_search/manager.py
--rw-r--r--   0        0        0    12219 2023-01-20 21:05:24.596393 patent_client-3.2.2/src/patent_client/uspto/public_search/model.py
--rw-r--r--   0        0        0     7145 2023-01-20 21:05:24.596393 patent_client-3.2.2/src/patent_client/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4331 2023-01-20 21:05:24.596393 patent_client-3.2.2/src/patent_client/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2023-01-20 21:05:24.596393 patent_client-3.2.2/src/patent_client/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     3324 2023-01-20 21:05:24.596393 patent_client-3.2.2/src/patent_client/uspto/public_search/query_test.py
--rw-r--r--   0        0        0    10290 2023-01-20 21:05:24.596393 patent_client-3.2.2/src/patent_client/uspto/public_search/schema.py
--rw-r--r--   0        0        0     1094 2023-01-20 21:05:24.596393 patent_client-3.2.2/src/patent_client/uspto/public_search/schema_test.py
--rw-r--r--   0        0        0   387227 2023-01-20 21:05:24.608394 patent_client-3.2.2/src/patent_client/uspto/public_search/test/biblio.json
--rw-r--r--   0        0        0   213101 2023-01-20 21:05:24.608394 patent_client-3.2.2/src/patent_client/uspto/public_search/test/biblio_expected.json
--rw-r--r--   0        0        0  2431829 2023-01-20 21:05:24.608394 patent_client-3.2.2/src/patent_client/uspto/public_search/test/docs.json
--rw-r--r--   0        0        0  1880230 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/uspto/public_search/test/docs_expected.json
--rw-r--r--   0        0        0      565 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/__init__.py
--rw-r--r--   0        0        0        0 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/base/__init__.py
--rw-r--r--   0        0        0     5030 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/base/manager.py
--rw-r--r--   0        0        0     1696 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/base/model.py
--rw-r--r--   0        0        0      775 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/base/model_test.py
--rw-r--r--   0        0        0     3148 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/base/related.py
--rw-r--r--   0        0        0        0 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/base/test_manager.py
--rw-r--r--   0        0        0     1913 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/base/util.py
--rw-r--r--   0        0        0        0 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4263 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6204 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      834 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3565 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      931 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      204 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/datetime/__init__.py
--rw-r--r--   0        0        0     5774 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/datetime/date_parse.py
--rw-r--r--   0        0        0     9054 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/datetime/date_parse_test.py
--rw-r--r--   0        0        0    15027 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/datetime/functional.py
--rw-r--r--   0        0        0    12808 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/datetime/regex_helper.py
--rw-r--r--   0        0        0      611 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/format.py
--rw-r--r--   0        0        0     2699 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2023-01-20 21:05:24.612393 patent_client-3.2.2/src/patent_client/version.py
--rw-r--r--   0        0        0     7596 1970-01-01 00:00:00.000000 patent_client-3.2.2/setup.py
--rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 patent_client-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0      593 2023-04-30 00:17:13.630604 patent_client-3.2.3/LICENSE
+-rw-r--r--   0        0        0     4414 2023-04-30 00:17:13.630604 patent_client-3.2.3/README.md
+-rw-r--r--   0        0        0     3485 2023-04-30 00:17:13.670605 patent_client-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2590 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/default_settings.yml
+-rw-r--r--   0        0        0        0 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/epo/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:17:13.670605 patent_client-3.2.3/src/patent_client/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      350 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/api.py
+-rw-r--r--   0        0        0      406 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     8854 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/examples/example.xml
+-rw-r--r--   0        0        0     7248 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/expected/example.json
+-rw-r--r--   0        0        0     8853 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/expected/example.xml
+-rw-r--r--   0        0        0      304 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1180 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/model.py
+-rw-r--r--   0        0        0     1603 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      594 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0       77 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      355 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      380 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0   285423 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx
+-rw-r--r--   0        0        0      323 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2117 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     4163 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      283 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4041 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0      904 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0    76105 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/example.xml
+-rw-r--r--   0        0        0    44095 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/example.json
+-rw-r--r--   0        0        0    76104 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/example.xml
+-rw-r--r--   0        0        0    11924 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/us_example.json
+-rw-r--r--   0        0        0    22970 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/test/us_example.xml
+-rw-r--r--   0        0        0      114 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1239 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1269 2023-04-30 00:17:13.674605 patent_client-3.2.3/src/patent_client/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1102 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      600 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      972 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5024 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/api.py
+-rw-r--r--   0        0        0     1884 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     3127 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2043 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      399 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2633 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1095 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     1610 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      776 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      306 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3943 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      891 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1652 2023-04-30 00:17:13.678604 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      668 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3099 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     3973 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0     5916 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     9015 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34663 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     2318 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/session.py
+-rw-r--r--   0        0        0     1613 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/epo/ops/util.py
+-rw-r--r--   0        0        0     5991 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/parser.py
+-rw-r--r--   0        0        0     1129 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/session.py
+-rw-r--r--   0        0        0     1300 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/test_parser.py
+-rw-r--r--   0        0        0      278 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/uspto/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-30 00:17:13.682605 patent_client-3.2.3/src/patent_client/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     3822 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4269 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     3404 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/model.py
+-rw-r--r--   0        0        0     3473 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/schema.py
+-rw-r--r--   0        0        0     2234 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/schema_test.py
+-rw-r--r--   0        0        0    13274 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_1.xml
+-rw-r--r--   0        0        0    11638 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_2.xml
+-rw-r--r--   0        0        0   277704 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_3.xml
+-rw-r--r--   0        0        0       76 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     1161 2023-04-30 00:17:13.694605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     2983 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1979 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     5405 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3705 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     5062 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5146 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     2094 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/schema.py
+-rw-r--r--   0        0        0      983 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/schema_test.py
+-rw-r--r--   0        0        0      271 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/session.py
+-rw-r--r--   0        0        0     4134 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      117 2023-04-30 00:17:13.698605 patent_client-3.2.3/src/patent_client/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     7525 2023-04-30 00:17:13.722605 patent_client-3.2.3/src/patent_client/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9017 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    19234 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/model.py
+-rw-r--r--   0        0        0     8250 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/schema.py
+-rw-r--r--   0        0        0      529 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/schema_test.py
+-rw-r--r--   0        0        0    94546 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/test/app_12721698.json
+-rw-r--r--   0        0        0    15274 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/peds/test/expected.json
+-rw-r--r--   0        0        0      331 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0     5774 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/developer.uspto.gov.crt
+-rw-r--r--   0        0        0     3207 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2135 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     7387 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/model.py
+-rw-r--r--   0        0        0    69917 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/ptabApiV2.json
+-rw-r--r--   0        0        0     3597 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/schema.py
+-rw-r--r--   0        0        0      282 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/session.py
+-rw-r--r--   0        0        0      159 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/ptab/util.py
+-rw-r--r--   0        0        0       72 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     4943 2023-04-30 00:17:13.726605 patent_client-3.2.3/src/patent_client/uspto/public_search/api.py
+-rw-r--r--   0        0        0     3891 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/manager.py
+-rw-r--r--   0        0        0    12219 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/model.py
+-rw-r--r--   0        0        0     7277 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4331 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     3689 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0    10290 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/schema.py
+-rw-r--r--   0        0        0     1254 2023-04-30 00:17:13.810605 patent_client-3.2.3/src/patent_client/uspto/public_search/schema_test.py
+-rw-r--r--   0        0        0   387227 2023-04-30 00:17:13.822605 patent_client-3.2.3/src/patent_client/uspto/public_search/test/biblio.json
+-rw-r--r--   0        0        0   213101 2023-04-30 00:17:13.822605 patent_client-3.2.3/src/patent_client/uspto/public_search/test/biblio_expected.json
+-rw-r--r--   0        0        0  2431829 2023-04-30 00:17:13.826605 patent_client-3.2.3/src/patent_client/uspto/public_search/test/docs.json
+-rw-r--r--   0        0        0  1880230 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/uspto/public_search/test/docs_expected.json
+-rw-r--r--   0        0        0      565 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/__init__.py
+-rw-r--r--   0        0        0     5030 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/manager.py
+-rw-r--r--   0        0        0     1696 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/model.py
+-rw-r--r--   0        0        0      775 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/model_test.py
+-rw-r--r--   0        0        0     3148 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/related.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/test_manager.py
+-rw-r--r--   0        0        0     1913 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/base/util.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4263 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6204 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      834 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3565 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      931 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      204 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/__init__.py
+-rw-r--r--   0        0        0     5774 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/date_parse.py
+-rw-r--r--   0        0        0     9054 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/date_parse_test.py
+-rw-r--r--   0        0        0    15027 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/functional.py
+-rw-r--r--   0        0        0    12808 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/datetime/regex_helper.py
+-rw-r--r--   0        0        0      611 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/format.py
+-rw-r--r--   0        0        0     2699 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2023-04-30 00:17:13.830605 patent_client-3.2.3/src/patent_client/version.py
+-rw-r--r--   0        0        0     6965 1970-01-01 00:00:00.000000 patent_client-3.2.3/PKG-INFO
```

### Comparing `patent_client-3.2.2/LICENSE` & `patent_client-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/README.md` & `patent_client-3.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 Docs, including a fulsome Getting Started and User Guide are available on [Read the Docs](http://patent-client.readthedocs.io). The Examples folder includes examples of using `patent_client` for
 many common IP tasks
 
 ## Coverage
 
 - [United States Patent & Trademark Office][USPTO]
 
-  - [Patent Public Search][PPS] - Full Support
   - [Patent Examination Data][PEDS] - Full Support
   - [Global Dossier][GD] - Full Support
   - [Patent Assignment Data][Assignment] - Lookup Support
   - [Patent Trial & Appeal Board API v2][PTAB] - Supports Proceedings, Decisions, and Documents
+  - ~~[Patent Public Search][PPS] - Full Support~~ (Broken due to USPTO WAF)
 
 
 - [European Patent Office - Open Patent Services][OPS]
 
   - Inpadoc - Full Support
   - EPO Register - No Support (in progress)
   - Classification - No Support
@@ -64,24 +64,15 @@
 
 ## Quick Start
 
 To use the project:
 
 ```python
 # Import the model classes you need
->>> from patent_client import Inpadoc, Assignment, USApplication, PatentBiblio
-
-# Fetch US Patents with the word "tennis" in their title issued in 2010
->>> pats = PatentBiblio.objects.filter(title="tennis", issue_date="2010-01-01->2010-12-31")
->>> len(pats) > 10
-True
-
-# Look at the first one
->>> pats[0]
-PublicationBiblio(publication_number=7841958, publication_date=2010-11-30, patent_title=Modular table tennis game)
+>>> from patent_client import Inpadoc, Assignment, USApplication
 
 # Fetch US Applications
 >>> app = USApplication.objects.get('15710770')
 >>> app.patent_title
 'Camera Assembly with Concave-Shaped Front Face'
 
 # Fetch from USPTO Assignments
```

### Comparing `patent_client-3.2.2/pyproject.toml` & `patent_client-3.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent_client"
-version = "3.2.2"
+version = "3.2.3"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
```

### Comparing `patent_client-3.2.2/src/patent_client/__init__.py` & `patent_client-3.2.3/src/patent_client/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/family/fixtures/examples/example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/examples/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/family/fixtures/expected/example.json` & `patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/expected/example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/family/fixtures/expected/example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/family/fixtures/expected/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/family/model.py` & `patent_client-3.2.3/src/patent_client/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/family/schema.py` & `patent_client-3.2.3/src/patent_client/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/family/schema_test.py` & `patent_client-3.2.3/src/patent_client/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/legal_code_descriptions_20221112.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/model.py` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/national_codes.py` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/national_codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,18 @@
 
 def has_current_spreadsheet():
     con = sqlite3.connect(db_location, timeout=30)
     cur = con.cursor()
     try:
         fname = cur.execute("SELECT * FROM meta").fetchone()[0]
         date_string = re.search(r"legal_code_descriptions_(\d+)\.xlsx", fname).group(1)
-        date = datetime.datetime.strptime(date_string, "%Y%m%d").date()
+        try:
+            date = datetime.datetime.strptime(date_string, "%Y%W").date()
+        except ValueError:
+            date = datetime.datetime.strptime(date_string, "%Y%m%d").date()
         age = datetime.datetime.now().date() - date
         logger.debug(f"Legal Code Database is {age} days old")
         return age.days <= 30
     except (sqlite3.OperationalError, TypeError):
         return False
```

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/schema.py` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/schema_test.py` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/test/example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/test/expected/example.json` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/test/expected/example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/test/expected/us_example.json` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/expected/us_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/legal/test/us_example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/legal/test/us_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/number_service/api.py` & `patent_client-3.2.3/src/patent_client/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/number_service/api_test.py` & `patent_client-3.2.3/src/patent_client/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/number_service/errors.py` & `patent_client-3.2.3/src/patent_client/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/number_service/errors.txt` & `patent_client-3.2.3/src/patent_client/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/number_service/messages.txt` & `patent_client-3.2.3/src/patent_client/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/number_service/model.py` & `patent_client-3.2.3/src/patent_client/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/number_service/schema.py` & `patent_client-3.2.3/src/patent_client/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/api.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/api_test.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/api_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 expected_dir = Path(__file__).parent / "test" / "expected"
 
 
 def test_doc_example_biblio():
     result = PublishedApi.biblio.get_biblio("EP1000000.A1", format="epodoc")
     expected_file = expected_dir / "ep1000000_biblio_result.xml"
-    # expected_file.write_text(result)
-    expected = expected_file.read_text()
+    expected_file.write_text(result, encoding="utf8")
+    expected = expected_file.read_text(encoding="utf8")
     assert result == expected
 
 
 def test_doc_example_full_cycle():
     result = PublishedApi.biblio.get_full_cycle("EP1000000.A1", format="epodoc")
     expected_file = expected_dir / "ep1000000_full_cycle_result.xml"
-    # expected_file.write_text(result)
-    expected = expected_file.read_text()
+    expected_file.write_text(result, encoding="utf8")
+    expected = expected_file.read_text(encoding="utf8")
     assert result == expected
 
 
 def test_doc_example_abstract():
     result = PublishedApi.biblio.get_abstract("EP1000000.A1", format="epodoc")
     expected_file = expected_dir / "ep1000000_abstract_result.xml"
-    # expected_file.write_text(result)
-    expected = expected_file.read_text()
+    expected_file.write_text(result, encoding="utf8")
+    expected = expected_file.read_text(encoding="utf8")
     assert result == expected
 
 
 def test_search():
     result = PublishedApi.search.search("ti=plastic")
     expected_file = expected_dir / "search_result.xml"
     # expected_file.write_text(result)
```

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/cql.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/manager.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/manager_test.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/model/biblio.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/model/fulltext.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/model/images.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/model/search.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/schema/biblio.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/schema/fulltext.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/schema/images.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/schema/search.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/schema_test.py` & `patent_client-3.2.3/src/patent_client/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/biblio_example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/biblio_example_2.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/biblio_example_3.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/biblio_example_4.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/claims_example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/claims_example_2.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/description_example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/claims_example.json` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/image_example.json` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/expected/search_result.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/full_cycle_example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/image_example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/published/test/search_example.xml` & `patent_client-3.2.3/src/patent_client/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/session.py` & `patent_client-3.2.3/src/patent_client/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/epo/ops/util.py` & `patent_client-3.2.3/src/patent_client/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/parser.py` & `patent_client-3.2.3/src/patent_client/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/session.py` & `patent_client-3.2.3/src/patent_client/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/settings.py` & `patent_client-3.2.3/src/patent_client/settings.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/test_parser.py` & `patent_client-3.2.3/src/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/assignment/manager.py` & `patent_client-3.2.3/src/patent_client/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/assignment/manager_test.py` & `patent_client-3.2.3/src/patent_client/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/assignment/model.py` & `patent_client-3.2.3/src/patent_client/uspto/assignment/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/assignment/schema.py` & `patent_client-3.2.3/src/patent_client/uspto/assignment/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/assignment/schema_test.py` & `patent_client-3.2.3/src/patent_client/uspto/assignment/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/assignment/test/assignment_1.xml` & `patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/assignment/test/assignment_2.xml` & `patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/assignment/test/assignment_3.xml` & `patent_client-3.2.3/src/patent_client/uspto/assignment/test/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/api.py` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/gd_input.csv` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/manager.py` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/model.py` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     __manager__ = "patent_client.uspto.global_dossier.manager.GlobalDossierApplicationManager"
     app_num: "str" = None
     app_date: "datetime.date" = None
     country_code: "str" = None
     kind_code: "str" = None
     doc_num: "GlobalDossierDocumentNumber" = None
     title: "str" = None
-    applicantNames: "str" = None
+    applicant_names: "str" = None
     ip_5: "bool" = None
     priority_claim_list: "ListCollection[GlobalDossierPriorityClaim]" = field(default_factory=ListCollection)
     pub_list: "ListCollection[GlobalDossierPublication]" = field(default_factory=ListCollection)
 
     def __repr__(self):
         return f"GlobalDossierApplication(app_num={self.app_num}, country_code={self.country_code})"
 
@@ -130,16 +130,18 @@
     date: "datetime.date" = None
     doc_format: "str" = None
     pages: "int" = None
     doc_code_desc: "str" = None
     doc_group_code: "str" = None
     shareable: "bool" = None
 
-    def download(self, path="."):
-        out_path = Path(path).expanduser() / f'{self.date.isoformat()} - {self.doc_desc.replace("/", "_")}'
+    def download(self, filename="", path="."):
+        out_path = Path(path).expanduser() / (
+            f'{self.date.isoformat()} - {self.doc_desc.replace("/", "_")}.pdf' if not filename else filename
+        )
         return global_dossier_api.get_document(self.country, self.doc_number, self.doc_id, out_path=out_path)
 
 
 @dataclass
 class DocumentList(Model):
     __manager__ = "patent_client.uspto.global_dossier.manager.GlobalDossierDocument"
     title: "str" = None
```

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/model_test.py` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/model_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,33 +34,37 @@
     assert isinstance(result.documents, list)
     assert isinstance(result.documents[0], Document)
     assert isinstance(result.office_actions, list)
     assert isinstance(result.office_actions[0], Document)
 
 
 def test_links():
+
+    app = GlobalDossierApplication.objects.get("16123456")
     assert (
-        GlobalDossierApplication.objects.get("16123456").us_application.patent_title
+        app.us_application.patent_title
         == "LEARNING ASSISTANCE DEVICE, METHOD OF OPERATING LEARNING ASSISTANCE DEVICE, LEARNING ASSISTANCE PROGRAM, LEARNING ASSISTANCE SYSTEM, AND TERMINAL DEVICE"
     )
-    assert (
-        GlobalDossierApplication.objects.get("16123456").us_publication.patent_title
-        == "Learning assistance device, method of operating learning assistance device, learning assistance program, learning assistance system, and terminal device"
-    )
-    assert (
-        GlobalDossierApplication.objects.get("16123456").us_patent.patent_title
-        == "Learning assistance device, method of operating learning assistance device, learning assistance program, learning assistance system, and terminal device"
-    )
-    assert GlobalDossierApplication.objects.get("16123456").us_assignments.first().id == "46816-108"
+    # Broken links to Public Patent Search
+    # assert (
+    #    GlobalDossierApplication.objects.get("16123456").us_publication.patent_title
+    #    == "Learning assistance device, method of operating learning assistance device, learning assistance program, learning assistance system, and terminal device"
+    # )
+    # assert (
+    #    GlobalDossierApplication.objects.get("16123456").us_patent.patent_title
+    #    == "Learning assistance device, method of operating learning assistance device, learning assistance program, learning assistance system, and terminal device"
+    # )
+    assert app.us_assignments.first().id == "46816-108"
     with pytest.raises(ValueError):
         GlobalDossierApplication.objects.get(publication="EP1000000").us_application
-    with pytest.raises(ValueError):
-        GlobalDossierApplication.objects.get(publication="EP1000000").us_publication
-    with pytest.raises(ValueError):
-        GlobalDossierApplication.objects.get(publication="EP1000000").us_patent
+    # Broken links to Public Patent Search
+    # with pytest.raises(ValueError):
+    #    GlobalDossierApplication.objects.get(publication="EP1000000").us_publication
+    # with pytest.raises(ValueError):
+    #    GlobalDossierApplication.objects.get(publication="EP1000000").us_patent
     with pytest.raises(ValueError):
         GlobalDossierApplication.objects.get(publication="EP1000000").us_assignments
 
 
 def test_raises_errors_on_db_methods():
     with pytest.raises(NotImplementedError):
         GlobalDossier.objects.filter("something")
@@ -74,7 +78,14 @@
         GlobalDossierDocument().filter("something")
     with pytest.raises(NotImplementedError):
         GlobalDossierDocument().order_by("something")
     with pytest.raises(NotImplementedError):
         GlobalDossierDocument().limit("something")
     with pytest.raises(NotImplementedError):
         GlobalDossierDocument().offset("something")
+
+
+def test_issue_99():
+    app = GlobalDossierApplication.objects.get("16740760", type="application", office="US")
+    assert app.app_num == "16740760"
+    app = GlobalDossierApplication.objects.get("17193105")
+    assert app.app_num == "17193105"
```

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/query.py` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/query_test.py` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/schema.py` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 class GlobalDossierApplicationSchema(Schema):
     app_num = f.Str()
     app_date = f.Date("appDateStr")
     country_code = f.Str()
     kind_code = f.Str()
     doc_num = GlobalDossierDocumentNumberSchema("docNum")
     title = f.Str()
-    applicantNames = f.Str()
+    applicant_names = f.Str()
     ip_5 = f.Bool("ip5")
     priority_claim_list = f.List(GlobalDossierPriorityClaimSchema)
     pub_list = f.List(GlobalDossierPublicationSchema)
 
 
 class GlobalDossierSchema(Schema):
     country = f.Str()
```

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/schema_test.py` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/test/app.json` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/test/app_expected.json` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/test/doc_list.json` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-3.2.3/src/patent_client/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/peds/manager.py` & `patent_client-3.2.3/src/patent_client/uspto/peds/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/peds/manager_test.py` & `patent_client-3.2.3/src/patent_client/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/peds/model.py` & `patent_client-3.2.3/src/patent_client/uspto/peds/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/peds/schema.py` & `patent_client-3.2.3/src/patent_client/uspto/peds/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/peds/schema_test.py` & `patent_client-3.2.3/src/patent_client/uspto/peds/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/peds/test/app_12721698.json` & `patent_client-3.2.3/src/patent_client/uspto/peds/test/app_12721698.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/peds/test/expected.json` & `patent_client-3.2.3/src/patent_client/uspto/peds/test/expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/ptab/developer.uspto.gov.crt` & `patent_client-3.2.3/src/patent_client/uspto/ptab/developer.uspto.gov.crt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/ptab/manager.py` & `patent_client-3.2.3/src/patent_client/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/ptab/manager_test.py` & `patent_client-3.2.3/src/patent_client/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/ptab/model.py` & `patent_client-3.2.3/src/patent_client/uspto/ptab/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/ptab/ptabApiV2.json` & `patent_client-3.2.3/src/patent_client/uspto/ptab/ptabApiV2.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/ptab/schema.py` & `patent_client-3.2.3/src/patent_client/uspto/ptab/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/api.py` & `patent_client-3.2.3/src/patent_client/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/manager.py` & `patent_client-3.2.3/src/patent_client/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/model.py` & `patent_client-3.2.3/src/patent_client/uspto/public_search/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/model_test.py` & `patent_client-3.2.3/src/patent_client/uspto/public_search/model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import pytest
+
 from .model import Patent
 from .model import PatentBiblio
 from .model import PublicSearch
 from .model import PublishedApplication
 from .model import PublishedApplicationBiblio
 
 
-def test_simple_lookup():
-    app = PublicSearch.objects.get(patent_number="6103599")
-    assert app.appl_id == "09089931"
-    assert app.guid == "US-6103599-A"
-    assert app.patent_title == "Planarizing technique for multilayered substrates"
-
-
+@pytest.mark.skip("PPS API currently broken :(")
 class TestPatents:
+    def test_simple_lookup():
+        app = PublicSearch.objects.get(patent_number="6103599")
+        assert app.appl_id == "09089931"
+        assert app.guid == "US-6103599-A"
+        assert app.patent_title == "Planarizing technique for multilayered substrates"
+
     def test_tennis_patents(self):
         tennis_patents = Patent.objects.filter(title="tennis", assignee_name="wilson")
         assert len(tennis_patents) > 10
 
     def test_fetch_patent(self):
         pat = Patent.objects.get(6095661)
         assert pat.patent_title == "Method and apparatus for an L.E.D. flashlight"
@@ -113,14 +115,15 @@
     def test_can_get_images(self, tmp_path):
         pat = Patent.objects.get("6103599")
         path = pat.download_images(path=tmp_path)
         assert path == tmp_path / "US-6103599-A.pdf"
         assert path.exists()
 
 
+@pytest.mark.skip("PPS API currently broken :(")
 class TestPublishedApplicationFullText:
     def test_fetch_publication(self):
         pub_no = 20_160_009_839
         pub = PublishedApplication.objects.get(pub_no)
         assert (
             pub.patent_title == "POLYMER PRODUCTS AND MULTI-STAGE POLYMERIZATION PROCESSES FOR THE PRODUCTION THEREOF"
         )
```

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/query.py` & `patent_client-3.2.3/src/patent_client/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/query_config.csv` & `patent_client-3.2.3/src/patent_client/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/query_test.py` & `patent_client-3.2.3/src/patent_client/uspto/public_search/query_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,90 +1,86 @@
 import pytest
 from dateutil.parser import parse as parse_dt
 
 from .manager import PatentBiblioManager
 from .query import QueryException
 
 
-def test_default_query():
-    assert PatentBiblioManager().filter("6103599")._query == '"6103599".PN.'
-
-
-def test_plural_default_query():
-    assert PatentBiblioManager().filter("6103599", "6103600")._query == '("6103599" "6103600").PN.'
-
-
-def test_keyword_query():
-    assert PatentBiblioManager().filter(appl_id="6103599")._query == '"6103599".APNR.'
-
-
-def test_plural_keyword_query():
-    assert PatentBiblioManager().filter(appl_id=("11111111", "11222222"))._query == '("11111111" "11222222").APNR.'
-
-
-def test_keyword_date_query():
-    assert PatentBiblioManager().filter(app_filing_date="2021-01-01")._query == '@APD="20210101"'
-    assert PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01"))._query == '@APD="20210101"'
-    assert PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01").date())._query == '@APD="20210101"'
-
-
-def test_keyword_date_range_query():
-    assert PatentBiblioManager().filter(app_filing_date="2021-01-01->2021-02-01")._query == "@APD>=20210101<=20210201"
-    assert (
-        PatentBiblioManager().filter(app_filing_date__range=("2021-01-01", "2021-02-01"))._query
-        == "@APD>=20210101<=20210201"
-    )
-    assert (
-        PatentBiblioManager().filter(app_filing_date__range=(parse_dt("2021-01-01"), parse_dt("2021-02-01")))._query
-        == "@APD>=20210101<=20210201"
-    )
-
-
-def test_date_operator_queries():
-    assert PatentBiblioManager().filter(app_filing_date__gt="2021-01-01")._query == '@APD>"20210101"'
-    assert PatentBiblioManager().filter(app_filing_date__gte="2021-01-01")._query == '@APD>="20210101"'
-    assert PatentBiblioManager().filter(app_filing_date__lt="2021-01-01")._query == '@APD<"20210101"'
-    assert PatentBiblioManager().filter(app_filing_date__lte="2021-01-01")._query == '@APD<="20210101"'
-
-
-def test_error_query():
-    with pytest.raises(QueryException):
-        PatentBiblioManager().filter(blargh="2021-01-01")._query
-
-
-def test_error_date_query():
-    with pytest.raises(QueryException):
-        q = PatentBiblioManager().filter(app_filing_date="2021-00-01")._query
-    with pytest.raises(QueryException):
-        q = PatentBiblioManager().filter(app_filing_date=False)._query
-
-
-def test_multiple_fields():
-    assert (
-        PatentBiblioManager().filter("6103599", app_filing_date="2021-01-01")._query
-        == '@APD="20210101" AND "6103599".PN.'
-    )
-    assert (
-        PatentBiblioManager().filter("6103599").filter(app_filing_date="2021-01-01")._query
-        == '"6103599".PN. AND @APD="20210101"'
-    )
-    assert (
-        PatentBiblioManager().filter(patent_number="6103599", app_filing_date="2021-01-01")._query
-        == '@APD="20210101" AND "6103599".PN.'
-    )
-
-
-def test_raw_query():
-    assert PatentBiblioManager().filter(query="example query")._query == "example query"
-
-
-def test_raw_query_with_keywords():
-    assert (
-        PatentBiblioManager().filter(query="some text", patent_number="6103599")._query == '"6103599".PN. AND some text'
-    )
-
-
-def test_default_or():
-    assert (
-        PatentBiblioManager().option(default_operator="OR").filter(patent_number="6103599", appl_id="1234567")._query
-        == '"1234567".APNR. OR "6103599".PN.'
-    )
+@pytest.mark.skip("PPS API currently broken :(")
+class QueryTest:
+    def test_default_query():
+        assert PatentBiblioManager().filter("6103599")._query == '"6103599".PN.'
+
+    def test_plural_default_query():
+        assert PatentBiblioManager().filter("6103599", "6103600")._query == '("6103599" "6103600").PN.'
+
+    def test_keyword_query():
+        assert PatentBiblioManager().filter(appl_id="6103599")._query == '"6103599".APNR.'
+
+    def test_plural_keyword_query():
+        assert PatentBiblioManager().filter(appl_id=("11111111", "11222222"))._query == '("11111111" "11222222").APNR.'
+
+    def test_keyword_date_query():
+        assert PatentBiblioManager().filter(app_filing_date="2021-01-01")._query == '@APD="20210101"'
+        assert PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01"))._query == '@APD="20210101"'
+        assert PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01").date())._query == '@APD="20210101"'
+
+    def test_keyword_date_range_query():
+        assert (
+            PatentBiblioManager().filter(app_filing_date="2021-01-01->2021-02-01")._query == "@APD>=20210101<=20210201"
+        )
+        assert (
+            PatentBiblioManager().filter(app_filing_date__range=("2021-01-01", "2021-02-01"))._query
+            == "@APD>=20210101<=20210201"
+        )
+        assert (
+            PatentBiblioManager().filter(app_filing_date__range=(parse_dt("2021-01-01"), parse_dt("2021-02-01")))._query
+            == "@APD>=20210101<=20210201"
+        )
+
+    def test_date_operator_queries():
+        assert PatentBiblioManager().filter(app_filing_date__gt="2021-01-01")._query == '@APD>"20210101"'
+        assert PatentBiblioManager().filter(app_filing_date__gte="2021-01-01")._query == '@APD>="20210101"'
+        assert PatentBiblioManager().filter(app_filing_date__lt="2021-01-01")._query == '@APD<"20210101"'
+        assert PatentBiblioManager().filter(app_filing_date__lte="2021-01-01")._query == '@APD<="20210101"'
+
+    def test_error_query():
+        with pytest.raises(QueryException):
+            PatentBiblioManager().filter(blargh="2021-01-01")._query
+
+    def test_error_date_query():
+        with pytest.raises(QueryException):
+            q = PatentBiblioManager().filter(app_filing_date="2021-00-01")._query
+        with pytest.raises(QueryException):
+            q = PatentBiblioManager().filter(app_filing_date=False)._query
+
+    def test_multiple_fields():
+        assert (
+            PatentBiblioManager().filter("6103599", app_filing_date="2021-01-01")._query
+            == '@APD="20210101" AND "6103599".PN.'
+        )
+        assert (
+            PatentBiblioManager().filter("6103599").filter(app_filing_date="2021-01-01")._query
+            == '"6103599".PN. AND @APD="20210101"'
+        )
+        assert (
+            PatentBiblioManager().filter(patent_number="6103599", app_filing_date="2021-01-01")._query
+            == '@APD="20210101" AND "6103599".PN.'
+        )
+
+    def test_raw_query():
+        assert PatentBiblioManager().filter(query="example query")._query == "example query"
+
+    def test_raw_query_with_keywords():
+        assert (
+            PatentBiblioManager().filter(query="some text", patent_number="6103599")._query
+            == '"6103599".PN. AND some text'
+        )
+
+    def test_default_or():
+        assert (
+            PatentBiblioManager()
+            .option(default_operator="OR")
+            .filter(patent_number="6103599", appl_id="1234567")
+            ._query
+            == '"1234567".APNR. OR "6103599".PN.'
+        )
```

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/schema.py` & `patent_client-3.2.3/src/patent_client/uspto/public_search/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/schema_test.py` & `patent_client-3.2.3/src/patent_client/uspto/public_search/schema_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import json
 from pathlib import Path
 
+import pytest
 from patent_client.util.test import compare_dicts
 
 from .schema import PublicSearchDocumentSchema
 from .schema import PublicSearchSchema
 
 test_dir = Path(__file__).parent / "test"
 
 
-def test_biblio():
-    data = (test_dir / "biblio.json").read_text()
-    parser = PublicSearchSchema()
-    result = parser.load_batch(data)
-    expected_file = test_dir / "biblio_expected.json"
-    expected_file.write_text(result.to_json(indent=2))
-    expected = json.loads(expected_file.read_text())
-    result_json = json.loads(result.to_json())
-    for i in range(len(expected)):
-        compare_dicts(expected[i], result_json[i])
-
-
-def test_docs():
-    data = (test_dir / "docs.json").read_text()
-    parser = PublicSearchDocumentSchema()
-    result = parser.load_batch(data)
-    expected_file = test_dir / "docs_expected.json"
-    expected_file.write_text(result.to_json(indent=2))
-    expected = json.loads(expected_file.read_text())
-    result_json = json.loads(result.to_json())
-    for i in range(len(expected)):
-        compare_dicts(expected[i], result_json[i])
+@pytest.mark.skip("PPS API currently broken :(")
+class TestSchema:
+    def test_biblio():
+        data = (test_dir / "biblio.json").read_text()
+        parser = PublicSearchSchema()
+        result = parser.load_batch(data)
+        expected_file = test_dir / "biblio_expected.json"
+        expected_file.write_text(result.to_json(indent=2))
+        expected = json.loads(expected_file.read_text())
+        result_json = json.loads(result.to_json())
+        for i in range(len(expected)):
+            compare_dicts(expected[i], result_json[i])
+
+    def test_docs():
+        data = (test_dir / "docs.json").read_text()
+        parser = PublicSearchDocumentSchema()
+        result = parser.load_batch(data)
+        expected_file = test_dir / "docs_expected.json"
+        expected_file.write_text(result.to_json(indent=2))
+        expected = json.loads(expected_file.read_text())
+        result_json = json.loads(result.to_json())
+        for i in range(len(expected)):
+            compare_dicts(expected[i], result_json[i])
```

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/test/biblio.json` & `patent_client-3.2.3/src/patent_client/uspto/public_search/test/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/test/biblio_expected.json` & `patent_client-3.2.3/src/patent_client/uspto/public_search/test/biblio_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/test/docs.json` & `patent_client-3.2.3/src/patent_client/uspto/public_search/test/docs.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/uspto/public_search/test/docs_expected.json` & `patent_client-3.2.3/src/patent_client/uspto/public_search/test/docs_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/__init__.py` & `patent_client-3.2.3/src/patent_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/base/manager.py` & `patent_client-3.2.3/src/patent_client/util/base/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/base/model.py` & `patent_client-3.2.3/src/patent_client/util/base/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/base/model_test.py` & `patent_client-3.2.3/src/patent_client/util/base/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/base/related.py` & `patent_client-3.2.3/src/patent_client/util/base/related.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/base/util.py` & `patent_client-3.2.3/src/patent_client/util/base/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-3.2.3/src/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-3.2.3/src/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/claims/examples/published_claims.json` & `patent_client-3.2.3/src/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/claims/examples/published_claims.txt` & `patent_client-3.2.3/src/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/claims/model.py` & `patent_client-3.2.3/src/patent_client/util/claims/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/claims/parser.py` & `patent_client-3.2.3/src/patent_client/util/claims/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/claims/parser_test.py` & `patent_client-3.2.3/src/patent_client/util/claims/parser_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/datetime/date_parse.py` & `patent_client-3.2.3/src/patent_client/util/datetime/date_parse.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/datetime/date_parse_test.py` & `patent_client-3.2.3/src/patent_client/util/datetime/date_parse_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/datetime/functional.py` & `patent_client-3.2.3/src/patent_client/util/datetime/functional.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/datetime/regex_helper.py` & `patent_client-3.2.3/src/patent_client/util/datetime/regex_helper.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/format.py` & `patent_client-3.2.3/src/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/src/patent_client/util/test.py` & `patent_client-3.2.3/src/patent_client/util/test.py`

 * *Files identical despite different names*

### Comparing `patent_client-3.2.2/PKG-INFO` & `patent_client-3.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patent-client
-Version: 3.2.2
+Version: 3.2.3
 Summary: A set of ORM-style clients for publicly available intellectual property data
 Home-page: https://github.com/parkerhancock/patent_client
 License: Apache Software License 2.0
 Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -73,19 +73,19 @@
 Docs, including a fulsome Getting Started and User Guide are available on [Read the Docs](http://patent-client.readthedocs.io). The Examples folder includes examples of using `patent_client` for
 many common IP tasks
 
 ## Coverage
 
 - [United States Patent & Trademark Office][USPTO]
 
-  - [Patent Public Search][PPS] - Full Support
   - [Patent Examination Data][PEDS] - Full Support
   - [Global Dossier][GD] - Full Support
   - [Patent Assignment Data][Assignment] - Lookup Support
   - [Patent Trial & Appeal Board API v2][PTAB] - Supports Proceedings, Decisions, and Documents
+  - ~~[Patent Public Search][PPS] - Full Support~~ (Broken due to USPTO WAF)
 
 
 - [European Patent Office - Open Patent Services][OPS]
 
   - Inpadoc - Full Support
   - EPO Register - No Support (in progress)
   - Classification - No Support
@@ -117,24 +117,15 @@
 
 ## Quick Start
 
 To use the project:
 
 ```python
 # Import the model classes you need
->>> from patent_client import Inpadoc, Assignment, USApplication, PatentBiblio
-
-# Fetch US Patents with the word "tennis" in their title issued in 2010
->>> pats = PatentBiblio.objects.filter(title="tennis", issue_date="2010-01-01->2010-12-31")
->>> len(pats) > 10
-True
-
-# Look at the first one
->>> pats[0]
-PublicationBiblio(publication_number=7841958, publication_date=2010-11-30, patent_title=Modular table tennis game)
+>>> from patent_client import Inpadoc, Assignment, USApplication
 
 # Fetch US Applications
 >>> app = USApplication.objects.get('15710770')
 >>> app.patent_title
 'Camera Assembly with Concave-Shaped Front Face'
 
 # Fetch from USPTO Assignments
```

