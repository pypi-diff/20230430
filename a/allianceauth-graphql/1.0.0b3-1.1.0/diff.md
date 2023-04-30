# Comparing `tmp/allianceauth_graphql-1.0.0b3.tar.gz` & `tmp/allianceauth_graphql-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth_graphql-1.0.0b3.tar", last modified: Sat Mar 11 15:38:16 2023, max compression
+gzip compressed data, was "allianceauth_graphql-1.1.0.tar", last modified: Sun Apr 30 08:50:44 2023, max compression
```

## Comparing `allianceauth_graphql-1.0.0b3.tar` & `allianceauth_graphql-1.1.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.267184 allianceauth_graphql-1.0.0b3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-11 15:38:16.267184 allianceauth_graphql-1.0.0b3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4821 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.259184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/
--rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.259184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/analytics/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/analytics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/analytics/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/analytics/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      171 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.259184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/forms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9380 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1123 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      770 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.259184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/inputs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7099 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3894 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1874 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/corputils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/corputils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/corputils/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1548 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/corputils/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1713 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/corputils/types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/esi/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/esi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/esi/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/esi/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/esi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/eveonline/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/eveonline/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/eveonline/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/eveonline/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/eveonline/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/fleetactivitytracking/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/fleetactivitytracking/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6342 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/fleetactivitytracking/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4824 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/fleetactivitytracking/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/fleetactivitytracking/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/groupmanagement/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/groupmanagement/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17390 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/groupmanagement/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6361 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/groupmanagement/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2962 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/groupmanagement/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/inputs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6335 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3771 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1794 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/migrations/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/migrations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.263184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/notifications/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/notifications/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1885 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/notifications/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/notifications/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/notifications/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.267184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/optimer/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/optimer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/optimer/forms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3420 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/optimer/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/optimer/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/optimer/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.267184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/permissions_tool/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/permissions_tool/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/permissions_tool/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2111 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/permissions_tool/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/permissions_tool/types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1354 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.267184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/srp/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/srp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/srp/forms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10585 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/srp/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/srp/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      406 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/srp/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.267184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    25476 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_community_creation_allianceauth_pve.py
--rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_corputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_esi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_eveonline.py
--rw-r--r--   0 runner    (1001) docker     (123)    26501 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_fleetactivitytracking.py
--rw-r--r--   0 runner    (1001) docker     (123)    50507 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_groupmanagement.py
--rw-r--r--   0 runner    (1001) docker     (123)    28862 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_hrapplications.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_optimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_permission_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_srp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_timerboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.267184 allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      771 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/inputs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3554 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/mutations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/queries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 15:38:16.259184 allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-11 15:38:16.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-03-11 15:38:16.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 15:38:16.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 15:38:16.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-11 15:38:16.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-11 15:38:16.000000 allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-03-11 15:38:05.000000 allianceauth_graphql-1.0.0b3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1688 2023-03-11 15:38:16.271184 allianceauth_graphql-1.0.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.499049 allianceauth_graphql-1.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-30 08:50:44.503049 allianceauth_graphql-1.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4807 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.479049 allianceauth_graphql-1.1.0/allianceauth_graphql/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.483049 allianceauth_graphql-1.1.0/allianceauth_graphql/analytics/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/analytics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/analytics/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/analytics/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      171 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.483049 allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9380 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      770 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.483049 allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.487049 allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/inputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7099 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3894 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1874 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.487049 allianceauth_graphql-1.1.0/allianceauth_graphql/corputils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/corputils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/corputils/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1548 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/corputils/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1713 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/corputils/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.487049 allianceauth_graphql-1.1.0/allianceauth_graphql/esi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/esi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/esi/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/esi/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/esi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.487049 allianceauth_graphql-1.1.0/allianceauth_graphql/eveonline/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/eveonline/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/eveonline/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/eveonline/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/eveonline/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.487049 allianceauth_graphql-1.1.0/allianceauth_graphql/fleetactivitytracking/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/fleetactivitytracking/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6342 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/fleetactivitytracking/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4824 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/fleetactivitytracking/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/fleetactivitytracking/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.487049 allianceauth_graphql-1.1.0/allianceauth_graphql/groupmanagement/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/groupmanagement/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17390 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/groupmanagement/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6361 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/groupmanagement/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2962 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/groupmanagement/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.491049 allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/inputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6335 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3771 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1794 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.491049 allianceauth_graphql-1.1.0/allianceauth_graphql/migrations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/migrations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.491049 allianceauth_graphql-1.1.0/allianceauth_graphql/notifications/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/notifications/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1885 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/notifications/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/notifications/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/notifications/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.491049 allianceauth_graphql-1.1.0/allianceauth_graphql/optimer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/optimer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/optimer/forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3420 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/optimer/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/optimer/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/optimer/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.495049 allianceauth_graphql-1.1.0/allianceauth_graphql/permissions_tool/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/permissions_tool/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/permissions_tool/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2111 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/permissions_tool/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/permissions_tool/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1354 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.495049 allianceauth_graphql-1.1.0/allianceauth_graphql/srp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/srp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/srp/forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10585 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/srp/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/srp/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      406 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/srp/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.499049 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28898 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25476 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_community_creation_allianceauth_pve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_corputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_esi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_eveonline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26501 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_fleetactivitytracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50507 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_groupmanagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28862 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_hrapplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_optimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_permission_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_srp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_timerboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.499049 allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      771 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/inputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3554 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/mutations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/allianceauth_graphql/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:50:44.479049 allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-30 08:50:44.000000 allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-30 08:50:44.000000 allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:50:44.000000 allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:50:44.000000 allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-30 08:50:44.000000 allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 08:50:44.000000 allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-30 08:50:25.000000 allianceauth_graphql-1.1.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-04-30 08:50:44.503049 allianceauth_graphql-1.1.0/setup.cfg
```

### Comparing `allianceauth_graphql-1.0.0b3/LICENSE` & `allianceauth_graphql-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/PKG-INFO` & `allianceauth_graphql-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth_graphql
-Version: 1.0.0b3
+Version: 1.1.0
 Summary: GraphQL integration for AllianceAuth
 Home-page: https://github.com/Maestro-Zacht/allianceauth-graphql
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_graphql,GraphQL,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -130,15 +130,15 @@
 7. Restart AllianceAuth.
 
 
 Community Creations Integration
 -------------------------------
 
 Currently the package supports the integration with the following community packages:
