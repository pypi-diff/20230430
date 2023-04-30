# Comparing `tmp/cmap-0.0.0rc0.tar.gz` & `tmp/cmap-0.0.1.tar.gz`

## Comparing `cmap-0.0.0rc0.tar` & `cmap-0.0.1.tar`

### file list

```diff
@@ -1,23 +1,195 @@
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.github_changelog_generator
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/setup.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.github/dependabot.yml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.github/workflows/cron.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.ruff_cache/content-v2/sha256/5a/a7/4a6e2cf9897f337083ba13e9bd753ad13bce2c47b50da485c6028d78ee5d
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.ruff_cache/content-v2/sha256/72/5f/a0b9bd75ba2aec12a8dc6e6b233ca40b141be9bb5b423b6b2bc3a099ca14
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.ruff_cache/content-v2/sha256/8d/b9/d0a78c925b86ce6d1cfbeccc5220ae01233f9e0aef4e4eb8b1d592b19cee
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.ruff_cache/index-v5/28/99/6c72ceffc85196c72cbcb93ab16b9f37e928
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.ruff_cache/index-v5/3d/53/7e2b271587ebcfb8ff981cdde03eaa96ab9d
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.ruff_cache/index-v5/54/30/5a3015f92f9f8f405d016bd6f20e61856330
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/src/cmap/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/src/cmap/py.typed
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/tests/test_cmap.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/LICENSE
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/README.md
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 cmap-0.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/__init__.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/_catalog.py
+-rw-r--r--   0        0        0    20363 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/_color.py
+-rw-r--r--   0        0        0    44204 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/_colormap.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/_external.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/__init__.py
+-rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/bids/__init__.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/bids/record.json
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/chrisluts/record.json
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cividis/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cividis/record.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmap/record.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/__init__.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/algae.py
+-rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/amp.py
+-rw-r--r--   0        0        0    22339 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/balance.py
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/curl.py
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/deep.py
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/delta.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/dense.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/diff.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/haline.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/ice.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/matter.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/oxy.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/phase.py
+-rw-r--r--   0        0        0    17189 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/rain.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/record.json
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/solar.py
+-rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/speed.py
+-rw-r--r--   0        0        0    21589 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/tarn.py
+-rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/tempo.py
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/thermal.py
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/topo.py
+-rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cmocean/turbid.py
+-rw-r--r--   0        0        0    39760 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorbrewer/__init__.py
+-rw-r--r--   0        0        0    45183 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorbrewer/record.json
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C1.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C10.py
+-rw-r--r--   0        0        0     9105 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C11.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C2.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C3.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C4.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C5.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C6.py
+-rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C7.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C8.py
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_C9.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBC1.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBC2.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBD1.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBD2.py
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBL1.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBL2.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBL3.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBL4.py
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBTC1.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBTC2.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBTD1.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBTL1.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBTL2.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBTL3.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_CBTL4.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D1.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D10.py
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D11.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D12.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D13.py
+-rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D1A.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D2.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D3.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D4.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D5.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D6.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D7.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D8.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_D9.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_I1.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_I2.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_I3.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L1.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L10.py
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L11.py
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L12.py
+-rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L13.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L14.py
+-rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L15.py
+-rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L16.py
+-rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L17.py
+-rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L18.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L19.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L2.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L20.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L3.py
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L4.py
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L5.py
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L6.py
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L7.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L8.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_L9.py
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_R1.py
+-rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_R2.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_R3.py
+-rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/CET_R4.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/__init__.py
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/colorcet/record.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/__init__.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/acton.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/bam.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/bamO.py
+-rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/bamako.py
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/batlow.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/batlowK.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/batlowW.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/berlin.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/bilbao.py
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/broc.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/brocO.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/buda.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/bukavu.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/cork.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/corkO.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/davos.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/devon.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/fes.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/grayC.py
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/hawaii.py
+-rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/imola.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/lajolla.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/lapaz.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/lisbon.py
+-rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/nuuk.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/oleron.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/oslo.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/record.json
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/roma.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/romaO.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/tofino.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/tokyo.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/turku.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/vanimo.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/vik.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/crameri/vikO.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cubehelix/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/cubehelix/record.json
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/glasbey/__init__.py
+-rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/glasbey/_glasbey.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/glasbey/_grids.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/glasbey/_internals.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/glasbey/prebuilt.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/glasbey/record.json
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/gnuplot/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/gnuplot/record.json
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/google/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/google/record.json
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/imagej/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/imagej/record.json
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/matlab/__init__.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/matlab/record.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/matplotlib/_CMRmap.py
+-rw-r--r--   0        0        0    45909 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/matplotlib/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/matplotlib/_coolwarm.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/matplotlib/_wistia.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/matplotlib/record.json
+-rw-r--r--   0        0        0    64086 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/seaborn/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/seaborn/record.json
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/tableau/__init__.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/tableau/record.json
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/vispy/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/vispy/record.json
+-rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/yorick/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmap-0.0.1/src/cmap/data/yorick/record.json
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cmap-0.0.1/tests/test_catalog.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 cmap-0.0.1/tests/test_color.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 cmap-0.0.1/tests/test_colormap.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 cmap-0.0.1/tests/test_data.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 cmap-0.0.1/tests/test_glasbey.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 cmap-0.0.1/tests/test_model_fields.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 cmap-0.0.1/tests/test_third_party.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 cmap-0.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 cmap-0.0.1/.gitignore
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 cmap-0.0.1/README.md
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 cmap-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE_CMOCEAN
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE_COLORBREWER
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE_COLORCET
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE_CRAMERI
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE_CVIDIS
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE_GLASBEY
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE_WISTIA
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 cmap-0.0.1/LICENSE/LICENSE_YORICK
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 cmap-0.0.1/PKG-INFO
```

### Comparing `cmap-0.0.0rc0/.gitignore` & `cmap-0.0.1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 sdist/
 var/
 wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 
+.DS_Store
+
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
 # Installer logs
@@ -102,7 +104,10 @@
 .mypy_cache/
 
 # IDE settings
 .vscode/
 
 cmap/_version.py
 src/cmap/_version.py
+docs/assets/_data/
+
+.ruff_cache/
```

### Comparing `cmap-0.0.0rc0/LICENSE` & `cmap-0.0.1/LICENSE/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-BSD License
+BSD License for cmap package
 
 Copyright (c) 2022, Talley Lambert
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
```

