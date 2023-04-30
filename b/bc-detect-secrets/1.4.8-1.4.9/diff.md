# Comparing `tmp/bc-detect-secrets-1.4.8.tar.gz` & `tmp/bc-detect-secrets-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bc-detect-secrets-1.4.8.tar", last modified: Sun Jan  8 09:37:11 2023, max compression
+gzip compressed data, was "dist/bc-detect-secrets-1.4.9.tar", last modified: Mon Jan 16 12:11:03 2023, max compression
```

## Comparing `bc-detect-secrets-1.4.8.tar` & `bc-detect-secrets-1.4.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/
--rw-r--r--   0 root         (0) root         (0)       51 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    28675 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22360 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/
--rw-r--r--   0 root         (0) root         (0)    28675 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3142 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/
--rw-r--r--   0 root         (0) root         (0)       69 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/__main__.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-08 09:37:07.000000 bc-detect-secrets-1.4.8/detect_secrets/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/
--rw-r--r--   0 root         (0) root         (0)      212 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/analytics.py
--rw-r--r--   0 root         (0) root         (0)     3352 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/audit.py
--rw-r--r--   0 root         (0) root         (0)     6820 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/common.py
--rw-r--r--   0 root         (0) root         (0)     8777 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/compare.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/io.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/iterator.py
--rw-r--r--   0 root         (0) root         (0)     3018 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/audit/report.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4812 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/baseline.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/core/plugins/
--rw-r--r--   0 root         (0) root         (0)       82 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/plugins/initialize.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/plugins/util.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/potential_secret.py
--rw-r--r--   0 root         (0) root         (0)    14715 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/scan.py
--rw-r--r--   0 root         (0) root         (0)    11635 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/secrets_collection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/core/upgrades/
--rw-r--r--   0 root         (0) root         (0)      337 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/upgrades/__init__.py
--rw-r--r--   0 root         (0) root         (0)      334 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/upgrades/v0_12.py
--rw-r--r--   0 root         (0) root         (0)     4215 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/upgrades/v1_0.py
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/upgrades/v1_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/core/usage/
--rw-r--r--   0 root         (0) root         (0)     6446 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/usage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/usage/audit.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/usage/baseline.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/usage/common.py
--rw-r--r--   0 root         (0) root         (0)     8280 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/usage/filters.py
--rw-r--r--   0 root         (0) root         (0)     5294 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/usage/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/core/usage/scan.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/custom_types.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/
--rw-r--r--   0 root         (0) root         (0)      205 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3015 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/allowlist.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/gibberish/
--rw-r--r--   0 root         (0) root         (0)     3185 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/gibberish/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8602 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/gibberish/rfc.model
--rw-r--r--   0 root         (0) root         (0)     6537 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/heuristic.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/regex.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/util.py
--rw-r--r--   0 root         (0) root         (0)     2283 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/filters/wordlist.py
--rw-r--r--   0 root         (0) root         (0)     5167 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      484 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     5804 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/aws.py
--rw-r--r--   0 root         (0) root         (0)      423 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/azure_storage_key.py
--rw-r--r--   0 root         (0) root         (0)     8396 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/base.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     3885 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/cloudant.py
--rw-r--r--   0 root         (0) root         (0)      509 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/discord.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/github_token.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/high_entropy_strings.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/ibm_cloud_iam.py
--rw-r--r--   0 root         (0) root         (0)     5345 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/ibm_cos_hmac.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/jwt.py
--rw-r--r--   0 root         (0) root         (0)    12328 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/keyword.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/mailchimp.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/npm.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/private_key.py
--rw-r--r--   0 root         (0) root         (0)      457 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/sendgrid.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/slack.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/softlayer.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/square_oauth.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/stripe.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/plugins/twilio.py
--rw-r--r--   0 root         (0) root         (0)     4748 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/pre_commit_hook.py
--rw-r--r--   0 root         (0) root         (0)    10345 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/transformers/
--rw-r--r--   0 root         (0) root         (0)     1364 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/transformers/base.py
--rw-r--r--   0 root         (0) root         (0)     8689 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/transformers/config.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/transformers/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12209 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/transformers/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/detect_secrets/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/code_snippet.py
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/color.py
--rw-r--r--   0 root         (0) root         (0)     1348 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/filetype.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/git.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/importlib.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/inject.py
--rw-r--r--   0 root         (0) root         (0)      469 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/path.py
--rw-r--r--   0 root         (0) root         (0)     1388 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/detect_secrets/util/semver.py
--rw-r--r--   0 root         (0) root         (0)      476 2023-01-08 09:37:11.000000 bc-detect-secrets-1.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2126 2023-01-08 09:37:06.000000 bc-detect-secrets-1.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    28675 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    22360 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    28675 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-01-16 12:10:58.000000 bc-detect-secrets-1.4.9/detect_secrets/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/analytics.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/audit.py
+-rw-r--r--   0 root         (0) root         (0)     6820 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/common.py
+-rw-r--r--   0 root         (0) root         (0)     8777 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/compare.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/io.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/iterator.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/audit/report.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4812 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/baseline.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/core/plugins/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/plugins/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/plugins/util.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/potential_secret.py
+-rw-r--r--   0 root         (0) root         (0)    14715 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/scan.py
+-rw-r--r--   0 root         (0) root         (0)    11635 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/secrets_collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/core/upgrades/
+-rw-r--r--   0 root         (0) root         (0)      337 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/upgrades/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      334 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/upgrades/v0_12.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/upgrades/v1_0.py
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/upgrades/v1_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/core/usage/
+-rw-r--r--   0 root         (0) root         (0)     6446 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/usage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/usage/audit.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/usage/baseline.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/usage/common.py
+-rw-r--r--   0 root         (0) root         (0)     8280 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/usage/filters.py
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/usage/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/core/usage/scan.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/custom_types.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/
+-rw-r--r--   0 root         (0) root         (0)      205 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/allowlist.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/gibberish/
+-rw-r--r--   0 root         (0) root         (0)     3185 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/gibberish/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/gibberish/rfc.model
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/heuristic.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/regex.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/util.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/filters/wordlist.py
+-rw-r--r--   0 root         (0) root         (0)     5167 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      484 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     5804 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/aws.py
+-rw-r--r--   0 root         (0) root         (0)      423 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/azure_storage_key.py
+-rw-r--r--   0 root         (0) root         (0)     8396 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/base.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/cloudant.py
+-rw-r--r--   0 root         (0) root         (0)      509 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/discord.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/github_token.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/high_entropy_strings.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/ibm_cloud_iam.py
+-rw-r--r--   0 root         (0) root         (0)     5345 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/ibm_cos_hmac.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/jwt.py
+-rw-r--r--   0 root         (0) root         (0)    12341 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/mailchimp.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/npm.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/private_key.py
+-rw-r--r--   0 root         (0) root         (0)      457 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/sendgrid.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/slack.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/softlayer.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/square_oauth.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/stripe.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/plugins/twilio.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/pre_commit_hook.py
+-rw-r--r--   0 root         (0) root         (0)    10345 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/transformers/
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/transformers/base.py
+-rw-r--r--   0 root         (0) root         (0)     8689 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/transformers/config.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/transformers/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12209 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/transformers/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/detect_secrets/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/code_snippet.py
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/color.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/filetype.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/git.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/importlib.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/inject.py
+-rw-r--r--   0 root         (0) root         (0)      469 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/detect_secrets/util/semver.py
+-rw-r--r--   0 root         (0) root         (0)      476 2023-01-16 12:11:03.000000 bc-detect-secrets-1.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-01-16 12:10:57.000000 bc-detect-secrets-1.4.9/setup.py
```

### Comparing `bc-detect-secrets-1.4.8/PKG-INFO` & `bc-detect-secrets-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc-detect-secrets
-Version: 1.4.8
+Version: 1.4.9
 Summary: Tool for detecting secrets in the codebase
 Home-page: https://github.com/bridgecrewio/detect-secrets
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Description: [![Build Status](https://github.com/bridgecrewio/detect-secrets/actions/workflows/release.yml/badge.svg)](https://github.com/bridgecrewio/detect-secrets/actions/workflows/release.yml?query=branch%3Amaster++)
         [![PyPI version](https://badge.fury.io/py/bc-detect-secrets.svg)](https://badge.fury.io/py/bc-detect-secrets)
```

### Comparing `bc-detect-secrets-1.4.8/README.md` & `bc-detect-secrets-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/PKG-INFO` & `bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc-detect-secrets
-Version: 1.4.8
+Version: 1.4.9
 Summary: Tool for detecting secrets in the codebase
 Home-page: https://github.com/bridgecrewio/detect-secrets
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Description: [![Build Status](https://github.com/bridgecrewio/detect-secrets/actions/workflows/release.yml/badge.svg)](https://github.com/bridgecrewio/detect-secrets/actions/workflows/release.yml?query=branch%3Amaster++)
         [![PyPI version](https://badge.fury.io/py/bc-detect-secrets.svg)](https://badge.fury.io/py/bc-detect-secrets)
```

### Comparing `bc-detect-secrets-1.4.8/bc_detect_secrets.egg-info/SOURCES.txt` & `bc-detect-secrets-1.4.9/bc_detect_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/audit/analytics.py` & `bc-detect-secrets-1.4.9/detect_secrets/audit/analytics.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/audit/audit.py` & `bc-detect-secrets-1.4.9/detect_secrets/audit/audit.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/audit/common.py` & `bc-detect-secrets-1.4.9/detect_secrets/audit/common.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/audit/compare.py` & `bc-detect-secrets-1.4.9/detect_secrets/audit/compare.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/audit/io.py` & `bc-detect-secrets-1.4.9/detect_secrets/audit/io.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/audit/iterator.py` & `bc-detect-secrets-1.4.9/detect_secrets/audit/iterator.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/audit/report.py` & `bc-detect-secrets-1.4.9/detect_secrets/audit/report.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/constants.py` & `bc-detect-secrets-1.4.9/detect_secrets/constants.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/baseline.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/baseline.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/log.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/log.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/plugins/initialize.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/plugins/initialize.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/plugins/util.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/plugins/util.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/potential_secret.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/potential_secret.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/scan.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/scan.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/secrets_collection.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/secrets_collection.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/upgrades/v1_0.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/upgrades/v1_0.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/upgrades/v1_1.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/upgrades/v1_1.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/usage/__init__.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/usage/audit.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/usage/audit.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/usage/baseline.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/usage/baseline.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/usage/common.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/usage/common.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/usage/filters.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/usage/filters.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/usage/plugins.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/usage/plugins.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/core/usage/scan.py` & `bc-detect-secrets-1.4.9/detect_secrets/core/usage/scan.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/custom_types.py` & `bc-detect-secrets-1.4.9/detect_secrets/custom_types.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/exceptions.py` & `bc-detect-secrets-1.4.9/detect_secrets/exceptions.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/filters/allowlist.py` & `bc-detect-secrets-1.4.9/detect_secrets/filters/allowlist.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/filters/common.py` & `bc-detect-secrets-1.4.9/detect_secrets/filters/common.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/filters/gibberish/__init__.py` & `bc-detect-secrets-1.4.9/detect_secrets/filters/gibberish/__init__.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/filters/gibberish/rfc.model` & `bc-detect-secrets-1.4.9/detect_secrets/filters/gibberish/rfc.model`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/filters/heuristic.py` & `bc-detect-secrets-1.4.9/detect_secrets/filters/heuristic.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/filters/regex.py` & `bc-detect-secrets-1.4.9/detect_secrets/filters/regex.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/filters/util.py` & `bc-detect-secrets-1.4.9/detect_secrets/filters/util.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/filters/wordlist.py` & `bc-detect-secrets-1.4.9/detect_secrets/filters/wordlist.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/main.py` & `bc-detect-secrets-1.4.9/detect_secrets/main.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/aws.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/aws.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/base.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/base.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/basic_auth.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/basic_auth.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/cloudant.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/cloudant.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/high_entropy_strings.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/high_entropy_strings.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/ibm_cloud_iam.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/ibm_cloud_iam.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/ibm_cos_hmac.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/ibm_cos_hmac.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/jwt.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/jwt.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/keyword.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/keyword.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     'private_?key',
     'client_?key',
     'db_?pass',
     'database_?pass',
     'key_?pass',
     'password',
     'passwd',
+    'token',
     '_pass\\b',
     'pwd',
     'secret',
     'contraseña',
     'contrasena',
 )
 # Includes ], ', " as closing
```

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/mailchimp.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/mailchimp.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/private_key.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/private_key.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/slack.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/slack.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/softlayer.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/softlayer.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/plugins/stripe.py` & `bc-detect-secrets-1.4.9/detect_secrets/plugins/stripe.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/pre_commit_hook.py` & `bc-detect-secrets-1.4.9/detect_secrets/pre_commit_hook.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/settings.py` & `bc-detect-secrets-1.4.9/detect_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/transformers/__init__.py` & `bc-detect-secrets-1.4.9/detect_secrets/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/transformers/base.py` & `bc-detect-secrets-1.4.9/detect_secrets/transformers/base.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/transformers/config.py` & `bc-detect-secrets-1.4.9/detect_secrets/transformers/config.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/transformers/yaml.py` & `bc-detect-secrets-1.4.9/detect_secrets/transformers/yaml.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/util/code_snippet.py` & `bc-detect-secrets-1.4.9/detect_secrets/util/code_snippet.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/util/color.py` & `bc-detect-secrets-1.4.9/detect_secrets/util/color.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/util/filetype.py` & `bc-detect-secrets-1.4.9/detect_secrets/util/filetype.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/util/git.py` & `bc-detect-secrets-1.4.9/detect_secrets/util/git.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/util/importlib.py` & `bc-detect-secrets-1.4.9/detect_secrets/util/importlib.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/util/inject.py` & `bc-detect-secrets-1.4.9/detect_secrets/util/inject.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/detect_secrets/util/semver.py` & `bc-detect-secrets-1.4.9/detect_secrets/util/semver.py`

 * *Files identical despite different names*

### Comparing `bc-detect-secrets-1.4.8/setup.py` & `bc-detect-secrets-1.4.9/setup.py`

 * *Files identical despite different names*