-* allianceauth-pve: v1.8.x v1.9.x v1.10.x
+* allianceauth-pve: v1.11.x
 
 Be sure to check if you have the right versions of these package or the GraphQL will not have the same behaviour as the apps.
 
 
 Settings
 --------
```

### Comparing `allianceauth_graphql-1.0.0b3/README.md` & `allianceauth_graphql-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 7. Restart AllianceAuth.
 
 
 Community Creations Integration
 -------------------------------
 
 Currently the package supports the integration with the following community packages:
-* allianceauth-pve: v1.8.x v1.9.x v1.10.x
+* allianceauth-pve: v1.11.x
 
 Be sure to check if you have the right versions of these package or the GraphQL will not have the same behaviour as the apps.
 
 
 Settings
 --------
```

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 
 
 class UserProfileType(DjangoObjectType):
     state = graphene.Field(StateType, required=True)
 
     class Meta:
         model = UserProfile
+        fields = ('id', 'user', 'main_character', 'state', )
 
 
 class UserType(DjangoObjectType):
     class Meta:
         model = User
-        fields = ('id', 'username', 'profile', 'character_ownerships',)
+        fields = ('id', 'username', 'profile',)
 
 
 class GroupStatusEnum(graphene.Enum):
     JOINED = 1
     PENDING = 2
     CAN_JOIN = 3
     CAN_APPLY = 4
```

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/authentication/views.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/authentication/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/inputs.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/inputs.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/community_creations/allianceauth_pve_integration/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/community_creations/allianceauth_pve_integration/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/corputils/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/corputils/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/corputils/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/corputils/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/corputils/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/corputils/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/decorators.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/esi/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/esi/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/eveonline/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/eveonline/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/fleetactivitytracking/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/fleetactivitytracking/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/fleetactivitytracking/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/fleetactivitytracking/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/fleetactivitytracking/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/fleetactivitytracking/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/groupmanagement/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/groupmanagement/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/groupmanagement/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/groupmanagement/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/groupmanagement/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/groupmanagement/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/hrapplications/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/hrapplications/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/notifications/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/notifications/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/optimer/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/optimer/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/optimer/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/optimer/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/permissions_tool/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/permissions_tool/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/permissions_tool/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/permissions_tool/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/schema.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/srp/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/srp/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/srp/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/srp/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_authentication.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -570,19 +570,14 @@
             '''
             mutation testM($input: String!) {
                 authenticationAddCharacter(newCharSsoToken: $input) {
                     errors
                     ok
                     me {
                         id
-                        characterOwnerships {
-                            character {
-                                id
-                            }
-                        }
                     }
                 }
             }
             ''',
             operation_name='testM',
             input_data='nice_token'
         )
@@ -592,27 +587,22 @@
             {
                 'data': {
                     'authenticationAddCharacter': {
                         'errors': [],
                         'ok': True,
                         'me': {
                             'id': str(self.user.pk),
-                            'characterOwnerships': [
-                                {
-                                    'character': {
-                                        'id': str(self.newchar.pk)
-                                    }
-                                }
-                            ]
                         }
                     }
                 }
             }
         )
-    
+
+        self.assertEqual(self.user.character_ownerships.count(), 1)
+        self.assertEqual(self.user.character_ownerships.first().character, self.newchar)
 
 
 class TestRefreshEsiTokenMutation(GraphQLTestCase):
 
     @classmethod
     def setUpTestData(cls):
         cls.user = UserFactory()
```

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_community_creation_allianceauth_pve.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_community_creation_allianceauth_pve.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_corputils.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_corputils.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_esi.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_esi.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_eveonline.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_eveonline.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_fleetactivitytracking.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_fleetactivitytracking.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_groupmanagement.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_groupmanagement.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_hrapplications.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_hrapplications.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_notifications.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_optimer.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_optimer.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_permission_tool.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_permission_tool.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_srp.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_srp.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/tests/test_timerboard.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/tests/test_timerboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/inputs.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/inputs.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/mutations.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/mutations.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/queries.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/queries.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql/timerboard/types.py` & `allianceauth_graphql-1.1.0/allianceauth_graphql/timerboard/types.py`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/PKG-INFO` & `allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-graphql
-Version: 1.0.0b3
+Version: 1.1.0
 Summary: GraphQL integration for AllianceAuth
 Home-page: https://github.com/Maestro-Zacht/allianceauth-graphql
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_graphql,GraphQL,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -130,15 +130,15 @@
 7. Restart AllianceAuth.
 
 
 Community Creations Integration
 -------------------------------
 
 Currently the package supports the integration with the following community packages:
-* allianceauth-pve: v1.8.x v1.9.x v1.10.x
+* allianceauth-pve: v1.11.x
 
 Be sure to check if you have the right versions of these package or the GraphQL will not have the same behaviour as the apps.
 
 
 Settings
 --------
```

### Comparing `allianceauth_graphql-1.0.0b3/allianceauth_graphql.egg-info/SOURCES.txt` & `allianceauth_graphql-1.1.0/allianceauth_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allianceauth_graphql-1.0.0b3/setup.cfg` & `allianceauth_graphql-1.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.0b3
+current_version = 1.1.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
@@ -43,15 +43,15 @@
 	eveonline
 url = https://github.com/Maestro-Zacht/allianceauth-graphql
 
 [options]
 packages = find:
 python_requires = ~=3.8
 install_requires = 
-	allianceauth~=3.3.0
+	allianceauth~=3.4.0
 	graphene-django~=3.0.0
 	django-graphql-jwt~=0.3.0
 	allianceauth-app-utils~=1.15
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
```

