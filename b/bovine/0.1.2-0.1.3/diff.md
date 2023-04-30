# Comparing `tmp/bovine-0.1.2.tar.gz` & `tmp/bovine-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.1.2.tar", max compression
+gzip compressed data, was "bovine-0.1.3.tar", max compression
```

## Comparing `bovine-0.1.2.tar` & `bovine-0.1.3.tar`

### file list

```diff
@@ -1,104 +1,107 @@
--rw-r--r--   0        0        0     1364 2023-04-20 10:27:12.601485 bovine-0.1.2/README.md
--rw-r--r--   0        0        0     8584 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 10:27:12.733486 bovine-0.1.2/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0      173 2023-04-20 10:27:49.365802 bovine-0.1.2/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3092 2023-04-20 10:27:49.365802 bovine-0.1.2/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
--rw-r--r--   0        0        0     2477 2023-04-20 10:27:49.785805 bovine-0.1.2/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
--rw-r--r--   0        0        0      906 2023-04-20 10:27:49.893806 bovine-0.1.2/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
--rw-r--r--   0        0        0     3638 2023-04-20 10:27:49.901806 bovine-0.1.2/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2736 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitypub/authorization_wrapper.py
--rw-r--r--   0        0        0     2219 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      429 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0     2757 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0     4682 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     4268 2023-04-20 10:27:49.885806 bovine-0.1.2/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4249 2023-04-20 10:27:49.885806 bovine-0.1.2/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4086 2023-04-20 10:27:49.889806 bovine-0.1.2/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4560 2023-04-20 10:27:50.065808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3305 2023-04-20 10:27:50.073808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3168 2023-04-20 10:27:50.077808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1929 2023-04-20 10:27:50.081808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1368 2023-04-20 10:27:50.085808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     4195 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     4240 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0     2163 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1418 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0     1381 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1010 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      809 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_ordered_collection_page.py
--rw-r--r--   0        0        0     2354 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0     2836 2023-04-20 10:27:49.889806 bovine-0.1.2/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      908 2023-04-20 10:27:49.893806 bovine-0.1.2/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
--rw-r--r--   0        0        0     4763 2023-04-20 10:27:50.093808 bovine-0.1.2/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      787 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     2081 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/__init__.py
--rw-r--r--   0        0        0     2209 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      268 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/consts.cpython-310.pyc
--rw-r--r--   0        0        0     1472 2023-04-20 10:27:49.781805 bovine-0.1.2/bovine/clients/__pycache__/event_source.cpython-310.pyc
--rw-r--r--   0        0        0     1014 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
--rw-r--r--   0        0        0     2508 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc
--rw-r--r--   0        0        0     1237 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
--rw-r--r--   0        0        0     2471 2023-04-20 10:27:49.781805 bovine-0.1.2/bovine/clients/__pycache__/signed_http.cpython-310.pyc
--rw-r--r--   0        0        0     1471 2023-04-20 10:27:49.781805 bovine-0.1.2/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc
--rw-r--r--   0        0        0     1352 2023-04-20 10:27:50.101808 bovine-0.1.2/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1576 2023-04-20 10:27:50.101808 bovine-0.1.2/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1217 2023-04-20 10:27:50.105808 bovine-0.1.2/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2094 2023-04-20 10:27:50.109808 bovine-0.1.2/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      821 2023-04-20 10:27:50.109808 bovine-0.1.2/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0       91 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/consts.py
--rw-r--r--   0        0        0     1106 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/event_source.py
--rw-r--r--   0        0        0      787 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3176 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/moo_auth_client.py
--rw-r--r--   0        0        0      948 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     3278 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     1074 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/signed_http_client.py
--rw-r--r--   0        0        0      609 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0      624 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      319 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1145 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      529 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     3999 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     3634 2023-04-20 10:27:49.609804 bovine-0.1.2/bovine/crypto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2863 2023-04-20 10:27:49.741805 bovine-0.1.2/bovine/crypto/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     2909 2023-04-20 10:27:49.741805 bovine-0.1.2/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
--rw-r--r--   0        0        0     2257 2023-04-20 10:27:49.741805 bovine-0.1.2/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2023-04-20 10:27:49.781805 bovine-0.1.2/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
--rw-r--r--   0        0        0     2363 2023-04-20 10:27:50.053808 bovine-0.1.2/bovine/crypto/__pycache__/test.cpython-310.pyc
--rw-r--r--   0        0        0     5810 2023-04-20 10:27:50.125808 bovine-0.1.2/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2742 2023-04-20 10:27:50.133808 bovine-0.1.2/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     7454 2023-04-20 10:27:50.145808 bovine-0.1.2/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2674 2023-04-20 10:27:50.153808 bovine-0.1.2/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2664 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test.py
--rw-r--r--   0        0        0     4989 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      302 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/ed25519_key.py
--rw-r--r--   0        0        0      864 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/msg.py
--rw-r--r--   0        0        0      178 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/test_bovine_client.py
--rw-r--r--   0        0        0      282 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/test_types.py
--rw-r--r--   0        0        0     2397 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/types.py
--rw-r--r--   0        0        0      667 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/__init__.py
--rw-r--r--   0        0        0      848 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      877 2023-04-20 10:27:49.741805 bovine-0.1.2/bovine/utils/__pycache__/date.cpython-310.pyc
--rw-r--r--   0        0        0     3443 2023-04-20 10:27:50.161809 bovine-0.1.2/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1662 2023-04-20 10:27:50.165809 bovine-0.1.2/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      973 2023-04-20 10:27:50.165809 bovine-0.1.2/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      519 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/date.py
--rw-r--r--   0        0        0     1159 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/msg/__init__.py
--rw-r--r--   0        0        0     1722 2023-04-20 10:27:50.169809 bovine-0.1.2/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1922 2023-04-20 10:27:50.173809 bovine-0.1.2/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      622 2023-04-20 10:27:50.169809 bovine-0.1.2/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0        0        0      557 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/msg/test_validation.py
--rw-r--r--   0        0        0      243 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/msg/validation.py
--rw-r--r--   0        0        0      181 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/test.py
--rw-r--r--   0        0        0      737 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/test_date.py
--rw-r--r--   0        0        0      452 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      191 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0     1211 2023-04-20 10:27:12.605485 bovine-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 bovine-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1364 2023-04-30 17:02:34.666958 bovine-0.1.3/README.md
+-rw-r--r--   0        0        0     9265 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 17:02:34.802960 bovine-0.1.3/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-30 17:03:24.323409 bovine-0.1.3/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3612 2023-04-30 17:03:24.323409 bovine-0.1.3/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     2819 2023-04-30 17:03:24.767413 bovine-0.1.3/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
+-rw-r--r--   0        0        0      922 2023-04-30 17:03:24.883414 bovine-0.1.3/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
+-rw-r--r--   0        0        0     3638 2023-04-30 17:03:24.895414 bovine-0.1.3/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1212 2023-04-30 17:03:25.031416 bovine-0.1.3/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3339 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/authorization_wrapper.py
+-rw-r--r--   0        0        0     2837 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      434 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0     2757 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0      498 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitypub/test_collection_helper.py
+-rw-r--r--   0        0        0     4957 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4645 2023-04-30 17:03:24.875414 bovine-0.1.3/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4269 2023-04-30 17:03:24.879414 bovine-0.1.3/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4086 2023-04-30 17:03:24.879414 bovine-0.1.3/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4584 2023-04-30 17:03:25.039415 bovine-0.1.3/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3327 2023-04-30 17:03:25.047416 bovine-0.1.3/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3188 2023-04-30 17:03:25.051416 bovine-0.1.3/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1951 2023-04-30 17:03:25.055416 bovine-0.1.3/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1386 2023-04-30 17:03:25.059416 bovine-0.1.3/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     4203 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     4240 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2195 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1442 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0     1397 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1034 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      817 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0     2836 2023-04-30 17:03:24.879414 bovine-0.1.3/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2023-04-30 17:03:24.883414 bovine-0.1.3/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
+-rw-r--r--   0        0        0     4763 2023-04-30 17:03:25.071416 bovine-0.1.3/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      787 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     2722 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     2854 2023-04-30 17:03:24.575411 bovine-0.1.3/bovine/clients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/clients/__pycache__/bearer.cpython-310.pyc
+-rw-r--r--   0        0        0      268 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/clients/__pycache__/consts.cpython-310.pyc
+-rw-r--r--   0        0        0     1719 2023-04-30 17:03:24.619412 bovine-0.1.3/bovine/clients/__pycache__/event_source.cpython-310.pyc
+-rw-r--r--   0        0        0     1014 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
+-rw-r--r--   0        0        0     2534 2023-04-30 17:03:24.619412 bovine-0.1.3/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
+-rw-r--r--   0        0        0     1237 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
+-rw-r--r--   0        0        0     1529 2023-04-30 17:03:24.767413 bovine-0.1.3/bovine/clients/__pycache__/signed_http.cpython-310.pyc
+-rw-r--r--   0        0        0     2479 2023-04-30 17:03:24.767413 bovine-0.1.3/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
+-rw-r--r--   0        0        0     1352 2023-04-30 17:03:25.075416 bovine-0.1.3/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2648 2023-04-30 17:03:25.079416 bovine-0.1.3/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1217 2023-04-30 17:03:25.083416 bovine-0.1.3/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2102 2023-04-30 17:03:25.083416 bovine-0.1.3/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      814 2023-04-30 17:03:25.087416 bovine-0.1.3/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1794 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/bearer.py
+-rw-r--r--   0        0        0       91 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1520 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      787 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3001 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/moo_auth.py
+-rw-r--r--   0        0        0      948 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     1150 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     3278 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/signed_http_methods.py
+-rw-r--r--   0        0        0      609 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0     1149 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1153 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      522 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     4141 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     3749 2023-04-30 17:03:24.623412 bovine-0.1.3/bovine/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2863 2023-04-30 17:03:24.763413 bovine-0.1.3/bovine/crypto/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     2909 2023-04-30 17:03:24.763413 bovine-0.1.3/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
+-rw-r--r--   0        0        0     2257 2023-04-30 17:03:24.763413 bovine-0.1.3/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-04-30 17:03:24.767413 bovine-0.1.3/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2363 2023-04-30 17:03:25.027415 bovine-0.1.3/bovine/crypto/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5821 2023-04-30 17:03:25.095416 bovine-0.1.3/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2742 2023-04-30 17:03:25.099416 bovine-0.1.3/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     7454 2023-04-30 17:03:25.107416 bovine-0.1.3/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2674 2023-04-30 17:03:25.115416 bovine-0.1.3/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2664 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4995 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      302 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/ed25519_key.py
+-rw-r--r--   0        0        0      864 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/msg.py
+-rw-r--r--   0        0        0      178 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0      282 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/types.py
+-rw-r--r--   0        0        0      667 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-30 17:03:24.575411 bovine-0.1.3/bovine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      877 2023-04-30 17:03:24.579411 bovine-0.1.3/bovine/utils/__pycache__/date.cpython-310.pyc
+-rw-r--r--   0        0        0     3465 2023-04-30 17:03:25.123416 bovine-0.1.3/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1662 2023-04-30 17:03:25.127416 bovine-0.1.3/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      973 2023-04-30 17:03:25.131416 bovine-0.1.3/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      519 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/date.py
+-rw-r--r--   0        0        0     1210 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/msg/__init__.py
+-rw-r--r--   0        0        0     1795 2023-04-30 17:03:25.131416 bovine-0.1.3/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1967 2023-04-30 17:03:25.135416 bovine-0.1.3/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      659 2023-04-30 17:03:25.135416 bovine-0.1.3/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0        0        0      599 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/msg/test_validation.py
+-rw-r--r--   0        0        0      261 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/msg/validation.py
+-rw-r--r--   0        0        0      761 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      191 2023-04-30 17:02:34.666958 bovine-0.1.3/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1229 2023-04-30 17:02:34.670958 bovine-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 bovine-0.1.3/PKG-INFO
```

### Comparing `bovine-0.1.2/README.md` & `bovine-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/__init__.py` & `bovine-0.1.3/bovine/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import logging
 from typing import Optional
 from urllib.parse import urlparse
 
 import tomli
 
 from .activitypub.authorization_wrapper import AuthorizationWrapper
-from .activitypub.collection_helper import CollectionHelper
+from .activitypub.collection_helper import CollectionHelper, all_collection_elements
+from .activitystreams import Collection
 from .activitystreams.activity_factory import ActivityFactory
 from .activitystreams.object_factory import ObjectFactory
 
 logger = logging.getLogger(__name__)
 
 
 class BovineClient(AuthorizationWrapper):
@@ -33,16 +34,18 @@
         await actor.init()
         await do_something(actor)
 
     I still call the variable actor as it represents the ActivityPub Actor through
     a client.
 
     :param config:
-        Configuration with keys "host" and "private_key" -> Moo-Auth-1;
-        with keys "account_url", "public_key_url", and "private_key" -> HTTP Signatures
+
+        * Moo-Auth-1: keys "host" and "private_key"
+        * HTTP Signatures: keys "account_url", "public_key_url", and "private_key"
+        * Bearer Authorization: keys "account_url", "access_token"
 
     """
 
     def __init__(self, config):
         super().__init__()
 
         self.actor_id = None
@@ -114,14 +117,25 @@
         The syntax for this will probably change"""
         if self.information is None:
             await self.load()
 
         event_source_url = self.information["endpoints"]["eventSource"]
         return self.client.event_source(event_source_url)
 
+    async def simplify_collection(self, collection):
+        """Returns a Collection containing all items from the passed collection
+        or collection id"""
+        items = await all_collection_elements(self, collection)
+
+        if isinstance(collection, str):
+            collection_id = collection
+        else:
+            collection_id = collection.get("id")
+        return Collection(id=collection_id, items=items).build()
+
     @property
     def activity_factory(self):
         """Returns an ActivityFactory for objects corresponding to the client's actor"""
         if self._activity_factory is None:
             self._activity_factory = ActivityFactory(self.information)
         return self._activity_factory
 
@@ -137,14 +151,19 @@
         return self.activity_factory, self.object_factory
 
     @property
     def host(self):
         """The host the actor is on"""
         return urlparse(self.actor_id).netloc
 
+    @property
+    def followers(self) -> str:
+        """The id of the follows collection"""
+        return self.information["followers"]
+
     async def inbox(self):
         """Provides a CollectionHelper for the Actors inbox"""
         inbox_collection = CollectionHelper(self.information["inbox"], self)
         await inbox_collection.refresh()
         return inbox_collection
 
     async def outbox(self):
```

### Comparing `bovine-0.1.2/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc` & `bovine-0.1.3/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2736 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,226 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 b00a 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0b0d 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
+00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6406 6c0a 6d0b 5a0b 0100 6500 a00c 650d  d.l.m.Z...e...e.
-00000080: a101 5a0e 4700 6407 6408 8400 6408 8302  ..Z.G.d.d...d...
-00000090: 5a0f 6401 5300 2909 e900 0000 004e 2901  Z.d.S.)......N).
-000000a0: da08 4f70 7469 6f6e 616c 2901 da19 6c6f  ..Optional)...lo
-000000b0: 6f6b 7570 5f64 6964 5f77 6974 685f 7765  okup_did_with_we
-000000c0: 6266 696e 6765 7229 01da 0d4d 6f6f 4175  bfinger)...MooAu
-000000d0: 7468 436c 6965 6e74 2901 da10 5369 676e  thClient)...Sign
-000000e0: 6564 4874 7470 436c 6965 6e74 2901 da16  edHttpClient)...
-000000f0: 7072 6976 6174 655f 6b65 795f 746f 5f64  private_key_to_d
-00000100: 6964 5f6b 6579 6300 0000 0000 0000 0000  id_keyc.........
-00000110: 0000 0000 0000 0008 0000 0040 0000 0073  ...........@...s
-00000120: a600 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
-00000130: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
-00000140: 8400 5a05 641c 6408 6506 6507 6a08 1900  ..Z.d.d.e.e.j...
-00000150: 6602 6409 640a 8405 5a09 0907 641c 640b  f.d.d...Z...d.d.
-00000160: 650a 640c 650a 6408 6506 6507 6a08 1900  e.d.e.d.e.e.j...
-00000170: 6606 640d 640e 8405 5a0b 640f 650a 6602  f.d.d...Z.d.e.f.
-00000180: 6410 6411 8404 5a0c 0907 641c 6412 650a  d.d...Z...d.d.e.
-00000190: 640c 650a 6408 6506 6507 6a08 1900 6606  d.e.d.e.e.j...f.
-000001a0: 6413 6414 8405 5a0d 6415 6416 8400 5a0e  d.d...Z.d.d...Z.
-000001b0: 6417 6418 8400 5a0f 6419 6510 6602 641a  d.d...Z.d.e.f.d.
-000001c0: 641b 8404 5a11 6407 5300 291d da14 4175  d...Z.d.S.)...Au
-000001d0: 7468 6f72 697a 6174 696f 6e57 7261 7070  thorizationWrapp
-000001e0: 6572 6301 0000 0000 0000 0000 0000 0001  erc.............
-000001f0: 0000 0002 0000 0043 0000 0073 1c00 0000  .......C...s....
-00000200: 6400 7c00 5f00 6400 7c00 5f01 6400 7c00  d.|._.d.|._.d.|.
-00000210: 5f02 6400 7c00 5f03 6400 5300 a901 4e29  _.d.|._.d.S...N)
-00000220: 04da 0663 6f6e 6669 67da 0861 6374 6f72  ...config..actor
-00000230: 5f69 64da 0663 6c69 656e 74da 0773 6573  _id..client..ses
-00000240: 7369 6f6e a901 da04 7365 6c66 a900 720f  sion....self..r.
-00000250: 0000 00fa 5d2f 776f 6f64 7065 636b 6572  ....]/woodpecker
-00000260: 2f73 7263 2f63 6f64 6562 6572 672e 6f72  /src/codeberg.or
-00000270: 672f 626f 7669 6e65 2f62 6f76 696e 652f  g/bovine/bovine/
-00000280: 626f 7669 6e65 2f62 6f76 696e 652f 6163  bovine/bovine/ac
-00000290: 7469 7669 7479 7075 622f 6175 7468 6f72  tivitypub/author
-000002a0: 697a 6174 696f 6e5f 7772 6170 7065 722e  ization_wrapper.
-000002b0: 7079 da08 5f5f 696e 6974 5f5f 0f00 0000  py..__init__....
-000002c0: 7308 0000 0006 0106 0106 010a 017a 1d41  s............z.A
-000002d0: 7574 686f 7269 7a61 7469 6f6e 5772 6170  uthorizationWrap
-000002e0: 7065 722e 5f5f 696e 6974 5f5f 6301 0000  per.__init__c...
-000002f0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000300: 00c3 0000 0073 1400 0000 8101 7c00 a000  .....s......|...
-00000310: a100 4900 6400 4800 0100 7c00 5300 7208  ..I.d.H...|.S.r.
-00000320: 0000 0029 01da 0469 6e69 7472 0d00 0000  ...)...initr....
-00000330: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00000340: 0a5f 5f61 656e 7465 725f 5f15 0000 0073  .__aenter__....s
-00000350: 0600 0000 0280 0e01 0401 7a1f 4175 7468  ..........z.Auth
-00000360: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
-00000370: 2e5f 5f61 656e 7465 725f 5f63 0100 0000  .__aenter__c....
-00000380: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000390: c700 0000 7316 0000 0081 017c 006a 00a0  ....s......|.j..
-000003a0: 01a1 0049 0064 0048 0001 0064 0053 0072  ...I.d.H...d.S.r
-000003b0: 0800 0000 2902 720c 0000 00da 0563 6c6f  ....).r......clo
-000003c0: 7365 2902 720e 0000 00da 0461 7267 7372  se).r......argsr
-000003d0: 0f00 0000 720f 0000 0072 1000 0000 da09  ....r....r......
-000003e0: 5f5f 6165 7869 745f 5f19 0000 0073 0400  __aexit__....s..
-000003f0: 0000 0280 1401 7a1e 4175 7468 6f72 697a  ......z.Authoriz
-00000400: 6174 696f 6e57 7261 7070 6572 2e5f 5f61  ationWrapper.__a
-00000410: 6578 6974 5f5f 4e72 0c00 0000 6302 0000  exit__Nr....c...
-00000420: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00000430: 00c3 0000 0073 9200 0000 8101 7c01 7c00  .....s......|.|.
-00000440: 5f00 7c01 6400 7500 720d 7401 a002 a100  _.|.d.u.r.t.....
-00000450: 7c00 5f00 7c00 6a03 7312 4a00 8201 7c00  |._.|.j.s.J...|.
-00000460: a004 a100 722a 7c00 6a05 7c00 6a03 6401  ....r*|.j.|.j.d.
-00000470: 1900 7c00 6a03 6402 1900 7c00 6a00 6403  ..|.j.d...|.j.d.
-00000480: 8d03 4900 6400 4800 0100 6400 5300 7c00  ..I.d.H...d.S.|.
-00000490: a006 a100 7245 7c00 6a03 6404 1900 7c00  ....rE|.j.d...|.
-000004a0: 5f07 7c00 6a08 7c00 6a03 6405 1900 7c00  _.|.j.|.j.d...|.
-000004b0: 6a03 6402 1900 7c00 6a00 6403 8d03 0100  j.d...|.j.d.....
-000004c0: 6400 5300 7409 6406 8301 8201 2907 4eda  d.S.t.d.....).N.
-000004d0: 0468 6f73 74da 0b70 7269 7661 7465 5f6b  .host..private_k
-000004e0: 6579 2901 720c 0000 00da 0b61 6363 6f75  ey).r......accou
-000004f0: 6e74 5f75 726c da0e 7075 626c 6963 5f6b  nt_url..public_k
-00000500: 6579 5f75 726c 7a27 4e6f 206b 6e6f 776e  ey_urlz'No known
-00000510: 2061 7574 686f 7269 7a61 7469 6f6e 206d   authorization m
-00000520: 6574 686f 6420 6176 6169 6c61 626c 6529  ethod available)
-00000530: 0a72 0c00 0000 da07 6169 6f68 7474 70da  .r......aiohttp.
-00000540: 0d43 6c69 656e 7453 6573 7369 6f6e 7209  .ClientSessionr.
-00000550: 0000 00da 0d5f 6861 735f 6d6f 6f5f 6175  ....._has_moo_au
-00000560: 7468 da21 7769 7468 5f68 6f73 745f 616e  th.!with_host_an
-00000570: 645f 6564 3235 3531 395f 7072 6976 6174  d_ed25519_privat
-00000580: 655f 6b65 79da 135f 6861 735f 6874 7470  e_key.._has_http
-00000590: 5f73 6967 6e61 7475 7265 720a 0000 00da  _signaturer.....
-000005a0: 1377 6974 685f 6874 7470 5f73 6967 6e61  .with_http_signa
-000005b0: 7475 7265 da09 4578 6365 7074 696f 6e29  ture..Exception)
-000005c0: 0272 0e00 0000 720c 0000 0072 0f00 0000  .r....r....r....
-000005d0: 720f 0000 0072 1000 0000 7212 0000 001c  r....r....r.....
-000005e0: 0000 0073 2200 0000 0280 0601 0801 0a01  ...s"...........
-000005f0: 0a02 0802 0401 1401 10ff 0803 0c01 0401  ................
-00000600: 0801 0801 0401 0afd 0806 7a19 4175 7468  ..........z.Auth
-00000610: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
-00000620: 2e69 6e69 7472 1700 0000 7218 0000 0063  .initr....r....c
-00000630: 0400 0000 0000 0000 0000 0000 0500 0000  ................
-00000640: 0400 0000 c300 0000 7340 0000 0081 017c  ........s@.....|
-00000650: 0364 0075 0072 0974 00a0 01a1 007d 0374  .d.u.r.t.....}.t
-00000660: 027c 0283 017d 0474 037c 037c 017c 0483  .|...}.t.|.|.|..
-00000670: 0349 0064 0048 007c 005f 0474 057c 037c  .I.d.H.|._.t.|.|
-00000680: 047c 0283 037c 005f 067c 0053 0072 0800  .|...|._.|.S.r..
-00000690: 0000 2907 721b 0000 0072 1c00 0000 7206  ..).r....r....r.
-000006a0: 0000 0072 0300 0000 720a 0000 0072 0400  ...r....r....r..
-000006b0: 0000 720b 0000 0029 0572 0e00 0000 7217  ..r....).r....r.
-000006c0: 0000 0072 1800 0000 720c 0000 005a 0764  ...r....r....Z.d
-000006d0: 6964 5f6b 6579 720f 0000 0072 0f00 0000  id_keyr....r....
-000006e0: 7210 0000 0072 1e00 0000 3100 0000 730e  r....r....1...s.
-000006f0: 0000 0002 8008 0608 0108 0114 020e 0204  ................
-00000700: 027a 3641 7574 686f 7269 7a61 7469 6f6e  .z6Authorization
-00000710: 5772 6170 7065 722e 7769 7468 5f68 6f73  Wrapper.with_hos
-00000720: 745f 616e 645f 6564 3235 3531 395f 7072  t_and_ed25519_pr
-00000730: 6976 6174 655f 6b65 7972 0a00 0000 6302  ivate_keyr....c.
-00000740: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000750: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
-00000760: 5f00 7c00 5300 7208 0000 0029 0172 0a00  _.|.S.r....).r..
-00000770: 0000 2902 720e 0000 0072 0a00 0000 720f  ..).r....r....r.
-00000780: 0000 0072 0f00 0000 7210 0000 00da 0d77  ...r....r......w
-00000790: 6974 685f 6163 746f 725f 6964 4100 0000  ith_actor_idA...
-000007a0: 7304 0000 0006 0104 017a 2241 7574 686f  s........z"Autho
-000007b0: 7269 7a61 7469 6f6e 5772 6170 7065 722e  rizationWrapper.
-000007c0: 7769 7468 5f61 6374 6f72 5f69 6472 1a00  with_actor_idr..
-000007d0: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
-000007e0: 0000 0004 0000 0043 0000 0073 2200 0000  .......C...s"...
-000007f0: 7c03 6400 7500 7208 7400 a001 a100 7d03  |.d.u.r.t.....}.
-00000800: 7402 7c03 7c01 7c02 8303 7c00 5f03 7c00  t.|.|.|...|._.|.
-00000810: 5300 7208 0000 0029 0472 1b00 0000 721c  S.r....).r....r.
-00000820: 0000 0072 0500 0000 720b 0000 0029 0472  ...r....r....).r
-00000830: 0e00 0000 721a 0000 0072 1800 0000 720c  ....r....r....r.
-00000840: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00000850: 0000 7220 0000 0045 0000 0073 0800 0000  ..r ...E...s....
-00000860: 0806 0801 0e02 0402 7a28 4175 7468 6f72  ........z(Author
-00000870: 697a 6174 696f 6e57 7261 7070 6572 2e77  izationWrapper.w
-00000880: 6974 685f 6874 7470 5f73 6967 6e61 7475  ith_http_signatu
-00000890: 7265 6301 0000 0000 0000 0000 0000 0001  rec.............
-000008a0: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
-000008b0: 7c00 a000 6700 6401 a201 a101 5300 2902  |...g.d.....S.).
-000008c0: 4e29 0372 1900 0000 721a 0000 0072 1800  N).r....r....r..
-000008d0: 0000 a901 da09 5f68 6173 5f6b 6579 7372  ......_has_keysr
-000008e0: 0d00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-000008f0: 0000 0072 1f00 0000 5200 0000 f302 0000  ...r....R.......
-00000900: 000e 017a 2841 7574 686f 7269 7a61 7469  ...z(Authorizati
-00000910: 6f6e 5772 6170 7065 722e 5f68 6173 5f68  onWrapper._has_h
-00000920: 7474 705f 7369 676e 6174 7572 6563 0100  ttp_signaturec..
-00000930: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00000940: 0000 4300 0000 730e 0000 007c 00a0 0064  ..C...s....|...d
-00000950: 0164 0267 02a1 0153 0029 034e 7217 0000  .d.g...S.).Nr...
-00000960: 0072 1800 0000 7223 0000 0072 0d00 0000  .r....r#...r....
-00000970: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000980: 1d00 0000 5500 0000 7225 0000 007a 2241  ....U...r%...z"A
-00000990: 7574 686f 7269 7a61 7469 6f6e 5772 6170  uthorizationWrap
-000009a0: 7065 722e 5f68 6173 5f6d 6f6f 5f61 7574  per._has_moo_aut
-000009b0: 68da 086b 6579 5f6c 6973 7463 0200 0000  h..key_listc....
-000009c0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-000009d0: 4300 0000 731e 0000 007c 0144 005d 0a7d  C...s....|.D.].}
-000009e0: 027c 027c 006a 0076 0172 0c01 0064 0153  .|.|.j.v.r...d.S
-000009f0: 0071 0264 0253 0029 034e 4654 2901 7209  .q.d.S.).NFT).r.
-00000a00: 0000 0029 0372 0e00 0000 7226 0000 00da  ...).r....r&....
-00000a10: 036b 6579 720f 0000 0072 0f00 0000 7210  .keyr....r....r.
-00000a20: 0000 0072 2400 0000 5800 0000 730a 0000  ...r$...X...s...
-00000a30: 0008 010a 0106 0102 ff04 037a 1e41 7574  ...........z.Aut
-00000a40: 686f 7269 7a61 7469 6f6e 5772 6170 7065  horizationWrappe
-00000a50: 722e 5f68 6173 5f6b 6579 7372 0800 0000  r._has_keysr....
-00000a60: 2912 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000a70: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000a80: 6e61 6d65 5f5f 7211 0000 0072 1300 0000  name__r....r....
-00000a90: 7216 0000 0072 0200 0000 721b 0000 0072  r....r....r....r
-00000aa0: 1c00 0000 7212 0000 00da 0373 7472 721e  ....r......strr.
-00000ab0: 0000 0072 2200 0000 7220 0000 0072 1f00  ...r"...r ...r..
-00000ac0: 0000 721d 0000 00da 046c 6973 7472 2400  ..r......listr$.
-00000ad0: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000ae0: 0072 1000 0000 7207 0000 000e 0000 0073  .r....r........s
-00000af0: 3200 0000 0800 0801 0806 0804 1603 0219  2...............
-00000b00: 04fc 0202 02fe 0203 02fd 0804 0afc 0e10  ................
-00000b10: 0208 04fc 0202 02fe 0203 02fd 0804 0afc  ................
-00000b20: 080d 0803 1203 7207 0000 0029 10da 076c  ......r....)...l
-00000b30: 6f67 6769 6e67 da06 7479 7069 6e67 7202  ogging..typingr.
-00000b40: 0000 0072 1b00 0000 5a0e 626f 7669 6e65  ...r....Z.bovine
-00000b50: 2e63 6c69 656e 7473 7203 0000 005a 1e62  .clientsr....Z.b
-00000b60: 6f76 696e 652e 636c 6965 6e74 732e 6d6f  ovine.clients.mo
-00000b70: 6f5f 6175 7468 5f63 6c69 656e 7472 0400  o_auth_clientr..
-00000b80: 0000 5a21 626f 7669 6e65 2e63 6c69 656e  ..Z!bovine.clien
-00000b90: 7473 2e73 6967 6e65 645f 6874 7470 5f63  ts.signed_http_c
-00000ba0: 6c69 656e 7472 0500 0000 5a0d 626f 7669  lientr....Z.bovi
-00000bb0: 6e65 2e63 7279 7074 6f72 0600 0000 da09  ne.cryptor......
-00000bc0: 6765 744c 6f67 6765 7272 2800 0000 da06  getLoggerr(.....
-00000bd0: 6c6f 6767 6572 7207 0000 0072 0f00 0000  loggerr....r....
-00000be0: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00000bf0: 083c 6d6f 6475 6c65 3e01 0000 0073 1200  .<module>....s..
-00000c00: 0000 0800 0c01 0802 0c02 0c01 0c01 0c01  ................
-00000c10: 0a02 1203                                ....
+00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
+00000080: 6d0d 5a0d 0100 6500 a00e 650f a101 5a10  m.Z...e...e...Z.
+00000090: 4700 6408 6409 8400 6409 8302 5a11 6401  G.d.d...d...Z.d.
+000000a0: 5300 290a e900 0000 004e 2901 da08 4f70  S.)......N)...Op
+000000b0: 7469 6f6e 616c 2901 da19 6c6f 6f6b 7570  tional)...lookup
+000000c0: 5f64 6964 5f77 6974 685f 7765 6266 696e  _did_with_webfin
+000000d0: 6765 7229 01da 1042 6561 7265 7241 7574  ger)...BearerAut
+000000e0: 6843 6c69 656e 7429 01da 0d4d 6f6f 4175  hClient)...MooAu
+000000f0: 7468 436c 6965 6e74 2901 da10 5369 676e  thClient)...Sign
+00000100: 6564 4874 7470 436c 6965 6e74 2901 da16  edHttpClient)...
+00000110: 7072 6976 6174 655f 6b65 795f 746f 5f64  private_key_to_d
+00000120: 6964 5f6b 6579 6300 0000 0000 0000 0000  id_keyc.........
+00000130: 0000 0000 0000 0008 0000 0040 0000 0073  ...........@...s
+00000140: ca00 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
+00000150: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+00000160: 8400 5a05 6421 6408 6506 6507 6a08 1900  ..Z.d!d.e.e.j...
+00000170: 6602 6409 640a 8405 5a09 0907 6421 640b  f.d.d...Z...d!d.
+00000180: 650a 640c 650a 6408 6506 6507 6a08 1900  e.d.e.d.e.e.j...
+00000190: 6606 640d 640e 8405 5a0b 640f 650a 6602  f.d.d...Z.d.e.f.
+000001a0: 6410 6411 8404 5a0c 0907 6421 6412 650a  d.d...Z...d!d.e.
+000001b0: 640c 650a 6408 6506 6507 6a08 1900 6606  d.e.d.e.e.j...f.
+000001c0: 6413 6414 8405 5a0d 0907 6421 6415 650a  d.d...Z...d!d.e.
+000001d0: 6408 6506 6507 6a08 1900 6604 6416 6417  d.e.e.j...f.d.d.
+000001e0: 8405 5a0e 6418 6419 8400 5a0f 641a 641b  ..Z.d.d...Z.d.d.
+000001f0: 8400 5a10 641c 641d 8400 5a11 641e 6512  ..Z.d.d...Z.d.e.
+00000200: 6602 641f 6420 8404 5a13 6407 5300 2922  f.d.d ..Z.d.S.)"
+00000210: da14 4175 7468 6f72 697a 6174 696f 6e57  ..AuthorizationW
+00000220: 7261 7070 6572 6301 0000 0000 0000 0000  rapperc.........
+00000230: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000240: 1c00 0000 6400 7c00 5f00 6400 7c00 5f01  ....d.|._.d.|._.
+00000250: 6400 7c00 5f02 6400 7c00 5f03 6400 5300  d.|._.d.|._.d.S.
+00000260: a901 4e29 04da 0663 6f6e 6669 67da 0861  ..N)...config..a
+00000270: 6374 6f72 5f69 64da 0663 6c69 656e 74da  ctor_id..client.
+00000280: 0773 6573 7369 6f6e a901 da04 7365 6c66  .session....self
+00000290: a900 7210 0000 00fa 5d2f 776f 6f64 7065  ..r.....]/woodpe
+000002a0: 636b 6572 2f73 7263 2f63 6f64 6562 6572  cker/src/codeber
+000002b0: 672e 6f72 672f 626f 7669 6e65 2f62 6f76  g.org/bovine/bov
+000002c0: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
+000002d0: 652f 6163 7469 7669 7479 7075 622f 6175  e/activitypub/au
+000002e0: 7468 6f72 697a 6174 696f 6e5f 7772 6170  thorization_wrap
+000002f0: 7065 722e 7079 da08 5f5f 696e 6974 5f5f  per.py..__init__
+00000300: 1000 0000 7308 0000 0006 0106 0106 010a  ....s...........
+00000310: 017a 1d41 7574 686f 7269 7a61 7469 6f6e  .z.Authorization
+00000320: 5772 6170 7065 722e 5f5f 696e 6974 5f5f  Wrapper.__init__
+00000330: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000340: 0002 0000 00c3 0000 0073 1400 0000 8101  .........s......
+00000350: 7c00 a000 a100 4900 6400 4800 0100 7c00  |.....I.d.H...|.
+00000360: 5300 7209 0000 0029 01da 0469 6e69 7472  S.r....)...initr
+00000370: 0e00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
+00000380: 0000 00da 0a5f 5f61 656e 7465 725f 5f16  .....__aenter__.
+00000390: 0000 0073 0600 0000 0280 0e01 0401 7a1f  ...s..........z.
+000003a0: 4175 7468 6f72 697a 6174 696f 6e57 7261  AuthorizationWra
+000003b0: 7070 6572 2e5f 5f61 656e 7465 725f 5f63  pper.__aenter__c
+000003c0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000003d0: 0200 0000 c700 0000 7316 0000 0081 017c  ........s......|
+000003e0: 006a 00a0 01a1 0049 0064 0048 0001 0064  .j.....I.d.H...d
+000003f0: 0053 0072 0900 0000 2902 720d 0000 00da  .S.r....).r.....
+00000400: 0563 6c6f 7365 2902 720f 0000 00da 0461  .close).r......a
+00000410: 7267 7372 1000 0000 7210 0000 0072 1100  rgsr....r....r..
+00000420: 0000 da09 5f5f 6165 7869 745f 5f1a 0000  ....__aexit__...
+00000430: 0073 0400 0000 0280 1401 7a1e 4175 7468  .s........z.Auth
+00000440: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
+00000450: 2e5f 5f61 6578 6974 5f5f 4e72 0d00 0000  .__aexit__Nr....
+00000460: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000470: 0005 0000 00c3 0000 0073 c000 0000 8101  .........s......
+00000480: 7c01 7c00 5f00 7c01 6400 7500 720d 7401  |.|._.|.d.u.r.t.
+00000490: a002 a100 7c00 5f00 7c00 6a03 7312 4a00  ....|._.|.j.s.J.
+000004a0: 8201 7c00 a004 a100 722a 7c00 6a05 7c00  ..|.....r*|.j.|.
+000004b0: 6a03 6401 1900 7c00 6a03 6402 1900 7c00  j.d...|.j.d...|.
+000004c0: 6a00 6403 8d03 4900 6400 4800 0100 6400  j.d...I.d.H...d.
+000004d0: 5300 7c00 a006 a100 7245 7c00 6a03 6404  S.|.....rE|.j.d.
+000004e0: 1900 7c00 5f07 7c00 6a08 7c00 6a03 6405  ..|._.|.j.|.j.d.
+000004f0: 1900 7c00 6a03 6402 1900 7c00 6a00 6403  ..|.j.d...|.j.d.
+00000500: 8d03 0100 6400 5300 7c00 a009 a100 725c  ....d.S.|.....r\
+00000510: 7c00 6a03 6404 1900 7c00 5f07 7c00 6a0a  |.j.d...|._.|.j.
+00000520: 7c00 6a03 6406 1900 7c00 6a00 6403 8d02  |.j.d...|.j.d...
+00000530: 0100 6400 5300 740b 6407 8301 8201 2908  ..d.S.t.d.....).
+00000540: 4eda 0468 6f73 74da 0b70 7269 7661 7465  N..host..private
+00000550: 5f6b 6579 2901 720d 0000 00da 0b61 6363  _key).r......acc
+00000560: 6f75 6e74 5f75 726c da0e 7075 626c 6963  ount_url..public
+00000570: 5f6b 6579 5f75 726c da0c 6163 6365 7373  _key_url..access
+00000580: 5f74 6f6b 656e 7a27 4e6f 206b 6e6f 776e  _tokenz'No known
+00000590: 2061 7574 686f 7269 7a61 7469 6f6e 206d   authorization m
+000005a0: 6574 686f 6420 6176 6169 6c61 626c 6529  ethod available)
+000005b0: 0c72 0d00 0000 da07 6169 6f68 7474 70da  .r......aiohttp.
+000005c0: 0d43 6c69 656e 7453 6573 7369 6f6e 720a  .ClientSessionr.
+000005d0: 0000 00da 0d5f 6861 735f 6d6f 6f5f 6175  ....._has_moo_au
+000005e0: 7468 da21 7769 7468 5f68 6f73 745f 616e  th.!with_host_an
+000005f0: 645f 6564 3235 3531 395f 7072 6976 6174  d_ed25519_privat
+00000600: 655f 6b65 79da 135f 6861 735f 6874 7470  e_key.._has_http
+00000610: 5f73 6967 6e61 7475 7265 720b 0000 00da  _signaturer.....
+00000620: 1377 6974 685f 6874 7470 5f73 6967 6e61  .with_http_signa
+00000630: 7475 7265 da10 5f68 6173 5f62 6561 7265  ture.._has_beare
+00000640: 725f 6175 7468 da11 7769 7468 5f62 6561  r_auth..with_bea
+00000650: 7265 725f 746f 6b65 6eda 0945 7863 6570  rer_token..Excep
+00000660: 7469 6f6e 2902 720f 0000 0072 0d00 0000  tion).r....r....
+00000670: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+00000680: 1300 0000 1d00 0000 7328 0000 0002 8006  ........s(......
+00000690: 0108 010a 010a 0208 0204 0114 0110 ff08  ................
+000006a0: 030c 0104 0108 0108 0104 010a fd08 050c  ................
+000006b0: 011a 0108 027a 1941 7574 686f 7269 7a61  .....z.Authoriza
+000006c0: 7469 6f6e 5772 6170 7065 722e 696e 6974  tionWrapper.init
+000006d0: 7218 0000 0072 1900 0000 6304 0000 0000  r....r....c.....
+000006e0: 0000 0000 0000 0005 0000 0004 0000 00c3  ................
+000006f0: 0000 0073 4000 0000 8101 7c03 6400 7500  ...s@.....|.d.u.
+00000700: 7209 7400 a001 a100 7d03 7402 7c02 8301  r.t.....}.t.|...
+00000710: 7d04 7403 7c03 7c01 7c04 8303 4900 6400  }.t.|.|.|...I.d.
+00000720: 4800 7c00 5f04 7405 7c03 7c04 7c02 8303  H.|._.t.|.|.|...
+00000730: 7c00 5f06 7c00 5300 7209 0000 0029 0772  |._.|.S.r....).r
+00000740: 1d00 0000 721e 0000 0072 0700 0000 7203  ....r....r....r.
+00000750: 0000 0072 0b00 0000 7205 0000 0072 0c00  ...r....r....r..
+00000760: 0000 2905 720f 0000 0072 1800 0000 7219  ..).r....r....r.
+00000770: 0000 0072 0d00 0000 5a07 6469 645f 6b65  ...r....Z.did_ke
+00000780: 7972 1000 0000 7210 0000 0072 1100 0000  yr....r....r....
+00000790: 7220 0000 0035 0000 0073 0e00 0000 0280  r ...5...s......
+000007a0: 0806 0801 0801 1402 0e02 0402 7a36 4175  ............z6Au
+000007b0: 7468 6f72 697a 6174 696f 6e57 7261 7070  thorizationWrapp
+000007c0: 6572 2e77 6974 685f 686f 7374 5f61 6e64  er.with_host_and
+000007d0: 5f65 6432 3535 3139 5f70 7269 7661 7465  _ed25519_private
+000007e0: 5f6b 6579 720b 0000 0063 0200 0000 0000  _keyr....c......
+000007f0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00000800: 0000 730a 0000 007c 017c 005f 007c 0053  ..s....|.|._.|.S
+00000810: 0072 0900 0000 2901 720b 0000 0029 0272  .r....).r....).r
+00000820: 0f00 0000 720b 0000 0072 1000 0000 7210  ....r....r....r.
+00000830: 0000 0072 1100 0000 da0d 7769 7468 5f61  ...r......with_a
+00000840: 6374 6f72 5f69 6445 0000 0073 0400 0000  ctor_idE...s....
+00000850: 0601 0401 7a22 4175 7468 6f72 697a 6174  ....z"Authorizat
+00000860: 696f 6e57 7261 7070 6572 2e77 6974 685f  ionWrapper.with_
+00000870: 6163 746f 725f 6964 721b 0000 0063 0400  actor_idr....c..
+00000880: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00000890: 0000 4300 0000 7322 0000 007c 0364 0075  ..C...s"...|.d.u
+000008a0: 0072 0874 00a0 01a1 007d 0374 027c 037c  .r.t.....}.t.|.|
+000008b0: 017c 0283 037c 005f 037c 0053 0072 0900  .|...|._.|.S.r..
+000008c0: 0000 2904 721d 0000 0072 1e00 0000 7206  ..).r....r....r.
+000008d0: 0000 0072 0c00 0000 2904 720f 0000 0072  ...r....).r....r
+000008e0: 1b00 0000 7219 0000 0072 0d00 0000 7210  ....r....r....r.
+000008f0: 0000 0072 1000 0000 7211 0000 0072 2200  ...r....r....r".
+00000900: 0000 4900 0000 7308 0000 0008 0608 010e  ..I...s.........
+00000910: 0204 027a 2841 7574 686f 7269 7a61 7469  ...z(Authorizati
+00000920: 6f6e 5772 6170 7065 722e 7769 7468 5f68  onWrapper.with_h
+00000930: 7474 705f 7369 676e 6174 7572 6572 1c00  ttp_signaturer..
+00000940: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+00000950: 0000 0003 0000 0043 0000 0073 2000 0000  .......C...s ...
+00000960: 7c02 6400 7500 7208 7400 a001 a100 7d02  |.d.u.r.t.....}.
+00000970: 7402 7c02 7c01 8302 7c00 5f03 7c00 5300  t.|.|...|._.|.S.
+00000980: 7209 0000 0029 0472 1d00 0000 721e 0000  r....).r....r...
+00000990: 0072 0400 0000 720c 0000 0029 0372 0f00  .r....r....).r..
+000009a0: 0000 721c 0000 0072 0d00 0000 7210 0000  ..r....r....r...
+000009b0: 0072 1000 0000 7211 0000 0072 2400 0000  .r....r....r$...
+000009c0: 5600 0000 7308 0000 0008 0508 010c 0204  V...s...........
+000009d0: 027a 2641 7574 686f 7269 7a61 7469 6f6e  .z&Authorization
+000009e0: 5772 6170 7065 722e 7769 7468 5f62 6561  Wrapper.with_bea
+000009f0: 7265 725f 746f 6b65 6e63 0100 0000 0000  rer_tokenc......
+00000a00: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000a10: 0000 730e 0000 007c 00a0 0067 0064 01a2  ..s....|...g.d..
+00000a20: 01a1 0153 0029 024e 2903 721a 0000 0072  ...S.).N).r....r
+00000a30: 1b00 0000 7219 0000 00a9 01da 095f 6861  ....r........_ha
+00000a40: 735f 6b65 7973 720e 0000 0072 1000 0000  s_keysr....r....
+00000a50: 7210 0000 0072 1100 0000 7221 0000 0062  r....r....r!...b
+00000a60: 0000 00f3 0200 0000 0e01 7a28 4175 7468  ..........z(Auth
+00000a70: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
+00000a80: 2e5f 6861 735f 6874 7470 5f73 6967 6e61  ._has_http_signa
+00000a90: 7475 7265 6301 0000 0000 0000 0000 0000  turec...........
+00000aa0: 0001 0000 0004 0000 0043 0000 00f3 0e00  .........C......
+00000ab0: 0000 7c00 a000 6401 6402 6702 a101 5300  ..|...d.d.g...S.
+00000ac0: 2903 4e72 1800 0000 7219 0000 0072 2700  ).Nr....r....r'.
+00000ad0: 0000 720e 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000ae0: 0072 1100 0000 721f 0000 0065 0000 0072  .r....r....e...r
+00000af0: 2900 0000 7a22 4175 7468 6f72 697a 6174  )...z"Authorizat
+00000b00: 696f 6e57 7261 7070 6572 2e5f 6861 735f  ionWrapper._has_
+00000b10: 6d6f 6f5f 6175 7468 6301 0000 0000 0000  moo_authc.......
+00000b20: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00000b30: 0072 2a00 0000 2903 4e72 1a00 0000 721c  .r*...).Nr....r.
+00000b40: 0000 0072 2700 0000 720e 0000 0072 1000  ...r'...r....r..
+00000b50: 0000 7210 0000 0072 1100 0000 7223 0000  ..r....r....r#..
+00000b60: 0068 0000 0072 2900 0000 7a25 4175 7468  .h...r)...z%Auth
+00000b70: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
+00000b80: 2e5f 6861 735f 6265 6172 6572 5f61 7574  ._has_bearer_aut
+00000b90: 68da 086b 6579 5f6c 6973 7463 0200 0000  h..key_listc....
+00000ba0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000bb0: 4300 0000 731e 0000 007c 0144 005d 0a7d  C...s....|.D.].}
+00000bc0: 027c 027c 006a 0076 0172 0c01 0064 0153  .|.|.j.v.r...d.S
+00000bd0: 0071 0264 0253 0029 034e 4654 2901 720a  .q.d.S.).NFT).r.
+00000be0: 0000 0029 0372 0f00 0000 722b 0000 00da  ...).r....r+....
+00000bf0: 036b 6579 7210 0000 0072 1000 0000 7211  .keyr....r....r.
+00000c00: 0000 0072 2800 0000 6b00 0000 730a 0000  ...r(...k...s...
+00000c10: 0008 010a 0106 0102 ff04 037a 1e41 7574  ...........z.Aut
+00000c20: 686f 7269 7a61 7469 6f6e 5772 6170 7065  horizationWrappe
+00000c30: 722e 5f68 6173 5f6b 6579 7372 0900 0000  r._has_keysr....
+00000c40: 2914 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000c50: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000c60: 6e61 6d65 5f5f 7212 0000 0072 1400 0000  name__r....r....
+00000c70: 7217 0000 0072 0200 0000 721d 0000 0072  r....r....r....r
+00000c80: 1e00 0000 7213 0000 00da 0373 7472 7220  ....r......strr 
+00000c90: 0000 0072 2600 0000 7222 0000 0072 2400  ...r&...r"...r$.
+00000ca0: 0000 7221 0000 0072 1f00 0000 7223 0000  ..r!...r....r#..
+00000cb0: 00da 046c 6973 7472 2800 0000 7210 0000  ...listr(...r...
+00000cc0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000cd0: 7208 0000 000f 0000 0073 4000 0000 0800  r........s@.....
+00000ce0: 0801 0806 0804 1603 021c 04fc 0202 02fe  ................
+00000cf0: 0203 02fd 0804 0afc 0e10 0208 04fc 0202  ................
+00000d00: 02fe 0203 02fd 0804 0afc 0210 04fd 0202  ................
+00000d10: 02fe 0803 0afd 080c 0803 0803 1203 7208  ..............r.
+00000d20: 0000 0029 12da 076c 6f67 6769 6e67 da06  ...)...logging..
+00000d30: 7479 7069 6e67 7202 0000 0072 1d00 0000  typingr....r....
+00000d40: 5a0e 626f 7669 6e65 2e63 6c69 656e 7473  Z.bovine.clients
+00000d50: 7203 0000 005a 1562 6f76 696e 652e 636c  r....Z.bovine.cl
+00000d60: 6965 6e74 732e 6265 6172 6572 7204 0000  ients.bearerr...
+00000d70: 005a 1762 6f76 696e 652e 636c 6965 6e74  .Z.bovine.client
+00000d80: 732e 6d6f 6f5f 6175 7468 7205 0000 005a  s.moo_authr....Z
+00000d90: 1a62 6f76 696e 652e 636c 6965 6e74 732e  .bovine.clients.
+00000da0: 7369 676e 6564 5f68 7474 7072 0600 0000  signed_httpr....
+00000db0: 5a0d 626f 7669 6e65 2e63 7279 7074 6f72  Z.bovine.cryptor
+00000dc0: 0700 0000 da09 6765 744c 6f67 6765 7272  ......getLoggerr
+00000dd0: 2d00 0000 da06 6c6f 6767 6572 7208 0000  -.....loggerr...
+00000de0: 0072 1000 0000 7210 0000 0072 1000 0000  .r....r....r....
+00000df0: 7211 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000e00: 0000 0073 1400 0000 0800 0c01 0802 0c02  ...s............
+00000e10: 0c01 0c01 0c01 0c01 0a02 1203            ............
```

### Comparing `bovine-0.1.2/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc` & `bovine-0.1.3/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2219 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,155 +1,177 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 ab08 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 150b 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
+00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
-00000050: 6406 8400 5a05 4700 6407 6408 8400 6408  d...Z.G.d.d...d.
-00000060: 8302 5a06 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
-00000070: 2901 da0e 7072 696e 745f 6163 7469 7669  )...print_activi
-00000080: 7479 e901 0000 00a9 01da 1243 6f6c 6c65  ty.........Colle
-00000090: 6374 696f 6e49 7465 7261 746f 7263 0100  ctionIteratorc..
-000000a0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-000000b0: 0000 4300 0000 7346 0000 0064 017c 0076  ..C...sF...d.|.v
-000000c0: 0072 087c 0064 0119 007d 0064 0244 005d  .r.|.d...}.d.D.]
-000000d0: 167d 017c 017c 0076 0072 207c 007c 0119  .}.|.|.v.r |.|..
-000000e0: 0072 2074 006a 017c 007c 0119 0067 0064  .r t.j.|.|...g.d
-000000f0: 0364 048d 0302 0001 0053 0071 0a64 0553  .d.......S.q.d.S
-00000100: 0029 064e da06 6f62 6a65 6374 2904 da04  .).N..object)...
-00000110: 6e61 6d65 da07 7375 6d6d 6172 79da 0763  name..summary..c
-00000120: 6f6e 7465 6e74 da02 6964 5429 02da 0474  ontent..idT)...t
-00000130: 6167 73da 0573 7472 6970 7a10 2d2d 2d20  ags..stripz.--- 
-00000140: 756e 6b6e 6f77 6e20 202d 2d2d 2902 da06  unknown  ---)...
-00000150: 626c 6561 6368 da05 636c 6561 6e29 02da  bleach..clean)..
-00000160: 036f 626a da03 6b65 79a9 0072 1100 0000  .obj..key..r....
-00000170: fa59 2f77 6f6f 6470 6563 6b65 722f 7372  .Y/woodpecker/sr
-00000180: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
-00000190: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-000001a0: 696e 652f 626f 7669 6e65 2f61 6374 6976  ine/bovine/activ
-000001b0: 6974 7970 7562 2f63 6f6c 6c65 6374 696f  itypub/collectio
-000001c0: 6e5f 6865 6c70 6572 2e70 79da 1773 686f  n_helper.py..sho
-000001d0: 7274 5f76 6572 7369 6f6e 5f6f 665f 6f62  rt_version_of_ob
-000001e0: 6a65 6374 0800 0000 730e 0000 0008 0108  ject....s.......
-000001f0: 0108 0210 0118 0102 8004 0272 1300 0000  ...........r....
-00000200: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000210: 0003 0000 0040 0000 0073 4000 0000 6500  .....@...s@...e.
-00000220: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00000230: 6404 8400 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
-00000240: 6408 8400 5a06 6410 640a 640b 8401 5a07  d...Z.d.d.d...Z.
-00000250: 6411 640d 640e 8401 5a08 640f 5300 2912  d.d.d...Z.d.S.).
-00000260: da10 436f 6c6c 6563 7469 6f6e 4865 6c70  ..CollectionHelp
-00000270: 6572 6303 0000 0000 0000 0000 0000 0003  erc.............
-00000280: 0000 0002 0000 0043 0000 0073 2e00 0000  .......C...s....
-00000290: 7c01 7c00 5f00 7c02 7c00 5f01 6400 7c00  |.|._.|.|._.d.|.
-000002a0: 5f02 6400 7c00 5f03 6400 7c00 5f04 6400  _.d.|._.d.|._.d.
-000002b0: 7c00 5f05 6900 7c00 5f06 6400 5300 a901  |._.i.|._.d.S...
-000002c0: 4e29 07da 0d63 6f6c 6c65 6374 696f 6e5f  N)...collection_
-000002d0: 6964 da05 6163 746f 72da 1162 6173 6963  id..actor..basic
-000002e0: 5f69 6e66 6f72 6d61 7469 6f6e da05 6974  _information..it
-000002f0: 656d 73da 0a6e 6578 745f 6974 656d 73da  ems..next_items.
-00000300: 0a69 7465 6d5f 696e 6465 78da 0d65 6c65  .item_index..ele
-00000310: 6d65 6e74 5f63 6163 6865 2903 da04 7365  ment_cache)...se
-00000320: 6c66 7216 0000 0072 1700 0000 7211 0000  lfr....r....r...
-00000330: 0072 1100 0000 7212 0000 00da 085f 5f69  .r....r......__i
-00000340: 6e69 745f 5f14 0000 0073 0e00 0000 0601  nit__....s......
-00000350: 0601 0602 0601 0601 0601 0a02 7a19 436f  ............z.Co
-00000360: 6c6c 6563 7469 6f6e 4865 6c70 6572 2e5f  llectionHelper._
-00000370: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000380: 0000 0000 0200 0000 0400 0000 c300 0000  ................
-00000390: 7358 0000 0081 017c 006a 0064 0075 0072  sX.....|.j.d.u.r
-000003a0: 117c 006a 01a0 027c 006a 03a1 0149 0064  .|.j...|.j...I.d
-000003b0: 0048 007c 005f 007c 006a 01a0 027c 006a  .H.|._.|.j...|.j
-000003c0: 0064 0119 00a1 0149 0064 0048 007d 017c  .d.....I.d.H.}.|
-000003d0: 0164 0219 007c 005f 047c 0164 0319 007c  .d...|._.|.d...|
-000003e0: 005f 0564 047c 005f 0664 0053 0029 054e  ._.d.|._.d.S.).N
-000003f0: da05 6669 7273 74da 0c6f 7264 6572 6564  ..first..ordered
-00000400: 4974 656d 73da 046e 6578 7472 0100 0000  Items..nextr....
-00000410: 2907 7218 0000 0072 1700 0000 da03 6765  ).r....r......ge
-00000420: 7472 1600 0000 7219 0000 0072 1a00 0000  tr....r....r....
-00000430: 721b 0000 0029 0272 1d00 0000 da08 7265  r....).r......re
-00000440: 7370 6f6e 7365 7211 0000 0072 1100 0000  sponser....r....
-00000450: 7212 0000 00da 0772 6566 7265 7368 1f00  r......refresh..
-00000460: 0000 730e 0000 0002 800a 0116 0118 020a  ..s.............
-00000470: 020a 010a 017a 1843 6f6c 6c65 6374 696f  .....z.Collectio
-00000480: 6e48 656c 7065 722e 7265 6672 6573 6863  nHelper.refreshc
-00000490: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-000004a0: 0900 0000 c300 0000 7378 0000 0081 0174  ........sx.....t
-000004b0: 0083 0001 0074 0064 0174 017c 006a 0283  .....t.d.t.|.j..
-000004c0: 019b 009d 0283 0101 0074 0083 0001 0074  .........t.....t
-000004d0: 037c 006a 0283 0144 005d 235c 027d 017d  .|.j...D.]#\.}.}
-000004e0: 027c 00a0 047c 02a1 0149 0064 0048 007d  .|...|...I.d.H.}
-000004f0: 0374 007c 0164 029b 0464 037c 03a0 0564  .t.|.d...d.|...d
-00000500: 04a1 0164 059b 0464 0374 067c 0383 0164  ...d...d.t.|...d
-00000510: 0064 0685 0219 009b 009d 0583 0101 0071  .d.............q
-00000520: 1664 0053 0029 074e 7a0d 4974 656d 7320  .d.S.).Nz.Items 
-00000530: 6c6f 6164 6564 20da 0134 7a02 3a20 da04  loaded ..4z.: ..
-00000540: 7479 7065 da02 3130 e950 0000 0029 07da  type..10.P...)..
-00000550: 0570 7269 6e74 da03 6c65 6e72 1900 0000  .print..lenr....
-00000560: da09 656e 756d 6572 6174 65da 0b67 6574  ..enumerate..get
-00000570: 5f65 6c65 6d65 6e74 7222 0000 0072 1300  _elementr"...r..
-00000580: 0000 2904 721d 0000 00da 0369 6478 da04  ..).r......idx..
-00000590: 6974 656d 720f 0000 0072 1100 0000 7211  itemr....r....r.
-000005a0: 0000 0072 1200 0000 7208 0000 0029 0000  ...r....r....)..
-000005b0: 0073 1000 0000 0280 0601 1401 0601 1201  .s..............
-000005c0: 1001 3001 04fe 7a18 436f 6c6c 6563 7469  ..0...z.Collecti
-000005d0: 6f6e 4865 6c70 6572 2e73 756d 6d61 7279  onHelper.summary
-000005e0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000005f0: 0003 0000 00c3 0000 0073 4400 0000 8101  .........sD.....
-00000600: 7400 7c01 7401 8302 7308 7c01 5300 7c01  t.|.t...s.|.S.|.
-00000610: 7c00 6a02 7600 7212 7c00 6a02 7c01 1900  |.j.v.r.|.j.|...
-00000620: 5300 7c00 6a03 a004 7c01 a101 4900 6400  S.|.j...|...I.d.
-00000630: 4800 7d02 7c02 7c00 6a02 7c01 3c00 7c02  H.}.|.|.j.|.<.|.
-00000640: 5300 7215 0000 0029 05da 0a69 7369 6e73  S.r....)...isins
-00000650: 7461 6e63 65da 0373 7472 721c 0000 0072  tance..strr....r
-00000660: 1700 0000 da0d 7072 6f78 795f 656c 656d  ......proxy_elem
-00000670: 656e 7429 0372 1d00 0000 da07 656c 656d  ent).r......elem
-00000680: 656e 74da 0672 6573 756c 7472 1100 0000  ent..resultr....
-00000690: 7211 0000 0072 1200 0000 722c 0000 0031  r....r....r,...1
-000006a0: 0000 0073 1000 0000 0280 0a01 0401 0a02  ...s............
-000006b0: 0a01 1202 0a02 0402 7a1c 436f 6c6c 6563  ........z.Collec
-000006c0: 7469 6f6e 4865 6c70 6572 2e67 6574 5f65  tionHelper.get_e
-000006d0: 6c65 6d65 6e74 4663 0200 0000 0000 0000  lementFc........
-000006e0: 0000 0000 0400 0000 0400 0000 c300 0000  ................
-000006f0: 737c 0000 0081 017c 006a 0074 017c 006a  s|.....|.j.t.|.j
-00000700: 0283 016b 0572 217c 006a 03a0 047c 006a  ...k.r!|.j...|.j
-00000710: 05a1 0149 0064 0048 007d 027c 0004 006a  ...I.d.H.}.|...j
-00000720: 027c 0264 0119 0037 0002 005f 027c 0264  .|.d...7..._.|.d
-00000730: 0219 007c 005f 057c 006a 027c 006a 0019  ...|._.|.j.|.j..
-00000740: 007d 037c 0004 006a 0064 0337 0002 005f  .}.|...j.d.7..._
-00000750: 007c 00a0 067c 03a1 0149 0064 0048 007d  .|...|...I.d.H.}
-00000760: 037c 0172 3c74 077c 0383 0101 007c 0353  .|.r<t.|.....|.S
-00000770: 0029 044e 7220 0000 0072 2100 0000 7203  .).Nr ...r!...r.
-00000780: 0000 0029 0872 1b00 0000 722a 0000 0072  ...).r....r*...r
-00000790: 1900 0000 7217 0000 0072 2200 0000 721a  ....r....r"...r.
-000007a0: 0000 0072 2c00 0000 7202 0000 0029 0472  ...r,...r....).r
-000007b0: 1d00 0000 5a08 646f 5f70 7269 6e74 7223  ....Z.do_printr#
-000007c0: 0000 0072 3300 0000 7211 0000 0072 1100  ...r3...r....r..
-000007d0: 0000 7212 0000 00da 096e 6578 745f 6974  ..r......next_it
-000007e0: 656d 3e00 0000 7316 0000 0002 8010 0114  em>...s.........
-000007f0: 0112 010a 010c 020e 0110 0204 0208 0104  ................
-00000800: 027a 1a43 6f6c 6c65 6374 696f 6e48 656c  .z.CollectionHel
-00000810: 7065 722e 6e65 7874 5f69 7465 6de9 0a00  per.next_item...
-00000820: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00000830: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
-00000840: 7400 7c00 7c01 8302 5300 7215 0000 0072  t.|.|...S.r....r
-00000850: 0400 0000 2902 721d 0000 005a 0a6d 6178  ....).r....Z.max
-00000860: 5f6e 756d 6265 7272 1100 0000 7211 0000  _numberr....r...
-00000870: 0072 1200 0000 da07 6974 6572 6174 654e  .r......iterateN
-00000880: 0000 0073 0200 0000 0a01 7a18 436f 6c6c  ...s......z.Coll
-00000890: 6563 7469 6f6e 4865 6c70 6572 2e69 7465  ectionHelper.ite
-000008a0: 7261 7465 4e29 0146 2901 7235 0000 0029  rateN).F).r5...)
-000008b0: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000008c0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000008d0: 616d 655f 5f72 1e00 0000 7224 0000 0072  ame__r....r$...r
-000008e0: 0800 0000 722c 0000 0072 3400 0000 7236  ....r,...r4...r6
-000008f0: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
-00000900: 0000 7212 0000 0072 1400 0000 1300 0000  ..r....r........
-00000910: 730e 0000 0008 0008 0108 0b08 0a08 080a  s...............
-00000920: 0d0e 1072 1400 0000 2907 720d 0000 005a  ...r....).r....Z
-00000930: 2262 6f76 696e 652e 6163 7469 7669 7479  "bovine.activity
-00000940: 7374 7265 616d 732e 7574 696c 732e 7072  streams.utils.pr
-00000950: 696e 7472 0200 0000 5a13 636f 6c6c 6563  intr....Z.collec
-00000960: 7469 6f6e 5f69 7465 7261 746f 7272 0500  tion_iteratorr..
-00000970: 0000 7213 0000 0072 1400 0000 7211 0000  ..r....r....r...
-00000980: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-00000990: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
-000009a0: 0000 0008 000c 020c 0208 0312 0b         .............
+00000050: 6406 8400 5a05 6407 6408 8400 5a06 4700  d...Z.d.d...Z.G.
+00000060: 6409 640a 8400 640a 8302 5a07 6401 5300  d.d...d...Z.d.S.
+00000070: 290b e900 0000 004e 2901 da0e 7072 696e  )......N)...prin
+00000080: 745f 6163 7469 7669 7479 e901 0000 00a9  t_activity......
+00000090: 01da 1243 6f6c 6c65 6374 696f 6e49 7465  ...CollectionIte
+000000a0: 7261 746f 7263 0200 0000 0000 0000 0000  ratorc..........
+000000b0: 0000 0300 0000 0500 0000 c300 0000 7384  ..............s.
+000000c0: 0000 0081 0167 007d 0274 007c 0174 0183  .....g.}.t.|.t..
+000000d0: 0272 107c 00a0 027c 01a1 0149 0064 0048  .r.|...|...I.d.H
+000000e0: 007d 0164 017c 0176 0072 207c 0164 0119  .}.d.|.v.r |.d..
+000000f0: 007d 0274 007c 0274 0183 0272 207c 0267  .}.t.|.t...r |.g
+00000100: 017d 0264 027c 0176 0072 307c 0274 037c  .}.d.|.v.r0|.t.|
+00000110: 007c 0164 0219 0083 0249 0064 0048 0017  .|.d.....I.d.H..
+00000120: 0053 0064 037c 0176 0072 407c 0274 037c  .S.d.|.v.r@|.t.|
+00000130: 007c 0164 0319 0083 0249 0064 0048 0017  .|.d.....I.d.H..
+00000140: 0053 007c 0253 0029 044e da05 6974 656d  .S.|.S.).N..item
+00000150: 73da 0566 6972 7374 da04 6e65 7874 2904  s..first..next).
+00000160: da0a 6973 696e 7374 616e 6365 da03 7374  ..isinstance..st
+00000170: 72da 0d70 726f 7879 5f65 6c65 6d65 6e74  r..proxy_element
+00000180: da17 616c 6c5f 636f 6c6c 6563 7469 6f6e  ..all_collection
+00000190: 5f65 6c65 6d65 6e74 7329 03da 0663 6c69  _elements)...cli
+000001a0: 656e 74da 0a63 6f6c 6c65 6374 696f 6eda  ent..collection.
+000001b0: 0672 6573 756c 74a9 0072 1000 0000 fa59  .result..r.....Y
+000001c0: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
+000001d0: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
+000001e0: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
+000001f0: 652f 626f 7669 6e65 2f61 6374 6976 6974  e/bovine/activit
+00000200: 7970 7562 2f63 6f6c 6c65 6374 696f 6e5f  ypub/collection_
+00000210: 6865 6c70 6572 2e70 7972 0c00 0000 0800  helper.pyr......
+00000220: 0000 731a 0000 0002 8004 010a 0110 0108  ..s.............
+00000230: 0208 010a 0106 0108 0218 0108 0218 0104  ................
+00000240: 0272 0c00 0000 6301 0000 0000 0000 0000  .r....c.........
+00000250: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
+00000260: 4600 0000 6401 7c00 7600 7208 7c00 6401  F...d.|.v.r.|.d.
+00000270: 1900 7d00 6402 4400 5d16 7d01 7c01 7c00  ..}.d.D.].}.|.|.
+00000280: 7600 7220 7c00 7c01 1900 7220 7400 6a01  v.r |.|...r t.j.
+00000290: 7c00 7c01 1900 6700 6403 6404 8d03 0200  |.|...g.d.d.....
+000002a0: 0100 5300 710a 6405 5300 2906 4eda 066f  ..S.q.d.S.).N..o
+000002b0: 626a 6563 7429 04da 046e 616d 65da 0773  bject)...name..s
+000002c0: 756d 6d61 7279 da07 636f 6e74 656e 74da  ummary..content.
+000002d0: 0269 6454 2902 da04 7461 6773 da05 7374  .idT)...tags..st
+000002e0: 7269 707a 102d 2d2d 2075 6e6b 6e6f 776e  ripz.--- unknown
+000002f0: 2020 2d2d 2d29 02da 0662 6c65 6163 68da    ---)...bleach.
+00000300: 0563 6c65 616e 2902 da03 6f62 6ada 036b  .clean)...obj..k
+00000310: 6579 7210 0000 0072 1000 0000 7211 0000  eyr....r....r...
+00000320: 00da 1773 686f 7274 5f76 6572 7369 6f6e  ...short_version
+00000330: 5f6f 665f 6f62 6a65 6374 1b00 0000 730e  _of_object....s.
+00000340: 0000 0008 0108 0108 0210 0118 0102 8004  ................
+00000350: 0272 1d00 0000 6300 0000 0000 0000 0000  .r....c.........
+00000360: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000370: 4000 0000 6500 5a01 6400 5a02 6401 6402  @...e.Z.d.Z.d.d.
+00000380: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+00000390: 8400 5a05 6407 6408 8400 5a06 6410 640a  ..Z.d.d...Z.d.d.
+000003a0: 640b 8401 5a07 6411 640d 640e 8401 5a08  d...Z.d.d.d...Z.
+000003b0: 640f 5300 2912 da10 436f 6c6c 6563 7469  d.S.)...Collecti
+000003c0: 6f6e 4865 6c70 6572 6303 0000 0000 0000  onHelperc.......
+000003d0: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
+000003e0: 0073 2e00 0000 7c01 7c00 5f00 7c02 7c00  .s....|.|._.|.|.
+000003f0: 5f01 6400 7c00 5f02 6400 7c00 5f03 6400  _.d.|._.d.|._.d.
+00000400: 7c00 5f04 6400 7c00 5f05 6900 7c00 5f06  |._.d.|._.i.|._.
+00000410: 6400 5300 a901 4e29 07da 0d63 6f6c 6c65  d.S...N)...colle
+00000420: 6374 696f 6e5f 6964 da05 6163 746f 72da  ction_id..actor.
+00000430: 1162 6173 6963 5f69 6e66 6f72 6d61 7469  .basic_informati
+00000440: 6f6e 7206 0000 00da 0a6e 6578 745f 6974  onr......next_it
+00000450: 656d 73da 0a69 7465 6d5f 696e 6465 78da  ems..item_index.
+00000460: 0d65 6c65 6d65 6e74 5f63 6163 6865 2903  .element_cache).
+00000470: da04 7365 6c66 7220 0000 0072 2100 0000  ..selfr ...r!...
+00000480: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00000490: 085f 5f69 6e69 745f 5f27 0000 0073 0e00  .__init__'...s..
+000004a0: 0000 0601 0601 0602 0601 0601 0601 0a02  ................
+000004b0: 7a19 436f 6c6c 6563 7469 6f6e 4865 6c70  z.CollectionHelp
+000004c0: 6572 2e5f 5f69 6e69 745f 5f63 0100 0000  er.__init__c....
+000004d0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000004e0: c300 0000 7366 0000 0081 017c 006a 0064  ....sf.....|.j.d
+000004f0: 0075 0072 117c 006a 01a0 027c 006a 03a1  .u.r.|.j...|.j..
+00000500: 0149 0064 0048 007c 005f 0064 017c 006a  .I.d.H.|._.d.|.j
+00000510: 0076 0172 1864 0053 007c 006a 01a0 027c  .v.r.d.S.|.j...|
+00000520: 006a 0064 0119 00a1 0149 0064 0048 007d  .j.d.....I.d.H.}
+00000530: 017c 0164 0219 007c 005f 047c 0164 0319  .|.d...|._.|.d..
+00000540: 007c 005f 0564 047c 005f 0664 0053 0029  .|._.d.|._.d.S.)
+00000550: 054e 7207 0000 00da 0c6f 7264 6572 6564  .Nr......ordered
+00000560: 4974 656d 7372 0800 0000 7201 0000 0029  Itemsr....r....)
+00000570: 0772 2200 0000 7221 0000 00da 0367 6574  .r"...r!.....get
+00000580: 7220 0000 0072 0600 0000 7223 0000 0072  r ...r....r#...r
+00000590: 2400 0000 2902 7226 0000 00da 0872 6573  $...).r&.....res
+000005a0: 706f 6e73 6572 1000 0000 7210 0000 0072  ponser....r....r
+000005b0: 1100 0000 da07 7265 6672 6573 6832 0000  ......refresh2..
+000005c0: 0073 1200 0000 0280 0a01 1601 0a02 0401  .s..............
+000005d0: 1802 0a02 0a01 0a01 7a18 436f 6c6c 6563  ........z.Collec
+000005e0: 7469 6f6e 4865 6c70 6572 2e72 6566 7265  tionHelper.refre
+000005f0: 7368 6301 0000 0000 0000 0000 0000 0004  shc.............
+00000600: 0000 0009 0000 00c3 0000 0073 7800 0000  ...........sx...
+00000610: 8101 7400 8300 0100 7400 6401 7401 7c00  ..t.....t.d.t.|.
+00000620: 6a02 8301 9b00 9d02 8301 0100 7400 8300  j...........t...
+00000630: 0100 7403 7c00 6a02 8301 4400 5d23 5c02  ..t.|.j...D.]#\.
+00000640: 7d01 7d02 7c00 a004 7c02 a101 4900 6400  }.}.|...|...I.d.
+00000650: 4800 7d03 7400 7c01 6402 9b04 6403 7c03  H.}.t.|.d...d.|.
+00000660: a005 6404 a101 6405 9b04 6403 7406 7c03  ..d...d...d.t.|.
+00000670: 8301 6400 6406 8502 1900 9b00 9d05 8301  ..d.d...........
+00000680: 0100 7116 6400 5300 2907 4e7a 0d49 7465  ..q.d.S.).Nz.Ite
+00000690: 6d73 206c 6f61 6465 6420 da01 347a 023a  ms loaded ..4z.:
+000006a0: 20da 0474 7970 65da 0231 30e9 5000 0000   ..type..10.P...
+000006b0: 2907 da05 7072 696e 74da 036c 656e 7206  )...print..lenr.
+000006c0: 0000 00da 0965 6e75 6d65 7261 7465 da0b  .....enumerate..
+000006d0: 6765 745f 656c 656d 656e 7472 2900 0000  get_elementr)...
+000006e0: 721d 0000 0029 0472 2600 0000 da03 6964  r....).r&.....id
+000006f0: 78da 0469 7465 6d72 1b00 0000 7210 0000  x..itemr....r...
+00000700: 0072 1000 0000 7211 0000 0072 1400 0000  .r....r....r....
+00000710: 3f00 0000 7310 0000 0002 8006 0114 0106  ?...s...........
+00000720: 0112 0110 0130 0104 fe7a 1843 6f6c 6c65  .....0...z.Colle
+00000730: 6374 696f 6e48 656c 7065 722e 7375 6d6d  ctionHelper.summ
+00000740: 6172 7963 0200 0000 0000 0000 0000 0000  aryc............
+00000750: 0300 0000 0300 0000 c300 0000 7344 0000  ............sD..
+00000760: 0081 0174 007c 0174 0183 0273 087c 0153  ...t.|.t...s.|.S
+00000770: 007c 017c 006a 0276 0072 127c 006a 027c  .|.|.j.v.r.|.j.|
+00000780: 0119 0053 007c 006a 03a0 047c 01a1 0149  ...S.|.j...|...I
+00000790: 0064 0048 007d 027c 027c 006a 027c 013c  .d.H.}.|.|.j.|.<
+000007a0: 007c 0253 0072 1f00 0000 2905 7209 0000  .|.S.r....).r...
+000007b0: 0072 0a00 0000 7225 0000 0072 2100 0000  .r....r%...r!...
+000007c0: 720b 0000 0029 0372 2600 0000 da07 656c  r....).r&.....el
+000007d0: 656d 656e 7472 0f00 0000 7210 0000 0072  ementr....r....r
+000007e0: 1000 0000 7211 0000 0072 3300 0000 4700  ....r....r3...G.
+000007f0: 0000 7310 0000 0002 800a 0104 010a 020a  ..s.............
+00000800: 0112 020a 0204 027a 1c43 6f6c 6c65 6374  .......z.Collect
+00000810: 696f 6e48 656c 7065 722e 6765 745f 656c  ionHelper.get_el
+00000820: 656d 656e 7446 6302 0000 0000 0000 0000  ementFc.........
+00000830: 0000 0004 0000 0004 0000 00c3 0000 0073  ...............s
+00000840: 7c00 0000 8101 7c00 6a00 7401 7c00 6a02  |.....|.j.t.|.j.
+00000850: 8301 6b05 7221 7c00 6a03 a004 7c00 6a05  ..k.r!|.j...|.j.
+00000860: a101 4900 6400 4800 7d02 7c00 0400 6a02  ..I.d.H.}.|...j.
+00000870: 7c02 6401 1900 3700 0200 5f02 7c02 6402  |.d...7..._.|.d.
+00000880: 1900 7c00 5f05 7c00 6a02 7c00 6a00 1900  ..|._.|.j.|.j...
+00000890: 7d03 7c00 0400 6a00 6403 3700 0200 5f00  }.|...j.d.7..._.
+000008a0: 7c00 a006 7c03 a101 4900 6400 4800 7d03  |...|...I.d.H.}.
+000008b0: 7c01 723c 7407 7c03 8301 0100 7c03 5300  |.r<t.|.....|.S.
+000008c0: 2904 4e72 2800 0000 7208 0000 0072 0300  ).Nr(...r....r..
+000008d0: 0000 2908 7224 0000 0072 3100 0000 7206  ..).r$...r1...r.
+000008e0: 0000 0072 2100 0000 7229 0000 0072 2300  ...r!...r)...r#.
+000008f0: 0000 7233 0000 0072 0200 0000 2904 7226  ..r3...r....).r&
+00000900: 0000 005a 0864 6f5f 7072 696e 7472 2a00  ...Z.do_printr*.
+00000910: 0000 720f 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000920: 0072 1100 0000 da09 6e65 7874 5f69 7465  .r......next_ite
+00000930: 6d54 0000 0073 1600 0000 0280 1001 1401  mT...s..........
+00000940: 1201 0a01 0c02 0e01 1002 0402 0801 0402  ................
+00000950: 7a1a 436f 6c6c 6563 7469 6f6e 4865 6c70  z.CollectionHelp
+00000960: 6572 2e6e 6578 745f 6974 656d e90a 0000  er.next_item....
+00000970: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00000980: 0000 0300 0000 4300 0000 730a 0000 0074  ......C...s....t
+00000990: 007c 007c 0183 0253 0072 1f00 0000 7204  .|.|...S.r....r.
+000009a0: 0000 0029 0272 2600 0000 5a0a 6d61 785f  ...).r&...Z.max_
+000009b0: 6e75 6d62 6572 7210 0000 0072 1000 0000  numberr....r....
+000009c0: 7211 0000 00da 0769 7465 7261 7465 6400  r......iterated.
+000009d0: 0000 7302 0000 000a 017a 1843 6f6c 6c65  ..s......z.Colle
+000009e0: 6374 696f 6e48 656c 7065 722e 6974 6572  ctionHelper.iter
+000009f0: 6174 654e 2901 4629 0172 3800 0000 2909  ateN).F).r8...).
+00000a00: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000a10: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000a20: 6d65 5f5f 7227 0000 0072 2b00 0000 7214  me__r'...r+...r.
+00000a30: 0000 0072 3300 0000 7237 0000 0072 3900  ...r3...r7...r9.
+00000a40: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000a50: 0072 1100 0000 721e 0000 0026 0000 0073  .r....r....&...s
+00000a60: 0e00 0000 0800 0801 080b 080d 0808 0a0d  ................
+00000a70: 0e10 721e 0000 0029 0872 1900 0000 5a22  ..r....).r....Z"
+00000a80: 626f 7669 6e65 2e61 6374 6976 6974 7973  bovine.activitys
+00000a90: 7472 6561 6d73 2e75 7469 6c73 2e70 7269  treams.utils.pri
+00000aa0: 6e74 7202 0000 005a 1363 6f6c 6c65 6374  ntr....Z.collect
+00000ab0: 696f 6e5f 6974 6572 6174 6f72 7205 0000  ion_iteratorr...
+00000ac0: 0072 0c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000ad0: 7210 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+00000ae0: 1100 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000af0: 0000 730c 0000 0008 000c 020c 0208 0308  ..s.............
+00000b00: 1312 0b                                  ...
```

### Comparing `bovine-0.1.2/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2757 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 c50a 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 c50a 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6400 6401 6c0a 5a0a 6400 6403 6c0b 6d0c  d.d.l.Z.d.d.l.m.
 00000070: 5a0c 0100 6400 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
```

### Comparing `bovine-0.1.2/bovine/activitypub/authorization_wrapper.py` & `bovine-0.1.3/bovine/activitypub/authorization_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from typing import Optional
 
 import aiohttp
 
 from bovine.clients import lookup_did_with_webfinger
-from bovine.clients.moo_auth_client import MooAuthClient
-from bovine.clients.signed_http_client import SignedHttpClient
+from bovine.clients.bearer import BearerAuthClient
+from bovine.clients.moo_auth import MooAuthClient
+from bovine.clients.signed_http import SignedHttpClient
 from bovine.crypto import private_key_to_did_key
 
 logger = logging.getLogger(__name__)
 
 
 class AuthorizationWrapper:
     def __init__(self):
@@ -39,14 +40,17 @@
         elif self._has_http_signature():
             self.actor_id = self.config["account_url"]
             self.with_http_signature(
                 self.config["public_key_url"],
                 self.config["private_key"],
                 session=self.session,
             )
+        elif self._has_bearer_auth():
+            self.actor_id = self.config["account_url"]
+            self.with_bearer_token(self.config["access_token"], session=self.session)
         else:
             raise Exception("No known authorization method available")
 
     async def with_host_and_ed25519_private_key(
         self,
         host: str,
         private_key: str,
@@ -75,19 +79,34 @@
         if session is None:
             session = aiohttp.ClientSession()
 
         self.client = SignedHttpClient(session, public_key_url, private_key)
 
         return self
 
+    def with_bearer_token(
+        self,
+        access_token: str,
+        session: Optional[aiohttp.ClientSession] = None,
+    ):
+        if session is None:
+            session = aiohttp.ClientSession()
+
+        self.client = BearerAuthClient(session, access_token)
+
+        return self
+
     def _has_http_signature(self):
         return self._has_keys(["account_url", "public_key_url", "private_key"])
 
     def _has_moo_auth(self):
         return self._has_keys(["host", "private_key"])
 
+    def _has_bearer_auth(self):
+        return self._has_keys(["account_url", "access_token"])
+
     def _has_keys(self, key_list: list):
         for key in key_list:
             if key not in self.config:
                 return False
 
         return True
```

### Comparing `bovine-0.1.2/bovine/activitypub/collection_helper.py` & `bovine-0.1.3/bovine/activitypub/collection_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 import bleach
 
 from bovine.activitystreams.utils.print import print_activity
 
 from .collection_iterator import CollectionIterator
 
 
+async def all_collection_elements(client, collection):
+    result = []
+    if isinstance(collection, str):
+        collection = await client.proxy_element(collection)
+
+    if "items" in collection:
+        result = collection["items"]
+        if isinstance(result, str):
+            result = [result]
+
+    if "first" in collection:
+        return result + await all_collection_elements(client, collection["first"])
+
+    if "next" in collection:
+        return result + await all_collection_elements(client, collection["next"])
+
+    return result
+
+
 def short_version_of_object(obj):
     if "object" in obj:
         obj = obj["object"]
 
     for key in ["name", "summary", "content", "id"]:
         if key in obj and obj[key]:
             return bleach.clean(obj[key], tags=[], strip=True)
@@ -28,14 +47,17 @@
 
         self.element_cache = {}
 
     async def refresh(self):
         if self.basic_information is None:
             self.basic_information = await self.actor.get(self.collection_id)
 
+        if "first" not in self.basic_information:
+            return
+
         response = await self.actor.get(self.basic_information["first"])
 
         self.items = response["orderedItems"]
         self.next_items = response["next"]
         self.item_index = 0
 
     async def summary(self):
```

### Comparing `bovine-0.1.2/bovine/activitypub/test_actor.py` & `bovine-0.1.3/bovine/activitypub/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/activitystreams/__init__.py` & `bovine-0.1.3/bovine/activitystreams/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,28 @@
             endpoints["eventSource"] = self.event_source
         if self.proxy_url:
             endpoints["proxyUrl"] = self.proxy_url
         return endpoints
 
 
 @dataclass
+class Collection:
+    id: str
+    items: list
+
+    def build(self) -> dict:
+        return {
+            "@context": "https://www.w3.org/ns/activitystreams",
+            "id": self.id,
+            "items": self.items,
+            "type": "Collection",
+        }
+
+
+@dataclass
 class OrderedCollection:
     id: str
     items: list | None = None
     count: int = 0
     first: str | None = None
     last: str | None = None
```

### Comparing `bovine-0.1.2/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.3/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 4682 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,267 +1,291 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 4a12 0000  o.........AdJ...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 5d13 0000  o.......*.Nd]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 650b 6408 6504 6508 650a 6602 1900 6604  e.d.e.e.e.f...f.
 00000080: 6409 640a 8404 5a0c 6501 4700 640b 640c  d.d...Z.e.G.d.d.
 00000090: 8400 640c 8302 8301 5a0d 6501 4700 640d  ..d.....Z.e.G.d.
 000000a0: 640e 8400 640e 8302 8301 5a0e 6501 4700  d...d.....Z.e.G.
-000000b0: 640f 6410 8400 6410 8302 8301 5a0f 6411  d.d...d.....Z.d.
-000000c0: 5300 2912 e900 0000 0029 01da 0964 6174  S.)......)...dat
-000000d0: 6163 6c61 7373 2902 da08 4f70 7469 6f6e  aclass)...Option
-000000e0: 616c da05 5475 706c 6529 01da 0a56 6973  al..Tuple)...Vis
-000000f0: 6962 696c 6974 79e9 0100 0000 2901 da0f  ibility.....)...
-00000100: 4163 7469 7669 7479 4661 6374 6f72 7929  ActivityFactory)
-00000110: 01da 0d4f 626a 6563 7446 6163 746f 7279  ...ObjectFactory
-00000120: da0c 6163 746f 725f 6f62 6a65 6374 da06  ..actor_object..
-00000130: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-00000140: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00000150: 1200 0000 7400 7c00 8301 7401 7c00 6401  ....t.|...t.|.d.
-00000160: 8d01 6602 5300 2902 7a36 4275 696c 6473  ..f.S.).z6Builds
-00000170: 2061 6374 6976 6974 7920 616e 6420 6f62   activity and ob
-00000180: 6a65 6374 2066 6163 746f 7269 6573 2066  ject factories f
-00000190: 726f 6d20 6163 746f 7220 6f62 6a65 6374  rom actor object
-000001a0: 2901 5a11 6163 746f 725f 696e 666f 726d  ).Z.actor_inform
-000001b0: 6174 696f 6e29 0272 0700 0000 7208 0000  ation).r....r...
-000001c0: 0029 0172 0900 0000 a900 720b 0000 00fa  .).r......r.....
-000001d0: 542f 776f 6f64 7065 636b 6572 2f73 7263  T/woodpecker/src
-000001e0: 2f63 6f64 6562 6572 672e 6f72 672f 626f  /codeberg.org/bo
-000001f0: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
-00000200: 6e65 2f62 6f76 696e 652f 6163 7469 7669  ne/bovine/activi
-00000210: 7479 7374 7265 616d 732f 5f5f 696e 6974  tystreams/__init
-00000220: 5f5f 2e70 79da 1a66 6163 746f 7269 6573  __.py..factories
-00000230: 5f66 6f72 5f61 6374 6f72 5f6f 626a 6563  _for_actor_objec
-00000240: 740a 0000 0073 0200 0000 1204 720d 0000  t....s......r...
-00000250: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000260: 0000 0300 0000 4000 0000 7324 0100 0065  ......@...s$...e
-00000270: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-00000280: 0564 023c 0064 035a 0665 0465 0564 043c  .d.<.d.Z.e.e.d.<
-00000290: 0064 055a 0765 0865 0419 0065 0564 063c  .d.Z.e.e...e.d.<
-000002a0: 0064 055a 0965 0865 0419 0065 0564 073c  .d.Z.e.e...e.d.<
-000002b0: 0064 055a 0a65 0865 0419 0065 0564 083c  .d.Z.e.e...e.d.<
-000002c0: 0064 055a 0b65 0865 0419 0065 0564 093c  .d.Z.e.e...e.d.<
-000002d0: 0064 055a 0c65 0865 0419 0065 0564 0a3c  .d.Z.e.e...e.d.<
-000002e0: 0064 055a 0d65 0865 0419 0065 0564 0b3c  .d.Z.e.e...e.d.<
-000002f0: 0064 055a 0e65 0865 0419 0065 0564 0c3c  .d.Z.e.e...e.d.<
-00000300: 0064 055a 0f65 0865 0419 0065 0564 0d3c  .d.Z.e.e...e.d.<
-00000310: 0064 055a 1065 0865 0419 0065 0564 0e3c  .d.Z.e.e...e.d.<
-00000320: 0064 055a 1165 0865 0419 0065 0564 0f3c  .d.Z.e.e...e.d.<
-00000330: 0064 055a 1265 0865 0419 0065 0564 103c  .d.Z.e.e...e.d.<
-00000340: 0064 055a 1365 0865 1419 0065 0564 113c  .d.Z.e.e...e.d.<
-00000350: 0064 055a 1565 0865 0419 0065 0564 123c  .d.Z.e.e...e.d.<
-00000360: 0065 166a 1766 0164 1364 1484 015a 1864  .e.j.f.d.d...Z.d
-00000370: 1564 1684 005a 1964 1764 1884 005a 1a64  .d...Z.d.d...Z.d
-00000380: 1964 1a84 005a 1b64 1b64 1c84 005a 1c64  .d...Z.d.d...Z.d
-00000390: 0553 0029 1dda 0541 6374 6f72 7a37 4163  .S.)...Actorz7Ac
-000003a0: 746f 7220 636c 6173 7320 7265 7072 6573  tor class repres
-000003b0: 656e 7473 2074 6865 2062 6173 6963 2041  ents the basic A
-000003c0: 6374 6976 6974 7953 7472 6561 6d73 2061  ctivityStreams a
-000003d0: 6374 6f72 2eda 0269 645a 0650 6572 736f  ctor...idZ.Perso
-000003e0: 6eda 0474 7970 654e da04 6e61 6d65 da12  n..typeN..name..
-000003f0: 7072 6566 6572 7265 645f 7573 6572 6e61  preferred_userna
-00000400: 6d65 da05 696e 626f 78da 066f 7574 626f  me..inbox..outbo
-00000410: 78da 0966 6f6c 6c6f 7765 7273 da09 666f  x..followers..fo
-00000420: 6c6c 6f77 696e 67da 0a70 7562 6c69 635f  llowing..public_
-00000430: 6b65 79da 0f70 7562 6c69 635f 6b65 795f  key..public_key_
-00000440: 6e61 6d65 da0c 6576 656e 745f 736f 7572  name..event_sour
-00000450: 6365 da09 7072 6f78 795f 7572 6cda 0773  ce..proxy_url..s
-00000460: 756d 6d61 7279 da04 6963 6f6e da03 7572  ummary..icon..ur
-00000470: 6c63 0200 0000 0000 0000 0000 0000 0500  lc..............
-00000480: 0000 0400 0000 4300 0000 739c 0000 007c  ......C...s....|
-00000490: 00a0 00a1 007c 006a 017c 006a 0264 019c  .....|.j.|.j.d..
-000004a0: 037c 00a0 03a1 00a5 017c 006a 047c 0164  .|.......|.j.|.d
-000004b0: 028d 01a5 017d 027c 006a 0572 1c7c 006a  .....}.|.j.r.|.j
-000004c0: 057c 0264 033c 007c 0174 066a 076b 0272  .|.d.<.|.t.j.k.r
-000004d0: 237c 0253 007c 006a 0872 2c7c 006a 087c  #|.S.|.j.r,|.j.|
-000004e0: 0264 043c 006e 087c 006a 0572 347c 006a  .d.<.n.|.j.r4|.j
-000004f0: 057c 0264 043c 007c 006a 097c 006a 0a7c  .|.d.<.|.j.|.j.|
-00000500: 006a 0b64 059c 03a0 0ca1 0044 005d 0c5c  .j.d.......D.].\
-00000510: 027d 037d 047c 0464 0675 0172 4b7c 047c  .}.}.|.d.u.rK|.|
-00000520: 027c 033c 0071 3f7c 0253 0029 077a 3043  .|.<.q?|.S.).z0C
-00000530: 7265 6174 6573 2074 6865 206a 736f 6e2d  reates the json-
-00000540: 6c64 2072 6570 7265 7365 6e74 6174 696f  ld representatio
-00000550: 6e20 6f66 2074 6865 2061 6374 6f72 2e29  n of the actor.)
-00000560: 03fa 0840 636f 6e74 6578 7472 0f00 0000  ...@contextr....
-00000570: 7210 0000 0029 01da 0a76 6973 6962 696c  r....)...visibil
-00000580: 6974 795a 1170 7265 6665 7272 6564 5573  ityZ.preferredUs
-00000590: 6572 6e61 6d65 7211 0000 0029 0372 1b00  ernamer....).r..
-000005a0: 0000 721c 0000 0072 1d00 0000 4e29 0dda  ..r....r....N)..
-000005b0: 0e5f 6275 696c 645f 636f 6e74 6578 7472  ._build_contextr
-000005c0: 0f00 0000 7210 0000 00da 115f 6275 696c  ....r......_buil
-000005d0: 645f 7075 626c 6963 5f6b 6579 da10 5f62  d_public_key.._b
-000005e0: 7569 6c64 5f65 6e64 706f 696e 7473 7212  uild_endpointsr.
-000005f0: 0000 0072 0500 0000 da03 5745 4272 1100  ...r......WEBr..
-00000600: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000610: 00da 0569 7465 6d73 2905 da04 7365 6c66  ...items)...self
-00000620: 721f 0000 00da 0672 6573 756c 74da 036b  r......result..k
-00000630: 6579 da05 7661 6c75 6572 0b00 0000 720b  ey..valuer....r.
-00000640: 0000 0072 0c00 0000 da05 6275 696c 6426  ...r......build&
-00000650: 0000 0073 3400 0000 0603 0401 0401 04fd  ...s4...........
-00000660: 0604 02fc 0a05 04fb 0608 0a01 0a02 0401  ................
-00000670: 0602 0c01 0601 0a01 0403 0401 0401 04fd  ................
-00000680: 0404 0afc 0805 0801 0280 0402 7a0b 4163  ............z.Ac
-00000690: 746f 722e 6275 696c 6463 0100 0000 0000  tor.buildc......
-000006a0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-000006b0: 0000 7312 0000 007c 006a 0072 0764 0164  ..s....|.j.r.d.d
-000006c0: 0267 0253 0064 0153 0029 034e fa25 6874  .g.S.d.S.).N.%ht
-000006d0: 7470 733a 2f2f 7777 772e 7733 2e6f 7267  tps://www.w3.org
-000006e0: 2f6e 732f 6163 7469 7669 7479 7374 7265  /ns/activitystre
-000006f0: 616d 737a 1c68 7474 7073 3a2f 2f77 3369  amsz.https://w3i
-00000700: 642e 6f72 672f 7365 6375 7269 7479 2f76  d.org/security/v
-00000710: 3129 0172 1700 0000 a901 7225 0000 0072  1).r......r%...r
-00000720: 0b00 0000 720b 0000 0072 0c00 0000 7220  ....r....r....r 
-00000730: 0000 0045 0000 0073 0a00 0000 0601 0202  ...E...s........
-00000740: 0201 04fe 0405 7a14 4163 746f 722e 5f62  ......z.Actor._b
-00000750: 7569 6c64 5f63 6f6e 7465 7874 6301 0000  uild_contextc...
-00000760: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00000770: 0043 0000 0073 2c00 0000 7c00 6a00 7214  .C...s,...|.j.r.
-00000780: 6401 7c00 6a01 9b00 6402 7c00 6a02 9b00  d.|.j...d.|.j...
-00000790: 9d03 7c00 6a01 7c00 6a00 6403 9c03 6901  ..|.j.|.j.d...i.
-000007a0: 5300 6900 5300 2904 4e5a 0970 7562 6c69  S.i.S.).NZ.publi
-000007b0: 634b 6579 fa01 2329 0372 0f00 0000 da05  cKey..#).r......
-000007c0: 6f77 6e65 725a 0c70 7562 6c69 634b 6579  ownerZ.publicKey
-000007d0: 5065 6d29 0372 1700 0000 720f 0000 0072  Pem).r....r....r
-000007e0: 1800 0000 722b 0000 0072 0b00 0000 720b  ....r+...r....r.
-000007f0: 0000 0072 0c00 0000 7221 0000 004e 0000  ...r....r!...N..
-00000800: 0073 1000 0000 0601 0202 1001 0401 0401  .s..............
-00000810: 04fd 04ff 0407 7a17 4163 746f 722e 5f62  ......z.Actor._b
-00000820: 7569 6c64 5f70 7562 6c69 635f 6b65 7963  uild_public_keyc
-00000830: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000840: 0300 0000 4300 0000 7390 0000 0069 007d  ....C...s....i.}
-00000850: 027c 0174 006a 016b 0272 097c 0253 007c  .|.t.j.k.r.|.S.|
-00000860: 006a 0272 127c 006a 027c 0264 013c 006e  .j.r.|.j.|.d.<.n
-00000870: 057c 006a 037c 0264 013c 007c 006a 0472  .|.j.|.d.<.|.j.r
-00000880: 207c 006a 047c 0264 023c 006e 057c 006a   |.j.|.d.<.n.|.j
-00000890: 037c 0264 023c 007c 0174 006a 056b 0372  .|.d.<.|.t.j.k.r
-000008a0: 2c7c 0253 007c 00a0 06a1 007d 037c 0372  ,|.S.|.....}.|.r
-000008b0: 367c 037c 0264 033c 007c 006a 0772 3e7c  6|.|.d.<.|.j.r>|
-000008c0: 006a 077c 0264 043c 007c 006a 0872 467c  .j.|.d.<.|.j.rF|
-000008d0: 006a 087c 0264 053c 007c 0253 0029 064e  .j.|.d.<.|.S.).N
-000008e0: 7213 0000 0072 1400 0000 da09 656e 6470  r....r......endp
-000008f0: 6f69 6e74 7372 1500 0000 7216 0000 0029  ointsr....r....)
-00000900: 0972 0500 0000 7223 0000 0072 1300 0000  .r....r#...r....
-00000910: 720f 0000 0072 1400 0000 da05 4f57 4e45  r....r......OWNE
-00000920: 52da 155f 6275 696c 645f 7573 6572 5f65  R.._build_user_e
-00000930: 6e64 706f 696e 7473 7215 0000 0072 1600  ndpointsr....r..
-00000940: 0000 2904 7225 0000 0072 1f00 0000 7226  ..).r%...r....r&
-00000950: 0000 0072 2e00 0000 720b 0000 0072 0b00  ...r....r....r..
-00000960: 0000 720c 0000 0072 2200 0000 5900 0000  ..r....r"...Y...
-00000970: 7326 0000 0004 010a 0204 0106 020c 010a  s&..............
-00000980: 0206 020c 010a 020a 0204 0108 0204 0108  ................
-00000990: 0106 020a 0106 010a 0104 027a 1641 6374  ...........z.Act
-000009a0: 6f72 2e5f 6275 696c 645f 656e 6470 6f69  or._build_endpoi
-000009b0: 6e74 7363 0100 0000 0000 0000 0000 0000  ntsc............
-000009c0: 0200 0000 0300 0000 4300 0000 7328 0000  ........C...s(..
-000009d0: 0069 007d 017c 006a 0072 0a7c 006a 007c  .i.}.|.j.r.|.j.|
-000009e0: 0164 013c 007c 006a 0172 127c 006a 017c  .d.<.|.j.r.|.j.|
-000009f0: 0164 023c 007c 0153 0029 034e da0b 6576  .d.<.|.S.).N..ev
-00000a00: 656e 7453 6f75 7263 65da 0870 726f 7879  entSource..proxy
-00000a10: 5572 6c29 0272 1900 0000 721a 0000 0029  Url).r....r....)
-00000a20: 0272 2500 0000 722e 0000 0072 0b00 0000  .r%...r....r....
-00000a30: 720b 0000 0072 0c00 0000 7230 0000 0077  r....r....r0...w
-00000a40: 0000 0073 0c00 0000 0401 0601 0a01 0601  ...s............
-00000a50: 0a01 0401 7a1b 4163 746f 722e 5f62 7569  ....z.Actor._bui
-00000a60: 6c64 5f75 7365 725f 656e 6470 6f69 6e74  ld_user_endpoint
-00000a70: 7329 1dda 085f 5f6e 616d 655f 5fda 0a5f  s)...__name__.._
-00000a80: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000a90: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00000aa0: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
-00000ab0: 696f 6e73 5f5f 7210 0000 0072 1100 0000  ions__r....r....
-00000ac0: 7203 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00000ad0: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
-00000ae0: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-00000af0: 0000 721b 0000 0072 1c00 0000 da04 6469  ..r....r......di
-00000b00: 6374 721d 0000 0072 0500 0000 da06 5055  ctr....r......PU
-00000b10: 424c 4943 7229 0000 0072 2000 0000 7221  BLICr)...r ...r!
-00000b20: 0000 0072 2200 0000 7230 0000 0072 0b00  ...r"...r0...r..
-00000b30: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000b40: 0072 0e00 0000 1100 0000 732c 0000 000a  .r........s,....
-00000b50: 0004 0208 020c 0110 0110 0110 0110 0110  ................
-00000b60: 0110 0110 0110 0110 0110 0110 0210 0110  ................
-00000b70: 010e 0208 1f08 0908 0b0c 1e72 0e00 0000  ...........r....
-00000b80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000b90: 0003 0000 0040 0000 0073 6000 0000 6500  .....@...s`...e.
-00000ba0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
-00000bb0: 6402 5a05 6506 6402 4200 6504 6403 3c00  d.Z.e.d.B.e.d.<.
-00000bc0: 6404 5a07 6508 6504 6405 3c00 6402 5a09  d.Z.e.e.d.<.d.Z.
-00000bd0: 6503 6402 4200 6504 6406 3c00 6402 5a0a  e.d.B.e.d.<.d.Z.
-00000be0: 6503 6402 4200 6504 6407 3c00 6408 650b  e.d.B.e.d.<.d.e.
-00000bf0: 6602 6409 640a 8404 5a0c 6402 5300 290b  f.d.d...Z.d.S.).
-00000c00: da11 4f72 6465 7265 6443 6f6c 6c65 6374  ..OrderedCollect
-00000c10: 696f 6e72 0f00 0000 4e72 2400 0000 7201  ionr....Nr$...r.
-00000c20: 0000 00da 0563 6f75 6e74 da05 6669 7273  .....count..firs
-00000c30: 74da 046c 6173 7472 0a00 0000 6301 0000  t..lastr....c...
-00000c40: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00000c50: 0043 0000 0073 4600 0000 6401 7c00 6a00  .C...sF...d.|.j.
-00000c60: 7c00 6a01 6402 6403 9c04 7d01 7c00 6a02  |.j.d.d...}.|.j.
-00000c70: 7211 7c00 6a02 7c01 6404 3c00 7c00 6a03  r.|.j.|.d.<.|.j.
-00000c80: 7219 7c00 6a03 7c01 6405 3c00 7c00 6a04  r.|.j.|.d.<.|.j.
-00000c90: 7221 7c00 6a04 7c01 6406 3c00 7c01 5300  r!|.j.|.d.<.|.S.
-00000ca0: 2907 4e72 2a00 0000 723b 0000 0029 0472  ).Nr*...r;...).r
-00000cb0: 1e00 0000 720f 0000 00da 0a74 6f74 616c  ....r......total
-00000cc0: 4974 656d 7372 1000 0000 da0c 6f72 6465  Itemsr......orde
-00000cd0: 7265 6449 7465 6d73 723d 0000 0072 3e00  redItemsr=...r>.
-00000ce0: 0000 2905 720f 0000 0072 3c00 0000 7224  ..).r....r<...r$
-00000cf0: 0000 0072 3d00 0000 723e 0000 00a9 0272  ...r=...r>.....r
-00000d00: 2500 0000 7226 0000 0072 0b00 0000 720b  %...r&...r....r.
-00000d10: 0000 0072 0c00 0000 7229 0000 0088 0000  ...r....r)......
-00000d20: 0073 1800 0000 0202 0401 0401 0201 06fc  .s..............
-00000d30: 0607 0a01 0602 0a01 0602 0a01 0402 7a17  ..............z.
-00000d40: 4f72 6465 7265 6443 6f6c 6c65 6374 696f  OrderedCollectio
-00000d50: 6e2e 6275 696c 6429 0d72 3300 0000 7234  n.build).r3...r4
-00000d60: 0000 0072 3500 0000 7237 0000 0072 3800  ...r5...r7...r8.
-00000d70: 0000 7224 0000 00da 046c 6973 7472 3c00  ..r$.....listr<.
-00000d80: 0000 da03 696e 7472 3d00 0000 723e 0000  ....intr=...r>..
-00000d90: 0072 3900 0000 7229 0000 0072 0b00 0000  .r9...r)...r....
-00000da0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000db0: 3b00 0000 8000 0000 730e 0000 000a 0008  ;.......s.......
-00000dc0: 0210 010c 0110 0110 0112 0272 3b00 0000  ...........r;...
-00000dd0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000de0: 0003 0000 0040 0000 0073 5400 0000 6500  .....@...sT...e.
-00000df0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
-00000e00: 6505 6504 6402 3c00 6503 6504 6403 3c00  e.e.d.<.e.e.d.<.
-00000e10: 6404 5a06 6503 6404 4200 6504 6405 3c00  d.Z.e.d.B.e.d.<.
-00000e20: 6404 5a07 6503 6404 4200 6504 6406 3c00  d.Z.e.d.B.e.d.<.
-00000e30: 6407 6508 6602 6408 6409 8404 5a09 6404  d.e.f.d.d...Z.d.
-00000e40: 5300 290a da15 4f72 6465 7265 6443 6f6c  S.)...OrderedCol
-00000e50: 6c65 6374 696f 6e50 6167 6572 0f00 0000  lectionPager....
-00000e60: 7224 0000 00da 0770 6172 745f 6f66 4eda  r$.....part_ofN.
-00000e70: 046e 6578 74da 0470 7265 7672 0a00 0000  .next..prevr....
-00000e80: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000e90: 0006 0000 0043 0000 0073 3a00 0000 6401  .....C...s:...d.
-00000ea0: 7c00 6a00 7c00 6a01 7c00 6a02 6402 6403  |.j.|.j.|.j.d.d.
-00000eb0: 9c05 7d01 7c00 6a03 7213 7c00 6a03 7c01  ..}.|.j.r.|.j.|.
-00000ec0: 6404 3c00 7c00 6a04 721b 7c00 6a04 7c01  d.<.|.j.r.|.j.|.
-00000ed0: 6405 3c00 7c01 5300 2906 4e72 2a00 0000  d.<.|.S.).Nr*...
-00000ee0: 7244 0000 0029 0572 1e00 0000 720f 0000  rD...).r....r...
-00000ef0: 005a 0670 6172 744f 6672 4000 0000 7210  .Z.partOfr@...r.
-00000f00: 0000 0072 4600 0000 7247 0000 0029 0572  ...rF...rG...).r
-00000f10: 0f00 0000 7245 0000 0072 2400 0000 7246  ....rE...r$...rF
-00000f20: 0000 0072 4700 0000 7241 0000 0072 0b00  ...rG...rA...r..
-00000f30: 0000 720b 0000 0072 0c00 0000 7229 0000  ..r....r....r)..
-00000f40: 00a4 0000 0073 1600 0000 0202 0401 0401  .....s..........
-00000f50: 0401 0201 06fb 0608 0a01 0602 0a01 0402  ................
-00000f60: 7a1b 4f72 6465 7265 6443 6f6c 6c65 6374  z.OrderedCollect
-00000f70: 696f 6e50 6167 652e 6275 696c 6429 0a72  ionPage.build).r
-00000f80: 3300 0000 7234 0000 0072 3500 0000 7237  3...r4...r5...r7
-00000f90: 0000 0072 3800 0000 7242 0000 0072 4600  ...r8...rB...rF.
-00000fa0: 0000 7247 0000 0072 3900 0000 7229 0000  ..rG...r9...r)..
-00000fb0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000fc0: 720c 0000 0072 4400 0000 9c00 0000 730e  r....rD.......s.
-00000fd0: 0000 000a 0008 0208 0108 0110 0110 0112  ................
-00000fe0: 0272 4400 0000 4e29 10da 0b64 6174 6163  .rD...N)...datac
-00000ff0: 6c61 7373 6573 7202 0000 00da 0674 7970  lassesr......typ
-00001000: 696e 6772 0300 0000 7204 0000 00da 0c62  ingr....r......b
-00001010: 6f76 696e 652e 7479 7065 7372 0500 0000  ovine.typesr....
-00001020: da10 6163 7469 7669 7479 5f66 6163 746f  ..activity_facto
-00001030: 7279 7207 0000 00da 0e6f 626a 6563 745f  ryr......object_
-00001040: 6661 6374 6f72 7972 0800 0000 7239 0000  factoryr....r9..
-00001050: 0072 0d00 0000 720e 0000 0072 3b00 0000  .r....r....r;...
-00001060: 7244 0000 0072 0b00 0000 720b 0000 0072  rD...r....r....r
-00001070: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-00001080: 6c65 3e01 0000 0073 2000 0000 0c00 1001  le>....s .......
-00001090: 0c02 0c02 0c01 0203 0201 02ff 0a02 0afe  ................
-000010a0: 0207 1001 026e 1001 021b 1401            .....n......
+000000b0: 640f 6410 8400 6410 8302 8301 5a0f 6501  d.d...d.....Z.e.
+000000c0: 4700 6411 6412 8400 6412 8302 8301 5a10  G.d.d...d.....Z.
+000000d0: 6413 5300 2914 e900 0000 0029 01da 0964  d.S.)......)...d
+000000e0: 6174 6163 6c61 7373 2902 da08 4f70 7469  ataclass)...Opti
+000000f0: 6f6e 616c da05 5475 706c 6529 01da 0a56  onal..Tuple)...V
+00000100: 6973 6962 696c 6974 79e9 0100 0000 2901  isibility.....).
+00000110: da0f 4163 7469 7669 7479 4661 6374 6f72  ..ActivityFactor
+00000120: 7929 01da 0d4f 626a 6563 7446 6163 746f  y)...ObjectFacto
+00000130: 7279 da0c 6163 746f 725f 6f62 6a65 6374  ry..actor_object
+00000140: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
+00000150: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00000160: 0073 1200 0000 7400 7c00 8301 7401 7c00  .s....t.|...t.|.
+00000170: 6401 8d01 6602 5300 2902 7a36 4275 696c  d...f.S.).z6Buil
+00000180: 6473 2061 6374 6976 6974 7920 616e 6420  ds activity and 
+00000190: 6f62 6a65 6374 2066 6163 746f 7269 6573  object factories
+000001a0: 2066 726f 6d20 6163 746f 7220 6f62 6a65   from actor obje
+000001b0: 6374 2901 5a11 6163 746f 725f 696e 666f  ct).Z.actor_info
+000001c0: 726d 6174 696f 6e29 0272 0700 0000 7208  rmation).r....r.
+000001d0: 0000 0029 0172 0900 0000 a900 720b 0000  ...).r......r...
+000001e0: 00fa 542f 776f 6f64 7065 636b 6572 2f73  ..T/woodpecker/s
+000001f0: 7263 2f63 6f64 6562 6572 672e 6f72 672f  rc/codeberg.org/
+00000200: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+00000210: 7669 6e65 2f62 6f76 696e 652f 6163 7469  vine/bovine/acti
+00000220: 7669 7479 7374 7265 616d 732f 5f5f 696e  vitystreams/__in
+00000230: 6974 5f5f 2e70 79da 1a66 6163 746f 7269  it__.py..factori
+00000240: 6573 5f66 6f72 5f61 6374 6f72 5f6f 626a  es_for_actor_obj
+00000250: 6563 740a 0000 0073 0200 0000 1204 720d  ect....s......r.
+00000260: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000270: 0000 0000 0300 0000 4000 0000 7324 0100  ........@...s$..
+00000280: 0065 005a 0164 005a 0255 0064 015a 0365  .e.Z.d.Z.U.d.Z.e
+00000290: 0465 0564 023c 0064 035a 0665 0465 0564  .e.d.<.d.Z.e.e.d
+000002a0: 043c 0064 055a 0765 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+000002b0: 063c 0064 055a 0965 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+000002c0: 073c 0064 055a 0a65 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+000002d0: 083c 0064 055a 0b65 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+000002e0: 093c 0064 055a 0c65 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+000002f0: 0a3c 0064 055a 0d65 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+00000300: 0b3c 0064 055a 0e65 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+00000310: 0c3c 0064 055a 0f65 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+00000320: 0d3c 0064 055a 1065 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+00000330: 0e3c 0064 055a 1165 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+00000340: 0f3c 0064 055a 1265 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+00000350: 103c 0064 055a 1365 0865 1419 0065 0564  .<.d.Z.e.e...e.d
+00000360: 113c 0064 055a 1565 0865 0419 0065 0564  .<.d.Z.e.e...e.d
+00000370: 123c 0065 166a 1766 0164 1364 1484 015a  .<.e.j.f.d.d...Z
+00000380: 1864 1564 1684 005a 1964 1764 1884 005a  .d.d...Z.d.d...Z
+00000390: 1a64 1964 1a84 005a 1b64 1b64 1c84 005a  .d.d...Z.d.d...Z
+000003a0: 1c64 0553 0029 1dda 0541 6374 6f72 7a37  .d.S.)...Actorz7
+000003b0: 4163 746f 7220 636c 6173 7320 7265 7072  Actor class repr
+000003c0: 6573 656e 7473 2074 6865 2062 6173 6963  esents the basic
+000003d0: 2041 6374 6976 6974 7953 7472 6561 6d73   ActivityStreams
+000003e0: 2061 6374 6f72 2eda 0269 645a 0650 6572   actor...idZ.Per
+000003f0: 736f 6eda 0474 7970 654e da04 6e61 6d65  son..typeN..name
+00000400: da12 7072 6566 6572 7265 645f 7573 6572  ..preferred_user
+00000410: 6e61 6d65 da05 696e 626f 78da 066f 7574  name..inbox..out
+00000420: 626f 78da 0966 6f6c 6c6f 7765 7273 da09  box..followers..
+00000430: 666f 6c6c 6f77 696e 67da 0a70 7562 6c69  following..publi
+00000440: 635f 6b65 79da 0f70 7562 6c69 635f 6b65  c_key..public_ke
+00000450: 795f 6e61 6d65 da0c 6576 656e 745f 736f  y_name..event_so
+00000460: 7572 6365 da09 7072 6f78 795f 7572 6cda  urce..proxy_url.
+00000470: 0773 756d 6d61 7279 da04 6963 6f6e da03  .summary..icon..
+00000480: 7572 6c63 0200 0000 0000 0000 0000 0000  urlc............
+00000490: 0500 0000 0400 0000 4300 0000 739c 0000  ........C...s...
+000004a0: 007c 00a0 00a1 007c 006a 017c 006a 0264  .|.....|.j.|.j.d
+000004b0: 019c 037c 00a0 03a1 00a5 017c 006a 047c  ...|.......|.j.|
+000004c0: 0164 028d 01a5 017d 027c 006a 0572 1c7c  .d.....}.|.j.r.|
+000004d0: 006a 057c 0264 033c 007c 0174 066a 076b  .j.|.d.<.|.t.j.k
+000004e0: 0272 237c 0253 007c 006a 0872 2c7c 006a  .r#|.S.|.j.r,|.j
+000004f0: 087c 0264 043c 006e 087c 006a 0572 347c  .|.d.<.n.|.j.r4|
+00000500: 006a 057c 0264 043c 007c 006a 097c 006a  .j.|.d.<.|.j.|.j
+00000510: 0a7c 006a 0b64 059c 03a0 0ca1 0044 005d  .|.j.d.......D.]
+00000520: 0c5c 027d 037d 047c 0464 0675 0172 4b7c  .\.}.}.|.d.u.rK|
+00000530: 047c 027c 033c 0071 3f7c 0253 0029 077a  .|.|.<.q?|.S.).z
+00000540: 3043 7265 6174 6573 2074 6865 206a 736f  0Creates the jso
+00000550: 6e2d 6c64 2072 6570 7265 7365 6e74 6174  n-ld representat
+00000560: 696f 6e20 6f66 2074 6865 2061 6374 6f72  ion of the actor
+00000570: 2e29 03fa 0840 636f 6e74 6578 7472 0f00  .)...@contextr..
+00000580: 0000 7210 0000 0029 01da 0a76 6973 6962  ..r....)...visib
+00000590: 696c 6974 795a 1170 7265 6665 7272 6564  ilityZ.preferred
+000005a0: 5573 6572 6e61 6d65 7211 0000 0029 0372  Usernamer....).r
+000005b0: 1b00 0000 721c 0000 0072 1d00 0000 4e29  ....r....r....N)
+000005c0: 0dda 0e5f 6275 696c 645f 636f 6e74 6578  ..._build_contex
+000005d0: 7472 0f00 0000 7210 0000 00da 115f 6275  tr....r......_bu
+000005e0: 696c 645f 7075 626c 6963 5f6b 6579 da10  ild_public_key..
+000005f0: 5f62 7569 6c64 5f65 6e64 706f 696e 7473  _build_endpoints
+00000600: 7212 0000 0072 0500 0000 da03 5745 4272  r....r......WEBr
+00000610: 1100 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
+00000620: 0000 00da 0569 7465 6d73 2905 da04 7365  .....items)...se
+00000630: 6c66 721f 0000 00da 0672 6573 756c 74da  lfr......result.
+00000640: 036b 6579 da05 7661 6c75 6572 0b00 0000  .key..valuer....
+00000650: 720b 0000 0072 0c00 0000 da05 6275 696c  r....r......buil
+00000660: 6426 0000 0073 3400 0000 0603 0401 0401  d&...s4.........
+00000670: 04fd 0604 02fc 0a05 04fb 0608 0a01 0a02  ................
+00000680: 0401 0602 0c01 0601 0a01 0403 0401 0401  ................
+00000690: 04fd 0404 0afc 0805 0801 0280 0402 7a0b  ..............z.
+000006a0: 4163 746f 722e 6275 696c 6463 0100 0000  Actor.buildc....
+000006b0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+000006c0: 4300 0000 7312 0000 007c 006a 0072 0764  C...s....|.j.r.d
+000006d0: 0164 0267 0253 0064 0153 0029 034e fa25  .d.g.S.d.S.).N.%
+000006e0: 6874 7470 733a 2f2f 7777 772e 7733 2e6f  https://www.w3.o
+000006f0: 7267 2f6e 732f 6163 7469 7669 7479 7374  rg/ns/activityst
+00000700: 7265 616d 737a 1c68 7474 7073 3a2f 2f77  reamsz.https://w
+00000710: 3369 642e 6f72 672f 7365 6375 7269 7479  3id.org/security
+00000720: 2f76 3129 0172 1700 0000 a901 7225 0000  /v1).r......r%..
+00000730: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000740: 7220 0000 0045 0000 0073 0a00 0000 0601  r ...E...s......
+00000750: 0202 0201 04fe 0405 7a14 4163 746f 722e  ........z.Actor.
+00000760: 5f62 7569 6c64 5f63 6f6e 7465 7874 6301  _build_contextc.
+00000770: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+00000780: 0000 0043 0000 0073 2c00 0000 7c00 6a00  ...C...s,...|.j.
+00000790: 7214 6401 7c00 6a01 9b00 6402 7c00 6a02  r.d.|.j...d.|.j.
+000007a0: 9b00 9d03 7c00 6a01 7c00 6a00 6403 9c03  ....|.j.|.j.d...
+000007b0: 6901 5300 6900 5300 2904 4e5a 0970 7562  i.S.i.S.).NZ.pub
+000007c0: 6c69 634b 6579 fa01 2329 0372 0f00 0000  licKey..#).r....
+000007d0: da05 6f77 6e65 725a 0c70 7562 6c69 634b  ..ownerZ.publicK
+000007e0: 6579 5065 6d29 0372 1700 0000 720f 0000  eyPem).r....r...
+000007f0: 0072 1800 0000 722b 0000 0072 0b00 0000  .r....r+...r....
+00000800: 720b 0000 0072 0c00 0000 7221 0000 004e  r....r....r!...N
+00000810: 0000 0073 1000 0000 0601 0202 1001 0401  ...s............
+00000820: 0401 04fd 04ff 0407 7a17 4163 746f 722e  ........z.Actor.
+00000830: 5f62 7569 6c64 5f70 7562 6c69 635f 6b65  _build_public_ke
+00000840: 7963 0200 0000 0000 0000 0000 0000 0400  yc..............
+00000850: 0000 0300 0000 4300 0000 7390 0000 0069  ......C...s....i
+00000860: 007d 027c 0174 006a 016b 0272 097c 0253  .}.|.t.j.k.r.|.S
+00000870: 007c 006a 0272 127c 006a 027c 0264 013c  .|.j.r.|.j.|.d.<
+00000880: 006e 057c 006a 037c 0264 013c 007c 006a  .n.|.j.|.d.<.|.j
+00000890: 0472 207c 006a 047c 0264 023c 006e 057c  .r |.j.|.d.<.n.|
+000008a0: 006a 037c 0264 023c 007c 0174 006a 056b  .j.|.d.<.|.t.j.k
+000008b0: 0372 2c7c 0253 007c 00a0 06a1 007d 037c  .r,|.S.|.....}.|
+000008c0: 0372 367c 037c 0264 033c 007c 006a 0772  .r6|.|.d.<.|.j.r
+000008d0: 3e7c 006a 077c 0264 043c 007c 006a 0872  >|.j.|.d.<.|.j.r
+000008e0: 467c 006a 087c 0264 053c 007c 0253 0029  F|.j.|.d.<.|.S.)
+000008f0: 064e 7213 0000 0072 1400 0000 da09 656e  .Nr....r......en
+00000900: 6470 6f69 6e74 7372 1500 0000 7216 0000  dpointsr....r...
+00000910: 0029 0972 0500 0000 7223 0000 0072 1300  .).r....r#...r..
+00000920: 0000 720f 0000 0072 1400 0000 da05 4f57  ..r....r......OW
+00000930: 4e45 52da 155f 6275 696c 645f 7573 6572  NER.._build_user
+00000940: 5f65 6e64 706f 696e 7473 7215 0000 0072  _endpointsr....r
+00000950: 1600 0000 2904 7225 0000 0072 1f00 0000  ....).r%...r....
+00000960: 7226 0000 0072 2e00 0000 720b 0000 0072  r&...r....r....r
+00000970: 0b00 0000 720c 0000 0072 2200 0000 5900  ....r....r"...Y.
+00000980: 0000 7326 0000 0004 010a 0204 0106 020c  ..s&............
+00000990: 010a 0206 020c 010a 020a 0204 0108 0204  ................
+000009a0: 0108 0106 020a 0106 010a 0104 027a 1641  .............z.A
+000009b0: 6374 6f72 2e5f 6275 696c 645f 656e 6470  ctor._build_endp
+000009c0: 6f69 6e74 7363 0100 0000 0000 0000 0000  ointsc..........
+000009d0: 0000 0200 0000 0300 0000 4300 0000 7328  ..........C...s(
+000009e0: 0000 0069 007d 017c 006a 0072 0a7c 006a  ...i.}.|.j.r.|.j
+000009f0: 007c 0164 013c 007c 006a 0172 127c 006a  .|.d.<.|.j.r.|.j
+00000a00: 017c 0164 023c 007c 0153 0029 034e da0b  .|.d.<.|.S.).N..
+00000a10: 6576 656e 7453 6f75 7263 65da 0870 726f  eventSource..pro
+00000a20: 7879 5572 6c29 0272 1900 0000 721a 0000  xyUrl).r....r...
+00000a30: 0029 0272 2500 0000 722e 0000 0072 0b00  .).r%...r....r..
+00000a40: 0000 720b 0000 0072 0c00 0000 7230 0000  ..r....r....r0..
+00000a50: 0077 0000 0073 0c00 0000 0401 0601 0a01  .w...s..........
+00000a60: 0601 0a01 0401 7a1b 4163 746f 722e 5f62  ......z.Actor._b
+00000a70: 7569 6c64 5f75 7365 725f 656e 6470 6f69  uild_user_endpoi
+00000a80: 6e74 7329 1dda 085f 5f6e 616d 655f 5fda  nts)...__name__.
+00000a90: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000aa0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00000ab0: 5f5f da03 7374 72da 0f5f 5f61 6e6e 6f74  __..str..__annot
+00000ac0: 6174 696f 6e73 5f5f 7210 0000 0072 1100  ations__r....r..
+00000ad0: 0000 7203 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000ae0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000af0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00000b00: 1a00 0000 721b 0000 0072 1c00 0000 da04  ....r....r......
+00000b10: 6469 6374 721d 0000 0072 0500 0000 da06  dictr....r......
+00000b20: 5055 424c 4943 7229 0000 0072 2000 0000  PUBLICr)...r ...
+00000b30: 7221 0000 0072 2200 0000 7230 0000 0072  r!...r"...r0...r
+00000b40: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
+00000b50: 0000 0072 0e00 0000 1100 0000 732c 0000  ...r........s,..
+00000b60: 000a 0004 0208 020c 0110 0110 0110 0110  ................
+00000b70: 0110 0110 0110 0110 0110 0110 0110 0210  ................
+00000b80: 0110 010e 0208 1f08 0908 0b0c 1e72 0e00  .............r..
+00000b90: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000ba0: 0000 0003 0000 0040 0000 0073 2c00 0000  .......@...s,...
+00000bb0: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
+00000bc0: 3c00 6505 6504 6402 3c00 6403 6506 6602  <.e.e.d.<.d.e.f.
+00000bd0: 6404 6405 8404 5a07 6406 5300 2907 da0a  d.d...Z.d.S.)...
+00000be0: 436f 6c6c 6563 7469 6f6e 720f 0000 0072  Collectionr....r
+00000bf0: 2400 0000 720a 0000 0063 0100 0000 0000  $...r....c......
+00000c00: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+00000c10: 0000 7312 0000 0064 017c 006a 007c 006a  ..s....d.|.j.|.j
+00000c20: 0164 0264 039c 0453 0029 044e 722a 0000  .d.d...S.).Nr*..
+00000c30: 0072 3b00 0000 2904 721e 0000 0072 0f00  .r;...).r....r..
+00000c40: 0000 7224 0000 0072 1000 0000 2902 720f  ..r$...r....).r.
+00000c50: 0000 0072 2400 0000 722b 0000 0072 0b00  ...r$...r+...r..
+00000c60: 0000 720b 0000 0072 0c00 0000 7229 0000  ..r....r....r)..
+00000c70: 0085 0000 0073 0a00 0000 0202 0401 0401  .....s..........
+00000c80: 0201 06fc 7a10 436f 6c6c 6563 7469 6f6e  ....z.Collection
+00000c90: 2e62 7569 6c64 4e29 0872 3300 0000 7234  .buildN).r3...r4
+00000ca0: 0000 0072 3500 0000 7237 0000 0072 3800  ...r5...r7...r8.
+00000cb0: 0000 da04 6c69 7374 7239 0000 0072 2900  ....listr9...r).
+00000cc0: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00000cd0: 0072 0c00 0000 723b 0000 0080 0000 0073  .r....r;.......s
+00000ce0: 0800 0000 0a00 0802 0801 1202 723b 0000  ............r;..
+00000cf0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000d00: 0000 0300 0000 4000 0000 7360 0000 0065  ......@...s`...e
+00000d10: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
+00000d20: 0064 025a 0565 0664 0242 0065 0464 033c  .d.Z.e.d.B.e.d.<
+00000d30: 0064 045a 0765 0865 0464 053c 0064 025a  .d.Z.e.e.d.<.d.Z
+00000d40: 0965 0364 0242 0065 0464 063c 0064 025a  .e.d.B.e.d.<.d.Z
+00000d50: 0a65 0364 0242 0065 0464 073c 0064 0865  .e.d.B.e.d.<.d.e
+00000d60: 0b66 0264 0964 0a84 045a 0c64 0253 0029  .f.d.d...Z.d.S.)
+00000d70: 0bda 114f 7264 6572 6564 436f 6c6c 6563  ...OrderedCollec
+00000d80: 7469 6f6e 720f 0000 004e 7224 0000 0072  tionr....Nr$...r
+00000d90: 0100 0000 da05 636f 756e 74da 0566 6972  ......count..fir
+00000da0: 7374 da04 6c61 7374 720a 0000 0063 0100  st..lastr....c..
+00000db0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00000dc0: 0000 4300 0000 7346 0000 0064 017c 006a  ..C...sF...d.|.j
+00000dd0: 007c 006a 0164 0264 039c 047d 017c 006a  .|.j.d.d...}.|.j
+00000de0: 0272 117c 006a 027c 0164 043c 007c 006a  .r.|.j.|.d.<.|.j
+00000df0: 0372 197c 006a 037c 0164 053c 007c 006a  .r.|.j.|.d.<.|.j
+00000e00: 0472 217c 006a 047c 0164 063c 007c 0153  .r!|.j.|.d.<.|.S
+00000e10: 0029 074e 722a 0000 0072 3d00 0000 2904  .).Nr*...r=...).
+00000e20: 721e 0000 0072 0f00 0000 da0a 746f 7461  r....r......tota
+00000e30: 6c49 7465 6d73 7210 0000 00da 0c6f 7264  lItemsr......ord
+00000e40: 6572 6564 4974 656d 7372 3f00 0000 7240  eredItemsr?...r@
+00000e50: 0000 0029 0572 0f00 0000 723e 0000 0072  ...).r....r>...r
+00000e60: 2400 0000 723f 0000 0072 4000 0000 a902  $...r?...r@.....
+00000e70: 7225 0000 0072 2600 0000 720b 0000 0072  r%...r&...r....r
+00000e80: 0b00 0000 720c 0000 0072 2900 0000 9600  ....r....r).....
+00000e90: 0000 7318 0000 0002 0204 0104 0102 0106  ..s.............
+00000ea0: fc06 070a 0106 020a 0106 020a 0104 027a  ...............z
+00000eb0: 174f 7264 6572 6564 436f 6c6c 6563 7469  .OrderedCollecti
+00000ec0: 6f6e 2e62 7569 6c64 290d 7233 0000 0072  on.build).r3...r
+00000ed0: 3400 0000 7235 0000 0072 3700 0000 7238  4...r5...r7...r8
+00000ee0: 0000 0072 2400 0000 723c 0000 0072 3e00  ...r$...r<...r>.
+00000ef0: 0000 da03 696e 7472 3f00 0000 7240 0000  ....intr?...r@..
+00000f00: 0072 3900 0000 7229 0000 0072 0b00 0000  .r9...r)...r....
+00000f10: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000f20: 3d00 0000 8e00 0000 730e 0000 000a 0008  =.......s.......
+00000f30: 0210 010c 0110 0110 0112 0272 3d00 0000  ...........r=...
+00000f40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000f50: 0003 0000 0040 0000 0073 5400 0000 6500  .....@...sT...e.
+00000f60: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+00000f70: 6505 6504 6402 3c00 6503 6504 6403 3c00  e.e.d.<.e.e.d.<.
+00000f80: 6404 5a06 6503 6404 4200 6504 6405 3c00  d.Z.e.d.B.e.d.<.
+00000f90: 6404 5a07 6503 6404 4200 6504 6406 3c00  d.Z.e.d.B.e.d.<.
+00000fa0: 6407 6508 6602 6408 6409 8404 5a09 6404  d.e.f.d.d...Z.d.
+00000fb0: 5300 290a da15 4f72 6465 7265 6443 6f6c  S.)...OrderedCol
+00000fc0: 6c65 6374 696f 6e50 6167 6572 0f00 0000  lectionPager....
+00000fd0: 7224 0000 00da 0770 6172 745f 6f66 4eda  r$.....part_ofN.
+00000fe0: 046e 6578 74da 0470 7265 7672 0a00 0000  .next..prevr....
+00000ff0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001000: 0006 0000 0043 0000 0073 3a00 0000 6401  .....C...s:...d.
+00001010: 7c00 6a00 7c00 6a01 7c00 6a02 6402 6403  |.j.|.j.|.j.d.d.
+00001020: 9c05 7d01 7c00 6a03 7213 7c00 6a03 7c01  ..}.|.j.r.|.j.|.
+00001030: 6404 3c00 7c00 6a04 721b 7c00 6a04 7c01  d.<.|.j.r.|.j.|.
+00001040: 6405 3c00 7c01 5300 2906 4e72 2a00 0000  d.<.|.S.).Nr*...
+00001050: 7245 0000 0029 0572 1e00 0000 720f 0000  rE...).r....r...
+00001060: 005a 0670 6172 744f 6672 4200 0000 7210  .Z.partOfrB...r.
+00001070: 0000 0072 4700 0000 7248 0000 0029 0572  ...rG...rH...).r
+00001080: 0f00 0000 7246 0000 0072 2400 0000 7247  ....rF...r$...rG
+00001090: 0000 0072 4800 0000 7243 0000 0072 0b00  ...rH...rC...r..
+000010a0: 0000 720b 0000 0072 0c00 0000 7229 0000  ..r....r....r)..
+000010b0: 00b2 0000 0073 1600 0000 0202 0401 0401  .....s..........
+000010c0: 0401 0201 06fb 0608 0a01 0602 0a01 0402  ................
+000010d0: 7a1b 4f72 6465 7265 6443 6f6c 6c65 6374  z.OrderedCollect
+000010e0: 696f 6e50 6167 652e 6275 696c 6429 0a72  ionPage.build).r
+000010f0: 3300 0000 7234 0000 0072 3500 0000 7237  3...r4...r5...r7
+00001100: 0000 0072 3800 0000 723c 0000 0072 4700  ...r8...r<...rG.
+00001110: 0000 7248 0000 0072 3900 0000 7229 0000  ..rH...r9...r)..
+00001120: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
+00001130: 720c 0000 0072 4500 0000 aa00 0000 730e  r....rE.......s.
+00001140: 0000 000a 0008 0208 0108 0110 0110 0112  ................
+00001150: 0272 4500 0000 4e29 11da 0b64 6174 6163  .rE...N)...datac
+00001160: 6c61 7373 6573 7202 0000 00da 0674 7970  lassesr......typ
+00001170: 696e 6772 0300 0000 7204 0000 00da 0c62  ingr....r......b
+00001180: 6f76 696e 652e 7479 7065 7372 0500 0000  ovine.typesr....
+00001190: da10 6163 7469 7669 7479 5f66 6163 746f  ..activity_facto
+000011a0: 7279 7207 0000 00da 0e6f 626a 6563 745f  ryr......object_
+000011b0: 6661 6374 6f72 7972 0800 0000 7239 0000  factoryr....r9..
+000011c0: 0072 0d00 0000 720e 0000 0072 3b00 0000  .r....r....r;...
+000011d0: 723d 0000 0072 4500 0000 720b 0000 0072  r=...rE...r....r
+000011e0: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
+000011f0: 3c6d 6f64 756c 653e 0100 0000 7324 0000  <module>....s$..
+00001200: 000c 0010 010c 020c 020c 0102 0302 0102  ................
+00001210: ff0a 020a fe02 0710 0102 6e10 0102 0d10  ..........n.....
+00001220: 0102 1b14 01                             .....
```

### Comparing `bovine-0.1.2/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc` & `bovine-0.1.3/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 4195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,266 +1,267 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 6310 0000  o.........Adc...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 6b10 0000  o.......*.Ndk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6501  d.l.m.Z.m.Z...e.
 00000050: 4700 6403 6404 8400 6404 8302 8301 5a06  G.d.d...d.....Z.
 00000060: 4700 6405 6406 8400 6406 8302 5a07 6407  G.d.d...d...Z.d.
 00000070: 5300 2908 e900 0000 0029 02da 0964 6174  S.)......)...dat
 00000080: 6163 6c61 7373 da05 6669 656c 6429 02da  aclass..field)..
 00000090: 084f 7074 696f 6e61 6cda 0353 6574 6300  .Optional..Setc.
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000000b0: 0000 0040 0000 0073 ee00 0000 6500 5a01  ...@...s....e.Z.
+000000b0: 0000 0040 0000 0073 f400 0000 6500 5a01  ...@...s....e.Z.
 000000c0: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
 000000d0: 3c00 6403 5a06 6507 6504 1900 6505 6404  <.d.Z.e.e...e.d.
 000000e0: 3c00 6403 5a08 6507 6504 1900 6505 6405  <.d.Z.e.e...e.d.
 000000f0: 3c00 6403 5a09 6507 6504 1900 6505 6406  <.d.Z.e.e...e.d.
 00000100: 3c00 6403 5a0a 6507 6504 1900 6505 6407  <.d.Z.e.e...e.d.
 00000110: 3c00 650b 650c 6408 8d01 5a0d 650e 6504  <.e.e.d...Z.e.e.
 00000120: 1900 6505 6409 3c00 650b 650c 6408 8d01  ..e.d.<.e.e.d...
 00000130: 5a0f 650e 6504 1900 6505 640a 3c00 6403  Z.e.e...e.d.<.d.
 00000140: 5a10 6507 6504 1900 6505 640b 3c00 6403  Z.e.e...e.d.<.d.
 00000150: 5a11 6507 6504 1900 6505 640c 3c00 6403  Z.e.e...e.d.<.d.
 00000160: 5a12 6507 6504 1900 6505 640d 3c00 6403  Z.e.e...e.d.<.d.
 00000170: 5a13 6507 6504 1900 6505 640e 3c00 6403  Z.e.e...e.d.<.d.
 00000180: 5a14 6507 6504 1900 6505 640f 3c00 6410  Z.e.e...e.d.<.d.
 00000190: 6411 8400 5a15 6412 6413 8400 5a16 6414  d...Z.d.d...Z.d.
-000001a0: 6415 8400 5a17 6403 5300 2916 da08 4163  d...Z.d.S.)...Ac
-000001b0: 7469 7669 7479 7a7e 4120 6461 7461 636c  tivityz~A datacl
-000001c0: 6173 7320 7265 7072 6573 656e 7469 6e67  ass representing
-000001d0: 2061 6e20 6041 6374 6976 6974 7953 7472   an `ActivityStr
-000001e0: 6561 6d73 2041 6374 6976 6974 790a 2020  eams Activity.  
-000001f0: 2020 3c68 7474 7073 3a2f 2f77 7777 2e77    <https://www.w
-00000200: 332e 6f72 672f 5452 2f61 6374 6976 6974  3.org/TR/activit
-00000210: 7973 7472 6561 6d73 2d76 6f63 6162 756c  ystreams-vocabul
-00000220: 6172 792f 2361 6374 6976 6974 792d 7479  ary/#activity-ty
-00000230: 7065 733e 605f da04 7479 7065 4eda 0561  pes>`_..typeN..a
-00000240: 6374 6f72 da09 666f 6c6c 6f77 6572 73da  ctor..followers.
-00000250: 0269 64da 0970 7562 6c69 7368 6564 2901  .id..published).
-00000260: da0f 6465 6661 756c 745f 6661 6374 6f72  ..default_factor
-00000270: 79da 0274 6fda 0263 63da 046e 616d 65da  y..to..cc..name.
-00000280: 0773 756d 6d61 7279 da07 636f 6e74 656e  .summary..conten
-00000290: 74da 0674 6172 6765 74da 066f 626a 6563  t..target..objec
-000002a0: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-000002b0: 0000 0300 0000 4300 0000 7324 0000 007c  ......C...s$...|
-000002c0: 006a 00a0 0164 01a1 0101 007c 006a 0272  .j...d.....|.j.r
-000002d0: 107c 006a 03a0 017c 006a 02a1 0101 007c  .|.j...|.j.....|
-000002e0: 0053 0029 027a 406d 616b 6573 2074 6865  .S.).z@makes the
-000002f0: 2061 6374 6976 6974 7920 7075 626c 6963   activity public
-00000300: 2c20 692e 652e 2070 7562 6c69 6320 696e  , i.e. public in
-00000310: 2074 6f20 616e 6420 666f 6c6c 6f77 6572   to and follower
-00000320: 7320 696e 2063 63fa 2c68 7474 7073 3a2f  s in cc.,https:/
-00000330: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
-00000340: 6374 6976 6974 7973 7472 6561 6d73 2350  ctivitystreams#P
-00000350: 7562 6c69 6329 0472 0d00 0000 da03 6164  ublic).r......ad
-00000360: 6472 0900 0000 720e 0000 00a9 01da 0473  dr....r........s
-00000370: 656c 66a9 0072 1800 0000 fa5c 2f77 6f6f  elf..r.....\/woo
-00000380: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-00000390: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
-000003a0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-000003b0: 7669 6e65 2f61 6374 6976 6974 7973 7472  vine/activitystr
-000003c0: 6561 6d73 2f61 6374 6976 6974 795f 6661  eams/activity_fa
-000003d0: 6374 6f72 792e 7079 da09 6173 5f70 7562  ctory.py..as_pub
-000003e0: 6c69 6319 0000 0073 0800 0000 0c02 0601  lic....s........
-000003f0: 0e01 0401 7a12 4163 7469 7669 7479 2e61  ....z.Activity.a
-00000400: 735f 7075 626c 6963 6301 0000 0000 0000  s_publicc.......
-00000410: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000420: 0073 2400 0000 7c00 6a00 720a 7c00 6a01  .s$...|.j.r.|.j.
-00000430: a002 7c00 6a00 a101 0100 7c00 6a03 a002  ..|.j.....|.j...
-00000440: 6401 a101 0100 7c00 5300 2902 7a42 6d61  d.....|.S.).zBma
-00000450: 6b65 7320 7468 6520 6163 7469 7669 7479  kes the activity
-00000460: 2075 6e6c 6973 7465 642c 2069 2e65 2e20   unlisted, i.e. 
-00000470: 7075 626c 6963 2069 6e20 6363 2061 6e64  public in cc and
-00000480: 2066 6f6c 6c6f 7765 7273 2069 6e20 746f   followers in to
-00000490: 7214 0000 0029 0472 0900 0000 720d 0000  r....).r....r...
-000004a0: 0072 1500 0000 720e 0000 0072 1600 0000  .r....r....r....
-000004b0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-000004c0: 0b61 735f 756e 6c69 7374 6564 2000 0000  .as_unlisted ...
-000004d0: 7308 0000 0006 020e 010c 0104 017a 1441  s............z.A
-000004e0: 6374 6976 6974 792e 6173 5f75 6e6c 6973  ctivity.as_unlis
-000004f0: 7465 6463 0100 0000 0000 0000 0000 0000  tedc............
-00000500: 0500 0000 0800 0000 4300 0000 73ae 0000  ........C...s...
-00000510: 0064 017c 006a 007c 006a 0174 027c 006a  .d.|.j.|.j.t.|.j
-00000520: 0383 0174 027c 006a 047c 006a 0318 0083  ...t.|.j.|.j....
-00000530: 0164 029c 057d 017c 006a 057c 006a 067c  .d...}.|.j.|.j.|
-00000540: 006a 077c 006a 087c 006a 097c 006a 0a7c  .j.|.j.|.j.|.j.|
-00000550: 006a 0b64 039c 077d 027c 0164 0419 0064  .j.d...}.|.d...d
-00000560: 0575 0172 3574 0c7c 0164 0419 0083 0164  .u.r5t.|.d.....d
-00000570: 066b 0272 357c 0164 043d 007c 0164 0719  .k.r5|.d.=.|.d..
-00000580: 0064 0575 0172 4674 0c7c 0164 0719 0083  .d.u.rFt.|.d....
-00000590: 0164 066b 0272 467c 0164 073d 007c 02a0  .d.k.rF|.d.=.|..
-000005a0: 0da1 0044 005d 0a5c 027d 037d 047c 0472  ...D.].\.}.}.|.r
-000005b0: 547c 047c 017c 033c 0071 4a7c 0153 0029  T|.|.|.<.qJ|.S.)
-000005c0: 087a 4163 6f6e 7665 7274 7320 7468 6520  .zAconverts the 
-000005d0: 6163 7469 7669 7479 2069 6e74 6f20 6120  activity into a 
-000005e0: 6469 6374 2c20 7468 6174 2063 616e 2062  dict, that can b
-000005f0: 6520 7365 7269 616c 697a 6564 2074 6f20  e serialized to 
-00000600: 4a53 4f4e 7a25 6874 7470 733a 2f2f 7777  JSONz%https://ww
-00000610: 772e 7733 2e6f 7267 2f6e 732f 6163 7469  w.w3.org/ns/acti
-00000620: 7669 7479 7374 7265 616d 7329 057a 0840  vitystreams).z.@
-00000630: 636f 6e74 6578 7472 0700 0000 7208 0000  contextr....r...
-00000640: 0072 0d00 0000 720e 0000 0029 0772 0a00  .r....r....).r..
-00000650: 0000 720b 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000660: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000670: 720d 0000 004e 7201 0000 0072 0e00 0000  r....Nr....r....
-00000680: 290e 7207 0000 0072 0800 0000 da04 6c69  ).r....r......li
-00000690: 7374 720d 0000 0072 0e00 0000 720a 0000  str....r....r...
-000006a0: 0072 0b00 0000 720f 0000 0072 1000 0000  .r....r....r....
-000006b0: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-000006c0: 036c 656e da05 6974 656d 7329 0572 1700  .len..items).r..
-000006d0: 0000 da06 7265 7375 6c74 5a0c 6578 7472  ....resultZ.extr
-000006e0: 615f 6669 656c 6473 da03 6b65 79da 0576  a_fields..key..v
-000006f0: 616c 7565 7218 0000 0072 1800 0000 7219  aluer....r....r.
-00000700: 0000 00da 0562 7569 6c64 2700 0000 732e  .....build'...s.
-00000710: 0000 0002 0304 0104 0108 010e 0106 fb04  ................
-00000720: 0904 0104 0104 0104 0104 0104 0106 f91c  ................
-00000730: 0a06 011c 0106 0110 0204 0108 0102 8004  ................
-00000740: 027a 0e41 6374 6976 6974 792e 6275 696c  .z.Activity.buil
-00000750: 6429 18da 085f 5f6e 616d 655f 5fda 0a5f  d)...__name__.._
-00000760: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000770: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00000780: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
-00000790: 696f 6e73 5f5f 7208 0000 0072 0400 0000  ions__r....r....
-000007a0: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-000007b0: 0300 0000 da03 7365 7472 0d00 0000 7205  ......setr....r.
-000007c0: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
-000007d0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-000007e0: 0072 1a00 0000 721b 0000 0072 2200 0000  .r....r....r"...
-000007f0: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000800: 1900 0000 7206 0000 0005 0000 0073 2200  ....r........s".
-00000810: 0000 0a00 0402 0803 1001 1001 1001 1001  ................
-00000820: 1601 1601 1002 1001 1001 1002 1001 0802  ................
-00000830: 0807 0c07 7206 0000 0063 0000 0000 0000  ....r....c......
-00000840: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00000850: 0000 7358 0000 0065 005a 0164 005a 0264  ..sX...e.Z.d.Z.d
-00000860: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
-00000870: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
-00000880: 005a 0764 0a64 0b84 005a 0864 0c64 0d84  .Z.d.d...Z.d.d..
-00000890: 005a 0964 0e64 0f84 005a 0a64 1064 1184  .Z.d.d...Z.d.d..
-000008a0: 005a 0b64 1264 1384 005a 0c64 1453 0029  .Z.d.d...Z.d.S.)
-000008b0: 15da 0f41 6374 6976 6974 7946 6163 746f  ...ActivityFacto
-000008c0: 7279 7a49 4261 7369 6320 6661 6374 6f72  ryzIBasic factor
-000008d0: 7920 666f 7220 4163 7469 7669 7479 206f  y for Activity o
-000008e0: 626a 6563 7473 2e0a 0a20 2020 2055 7361  bjects...    Usa
-000008f0: 6c6c 7920 6372 6561 7465 6420 6279 2061  lly created by a
-00000900: 2042 6f76 696e 6543 6c69 656e 7463 0200   BovineClientc..
-00000910: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000920: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
-00000930: 0064 0053 0029 014e 2901 da0b 696e 666f  .d.S.).N)...info
-00000940: 726d 6174 696f 6e29 0272 1700 0000 da11  rmation).r......
-00000950: 6163 746f 725f 696e 666f 726d 6174 696f  actor_informatio
-00000960: 6e72 1800 0000 7218 0000 0072 1900 0000  nr....r....r....
-00000970: da08 5f5f 696e 6974 5f5f 4c00 0000 7302  ..__init__L...s.
-00000980: 0000 000a 017a 1841 6374 6976 6974 7946  .....z.ActivityF
-00000990: 6163 746f 7279 2e5f 5f69 6e69 745f 5f63  actory.__init__c
-000009a0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000009b0: 0a00 0000 4b00 0000 f336 0000 0074 0064  ....K....6...t.d
-000009c0: 0764 017c 0164 0219 0074 017c 01a0 0264  .d.|.d...t.|...d
-000009d0: 0367 00a1 0283 0174 017c 01a0 0264 0467  .g.....t.|...d.g
-000009e0: 00a1 0283 017c 0164 059c 057c 02a4 018e  .....|.d...|....
-000009f0: 0153 0029 087a 2341 6374 6976 6974 7920  .S.).z#Activity 
-00000a00: 6f66 2074 7970 6520 4372 6561 7465 2066  of type Create f
-00000a10: 726f 6d20 4f62 6a65 6374 5a06 4372 6561  rom ObjectZ.Crea
-00000a20: 7465 da0c 6174 7472 6962 7574 6564 546f  te..attributedTo
-00000a30: 720e 0000 0072 0d00 0000 a905 7207 0000  r....r......r...
-00000a40: 0072 0800 0000 720e 0000 0072 0d00 0000  .r....r....r....
-00000a50: 7213 0000 004e 7218 0000 00a9 0372 0600  r....Nr......r..
-00000a60: 0000 7229 0000 00da 0367 6574 a903 7217  ..r).....get..r.
-00000a70: 0000 00da 036f 626a da06 6b77 6172 6773  .....obj..kwargs
-00000a80: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000a90: 0663 7265 6174 654f 0000 00f3 1200 0000  .createO........
-00000aa0: 0402 0201 0601 0e01 0e01 0201 04fb 0206  ................
-00000ab0: 06fa 7a16 4163 7469 7669 7479 4661 6374  ..z.ActivityFact
-00000ac0: 6f72 792e 6372 6561 7465 6302 0000 0000  ory.createc.....
-00000ad0: 0000 0000 0000 0003 0000 000a 0000 004b  ...............K
-00000ae0: 0000 0072 2e00 0000 2908 7a23 4163 7469  ...r....).z#Acti
-00000af0: 7669 7479 206f 6620 7479 7065 2055 7064  vity of type Upd
-00000b00: 6174 6520 6672 6f6d 204f 626a 6563 745a  ate from ObjectZ
-00000b10: 0655 7064 6174 6572 2f00 0000 720e 0000  .Updater/...r...
-00000b20: 0072 0d00 0000 7230 0000 004e 7218 0000  .r....r0...Nr...
-00000b30: 0072 3100 0000 7233 0000 0072 1800 0000  .r1...r3...r....
-00000b40: 7218 0000 0072 1900 0000 da06 7570 6461  r....r......upda
-00000b50: 7465 5a00 0000 7237 0000 007a 1641 6374  teZ...r7...z.Act
-00000b60: 6976 6974 7946 6163 746f 7279 2e75 7064  ivityFactory.upd
-00000b70: 6174 6563 0200 0000 0000 0000 0000 0000  atec............
-00000b80: 0300 0000 0600 0000 4b00 0000 f31c 0000  ........K.......
-00000b90: 0074 0064 0564 017c 006a 0164 0219 007c  .t.d.d.|.j.d...|
-00000ba0: 0164 039c 037c 02a4 018e 0153 0029 067a  .d...|.....S.).z
-00000bb0: 0f4c 696b 6520 666f 7220 7461 7267 6574  .Like for target
-00000bc0: 5a04 4c69 6b65 720a 0000 00a9 0372 0700  Z.Liker......r..
-00000bd0: 0000 7208 0000 0072 1300 0000 4e72 1800  ..r....r....Nr..
-00000be0: 0000 a902 7206 0000 0072 2b00 0000 a903  ....r....r+.....
-00000bf0: 7217 0000 0072 1200 0000 7235 0000 0072  r....r....r5...r
-00000c00: 1800 0000 7218 0000 0072 1900 0000 da04  ....r....r......
-00000c10: 6c69 6b65 6500 0000 f30a 0000 0004 020c  likee...........
-00000c20: 0104 ff02 0106 ff7a 1441 6374 6976 6974  .......z.Activit
-00000c30: 7946 6163 746f 7279 2e6c 696b 6563 0200  yFactory.likec..
-00000c40: 0000 0000 0000 0000 0000 0300 0000 0600  ................
-00000c50: 0000 4b00 0000 7239 0000 0029 067a 1144  ..K...r9...).z.D
-00000c60: 656c 6574 6520 666f 7220 7461 7267 6574  elete for target
-00000c70: da06 4465 6c65 7465 720a 0000 0072 3a00  ..Deleter....r:.
-00000c80: 0000 4e72 1800 0000 723b 0000 0072 3c00  ..Nr....r;...r<.
-00000c90: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000ca0: 00da 0664 656c 6574 656b 0000 0072 3e00  ...deletek...r>.
-00000cb0: 0000 7a16 4163 7469 7669 7479 4661 6374  ..z.ActivityFact
-00000cc0: 6f72 792e 6465 6c65 7465 6302 0000 0000  ory.deletec.....
-00000cd0: 0000 0000 0000 0003 0000 0006 0000 004b  ...............K
-00000ce0: 0000 0072 3900 0000 2906 7a11 4163 6365  ...r9...).z.Acce
-00000cf0: 7074 2066 6f72 206f 626a 6563 74da 0641  pt for object..A
-00000d00: 6363 6570 7472 0a00 0000 723a 0000 004e  cceptr....r:...N
-00000d10: 7218 0000 0072 3b00 0000 7233 0000 0072  r....r;...r3...r
-00000d20: 1800 0000 7218 0000 0072 1900 0000 da06  ....r....r......
-00000d30: 6163 6365 7074 7100 0000 723e 0000 007a  acceptq...r>...z
-00000d40: 1641 6374 6976 6974 7946 6163 746f 7279  .ActivityFactory
-00000d50: 2e61 6363 6570 7463 0200 0000 0000 0000  .acceptc........
-00000d60: 0000 0000 0300 0000 0600 0000 4b00 0000  ............K...
-00000d70: 7239 0000 0029 067a 1152 656a 6563 7420  r9...).z.Reject 
-00000d80: 666f 7220 6f62 6a65 6374 5a06 5265 6a65  for objectZ.Reje
-00000d90: 6374 720a 0000 0072 3a00 0000 4e72 1800  ctr....r:...Nr..
-00000da0: 0000 723b 0000 0072 3300 0000 7218 0000  ..r;...r3...r...
-00000db0: 0072 1800 0000 7219 0000 00da 0672 656a  .r....r......rej
-00000dc0: 6563 7477 0000 0072 3e00 0000 7a16 4163  ectw...r>...z.Ac
-00000dd0: 7469 7669 7479 4661 6374 6f72 792e 7265  tivityFactory.re
-00000de0: 6a65 6374 6302 0000 0000 0000 0000 0000  jectc...........
-00000df0: 0003 0000 0009 0000 004b 0000 0073 2800  .........K...s(.
-00000e00: 0000 7400 6406 6401 7c00 6a01 6402 1900  ..t.d.d.|.j.d...
-00000e10: 7c01 7c00 6a01 a002 6403 6700 a102 6404  |.|.j...d.g...d.
-00000e20: 9c04 7c02 a401 8e01 5300 2907 7a13 416e  ..|.....S.).z.An
-00000e30: 6e6f 756e 6365 2066 6f72 206f 626a 6563  nounce for objec
-00000e40: 745a 0841 6e6e 6f75 6e63 6572 0a00 0000  tZ.Announcer....
-00000e50: 7209 0000 0029 0472 0700 0000 7208 0000  r....).r....r...
-00000e60: 0072 1300 0000 7209 0000 004e 7218 0000  .r....r....Nr...
-00000e70: 0029 0372 0600 0000 722b 0000 0072 3200  .).r....r+...r2.
-00000e80: 0000 7233 0000 0072 1800 0000 7218 0000  ..r3...r....r...
-00000e90: 0072 1900 0000 da08 616e 6e6f 756e 6365  .r......announce
-00000ea0: 7d00 0000 7310 0000 0004 0202 0108 0102  }...s...........
-00000eb0: 010c 0104 fc02 0506 fb7a 1841 6374 6976  .........z.Activ
-00000ec0: 6974 7946 6163 746f 7279 2e61 6e6e 6f75  ityFactory.annou
-00000ed0: 6e63 6563 0200 0000 0000 0000 0000 0000  ncec............
-00000ee0: 0300 0000 0700 0000 4b00 0000 7324 0000  ........K...s$..
-00000ef0: 0074 0064 0564 017c 006a 0164 0219 007c  .t.d.d.|.j.d...|
-00000f00: 0174 027c 0167 0183 0164 039c 047c 02a4  .t.|.g...d...|..
-00000f10: 018e 0153 0029 067a 1146 6f6c 6c6f 7720  ...S.).z.Follow 
-00000f20: 666f 7220 6f62 6a65 6374 5a06 466f 6c6c  for objectZ.Foll
-00000f30: 6f77 720a 0000 0029 0472 0700 0000 7208  owr....).r....r.
-00000f40: 0000 0072 1300 0000 720d 0000 004e 7218  ...r....r....Nr.
-00000f50: 0000 0029 0372 0600 0000 722b 0000 0072  ...).r....r+...r
-00000f60: 2900 0000 7233 0000 0072 1800 0000 7218  )...r3...r....r.
-00000f70: 0000 0072 1900 0000 da06 666f 6c6c 6f77  ...r......follow
-00000f80: 8700 0000 7310 0000 0004 0202 0108 0102  ....s...........
-00000f90: 0108 0104 fc02 0506 fb7a 1641 6374 6976  .........z.Activ
-00000fa0: 6974 7946 6163 746f 7279 2e66 6f6c 6c6f  ityFactory.follo
-00000fb0: 774e 290d 7223 0000 0072 2400 0000 7225  wN).r#...r$...r%
-00000fc0: 0000 0072 2600 0000 722d 0000 0072 3600  ...r&...r-...r6.
-00000fd0: 0000 7238 0000 0072 3d00 0000 7240 0000  ..r8...r=...r@..
-00000fe0: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
-00000ff0: 7245 0000 0072 1800 0000 7218 0000 0072  rE...r....r....r
-00001000: 1800 0000 7219 0000 0072 2a00 0000 4700  ....r....r*...G.
-00001010: 0000 7316 0000 0008 0004 0108 0408 0308  ..s.............
-00001020: 0b08 0b08 0608 0608 0608 060c 0a72 2a00  .............r*.
-00001030: 0000 4e29 08da 0b64 6174 6163 6c61 7373  ..N)...dataclass
-00001040: 6573 7202 0000 0072 0300 0000 da06 7479  esr....r......ty
-00001050: 7069 6e67 7204 0000 0072 0500 0000 7206  pingr....r....r.
-00001060: 0000 0072 2a00 0000 7218 0000 0072 1800  ...r*...r....r..
-00001070: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
-00001080: 6f64 756c 653e 0100 0000 730a 0000 0010  odule>....s.....
-00001090: 0010 0102 0310 0112 41                   ........A
+000001a0: 6517 6602 6415 6416 8404 5a18 6403 5300  e.f.d.d...Z.d.S.
+000001b0: 2917 da08 4163 7469 7669 7479 7a7e 4120  )...Activityz~A 
+000001c0: 6461 7461 636c 6173 7320 7265 7072 6573  dataclass repres
+000001d0: 656e 7469 6e67 2061 6e20 6041 6374 6976  enting an `Activ
+000001e0: 6974 7953 7472 6561 6d73 2041 6374 6976  ityStreams Activ
+000001f0: 6974 790a 2020 2020 3c68 7474 7073 3a2f  ity.    <https:/
+00000200: 2f77 7777 2e77 332e 6f72 672f 5452 2f61  /www.w3.org/TR/a
+00000210: 6374 6976 6974 7973 7472 6561 6d73 2d76  ctivitystreams-v
+00000220: 6f63 6162 756c 6172 792f 2361 6374 6976  ocabulary/#activ
+00000230: 6974 792d 7479 7065 733e 605f da04 7479  ity-types>`_..ty
+00000240: 7065 4eda 0561 6374 6f72 da09 666f 6c6c  peN..actor..foll
+00000250: 6f77 6572 73da 0269 64da 0970 7562 6c69  owers..id..publi
+00000260: 7368 6564 2901 da0f 6465 6661 756c 745f  shed)...default_
+00000270: 6661 6374 6f72 79da 0274 6fda 0263 63da  factory..to..cc.
+00000280: 046e 616d 65da 0773 756d 6d61 7279 da07  .name..summary..
+00000290: 636f 6e74 656e 74da 0674 6172 6765 74da  content..target.
+000002a0: 066f 626a 6563 7463 0100 0000 0000 0000  .objectc........
+000002b0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+000002c0: 7324 0000 007c 006a 00a0 0164 01a1 0101  s$...|.j...d....
+000002d0: 007c 006a 0272 107c 006a 03a0 017c 006a  .|.j.r.|.j...|.j
+000002e0: 02a1 0101 007c 0053 0029 027a 406d 616b  .....|.S.).z@mak
+000002f0: 6573 2074 6865 2061 6374 6976 6974 7920  es the activity 
+00000300: 7075 626c 6963 2c20 692e 652e 2070 7562  public, i.e. pub
+00000310: 6c69 6320 696e 2074 6f20 616e 6420 666f  lic in to and fo
+00000320: 6c6c 6f77 6572 7320 696e 2063 63fa 2c68  llowers in cc.,h
+00000330: 7474 7073 3a2f 2f77 7777 2e77 332e 6f72  ttps://www.w3.or
+00000340: 672f 6e73 2f61 6374 6976 6974 7973 7472  g/ns/activitystr
+00000350: 6561 6d73 2350 7562 6c69 6329 0472 0d00  eams#Public).r..
+00000360: 0000 da03 6164 6472 0900 0000 720e 0000  ....addr....r...
+00000370: 00a9 01da 0473 656c 66a9 0072 1800 0000  .....self..r....
+00000380: fa5c 2f77 6f6f 6470 6563 6b65 722f 7372  .\/woodpecker/sr
+00000390: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
+000003a0: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
+000003b0: 696e 652f 626f 7669 6e65 2f61 6374 6976  ine/bovine/activ
+000003c0: 6974 7973 7472 6561 6d73 2f61 6374 6976  itystreams/activ
+000003d0: 6974 795f 6661 6374 6f72 792e 7079 da09  ity_factory.py..
+000003e0: 6173 5f70 7562 6c69 6319 0000 0073 0800  as_public....s..
+000003f0: 0000 0c02 0601 0e01 0401 7a12 4163 7469  ..........z.Acti
+00000400: 7669 7479 2e61 735f 7075 626c 6963 6301  vity.as_publicc.
+00000410: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000420: 0000 0043 0000 0073 2400 0000 7c00 6a00  ...C...s$...|.j.
+00000430: 720a 7c00 6a01 a002 7c00 6a00 a101 0100  r.|.j...|.j.....
+00000440: 7c00 6a03 a002 6401 a101 0100 7c00 5300  |.j...d.....|.S.
+00000450: 2902 7a42 6d61 6b65 7320 7468 6520 6163  ).zBmakes the ac
+00000460: 7469 7669 7479 2075 6e6c 6973 7465 642c  tivity unlisted,
+00000470: 2069 2e65 2e20 7075 626c 6963 2069 6e20   i.e. public in 
+00000480: 6363 2061 6e64 2066 6f6c 6c6f 7765 7273  cc and followers
+00000490: 2069 6e20 746f 7214 0000 0029 0472 0900   in tor....).r..
+000004a0: 0000 720d 0000 0072 1500 0000 720e 0000  ..r....r....r...
+000004b0: 0072 1600 0000 7218 0000 0072 1800 0000  .r....r....r....
+000004c0: 7219 0000 00da 0b61 735f 756e 6c69 7374  r......as_unlist
+000004d0: 6564 2000 0000 7308 0000 0006 020e 010c  ed ...s.........
+000004e0: 0104 017a 1441 6374 6976 6974 792e 6173  ...z.Activity.as
+000004f0: 5f75 6e6c 6973 7465 64da 0672 6574 7572  _unlisted..retur
+00000500: 6e63 0100 0000 0000 0000 0000 0000 0500  nc..............
+00000510: 0000 0800 0000 4300 0000 73ae 0000 0064  ......C...s....d
+00000520: 017c 006a 007c 006a 0174 027c 006a 0383  .|.j.|.j.t.|.j..
+00000530: 0174 027c 006a 047c 006a 0318 0083 0164  .t.|.j.|.j.....d
+00000540: 029c 057d 017c 006a 057c 006a 067c 006a  ...}.|.j.|.j.|.j
+00000550: 077c 006a 087c 006a 097c 006a 0a7c 006a  .|.j.|.j.|.j.|.j
+00000560: 0b64 039c 077d 027c 0164 0419 0064 0575  .d...}.|.d...d.u
+00000570: 0172 3574 0c7c 0164 0419 0083 0164 066b  .r5t.|.d.....d.k
+00000580: 0272 357c 0164 043d 007c 0164 0719 0064  .r5|.d.=.|.d...d
+00000590: 0575 0172 4674 0c7c 0164 0719 0083 0164  .u.rFt.|.d.....d
+000005a0: 066b 0272 467c 0164 073d 007c 02a0 0da1  .k.rF|.d.=.|....
+000005b0: 0044 005d 0a5c 027d 037d 047c 0472 547c  .D.].\.}.}.|.rT|
+000005c0: 047c 017c 033c 0071 4a7c 0153 0029 087a  .|.|.<.qJ|.S.).z
+000005d0: 4163 6f6e 7665 7274 7320 7468 6520 6163  Aconverts the ac
+000005e0: 7469 7669 7479 2069 6e74 6f20 6120 6469  tivity into a di
+000005f0: 6374 2c20 7468 6174 2063 616e 2062 6520  ct, that can be 
+00000600: 7365 7269 616c 697a 6564 2074 6f20 4a53  serialized to JS
+00000610: 4f4e 7a25 6874 7470 733a 2f2f 7777 772e  ONz%https://www.
+00000620: 7733 2e6f 7267 2f6e 732f 6163 7469 7669  w3.org/ns/activi
+00000630: 7479 7374 7265 616d 7329 057a 0840 636f  tystreams).z.@co
+00000640: 6e74 6578 7472 0700 0000 7208 0000 0072  ntextr....r....r
+00000650: 0d00 0000 720e 0000 0029 0772 0a00 0000  ....r....).r....
+00000660: 720b 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000670: 1100 0000 7212 0000 0072 1300 0000 720d  ....r....r....r.
+00000680: 0000 004e 7201 0000 0072 0e00 0000 290e  ...Nr....r....).
+00000690: 7207 0000 0072 0800 0000 da04 6c69 7374  r....r......list
+000006a0: 720d 0000 0072 0e00 0000 720a 0000 0072  r....r....r....r
+000006b0: 0b00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+000006c0: 0000 0072 1200 0000 7213 0000 00da 036c  ...r....r......l
+000006d0: 656e da05 6974 656d 7329 0572 1700 0000  en..items).r....
+000006e0: da06 7265 7375 6c74 5a0c 6578 7472 615f  ..resultZ.extra_
+000006f0: 6669 656c 6473 da03 6b65 79da 0576 616c  fields..key..val
+00000700: 7565 7218 0000 0072 1800 0000 7219 0000  uer....r....r...
+00000710: 00da 0562 7569 6c64 2700 0000 732e 0000  ...build'...s...
+00000720: 0002 0304 0104 0108 010e 0106 fb04 0904  ................
+00000730: 0104 0104 0104 0104 0104 0106 f91c 0a06  ................
+00000740: 011c 0106 0110 0204 0108 0102 8004 027a  ...............z
+00000750: 0e41 6374 6976 6974 792e 6275 696c 6429  .Activity.build)
+00000760: 19da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000770: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000780: 616d 655f 5fda 075f 5f64 6f63 5f5f da03  ame__..__doc__..
+00000790: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
+000007a0: 6e73 5f5f 7208 0000 0072 0400 0000 7209  ns__r....r....r.
+000007b0: 0000 0072 0a00 0000 720b 0000 0072 0300  ...r....r....r..
+000007c0: 0000 da03 7365 7472 0d00 0000 7205 0000  ....setr....r...
+000007d0: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
+000007e0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000007f0: 1a00 0000 721b 0000 00da 0464 6963 7472  ....r......dictr
+00000800: 2300 0000 7218 0000 0072 1800 0000 7218  #...r....r....r.
+00000810: 0000 0072 1900 0000 7206 0000 0005 0000  ...r....r.......
+00000820: 0073 2200 0000 0a00 0402 0803 1001 1001  .s".............
+00000830: 1001 1001 1601 1601 1002 1001 1001 1002  ................
+00000840: 1001 0802 0807 1207 7206 0000 0063 0000  ........r....c..
+00000850: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00000860: 0000 4000 0000 7358 0000 0065 005a 0164  ..@...sX...e.Z.d
+00000870: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
+00000880: 0464 0584 005a 0564 0664 0784 005a 0664  .d...Z.d.d...Z.d
+00000890: 0864 0984 005a 0764 0a64 0b84 005a 0864  .d...Z.d.d...Z.d
+000008a0: 0c64 0d84 005a 0964 0e64 0f84 005a 0a64  .d...Z.d.d...Z.d
+000008b0: 1064 1184 005a 0b64 1264 1384 005a 0c64  .d...Z.d.d...Z.d
+000008c0: 1453 0029 15da 0f41 6374 6976 6974 7946  .S.)...ActivityF
+000008d0: 6163 746f 7279 7a49 4261 7369 6320 6661  actoryzIBasic fa
+000008e0: 6374 6f72 7920 666f 7220 4163 7469 7669  ctory for Activi
+000008f0: 7479 206f 626a 6563 7473 2e0a 0a20 2020  ty objects...   
+00000900: 2055 7361 6c6c 7920 6372 6561 7465 6420   Usally created 
+00000910: 6279 2061 2042 6f76 696e 6543 6c69 656e  by a BovineClien
+00000920: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00000930: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
+00000940: 017c 005f 0064 0053 0029 014e 2901 da0b  .|._.d.S.).N)...
+00000950: 696e 666f 726d 6174 696f 6e29 0272 1700  information).r..
+00000960: 0000 da11 6163 746f 725f 696e 666f 726d  ....actor_inform
+00000970: 6174 696f 6e72 1800 0000 7218 0000 0072  ationr....r....r
+00000980: 1900 0000 da08 5f5f 696e 6974 5f5f 4c00  ......__init__L.
+00000990: 0000 7302 0000 000a 017a 1841 6374 6976  ..s......z.Activ
+000009a0: 6974 7946 6163 746f 7279 2e5f 5f69 6e69  ityFactory.__ini
+000009b0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+000009c0: 0300 0000 0a00 0000 4b00 0000 f336 0000  ........K....6..
+000009d0: 0074 0064 0764 017c 0164 0219 0074 017c  .t.d.d.|.d...t.|
+000009e0: 01a0 0264 0367 00a1 0283 0174 017c 01a0  ...d.g.....t.|..
+000009f0: 0264 0467 00a1 0283 017c 0164 059c 057c  .d.g.....|.d...|
+00000a00: 02a4 018e 0153 0029 087a 2341 6374 6976  .....S.).z#Activ
+00000a10: 6974 7920 6f66 2074 7970 6520 4372 6561  ity of type Crea
+00000a20: 7465 2066 726f 6d20 4f62 6a65 6374 5a06  te from ObjectZ.
+00000a30: 4372 6561 7465 da0c 6174 7472 6962 7574  Create..attribut
+00000a40: 6564 546f 720e 0000 0072 0d00 0000 a905  edTor....r......
+00000a50: 7207 0000 0072 0800 0000 720e 0000 0072  r....r....r....r
+00000a60: 0d00 0000 7213 0000 004e 7218 0000 00a9  ....r....Nr.....
+00000a70: 0372 0600 0000 722a 0000 00da 0367 6574  .r....r*.....get
+00000a80: a903 7217 0000 00da 036f 626a da06 6b77  ..r......obj..kw
+00000a90: 6172 6773 7218 0000 0072 1800 0000 7219  argsr....r....r.
+00000aa0: 0000 00da 0663 7265 6174 654f 0000 00f3  .....createO....
+00000ab0: 1200 0000 0402 0201 0601 0e01 0e01 0201  ................
+00000ac0: 04fb 0206 06fa 7a16 4163 7469 7669 7479  ......z.Activity
+00000ad0: 4661 6374 6f72 792e 6372 6561 7465 6302  Factory.createc.
+00000ae0: 0000 0000 0000 0000 0000 0003 0000 000a  ................
+00000af0: 0000 004b 0000 0072 3000 0000 2908 7a23  ...K...r0...).z#
+00000b00: 4163 7469 7669 7479 206f 6620 7479 7065  Activity of type
+00000b10: 2055 7064 6174 6520 6672 6f6d 204f 626a   Update from Obj
+00000b20: 6563 745a 0655 7064 6174 6572 3100 0000  ectZ.Updater1...
+00000b30: 720e 0000 0072 0d00 0000 7232 0000 004e  r....r....r2...N
+00000b40: 7218 0000 0072 3300 0000 7235 0000 0072  r....r3...r5...r
+00000b50: 1800 0000 7218 0000 0072 1900 0000 da06  ....r....r......
+00000b60: 7570 6461 7465 5a00 0000 7239 0000 007a  updateZ...r9...z
+00000b70: 1641 6374 6976 6974 7946 6163 746f 7279  .ActivityFactory
+00000b80: 2e75 7064 6174 6563 0200 0000 0000 0000  .updatec........
+00000b90: 0000 0000 0300 0000 0600 0000 4b00 0000  ............K...
+00000ba0: f31c 0000 0074 0064 0564 017c 006a 0164  .....t.d.d.|.j.d
+00000bb0: 0219 007c 0164 039c 037c 02a4 018e 0153  ...|.d...|.....S
+00000bc0: 0029 067a 0f4c 696b 6520 666f 7220 7461  .).z.Like for ta
+00000bd0: 7267 6574 5a04 4c69 6b65 720a 0000 00a9  rgetZ.Liker.....
+00000be0: 0372 0700 0000 7208 0000 0072 1300 0000  .r....r....r....
+00000bf0: 4e72 1800 0000 a902 7206 0000 0072 2d00  Nr......r....r-.
+00000c00: 0000 a903 7217 0000 0072 1200 0000 7237  ....r....r....r7
+00000c10: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000c20: 0000 da04 6c69 6b65 6500 0000 f30a 0000  ....likee.......
+00000c30: 0004 020c 0104 ff02 0106 ff7a 1441 6374  ...........z.Act
+00000c40: 6976 6974 7946 6163 746f 7279 2e6c 696b  ivityFactory.lik
+00000c50: 6563 0200 0000 0000 0000 0000 0000 0300  ec..............
+00000c60: 0000 0600 0000 4b00 0000 723b 0000 0029  ......K...r;...)
+00000c70: 067a 1144 656c 6574 6520 666f 7220 7461  .z.Delete for ta
+00000c80: 7267 6574 da06 4465 6c65 7465 720a 0000  rget..Deleter...
+00000c90: 0072 3c00 0000 4e72 1800 0000 723d 0000  .r<...Nr....r=..
+00000ca0: 0072 3e00 0000 7218 0000 0072 1800 0000  .r>...r....r....
+00000cb0: 7219 0000 00da 0664 656c 6574 656b 0000  r......deletek..
+00000cc0: 0072 4000 0000 7a16 4163 7469 7669 7479  .r@...z.Activity
+00000cd0: 4661 6374 6f72 792e 6465 6c65 7465 6302  Factory.deletec.
+00000ce0: 0000 0000 0000 0000 0000 0003 0000 0006  ................
+00000cf0: 0000 004b 0000 0072 3b00 0000 2906 7a11  ...K...r;...).z.
+00000d00: 4163 6365 7074 2066 6f72 206f 626a 6563  Accept for objec
+00000d10: 74da 0641 6363 6570 7472 0a00 0000 723c  t..Acceptr....r<
+00000d20: 0000 004e 7218 0000 0072 3d00 0000 7235  ...Nr....r=...r5
+00000d30: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000d40: 0000 da06 6163 6365 7074 7100 0000 7240  ....acceptq...r@
+00000d50: 0000 007a 1641 6374 6976 6974 7946 6163  ...z.ActivityFac
+00000d60: 746f 7279 2e61 6363 6570 7463 0200 0000  tory.acceptc....
+00000d70: 0000 0000 0000 0000 0300 0000 0600 0000  ................
+00000d80: 4b00 0000 723b 0000 0029 067a 1152 656a  K...r;...).z.Rej
+00000d90: 6563 7420 666f 7220 6f62 6a65 6374 5a06  ect for objectZ.
+00000da0: 5265 6a65 6374 720a 0000 0072 3c00 0000  Rejectr....r<...
+00000db0: 4e72 1800 0000 723d 0000 0072 3500 0000  Nr....r=...r5...
+00000dc0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+00000dd0: 0672 656a 6563 7477 0000 0072 4000 0000  .rejectw...r@...
+00000de0: 7a16 4163 7469 7669 7479 4661 6374 6f72  z.ActivityFactor
+00000df0: 792e 7265 6a65 6374 6302 0000 0000 0000  y.rejectc.......
+00000e00: 0000 0000 0003 0000 0009 0000 004b 0000  .............K..
+00000e10: 0073 2800 0000 7400 6406 6401 7c00 6a01  .s(...t.d.d.|.j.
+00000e20: 6402 1900 7c01 7c00 6a01 a002 6403 6700  d...|.|.j...d.g.
+00000e30: a102 6404 9c04 7c02 a401 8e01 5300 2907  ..d...|.....S.).
+00000e40: 7a13 416e 6e6f 756e 6365 2066 6f72 206f  z.Announce for o
+00000e50: 626a 6563 745a 0841 6e6e 6f75 6e63 6572  bjectZ.Announcer
+00000e60: 0a00 0000 7209 0000 0029 0472 0700 0000  ....r....).r....
+00000e70: 7208 0000 0072 1300 0000 7209 0000 004e  r....r....r....N
+00000e80: 7218 0000 0029 0372 0600 0000 722d 0000  r....).r....r-..
+00000e90: 0072 3400 0000 7235 0000 0072 1800 0000  .r4...r5...r....
+00000ea0: 7218 0000 0072 1900 0000 da08 616e 6e6f  r....r......anno
+00000eb0: 756e 6365 7d00 0000 7310 0000 0004 0202  unce}...s.......
+00000ec0: 0108 0102 010c 0104 fc02 0506 fb7a 1841  .............z.A
+00000ed0: 6374 6976 6974 7946 6163 746f 7279 2e61  ctivityFactory.a
+00000ee0: 6e6e 6f75 6e63 6563 0200 0000 0000 0000  nnouncec........
+00000ef0: 0000 0000 0300 0000 0700 0000 4b00 0000  ............K...
+00000f00: 7324 0000 0074 0064 0564 017c 006a 0164  s$...t.d.d.|.j.d
+00000f10: 0219 007c 0174 027c 0167 0183 0164 039c  ...|.t.|.g...d..
+00000f20: 047c 02a4 018e 0153 0029 067a 1146 6f6c  .|.....S.).z.Fol
+00000f30: 6c6f 7720 666f 7220 6f62 6a65 6374 5a06  low for objectZ.
+00000f40: 466f 6c6c 6f77 720a 0000 0029 0472 0700  Followr....).r..
+00000f50: 0000 7208 0000 0072 1300 0000 720d 0000  ..r....r....r...
+00000f60: 004e 7218 0000 0029 0372 0600 0000 722d  .Nr....).r....r-
+00000f70: 0000 0072 2a00 0000 7235 0000 0072 1800  ...r*...r5...r..
+00000f80: 0000 7218 0000 0072 1900 0000 da06 666f  ..r....r......fo
+00000f90: 6c6c 6f77 8700 0000 7310 0000 0004 0202  llow....s.......
+00000fa0: 0108 0102 0108 0104 fc02 0506 fb7a 1641  .............z.A
+00000fb0: 6374 6976 6974 7946 6163 746f 7279 2e66  ctivityFactory.f
+00000fc0: 6f6c 6c6f 774e 290d 7224 0000 0072 2500  ollowN).r$...r%.
+00000fd0: 0000 7226 0000 0072 2700 0000 722f 0000  ..r&...r'...r/..
+00000fe0: 0072 3800 0000 723a 0000 0072 3f00 0000  .r8...r:...r?...
+00000ff0: 7242 0000 0072 4400 0000 7245 0000 0072  rB...rD...rE...r
+00001000: 4600 0000 7247 0000 0072 1800 0000 7218  F...rG...r....r.
+00001010: 0000 0072 1800 0000 7219 0000 0072 2c00  ...r....r....r,.
+00001020: 0000 4700 0000 7316 0000 0008 0004 0108  ..G...s.........
+00001030: 0408 0308 0b08 0b08 0608 0608 0608 060c  ................
+00001040: 0a72 2c00 0000 4e29 08da 0b64 6174 6163  .r,...N)...datac
+00001050: 6c61 7373 6573 7202 0000 0072 0300 0000  lassesr....r....
+00001060: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
+00001070: 0000 7206 0000 0072 2c00 0000 7218 0000  ..r....r,...r...
+00001080: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001090: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+000010a0: 0000 0010 0010 0102 0310 0112 41         ............A
```

### Comparing `bovine-0.1.2/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc` & `bovine-0.1.3/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 4240 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 9010 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 9010 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6404 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6502 4700 6406 6407 8400  m.Z...e.G.d.d...
 00000070: 6407 8302 8301 5a0a 4700 6408 6409 8400  d.....Z.G.d.d...
```

### Comparing `bovine-0.1.2/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2163 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,285 +1,287 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 7308 0000  o.........Ads...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 9308 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
+00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6402 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
-00000060: 6405 6406 8400 5a0a 6407 6408 8400 5a0b  d.d...Z.d.d...Z.
-00000070: 6409 640a 8400 5a0c 640b 640c 8400 5a0d  d.d...Z.d.d...Z.
-00000080: 640d 640e 8400 5a0e 6401 5300 290f e900  d.d...Z.d.S.)...
-00000090: 0000 004e e901 0000 0029 01da 0f41 6374  ...N.....)...Act
-000000a0: 6976 6974 7946 6163 746f 7279 2901 da06  ivityFactory)...
-000000b0: 4f62 6a65 6374 6300 0000 0000 0000 0000  Objectc.........
-000000c0: 0000 0008 0000 0007 0000 0043 0000 0073  ...........C...s
-000000d0: ee01 0000 7400 6401 6402 6403 9c02 8301  ....t.d.d.d.....
-000000e0: 7d00 7c00 a001 6404 a101 7d01 7c01 6a02  }.|...d...}.|.j.
-000000f0: a003 6404 a101 0100 7c01 6a04 a003 6405  ..d.....|.j...d.
-00000100: a101 0100 6406 7c01 5f05 7c01 a006 a100  ....d.|._.|.....
-00000110: 7d02 7c02 6407 1900 7d03 6408 7d04 7c03  }.|.d...}.d.}.|.
-00000120: 7c04 6b02 7d05 7c05 734e 7407 a008 6409  |.k.}.|.sNt...d.
-00000130: 7c05 6601 640a 7c03 7c04 6602 a104 7407  |.f.d.|.|.f...t.
-00000140: a009 7c03 a101 7407 a009 7c04 a101 640b  ..|...t...|...d.
-00000150: 9c02 1600 7d06 640c 640d 7c06 6901 1600  ....}.d.d.|.i...
-00000160: 7d07 740a 7407 a00b 7c07 a101 8301 8201  }.t.t...|.......
-00000170: 6400 0400 7d03 0400 7d05 7d04 7c02 640e  d...}...}.}.|.d.
-00000180: 1900 7d03 6404 6701 7d04 7c03 7c04 6b02  ..}.d.g.}.|.|.k.
-00000190: 7d05 7c05 7384 7407 a008 6409 7c05 6601  }.|.s.t...d.|.f.
-000001a0: 640a 7c03 7c04 6602 a104 7407 a009 7c03  d.|.|.f...t...|.
-000001b0: a101 7407 a009 7c04 a101 640b 9c02 1600  ..t...|...d.....
-000001c0: 7d06 640c 640d 7c06 6901 1600 7d07 740a  }.d.d.|.i...}.t.
-000001d0: 7407 a00b 7c07 a101 8301 8201 6400 0400  t...|.......d...
-000001e0: 7d03 0400 7d05 7d04 7c02 640f 1900 7d03  }...}.}.|.d...}.
-000001f0: 6405 6701 7d04 7c03 7c04 6b02 7d05 7c05  d.g.}.|.|.k.}.|.
-00000200: 73ba 7407 a008 6409 7c05 6601 640a 7c03  s.t...d.|.f.d.|.
-00000210: 7c04 6602 a104 7407 a009 7c03 a101 7407  |.f...t...|...t.
-00000220: a009 7c04 a101 640b 9c02 1600 7d06 640c  ..|...d.....}.d.
-00000230: 640d 7c06 6901 1600 7d07 740a 7407 a00b  d.|.i...}.t.t...
-00000240: 7c07 a101 8301 8201 6400 0400 7d03 0400  |.......d...}...
-00000250: 7d05 7d04 7c02 6410 1900 7d03 6411 7d04  }.}.|.d...}.d.}.
-00000260: 7c03 7c04 6b02 7d05 7c05 73ef 7407 a008  |.|.k.}.|.s.t...
-00000270: 6409 7c05 6601 640a 7c03 7c04 6602 a104  d.|.f.d.|.|.f...
-00000280: 7407 a009 7c03 a101 7407 a009 7c04 a101  t...|...t...|...
-00000290: 640b 9c02 1600 7d06 640c 640d 7c06 6901  d.....}.d.d.|.i.
-000002a0: 1600 7d07 740a 7407 a00b 7c07 a101 8301  ..}.t.t...|.....
-000002b0: 8201 6400 0400 7d03 0400 7d05 7d04 6400  ..d...}...}.}.d.
-000002c0: 5300 2912 4eda 0861 6374 6f72 5f69 64da  S.).N..actor_id.
-000002d0: 0966 6f6c 6c6f 7765 7273 a902 da02 6964  .followers....id
-000002e0: 7206 0000 00da 0674 6172 6765 74da 056f  r......target..o
-000002f0: 7468 6572 7504 0000 00f0 9f90 aefa 0840  theru..........@
-00000300: 636f 6e74 6578 74fa 2568 7474 7073 3a2f  context.%https:/
-00000310: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
-00000320: 6374 6976 6974 7973 7472 6561 6d73 a901  ctivitystreams..
-00000330: fa02 3d3d a901 7a12 2528 7079 3129 7320  ..==..z.%(py1)s 
-00000340: 3d3d 2025 2870 7934 2973 a902 da03 7079  == %(py4)s....py
-00000350: 31da 0370 7934 fa0e 6173 7365 7274 2025  1..py4..assert %
-00000360: 2870 7936 2973 da03 7079 36da 0274 6fda  (py6)s..py6..to.
-00000370: 0263 63da 0474 7970 65da 044c 696b 6529  .cc..type..Like)
-00000380: 0c72 0300 0000 da04 6c69 6b65 7215 0000  .r......liker...
-00000390: 00da 0361 6464 7216 0000 00da 0763 6f6e  ...addr......con
-000003a0: 7465 6e74 da05 6275 696c 64da 0a40 7079  tent..build..@py
-000003b0: 7465 7374 5f61 72da 115f 6361 6c6c 5f72  test_ar.._call_r
-000003c0: 6570 7263 6f6d 7061 7265 da09 5f73 6166  eprcompare.._saf
-000003d0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
-000003e0: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
-000003f0: 7870 6c61 6e61 7469 6f6e 2908 da10 6163  xplanation)...ac
-00000400: 7469 7669 7479 5f66 6163 746f 7279 7219  tivity_factoryr.
-00000410: 0000 00da 0672 6573 756c 74da 0b40 7079  .....result..@py
-00000420: 5f61 7373 6572 7430 da0b 4070 795f 6173  _assert0..@py_as
-00000430: 7365 7274 33da 0b40 7079 5f61 7373 6572  sert3..@py_asser
-00000440: 7432 da0b 4070 795f 666f 726d 6174 35da  t2..@py_format5.
-00000450: 0b40 7079 5f66 6f72 6d61 7437 a900 7229  .@py_format7..r)
-00000460: 0000 00fa 612f 776f 6f64 7065 636b 6572  ....a/woodpecker
-00000470: 2f73 7263 2f63 6f64 6562 6572 672e 6f72  /src/codeberg.or
-00000480: 672f 626f 7669 6e65 2f62 6f76 696e 652f  g/bovine/bovine/
-00000490: 626f 7669 6e65 2f62 6f76 696e 652f 6163  bovine/bovine/ac
-000004a0: 7469 7669 7479 7374 7265 616d 732f 7465  tivitystreams/te
-000004b0: 7374 5f61 6374 6976 6974 795f 6661 6374  st_activity_fact
-000004c0: 6f72 792e 7079 da1a 7465 7374 5f61 6374  ory.py..test_act
-000004d0: 6976 6974 795f 6661 6374 6f72 795f 6c69  ivity_factory_li
-000004e0: 6b65 0500 0000 7314 0000 000e 010a 020c  ke....s.........
-000004f0: 010c 0106 0108 026a 026c 026c 016e 0272  .......j.l.l.n.r
-00000500: 2b00 0000 6300 0000 0000 0000 0000 0000  +...c...........
-00000510: 0008 0000 0007 0000 0043 0000 0073 d401  .........C...s..
-00000520: 0000 7400 6401 6402 6403 9c02 8301 7d00  ..t.d.d.d.....}.
-00000530: 7c00 a001 6404 6405 6901 a101 7d01 7c01  |...d.d.i...}.|.
-00000540: a002 a100 7d02 7c02 6406 1900 7d03 6407  ....}.|.d...}.d.
-00000550: 7d04 7c03 7c04 6b02 7d05 7c05 7341 7403  }.|.|.k.}.|.sAt.
-00000560: a004 6408 7c05 6601 6409 7c03 7c04 6602  ..d.|.f.d.|.|.f.
-00000570: a104 7403 a005 7c03 a101 7403 a005 7c04  ..t...|...t...|.
-00000580: a101 640a 9c02 1600 7d06 640b 640c 7c06  ..d.....}.d.d.|.
-00000590: 6901 1600 7d07 7406 7403 a007 7c07 a101  i...}.t.t...|...
-000005a0: 8301 8201 6400 0400 7d03 0400 7d05 7d04  ....d...}...}.}.
-000005b0: 7c02 640d 1900 7d03 640e 7d04 7c03 7c04  |.d...}.d.}.|.|.
-000005c0: 6b02 7d05 7c05 7376 7403 a004 6408 7c05  k.}.|.svt...d.|.
-000005d0: 6601 6409 7c03 7c04 6602 a104 7403 a005  f.d.|.|.f...t...
-000005e0: 7c03 a101 7403 a005 7c04 a101 640a 9c02  |...t...|...d...
-000005f0: 1600 7d06 640b 640c 7c06 6901 1600 7d07  ..}.d.d.|.i...}.
-00000600: 7406 7403 a007 7c07 a101 8301 8201 6400  t.t...|.......d.
-00000610: 0400 7d03 0400 7d05 7d04 7c02 640f 1900  ..}...}.}.|.d...
-00000620: 7d03 6401 7d04 7c03 7c04 6b02 7d05 7c05  }.d.}.|.|.k.}.|.
-00000630: 73ab 7403 a004 6408 7c05 6601 6409 7c03  s.t...d.|.f.d.|.
-00000640: 7c04 6602 a104 7403 a005 7c03 a101 7403  |.f...t...|...t.
-00000650: a005 7c04 a101 640a 9c02 1600 7d06 640b  ..|...d.....}.d.
-00000660: 640c 7c06 6901 1600 7d07 7406 7403 a007  d.|.i...}.t.t...
-00000670: 7c07 a101 8301 8201 6400 0400 7d03 0400  |.......d...}...
-00000680: 7d05 7d04 7c02 6410 1900 6404 1900 7d03  }.}.|.d...d...}.
-00000690: 6405 7d04 7c03 7c04 6b02 7d05 7c05 73e2  d.}.|.|.k.}.|.s.
-000006a0: 7403 a004 6408 7c05 6601 6409 7c03 7c04  t...d.|.f.d.|.|.
-000006b0: 6602 a104 7403 a005 7c03 a101 7403 a005  f...t...|...t...
-000006c0: 7c04 a101 640a 9c02 1600 7d06 640b 640c  |...d.....}.d.d.
-000006d0: 7c06 6901 1600 7d07 7406 7403 a007 7c07  |.i...}.t.t...|.
-000006e0: a101 8301 8201 6400 0400 7d03 0400 7d05  ......d...}...}.
-000006f0: 7d04 6400 5300 2911 4e72 0500 0000 7206  }.d.S.).Nr....r.
-00000700: 0000 0072 0700 0000 7208 0000 00da 036f  ...r....r......o
-00000710: 626a 720b 0000 0072 0c00 0000 720d 0000  bjr....r....r...
-00000720: 0072 0f00 0000 7210 0000 0072 1300 0000  .r....r....r....
-00000730: 7214 0000 0072 1700 0000 da06 4163 6365  r....r......Acce
-00000740: 7074 da05 6163 746f 72da 066f 626a 6563  pt..actor..objec
-00000750: 7429 0872 0300 0000 da06 6163 6365 7074  t).r......accept
-00000760: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000770: 1f00 0000 7220 0000 0072 2100 0000 2908  ....r ...r!...).
-00000780: 7222 0000 0072 3000 0000 7223 0000 0072  r"...r0...r#...r
-00000790: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
-000007a0: 0000 0072 2800 0000 7229 0000 0072 2900  ...r(...r)...r).
-000007b0: 0000 722a 0000 00da 1c74 6573 745f 6163  ..r*.....test_ac
-000007c0: 7469 7669 7479 5f66 6163 746f 7279 5f61  tivity_factory_a
-000007d0: 6363 6570 7417 0000 0073 0e00 0000 0e01  ccept....s......
-000007e0: 0e02 0801 6a02 6a01 6a01 7201 7231 0000  ....j.j.j.r.r1..
-000007f0: 0063 0000 0000 0000 0000 0000 0000 0800  .c..............
-00000800: 0000 0700 0000 4300 0000 7378 0100 0074  ......C...sx...t
-00000810: 0064 0164 0264 039c 0283 017d 0074 0164  .d.d.d.....}.t.d
-00000820: 0464 0164 0564 068d 03a0 02a1 00a0 03a1  .d.d.d..........
-00000830: 007d 017c 00a0 047c 01a1 01a0 03a1 007d  .}.|...|.......}
-00000840: 027c 0264 0719 007d 0364 0567 017d 047c  .|.d...}.d.g.}.|
-00000850: 037c 046b 027d 057c 0573 4974 05a0 0664  .|.k.}.|.sIt...d
-00000860: 087c 0566 0164 097c 037c 0466 02a1 0474  .|.f.d.|.|.f...t
-00000870: 05a0 077c 03a1 0174 05a0 077c 04a1 0164  ...|...t...|...d
-00000880: 0a9c 0216 007d 0664 0b64 0c7c 0669 0116  .....}.d.d.|.i..
-00000890: 007d 0774 0874 05a0 097c 07a1 0183 0182  .}.t.t...|......
-000008a0: 0164 0004 007d 0304 007d 057d 047c 0264  .d...}...}.}.|.d
-000008b0: 0d19 007d 0364 0e67 017d 047c 037c 046b  ...}.d.g.}.|.|.k
-000008c0: 027d 057c 0573 7f74 05a0 0664 087c 0566  .}.|.s.t...d.|.f
-000008d0: 0164 097c 037c 0466 02a1 0474 05a0 077c  .d.|.|.f...t...|
-000008e0: 03a1 0174 05a0 077c 04a1 0164 0a9c 0216  ...t...|...d....
-000008f0: 007d 0664 0b64 0c7c 0669 0116 007d 0774  .}.d.d.|.i...}.t
-00000900: 0874 05a0 097c 07a1 0183 0182 0164 0004  .t...|.......d..
-00000910: 007d 0304 007d 057d 047c 0264 0f19 007d  .}...}.}.|.d...}
-00000920: 0364 017d 047c 037c 046b 027d 057c 0573  .d.}.|.|.k.}.|.s
-00000930: b474 05a0 0664 087c 0566 0164 097c 037c  .t...d.|.f.d.|.|
-00000940: 0466 02a1 0474 05a0 077c 03a1 0174 05a0  .f...t...|...t..
-00000950: 077c 04a1 0164 0a9c 0216 007d 0664 0b64  .|...d.....}.d.d
-00000960: 0c7c 0669 0116 007d 0774 0874 05a0 097c  .|.i...}.t.t...|
-00000970: 07a1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
-00000980: 057d 0464 0053 0029 104e 7205 0000 0072  .}.d.S.).Nr....r
-00000990: 0600 0000 7207 0000 00da 044e 6f74 65fa  ....r......Note.
-000009a0: 1161 6363 6f75 6e74 2f66 6f6c 6c6f 7765  .account/followe
-000009b0: 7273 2903 7217 0000 00da 0d61 7474 7269  rs).r......attri
-000009c0: 6275 7465 645f 746f 7206 0000 0072 1600  buted_tor....r..
-000009d0: 0000 720d 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000009e0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-000009f0: 7a2c 6874 7470 733a 2f2f 7777 772e 7733  z,https://www.w3
-00000a00: 2e6f 7267 2f6e 732f 6163 7469 7669 7479  .org/ns/activity
-00000a10: 7374 7265 616d 7323 5075 626c 6963 722e  streams#Publicr.
-00000a20: 0000 0029 0a72 0300 0000 7204 0000 00da  ...).r....r.....
-00000a30: 0961 735f 7075 626c 6963 721c 0000 00da  .as_publicr.....
-00000a40: 0663 7265 6174 6572 1d00 0000 721e 0000  .creater....r...
-00000a50: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00000a60: 2908 7222 0000 00da 046e 6f74 6572 2300  ).r".....noter#.
-00000a70: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
-00000a80: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
-00000a90: 7229 0000 0072 2a00 0000 da1c 7465 7374  r)...r*.....test
-00000aa0: 5f61 6374 6976 6974 795f 6661 6374 6f72  _activity_factor
-00000ab0: 795f 6372 6561 7465 2300 0000 7312 0000  y_create#...s...
-00000ac0: 000e 010c 0204 0104 0102 fd0e 066c 026c  .............l.l
-00000ad0: 016e 0172 3800 0000 6300 0000 0000 0000  .n.r8...c.......
-00000ae0: 0000 0000 000b 0000 0007 0000 0043 0000  .............C..
-00000af0: 0073 8801 0000 7400 6401 6402 6403 9c02  .s....t.d.d.d...
-00000b00: 8301 7d00 6404 7d01 7401 6405 6401 6406  ..}.d.}.t.d.d.d.
-00000b10: 7c01 6801 6407 8d04 a002 a100 7d02 7c00  |.h.d.......}.|.
-00000b20: a003 7c02 a101 a002 a100 7d03 6408 7d04  ..|.......}.d.}.
-00000b30: 7c04 7c03 7601 7d05 7c05 7353 7404 a005  |.|.v.}.|.sSt...
-00000b40: 6409 7c05 6601 640a 7c04 7c03 6602 a104  d.|.f.d.|.|.f...
-00000b50: 7404 a006 7c04 a101 640b 7407 a008 a100  t...|...d.t.....
-00000b60: 7600 733c 7404 a009 7c03 a101 7241 7404  v.s<t...|...rAt.
-00000b70: a006 7c03 a101 6e01 640b 640c 9c02 1600  ..|...n.d.d.....
-00000b80: 7d06 640d 640e 7c06 6901 1600 7d07 740a  }.d.d.|.i...}.t.
-00000b90: 7404 a00b 7c07 a101 8301 8201 6400 0400  t...|.......d...
-00000ba0: 7d04 7d05 7c03 640f 1900 7d04 7c01 6701  }.}.|.d...}.|.g.
-00000bb0: 7d08 7c04 7c08 6b02 7d05 7c05 7387 7404  }.|.|.k.}.|.s.t.
-00000bc0: a005 6410 7c05 6601 6411 7c04 7c08 6602  ..d.|.f.d.|.|.f.
-00000bd0: a104 7404 a006 7c04 a101 7404 a006 7c08  ..t...|...t...|.
-00000be0: a101 6412 9c02 1600 7d09 6413 6414 7c09  ..d.....}.d.d.|.
-00000bf0: 6901 1600 7d0a 740a 7404 a00b 7c0a a101  i...}.t.t...|...
-00000c00: 8301 8201 6400 0400 7d04 0400 7d05 7d08  ....d...}...}.}.
-00000c10: 7c03 6415 1900 7d04 6401 7d08 7c04 7c08  |.d...}.d.}.|.|.
-00000c20: 6b02 7d05 7c05 73bc 7404 a005 6410 7c05  k.}.|.s.t...d.|.
-00000c30: 6601 6411 7c04 7c08 6602 a104 7404 a006  f.d.|.|.f...t...
-00000c40: 7c04 a101 7404 a006 7c08 a101 6412 9c02  |...t...|...d...
-00000c50: 1600 7d09 6413 6414 7c09 6901 1600 7d0a  ..}.d.d.|.i...}.
-00000c60: 740a 7404 a00b 7c0a a101 8301 8201 6400  t.t...|.......d.
-00000c70: 0400 7d04 0400 7d05 7d08 6400 5300 2916  ..}...}.}.d.S.).
-00000c80: 4e72 0500 0000 7206 0000 0072 0700 0000  Nr....r....r....
-00000c90: 7a12 6874 7470 733a 2f2f 6162 656c 2f61  z.https://abel/a
-00000ca0: 6c69 6365 7232 0000 0072 3300 0000 2904  licer2...r3...).
-00000cb0: 7217 0000 0072 3400 0000 7206 0000 0072  r....r4...r....r
-00000cc0: 1500 0000 7216 0000 0029 01fa 066e 6f74  ....r....)...not
-00000cd0: 2069 6e29 017a 1625 2870 7931 2973 206e   in).z.%(py1)s n
-00000ce0: 6f74 2069 6e20 2528 7079 3329 7372 2300  ot in %(py3)sr#.
-00000cf0: 0000 2902 7211 0000 00da 0370 7933 7a0e  ..).r......py3z.
-00000d00: 6173 7365 7274 2025 2870 7935 2973 da03  assert %(py5)s..
-00000d10: 7079 3572 1500 0000 720d 0000 0072 0f00  py5r....r....r..
-00000d20: 0000 7210 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00000d30: 0072 2e00 0000 290c 7203 0000 0072 0400  .r....).r....r..
-00000d40: 0000 721c 0000 0072 3600 0000 721d 0000  ..r....r6...r...
-00000d50: 0072 1e00 0000 721f 0000 00da 0c40 7079  .r....r......@py
-00000d60: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
-00000d70: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
-00000d80: 676c 6f62 616c 5f6e 616d 6572 2000 0000  global_namer ...
-00000d90: 7221 0000 0029 0b72 2200 0000 da0c 7265  r!...).r".....re
-00000da0: 6d6f 7465 5f61 6374 6f72 7237 0000 0072  mote_actorr7...r
-00000db0: 2300 0000 7224 0000 0072 2600 0000 da0b  #...r$...r&.....
-00000dc0: 4070 795f 666f 726d 6174 34da 0b40 7079  @py_format4..@py
-00000dd0: 5f66 6f72 6d61 7436 7225 0000 0072 2700  _format6r%...r'.
-00000de0: 0000 7228 0000 0072 2900 0000 7229 0000  ..r(...r)...r)..
-00000df0: 0072 2a00 0000 da22 7465 7374 5f61 6374  .r*...."test_act
-00000e00: 6976 6974 795f 6661 6374 6f72 795f 6372  ivity_factory_cr
-00000e10: 6561 7465 5f6e 6f5f 6363 3200 0000 731c  eate_no_cc2...s.
-00000e20: 0000 000e 0104 0102 0102 0102 0102 0104  ................
-00000e30: 0104 fc04 0502 fb0e 0778 026c 016e 0172  .........x.l.n.r
-00000e40: 4200 0000 6300 0000 0000 0000 0000 0000  B...c...........
-00000e50: 0009 0000 0009 0000 0043 0000 0073 f600  .........C...s..
-00000e60: 0000 7400 6401 6402 6403 9c02 8301 7d00  ..t.d.d.d.....}.
-00000e70: 7c00 a001 6404 a101 a002 a100 7d01 7c01  |...d.......}.|.
-00000e80: 6a03 7d02 7c02 8300 7d03 7404 7c03 8301  j.}.|...}.t.|...
-00000e90: 7d04 6800 6405 a301 7d05 7c04 7c05 6b02  }.h.d...}.|.|.k.
-00000ea0: 7d06 7c06 736f 7405 a006 6406 7c06 6601  }.|.sot...d.|.f.
-00000eb0: 6407 7c04 7c05 6602 a104 6408 7407 a008  d.|.|.f...d.t...
-00000ec0: a100 7600 7337 7405 a009 7404 a101 723c  ..v.s7t...t...r<
-00000ed0: 7405 a00a 7404 a101 6e01 6408 6409 7407  t...t...n.d.d.t.
-00000ee0: a008 a100 7600 7348 7405 a009 7c01 a101  ....v.sHt...|...
-00000ef0: 724d 7405 a00a 7c01 a101 6e01 6409 7405  rMt...|...n.d.t.
-00000f00: a00a 7c02 a101 7405 a00a 7c03 a101 7405  ..|...t...|...t.
-00000f10: a00a 7c04 a101 7405 a00a 7c05 a101 640a  ..|...t...|...d.
-00000f20: 9c06 1600 7d07 640b 640c 7c07 6901 1600  ....}.d.d.|.i...
-00000f30: 7d08 740b 7405 a00c 7c08 a101 8301 8201  }.t.t...|.......
-00000f40: 6400 0400 7d02 0400 7d03 0400 7d04 0400  d...}...}...}...
-00000f50: 7d06 7d05 6400 5300 290d 4e72 0500 0000  }.}.d.S.).Nr....
-00000f60: 7206 0000 0072 0700 0000 7209 0000 003e  r....r....r....>
-00000f70: 0400 0000 720b 0000 0072 2e00 0000 722f  ....r....r....r/
-00000f80: 0000 0072 1700 0000 720d 0000 0029 017a  ...r....r....).z
-00000f90: 6225 2870 7937 2973 0a7b 2528 7079 3729  b%(py7)s.{%(py7)
-00000fa0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
-00000fb0: 3529 730a 7b25 2870 7935 2973 203d 2025  5)s.{%(py5)s = %
-00000fc0: 2870 7933 2973 0a7b 2528 7079 3329 7320  (py3)s.{%(py3)s 
-00000fd0: 3d20 2528 7079 3129 732e 6b65 7973 0a7d  = %(py1)s.keys.}
-00000fe0: 2829 0a7d 290a 7d20 3d3d 2025 2870 7931  ().}).} == %(py1
-00000ff0: 3029 73da 0373 6574 7223 0000 0029 06da  0)s..setr#...)..
-00001000: 0370 7930 7211 0000 0072 3a00 0000 723b  .py0r....r:...r;
-00001010: 0000 00da 0370 7937 5a04 7079 3130 7a0f  .....py7Z.py10z.
-00001020: 6173 7365 7274 2025 2870 7931 3229 735a  assert %(py12)sZ
-00001030: 0470 7931 3229 0d72 0300 0000 da06 6465  .py12).r......de
-00001040: 6c65 7465 721c 0000 00da 046b 6579 7372  leter......keysr
-00001050: 4300 0000 721d 0000 0072 1e00 0000 723c  C...r....r....r<
-00001060: 0000 0072 3d00 0000 723e 0000 0072 1f00  ...r=...r>...r..
-00001070: 0000 7220 0000 0072 2100 0000 2909 7222  ..r ...r!...).r"
-00001080: 0000 0072 2300 0000 7226 0000 00da 0b40  ...r#...r&.....@
-00001090: 7079 5f61 7373 6572 7434 5a0b 4070 795f  py_assert4Z.@py_
-000010a0: 6173 7365 7274 365a 0b40 7079 5f61 7373  assert6Z.@py_ass
-000010b0: 6572 7439 5a0b 4070 795f 6173 7365 7274  ert9Z.@py_assert
-000010c0: 385a 0c40 7079 5f66 6f72 6d61 7431 315a  8Z.@py_format11Z
-000010d0: 0c40 7079 5f66 6f72 6d61 7431 3372 2900  .@py_format13r).
-000010e0: 0000 7229 0000 0072 2a00 0000 da1c 7465  ..r)...r*.....te
-000010f0: 7374 5f61 6374 6976 6974 795f 6e6f 5f65  st_activity_no_e
-00001100: 6d70 7479 5f74 6f5f 6363 4300 0000 7306  mpty_to_ccC...s.
-00001110: 0000 000e 010e 02da 0272 4900 0000 290f  .........rI...).
-00001120: da08 6275 696c 7469 6e73 723c 0000 00da  ..builtinsr<....
-00001130: 195f 7079 7465 7374 2e61 7373 6572 7469  ._pytest.asserti
-00001140: 6f6e 2e72 6577 7269 7465 da09 6173 7365  on.rewrite..asse
-00001150: 7274 696f 6eda 0772 6577 7269 7465 721d  rtion..rewriter.
-00001160: 0000 0072 2200 0000 7203 0000 00da 0e6f  ...r"...r......o
-00001170: 626a 6563 745f 6661 6374 6f72 7972 0400  bject_factoryr..
-00001180: 0000 722b 0000 0072 3100 0000 7238 0000  ..r+...r1...r8..
-00001190: 0072 4200 0000 7249 0000 0072 2900 0000  .rB...rI...r)...
-000011a0: 7229 0000 0072 2900 0000 722a 0000 00da  r)...r)...r*....
-000011b0: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
-000011c0: 0000 2600 0c01 0803 0812 080c 080f 0c11  ..&.............
+00000060: 6410 6406 6407 8404 5a0a 6410 6408 6409  d.d.d...Z.d.d.d.
+00000070: 8404 5a0b 640a 640b 8400 5a0c 6410 640c  ..Z.d.d...Z.d.d.
+00000080: 640d 8404 5a0d 6410 640e 640f 8404 5a0e  d...Z.d.d.d...Z.
+00000090: 6401 5300 2911 e900 0000 004e e901 0000  d.S.)......N....
+000000a0: 0029 01da 0f41 6374 6976 6974 7946 6163  .)...ActivityFac
+000000b0: 746f 7279 2901 da06 4f62 6a65 6374 da06  tory)...Object..
+000000c0: 7265 7475 726e 6300 0000 0000 0000 0000  returnc.........
+000000d0: 0000 0008 0000 0007 0000 0043 0000 0073  ...........C...s
+000000e0: ee01 0000 7400 6401 6402 6403 9c02 8301  ....t.d.d.d.....
+000000f0: 7d00 7c00 a001 6404 a101 7d01 7c01 6a02  }.|...d...}.|.j.
+00000100: a003 6404 a101 0100 7c01 6a04 a003 6405  ..d.....|.j...d.
+00000110: a101 0100 6406 7c01 5f05 7c01 a006 a100  ....d.|._.|.....
+00000120: 7d02 7c02 6407 1900 7d03 6408 7d04 7c03  }.|.d...}.d.}.|.
+00000130: 7c04 6b02 7d05 7c05 734e 7407 a008 6409  |.k.}.|.sNt...d.
+00000140: 7c05 6601 640a 7c03 7c04 6602 a104 7407  |.f.d.|.|.f...t.
+00000150: a009 7c03 a101 7407 a009 7c04 a101 640b  ..|...t...|...d.
+00000160: 9c02 1600 7d06 640c 640d 7c06 6901 1600  ....}.d.d.|.i...
+00000170: 7d07 740a 7407 a00b 7c07 a101 8301 8201  }.t.t...|.......
+00000180: 6400 0400 7d03 0400 7d05 7d04 7c02 640e  d...}...}.}.|.d.
+00000190: 1900 7d03 6404 6701 7d04 7c03 7c04 6b02  ..}.d.g.}.|.|.k.
+000001a0: 7d05 7c05 7384 7407 a008 6409 7c05 6601  }.|.s.t...d.|.f.
+000001b0: 640a 7c03 7c04 6602 a104 7407 a009 7c03  d.|.|.f...t...|.
+000001c0: a101 7407 a009 7c04 a101 640b 9c02 1600  ..t...|...d.....
+000001d0: 7d06 640c 640d 7c06 6901 1600 7d07 740a  }.d.d.|.i...}.t.
+000001e0: 7407 a00b 7c07 a101 8301 8201 6400 0400  t...|.......d...
+000001f0: 7d03 0400 7d05 7d04 7c02 640f 1900 7d03  }...}.}.|.d...}.
+00000200: 6405 6701 7d04 7c03 7c04 6b02 7d05 7c05  d.g.}.|.|.k.}.|.
+00000210: 73ba 7407 a008 6409 7c05 6601 640a 7c03  s.t...d.|.f.d.|.
+00000220: 7c04 6602 a104 7407 a009 7c03 a101 7407  |.f...t...|...t.
+00000230: a009 7c04 a101 640b 9c02 1600 7d06 640c  ..|...d.....}.d.
+00000240: 640d 7c06 6901 1600 7d07 740a 7407 a00b  d.|.i...}.t.t...
+00000250: 7c07 a101 8301 8201 6400 0400 7d03 0400  |.......d...}...
+00000260: 7d05 7d04 7c02 6410 1900 7d03 6411 7d04  }.}.|.d...}.d.}.
+00000270: 7c03 7c04 6b02 7d05 7c05 73ef 7407 a008  |.|.k.}.|.s.t...
+00000280: 6409 7c05 6601 640a 7c03 7c04 6602 a104  d.|.f.d.|.|.f...
+00000290: 7407 a009 7c03 a101 7407 a009 7c04 a101  t...|...t...|...
+000002a0: 640b 9c02 1600 7d06 640c 640d 7c06 6901  d.....}.d.d.|.i.
+000002b0: 1600 7d07 740a 7407 a00b 7c07 a101 8301  ..}.t.t...|.....
+000002c0: 8201 6400 0400 7d03 0400 7d05 7d04 6400  ..d...}...}.}.d.
+000002d0: 5300 2912 4eda 0861 6374 6f72 5f69 64da  S.).N..actor_id.
+000002e0: 0966 6f6c 6c6f 7765 7273 a902 da02 6964  .followers....id
+000002f0: 7207 0000 00da 0674 6172 6765 74da 056f  r......target..o
+00000300: 7468 6572 7504 0000 00f0 9f90 aefa 0840  theru..........@
+00000310: 636f 6e74 6578 74fa 2568 7474 7073 3a2f  context.%https:/
+00000320: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
+00000330: 6374 6976 6974 7973 7472 6561 6d73 a901  ctivitystreams..
+00000340: fa02 3d3d a901 7a12 2528 7079 3129 7320  ..==..z.%(py1)s 
+00000350: 3d3d 2025 2870 7934 2973 a902 da03 7079  == %(py4)s....py
+00000360: 31da 0370 7934 fa0e 6173 7365 7274 2025  1..py4..assert %
+00000370: 2870 7936 2973 da03 7079 36da 0274 6fda  (py6)s..py6..to.
+00000380: 0263 63da 0474 7970 65da 044c 696b 6529  .cc..type..Like)
+00000390: 0c72 0300 0000 da04 6c69 6b65 7216 0000  .r......liker...
+000003a0: 00da 0361 6464 7217 0000 00da 0763 6f6e  ...addr......con
+000003b0: 7465 6e74 da05 6275 696c 64da 0a40 7079  tent..build..@py
+000003c0: 7465 7374 5f61 72da 115f 6361 6c6c 5f72  test_ar.._call_r
+000003d0: 6570 7263 6f6d 7061 7265 da09 5f73 6166  eprcompare.._saf
+000003e0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
+000003f0: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
+00000400: 7870 6c61 6e61 7469 6f6e 2908 da10 6163  xplanation)...ac
+00000410: 7469 7669 7479 5f66 6163 746f 7279 721a  tivity_factoryr.
+00000420: 0000 00da 0672 6573 756c 74da 0b40 7079  .....result..@py
+00000430: 5f61 7373 6572 7430 da0b 4070 795f 6173  _assert0..@py_as
+00000440: 7365 7274 33da 0b40 7079 5f61 7373 6572  sert3..@py_asser
+00000450: 7432 da0b 4070 795f 666f 726d 6174 35da  t2..@py_format5.
+00000460: 0b40 7079 5f66 6f72 6d61 7437 a900 722a  .@py_format7..r*
+00000470: 0000 00fa 612f 776f 6f64 7065 636b 6572  ....a/woodpecker
+00000480: 2f73 7263 2f63 6f64 6562 6572 672e 6f72  /src/codeberg.or
+00000490: 672f 626f 7669 6e65 2f62 6f76 696e 652f  g/bovine/bovine/
+000004a0: 626f 7669 6e65 2f62 6f76 696e 652f 6163  bovine/bovine/ac
+000004b0: 7469 7669 7479 7374 7265 616d 732f 7465  tivitystreams/te
+000004c0: 7374 5f61 6374 6976 6974 795f 6661 6374  st_activity_fact
+000004d0: 6f72 792e 7079 da1a 7465 7374 5f61 6374  ory.py..test_act
+000004e0: 6976 6974 795f 6661 6374 6f72 795f 6c69  ivity_factory_li
+000004f0: 6b65 0500 0000 7314 0000 000e 010a 020c  ke....s.........
+00000500: 010c 0106 0108 026a 026c 026c 016e 0272  .......j.l.l.n.r
+00000510: 2c00 0000 6300 0000 0000 0000 0000 0000  ,...c...........
+00000520: 0008 0000 0007 0000 0043 0000 0073 d401  .........C...s..
+00000530: 0000 7400 6401 6402 6403 9c02 8301 7d00  ..t.d.d.d.....}.
+00000540: 7c00 a001 6404 6405 6901 a101 7d01 7c01  |...d.d.i...}.|.
+00000550: a002 a100 7d02 7c02 6406 1900 7d03 6407  ....}.|.d...}.d.
+00000560: 7d04 7c03 7c04 6b02 7d05 7c05 7341 7403  }.|.|.k.}.|.sAt.
+00000570: a004 6408 7c05 6601 6409 7c03 7c04 6602  ..d.|.f.d.|.|.f.
+00000580: a104 7403 a005 7c03 a101 7403 a005 7c04  ..t...|...t...|.
+00000590: a101 640a 9c02 1600 7d06 640b 640c 7c06  ..d.....}.d.d.|.
+000005a0: 6901 1600 7d07 7406 7403 a007 7c07 a101  i...}.t.t...|...
+000005b0: 8301 8201 6400 0400 7d03 0400 7d05 7d04  ....d...}...}.}.
+000005c0: 7c02 640d 1900 7d03 640e 7d04 7c03 7c04  |.d...}.d.}.|.|.
+000005d0: 6b02 7d05 7c05 7376 7403 a004 6408 7c05  k.}.|.svt...d.|.
+000005e0: 6601 6409 7c03 7c04 6602 a104 7403 a005  f.d.|.|.f...t...
+000005f0: 7c03 a101 7403 a005 7c04 a101 640a 9c02  |...t...|...d...
+00000600: 1600 7d06 640b 640c 7c06 6901 1600 7d07  ..}.d.d.|.i...}.
+00000610: 7406 7403 a007 7c07 a101 8301 8201 6400  t.t...|.......d.
+00000620: 0400 7d03 0400 7d05 7d04 7c02 640f 1900  ..}...}.}.|.d...
+00000630: 7d03 6401 7d04 7c03 7c04 6b02 7d05 7c05  }.d.}.|.|.k.}.|.
+00000640: 73ab 7403 a004 6408 7c05 6601 6409 7c03  s.t...d.|.f.d.|.
+00000650: 7c04 6602 a104 7403 a005 7c03 a101 7403  |.f...t...|...t.
+00000660: a005 7c04 a101 640a 9c02 1600 7d06 640b  ..|...d.....}.d.
+00000670: 640c 7c06 6901 1600 7d07 7406 7403 a007  d.|.i...}.t.t...
+00000680: 7c07 a101 8301 8201 6400 0400 7d03 0400  |.......d...}...
+00000690: 7d05 7d04 7c02 6410 1900 6404 1900 7d03  }.}.|.d...d...}.
+000006a0: 6405 7d04 7c03 7c04 6b02 7d05 7c05 73e2  d.}.|.|.k.}.|.s.
+000006b0: 7403 a004 6408 7c05 6601 6409 7c03 7c04  t...d.|.f.d.|.|.
+000006c0: 6602 a104 7403 a005 7c03 a101 7403 a005  f...t...|...t...
+000006d0: 7c04 a101 640a 9c02 1600 7d06 640b 640c  |...d.....}.d.d.
+000006e0: 7c06 6901 1600 7d07 7406 7403 a007 7c07  |.i...}.t.t...|.
+000006f0: a101 8301 8201 6400 0400 7d03 0400 7d05  ......d...}...}.
+00000700: 7d04 6400 5300 2911 4e72 0600 0000 7207  }.d.S.).Nr....r.
+00000710: 0000 0072 0800 0000 7209 0000 00da 036f  ...r....r......o
+00000720: 626a 720c 0000 0072 0d00 0000 720e 0000  bjr....r....r...
+00000730: 0072 1000 0000 7211 0000 0072 1400 0000  .r....r....r....
+00000740: 7215 0000 0072 1800 0000 da06 4163 6365  r....r......Acce
+00000750: 7074 da05 6163 746f 72da 066f 626a 6563  pt..actor..objec
+00000760: 7429 0872 0300 0000 da06 6163 6365 7074  t).r......accept
+00000770: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000780: 2000 0000 7221 0000 0072 2200 0000 2908   ...r!...r"...).
+00000790: 7223 0000 0072 3100 0000 7224 0000 0072  r#...r1...r$...r
+000007a0: 2500 0000 7226 0000 0072 2700 0000 7228  %...r&...r'...r(
+000007b0: 0000 0072 2900 0000 722a 0000 0072 2a00  ...r)...r*...r*.
+000007c0: 0000 722b 0000 00da 1c74 6573 745f 6163  ..r+.....test_ac
+000007d0: 7469 7669 7479 5f66 6163 746f 7279 5f61  tivity_factory_a
+000007e0: 6363 6570 7417 0000 0073 0e00 0000 0e01  ccept....s......
+000007f0: 0e02 0801 6a02 6a01 6a01 7201 7232 0000  ....j.j.j.r.r2..
+00000800: 0063 0000 0000 0000 0000 0000 0000 0800  .c..............
+00000810: 0000 0700 0000 4300 0000 7378 0100 0074  ......C...sx...t
+00000820: 0064 0164 0264 039c 0283 017d 0074 0164  .d.d.d.....}.t.d
+00000830: 0464 0164 0564 068d 03a0 02a1 00a0 03a1  .d.d.d..........
+00000840: 007d 017c 00a0 047c 01a1 01a0 03a1 007d  .}.|...|.......}
+00000850: 027c 0264 0719 007d 0364 0567 017d 047c  .|.d...}.d.g.}.|
+00000860: 037c 046b 027d 057c 0573 4974 05a0 0664  .|.k.}.|.sIt...d
+00000870: 087c 0566 0164 097c 037c 0466 02a1 0474  .|.f.d.|.|.f...t
+00000880: 05a0 077c 03a1 0174 05a0 077c 04a1 0164  ...|...t...|...d
+00000890: 0a9c 0216 007d 0664 0b64 0c7c 0669 0116  .....}.d.d.|.i..
+000008a0: 007d 0774 0874 05a0 097c 07a1 0183 0182  .}.t.t...|......
+000008b0: 0164 0004 007d 0304 007d 057d 047c 0264  .d...}...}.}.|.d
+000008c0: 0d19 007d 0364 0e67 017d 047c 037c 046b  ...}.d.g.}.|.|.k
+000008d0: 027d 057c 0573 7f74 05a0 0664 087c 0566  .}.|.s.t...d.|.f
+000008e0: 0164 097c 037c 0466 02a1 0474 05a0 077c  .d.|.|.f...t...|
+000008f0: 03a1 0174 05a0 077c 04a1 0164 0a9c 0216  ...t...|...d....
+00000900: 007d 0664 0b64 0c7c 0669 0116 007d 0774  .}.d.d.|.i...}.t
+00000910: 0874 05a0 097c 07a1 0183 0182 0164 0004  .t...|.......d..
+00000920: 007d 0304 007d 057d 047c 0264 0f19 007d  .}...}.}.|.d...}
+00000930: 0364 017d 047c 037c 046b 027d 057c 0573  .d.}.|.|.k.}.|.s
+00000940: b474 05a0 0664 087c 0566 0164 097c 037c  .t...d.|.f.d.|.|
+00000950: 0466 02a1 0474 05a0 077c 03a1 0174 05a0  .f...t...|...t..
+00000960: 077c 04a1 0164 0a9c 0216 007d 0664 0b64  .|...d.....}.d.d
+00000970: 0c7c 0669 0116 007d 0774 0874 05a0 097c  .|.i...}.t.t...|
+00000980: 07a1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
+00000990: 057d 0464 0053 0029 104e 7206 0000 0072  .}.d.S.).Nr....r
+000009a0: 0700 0000 7208 0000 00da 044e 6f74 65fa  ....r......Note.
+000009b0: 1161 6363 6f75 6e74 2f66 6f6c 6c6f 7765  .account/followe
+000009c0: 7273 2903 7218 0000 00da 0d61 7474 7269  rs).r......attri
+000009d0: 6275 7465 645f 746f 7207 0000 0072 1700  buted_tor....r..
+000009e0: 0000 720e 0000 0072 1000 0000 7211 0000  ..r....r....r...
+000009f0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000a00: 7a2c 6874 7470 733a 2f2f 7777 772e 7733  z,https://www.w3
+00000a10: 2e6f 7267 2f6e 732f 6163 7469 7669 7479  .org/ns/activity
+00000a20: 7374 7265 616d 7323 5075 626c 6963 722f  streams#Publicr/
+00000a30: 0000 0029 0a72 0300 0000 7204 0000 00da  ...).r....r.....
+00000a40: 0961 735f 7075 626c 6963 721d 0000 00da  .as_publicr.....
+00000a50: 0663 7265 6174 6572 1e00 0000 721f 0000  .creater....r...
+00000a60: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+00000a70: 2908 7223 0000 00da 046e 6f74 6572 2400  ).r#.....noter$.
+00000a80: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
+00000a90: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
+00000aa0: 722a 0000 0072 2b00 0000 da1c 7465 7374  r*...r+.....test
+00000ab0: 5f61 6374 6976 6974 795f 6661 6374 6f72  _activity_factor
+00000ac0: 795f 6372 6561 7465 2300 0000 7312 0000  y_create#...s...
+00000ad0: 000e 010c 0204 0104 0102 fd0e 066c 026c  .............l.l
+00000ae0: 016e 0172 3900 0000 6300 0000 0000 0000  .n.r9...c.......
+00000af0: 0000 0000 000b 0000 0007 0000 0043 0000  .............C..
+00000b00: 0073 8801 0000 7400 6401 6402 6403 9c02  .s....t.d.d.d...
+00000b10: 8301 7d00 6404 7d01 7401 6405 6401 6406  ..}.d.}.t.d.d.d.
+00000b20: 7c01 6801 6407 8d04 a002 a100 7d02 7c00  |.h.d.......}.|.
+00000b30: a003 7c02 a101 a002 a100 7d03 6408 7d04  ..|.......}.d.}.
+00000b40: 7c04 7c03 7601 7d05 7c05 7353 7404 a005  |.|.v.}.|.sSt...
+00000b50: 6409 7c05 6601 640a 7c04 7c03 6602 a104  d.|.f.d.|.|.f...
+00000b60: 7404 a006 7c04 a101 640b 7407 a008 a100  t...|...d.t.....
+00000b70: 7600 733c 7404 a009 7c03 a101 7241 7404  v.s<t...|...rAt.
+00000b80: a006 7c03 a101 6e01 640b 640c 9c02 1600  ..|...n.d.d.....
+00000b90: 7d06 640d 640e 7c06 6901 1600 7d07 740a  }.d.d.|.i...}.t.
+00000ba0: 7404 a00b 7c07 a101 8301 8201 6400 0400  t...|.......d...
+00000bb0: 7d04 7d05 7c03 640f 1900 7d04 7c01 6701  }.}.|.d...}.|.g.
+00000bc0: 7d08 7c04 7c08 6b02 7d05 7c05 7387 7404  }.|.|.k.}.|.s.t.
+00000bd0: a005 6410 7c05 6601 6411 7c04 7c08 6602  ..d.|.f.d.|.|.f.
+00000be0: a104 7404 a006 7c04 a101 7404 a006 7c08  ..t...|...t...|.
+00000bf0: a101 6412 9c02 1600 7d09 6413 6414 7c09  ..d.....}.d.d.|.
+00000c00: 6901 1600 7d0a 740a 7404 a00b 7c0a a101  i...}.t.t...|...
+00000c10: 8301 8201 6400 0400 7d04 0400 7d05 7d08  ....d...}...}.}.
+00000c20: 7c03 6415 1900 7d04 6401 7d08 7c04 7c08  |.d...}.d.}.|.|.
+00000c30: 6b02 7d05 7c05 73bc 7404 a005 6410 7c05  k.}.|.s.t...d.|.
+00000c40: 6601 6411 7c04 7c08 6602 a104 7404 a006  f.d.|.|.f...t...
+00000c50: 7c04 a101 7404 a006 7c08 a101 6412 9c02  |...t...|...d...
+00000c60: 1600 7d09 6413 6414 7c09 6901 1600 7d0a  ..}.d.d.|.i...}.
+00000c70: 740a 7404 a00b 7c0a a101 8301 8201 6400  t.t...|.......d.
+00000c80: 0400 7d04 0400 7d05 7d08 6400 5300 2916  ..}...}.}.d.S.).
+00000c90: 4e72 0600 0000 7207 0000 0072 0800 0000  Nr....r....r....
+00000ca0: 7a12 6874 7470 733a 2f2f 6162 656c 2f61  z.https://abel/a
+00000cb0: 6c69 6365 7233 0000 0072 3400 0000 2904  licer3...r4...).
+00000cc0: 7218 0000 0072 3500 0000 7207 0000 0072  r....r5...r....r
+00000cd0: 1600 0000 7217 0000 0029 01fa 066e 6f74  ....r....)...not
+00000ce0: 2069 6e29 017a 1625 2870 7931 2973 206e   in).z.%(py1)s n
+00000cf0: 6f74 2069 6e20 2528 7079 3329 7372 2400  ot in %(py3)sr$.
+00000d00: 0000 2902 7212 0000 00da 0370 7933 7a0e  ..).r......py3z.
+00000d10: 6173 7365 7274 2025 2870 7935 2973 da03  assert %(py5)s..
+00000d20: 7079 3572 1600 0000 720e 0000 0072 1000  py5r....r....r..
+00000d30: 0000 7211 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00000d40: 0072 2f00 0000 290c 7203 0000 0072 0400  .r/...).r....r..
+00000d50: 0000 721d 0000 0072 3700 0000 721e 0000  ..r....r7...r...
+00000d60: 0072 1f00 0000 7220 0000 00da 0c40 7079  .r....r .....@py
+00000d70: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
+00000d80: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
+00000d90: 676c 6f62 616c 5f6e 616d 6572 2100 0000  global_namer!...
+00000da0: 7222 0000 0029 0b72 2300 0000 da0c 7265  r"...).r#.....re
+00000db0: 6d6f 7465 5f61 6374 6f72 7238 0000 0072  mote_actorr8...r
+00000dc0: 2400 0000 7225 0000 0072 2700 0000 da0b  $...r%...r'.....
+00000dd0: 4070 795f 666f 726d 6174 34da 0b40 7079  @py_format4..@py
+00000de0: 5f66 6f72 6d61 7436 7226 0000 0072 2800  _format6r&...r(.
+00000df0: 0000 7229 0000 0072 2a00 0000 722a 0000  ..r)...r*...r*..
+00000e00: 0072 2b00 0000 da22 7465 7374 5f61 6374  .r+...."test_act
+00000e10: 6976 6974 795f 6661 6374 6f72 795f 6372  ivity_factory_cr
+00000e20: 6561 7465 5f6e 6f5f 6363 3200 0000 731c  eate_no_cc2...s.
+00000e30: 0000 000e 0104 0102 0102 0102 0102 0104  ................
+00000e40: 0104 fc04 0502 fb0e 0778 026c 016e 0172  .........x.l.n.r
+00000e50: 4300 0000 6300 0000 0000 0000 0000 0000  C...c...........
+00000e60: 0009 0000 0009 0000 0043 0000 0073 f600  .........C...s..
+00000e70: 0000 7400 6401 6402 6403 9c02 8301 7d00  ..t.d.d.d.....}.
+00000e80: 7c00 a001 6404 a101 a002 a100 7d01 7c01  |...d.......}.|.
+00000e90: 6a03 7d02 7c02 8300 7d03 7404 7c03 8301  j.}.|...}.t.|...
+00000ea0: 7d04 6800 6405 a301 7d05 7c04 7c05 6b02  }.h.d...}.|.|.k.
+00000eb0: 7d06 7c06 736f 7405 a006 6406 7c06 6601  }.|.sot...d.|.f.
+00000ec0: 6407 7c04 7c05 6602 a104 6408 7407 a008  d.|.|.f...d.t...
+00000ed0: a100 7600 7337 7405 a009 7404 a101 723c  ..v.s7t...t...r<
+00000ee0: 7405 a00a 7404 a101 6e01 6408 6409 7407  t...t...n.d.d.t.
+00000ef0: a008 a100 7600 7348 7405 a009 7c01 a101  ....v.sHt...|...
+00000f00: 724d 7405 a00a 7c01 a101 6e01 6409 7405  rMt...|...n.d.t.
+00000f10: a00a 7c02 a101 7405 a00a 7c03 a101 7405  ..|...t...|...t.
+00000f20: a00a 7c04 a101 7405 a00a 7c05 a101 640a  ..|...t...|...d.
+00000f30: 9c06 1600 7d07 640b 640c 7c07 6901 1600  ....}.d.d.|.i...
+00000f40: 7d08 740b 7405 a00c 7c08 a101 8301 8201  }.t.t...|.......
+00000f50: 6400 0400 7d02 0400 7d03 0400 7d04 0400  d...}...}...}...
+00000f60: 7d06 7d05 6400 5300 290d 4e72 0600 0000  }.}.d.S.).Nr....
+00000f70: 7207 0000 0072 0800 0000 720a 0000 003e  r....r....r....>
+00000f80: 0400 0000 722f 0000 0072 3000 0000 7218  ....r/...r0...r.
+00000f90: 0000 0072 0c00 0000 720e 0000 0029 017a  ...r....r....).z
+00000fa0: 6225 2870 7937 2973 0a7b 2528 7079 3729  b%(py7)s.{%(py7)
+00000fb0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
+00000fc0: 3529 730a 7b25 2870 7935 2973 203d 2025  5)s.{%(py5)s = %
+00000fd0: 2870 7933 2973 0a7b 2528 7079 3329 7320  (py3)s.{%(py3)s 
+00000fe0: 3d20 2528 7079 3129 732e 6b65 7973 0a7d  = %(py1)s.keys.}
+00000ff0: 2829 0a7d 290a 7d20 3d3d 2025 2870 7931  ().}).} == %(py1
+00001000: 3029 73da 0373 6574 7224 0000 0029 06da  0)s..setr$...)..
+00001010: 0370 7930 7212 0000 0072 3b00 0000 723c  .py0r....r;...r<
+00001020: 0000 00da 0370 7937 5a04 7079 3130 7a0f  .....py7Z.py10z.
+00001030: 6173 7365 7274 2025 2870 7931 3229 735a  assert %(py12)sZ
+00001040: 0470 7931 3229 0d72 0300 0000 da06 6465  .py12).r......de
+00001050: 6c65 7465 721d 0000 00da 046b 6579 7372  leter......keysr
+00001060: 4400 0000 721e 0000 0072 1f00 0000 723d  D...r....r....r=
+00001070: 0000 0072 3e00 0000 723f 0000 0072 2000  ...r>...r?...r .
+00001080: 0000 7221 0000 0072 2200 0000 2909 7223  ..r!...r"...).r#
+00001090: 0000 0072 2400 0000 7227 0000 00da 0b40  ...r$...r'.....@
+000010a0: 7079 5f61 7373 6572 7434 5a0b 4070 795f  py_assert4Z.@py_
+000010b0: 6173 7365 7274 365a 0b40 7079 5f61 7373  assert6Z.@py_ass
+000010c0: 6572 7439 5a0b 4070 795f 6173 7365 7274  ert9Z.@py_assert
+000010d0: 385a 0c40 7079 5f66 6f72 6d61 7431 315a  8Z.@py_format11Z
+000010e0: 0c40 7079 5f66 6f72 6d61 7431 3372 2a00  .@py_format13r*.
+000010f0: 0000 722a 0000 0072 2b00 0000 da1c 7465  ..r*...r+.....te
+00001100: 7374 5f61 6374 6976 6974 795f 6e6f 5f65  st_activity_no_e
+00001110: 6d70 7479 5f74 6f5f 6363 4300 0000 7306  mpty_to_ccC...s.
+00001120: 0000 000e 010e 02da 0272 4a00 0000 2902  .........rJ...).
+00001130: 7205 0000 004e 290f da08 6275 696c 7469  r....N)...builti
+00001140: 6e73 723d 0000 00da 195f 7079 7465 7374  nsr=....._pytest
+00001150: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
+00001160: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
+00001170: 6577 7269 7465 721e 0000 0072 2300 0000  ewriter....r#...
+00001180: 7203 0000 00da 0e6f 626a 6563 745f 6661  r......object_fa
+00001190: 6374 6f72 7972 0400 0000 722c 0000 0072  ctoryr....r,...r
+000011a0: 3200 0000 7239 0000 0072 4300 0000 724a  2...r9...rC...rJ
+000011b0: 0000 0072 2a00 0000 722a 0000 0072 2a00  ...r*...r*...r*.
+000011c0: 0000 722b 0000 00da 083c 6d6f 6475 6c65  ..r+.....<module
+000011d0: 3e01 0000 0073 0e00 0000 2600 0c01 0a03  >....s....&.....
+000011e0: 0a12 080c 0a0f 0e11                      ........
```

### Comparing `bovine-0.1.2/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1418 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,207 +1,208 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 8a05 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 a205 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
+00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
-00000060: 6405 6406 8400 5a0a 6407 6408 8400 5a0b  d.d...Z.d.d...Z.
-00000070: 6409 640a 8400 5a0c 6401 5300 290b e900  d.d...Z.d.S.)...
-00000080: 0000 004e 2901 da0a 5669 7369 6269 6c69  ...N)...Visibili
-00000090: 7479 e901 0000 0029 01da 0541 6374 6f72  ty.....)...Actor
-000000a0: 6300 0000 0000 0000 0000 0000 000d 0000  c...............
-000000b0: 0009 0000 0043 0000 0073 4203 0000 7400  .....C...sB...t.
-000000c0: 6401 6402 8d01 7d00 7c00 a001 a100 7d01  d.d...}.|.....}.
-000000d0: 7c01 6a02 7d02 7c02 8300 7d03 7403 7c03  |.j.}.|...}.t.|.
-000000e0: 8301 7d04 6800 6403 a301 7d05 7c04 7c05  ..}.h.d...}.|.|.
-000000f0: 6b02 7d06 7c06 736a 7404 a005 6404 7c06  k.}.|.sjt...d.|.
-00000100: 6601 6405 7c04 7c05 6602 a104 6406 7406  f.d.|.|.f...d.t.
-00000110: a007 a100 7600 7332 7404 a008 7403 a101  ....v.s2t...t...
-00000120: 7237 7404 a009 7403 a101 6e01 6406 6407  r7t...t...n.d.d.
-00000130: 7406 a007 a100 7600 7343 7404 a008 7c01  t.....v.sCt...|.
-00000140: a101 7248 7404 a009 7c01 a101 6e01 6407  ..rHt...|...n.d.
-00000150: 7404 a009 7c02 a101 7404 a009 7c03 a101  t...|...t...|...
-00000160: 7404 a009 7c04 a101 7404 a009 7c05 a101  t...|...t...|...
-00000170: 6408 9c06 1600 7d07 6409 640a 7c07 6901  d.....}.d.d.|.i.
-00000180: 1600 7d08 740a 7404 a00b 7c08 a101 8301  ..}.t.t...|.....
-00000190: 8201 6400 0400 7d02 0400 7d03 0400 7d04  ..d...}...}...}.
-000001a0: 0400 7d06 7d05 640b 7c00 5f0c 7c00 a001  ..}.}.d.|._.|...
-000001b0: a100 7d01 7c01 6a02 7d02 7c02 8300 7d03  ..}.|.j.}.|...}.
-000001c0: 7403 7c03 8301 7d04 6800 640c a301 7d05  t.|...}.h.d...}.
-000001d0: 7c04 7c05 6b02 7d06 7c06 73dc 7404 a005  |.|.k.}.|.s.t...
-000001e0: 6404 7c06 6601 6405 7c04 7c05 6602 a104  d.|.f.d.|.|.f...
-000001f0: 6406 7406 a007 a100 7600 73a4 7404 a008  d.t.....v.s.t...
-00000200: 7403 a101 72a9 7404 a009 7403 a101 6e01  t...r.t...t...n.
-00000210: 6406 6407 7406 a007 a100 7600 73b5 7404  d.d.t.....v.s.t.
-00000220: a008 7c01 a101 72ba 7404 a009 7c01 a101  ..|...r.t...|...
-00000230: 6e01 6407 7404 a009 7c02 a101 7404 a009  n.d.t...|...t...
-00000240: 7c03 a101 7404 a009 7c04 a101 7404 a009  |...t...|...t...
-00000250: 7c05 a101 6408 9c06 1600 7d07 6409 640a  |...d.....}.d.d.
-00000260: 7c07 6901 1600 7d08 740a 7404 a00b 7c08  |.i...}.t.t...|.
-00000270: a101 8301 8201 6400 0400 7d02 0400 7d03  ......d...}...}.
-00000280: 0400 7d04 0400 7d06 7d05 640d 7c00 5f0d  ..}...}.}.d.|._.
-00000290: 640e 7c00 5f0e 7c00 a001 a100 7d01 7c01  d.|._.|.....}.|.
-000002a0: 6a02 7d02 7c02 8300 7d03 7403 7c03 8301  j.}.|...}.t.|...
-000002b0: 7d04 6800 640f a301 7d05 7c04 7c05 6b02  }.h.d...}.|.|.k.
-000002c0: 7d06 7c06 9001 7356 7404 a005 6404 7c06  }.|...sVt...d.|.
-000002d0: 6601 6405 7c04 7c05 6602 a104 6406 7406  f.d.|.|.f...d.t.
-000002e0: a007 a100 7600 9001 731c 7404 a008 7403  ....v...s.t...t.
-000002f0: a101 9001 7221 7404 a009 7403 a101 6e01  ....r!t...t...n.
-00000300: 6406 6407 7406 a007 a100 7600 9001 732f  d.d.t.....v...s/
-00000310: 7404 a008 7c01 a101 9001 7234 7404 a009  t...|.....r4t...
-00000320: 7c01 a101 6e01 6407 7404 a009 7c02 a101  |...n.d.t...|...
-00000330: 7404 a009 7c03 a101 7404 a009 7c04 a101  t...|...t...|...
-00000340: 7404 a009 7c05 a101 6408 9c06 1600 7d07  t...|...d.....}.
-00000350: 6409 640a 7c07 6901 1600 7d08 740a 7404  d.d.|.i...}.t.t.
-00000360: a00b 7c08 a101 8301 8201 6400 0400 7d02  ..|.......d...}.
-00000370: 0400 7d03 0400 7d04 0400 7d06 7d05 7c01  ..}...}...}.}.|.
-00000380: 6410 1900 7d09 7c00 6a0f 6411 1700 7c00  d...}.|.j.d...|.
-00000390: 6a0f 7c00 6a0d 6412 9c03 7d0a 7c09 7c0a  j.|.j.d...}.|.|.
-000003a0: 6b02 7d02 7c02 9001 7399 7404 a005 6404  k.}.|...s.t...d.
-000003b0: 7c02 6601 6413 7c09 7c0a 6602 a104 7404  |.f.d.|.|.f...t.
-000003c0: a009 7c09 a101 7404 a009 7c0a a101 6414  ..|...t...|...d.
-000003d0: 9c02 1600 7d0b 6415 6416 7c0b 6901 1600  ....}.d.d.|.i...
-000003e0: 7d0c 740a 7404 a00b 7c0c a101 8301 8201  }.t.t...|.......
-000003f0: 6400 0400 7d09 0400 7d02 7d0a 6400 5300  d...}...}.}.d.S.
-00000400: 2917 4efa 1c68 7474 703a 2f2f 6578 616d  ).N..http://exam
-00000410: 706c 652e 636f 6d2f 6163 746f 722f 3132  ple.com/actor/12
-00000420: 3329 01da 0269 643e 0500 0000 da05 696e  3)...id>......in
-00000430: 626f 7872 0600 0000 da04 7479 7065 fa08  boxr......type..
-00000440: 4063 6f6e 7465 7874 da06 6f75 7462 6f78  @context..outbox
-00000450: a901 fa02 3d3d 2901 7a62 2528 7079 3729  ....==).zb%(py7)
-00000460: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
-00000470: 7930 2973 2825 2870 7935 2973 0a7b 2528  y0)s(%(py5)s.{%(
-00000480: 7079 3529 7320 3d20 2528 7079 3329 730a  py5)s = %(py3)s.
-00000490: 7b25 2870 7933 2973 203d 2025 2870 7931  {%(py3)s = %(py1
-000004a0: 2973 2e6b 6579 730a 7d28 290a 7d29 0a7d  )s.keys.}().}).}
-000004b0: 203d 3d20 2528 7079 3130 2973 da03 7365   == %(py10)s..se
-000004c0: 74da 0672 6573 756c 7429 06da 0370 7930  t..result)...py0
-000004d0: da03 7079 31da 0370 7933 da03 7079 35da  ..py1..py3..py5.
-000004e0: 0370 7937 da04 7079 3130 7a0f 6173 7365  .py7..py10z.asse
-000004f0: 7274 2025 2870 7931 3229 73da 0470 7931  rt %(py12)s..py1
-00000500: 327a 084a 6f68 6e20 446f 653e 0600 0000  2z.John Doe>....
-00000510: da04 6e61 6d65 7206 0000 0072 0700 0000  ..namer....r....
-00000520: 7208 0000 0072 0900 0000 720a 0000 005a  r....r....r....Z
-00000530: 1130 3132 3334 3536 3738 3930 3132 3334  .012345678901234
-00000540: 3536 da03 6b65 793e 0700 0000 7216 0000  56..key>....r...
-00000550: 0072 0600 0000 7207 0000 00da 0970 7562  .r....r......pub
-00000560: 6c69 634b 6579 7208 0000 0072 0900 0000  licKeyr....r....
-00000570: 720a 0000 0072 1800 0000 7a04 236b 6579  r....r....z.#key
-00000580: 2903 7206 0000 00da 056f 776e 6572 da0c  ).r......owner..
-00000590: 7075 626c 6963 4b65 7950 656d a901 7a12  publicKeyPem..z.
-000005a0: 2528 7079 3129 7320 3d3d 2025 2870 7934  %(py1)s == %(py4
-000005b0: 2973 a902 7210 0000 00da 0370 7934 fa0e  )s..r......py4..
-000005c0: 6173 7365 7274 2025 2870 7936 2973 da03  assert %(py6)s..
-000005d0: 7079 3629 1072 0400 0000 da05 6275 696c  py6).r......buil
-000005e0: 64da 046b 6579 7372 0d00 0000 da0a 4070  d..keysr......@p
-000005f0: 7974 6573 745f 6172 da11 5f63 616c 6c5f  ytest_ar.._call_
-00000600: 7265 7072 636f 6d70 6172 65da 0c40 7079  reprcompare..@py
-00000610: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
-00000620: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
-00000630: 676c 6f62 616c 5f6e 616d 65da 095f 7361  global_name.._sa
-00000640: 6665 7265 7072 da0e 4173 7365 7274 696f  ferepr..Assertio
-00000650: 6e45 7272 6f72 da13 5f66 6f72 6d61 745f  nError.._format_
-00000660: 6578 706c 616e 6174 696f 6e72 1600 0000  explanationr....
-00000670: da0a 7075 626c 6963 5f6b 6579 da0f 7075  ..public_key..pu
-00000680: 626c 6963 5f6b 6579 5f6e 616d 6572 0600  blic_key_namer..
-00000690: 0000 290d da05 6163 746f 7272 0e00 0000  ..)...actorr....
-000006a0: da0b 4070 795f 6173 7365 7274 32da 0b40  ..@py_assert2..@
-000006b0: 7079 5f61 7373 6572 7434 da0b 4070 795f  py_assert4..@py_
-000006c0: 6173 7365 7274 36da 0b40 7079 5f61 7373  assert6..@py_ass
-000006d0: 6572 7439 da0b 4070 795f 6173 7365 7274  ert9..@py_assert
-000006e0: 38da 0c40 7079 5f66 6f72 6d61 7431 31da  8..@py_format11.
-000006f0: 0c40 7079 5f66 6f72 6d61 7431 33da 0b40  .@py_format13..@
-00000700: 7079 5f61 7373 6572 7430 da0b 4070 795f  py_assert0..@py_
-00000710: 6173 7365 7274 33da 0b40 7079 5f66 6f72  assert3..@py_for
-00000720: 6d61 7435 da0b 4070 795f 666f 726d 6174  mat5..@py_format
-00000730: 37a9 0072 3800 0000 fa56 2f77 6f6f 6470  7..r8....V/woodp
-00000740: 6563 6b65 722f 7372 632f 636f 6465 6265  ecker/src/codebe
-00000750: 7267 2e6f 7267 2f62 6f76 696e 652f 626f  rg.org/bovine/bo
-00000760: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
-00000770: 6e65 2f61 6374 6976 6974 7973 7472 6561  ne/activitystrea
-00000780: 6d73 2f74 6573 745f 6163 746f 722e 7079  ms/test_actor.py
-00000790: da0a 7465 7374 5f61 6374 6f72 0600 0000  ..test_actor....
-000007a0: 739e 0000 000a 0108 02d6 0206 0208 01d6  s...............
-000007b0: 0106 0206 0108 0102 0202 0828 f802 080e  ...........(....
-000007c0: f802 0804 f804 0808 f802 0802 f802 0806  ................
-000007d0: f802 0802 f804 0806 f804 0808 f802 0802  ................
-000007e0: f802 0806 f802 0802 f804 0804 f802 0802  ................
-000007f0: f802 0802 f802 0802 f802 0802 f802 0802  ................
-00000800: f802 0802 f802 0802 f802 0818 f802 0802  ................
-00000810: f802 0818 f80a 0a02 0406 fc02 0402 fc02  ................
-00000820: 0416 fc02 040e fc02 0402 fc02 0402 fc02  ................
-00000830: 0402 fc02 0402 fc02 0418 fc02 0402 fc02  ................
-00000840: 0414 fc72 3a00 0000 6300 0000 0000 0000  ...r:...c.......
-00000850: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
-00000860: 0073 7001 0000 7400 6401 6402 6403 6404  .sp...t.d.d.d.d.
-00000870: 8d03 7d00 7c00 a001 a100 7d01 7c01 6402  ..}.|.....}.|.d.
-00000880: 1900 7d02 6402 7d03 7c02 7c03 6b02 7d04  ..}.d.}.|.|.k.}.
-00000890: 7c04 733a 7402 a003 6405 7c04 6601 6406  |.s:t...d.|.f.d.
-000008a0: 7c02 7c03 6602 a104 7402 a004 7c02 a101  |.|.f...t...|...
-000008b0: 7402 a004 7c03 a101 6407 9c02 1600 7d05  t...|...d.....}.
-000008c0: 6408 6409 7c05 6901 1600 7d06 7405 7402  d.d.|.i...}.t.t.
-000008d0: a006 7c06 a101 8301 8201 6400 0400 7d02  ..|.......d...}.
-000008e0: 0400 7d04 7d03 7c01 6403 1900 7d02 6403  ..}.}.|.d...}.d.
-000008f0: 7d03 7c02 7c03 6b02 7d04 7c04 736f 7402  }.|.|.k.}.|.sot.
-00000900: a003 6405 7c04 6601 6406 7c02 7c03 6602  ..d.|.f.d.|.|.f.
-00000910: a104 7402 a004 7c02 a101 7402 a004 7c03  ..t...|...t...|.
-00000920: a101 6407 9c02 1600 7d05 6408 6409 7c05  ..d.....}.d.d.|.
-00000930: 6901 1600 7d06 7405 7402 a006 7c06 a101  i...}.t.t...|...
-00000940: 8301 8201 6400 0400 7d02 0400 7d04 7d03  ....d...}...}.}.
-00000950: 640a 7c00 5f07 7c00 6a01 7408 6a09 640b  d.|._.|.j.t.j.d.
-00000960: 8d01 7d01 7c01 640c 1900 640d 1900 7d02  ..}.|.d...d...}.
-00000970: 640a 7d03 7c02 7c03 6b02 7d04 7c04 73b0  d.}.|.|.k.}.|.s.
-00000980: 7402 a003 6405 7c04 6601 6406 7c02 7c03  t...d.|.f.d.|.|.
-00000990: 6602 a104 7402 a004 7c02 a101 7402 a004  f...t...|...t...
-000009a0: 7c03 a101 6407 9c02 1600 7d05 6408 6409  |...d.....}.d.d.
-000009b0: 7c05 6901 1600 7d06 7405 7402 a006 7c06  |.i...}.t.t...|.
-000009c0: a101 8301 8201 6400 0400 7d02 0400 7d04  ......d...}...}.
-000009d0: 7d03 6400 5300 290e 4e72 0500 0000 7207  }.d.S.).Nr....r.
-000009e0: 0000 0072 0a00 0000 a903 7206 0000 0072  ...r......r....r
-000009f0: 0700 0000 720a 0000 0072 0b00 0000 721b  ....r....r....r.
-00000a00: 0000 0072 1c00 0000 721e 0000 0072 1f00  ...r....r....r..
-00000a10: 0000 7a18 6874 7470 3a2f 2f65 7861 6d70  ..z.http://examp
-00000a20: 6c65 2e63 6f6d 2f70 726f 7879 2901 da0a  le.com/proxy)...
-00000a30: 7669 7369 6269 6c69 7479 da09 656e 6470  visibility..endp
-00000a40: 6f69 6e74 73da 0870 726f 7879 5572 6c29  oints..proxyUrl)
-00000a50: 0a72 0400 0000 7220 0000 0072 2200 0000  .r....r ...r"...
-00000a60: 7223 0000 0072 2700 0000 7228 0000 0072  r#...r'...r(...r
-00000a70: 2900 0000 da09 7072 6f78 795f 7572 6c72  ).....proxy_urlr
-00000a80: 0200 0000 da05 4f57 4e45 52a9 0772 2c00  ......OWNER..r,.
-00000a90: 0000 720e 0000 0072 3400 0000 7235 0000  ..r....r4...r5..
-00000aa0: 0072 2d00 0000 7236 0000 0072 3700 0000  .r-...r6...r7...
-00000ab0: 7238 0000 0072 3800 0000 7239 0000 00da  r8...r8...r9....
-00000ac0: 1174 6573 745f 6163 746f 725f 7365 636f  .test_actor_seco
-00000ad0: 6e64 2600 0000 730e 0000 000e 0108 026a  nd&...s........j
-00000ae0: 026a 0106 020e 0172 0272 4200 0000 6300  .j.....r.rB...c.
-00000af0: 0000 0000 0000 0000 0000 0007 0000 0007  ................
-00000b00: 0000 0043 0000 0073 9200 0000 7400 6401  ...C...s....t.d.
-00000b10: 6402 6403 6404 8d03 7d00 6405 6406 6901  d.d.d...}.d.d.i.
-00000b20: 7c00 5f01 7c00 a002 a100 7d01 7c01 6407  |._.|.....}.|.d.
-00000b30: 1900 7d02 6405 6406 6901 7d03 7c02 7c03  ..}.d.d.i.}.|.|.
-00000b40: 6b02 7d04 7c04 7341 7403 a004 6408 7c04  k.}.|.sAt...d.|.
-00000b50: 6601 6409 7c02 7c03 6602 a104 7403 a005  f.d.|.|.f...t...
-00000b60: 7c02 a101 7403 a005 7c03 a101 640a 9c02  |...t...|...d...
-00000b70: 1600 7d05 640b 640c 7c05 6901 1600 7d06  ..}.d.d.|.i...}.
-00000b80: 7406 7403 a007 7c06 a101 8301 8201 6400  t.t...|.......d.
-00000b90: 0400 7d02 0400 7d04 7d03 6400 5300 290d  ..}...}.}.d.S.).
-00000ba0: 4e72 0500 0000 7207 0000 0072 0a00 0000  Nr....r....r....
-00000bb0: 723b 0000 0072 0800 0000 5a05 496d 6167  r;...r....Z.Imag
-00000bc0: 65da 0469 636f 6e72 0b00 0000 721b 0000  e..iconr....r...
-00000bd0: 0072 1c00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000be0: 2908 7204 0000 0072 4300 0000 7220 0000  ).r....rC...r ..
-00000bf0: 0072 2200 0000 7223 0000 0072 2700 0000  .r"...r#...r'...
-00000c00: 7228 0000 0072 2900 0000 7241 0000 0072  r(...r)...rA...r
-00000c10: 3800 0000 7238 0000 0072 3900 0000 da14  8...r8...r9.....
-00000c20: 7465 7374 5f61 6374 6f72 5f77 6974 685f  test_actor_with_
-00000c30: 6963 6f6e 3400 0000 7308 0000 000e 010a  icon4...s.......
-00000c40: 0108 0272 0272 4400 0000 290d da08 6275  ...r.rD...)...bu
-00000c50: 696c 7469 6e73 7224 0000 00da 195f 7079  iltinsr$....._py
-00000c60: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
-00000c70: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
-00000c80: 6eda 0772 6577 7269 7465 7222 0000 00da  n..rewriter"....
-00000c90: 0c62 6f76 696e 652e 7479 7065 7372 0200  .bovine.typesr..
-00000ca0: 0000 da00 7204 0000 0072 3a00 0000 7242  ....r....r:...rB
-00000cb0: 0000 0072 4400 0000 7238 0000 0072 3800  ...rD...r8...r8.
-00000cc0: 0000 7238 0000 0072 3900 0000 da08 3c6d  ..r8...r9.....<m
-00000cd0: 6f64 756c 653e 0100 0000 730a 0000 0026  odule>....s....&
-00000ce0: 000c 0208 0308 200c 0e                   ...... ..
+00000060: 640c 6406 6407 8404 5a0a 640c 6408 6409  d.d.d...Z.d.d.d.
+00000070: 8404 5a0b 640c 640a 640b 8404 5a0c 6401  ..Z.d.d.d...Z.d.
+00000080: 5300 290d e900 0000 004e 2901 da0a 5669  S.)......N)...Vi
+00000090: 7369 6269 6c69 7479 e901 0000 0029 01da  sibility.....)..
+000000a0: 0541 6374 6f72 da06 7265 7475 726e 6300  .Actor..returnc.
+000000b0: 0000 0000 0000 0000 0000 000d 0000 0009  ................
+000000c0: 0000 0043 0000 0073 4203 0000 7400 6401  ...C...sB...t.d.
+000000d0: 6402 8d01 7d00 7c00 a001 a100 7d01 7c01  d...}.|.....}.|.
+000000e0: 6a02 7d02 7c02 8300 7d03 7403 7c03 8301  j.}.|...}.t.|...
+000000f0: 7d04 6800 6403 a301 7d05 7c04 7c05 6b02  }.h.d...}.|.|.k.
+00000100: 7d06 7c06 736a 7404 a005 6404 7c06 6601  }.|.sjt...d.|.f.
+00000110: 6405 7c04 7c05 6602 a104 6406 7406 a007  d.|.|.f...d.t...
+00000120: a100 7600 7332 7404 a008 7403 a101 7237  ..v.s2t...t...r7
+00000130: 7404 a009 7403 a101 6e01 6406 6407 7406  t...t...n.d.d.t.
+00000140: a007 a100 7600 7343 7404 a008 7c01 a101  ....v.sCt...|...
+00000150: 7248 7404 a009 7c01 a101 6e01 6407 7404  rHt...|...n.d.t.
+00000160: a009 7c02 a101 7404 a009 7c03 a101 7404  ..|...t...|...t.
+00000170: a009 7c04 a101 7404 a009 7c05 a101 6408  ..|...t...|...d.
+00000180: 9c06 1600 7d07 6409 640a 7c07 6901 1600  ....}.d.d.|.i...
+00000190: 7d08 740a 7404 a00b 7c08 a101 8301 8201  }.t.t...|.......
+000001a0: 6400 0400 7d02 0400 7d03 0400 7d04 0400  d...}...}...}...
+000001b0: 7d06 7d05 640b 7c00 5f0c 7c00 a001 a100  }.}.d.|._.|.....
+000001c0: 7d01 7c01 6a02 7d02 7c02 8300 7d03 7403  }.|.j.}.|...}.t.
+000001d0: 7c03 8301 7d04 6800 640c a301 7d05 7c04  |...}.h.d...}.|.
+000001e0: 7c05 6b02 7d06 7c06 73dc 7404 a005 6404  |.k.}.|.s.t...d.
+000001f0: 7c06 6601 6405 7c04 7c05 6602 a104 6406  |.f.d.|.|.f...d.
+00000200: 7406 a007 a100 7600 73a4 7404 a008 7403  t.....v.s.t...t.
+00000210: a101 72a9 7404 a009 7403 a101 6e01 6406  ..r.t...t...n.d.
+00000220: 6407 7406 a007 a100 7600 73b5 7404 a008  d.t.....v.s.t...
+00000230: 7c01 a101 72ba 7404 a009 7c01 a101 6e01  |...r.t...|...n.
+00000240: 6407 7404 a009 7c02 a101 7404 a009 7c03  d.t...|...t...|.
+00000250: a101 7404 a009 7c04 a101 7404 a009 7c05  ..t...|...t...|.
+00000260: a101 6408 9c06 1600 7d07 6409 640a 7c07  ..d.....}.d.d.|.
+00000270: 6901 1600 7d08 740a 7404 a00b 7c08 a101  i...}.t.t...|...
+00000280: 8301 8201 6400 0400 7d02 0400 7d03 0400  ....d...}...}...
+00000290: 7d04 0400 7d06 7d05 640d 7c00 5f0d 640e  }...}.}.d.|._.d.
+000002a0: 7c00 5f0e 7c00 a001 a100 7d01 7c01 6a02  |._.|.....}.|.j.
+000002b0: 7d02 7c02 8300 7d03 7403 7c03 8301 7d04  }.|...}.t.|...}.
+000002c0: 6800 640f a301 7d05 7c04 7c05 6b02 7d06  h.d...}.|.|.k.}.
+000002d0: 7c06 9001 7356 7404 a005 6404 7c06 6601  |...sVt...d.|.f.
+000002e0: 6405 7c04 7c05 6602 a104 6406 7406 a007  d.|.|.f...d.t...
+000002f0: a100 7600 9001 731c 7404 a008 7403 a101  ..v...s.t...t...
+00000300: 9001 7221 7404 a009 7403 a101 6e01 6406  ..r!t...t...n.d.
+00000310: 6407 7406 a007 a100 7600 9001 732f 7404  d.t.....v...s/t.
+00000320: a008 7c01 a101 9001 7234 7404 a009 7c01  ..|.....r4t...|.
+00000330: a101 6e01 6407 7404 a009 7c02 a101 7404  ..n.d.t...|...t.
+00000340: a009 7c03 a101 7404 a009 7c04 a101 7404  ..|...t...|...t.
+00000350: a009 7c05 a101 6408 9c06 1600 7d07 6409  ..|...d.....}.d.
+00000360: 640a 7c07 6901 1600 7d08 740a 7404 a00b  d.|.i...}.t.t...
+00000370: 7c08 a101 8301 8201 6400 0400 7d02 0400  |.......d...}...
+00000380: 7d03 0400 7d04 0400 7d06 7d05 7c01 6410  }...}...}.}.|.d.
+00000390: 1900 7d09 7c00 6a0f 6411 1700 7c00 6a0f  ..}.|.j.d...|.j.
+000003a0: 7c00 6a0d 6412 9c03 7d0a 7c09 7c0a 6b02  |.j.d...}.|.|.k.
+000003b0: 7d02 7c02 9001 7399 7404 a005 6404 7c02  }.|...s.t...d.|.
+000003c0: 6601 6413 7c09 7c0a 6602 a104 7404 a009  f.d.|.|.f...t...
+000003d0: 7c09 a101 7404 a009 7c0a a101 6414 9c02  |...t...|...d...
+000003e0: 1600 7d0b 6415 6416 7c0b 6901 1600 7d0c  ..}.d.d.|.i...}.
+000003f0: 740a 7404 a00b 7c0c a101 8301 8201 6400  t.t...|.......d.
+00000400: 0400 7d09 0400 7d02 7d0a 6400 5300 2917  ..}...}.}.d.S.).
+00000410: 4efa 1c68 7474 703a 2f2f 6578 616d 706c  N..http://exampl
+00000420: 652e 636f 6d2f 6163 746f 722f 3132 3329  e.com/actor/123)
+00000430: 01da 0269 643e 0500 0000 fa08 4063 6f6e  ...id>......@con
+00000440: 7465 7874 da05 696e 626f 7872 0700 0000  text..inboxr....
+00000450: da06 6f75 7462 6f78 da04 7479 7065 a901  ..outbox..type..
+00000460: fa02 3d3d 2901 7a62 2528 7079 3729 730a  ..==).zb%(py7)s.
+00000470: 7b25 2870 7937 2973 203d 2025 2870 7930  {%(py7)s = %(py0
+00000480: 2973 2825 2870 7935 2973 0a7b 2528 7079  )s(%(py5)s.{%(py
+00000490: 3529 7320 3d20 2528 7079 3329 730a 7b25  5)s = %(py3)s.{%
+000004a0: 2870 7933 2973 203d 2025 2870 7931 2973  (py3)s = %(py1)s
+000004b0: 2e6b 6579 730a 7d28 290a 7d29 0a7d 203d  .keys.}().}).} =
+000004c0: 3d20 2528 7079 3130 2973 da03 7365 74da  = %(py10)s..set.
+000004d0: 0672 6573 756c 7429 06da 0370 7930 da03  .result)...py0..
+000004e0: 7079 31da 0370 7933 da03 7079 35da 0370  py1..py3..py5..p
+000004f0: 7937 da04 7079 3130 7a0f 6173 7365 7274  y7..py10z.assert
+00000500: 2025 2870 7931 3229 73da 0470 7931 327a   %(py12)s..py12z
+00000510: 084a 6f68 6e20 446f 653e 0600 0000 da04  .John Doe>......
+00000520: 6e61 6d65 7208 0000 0072 0900 0000 7207  namer....r....r.
+00000530: 0000 0072 0a00 0000 720b 0000 005a 1130  ...r....r....Z.0
+00000540: 3132 3334 3536 3738 3930 3132 3334 3536  1234567890123456
+00000550: da03 6b65 793e 0700 0000 7217 0000 0072  ..key>....r....r
+00000560: 0800 0000 7209 0000 0072 0700 0000 720a  ....r....r....r.
+00000570: 0000 00da 0970 7562 6c69 634b 6579 720b  .....publicKeyr.
+00000580: 0000 0072 1900 0000 7a04 236b 6579 2903  ...r....z.#key).
+00000590: 7207 0000 00da 056f 776e 6572 da0c 7075  r......owner..pu
+000005a0: 626c 6963 4b65 7950 656d a901 7a12 2528  blicKeyPem..z.%(
+000005b0: 7079 3129 7320 3d3d 2025 2870 7934 2973  py1)s == %(py4)s
+000005c0: a902 7211 0000 00da 0370 7934 fa0e 6173  ..r......py4..as
+000005d0: 7365 7274 2025 2870 7936 2973 da03 7079  sert %(py6)s..py
+000005e0: 3629 1072 0400 0000 da05 6275 696c 64da  6).r......build.
+000005f0: 046b 6579 7372 0e00 0000 da0a 4070 7974  .keysr......@pyt
+00000600: 6573 745f 6172 da11 5f63 616c 6c5f 7265  est_ar.._call_re
+00000610: 7072 636f 6d70 6172 65da 0c40 7079 5f62  prcompare..@py_b
+00000620: 7569 6c74 696e 73da 066c 6f63 616c 73da  uiltins..locals.
+00000630: 185f 7368 6f75 6c64 5f72 6570 725f 676c  ._should_repr_gl
+00000640: 6f62 616c 5f6e 616d 65da 095f 7361 6665  obal_name.._safe
+00000650: 7265 7072 da0e 4173 7365 7274 696f 6e45  repr..AssertionE
+00000660: 7272 6f72 da13 5f66 6f72 6d61 745f 6578  rror.._format_ex
+00000670: 706c 616e 6174 696f 6e72 1700 0000 da0a  planationr......
+00000680: 7075 626c 6963 5f6b 6579 da0f 7075 626c  public_key..publ
+00000690: 6963 5f6b 6579 5f6e 616d 6572 0700 0000  ic_key_namer....
+000006a0: 290d da05 6163 746f 7272 0f00 0000 da0b  )...actorr......
+000006b0: 4070 795f 6173 7365 7274 32da 0b40 7079  @py_assert2..@py
+000006c0: 5f61 7373 6572 7434 da0b 4070 795f 6173  _assert4..@py_as
+000006d0: 7365 7274 36da 0b40 7079 5f61 7373 6572  sert6..@py_asser
+000006e0: 7439 da0b 4070 795f 6173 7365 7274 38da  t9..@py_assert8.
+000006f0: 0c40 7079 5f66 6f72 6d61 7431 31da 0c40  .@py_format11..@
+00000700: 7079 5f66 6f72 6d61 7431 33da 0b40 7079  py_format13..@py
+00000710: 5f61 7373 6572 7430 da0b 4070 795f 6173  _assert0..@py_as
+00000720: 7365 7274 33da 0b40 7079 5f66 6f72 6d61  sert3..@py_forma
+00000730: 7435 da0b 4070 795f 666f 726d 6174 37a9  t5..@py_format7.
+00000740: 0072 3900 0000 fa56 2f77 6f6f 6470 6563  .r9....V/woodpec
+00000750: 6b65 722f 7372 632f 636f 6465 6265 7267  ker/src/codeberg
+00000760: 2e6f 7267 2f62 6f76 696e 652f 626f 7669  .org/bovine/bovi
+00000770: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
+00000780: 2f61 6374 6976 6974 7973 7472 6561 6d73  /activitystreams
+00000790: 2f74 6573 745f 6163 746f 722e 7079 da0a  /test_actor.py..
+000007a0: 7465 7374 5f61 6374 6f72 0600 0000 739e  test_actor....s.
+000007b0: 0000 000a 0108 02d6 0206 0208 01d6 0106  ................
+000007c0: 0206 0108 0102 0202 0828 f802 080e f802  .........(......
+000007d0: 0804 f804 0808 f802 0802 f802 0806 f802  ................
+000007e0: 0802 f804 0806 f804 0808 f802 0802 f802  ................
+000007f0: 0806 f802 0802 f804 0804 f802 0802 f802  ................
+00000800: 0802 f802 0802 f802 0802 f802 0802 f802  ................
+00000810: 0802 f802 0802 f802 0818 f802 0802 f802  ................
+00000820: 0818 f80a 0a02 0406 fc02 0402 fc02 0416  ................
+00000830: fc02 040e fc02 0402 fc02 0402 fc02 0402  ................
+00000840: fc02 0402 fc02 0418 fc02 0402 fc02 0414  ................
+00000850: fc72 3b00 0000 6300 0000 0000 0000 0000  .r;...c.........
+00000860: 0000 0007 0000 0007 0000 0043 0000 0073  ...........C...s
+00000870: 7001 0000 7400 6401 6402 6403 6404 8d03  p...t.d.d.d.d...
+00000880: 7d00 7c00 a001 a100 7d01 7c01 6402 1900  }.|.....}.|.d...
+00000890: 7d02 6402 7d03 7c02 7c03 6b02 7d04 7c04  }.d.}.|.|.k.}.|.
+000008a0: 733a 7402 a003 6405 7c04 6601 6406 7c02  s:t...d.|.f.d.|.
+000008b0: 7c03 6602 a104 7402 a004 7c02 a101 7402  |.f...t...|...t.
+000008c0: a004 7c03 a101 6407 9c02 1600 7d05 6408  ..|...d.....}.d.
+000008d0: 6409 7c05 6901 1600 7d06 7405 7402 a006  d.|.i...}.t.t...
+000008e0: 7c06 a101 8301 8201 6400 0400 7d02 0400  |.......d...}...
+000008f0: 7d04 7d03 7c01 6403 1900 7d02 6403 7d03  }.}.|.d...}.d.}.
+00000900: 7c02 7c03 6b02 7d04 7c04 736f 7402 a003  |.|.k.}.|.sot...
+00000910: 6405 7c04 6601 6406 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
+00000920: 7402 a004 7c02 a101 7402 a004 7c03 a101  t...|...t...|...
+00000930: 6407 9c02 1600 7d05 6408 6409 7c05 6901  d.....}.d.d.|.i.
+00000940: 1600 7d06 7405 7402 a006 7c06 a101 8301  ..}.t.t...|.....
+00000950: 8201 6400 0400 7d02 0400 7d04 7d03 640a  ..d...}...}.}.d.
+00000960: 7c00 5f07 7c00 6a01 7408 6a09 640b 8d01  |._.|.j.t.j.d...
+00000970: 7d01 7c01 640c 1900 640d 1900 7d02 640a  }.|.d...d...}.d.
+00000980: 7d03 7c02 7c03 6b02 7d04 7c04 73b0 7402  }.|.|.k.}.|.s.t.
+00000990: a003 6405 7c04 6601 6406 7c02 7c03 6602  ..d.|.f.d.|.|.f.
+000009a0: a104 7402 a004 7c02 a101 7402 a004 7c03  ..t...|...t...|.
+000009b0: a101 6407 9c02 1600 7d05 6408 6409 7c05  ..d.....}.d.d.|.
+000009c0: 6901 1600 7d06 7405 7402 a006 7c06 a101  i...}.t.t...|...
+000009d0: 8301 8201 6400 0400 7d02 0400 7d04 7d03  ....d...}...}.}.
+000009e0: 6400 5300 290e 4e72 0600 0000 7209 0000  d.S.).Nr....r...
+000009f0: 0072 0a00 0000 a903 7207 0000 0072 0900  .r......r....r..
+00000a00: 0000 720a 0000 0072 0c00 0000 721c 0000  ..r....r....r...
+00000a10: 0072 1d00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000a20: 7a18 6874 7470 3a2f 2f65 7861 6d70 6c65  z.http://example
+00000a30: 2e63 6f6d 2f70 726f 7879 2901 da0a 7669  .com/proxy)...vi
+00000a40: 7369 6269 6c69 7479 da09 656e 6470 6f69  sibility..endpoi
+00000a50: 6e74 73da 0870 726f 7879 5572 6c29 0a72  nts..proxyUrl).r
+00000a60: 0400 0000 7221 0000 0072 2300 0000 7224  ....r!...r#...r$
+00000a70: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+00000a80: 0000 da09 7072 6f78 795f 7572 6c72 0200  ....proxy_urlr..
+00000a90: 0000 da05 4f57 4e45 52a9 0772 2d00 0000  ....OWNER..r-...
+00000aa0: 720f 0000 0072 3500 0000 7236 0000 0072  r....r5...r6...r
+00000ab0: 2e00 0000 7237 0000 0072 3800 0000 7239  ....r7...r8...r9
+00000ac0: 0000 0072 3900 0000 723a 0000 00da 1174  ...r9...r:.....t
+00000ad0: 6573 745f 6163 746f 725f 7365 636f 6e64  est_actor_second
+00000ae0: 2600 0000 730e 0000 000e 0108 026a 026a  &...s........j.j
+00000af0: 0106 020e 0172 0272 4300 0000 6300 0000  .....r.rC...c...
+00000b00: 0000 0000 0000 0000 0007 0000 0007 0000  ................
+00000b10: 0043 0000 0073 9200 0000 7400 6401 6402  .C...s....t.d.d.
+00000b20: 6403 6404 8d03 7d00 6405 6406 6901 7c00  d.d...}.d.d.i.|.
+00000b30: 5f01 7c00 a002 a100 7d01 7c01 6407 1900  _.|.....}.|.d...
+00000b40: 7d02 6405 6406 6901 7d03 7c02 7c03 6b02  }.d.d.i.}.|.|.k.
+00000b50: 7d04 7c04 7341 7403 a004 6408 7c04 6601  }.|.sAt...d.|.f.
+00000b60: 6409 7c02 7c03 6602 a104 7403 a005 7c02  d.|.|.f...t...|.
+00000b70: a101 7403 a005 7c03 a101 640a 9c02 1600  ..t...|...d.....
+00000b80: 7d05 640b 640c 7c05 6901 1600 7d06 7406  }.d.d.|.i...}.t.
+00000b90: 7403 a007 7c06 a101 8301 8201 6400 0400  t...|.......d...
+00000ba0: 7d02 0400 7d04 7d03 6400 5300 290d 4e72  }...}.}.d.S.).Nr
+00000bb0: 0600 0000 7209 0000 0072 0a00 0000 723c  ....r....r....r<
+00000bc0: 0000 0072 0b00 0000 5a05 496d 6167 65da  ...r....Z.Image.
+00000bd0: 0469 636f 6e72 0c00 0000 721c 0000 0072  .iconr....r....r
+00000be0: 1d00 0000 721f 0000 0072 2000 0000 2908  ....r....r ...).
+00000bf0: 7204 0000 0072 4400 0000 7221 0000 0072  r....rD...r!...r
+00000c00: 2300 0000 7224 0000 0072 2800 0000 7229  #...r$...r(...r)
+00000c10: 0000 0072 2a00 0000 7242 0000 0072 3900  ...r*...rB...r9.
+00000c20: 0000 7239 0000 0072 3a00 0000 da14 7465  ..r9...r:.....te
+00000c30: 7374 5f61 6374 6f72 5f77 6974 685f 6963  st_actor_with_ic
+00000c40: 6f6e 3400 0000 7308 0000 000e 010a 0108  on4...s.........
+00000c50: 0272 0272 4500 0000 2902 7205 0000 004e  .r.rE...).r....N
+00000c60: 290d da08 6275 696c 7469 6e73 7225 0000  )...builtinsr%..
+00000c70: 00da 195f 7079 7465 7374 2e61 7373 6572  ..._pytest.asser
+00000c80: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
+00000c90: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
+00000ca0: 7223 0000 00da 0c62 6f76 696e 652e 7479  r#.....bovine.ty
+00000cb0: 7065 7372 0200 0000 da00 7204 0000 0072  pesr......r....r
+00000cc0: 3b00 0000 7243 0000 0072 4500 0000 7239  ;...rC...rE...r9
+00000cd0: 0000 0072 3900 0000 7239 0000 0072 3a00  ...r9...r9...r:.
+00000ce0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000cf0: 730a 0000 0026 000c 020a 030a 200e 0e    s....&...... ..
```

### Comparing `bovine-0.1.2/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1381 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,198 +1,200 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 6505 0000  o.........Ade...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 7505 0000  o.......*.Ndu...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
+00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6403 6404  d.d.l.m.Z...d.d.
-00000060: 6c09 6d0a 5a0a 0100 6405 6406 8400 5a0b  l.m.Z...d.d...Z.
-00000070: 6407 6408 8400 5a0c 6401 5300 2909 e900  d.d...Z.d.S.)...
-00000080: 0000 004e 2901 da09 4173 796e 634d 6f63  ...N)...AsyncMoc
-00000090: 6be9 0100 0000 2901 da0d 4f62 6a65 6374  k.....)...Object
-000000a0: 4661 6374 6f72 7963 0000 0000 0000 0000  Factoryc........
-000000b0: 0000 0000 0e00 0000 0900 0000 4300 0000  ............C...
-000000c0: 73da 0100 0074 0064 0164 0264 039c 0283  s....t.d.d.d....
-000000d0: 017d 007c 00a0 01a1 00a0 02a1 007d 0164  .}.|.........}.d
-000000e0: 047c 015f 037c 01a0 04a1 007d 027c 026a  .|._.|.....}.|.j
-000000f0: 057d 037c 0383 007d 0474 067c 0483 017d  .}.|...}.t.|...}
-00000100: 0568 0064 05a3 017d 067c 057c 066b 027d  .h.d...}.|.|.k.}
-00000110: 077c 0773 7574 07a0 0864 067c 0766 0164  .|.sut...d.|.f.d
-00000120: 077c 057c 0666 02a1 0464 0874 09a0 0aa1  .|.|.f...d.t....
-00000130: 0076 0073 3d74 07a0 0b74 06a1 0172 4274  .v.s=t...t...rBt
-00000140: 07a0 0c74 06a1 016e 0164 0864 0974 09a0  ...t...n.d.d.t..
-00000150: 0aa1 0076 0073 4e74 07a0 0b7c 02a1 0172  ...v.sNt...|...r
-00000160: 5374 07a0 0c7c 02a1 016e 0164 0974 07a0  St...|...n.d.t..
-00000170: 0c7c 03a1 0174 07a0 0c7c 04a1 0174 07a0  .|...t...|...t..
-00000180: 0c7c 05a1 0174 07a0 0c7c 06a1 0164 0a9c  .|...t...|...d..
-00000190: 0616 007d 0864 0b64 0c7c 0869 0116 007d  ...}.d.d.|.i...}
-000001a0: 0974 0d74 07a0 0e7c 09a1 0183 0182 0164  .t.t...|.......d
-000001b0: 0004 007d 0304 007d 0404 007d 0504 007d  ...}...}...}...}
-000001c0: 077d 067c 0264 0d19 007d 0a64 0e67 017d  .}.|.d...}.d.g.}
-000001d0: 0b7c 0a7c 0b6b 027d 037c 0373 af74 07a0  .|.|.k.}.|.s.t..
-000001e0: 0864 067c 0366 0164 0f7c 0a7c 0b66 02a1  .d.|.f.d.|.|.f..
-000001f0: 0474 07a0 0c7c 0aa1 0174 07a0 0c7c 0ba1  .t...|...t...|..
-00000200: 0164 109c 0216 007d 0c64 1164 127c 0c69  .d.....}.d.d.|.i
-00000210: 0116 007d 0d74 0d74 07a0 0e7c 0da1 0183  ...}.t.t...|....
-00000220: 0182 0164 0004 007d 0a04 007d 037d 0b7c  ...d...}...}.}.|
-00000230: 0264 1319 007d 0a64 0267 017d 0b7c 0a7c  .d...}.d.g.}.|.|
-00000240: 0b6b 027d 037c 0373 e574 07a0 0864 067c  .k.}.|.s.t...d.|
-00000250: 0366 0164 0f7c 0a7c 0b66 02a1 0474 07a0  .f.d.|.|.f...t..
-00000260: 0c7c 0aa1 0174 07a0 0c7c 0ba1 0164 109c  .|...t...|...d..
-00000270: 0216 007d 0c64 1164 127c 0c69 0116 007d  ...}.d.d.|.i...}
-00000280: 0d74 0d74 07a0 0e7c 0da1 0183 0182 0164  .t.t...|.......d
-00000290: 0004 007d 0a04 007d 037d 0b64 0053 0029  ...}...}.}.d.S.)
-000002a0: 144e da08 6163 746f 725f 6964 da09 666f  .N..actor_id..fo
-000002b0: 6c6c 6f77 6572 7329 02da 0269 6472 0600  llowers)...idr..
-000002c0: 0000 da04 7465 7874 3e06 0000 00da 0263  ....text>......c
-000002d0: 63da 0763 6f6e 7465 6e74 da04 7479 7065  c..content..type
-000002e0: da0c 6174 7472 6962 7574 6564 546f fa08  ..attributedTo..
-000002f0: 4063 6f6e 7465 7874 da02 746f a901 fa02  @context..to....
-00000300: 3d3d a901 7a62 2528 7079 3729 730a 7b25  ==..zb%(py7)s.{%
-00000310: 2870 7937 2973 203d 2025 2870 7930 2973  (py7)s = %(py0)s
-00000320: 2825 2870 7935 2973 0a7b 2528 7079 3529  (%(py5)s.{%(py5)
-00000330: 7320 3d20 2528 7079 3329 730a 7b25 2870  s = %(py3)s.{%(p
-00000340: 7933 2973 203d 2025 2870 7931 2973 2e6b  y3)s = %(py1)s.k
-00000350: 6579 730a 7d28 290a 7d29 0a7d 203d 3d20  eys.}().}).} == 
-00000360: 2528 7079 3130 2973 da03 7365 74da 0672  %(py10)s..set..r
-00000370: 6573 756c 74a9 06da 0370 7930 da03 7079  esult....py0..py
-00000380: 31da 0370 7933 da03 7079 35da 0370 7937  1..py3..py5..py7
-00000390: da04 7079 3130 fa0f 6173 7365 7274 2025  ..py10..assert %
-000003a0: 2870 7931 3229 73da 0470 7931 3272 0e00  (py12)s..py12r..
-000003b0: 0000 7a2c 6874 7470 733a 2f2f 7777 772e  ..z,https://www.
-000003c0: 7733 2e6f 7267 2f6e 732f 6163 7469 7669  w3.org/ns/activi
-000003d0: 7479 7374 7265 616d 7323 5075 626c 6963  tystreams#Public
-000003e0: a901 7a12 2528 7079 3129 7320 3d3d 2025  ..z.%(py1)s == %
-000003f0: 2870 7934 2973 a902 7216 0000 00da 0370  (py4)s..r......p
-00000400: 7934 fa0e 6173 7365 7274 2025 2870 7936  y4..assert %(py6
-00000410: 2973 da03 7079 3672 0900 0000 290f 7204  )s..py6r....).r.
-00000420: 0000 00da 046e 6f74 65da 0961 735f 7075  .....note..as_pu
-00000430: 626c 6963 720a 0000 00da 0562 7569 6c64  blicr......build
-00000440: da04 6b65 7973 7212 0000 00da 0a40 7079  ..keysr......@py
-00000450: 7465 7374 5f61 72da 115f 6361 6c6c 5f72  test_ar.._call_r
-00000460: 6570 7263 6f6d 7061 7265 da0c 4070 795f  eprcompare..@py_
-00000470: 6275 696c 7469 6e73 da06 6c6f 6361 6c73  builtins..locals
-00000480: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
-00000490: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
-000004a0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
-000004b0: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
-000004c0: 7870 6c61 6e61 7469 6f6e 290e da0e 6f62  xplanation)...ob
-000004d0: 6a65 6374 5f66 6163 746f 7279 7222 0000  ject_factoryr"..
-000004e0: 0072 1300 0000 da0b 4070 795f 6173 7365  .r......@py_asse
-000004f0: 7274 32da 0b40 7079 5f61 7373 6572 7434  rt2..@py_assert4
-00000500: da0b 4070 795f 6173 7365 7274 36da 0b40  ..@py_assert6..@
-00000510: 7079 5f61 7373 6572 7439 da0b 4070 795f  py_assert9..@py_
-00000520: 6173 7365 7274 38da 0c40 7079 5f66 6f72  assert8..@py_for
-00000530: 6d61 7431 31da 0c40 7079 5f66 6f72 6d61  mat11..@py_forma
-00000540: 7431 33da 0b40 7079 5f61 7373 6572 7430  t13..@py_assert0
-00000550: da0b 4070 795f 6173 7365 7274 33da 0b40  ..@py_assert3..@
-00000560: 7079 5f66 6f72 6d61 7435 da0b 4070 795f  py_format5..@py_
-00000570: 666f 726d 6174 37a9 0072 3a00 0000 fa5f  format7..r:...._
-00000580: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
-00000590: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
-000005a0: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
-000005b0: 652f 626f 7669 6e65 2f61 6374 6976 6974  e/bovine/activit
-000005c0: 7973 7472 6561 6d73 2f74 6573 745f 6f62  ystreams/test_ob
-000005d0: 6a65 6374 5f66 6163 746f 7279 2e70 79da  ject_factory.py.
-000005e0: 1374 6573 745f 6f62 6a65 6374 5f66 6163  .test_object_fac
-000005f0: 746f 7279 0700 0000 736a 0000 000e 010c  tory....sj......
-00000600: 0206 0108 0102 0202 0726 f902 070e f902  .........&......
-00000610: 0704 f904 0706 f902 0702 f902 0704 f902  ................
-00000620: 0702 f904 0706 f904 0706 f902 0702 f902  ................
-00000630: 0704 f902 0702 f904 0704 f902 0702 f902  ................
-00000640: 0702 f902 0702 f902 0702 f902 0702 f902  ................
-00000650: 0702 f902 0702 f902 0718 f902 0702 f902  ................
-00000660: 0718 f96c 0970 0172 3c00 0000 6300 0000  ...l.p.r<...c...
-00000670: 0000 0000 0000 0000 0013 0000 0009 0000  ................
-00000680: 00c3 0000 0073 8402 0000 8101 7400 8300  .....s......t...
-00000690: 7d00 7400 8300 7d01 6401 7d02 7c01 7c00  }.t...}.d.}.|.|.
-000006a0: 6a01 6a02 5f03 7404 a005 6402 7c02 6403  j.j._.t...d.|.d.
-000006b0: 6404 6405 9c04 a101 7c01 6a06 5f03 7407  d.d.....|.j._.t.
-000006c0: 7c00 6406 8d01 7d03 7c03 a008 7c02 a101  |.d...}.|...|...
-000006d0: 4900 6400 4800 7d04 7c04 a009 a100 7d05  I.d.H.}.|.....}.
-000006e0: 7c05 6a0a 7d06 7c06 8300 7d07 740b 7c07  |.j.}.|...}.t.|.
-000006f0: 8301 7d08 6800 6407 a301 7d09 7c08 7c09  ..}.h.d...}.|.|.
-00000700: 6b02 7d0a 7c0a 738c 740c a00d 6408 7c0a  k.}.|.s.t...d.|.
-00000710: 6601 6409 7c08 7c09 6602 a104 640a 740e  f.d.|.|.f...d.t.
-00000720: a00f a100 7600 7354 740c a010 740b a101  ....v.sTt...t...
-00000730: 7259 740c a011 740b a101 6e01 640a 640b  rYt...t...n.d.d.
-00000740: 740e a00f a100 7600 7365 740c a010 7c05  t.....v.set...|.
-00000750: a101 726a 740c a011 7c05 a101 6e01 640b  ..rjt...|...n.d.
-00000760: 740c a011 7c06 a101 740c a011 7c07 a101  t...|...t...|...
-00000770: 740c a011 7c08 a101 740c a011 7c09 a101  t...|...t...|...
-00000780: 640c 9c06 1600 7d0b 640d 640e 7c0b 6901  d.....}.d.d.|.i.
-00000790: 1600 7d0c 7412 740c a013 7c0c a101 8301  ..}.t.t...|.....
-000007a0: 8201 6400 0400 7d06 0400 7d07 0400 7d08  ..d...}...}...}.
-000007b0: 0400 7d0a 7d09 7c05 640f 1900 7d0d 6410  ..}.}.|.d...}.d.
-000007c0: 7d0e 7c0d 7c0e 6b02 7d06 7c06 73c5 740c  }.|.|.k.}.|.s.t.
-000007d0: a00d 6408 7c06 6601 6411 7c0d 7c0e 6602  ..d.|.f.d.|.|.f.
-000007e0: a104 740c a011 7c0d a101 740c a011 7c0e  ..t...|...t...|.
-000007f0: a101 6412 9c02 1600 7d0f 6413 6414 7c0f  ..d.....}.d.d.|.
-00000800: 6901 1600 7d10 7412 740c a013 7c10 a101  i...}.t.t...|...
-00000810: 8301 8201 6400 0400 7d0d 0400 7d06 7d0e  ....d...}...}.}.
-00000820: 7c05 6415 1900 7d0d 7c0d 7c02 6b02 7d06  |.d...}.|.|.k.}.
-00000830: 7c06 9001 7306 740c a00d 6408 7c06 6601  |...s.t...d.|.f.
-00000840: 6416 7c0d 7c02 6602 a104 740c a011 7c0d  d.|.|.f...t...|.
-00000850: a101 6417 740e a00f a100 7600 73ef 740c  ..d.t.....v.s.t.
-00000860: a010 7c02 a101 72f4 740c a011 7c02 a101  ..|...r.t...|...
-00000870: 6e01 6417 6418 9c02 1600 7d11 6419 641a  n.d.d.....}.d.d.
-00000880: 7c11 6901 1600 7d12 7412 740c a013 7c12  |.i...}.t.t...|.
-00000890: a101 8301 8201 6400 0400 7d0d 7d06 7c05  ......d...}.}.|.
-000008a0: 641b 1900 7d0d 641c 7d0e 7c0d 7c0e 6b02  d...}.d.}.|.|.k.
-000008b0: 7d06 7c06 9001 733a 740c a00d 6408 7c06  }.|...s:t...d.|.
-000008c0: 6601 6411 7c0d 7c0e 6602 a104 740c a011  f.d.|.|.f...t...
-000008d0: 7c0d a101 740c a011 7c0e a101 6412 9c02  |...t...|...d...
-000008e0: 1600 7d0f 6413 6414 7c0f 6901 1600 7d10  ..}.d.d.|.i...}.
-000008f0: 7412 740c a013 7c10 a101 8301 8201 6400  t.t...|.......d.
-00000900: 0400 7d0d 0400 7d06 7d0e 6400 5300 291d  ..}...}.}.d.S.).
-00000910: 4e7a 1468 7474 7073 3a2f 2f72 656d 6f74  Nz.https://remot
-00000920: 652f 616c 6963 657a 2568 7474 7073 3a2f  e/alicez%https:/
-00000930: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
-00000940: 6374 6976 6974 7973 7472 6561 6d73 da06  ctivitystreams..
-00000950: 5065 7273 6f6e 5a06 616c 7973 7361 2904  PersonZ.alyssa).
-00000960: 720d 0000 0072 0700 0000 720b 0000 00da  r....r....r.....
-00000970: 1170 7265 6665 7272 6564 5573 6572 6e61  .preferredUserna
-00000980: 6d65 2901 da06 636c 6965 6e74 3e04 0000  me)...client>...
-00000990: 0072 0d00 0000 da04 6e61 6d65 720b 0000  .r......namer...
-000009a0: 00da 0468 7265 6672 0f00 0000 7211 0000  ...hrefr....r...
-000009b0: 0072 1200 0000 da07 6d65 6e74 696f 6e72  .r......mentionr
-000009c0: 1400 0000 721b 0000 0072 1c00 0000 720b  ....r....r....r.
-000009d0: 0000 00da 074d 656e 7469 6f6e 721d 0000  .....Mentionr...
-000009e0: 0072 1e00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-000009f0: 7241 0000 0029 017a 1225 2870 7931 2973  rA...).z.%(py1)s
-00000a00: 203d 3d20 2528 7079 3329 73da 0a72 656d   == %(py3)s..rem
-00000a10: 6f74 655f 7572 6929 0272 1600 0000 7217  ote_uri).r....r.
-00000a20: 0000 007a 0e61 7373 6572 7420 2528 7079  ...z.assert %(py
-00000a30: 3529 7372 1800 0000 7240 0000 007a 0d61  5)sr....r@...z.a
-00000a40: 6c79 7373 6140 7265 6d6f 7465 2914 7202  lyssa@remote).r.
-00000a50: 0000 0072 3f00 0000 da03 6765 74da 0c72  ...r?.....get..r
-00000a60: 6574 7572 6e5f 7661 6c75 65da 046a 736f  eturn_value..jso
-00000a70: 6eda 0564 756d 7073 7208 0000 0072 0400  n..dumpsr....r..
-00000a80: 0000 da15 6d65 6e74 696f 6e5f 666f 725f  ....mention_for_
-00000a90: 6163 746f 725f 7572 6972 2400 0000 7225  actor_urir$...r%
-00000aa0: 0000 0072 1200 0000 7226 0000 0072 2700  ...r....r&...r'.
-00000ab0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-00000ac0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
-00000ad0: 2913 5a0b 6d6f 636b 5f63 6c69 656e 745a  ).Z.mock_clientZ
-00000ae0: 0d6d 6f63 6b5f 7265 7370 6f6e 7365 7244  .mock_responserD
-00000af0: 0000 0072 2e00 0000 5a0e 6d65 6e74 696f  ...r....Z.mentio
-00000b00: 6e5f 6f62 6a65 6374 7242 0000 0072 2f00  n_objectrB...r/.
-00000b10: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
-00000b20: 0072 3300 0000 7234 0000 0072 3500 0000  .r3...r4...r5...
-00000b30: 7236 0000 0072 3700 0000 7238 0000 0072  r6...r7...r8...r
-00000b40: 3900 0000 da0b 4070 795f 666f 726d 6174  9.....@py_format
-00000b50: 34da 0b40 7079 5f66 6f72 6d61 7436 723a  4..@py_format6r:
-00000b60: 0000 0072 3a00 0000 723b 0000 00da 1a74  ...r:...r;.....t
-00000b70: 6573 745f 6d65 6e74 696f 6e5f 666f 725f  est_mention_for_
-00000b80: 6163 746f 725f 7572 691b 0000 0073 2600  actor_uri....s&.
-00000b90: 0000 0280 0601 0601 0401 0a02 0402 0202  ................
-00000ba0: 0201 0201 0201 04fc 08ff 0a09 1002 0801  ................
-00000bb0: d602 6a01 7e01 7001 724c 0000 0029 0dda  ..j.~.p.rL...)..
-00000bc0: 0862 7569 6c74 696e 7372 2800 0000 da19  .builtinsr(.....
-00000bd0: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
-00000be0: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
-00000bf0: 7469 6f6e da07 7265 7772 6974 6572 2600  tion..rewriter&.
-00000c00: 0000 7247 0000 00da 0d75 6e69 7474 6573  ..rG.....unittes
-00000c10: 742e 6d6f 636b 7202 0000 0072 2e00 0000  t.mockr....r....
-00000c20: 7204 0000 0072 3c00 0000 724c 0000 0072  r....r<...rL...r
-00000c30: 3a00 0000 723a 0000 0072 3a00 0000 723b  :...r:...r:...r;
-00000c40: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000c50: 0073 0a00 0000 2200 0c01 0c02 0803 0c14  .s....".........
+00000060: 6c09 6d0a 5a0a 0100 640a 6406 6407 8404  l.m.Z...d.d.d...
+00000070: 5a0b 640a 6408 6409 8404 5a0c 6401 5300  Z.d.d.d...Z.d.S.
+00000080: 290b e900 0000 004e 2901 da09 4173 796e  )......N)...Asyn
+00000090: 634d 6f63 6be9 0100 0000 2901 da0d 4f62  cMock.....)...Ob
+000000a0: 6a65 6374 4661 6374 6f72 79da 0672 6574  jectFactory..ret
+000000b0: 7572 6e63 0000 0000 0000 0000 0000 0000  urnc............
+000000c0: 0e00 0000 0900 0000 4300 0000 73da 0100  ........C...s...
+000000d0: 0074 0064 0164 0264 039c 0283 017d 007c  .t.d.d.d.....}.|
+000000e0: 00a0 01a1 00a0 02a1 007d 0164 047c 015f  .........}.d.|._
+000000f0: 037c 01a0 04a1 007d 027c 026a 057d 037c  .|.....}.|.j.}.|
+00000100: 0383 007d 0474 067c 0483 017d 0568 0064  ...}.t.|...}.h.d
+00000110: 05a3 017d 067c 057c 066b 027d 077c 0773  ...}.|.|.k.}.|.s
+00000120: 7574 07a0 0864 067c 0766 0164 077c 057c  ut...d.|.f.d.|.|
+00000130: 0666 02a1 0464 0874 09a0 0aa1 0076 0073  .f...d.t.....v.s
+00000140: 3d74 07a0 0b74 06a1 0172 4274 07a0 0c74  =t...t...rBt...t
+00000150: 06a1 016e 0164 0864 0974 09a0 0aa1 0076  ...n.d.d.t.....v
+00000160: 0073 4e74 07a0 0b7c 02a1 0172 5374 07a0  .sNt...|...rSt..
+00000170: 0c7c 02a1 016e 0164 0974 07a0 0c7c 03a1  .|...n.d.t...|..
+00000180: 0174 07a0 0c7c 04a1 0174 07a0 0c7c 05a1  .t...|...t...|..
+00000190: 0174 07a0 0c7c 06a1 0164 0a9c 0616 007d  .t...|...d.....}
+000001a0: 0864 0b64 0c7c 0869 0116 007d 0974 0d74  .d.d.|.i...}.t.t
+000001b0: 07a0 0e7c 09a1 0183 0182 0164 0004 007d  ...|.......d...}
+000001c0: 0304 007d 0404 007d 0504 007d 077d 067c  ...}...}...}.}.|
+000001d0: 0264 0d19 007d 0a64 0e67 017d 0b7c 0a7c  .d...}.d.g.}.|.|
+000001e0: 0b6b 027d 037c 0373 af74 07a0 0864 067c  .k.}.|.s.t...d.|
+000001f0: 0366 0164 0f7c 0a7c 0b66 02a1 0474 07a0  .f.d.|.|.f...t..
+00000200: 0c7c 0aa1 0174 07a0 0c7c 0ba1 0164 109c  .|...t...|...d..
+00000210: 0216 007d 0c64 1164 127c 0c69 0116 007d  ...}.d.d.|.i...}
+00000220: 0d74 0d74 07a0 0e7c 0da1 0183 0182 0164  .t.t...|.......d
+00000230: 0004 007d 0a04 007d 037d 0b7c 0264 1319  ...}...}.}.|.d..
+00000240: 007d 0a64 0267 017d 0b7c 0a7c 0b6b 027d  .}.d.g.}.|.|.k.}
+00000250: 037c 0373 e574 07a0 0864 067c 0366 0164  .|.s.t...d.|.f.d
+00000260: 0f7c 0a7c 0b66 02a1 0474 07a0 0c7c 0aa1  .|.|.f...t...|..
+00000270: 0174 07a0 0c7c 0ba1 0164 109c 0216 007d  .t...|...d.....}
+00000280: 0c64 1164 127c 0c69 0116 007d 0d74 0d74  .d.d.|.i...}.t.t
+00000290: 07a0 0e7c 0da1 0183 0182 0164 0004 007d  ...|.......d...}
+000002a0: 0a04 007d 037d 0b64 0053 0029 144e da08  ...}.}.d.S.).N..
+000002b0: 6163 746f 725f 6964 da09 666f 6c6c 6f77  actor_id..follow
+000002c0: 6572 7329 02da 0269 6472 0700 0000 da04  ers)...idr......
+000002d0: 7465 7874 3e06 0000 00fa 0840 636f 6e74  text>......@cont
+000002e0: 6578 74da 0274 6fda 0c61 7474 7269 6275  ext..to..attribu
+000002f0: 7465 6454 6fda 0474 7970 65da 0263 63da  tedTo..type..cc.
+00000300: 0763 6f6e 7465 6e74 a901 fa02 3d3d a901  .content....==..
+00000310: 7a62 2528 7079 3729 730a 7b25 2870 7937  zb%(py7)s.{%(py7
+00000320: 2973 203d 2025 2870 7930 2973 2825 2870  )s = %(py0)s(%(p
+00000330: 7935 2973 0a7b 2528 7079 3529 7320 3d20  y5)s.{%(py5)s = 
+00000340: 2528 7079 3329 730a 7b25 2870 7933 2973  %(py3)s.{%(py3)s
+00000350: 203d 2025 2870 7931 2973 2e6b 6579 730a   = %(py1)s.keys.
+00000360: 7d28 290a 7d29 0a7d 203d 3d20 2528 7079  }().}).} == %(py
+00000370: 3130 2973 da03 7365 74da 0672 6573 756c  10)s..set..resul
+00000380: 74a9 06da 0370 7930 da03 7079 31da 0370  t....py0..py1..p
+00000390: 7933 da03 7079 35da 0370 7937 da04 7079  y3..py5..py7..py
+000003a0: 3130 fa0f 6173 7365 7274 2025 2870 7931  10..assert %(py1
+000003b0: 3229 73da 0470 7931 3272 0b00 0000 7a2c  2)s..py12r....z,
+000003c0: 6874 7470 733a 2f2f 7777 772e 7733 2e6f  https://www.w3.o
+000003d0: 7267 2f6e 732f 6163 7469 7669 7479 7374  rg/ns/activityst
+000003e0: 7265 616d 7323 5075 626c 6963 a901 7a12  reams#Public..z.
+000003f0: 2528 7079 3129 7320 3d3d 2025 2870 7934  %(py1)s == %(py4
+00000400: 2973 a902 7217 0000 00da 0370 7934 fa0e  )s..r......py4..
+00000410: 6173 7365 7274 2025 2870 7936 2973 da03  assert %(py6)s..
+00000420: 7079 3672 0e00 0000 290f 7204 0000 00da  py6r....).r.....
+00000430: 046e 6f74 65da 0961 735f 7075 626c 6963  .note..as_public
+00000440: 720f 0000 00da 0562 7569 6c64 da04 6b65  r......build..ke
+00000450: 7973 7213 0000 00da 0a40 7079 7465 7374  ysr......@pytest
+00000460: 5f61 72da 115f 6361 6c6c 5f72 6570 7263  _ar.._call_reprc
+00000470: 6f6d 7061 7265 da0c 4070 795f 6275 696c  ompare..@py_buil
+00000480: 7469 6e73 da06 6c6f 6361 6c73 da18 5f73  tins..locals.._s
+00000490: 686f 756c 645f 7265 7072 5f67 6c6f 6261  hould_repr_globa
+000004a0: 6c5f 6e61 6d65 da09 5f73 6166 6572 6570  l_name.._saferep
+000004b0: 72da 0e41 7373 6572 7469 6f6e 4572 726f  r..AssertionErro
+000004c0: 72da 135f 666f 726d 6174 5f65 7870 6c61  r.._format_expla
+000004d0: 6e61 7469 6f6e 290e da0e 6f62 6a65 6374  nation)...object
+000004e0: 5f66 6163 746f 7279 7223 0000 0072 1400  _factoryr#...r..
+000004f0: 0000 da0b 4070 795f 6173 7365 7274 32da  ....@py_assert2.
+00000500: 0b40 7079 5f61 7373 6572 7434 da0b 4070  .@py_assert4..@p
+00000510: 795f 6173 7365 7274 36da 0b40 7079 5f61  y_assert6..@py_a
+00000520: 7373 6572 7439 da0b 4070 795f 6173 7365  ssert9..@py_asse
+00000530: 7274 38da 0c40 7079 5f66 6f72 6d61 7431  rt8..@py_format1
+00000540: 31da 0c40 7079 5f66 6f72 6d61 7431 33da  1..@py_format13.
+00000550: 0b40 7079 5f61 7373 6572 7430 da0b 4070  .@py_assert0..@p
+00000560: 795f 6173 7365 7274 33da 0b40 7079 5f66  y_assert3..@py_f
+00000570: 6f72 6d61 7435 da0b 4070 795f 666f 726d  ormat5..@py_form
+00000580: 6174 37a9 0072 3b00 0000 fa5f 2f77 6f6f  at7..r;...._/woo
+00000590: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
+000005a0: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
+000005b0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+000005c0: 7669 6e65 2f61 6374 6976 6974 7973 7472  vine/activitystr
+000005d0: 6561 6d73 2f74 6573 745f 6f62 6a65 6374  eams/test_object
+000005e0: 5f66 6163 746f 7279 2e70 79da 1374 6573  _factory.py..tes
+000005f0: 745f 6f62 6a65 6374 5f66 6163 746f 7279  t_object_factory
+00000600: 0700 0000 736a 0000 000e 010c 0206 0108  ....sj..........
+00000610: 0102 0202 0726 f902 070e f902 0704 f904  .....&..........
+00000620: 0706 f902 0702 f902 0704 f902 0702 f904  ................
+00000630: 0706 f904 0706 f902 0702 f902 0704 f902  ................
+00000640: 0702 f904 0704 f902 0702 f902 0702 f902  ................
+00000650: 0702 f902 0702 f902 0702 f902 0702 f902  ................
+00000660: 0702 f902 0718 f902 0702 f902 0718 f96c  ...............l
+00000670: 0970 0172 3d00 0000 6300 0000 0000 0000  .p.r=...c.......
+00000680: 0000 0000 0013 0000 0009 0000 00c3 0000  ................
+00000690: 0073 8402 0000 8101 7400 8300 7d00 7400  .s......t...}.t.
+000006a0: 8300 7d01 6401 7d02 7c01 7c00 6a01 6a02  ..}.d.}.|.|.j.j.
+000006b0: 5f03 7404 a005 6402 7c02 6403 6404 6405  _.t...d.|.d.d.d.
+000006c0: 9c04 a101 7c01 6a06 5f03 7407 7c00 6406  ....|.j._.t.|.d.
+000006d0: 8d01 7d03 7c03 a008 7c02 a101 4900 6400  ..}.|...|...I.d.
+000006e0: 4800 7d04 7c04 a009 a100 7d05 7c05 6a0a  H.}.|.....}.|.j.
+000006f0: 7d06 7c06 8300 7d07 740b 7c07 8301 7d08  }.|...}.t.|...}.
+00000700: 6800 6407 a301 7d09 7c08 7c09 6b02 7d0a  h.d...}.|.|.k.}.
+00000710: 7c0a 738c 740c a00d 6408 7c0a 6601 6409  |.s.t...d.|.f.d.
+00000720: 7c08 7c09 6602 a104 640a 740e a00f a100  |.|.f...d.t.....
+00000730: 7600 7354 740c a010 740b a101 7259 740c  v.sTt...t...rYt.
+00000740: a011 740b a101 6e01 640a 640b 740e a00f  ..t...n.d.d.t...
+00000750: a100 7600 7365 740c a010 7c05 a101 726a  ..v.set...|...rj
+00000760: 740c a011 7c05 a101 6e01 640b 740c a011  t...|...n.d.t...
+00000770: 7c06 a101 740c a011 7c07 a101 740c a011  |...t...|...t...
+00000780: 7c08 a101 740c a011 7c09 a101 640c 9c06  |...t...|...d...
+00000790: 1600 7d0b 640d 640e 7c0b 6901 1600 7d0c  ..}.d.d.|.i...}.
+000007a0: 7412 740c a013 7c0c a101 8301 8201 6400  t.t...|.......d.
+000007b0: 0400 7d06 0400 7d07 0400 7d08 0400 7d0a  ..}...}...}...}.
+000007c0: 7d09 7c05 640f 1900 7d0d 6410 7d0e 7c0d  }.|.d...}.d.}.|.
+000007d0: 7c0e 6b02 7d06 7c06 73c5 740c a00d 6408  |.k.}.|.s.t...d.
+000007e0: 7c06 6601 6411 7c0d 7c0e 6602 a104 740c  |.f.d.|.|.f...t.
+000007f0: a011 7c0d a101 740c a011 7c0e a101 6412  ..|...t...|...d.
+00000800: 9c02 1600 7d0f 6413 6414 7c0f 6901 1600  ....}.d.d.|.i...
+00000810: 7d10 7412 740c a013 7c10 a101 8301 8201  }.t.t...|.......
+00000820: 6400 0400 7d0d 0400 7d06 7d0e 7c05 6415  d...}...}.}.|.d.
+00000830: 1900 7d0d 7c0d 7c02 6b02 7d06 7c06 9001  ..}.|.|.k.}.|...
+00000840: 7306 740c a00d 6408 7c06 6601 6416 7c0d  s.t...d.|.f.d.|.
+00000850: 7c02 6602 a104 740c a011 7c0d a101 6417  |.f...t...|...d.
+00000860: 740e a00f a100 7600 73ef 740c a010 7c02  t.....v.s.t...|.
+00000870: a101 72f4 740c a011 7c02 a101 6e01 6417  ..r.t...|...n.d.
+00000880: 6418 9c02 1600 7d11 6419 641a 7c11 6901  d.....}.d.d.|.i.
+00000890: 1600 7d12 7412 740c a013 7c12 a101 8301  ..}.t.t...|.....
+000008a0: 8201 6400 0400 7d0d 7d06 7c05 641b 1900  ..d...}.}.|.d...
+000008b0: 7d0d 641c 7d0e 7c0d 7c0e 6b02 7d06 7c06  }.d.}.|.|.k.}.|.
+000008c0: 9001 733a 740c a00d 6408 7c06 6601 6411  ..s:t...d.|.f.d.
+000008d0: 7c0d 7c0e 6602 a104 740c a011 7c0d a101  |.|.f...t...|...
+000008e0: 740c a011 7c0e a101 6412 9c02 1600 7d0f  t...|...d.....}.
+000008f0: 6413 6414 7c0f 6901 1600 7d10 7412 740c  d.d.|.i...}.t.t.
+00000900: a013 7c10 a101 8301 8201 6400 0400 7d0d  ..|.......d...}.
+00000910: 0400 7d06 7d0e 6400 5300 291d 4e7a 1468  ..}.}.d.S.).Nz.h
+00000920: 7474 7073 3a2f 2f72 656d 6f74 652f 616c  ttps://remote/al
+00000930: 6963 657a 2568 7474 7073 3a2f 2f77 7777  icez%https://www
+00000940: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
+00000950: 6974 7973 7472 6561 6d73 da06 5065 7273  itystreams..Pers
+00000960: 6f6e 5a06 616c 7973 7361 2904 720a 0000  onZ.alyssa).r...
+00000970: 0072 0800 0000 720d 0000 00da 1170 7265  .r....r......pre
+00000980: 6665 7272 6564 5573 6572 6e61 6d65 2901  ferredUsername).
+00000990: da06 636c 6965 6e74 3e04 0000 00da 046e  ..client>......n
+000009a0: 616d 65da 0468 7265 6672 0d00 0000 720a  ame..hrefr....r.
+000009b0: 0000 0072 1000 0000 7212 0000 0072 1300  ...r....r....r..
+000009c0: 0000 da07 6d65 6e74 696f 6e72 1500 0000  ....mentionr....
+000009d0: 721c 0000 0072 1d00 0000 720d 0000 00da  r....r....r.....
+000009e0: 074d 656e 7469 6f6e 721e 0000 0072 1f00  .Mentionr....r..
+000009f0: 0000 7221 0000 0072 2200 0000 7242 0000  ..r!...r"...rB..
+00000a00: 0029 017a 1225 2870 7931 2973 203d 3d20  .).z.%(py1)s == 
+00000a10: 2528 7079 3329 73da 0a72 656d 6f74 655f  %(py3)s..remote_
+00000a20: 7572 6929 0272 1700 0000 7218 0000 007a  uri).r....r....z
+00000a30: 0e61 7373 6572 7420 2528 7079 3529 7372  .assert %(py5)sr
+00000a40: 1900 0000 7241 0000 007a 0d61 6c79 7373  ....rA...z.alyss
+00000a50: 6140 7265 6d6f 7465 2914 7202 0000 0072  a@remote).r....r
+00000a60: 4000 0000 da03 6765 74da 0c72 6574 7572  @.....get..retur
+00000a70: 6e5f 7661 6c75 65da 046a 736f 6eda 0564  n_value..json..d
+00000a80: 756d 7073 7209 0000 0072 0400 0000 da15  umpsr....r......
+00000a90: 6d65 6e74 696f 6e5f 666f 725f 6163 746f  mention_for_acto
+00000aa0: 725f 7572 6972 2500 0000 7226 0000 0072  r_urir%...r&...r
+00000ab0: 1300 0000 7227 0000 0072 2800 0000 7229  ....r'...r(...r)
+00000ac0: 0000 0072 2a00 0000 722b 0000 0072 2c00  ...r*...r+...r,.
+00000ad0: 0000 722d 0000 0072 2e00 0000 2913 5a0b  ..r-...r....).Z.
+00000ae0: 6d6f 636b 5f63 6c69 656e 745a 0d6d 6f63  mock_clientZ.moc
+00000af0: 6b5f 7265 7370 6f6e 7365 7245 0000 0072  k_responserE...r
+00000b00: 2f00 0000 5a0e 6d65 6e74 696f 6e5f 6f62  /...Z.mention_ob
+00000b10: 6a65 6374 7243 0000 0072 3000 0000 7231  jectrC...r0...r1
+00000b20: 0000 0072 3200 0000 7233 0000 0072 3400  ...r2...r3...r4.
+00000b30: 0000 7235 0000 0072 3600 0000 7237 0000  ..r5...r6...r7..
+00000b40: 0072 3800 0000 7239 0000 0072 3a00 0000  .r8...r9...r:...
+00000b50: da0b 4070 795f 666f 726d 6174 34da 0b40  ..@py_format4..@
+00000b60: 7079 5f66 6f72 6d61 7436 723b 0000 0072  py_format6r;...r
+00000b70: 3b00 0000 723c 0000 00da 1a74 6573 745f  ;...r<.....test_
+00000b80: 6d65 6e74 696f 6e5f 666f 725f 6163 746f  mention_for_acto
+00000b90: 725f 7572 691b 0000 0073 2600 0000 0280  r_uri....s&.....
+00000ba0: 0601 0601 0401 0a02 0402 0202 0201 0201  ................
+00000bb0: 0201 04fc 08ff 0a09 1002 0801 d602 6a01  ..............j.
+00000bc0: 7e01 7001 724d 0000 0029 0272 0500 0000  ~.p.rM...).r....
+00000bd0: 4e29 0dda 0862 7569 6c74 696e 7372 2900  N)...builtinsr).
+00000be0: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
+00000bf0: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
+00000c00: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
+00000c10: 6572 2700 0000 7248 0000 00da 0d75 6e69  er'...rH.....uni
+00000c20: 7474 6573 742e 6d6f 636b 7202 0000 0072  ttest.mockr....r
+00000c30: 2f00 0000 7204 0000 0072 3d00 0000 724d  /...r....r=...rM
+00000c40: 0000 0072 3b00 0000 723b 0000 0072 3b00  ...r;...r;...r;.
+00000c50: 0000 723c 0000 00da 083c 6d6f 6475 6c65  ..r<.....<module
+00000c60: 3e01 0000 0073 0a00 0000 2200 0c01 0c02  >....s....".....
+00000c70: 0a03 0e14                                ....
```

### Comparing `bovine-0.1.2/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1010 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,122 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 f203 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0a04 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
+00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
-00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
-00000060: 8400 5a09 6408 6409 8400 5a0a 6401 5300  ..Z.d.d...Z.d.S.
-00000070: 290a e900 0000 004e e901 0000 0029 01da  )......N.....)..
-00000080: 114f 7264 6572 6564 436f 6c6c 6563 7469  .OrderedCollecti
-00000090: 6f6e 6300 0000 0000 0000 0000 0000 0005  onc.............
-000000a0: 0000 0007 0000 0043 0000 0073 9400 0000  .......C...s....
-000000b0: 7400 6401 6402 8d01 a001 a100 7d00 6403  t.d.d.......}.d.
-000000c0: 6401 6404 6405 6406 9c04 7d01 7c00 7c01  d.d.d.d...}.|.|.
-000000d0: 6b02 7d02 7c02 7344 7402 a003 6407 7c02  k.}.|.sDt...d.|.
-000000e0: 6601 6408 7c00 7c01 6602 a104 6409 7404  f.d.|.|.f...d.t.
-000000f0: a005 a100 7600 7329 7402 a006 7c00 a101  ....v.s)t...|...
-00000100: 722e 7402 a007 7c00 a101 6e01 6409 7402  r.t...|...n.d.t.
-00000110: a007 7c01 a101 640a 9c02 1600 7d03 640b  ..|...d.....}.d.
-00000120: 640c 7c03 6901 1600 7d04 7408 7402 a009  d.|.i...}.t.t...
-00000130: 7c04 a101 8301 8201 6400 0400 7d02 7d01  |.......d...}.}.
-00000140: 6400 5300 290d 4eda 0375 726c 2901 da02  d.S.).N..url)...
-00000150: 6964 fa25 6874 7470 733a 2f2f 7777 772e  id.%https://www.
-00000160: 7733 2e6f 7267 2f6e 732f 6163 7469 7669  w3.org/ns/activi
-00000170: 7479 7374 7265 616d 7372 0100 0000 7203  tystreamsr....r.
-00000180: 0000 0029 04fa 0840 636f 6e74 6578 7472  ...)...@contextr
-00000190: 0500 0000 da0a 746f 7461 6c49 7465 6d73  ......totalItems
-000001a0: da04 7479 7065 a901 fa02 3d3d a901 7a12  ..type....==..z.
-000001b0: 2528 7079 3029 7320 3d3d 2025 2870 7933  %(py0)s == %(py3
-000001c0: 2973 da06 7265 7375 6c74 a902 da03 7079  )s..result....py
-000001d0: 30da 0370 7933 fa0e 6173 7365 7274 2025  0..py3..assert %
-000001e0: 2870 7935 2973 da03 7079 35a9 0a72 0300  (py5)s..py5..r..
-000001f0: 0000 da05 6275 696c 64da 0a40 7079 7465  ....build..@pyte
-00000200: 7374 5f61 72da 115f 6361 6c6c 5f72 6570  st_ar.._call_rep
-00000210: 7263 6f6d 7061 7265 da0c 4070 795f 6275  rcompare..@py_bu
-00000220: 696c 7469 6e73 da06 6c6f 6361 6c73 da18  iltins..locals..
-00000230: 5f73 686f 756c 645f 7265 7072 5f67 6c6f  _should_repr_glo
-00000240: 6261 6c5f 6e61 6d65 da09 5f73 6166 6572  bal_name.._safer
-00000250: 6570 72da 0e41 7373 6572 7469 6f6e 4572  epr..AssertionEr
-00000260: 726f 72da 135f 666f 726d 6174 5f65 7870  ror.._format_exp
-00000270: 6c61 6e61 7469 6f6e a905 720d 0000 00da  lanation..r.....
-00000280: 0b40 7079 5f61 7373 6572 7432 da0b 4070  .@py_assert2..@p
-00000290: 795f 6173 7365 7274 31da 0b40 7079 5f66  y_assert1..@py_f
-000002a0: 6f72 6d61 7434 da0b 4070 795f 666f 726d  ormat4..@py_form
-000002b0: 6174 36a9 0072 2200 0000 fa6b 2f77 6f6f  at6..r"....k/woo
-000002c0: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
-000002d0: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
-000002e0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-000002f0: 7669 6e65 2f61 6374 6976 6974 7973 7472  vine/activitystr
-00000300: 6561 6d73 2f74 6573 745f 6f72 6465 7265  eams/test_ordere
-00000310: 645f 636f 6c6c 6563 7469 6f6e 5f62 7569  d_collection_bui
-00000320: 6c64 6572 2e70 79da 1f74 6573 745f 6f72  lder.py..test_or
-00000330: 6465 7265 645f 636f 6c6c 6563 7469 6f6e  dered_collection
-00000340: 5f62 7569 6c64 6572 0400 0000 7330 0000  _builder....s0..
-00000350: 000e 011c 0202 050e fb02 0504 fb04 0506  ................
-00000360: fb02 0502 fb02 0504 fb02 0502 fb04 0504  ................
-00000370: fb02 0502 fb02 0518 fb02 0502 fb02 0510  ................
-00000380: fb72 2400 0000 6300 0000 0000 0000 0000  .r$...c.........
-00000390: 0000 0005 0000 0007 0000 0043 0000 0073  ...........C...s
-000003a0: a600 0000 7400 6401 6402 6403 6404 6901  ....t.d.d.d.d.i.
-000003b0: 6701 6405 8d03 a001 a100 7d00 6406 6401  g.d.......}.d.d.
-000003c0: 6403 6404 6901 6701 6402 6407 6408 9c05  d.d.i.g.d.d.d...
-000003d0: 7d01 7c00 7c01 6b02 7d02 7c02 734d 7402  }.|.|.k.}.|.sMt.
-000003e0: a003 6409 7c02 6601 640a 7c00 7c01 6602  ..d.|.f.d.|.|.f.
-000003f0: a104 640b 7404 a005 a100 7600 7332 7402  ..d.t.....v.s2t.
-00000400: a006 7c00 a101 7237 7402 a007 7c00 a101  ..|...r7t...|...
-00000410: 6e01 640b 7402 a007 7c01 a101 640c 9c02  n.d.t...|...d...
-00000420: 1600 7d03 640d 640e 7c03 6901 1600 7d04  ..}.d.d.|.i...}.
-00000430: 7408 7402 a009 7c04 a101 8301 8201 6400  t.t...|.......d.
-00000440: 0400 7d02 7d01 6400 5300 290f 4e72 0400  ..}.}.d.S.).Nr..
-00000450: 0000 7202 0000 00da 0469 7465 6dda 0131  ..r......item..1
-00000460: 2903 7205 0000 00da 0563 6f75 6e74 da05  ).r......count..
-00000470: 6974 656d 7372 0600 0000 7203 0000 0029  itemsr....r....)
-00000480: 0572 0700 0000 7205 0000 00da 0c6f 7264  .r....r......ord
-00000490: 6572 6564 4974 656d 7372 0800 0000 7209  eredItemsr....r.
-000004a0: 0000 0072 0a00 0000 720c 0000 0072 0d00  ...r....r....r..
-000004b0: 0000 720e 0000 0072 1100 0000 7212 0000  ..r....r....r...
-000004c0: 0072 1300 0000 721d 0000 0072 2200 0000  .r....r....r"...
-000004d0: 7222 0000 0072 2300 0000 da2a 7465 7374  r"...r#....*test
-000004e0: 5f6f 7264 6572 6564 5f63 6f6c 6c65 6374  _ordered_collect
-000004f0: 696f 6e5f 6275 696c 6465 725f 7769 7468  ion_builder_with
-00000500: 5f69 7465 6d73 0f00 0000 7330 0000 0018  _items....s0....
-00000510: 0124 0202 060e fa02 0604 fa04 0606 fa02  .$..............
-00000520: 0602 fa02 0604 fa02 0602 fa04 0604 fa02  ................
-00000530: 0602 fa02 0618 fa02 0602 fa02 0610 fa72  ...............r
-00000540: 2a00 0000 6300 0000 0000 0000 0000 0000  *...c...........
-00000550: 0005 0000 0007 0000 0043 0000 0073 9e00  .........C...s..
-00000560: 0000 7400 6401 6402 6403 6404 6405 8d04  ..t.d.d.d.d.d...
-00000570: a001 a100 7d00 6406 6401 6403 6404 6402  ....}.d.d.d.d.d.
-00000580: 6407 6408 9c06 7d01 7c00 7c01 6b02 7d02  d.d...}.|.|.k.}.
-00000590: 7c02 7349 7402 a003 6409 7c02 6601 640a  |.sIt...d.|.f.d.
-000005a0: 7c00 7c01 6602 a104 640b 7404 a005 a100  |.|.f...d.t.....
-000005b0: 7600 732e 7402 a006 7c00 a101 7233 7402  v.s.t...|...r3t.
-000005c0: a007 7c00 a101 6e01 640b 7402 a007 7c01  ..|...n.d.t...|.
-000005d0: a101 640c 9c02 1600 7d03 640d 640e 7c03  ..d.....}.d.d.|.
-000005e0: 6901 1600 7d04 7408 7402 a009 7c04 a101  i...}.t.t...|...
-000005f0: 8301 8201 6400 0400 7d02 7d01 6400 5300  ....d...}.}.d.S.
-00000600: 290f 4e72 0400 0000 7202 0000 00da 0566  ).Nr....r......f
-00000610: 6972 7374 da04 6c61 7374 2904 7205 0000  irst..last).r...
-00000620: 0072 2700 0000 722b 0000 0072 2c00 0000  .r'...r+...r,...
-00000630: 7206 0000 0072 0300 0000 2906 7207 0000  r....r....).r...
-00000640: 0072 0500 0000 722b 0000 0072 2c00 0000  .r....r+...r,...
-00000650: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000660: 0c00 0000 720d 0000 0072 0e00 0000 7211  ....r....r....r.
-00000670: 0000 0072 1200 0000 7213 0000 0072 1d00  ...r....r....r..
-00000680: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00000690: 00da 2e74 6573 745f 6f72 6465 7265 645f  ...test_ordered_
-000006a0: 636f 6c6c 6563 7469 6f6e 5f62 7569 6c64  collection_build
-000006b0: 6572 5f77 6974 685f 6669 7374 5f6c 6173  er_with_fist_las
-000006c0: 741b 0000 0073 3000 0000 1401 2002 0207  t....s0..... ...
-000006d0: 0ef9 0207 04f9 0407 06f9 0207 02f9 0207  ................
-000006e0: 04f9 0207 02f9 0407 04f9 0207 02f9 0207  ................
-000006f0: 18f9 0207 02f9 0207 10f9 722d 0000 0029  ..........r-...)
-00000700: 0bda 0862 7569 6c74 696e 7372 1700 0000  ...builtinsr....
-00000710: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-00000720: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-00000730: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-00000740: 1500 0000 da00 7203 0000 0072 2400 0000  ......r....r$...
-00000750: 722a 0000 0072 2d00 0000 7222 0000 0072  r*...r-...r"...r
-00000760: 2200 0000 7222 0000 0072 2300 0000 da08  "...r"...r#.....
-00000770: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000780: 0026 0008 0308 0b0c 0c                   .&.......
+00000050: 5a07 0100 640b 6405 6406 8404 5a08 640b  Z...d.d.d...Z.d.
+00000060: 6407 6408 8404 5a09 640b 6409 640a 8404  d.d...Z.d.d.d...
+00000070: 5a0a 6401 5300 290c e900 0000 004e e901  Z.d.S.)......N..
+00000080: 0000 0029 01da 114f 7264 6572 6564 436f  ...)...OrderedCo
+00000090: 6c6c 6563 7469 6f6e da06 7265 7475 726e  llection..return
+000000a0: 6300 0000 0000 0000 0000 0000 0005 0000  c...............
+000000b0: 0007 0000 0043 0000 0073 9400 0000 7400  .....C...s....t.
+000000c0: 6401 6402 8d01 a001 a100 7d00 6403 6401  d.d.......}.d.d.
+000000d0: 6404 6405 6406 9c04 7d01 7c00 7c01 6b02  d.d.d...}.|.|.k.
+000000e0: 7d02 7c02 7344 7402 a003 6407 7c02 6601  }.|.sDt...d.|.f.
+000000f0: 6408 7c00 7c01 6602 a104 6409 7404 a005  d.|.|.f...d.t...
+00000100: a100 7600 7329 7402 a006 7c00 a101 722e  ..v.s)t...|...r.
+00000110: 7402 a007 7c00 a101 6e01 6409 7402 a007  t...|...n.d.t...
+00000120: 7c01 a101 640a 9c02 1600 7d03 640b 640c  |...d.....}.d.d.
+00000130: 7c03 6901 1600 7d04 7408 7402 a009 7c04  |.i...}.t.t...|.
+00000140: a101 8301 8201 6400 0400 7d02 7d01 6400  ......d...}.}.d.
+00000150: 5300 290d 4eda 0375 726c 2901 da02 6964  S.).N..url)...id
+00000160: fa25 6874 7470 733a 2f2f 7777 772e 7733  .%https://www.w3
+00000170: 2e6f 7267 2f6e 732f 6163 7469 7669 7479  .org/ns/activity
+00000180: 7374 7265 616d 7372 0100 0000 7203 0000  streamsr....r...
+00000190: 0029 04fa 0840 636f 6e74 6578 7472 0600  .)...@contextr..
+000001a0: 0000 da0a 746f 7461 6c49 7465 6d73 da04  ....totalItems..
+000001b0: 7479 7065 a901 fa02 3d3d a901 7a12 2528  type....==..z.%(
+000001c0: 7079 3029 7320 3d3d 2025 2870 7933 2973  py0)s == %(py3)s
+000001d0: da06 7265 7375 6c74 a902 da03 7079 30da  ..result....py0.
+000001e0: 0370 7933 fa0e 6173 7365 7274 2025 2870  .py3..assert %(p
+000001f0: 7935 2973 da03 7079 35a9 0a72 0300 0000  y5)s..py5..r....
+00000200: da05 6275 696c 64da 0a40 7079 7465 7374  ..build..@pytest
+00000210: 5f61 72da 115f 6361 6c6c 5f72 6570 7263  _ar.._call_reprc
+00000220: 6f6d 7061 7265 da0c 4070 795f 6275 696c  ompare..@py_buil
+00000230: 7469 6e73 da06 6c6f 6361 6c73 da18 5f73  tins..locals.._s
+00000240: 686f 756c 645f 7265 7072 5f67 6c6f 6261  hould_repr_globa
+00000250: 6c5f 6e61 6d65 da09 5f73 6166 6572 6570  l_name.._saferep
+00000260: 72da 0e41 7373 6572 7469 6f6e 4572 726f  r..AssertionErro
+00000270: 72da 135f 666f 726d 6174 5f65 7870 6c61  r.._format_expla
+00000280: 6e61 7469 6f6e a905 720e 0000 00da 0b40  nation..r......@
+00000290: 7079 5f61 7373 6572 7432 da0b 4070 795f  py_assert2..@py_
+000002a0: 6173 7365 7274 31da 0b40 7079 5f66 6f72  assert1..@py_for
+000002b0: 6d61 7434 da0b 4070 795f 666f 726d 6174  mat4..@py_format
+000002c0: 36a9 0072 2300 0000 fa6b 2f77 6f6f 6470  6..r#....k/woodp
+000002d0: 6563 6b65 722f 7372 632f 636f 6465 6265  ecker/src/codebe
+000002e0: 7267 2e6f 7267 2f62 6f76 696e 652f 626f  rg.org/bovine/bo
+000002f0: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+00000300: 6e65 2f61 6374 6976 6974 7973 7472 6561  ne/activitystrea
+00000310: 6d73 2f74 6573 745f 6f72 6465 7265 645f  ms/test_ordered_
+00000320: 636f 6c6c 6563 7469 6f6e 5f62 7569 6c64  collection_build
+00000330: 6572 2e70 79da 1f74 6573 745f 6f72 6465  er.py..test_orde
+00000340: 7265 645f 636f 6c6c 6563 7469 6f6e 5f62  red_collection_b
+00000350: 7569 6c64 6572 0400 0000 7330 0000 000e  uilder....s0....
+00000360: 011c 0202 050e fb02 0504 fb04 0506 fb02  ................
+00000370: 0502 fb02 0504 fb02 0502 fb04 0504 fb02  ................
+00000380: 0502 fb02 0518 fb02 0502 fb02 0510 fb72  ...............r
+00000390: 2500 0000 6300 0000 0000 0000 0000 0000  %...c...........
+000003a0: 0005 0000 0007 0000 0043 0000 0073 a600  .........C...s..
+000003b0: 0000 7400 6401 6402 6403 6404 6901 6701  ..t.d.d.d.d.i.g.
+000003c0: 6405 8d03 a001 a100 7d00 6406 6401 6403  d.......}.d.d.d.
+000003d0: 6404 6901 6701 6402 6407 6408 9c05 7d01  d.i.g.d.d.d...}.
+000003e0: 7c00 7c01 6b02 7d02 7c02 734d 7402 a003  |.|.k.}.|.sMt...
+000003f0: 6409 7c02 6601 640a 7c00 7c01 6602 a104  d.|.f.d.|.|.f...
+00000400: 640b 7404 a005 a100 7600 7332 7402 a006  d.t.....v.s2t...
+00000410: 7c00 a101 7237 7402 a007 7c00 a101 6e01  |...r7t...|...n.
+00000420: 640b 7402 a007 7c01 a101 640c 9c02 1600  d.t...|...d.....
+00000430: 7d03 640d 640e 7c03 6901 1600 7d04 7408  }.d.d.|.i...}.t.
+00000440: 7402 a009 7c04 a101 8301 8201 6400 0400  t...|.......d...
+00000450: 7d02 7d01 6400 5300 290f 4e72 0500 0000  }.}.d.S.).Nr....
+00000460: 7202 0000 00da 0469 7465 6dda 0131 2903  r......item..1).
+00000470: 7206 0000 00da 0563 6f75 6e74 da05 6974  r......count..it
+00000480: 656d 7372 0700 0000 7203 0000 0029 0572  emsr....r....).r
+00000490: 0800 0000 7206 0000 00da 0c6f 7264 6572  ....r......order
+000004a0: 6564 4974 656d 7372 0900 0000 720a 0000  edItemsr....r...
+000004b0: 0072 0b00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+000004c0: 720f 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000004d0: 1400 0000 721e 0000 0072 2300 0000 7223  ....r....r#...r#
+000004e0: 0000 0072 2400 0000 da2a 7465 7374 5f6f  ...r$....*test_o
+000004f0: 7264 6572 6564 5f63 6f6c 6c65 6374 696f  rdered_collectio
+00000500: 6e5f 6275 696c 6465 725f 7769 7468 5f69  n_builder_with_i
+00000510: 7465 6d73 0f00 0000 7330 0000 0018 0124  tems....s0.....$
+00000520: 0202 060e fa02 0604 fa04 0606 fa02 0602  ................
+00000530: fa02 0604 fa02 0602 fa04 0604 fa02 0602  ................
+00000540: fa02 0618 fa02 0602 fa02 0610 fa72 2b00  .............r+.
+00000550: 0000 6300 0000 0000 0000 0000 0000 0005  ..c.............
+00000560: 0000 0007 0000 0043 0000 0073 9e00 0000  .......C...s....
+00000570: 7400 6401 6402 6403 6404 6405 8d04 a001  t.d.d.d.d.d.....
+00000580: a100 7d00 6406 6401 6403 6404 6402 6407  ..}.d.d.d.d.d.d.
+00000590: 6408 9c06 7d01 7c00 7c01 6b02 7d02 7c02  d...}.|.|.k.}.|.
+000005a0: 7349 7402 a003 6409 7c02 6601 640a 7c00  sIt...d.|.f.d.|.
+000005b0: 7c01 6602 a104 640b 7404 a005 a100 7600  |.f...d.t.....v.
+000005c0: 732e 7402 a006 7c00 a101 7233 7402 a007  s.t...|...r3t...
+000005d0: 7c00 a101 6e01 640b 7402 a007 7c01 a101  |...n.d.t...|...
+000005e0: 640c 9c02 1600 7d03 640d 640e 7c03 6901  d.....}.d.d.|.i.
+000005f0: 1600 7d04 7408 7402 a009 7c04 a101 8301  ..}.t.t...|.....
+00000600: 8201 6400 0400 7d02 7d01 6400 5300 290f  ..d...}.}.d.S.).
+00000610: 4e72 0500 0000 7202 0000 00da 0566 6972  Nr....r......fir
+00000620: 7374 da04 6c61 7374 2904 7206 0000 0072  st..last).r....r
+00000630: 2800 0000 722c 0000 0072 2d00 0000 7207  (...r,...r-...r.
+00000640: 0000 0072 0300 0000 2906 7208 0000 0072  ...r....).r....r
+00000650: 0600 0000 722c 0000 0072 2d00 0000 7209  ....r,...r-...r.
+00000660: 0000 0072 0a00 0000 720b 0000 0072 0d00  ...r....r....r..
+00000670: 0000 720e 0000 0072 0f00 0000 7212 0000  ..r....r....r...
+00000680: 0072 1300 0000 7214 0000 0072 1e00 0000  .r....r....r....
+00000690: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
+000006a0: 2e74 6573 745f 6f72 6465 7265 645f 636f  .test_ordered_co
+000006b0: 6c6c 6563 7469 6f6e 5f62 7569 6c64 6572  llection_builder
+000006c0: 5f77 6974 685f 6669 7374 5f6c 6173 741b  _with_fist_last.
+000006d0: 0000 0073 3000 0000 1401 2002 0207 0ef9  ...s0..... .....
+000006e0: 0207 04f9 0407 06f9 0207 02f9 0207 04f9  ................
+000006f0: 0207 02f9 0407 04f9 0207 02f9 0207 18f9  ................
+00000700: 0207 02f9 0207 10f9 722e 0000 0029 0272  ........r....).r
+00000710: 0400 0000 4e29 0bda 0862 7569 6c74 696e  ....N)...builtin
+00000720: 7372 1800 0000 da19 5f70 7974 6573 742e  sr......_pytest.
+00000730: 6173 7365 7274 696f 6e2e 7265 7772 6974  assertion.rewrit
+00000740: 65da 0961 7373 6572 7469 6f6e da07 7265  e..assertion..re
+00000750: 7772 6974 6572 1600 0000 da00 7203 0000  writer......r...
+00000760: 0072 2500 0000 722b 0000 0072 2e00 0000  .r%...r+...r....
+00000770: 7223 0000 0072 2300 0000 7223 0000 0072  r#...r#...r#...r
+00000780: 2400 0000 da08 3c6d 6f64 756c 653e 0100  $.....<module>..
+00000790: 0000 7308 0000 0026 000a 030a 0b0e 0c    ..s....&.......
```

### Comparing `bovine-0.1.2/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 809 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,85 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 2903 0000  o.........Ad)...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 6102 0000  o.......*.Nda...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
+00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
-00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
-00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
-00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
-00000070: 154f 7264 6572 6564 436f 6c6c 6563 7469  .OrderedCollecti
-00000080: 6f6e 5061 6765 6300 0000 0000 0000 0000  onPagec.........
-00000090: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
-000000a0: 4001 0000 7400 6401 6402 6403 6701 6404  @...t.d.d.d.g.d.
-000000b0: 8d03 a001 a100 7d00 6405 6401 6402 6403  ......}.d.d.d.d.
-000000c0: 6701 6406 6407 9c05 7d01 7c00 7c01 6b02  g.d.d...}.|.|.k.
-000000d0: 7d02 7c02 7349 7402 a003 6408 7c02 6601  }.|.sIt...d.|.f.
-000000e0: 6409 7c00 7c01 6602 a104 640a 7404 a005  d.|.|.f...d.t...
-000000f0: a100 7600 732e 7402 a006 7c00 a101 7233  ..v.s.t...|...r3
-00000100: 7402 a007 7c00 a101 6e01 640a 7402 a007  t...|...n.d.t...
-00000110: 7c01 a101 640b 9c02 1600 7d03 640c 640d  |...d.....}.d.d.
-00000120: 7c03 6901 1600 7d04 7408 7402 a009 7c04  |.i...}.t.t...|.
-00000130: a101 8301 8201 6400 0400 7d02 7d01 7400  ......d...}.}.t.
-00000140: 6401 6402 6403 6701 640e 640f 6410 8d05  d.d.d.g.d.d.d...
-00000150: a001 a100 7d00 6405 6401 640e 640f 6402  ....}.d.d.d.d.d.
-00000160: 6403 6701 6406 6411 9c07 7d01 7c00 7c01  d.g.d.d...}.|.|.
-00000170: 6b02 7d02 7c02 739a 7402 a003 6408 7c02  k.}.|.s.t...d.|.
-00000180: 6601 6409 7c00 7c01 6602 a104 640a 7404  f.d.|.|.f...d.t.
-00000190: a005 a100 7600 737f 7402 a006 7c00 a101  ....v.s.t...|...
-000001a0: 7284 7402 a007 7c00 a101 6e01 640a 7402  r.t...|...n.d.t.
-000001b0: a007 7c01 a101 640b 9c02 1600 7d03 640c  ..|...d.....}.d.
-000001c0: 640d 7c03 6901 1600 7d04 7408 7402 a009  d.|.i...}.t.t...
-000001d0: 7c04 a101 8301 8201 6400 0400 7d02 7d01  |.......d...}.}.
-000001e0: 6400 5300 2912 4e7a 0a75 726c 3f70 6167  d.S.).Nz.url?pag
-000001f0: 653d 31da 0375 726c 5a03 6964 3129 03da  e=1..urlZ.id1)..
-00000200: 0269 64da 0770 6172 745f 6f66 da05 6974  .id..part_of..it
-00000210: 656d 737a 2568 7474 7073 3a2f 2f77 7777  emsz%https://www
-00000220: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
-00000230: 6974 7973 7472 6561 6d73 7203 0000 0029  itystreamsr....)
-00000240: 05fa 0840 636f 6e74 6578 7472 0500 0000  ...@contextr....
-00000250: da06 7061 7274 4f66 da0c 6f72 6465 7265  ..partOf..ordere
-00000260: 6449 7465 6d73 da04 7479 7065 2901 fa02  dItems..type)...
-00000270: 3d3d 2901 7a12 2528 7079 3029 7320 3d3d  ==).z.%(py0)s ==
-00000280: 2025 2870 7933 2973 da06 7265 7375 6c74   %(py3)s..result
-00000290: 2902 da03 7079 30da 0370 7933 7a0e 6173  )...py0..py3z.as
-000002a0: 7365 7274 2025 2870 7935 2973 da03 7079  sert %(py5)s..py
-000002b0: 355a 086e 6578 745f 7572 6c5a 0870 7265  5Z.next_urlZ.pre
-000002c0: 765f 7572 6c29 0572 0500 0000 7206 0000  v_url).r....r...
-000002d0: 0072 0700 0000 da04 6e65 7874 da04 7072  .r......next..pr
-000002e0: 6576 2907 7208 0000 0072 0500 0000 7211  ev).r....r....r.
-000002f0: 0000 0072 1200 0000 7209 0000 0072 0a00  ...r....r....r..
-00000300: 0000 720b 0000 0029 0a72 0300 0000 da05  ..r....).r......
-00000310: 6275 696c 64da 0a40 7079 7465 7374 5f61  build..@pytest_a
-00000320: 72da 115f 6361 6c6c 5f72 6570 7263 6f6d  r.._call_reprcom
-00000330: 7061 7265 da0c 4070 795f 6275 696c 7469  pare..@py_builti
-00000340: 6e73 da06 6c6f 6361 6c73 da18 5f73 686f  ns..locals.._sho
-00000350: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
-00000360: 6e61 6d65 da09 5f73 6166 6572 6570 72da  name.._saferepr.
-00000370: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000380: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
-00000390: 7469 6f6e 2905 720d 0000 00da 0b40 7079  tion).r......@py
-000003a0: 5f61 7373 6572 7432 da0b 4070 795f 6173  _assert2..@py_as
-000003b0: 7365 7274 31da 0b40 7079 5f66 6f72 6d61  sert1..@py_forma
-000003c0: 7434 da0b 4070 795f 666f 726d 6174 36a9  t4..@py_format6.
-000003d0: 0072 2000 0000 fa68 2f77 6f6f 6470 6563  .r ....h/woodpec
-000003e0: 6b65 722f 7372 632f 636f 6465 6265 7267  ker/src/codeberg
-000003f0: 2e6f 7267 2f62 6f76 696e 652f 626f 7669  .org/bovine/bovi
-00000400: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
-00000410: 2f61 6374 6976 6974 7973 7472 6561 6d73  /activitystreams
-00000420: 2f74 6573 745f 6f72 6465 7265 645f 636f  /test_ordered_co
-00000430: 6c6c 6563 7469 6f6e 5f70 6167 652e 7079  llection_page.py
-00000440: da1c 7465 7374 5f6f 7264 6572 6564 5f63  ..test_ordered_c
-00000450: 6f6c 6c65 6374 696f 6e5f 7061 6765 0400  ollection_page..
-00000460: 0000 7370 0000 0002 0108 0104 ff04 0202  ..sp............
-00000470: fe20 0402 060e fa02 0604 fa04 0606 fa02  . ..............
-00000480: 0602 fa02 0604 fa02 0602 fa04 0604 fa02  ................
-00000490: 0602 fa02 0618 fa02 0602 fa02 060c fa02  ................
-000004a0: 080c 0104 ff04 0202 fe24 0402 080e f802  .........$......
-000004b0: 0804 f804 0806 f802 0802 f802 0804 f802  ................
-000004c0: 0802 f804 0804 f802 0802 f802 0818 f802  ................
-000004d0: 0802 f802 0810 f872 2200 0000 2909 da08  .......r"...)...
-000004e0: 6275 696c 7469 6e73 7216 0000 00da 195f  builtinsr......_
-000004f0: 7079 7465 7374 2e61 7373 6572 7469 6f6e  pytest.assertion
-00000500: 2e72 6577 7269 7465 da09 6173 7365 7274  .rewrite..assert
-00000510: 696f 6eda 0772 6577 7269 7465 7214 0000  ion..rewriter...
-00000520: 00da 0072 0300 0000 7222 0000 0072 2000  ...r....r"...r .
-00000530: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
-00000540: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000550: 0400 0000 2600 0c03                      ....&...
+00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
+00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
+00000060: 6408 6406 6407 8404 5a0a 6401 5300 2909  d.d.d...Z.d.S.).
+00000070: e900 0000 004e 2901 da09 4173 796e 634d  .....N)...AsyncM
+00000080: 6f63 6be9 0100 0000 2901 da0b 4576 656e  ock.....)...Even
+00000090: 7453 6f75 7263 65da 0672 6574 7572 6e63  tSource..returnc
+000000a0: 0000 0000 0000 0000 0000 0000 0a00 0000  ................
+000000b0: 0700 0000 c300 0000 7376 0100 0081 0174  ........sv.....t
+000000c0: 0083 007d 0074 0083 007d 0174 007c 0164  ...}.t...}.t.|.d
+000000d0: 018d 017d 027c 027c 006a 015f 0274 037c  ...}.|.|.j._.t.|
+000000e0: 0064 0283 027d 0367 0064 03a2 017c 016a  .d...}.g.d...|.j
+000000f0: 045f 027c 03a0 05a1 0049 0064 0048 007d  ._.|.....I.d.H.}
+00000100: 047c 046a 067d 0564 047d 067c 057c 066b  .|.j.}.d.}.|.|.k
+00000110: 027d 077c 0773 6174 07a0 0864 057c 0766  .}.|.sat...d.|.f
+00000120: 0164 067c 057c 0666 02a1 0464 0774 09a0  .d.|.|.f...d.t..
+00000130: 0aa1 0076 0073 4274 07a0 0b7c 04a1 0172  ...v.sBt...|...r
+00000140: 4774 07a0 0c7c 04a1 016e 0164 0774 07a0  Gt...|...n.d.t..
+00000150: 0c7c 05a1 0174 07a0 0c7c 06a1 0164 089c  .|...t...|...d..
+00000160: 0316 007d 0864 0964 0a7c 0869 0116 007d  ...}.d.d.|.i...}
+00000170: 0974 0d74 07a0 0e7c 09a1 0183 0182 0164  .t.t...|.......d
+00000180: 0004 007d 0504 007d 077d 0667 0064 0ba2  ...}...}.}.g.d..
+00000190: 017c 016a 045f 027c 03a0 05a1 0049 0064  .|.j._.|.....I.d
+000001a0: 0048 007d 047c 046a 067d 0564 047d 067c  .H.}.|.j.}.d.}.|
+000001b0: 057c 066b 027d 077c 0773 b374 07a0 0864  .|.k.}.|.s.t...d
+000001c0: 057c 0766 0164 067c 057c 0666 02a1 0464  .|.f.d.|.|.f...d
+000001d0: 0774 09a0 0aa1 0076 0073 9474 07a0 0b7c  .t.....v.s.t...|
+000001e0: 04a1 0172 9974 07a0 0c7c 04a1 016e 0164  ...r.t...|...n.d
+000001f0: 0774 07a0 0c7c 05a1 0174 07a0 0c7c 06a1  .t...|...t...|..
+00000200: 0164 089c 0316 007d 0864 0964 0a7c 0869  .d.....}.d.d.|.i
+00000210: 0116 007d 0974 0d74 07a0 0e7c 09a1 0183  ...}.t.t...|....
+00000220: 0182 0164 0004 007d 0504 007d 077d 0664  ...d...}...}.}.d
+00000230: 0053 0029 0c4e 2901 da07 636f 6e74 656e  .S.).N)...conten
+00000240: 74da 0375 726c 2905 f30b 0000 0064 6174  t..url)......dat
+00000250: 613a 2074 6578 740a f301 0000 000a 7209  a: text.......r.
+00000260: 0000 0072 0900 0000 7209 0000 00da 0474  ...r....r......t
+00000270: 6578 7429 01fa 023d 3d29 017a 2c25 2870  ext)...==).z,%(p
+00000280: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
+00000290: 2528 7079 3029 732e 6461 7461 0a7d 203d  %(py0)s.data.} =
+000002a0: 3d20 2528 7079 3529 73da 0565 7665 6e74  = %(py5)s..event
+000002b0: 2903 da03 7079 30da 0370 7932 da03 7079  )...py0..py2..py
+000002c0: 357a 0e61 7373 6572 7420 2528 7079 3729  5z.assert %(py7)
+000002d0: 73da 0370 7937 2904 7209 0000 0072 0900  s..py7).r....r..
+000002e0: 0000 7208 0000 0072 0900 0000 290f 7202  ..r....r....).r.
+000002f0: 0000 00da 0367 6574 da0c 7265 7475 726e  .....get..return
+00000300: 5f76 616c 7565 7204 0000 00da 095f 5f61  _valuer......__a
+00000310: 6974 6572 5f5f da09 5f5f 616e 6578 745f  iter__..__anext_
+00000320: 5fda 0464 6174 61da 0a40 7079 7465 7374  _..data..@pytest
+00000330: 5f61 72da 115f 6361 6c6c 5f72 6570 7263  _ar.._call_reprc
+00000340: 6f6d 7061 7265 da0c 4070 795f 6275 696c  ompare..@py_buil
+00000350: 7469 6e73 da06 6c6f 6361 6c73 da18 5f73  tins..locals.._s
+00000360: 686f 756c 645f 7265 7072 5f67 6c6f 6261  hould_repr_globa
+00000370: 6c5f 6e61 6d65 da09 5f73 6166 6572 6570  l_name.._saferep
+00000380: 72da 0e41 7373 6572 7469 6f6e 4572 726f  r..AssertionErro
+00000390: 72da 135f 666f 726d 6174 5f65 7870 6c61  r.._format_expla
+000003a0: 6e61 7469 6f6e 290a da07 7365 7373 696f  nation)...sessio
+000003b0: 6e72 0600 0000 da08 7265 7370 6f6e 7365  nr......response
+000003c0: da0c 6576 656e 745f 736f 7572 6365 720c  ..event_sourcer.
+000003d0: 0000 00da 0b40 7079 5f61 7373 6572 7431  .....@py_assert1
+000003e0: da0b 4070 795f 6173 7365 7274 34da 0b40  ..@py_assert4..@
+000003f0: 7079 5f61 7373 6572 7433 da0b 4070 795f  py_assert3..@py_
+00000400: 666f 726d 6174 36da 0b40 7079 5f66 6f72  format6..@py_for
+00000410: 6d61 7438 a900 7226 0000 00fa 552f 776f  mat8..r&....U/wo
+00000420: 6f64 7065 636b 6572 2f73 7263 2f63 6f64  odpecker/src/cod
+00000430: 6562 6572 672e 6f72 672f 626f 7669 6e65  eberg.org/bovine
+00000440: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+00000450: 6f76 696e 652f 636c 6965 6e74 732f 7465  ovine/clients/te
+00000460: 7374 5f65 7665 6e74 5f73 6f75 7263 652e  st_event_source.
+00000470: 7079 da11 7465 7374 5f65 7665 6e74 5f73  py..test_event_s
+00000480: 6f75 7263 6506 0000 0073 1800 0000 0280  ource....s......
+00000490: 0601 0601 0a01 0801 0a02 0c02 0e01 8a01  ................
+000004a0: 0c02 0e01 8e01 7228 0000 0029 0272 0500  ......r(...).r..
+000004b0: 0000 4e29 0bda 0862 7569 6c74 696e 7372  ..N)...builtinsr
+000004c0: 1800 0000 da19 5f70 7974 6573 742e 6173  ......_pytest.as
+000004d0: 7365 7274 696f 6e2e 7265 7772 6974 65da  sertion.rewrite.
+000004e0: 0961 7373 6572 7469 6f6e da07 7265 7772  .assertion..rewr
+000004f0: 6974 6572 1600 0000 da0d 756e 6974 7465  iter......unitte
+00000500: 7374 2e6d 6f63 6b72 0200 0000 7220 0000  st.mockr....r ..
+00000510: 0072 0400 0000 7228 0000 0072 2600 0000  .r....r(...r&...
+00000520: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
+00000530: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
+00000540: 0000 2600 0c02 0e03                      ..&.....
```

### Comparing `bovine-0.1.2/bovine/activitystreams/activity_factory.py` & `bovine-0.1.3/bovine/activitystreams/activity_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def as_unlisted(self):
         """makes the activity unlisted, i.e. public in cc and followers in to"""
         if self.followers:
             self.to.add(self.followers)
         self.cc.add("https://www.w3.org/ns/activitystreams#Public")
         return self
 
-    def build(self):
+    def build(self) -> dict:
         """converts the activity into a dict, that can be serialized to JSON"""
         result = {
             "@context": "https://www.w3.org/ns/activitystreams",
             "type": self.type,
             "actor": self.actor,
             "to": list(self.to),
             "cc": list(self.cc - self.to),
```

### Comparing `bovine-0.1.2/bovine/activitystreams/object_factory.py` & `bovine-0.1.3/bovine/activitystreams/object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/activitystreams/test_activity_factory.py` & `bovine-0.1.3/bovine/activitystreams/test_activity_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .activity_factory import ActivityFactory
 from .object_factory import Object
 
 
-def test_activity_factory_like():
+def test_activity_factory_like() -> None:
     activity_factory = ActivityFactory({"id": "actor_id", "followers": "followers"})
 
     like = activity_factory.like("target")
     like.to.add("target")
     like.cc.add("other")
     like.content = "🐮"
 
@@ -16,15 +16,15 @@
 
     assert result["to"] == ["target"]
     assert result["cc"] == ["other"]
 
     assert result["type"] == "Like"
 
 
-def test_activity_factory_accept():
+def test_activity_factory_accept() -> None:
     activity_factory = ActivityFactory({"id": "actor_id", "followers": "followers"})
 
     accept = activity_factory.accept({"id": "obj"})
     result = accept.build()
 
     assert result["@context"] == "https://www.w3.org/ns/activitystreams"
     assert result["type"] == "Accept"
@@ -43,15 +43,15 @@
     result = activity_factory.create(note).build()
 
     assert result["cc"] == ["account/followers"]
     assert result["to"] == ["https://www.w3.org/ns/activitystreams#Public"]
     assert result["actor"] == "actor_id"
 
 
-def test_activity_factory_create_no_cc():
+def test_activity_factory_create_no_cc() -> None:
     activity_factory = ActivityFactory({"id": "actor_id", "followers": "followers"})
     remote_actor = "https://abel/alice"
     note = Object(
         type="Note",
         attributed_to="actor_id",
         followers="account/followers",
         to={remote_actor},
@@ -60,13 +60,13 @@
     result = activity_factory.create(note).build()
 
     assert "cc" not in result
     assert result["to"] == [remote_actor]
     assert result["actor"] == "actor_id"
 
 
-def test_activity_no_empty_to_cc():
+def test_activity_no_empty_to_cc() -> None:
     activity_factory = ActivityFactory({"id": "actor_id", "followers": "followers"})
 
     result = activity_factory.delete("target").build()
 
     assert set(result.keys()) == {"@context", "type", "object", "actor"}
```

### Comparing `bovine-0.1.2/bovine/activitystreams/test_actor.py` & `bovine-0.1.3/bovine/activitystreams/test_actor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bovine.types import Visibility
 
 from . import Actor
 
 
-def test_actor():
+def test_actor() -> None:
     actor = Actor(id="http://example.com/actor/123")
 
     result = actor.build()
 
     assert set(result.keys()) == {"type", "id", "@context", "outbox", "inbox"}
 
     actor.name = "John Doe"
@@ -31,28 +31,28 @@
     assert result["publicKey"] == {
         "id": actor.id + "#key",
         "owner": actor.id,
         "publicKeyPem": actor.public_key,
     }
 
 
-def test_actor_second():
+def test_actor_second() -> None:
     actor = Actor(id="http://example.com/actor/123", inbox="inbox", outbox="outbox")
 
     result = actor.build()
 
     assert result["inbox"] == "inbox"
     assert result["outbox"] == "outbox"
 
     actor.proxy_url = "http://example.com/proxy"
     result = actor.build(visibility=Visibility.OWNER)
 
     assert result["endpoints"]["proxyUrl"] == "http://example.com/proxy"
 
 
-def test_actor_with_icon():
+def test_actor_with_icon() -> None:
     actor = Actor(id="http://example.com/actor/123", inbox="inbox", outbox="outbox")
     actor.icon = {"type": "Image"}
 
     result = actor.build()
 
     assert result["icon"] == {"type": "Image"}
```

### Comparing `bovine-0.1.2/bovine/activitystreams/test_object_factory.py` & `bovine-0.1.3/bovine/activitystreams/test_object_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from unittest.mock import AsyncMock
 
 from .object_factory import ObjectFactory
 
 
-def test_object_factory():
+def test_object_factory() -> None:
     object_factory = ObjectFactory({"id": "actor_id", "followers": "followers"})
 
     note = object_factory.note().as_public()
     note.content = "text"
     result = note.build()
 
     assert set(result.keys()) == {
@@ -20,15 +20,15 @@
         "cc",
     }
 
     assert result["to"] == ["https://www.w3.org/ns/activitystreams#Public"]
     assert result["cc"] == ["followers"]
 
 
-async def test_mention_for_actor_uri():
+async def test_mention_for_actor_uri() -> None:
     mock_client = AsyncMock()
     mock_response = AsyncMock()
     remote_uri = "https://remote/alice"
 
     mock_client.client.get.return_value = mock_response
 
     mock_response.text.return_value = json.dumps(
```

### Comparing `bovine-0.1.2/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.1.3/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from . import OrderedCollection
 
 
-def test_ordered_collection_builder():
+def test_ordered_collection_builder() -> None:
     result = OrderedCollection(id="url").build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url",
         "totalItems": 0,
         "type": "OrderedCollection",
     }
 
 
-def test_ordered_collection_builder_with_items():
+def test_ordered_collection_builder_with_items() -> None:
     result = OrderedCollection(id="url", count=1, items=[{"item": "1"}]).build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url",
         "orderedItems": [{"item": "1"}],
         "totalItems": 1,
         "type": "OrderedCollection",
     }
 
 
-def test_ordered_collection_builder_with_fist_last():
+def test_ordered_collection_builder_with_fist_last() -> None:
     result = OrderedCollection(id="url", count=1, first="first", last="last").build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url",
         "first": "first",
         "last": "last",
```

### Comparing `bovine-0.1.2/bovine/activitystreams/test_ordered_collection_page.py` & `bovine-0.1.3/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from . import OrderedCollectionPage
 
 
-def test_ordered_collection_page():
+def test_ordered_collection_page() -> None:
     result = OrderedCollectionPage(
         id="url?page=1", part_of="url", items=["id1"]
     ).build()
 
     assert result == {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": "url?page=1",
```

### Comparing `bovine-0.1.2/bovine/activitystreams/utils/__init__.py` & `bovine-0.1.3/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.3/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 3209 0000  o.........Ad2...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 3209 0000  o.......*.Nd2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6504 6404 6505 6604  m.Z...d.e.d.e.f.
 00000050: 6405 6406 8404 5a06 6403 6501 6504 6505  d.d...Z.d.e.e.e.
 00000060: 4200 1900 6404 6501 6505 1900 6604 6407  B...d.e.e...f.d.
 00000070: 6408 8404 5a07 6409 640a 8400 5a08 6403  d...Z.d.d...Z.d.
```

### Comparing `bovine-0.1.2/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc` & `bovine-0.1.3/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 1303 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 1303 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 8400 5a01 6404  d.l.Z.d.d...Z.d.
 00000040: 6405 8400 5a02 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000050: 004e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
 00000060: 0000 0007 0000 0043 0000 0073 6000 0000  .......C...s`...
 00000070: 6401 7c00 7600 7217 7400 6402 7c00 6401  d.|.v.r.t.d.|.d.
```

### Comparing `bovine-0.1.2/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 da08 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 da08 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6405 6406  Z.m.Z.m.Z...d.d.
 00000070: 8400 5a0d 6407 6408 8400 5a0e 6409 640a  ..Z.d.d...Z.d.d.
@@ -30,19 +30,19 @@
 000001d0: 740d 7407 a00e 7c05 a101 8301 8201 6400  t.t...|.......d.
 000001e0: 0400 7d03 7d02 6400 5300 290f 4eda 044e  ..}.}.d.S.).N..N
 000001f0: 6f74 65da 0761 6363 6f75 6e74 fa11 6163  ote..account..ac
 00000200: 636f 756e 742f 666f 6c6c 6f77 6572 73a9  count/followers.
 00000210: 03da 0474 7970 65da 0d61 7474 7269 6275  ...type..attribu
 00000220: 7465 645f 746f da09 666f 6c6c 6f77 6572  ted_to..follower
 00000230: 73da 0263 63da 0274 6fda 0473 616d 653e  s..cc..to..same>
-00000240: 0500 0000 7211 0000 0072 0f00 0000 720a  ....r....r....r.
-00000250: 0000 007a 2c68 7474 7073 3a2f 2f77 7777  ...z,https://www
-00000260: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
-00000270: 6974 7973 7472 6561 6d73 2350 7562 6c69  itystreams#Publi
-00000280: 6372 1000 0000 a901 fa02 3d3d 2901 7a12  cr........==).z.
+00000240: 0500 0000 7a2c 6874 7470 733a 2f2f 7777  ....z,https://ww
+00000250: 772e 7733 2e6f 7267 2f6e 732f 6163 7469  w.w3.org/ns/acti
+00000260: 7669 7479 7374 7265 616d 7323 5075 626c  vitystreams#Publ
+00000270: 6963 7211 0000 0072 1000 0000 720a 0000  icr....r....r...
+00000280: 0072 0f00 0000 a901 fa02 3d3d 2901 7a12  .r........==).z.
 00000290: 2528 7079 3029 7320 3d3d 2025 2870 7933  %(py0)s == %(py3
 000002a0: 2973 da0a 7265 6369 7069 656e 7473 2902  )s..recipients).
 000002b0: da03 7079 30da 0370 7933 7a0e 6173 7365  ..py0..py3z.asse
 000002c0: 7274 2025 2870 7935 2973 da03 7079 3529  rt %(py5)s..py5)
 000002d0: 0f72 0200 0000 da09 6173 5f70 7562 6c69  .r......as_publi
 000002e0: 6372 0f00 0000 da03 6164 6472 1000 0000  cr......addr....
 000002f0: da05 6275 696c 6472 0700 0000 da0a 4070  ..buildr......@p
```

### Comparing `bovine-0.1.2/bovine/activitystreams/utils/print.py` & `bovine-0.1.3/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/activitystreams/utils/test_utils.py` & `bovine-0.1.3/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/clients/__init__.py` & `bovine-0.1.3/bovine/clients/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import traceback
 
+import aiodns
 import aiohttp
 
 from bovine.utils import parse_fediverse_handle
 
 from .lookup_account import lookup_with_webfinger
 from .nodeinfo import fetch_nodeinfo20, fetch_nodeinfo_document
 
@@ -41,14 +42,33 @@
     """
     webfinger_url = f"https://{domain}/.well-known/webfinger"
     params = {"resource": did}
 
     return await lookup_with_webfinger(session, webfinger_url, params)
 
 
+async def lookup_with_dns(session: aiohttp.ClientSession, domain: str) -> str | None:
+    """Looks up the actor url associated with the dns entry for domain. See
+    `FEP-612d: Identifying ActivityPub Objects through DNS
+    <https://codeberg.org/fediverse/fep/src/branch/main/feps/fep-612d.md>`_ for
+    the mechanism.
+
+    :param session: the aiohttp.ClientSession to use
+    :param domain: the domain to perform the lookup from
+    """
+
+    resolver = aiodns.DNSResolver()
+    try:
+        (result,) = await resolver.query(f"_apobjid.{domain}", "TXT")
+
+        return result.text
+    except Exception:
+        return None
+
+
 async def fetch_nodeinfo(session: aiohttp.ClientSession, domain: str) -> dict | None:
     """Fetches the nodeinfo 2.0 object from domain using the /.well-known/nodeinfo
     endpoint"""
 
     try:
         data = await fetch_nodeinfo_document(session, domain)
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,139 +1,179 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 2108 0000  o.........Ad!...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 a20a 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
+00000020: 0009 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 0100 6403 6404 6c05 6d06 5a06 0100 6403  ..d.d.l.m.Z...d.
-00000060: 6405 6c07 6d08 5a08 6d09 5a09 0100 6500  d.l.m.Z.m.Z...e.
-00000070: a00a 650b a101 5a0c 6406 6502 6a0d 6407  ..e...Z.d.e.j.d.
-00000080: 650e 6408 650e 6401 4200 6606 6409 640a  e.d.e.d.B.f.d.d.
-00000090: 8404 5a0f 6406 6502 6a0d 640b 650e 640c  ..Z.d.e.j.d.e.d.
-000000a0: 650e 6408 650e 6401 4200 6608 640d 640e  e.d.e.d.B.f.d.d.
-000000b0: 8404 5a10 6406 6502 6a0d 640b 650e 6408  ..Z.d.e.j.d.e.d.
-000000c0: 6511 6401 4200 6606 640f 6410 8404 5a12  e.d.B.f.d.d...Z.
-000000d0: 6401 5300 2911 e900 0000 004e 2901 da16  d.S.)......N)...
-000000e0: 7061 7273 655f 6665 6469 7665 7273 655f  parse_fediverse_
-000000f0: 6861 6e64 6c65 e901 0000 00a9 01da 156c  handle.........l
-00000100: 6f6f 6b75 705f 7769 7468 5f77 6562 6669  ookup_with_webfi
-00000110: 6e67 6572 2902 da10 6665 7463 685f 6e6f  nger)...fetch_no
-00000120: 6465 696e 666f 3230 da17 6665 7463 685f  deinfo20..fetch_
-00000130: 6e6f 6465 696e 666f 5f64 6f63 756d 656e  nodeinfo_documen
-00000140: 74da 0773 6573 7369 6f6e da10 6665 6469  t..session..fedi
-00000150: 7665 7273 655f 6861 6e64 6c65 da06 7265  verse_handle..re
-00000160: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
-00000170: 0006 0000 0005 0000 00c3 0000 0073 4000  .............s@.
-00000180: 0000 8101 7400 7c01 8301 5c02 7d02 7d03  ....t.|...\.}.}.
-00000190: 6401 7c03 9b00 6402 9d03 7d04 6403 6404  d.|...d...}.d.d.
-000001a0: 7c02 9b00 6405 7c03 9b00 9d04 6901 7d05  |...d.|.....i.}.
-000001b0: 7401 7c00 7c04 7c05 8303 4900 6406 4800  t.|.|.|...I.d.H.
-000001c0: 5300 2907 6108 0100 004c 6f6f 6b73 2075  S.).a....Looks u
-000001d0: 7020 7468 6520 6163 746f 7220 7572 6c20  p the actor url 
-000001e0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-000001f0: 6120 4665 6469 5665 7273 6520 6861 6e64  a FediVerse hand
-00000200: 6c65 2c0a 2020 2020 692e 652e 2061 6e20  le,.    i.e. an 
-00000210: 6964 656e 7469 6669 6572 206f 6620 7468  identifier of th
-00000220: 6520 666f 726d 2075 7365 726e 616d 6540  e form username@
-00000230: 646f 6d61 696e 2c20 7573 696e 670a 2020  domain, using.  
-00000240: 2020 7468 6520 7765 6266 696e 6765 7220    the webfinger 
-00000250: 656e 6470 6f69 6e74 0a0a 2020 2020 3a70  endpoint..    :p
-00000260: 6172 616d 2073 6573 7369 6f6e 3a20 7468  aram session: th
-00000270: 6520 6169 6f68 7474 702e 436c 6965 6e74  e aiohttp.Client
-00000280: 5365 7373 696f 6e20 746f 2075 7365 0a20  Session to use. 
-00000290: 2020 203a 7061 7261 6d20 6665 6469 7665     :param fedive
-000002a0: 7273 655f 6861 6e64 6c65 3a20 7468 6520  rse_handle: the 
-000002b0: 4665 6469 5665 7273 6520 6861 6e64 6c65  FediVerse handle
-000002c0: 2061 7320 6120 7374 7269 6e67 0a20 2020   as a string.   
-000002d0: 20fa 0868 7474 7073 3a2f 2ffa 162f 2e77   ..https://../.w
-000002e0: 656c 6c2d 6b6e 6f77 6e2f 7765 6266 696e  ell-known/webfin
-000002f0: 6765 72da 0872 6573 6f75 7263 657a 0561  ger..resourcez.a
-00000300: 6363 743a fa01 404e 2902 7202 0000 0072  cct:..@N).r....r
-00000310: 0500 0000 2906 7208 0000 0072 0900 0000  ....).r....r....
-00000320: da08 7573 6572 6e61 6d65 da06 646f 6d61  ..username..doma
-00000330: 696e da0d 7765 6266 696e 6765 725f 7572  in..webfinger_ur
-00000340: 6cda 0670 6172 616d 73a9 0072 1300 0000  l..params..r....
-00000350: fa4c 2f77 6f6f 6470 6563 6b65 722f 7372  .L/woodpecker/sr
-00000360: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
-00000370: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-00000380: 696e 652f 626f 7669 6e65 2f63 6c69 656e  ine/bovine/clien
-00000390: 7473 2f5f 5f69 6e69 745f 5f2e 7079 da1d  ts/__init__.py..
-000003a0: 6c6f 6f6b 7570 5f61 6363 6f75 6e74 5f77  lookup_account_w
-000003b0: 6974 685f 7765 6266 696e 6765 720e 0000  ith_webfinger...
-000003c0: 0073 0a00 0000 0280 0c0a 0c02 1401 1202  .s..............
-000003d0: 7215 0000 0072 1000 0000 da03 6469 6463  r....r......didc
-000003e0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-000003f0: 0400 0000 c300 0000 7328 0000 0081 0164  ........s(.....d
-00000400: 017c 019b 0064 029d 037d 0364 037c 0269  .|...d...}.d.|.i
-00000410: 017d 0474 007c 007c 037c 0483 0349 0064  .}.t.|.|.|...I.d
-00000420: 0448 0053 0029 057a ff4c 6f6f 6b73 2075  .H.S.).z.Looks u
-00000430: 7020 7468 6520 6163 746f 7220 7572 6c20  p the actor url 
-00000440: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-00000450: 6120 6469 6420 616e 6420 646f 6d61 696e  a did and domain
-00000460: 0a20 2020 2075 7369 6e67 2074 6865 2077  .    using the w
-00000470: 6562 6669 6e67 6572 2065 6e64 706f 696e  ebfinger endpoin
-00000480: 740a 0a20 2020 203a 7061 7261 6d20 7365  t..    :param se
-00000490: 7373 696f 6e3a 2074 6865 2061 696f 6874  ssion: the aioht
-000004a0: 7470 2e43 6c69 656e 7453 6573 7369 6f6e  tp.ClientSession
-000004b0: 2074 6f20 7573 650a 2020 2020 3a70 6172   to use.    :par
-000004c0: 616d 2064 6f6d 6169 6e3a 2074 6865 2064  am domain: the d
-000004d0: 6f6d 6169 6e20 746f 2070 6572 666f 726d  omain to perform
-000004e0: 2074 6865 206c 6f6f 6b75 7020 6672 6f6d   the lookup from
-000004f0: 0a20 2020 203a 7061 7261 6d20 6469 643a  .    :param did:
-00000500: 2074 6865 2064 6964 206b 6579 2074 6f20   the did key to 
-00000510: 7065 7266 6f72 6d20 6c6f 6f6b 7570 2077  perform lookup w
-00000520: 6974 680a 2020 2020 720b 0000 0072 0c00  ith.    r....r..
-00000530: 0000 720d 0000 004e 7204 0000 0029 0572  ..r....Nr....).r
-00000540: 0800 0000 7210 0000 0072 1600 0000 7211  ....r....r....r.
-00000550: 0000 0072 1200 0000 7213 0000 0072 1300  ...r....r....r..
-00000560: 0000 7214 0000 00da 196c 6f6f 6b75 705f  ..r......lookup_
-00000570: 6469 645f 7769 7468 5f77 6562 6669 6e67  did_with_webfing
-00000580: 6572 2000 0000 7308 0000 0002 800c 0a08  er ...s.........
-00000590: 0112 0272 1700 0000 6302 0000 0000 0000  ...r....c.......
-000005a0: 0000 0000 0006 0000 000a 0000 00c3 0000  ................
-000005b0: 0073 9e00 0000 8101 7a25 7400 7c00 7c01  .s......z%t.|.|.
-000005c0: 8302 4900 6401 4800 7d02 7c02 6402 1900  ..I.d.H.}.|.d...
-000005d0: 4400 5d15 7d03 7c03 6403 1900 6404 6b02  D.].}.|.d...d.k.
-000005e0: 7223 7401 7c00 7c03 6405 1900 8302 4900  r#t.|.|.d.....I.
-000005f0: 6401 4800 0200 0100 5700 5300 710e 5700  d.H.....W.S.q.W.
-00000600: 6401 5300 0400 7402 794e 0100 7d04 0100  d.S...t.yN..}...
-00000610: 7a1c 7403 a004 7405 7c04 8301 a101 0100  z.t...t.|.......
-00000620: 7406 a007 a100 a008 a100 4400 5d07 7d05  t.........D.].}.
-00000630: 7403 a004 7c05 a101 0100 713b 5700 5900  t...|.....q;W.Y.
-00000640: 6401 7d04 7e04 6401 5300 6401 7d04 7e04  d.}.~.d.S.d.}.~.
-00000650: 7701 7700 2906 7a58 4665 7463 6865 7320  w.w.).zXFetches 
-00000660: 7468 6520 6e6f 6465 696e 666f 2032 2e30  the nodeinfo 2.0
-00000670: 206f 626a 6563 7420 6672 6f6d 2064 6f6d   object from dom
-00000680: 6169 6e20 7573 696e 6720 7468 6520 2f2e  ain using the /.
-00000690: 7765 6c6c 2d6b 6e6f 776e 2f6e 6f64 6569  well-known/nodei
-000006a0: 6e66 6f0a 2020 2020 656e 6470 6f69 6e74  nfo.    endpoint
-000006b0: 4eda 056c 696e 6b73 da03 7265 6c7a 2f68  N..links..relz/h
-000006c0: 7474 703a 2f2f 6e6f 6465 696e 666f 2e64  ttp://nodeinfo.d
-000006d0: 6961 7370 6f72 612e 736f 6674 7761 7265  iaspora.software
-000006e0: 2f6e 732f 7363 6865 6d61 2f32 2e30 5a04  /ns/schema/2.0Z.
-000006f0: 6872 6566 2909 7207 0000 0072 0600 0000  href).r....r....
-00000700: da09 4578 6365 7074 696f 6eda 066c 6f67  ..Exception..log
-00000710: 6765 72da 0565 7272 6f72 da03 7374 72da  ger..error..str.
-00000720: 0974 7261 6365 6261 636b da0a 666f 726d  .traceback..form
-00000730: 6174 5f65 7863 da0a 7370 6c69 746c 696e  at_exc..splitlin
-00000740: 6573 2906 7208 0000 0072 1000 0000 da04  es).r....r......
-00000750: 6461 7461 da04 6c69 6e6b da01 655a 086c  data..link..eZ.l
-00000760: 6f67 5f6c 696e 6572 1300 0000 7213 0000  og_liner....r...
-00000770: 0072 1400 0000 da0e 6665 7463 685f 6e6f  .r......fetch_no
-00000780: 6465 696e 666f 3000 0000 731e 0000 0002  deinfo0...s.....
-00000790: 8002 0410 010c 020c 011a 0102 ff06 030e  ................
-000007a0: 020e 0110 010c 010e 0108 8002 fc72 2400  .............r$.
-000007b0: 0000 2913 da07 6c6f 6767 696e 6772 1e00  ..)...loggingr..
-000007c0: 0000 da07 6169 6f68 7474 705a 0c62 6f76  ....aiohttpZ.bov
-000007d0: 696e 652e 7574 696c 7372 0200 0000 5a0e  ine.utilsr....Z.
-000007e0: 6c6f 6f6b 7570 5f61 6363 6f75 6e74 7205  lookup_accountr.
-000007f0: 0000 005a 086e 6f64 6569 6e66 6f72 0600  ...Z.nodeinfor..
-00000800: 0000 7207 0000 00da 0967 6574 4c6f 6767  ..r......getLogg
-00000810: 6572 da08 5f5f 6e61 6d65 5f5f 721b 0000  er..__name__r...
-00000820: 00da 0d43 6c69 656e 7453 6573 7369 6f6e  ...ClientSession
-00000830: 721d 0000 0072 1500 0000 7217 0000 00da  r....r....r.....
-00000840: 0464 6963 7472 2400 0000 7213 0000 0072  .dictr$...r....r
-00000850: 1300 0000 7213 0000 0072 1400 0000 da08  ....r....r......
-00000860: 3c6d 6f64 756c 653e 0100 0000 7330 0000  <module>....s0..
-00000870: 0008 0008 0108 020c 020c 0210 010a 0202  ................
-00000880: 0304 0102 ff02 0102 ff06 020a fe02 1204  ................
-00000890: 0102 ff02 0102 ff02 0102 ff06 020a fe20  ............... 
-000008a0: 10                                       .
+00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
+00000050: 6402 6c04 6d05 5a05 0100 6403 6404 6c06  d.l.m.Z...d.d.l.
+00000060: 6d07 5a07 0100 6403 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000070: 6d0a 5a0a 0100 6500 a00b 650c a101 5a0d  m.Z...e...e...Z.
+00000080: 6406 6503 6a0e 6407 650f 6408 650f 6401  d.e.j.d.e.d.e.d.
+00000090: 4200 6606 6409 640a 8404 5a10 6406 6503  B.f.d.d...Z.d.e.
+000000a0: 6a0e 640b 650f 640c 650f 6408 650f 6401  j.d.e.d.e.d.e.d.
+000000b0: 4200 6608 640d 640e 8404 5a11 6406 6503  B.f.d.d...Z.d.e.
+000000c0: 6a0e 640b 650f 6408 650f 6401 4200 6606  j.d.e.d.e.d.B.f.
+000000d0: 640f 6410 8404 5a12 6406 6503 6a0e 640b  d.d...Z.d.e.j.d.
+000000e0: 650f 6408 6513 6401 4200 6606 6411 6412  e.d.e.d.B.f.d.d.
+000000f0: 8404 5a14 6401 5300 2913 e900 0000 004e  ..Z.d.S.)......N
+00000100: 2901 da16 7061 7273 655f 6665 6469 7665  )...parse_fedive
+00000110: 7273 655f 6861 6e64 6c65 e901 0000 00a9  rse_handle......
+00000120: 01da 156c 6f6f 6b75 705f 7769 7468 5f77  ...lookup_with_w
+00000130: 6562 6669 6e67 6572 2902 da10 6665 7463  ebfinger)...fetc
+00000140: 685f 6e6f 6465 696e 666f 3230 da17 6665  h_nodeinfo20..fe
+00000150: 7463 685f 6e6f 6465 696e 666f 5f64 6f63  tch_nodeinfo_doc
+00000160: 756d 656e 74da 0773 6573 7369 6f6e da10  ument..session..
+00000170: 6665 6469 7665 7273 655f 6861 6e64 6c65  fediverse_handle
+00000180: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
+00000190: 0000 0000 0006 0000 0005 0000 00c3 0000  ................
+000001a0: 0073 4000 0000 8101 7400 7c01 8301 5c02  .s@.....t.|...\.
+000001b0: 7d02 7d03 6401 7c03 9b00 6402 9d03 7d04  }.}.d.|...d...}.
+000001c0: 6403 6404 7c02 9b00 6405 7c03 9b00 9d04  d.d.|...d.|.....
+000001d0: 6901 7d05 7401 7c00 7c04 7c05 8303 4900  i.}.t.|.|.|...I.
+000001e0: 6406 4800 5300 2907 6108 0100 004c 6f6f  d.H.S.).a....Loo
+000001f0: 6b73 2075 7020 7468 6520 6163 746f 7220  ks up the actor 
+00000200: 7572 6c20 6173 736f 6369 6174 6564 2077  url associated w
+00000210: 6974 6820 6120 4665 6469 5665 7273 6520  ith a FediVerse 
+00000220: 6861 6e64 6c65 2c0a 2020 2020 692e 652e  handle,.    i.e.
+00000230: 2061 6e20 6964 656e 7469 6669 6572 206f   an identifier o
+00000240: 6620 7468 6520 666f 726d 2075 7365 726e  f the form usern
+00000250: 616d 6540 646f 6d61 696e 2c20 7573 696e  ame@domain, usin
+00000260: 670a 2020 2020 7468 6520 7765 6266 696e  g.    the webfin
+00000270: 6765 7220 656e 6470 6f69 6e74 0a0a 2020  ger endpoint..  
+00000280: 2020 3a70 6172 616d 2073 6573 7369 6f6e    :param session
+00000290: 3a20 7468 6520 6169 6f68 7474 702e 436c  : the aiohttp.Cl
+000002a0: 6965 6e74 5365 7373 696f 6e20 746f 2075  ientSession to u
+000002b0: 7365 0a20 2020 203a 7061 7261 6d20 6665  se.    :param fe
+000002c0: 6469 7665 7273 655f 6861 6e64 6c65 3a20  diverse_handle: 
+000002d0: 7468 6520 4665 6469 5665 7273 6520 6861  the FediVerse ha
+000002e0: 6e64 6c65 2061 7320 6120 7374 7269 6e67  ndle as a string
+000002f0: 0a20 2020 20fa 0868 7474 7073 3a2f 2ffa  .    ..https://.
+00000300: 162f 2e77 656c 6c2d 6b6e 6f77 6e2f 7765  ./.well-known/we
+00000310: 6266 696e 6765 72da 0872 6573 6f75 7263  bfinger..resourc
+00000320: 657a 0561 6363 743a fa01 404e 2902 7202  ez.acct:..@N).r.
+00000330: 0000 0072 0500 0000 2906 7208 0000 0072  ...r....).r....r
+00000340: 0900 0000 da08 7573 6572 6e61 6d65 da06  ......username..
+00000350: 646f 6d61 696e da0d 7765 6266 696e 6765  domain..webfinge
+00000360: 725f 7572 6cda 0670 6172 616d 73a9 0072  r_url..params..r
+00000370: 1300 0000 fa4c 2f77 6f6f 6470 6563 6b65  .....L/woodpecke
+00000380: 722f 7372 632f 636f 6465 6265 7267 2e6f  r/src/codeberg.o
+00000390: 7267 2f62 6f76 696e 652f 626f 7669 6e65  rg/bovine/bovine
+000003a0: 2f62 6f76 696e 652f 626f 7669 6e65 2f63  /bovine/bovine/c
+000003b0: 6c69 656e 7473 2f5f 5f69 6e69 745f 5f2e  lients/__init__.
+000003c0: 7079 da1d 6c6f 6f6b 7570 5f61 6363 6f75  py..lookup_accou
+000003d0: 6e74 5f77 6974 685f 7765 6266 696e 6765  nt_with_webfinge
+000003e0: 720f 0000 0073 0a00 0000 0280 0c0a 0c02  r....s..........
+000003f0: 1401 1202 7215 0000 0072 1000 0000 da03  ....r....r......
+00000400: 6469 6463 0300 0000 0000 0000 0000 0000  didc............
+00000410: 0500 0000 0400 0000 c300 0000 7328 0000  ............s(..
+00000420: 0081 0164 017c 019b 0064 029d 037d 0364  ...d.|...d...}.d
+00000430: 037c 0269 017d 0474 007c 007c 037c 0483  .|.i.}.t.|.|.|..
+00000440: 0349 0064 0448 0053 0029 057a ff4c 6f6f  .I.d.H.S.).z.Loo
+00000450: 6b73 2075 7020 7468 6520 6163 746f 7220  ks up the actor 
+00000460: 7572 6c20 6173 736f 6369 6174 6564 2077  url associated w
+00000470: 6974 6820 6120 6469 6420 616e 6420 646f  ith a did and do
+00000480: 6d61 696e 0a20 2020 2075 7369 6e67 2074  main.    using t
+00000490: 6865 2077 6562 6669 6e67 6572 2065 6e64  he webfinger end
+000004a0: 706f 696e 740a 0a20 2020 203a 7061 7261  point..    :para
+000004b0: 6d20 7365 7373 696f 6e3a 2074 6865 2061  m session: the a
+000004c0: 696f 6874 7470 2e43 6c69 656e 7453 6573  iohttp.ClientSes
+000004d0: 7369 6f6e 2074 6f20 7573 650a 2020 2020  sion to use.    
+000004e0: 3a70 6172 616d 2064 6f6d 6169 6e3a 2074  :param domain: t
+000004f0: 6865 2064 6f6d 6169 6e20 746f 2070 6572  he domain to per
+00000500: 666f 726d 2074 6865 206c 6f6f 6b75 7020  form the lookup 
+00000510: 6672 6f6d 0a20 2020 203a 7061 7261 6d20  from.    :param 
+00000520: 6469 643a 2074 6865 2064 6964 206b 6579  did: the did key
+00000530: 2074 6f20 7065 7266 6f72 6d20 6c6f 6f6b   to perform look
+00000540: 7570 2077 6974 680a 2020 2020 720b 0000  up with.    r...
+00000550: 0072 0c00 0000 720d 0000 004e 7204 0000  .r....r....Nr...
+00000560: 0029 0572 0800 0000 7210 0000 0072 1600  .).r....r....r..
+00000570: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000580: 0072 1300 0000 7214 0000 00da 196c 6f6f  .r....r......loo
+00000590: 6b75 705f 6469 645f 7769 7468 5f77 6562  kup_did_with_web
+000005a0: 6669 6e67 6572 2100 0000 7308 0000 0002  finger!...s.....
+000005b0: 800c 0a08 0112 0272 1700 0000 6302 0000  .......r....c...
+000005c0: 0000 0000 0000 0000 0004 0000 0008 0000  ................
+000005d0: 00c3 0000 0073 4200 0000 8101 7400 a001  .....sB.....t...
+000005e0: a100 7d02 7a11 7c02 a002 6401 7c01 9b00  ..}.z.|...d.|...
+000005f0: 9d02 6402 a102 4900 6403 4800 5c01 7d03  ..d...I.d.H.\.}.
+00000600: 7c03 6a03 5700 5300 0400 7404 7920 0100  |.j.W.S...t.y ..
+00000610: 0100 0100 5900 6403 5300 7700 2904 6156  ....Y.d.S.w.).aV
+00000620: 0100 004c 6f6f 6b73 2075 7020 7468 6520  ...Looks up the 
+00000630: 6163 746f 7220 7572 6c20 6173 736f 6369  actor url associ
+00000640: 6174 6564 2077 6974 6820 7468 6520 646e  ated with the dn
+00000650: 7320 656e 7472 7920 666f 7220 646f 6d61  s entry for doma
+00000660: 696e 2e20 5365 650a 2020 2020 6046 4550  in. See.    `FEP
+00000670: 2d36 3132 643a 2049 6465 6e74 6966 7969  -612d: Identifyi
+00000680: 6e67 2041 6374 6976 6974 7950 7562 204f  ng ActivityPub O
+00000690: 626a 6563 7473 2074 6872 6f75 6768 2044  bjects through D
+000006a0: 4e53 0a20 2020 203c 6874 7470 733a 2f2f  NS.    <https://
+000006b0: 636f 6465 6265 7267 2e6f 7267 2f66 6564  codeberg.org/fed
+000006c0: 6976 6572 7365 2f66 6570 2f73 7263 2f62  iverse/fep/src/b
+000006d0: 7261 6e63 682f 6d61 696e 2f66 6570 732f  ranch/main/feps/
+000006e0: 6665 702d 3631 3264 2e6d 643e 605f 2066  fep-612d.md>`_ f
+000006f0: 6f72 0a20 2020 2074 6865 206d 6563 6861  or.    the mecha
+00000700: 6e69 736d 2e0a 0a20 2020 203a 7061 7261  nism...    :para
+00000710: 6d20 7365 7373 696f 6e3a 2074 6865 2061  m session: the a
+00000720: 696f 6874 7470 2e43 6c69 656e 7453 6573  iohttp.ClientSes
+00000730: 7369 6f6e 2074 6f20 7573 650a 2020 2020  sion to use.    
+00000740: 3a70 6172 616d 2064 6f6d 6169 6e3a 2074  :param domain: t
+00000750: 6865 2064 6f6d 6169 6e20 746f 2070 6572  he domain to per
+00000760: 666f 726d 2074 6865 206c 6f6f 6b75 7020  form the lookup 
+00000770: 6672 6f6d 0a20 2020 207a 095f 6170 6f62  from.    z._apob
+00000780: 6a69 642e da03 5458 544e 2905 da06 6169  jid...TXTN)...ai
+00000790: 6f64 6e73 da0b 444e 5352 6573 6f6c 7665  odns..DNSResolve
+000007a0: 72da 0571 7565 7279 da04 7465 7874 da09  r..query..text..
+000007b0: 4578 6365 7074 696f 6e29 0472 0800 0000  Exception).r....
+000007c0: 7210 0000 00da 0872 6573 6f6c 7665 72da  r......resolver.
+000007d0: 0672 6573 756c 7472 1300 0000 7213 0000  .resultr....r...
+000007e0: 0072 1400 0000 da0f 6c6f 6f6b 7570 5f77  .r......lookup_w
+000007f0: 6974 685f 646e 7331 0000 0073 1000 0000  ith_dns1...s....
+00000800: 0280 080a 0201 1a01 0802 0c01 0601 02ff  ................
+00000810: 7220 0000 0063 0200 0000 0000 0000 0000  r ...c..........
+00000820: 0000 0600 0000 0a00 0000 c300 0000 739e  ..............s.
+00000830: 0000 0081 017a 2574 007c 007c 0183 0249  .....z%t.|.|...I
+00000840: 0064 0148 007d 027c 0264 0219 0044 005d  .d.H.}.|.d...D.]
+00000850: 157d 037c 0364 0319 0064 046b 0272 2374  .}.|.d...d.k.r#t
+00000860: 017c 007c 0364 0519 0083 0249 0064 0148  .|.|.d.....I.d.H
+00000870: 0002 0001 0057 0053 0071 0e57 0064 0153  .....W.S.q.W.d.S
+00000880: 0004 0074 0279 4e01 007d 0401 007a 1c74  ...t.yN..}...z.t
+00000890: 03a0 0474 057c 0483 01a1 0101 0074 06a0  ...t.|.......t..
+000008a0: 07a1 00a0 08a1 0044 005d 077d 0574 03a0  .......D.].}.t..
+000008b0: 047c 05a1 0101 0071 3b57 0059 0064 017d  .|.....q;W.Y.d.}
+000008c0: 047e 0464 0153 0064 017d 047e 0477 0177  .~.d.S.d.}.~.w.w
+000008d0: 0029 067a 5846 6574 6368 6573 2074 6865  .).zXFetches the
+000008e0: 206e 6f64 6569 6e66 6f20 322e 3020 6f62   nodeinfo 2.0 ob
+000008f0: 6a65 6374 2066 726f 6d20 646f 6d61 696e  ject from domain
+00000900: 2075 7369 6e67 2074 6865 202f 2e77 656c   using the /.wel
+00000910: 6c2d 6b6e 6f77 6e2f 6e6f 6465 696e 666f  l-known/nodeinfo
+00000920: 0a20 2020 2065 6e64 706f 696e 744e da05  .    endpointN..
+00000930: 6c69 6e6b 73da 0372 656c 7a2f 6874 7470  links..relz/http
+00000940: 3a2f 2f6e 6f64 6569 6e66 6f2e 6469 6173  ://nodeinfo.dias
+00000950: 706f 7261 2e73 6f66 7477 6172 652f 6e73  pora.software/ns
+00000960: 2f73 6368 656d 612f 322e 305a 0468 7265  /schema/2.0Z.hre
+00000970: 6629 0972 0700 0000 7206 0000 0072 1d00  f).r....r....r..
+00000980: 0000 da06 6c6f 6767 6572 da05 6572 726f  ....logger..erro
+00000990: 72da 0373 7472 da09 7472 6163 6562 6163  r..str..tracebac
+000009a0: 6bda 0a66 6f72 6d61 745f 6578 63da 0a73  k..format_exc..s
+000009b0: 706c 6974 6c69 6e65 7329 0672 0800 0000  plitlines).r....
+000009c0: 7210 0000 00da 0464 6174 61da 046c 696e  r......data..lin
+000009d0: 6bda 0165 5a08 6c6f 675f 6c69 6e65 7213  k..eZ.log_liner.
+000009e0: 0000 0072 1300 0000 7214 0000 00da 0e66  ...r....r......f
+000009f0: 6574 6368 5f6e 6f64 6569 6e66 6f44 0000  etch_nodeinfoD..
+00000a00: 0073 1e00 0000 0280 0204 1001 0c02 0c01  .s..............
+00000a10: 1a01 02ff 0603 0e02 0e01 1001 0c01 0e01  ................
+00000a20: 0880 02fc 722c 0000 0029 15da 076c 6f67  ....r,...)...log
+00000a30: 6769 6e67 7226 0000 0072 1900 0000 da07  gingr&...r......
+00000a40: 6169 6f68 7474 705a 0c62 6f76 696e 652e  aiohttpZ.bovine.
+00000a50: 7574 696c 7372 0200 0000 5a0e 6c6f 6f6b  utilsr....Z.look
+00000a60: 7570 5f61 6363 6f75 6e74 7205 0000 005a  up_accountr....Z
+00000a70: 086e 6f64 6569 6e66 6f72 0600 0000 7207  .nodeinfor....r.
+00000a80: 0000 00da 0967 6574 4c6f 6767 6572 da08  .....getLogger..
+00000a90: 5f5f 6e61 6d65 5f5f 7223 0000 00da 0d43  __name__r#.....C
+00000aa0: 6c69 656e 7453 6573 7369 6f6e 7225 0000  lientSessionr%..
+00000ab0: 0072 1500 0000 7217 0000 0072 2000 0000  .r....r....r ...
+00000ac0: da04 6469 6374 722c 0000 0072 1300 0000  ..dictr,...r....
+00000ad0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
+00000ae0: 083c 6d6f 6475 6c65 3e01 0000 0073 3400  .<module>....s4.
+00000af0: 0000 0800 0801 0802 0801 0c02 0c02 1001  ................
+00000b00: 0a02 0203 0401 02ff 0201 02ff 0602 0afe  ................
+00000b10: 0212 0401 02ff 0201 02ff 0201 02ff 0602  ................
+00000b20: 0afe 1c10 2013                           .... .
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/event_source.cpython-310.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/event_source.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,108 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 5204 0000  o.........AdR...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 f005 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 4700 6403 6404 8400 6404 8302 5a03  ..G.d.d...d...Z.
-00000050: 6401 5300 2905 e900 0000 004e 2901 da0f  d.S.)......N)...
-00000060: 5365 7276 6572 5365 6e74 4576 656e 7463  ServerSentEventc
-00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0700 0000 4000 0000 7340 0000 0065 005a  ....@...s@...e.Z
-00000090: 0164 005a 0269 0066 0164 0165 036a 0464  .d.Z.i.f.d.e.j.d
-000000a0: 0265 0564 0365 0666 0664 0464 0584 055a  .e.d.e.f.d.d...Z
-000000b0: 0764 0664 0784 005a 0864 0864 0984 005a  .d.d...Z.d.d...Z
-000000c0: 0964 0a64 0b84 005a 0a64 0c53 0029 0dda  .d.d...Z.d.S.)..
-000000d0: 0b45 7665 6e74 536f 7572 6365 da07 7365  .EventSource..se
-000000e0: 7373 696f 6eda 0375 726c da07 6865 6164  ssion..url..head
-000000f0: 6572 7363 0400 0000 0000 0000 0000 0000  ersc............
-00000100: 0400 0000 0200 0000 4300 0000 731c 0000  ........C...s...
-00000110: 007c 017c 005f 007c 027c 005f 017c 037c  .|.|._.|.|._.|.|
-00000120: 005f 0264 007c 005f 0364 0053 00a9 014e  ._.d.|._.d.S...N
-00000130: 2904 7204 0000 0072 0500 0000 7206 0000  ).r....r....r...
-00000140: 00da 0872 6573 706f 6e73 6529 04da 0473  ...response)...s
-00000150: 656c 6672 0400 0000 7205 0000 0072 0600  elfr....r....r..
-00000160: 0000 a900 720a 0000 00fa 502f 776f 6f64  ....r.....P/wood
-00000170: 7065 636b 6572 2f73 7263 2f63 6f64 6562  pecker/src/codeb
-00000180: 6572 672e 6f72 672f 626f 7669 6e65 2f62  erg.org/bovine/b
-00000190: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-000001a0: 696e 652f 636c 6965 6e74 732f 6576 656e  ine/clients/even
-000001b0: 745f 736f 7572 6365 2e70 79da 085f 5f69  t_source.py..__i
-000001c0: 6e69 745f 5f07 0000 0073 0800 0000 0601  nit__....s......
-000001d0: 0601 0601 0a01 7a14 4576 656e 7453 6f75  ......z.EventSou
-000001e0: 7263 652e 5f5f 696e 6974 5f5f 6301 0000  rce.__init__c...
-000001f0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00000200: 00c3 0000 0073 3800 0000 8101 7400 6a01  .....s8.....t.j.
-00000210: 6400 6401 8d01 7d01 7c00 6a02 6a03 7c00  d.d...}.|.j.j.|.
-00000220: 6a04 6402 6403 6901 7c00 6a05 a501 7c01  j.d.d.i.|.j...|.
-00000230: 6404 8d03 4900 6400 4800 7c00 5f06 6400  d...I.d.H.|._.d.
-00000240: 5300 2905 4e29 01da 0574 6f74 616c da06  S.).N)...total..
-00000250: 4163 6365 7074 7a11 7465 7874 2f65 7665  Acceptz.text/eve
-00000260: 6e74 2d73 7472 6561 6d29 0272 0600 0000  nt-stream).r....
-00000270: da07 7469 6d65 6f75 7429 07da 0761 696f  ..timeout)...aio
-00000280: 6874 7470 da0d 436c 6965 6e74 5469 6d65  http..ClientTime
-00000290: 6f75 7472 0400 0000 da03 6765 7472 0500  outr......getr..
-000002a0: 0000 7206 0000 0072 0800 0000 2902 7209  ..r....r....).r.
-000002b0: 0000 0072 0f00 0000 720a 0000 0072 0a00  ...r....r....r..
-000002c0: 0000 720b 0000 00da 0f63 7265 6174 655f  ..r......create_
-000002d0: 7265 7370 6f6e 7365 0d00 0000 730e 0000  response....s...
-000002e0: 0002 800c 0106 0204 010c 0102 0112 fd7a  ...............z
-000002f0: 1b45 7665 6e74 536f 7572 6365 2e63 7265  .EventSource.cre
-00000300: 6174 655f 7265 7370 6f6e 7365 6301 0000  ate_responsec...
-00000310: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00000320: 0043 0000 0073 0400 0000 7c00 5300 7207  .C...s....|.S.r.
-00000330: 0000 0072 0a00 0000 2901 7209 0000 0072  ...r....).r....r
-00000340: 0a00 0000 720a 0000 0072 0b00 0000 da09  ....r....r......
-00000350: 5f5f 6169 7465 725f 5f16 0000 0073 0200  __aiter__....s..
-00000360: 0000 0401 7a15 4576 656e 7453 6f75 7263  ....z.EventSourc
-00000370: 652e 5f5f 6169 7465 725f 5f63 0100 0000  e.__aiter__c....
-00000380: 0000 0000 0000 0000 0500 0000 0700 0000  ................
-00000390: c300 0000 7380 0000 0081 017c 006a 0064  ....s......|.j.d
-000003a0: 0075 0072 0d7c 00a0 01a1 0049 0064 0048  .u.r.|.....I.d.H
-000003b0: 0001 0064 017d 017c 006a 006a 0232 007a  ...d.}.|.j.j.2.z
-000003c0: 2933 0064 0048 0057 007d 027c 02a0 0364  )3.d.H.W.}.|...d
-000003d0: 02a1 017d 037c 0364 0319 0064 046b 0272  ...}.|.d...d.k.r
-000003e0: 2571 137c 0364 056b 0272 3674 04a0 057c  %q.|.d.k.r6t...|
-000003f0: 01a1 017d 047c 046a 0672 357c 0402 0001  ...}.|.j.r5|....
-00000400: 0053 0071 137c 019b 007c 039b 009d 027d  .S.q.|...|.....}
-00000410: 0171 1336 0064 0053 0029 064e da00 7a05  .q.6.d.S.).N..z.
-00000420: 7574 662d 3872 0100 0000 fa01 3ada 010a  utf-8r......:...
-00000430: 2907 7208 0000 0072 1300 0000 da07 636f  ).r....r......co
-00000440: 6e74 656e 74da 0664 6563 6f64 6572 0200  ntent..decoder..
-00000450: 0000 5a0a 7061 7273 655f 7574 6638 da04  ..Z.parse_utf8..
-00000460: 6461 7461 2905 7209 0000 005a 0874 6f5f  data).r....Z.to_
-00000470: 7061 7273 655a 0d6c 696e 655f 696e 5f62  parseZ.line_in_b
-00000480: 7974 6573 da04 6c69 6e65 da05 6576 656e  ytes..line..even
-00000490: 7472 0a00 0000 720a 0000 0072 0b00 0000  tr....r....r....
-000004a0: da09 5f5f 616e 6578 745f 5f19 0000 0073  ..__anext__....s
-000004b0: 1e00 0000 0280 0a01 0e01 0402 1402 0a01  ................
-000004c0: 0c01 0201 0801 0a01 0601 0801 02ff 0e03  ................
-000004d0: 06f7 7a15 4576 656e 7453 6f75 7263 652e  ..z.EventSource.
-000004e0: 5f5f 616e 6578 745f 5f4e 290b da08 5f5f  __anext__N)...__
-000004f0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000500: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000510: 7210 0000 00da 0d43 6c69 656e 7453 6573  r......ClientSes
-00000520: 7369 6f6e da03 7374 72da 0464 6963 7472  sion..str..dictr
-00000530: 0c00 0000 7213 0000 0072 1400 0000 721d  ....r....r....r.
-00000540: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
-00000550: 0000 720b 0000 0072 0300 0000 0600 0000  ..r....r........
-00000560: 730a 0000 0008 001c 0108 0608 090c 0372  s..............r
-00000570: 0300 0000 2904 7210 0000 005a 0c62 6f76  ....).r....Z.bov
-00000580: 696e 652e 7479 7065 7372 0200 0000 7203  ine.typesr....r.
-00000590: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
-000005a0: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000005b0: 3e01 0000 0073 0600 0000 0800 0c02 1203  >....s..........
+00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 4700  Z.d.d.l.m.Z...G.
+00000050: 6404 6405 8400 6405 8302 5a05 6402 5300  d.d...d...Z.d.S.
+00000060: 2906 e900 0000 0029 01da 0444 6963 744e  )......)...DictN
+00000070: 2901 da0f 5365 7276 6572 5365 6e74 4576  )...ServerSentEv
+00000080: 656e 7463 0000 0000 0000 0000 0000 0000  entc............
+00000090: 0000 0000 0900 0000 4000 0000 7354 0000  ........@...sT..
+000000a0: 0065 005a 0164 005a 0269 0066 0164 0165  .e.Z.d.Z.i.f.d.e
+000000b0: 036a 0464 0265 0564 0365 0665 0565 0566  .j.d.e.d.e.e.e.f
+000000c0: 0219 0066 0664 0464 0584 055a 0764 0e64  ...f.d.d...Z.d.d
+000000d0: 0864 0984 045a 0864 0a64 0b84 005a 0964  .d...Z.d.d...Z.d
+000000e0: 0665 0a64 0742 0066 0264 0c64 0d84 045a  .e.d.B.f.d.d...Z
+000000f0: 0b64 0753 0029 0fda 0b45 7665 6e74 536f  .d.S.)...EventSo
+00000100: 7572 6365 da07 7365 7373 696f 6eda 0375  urce..session..u
+00000110: 726c da07 6865 6164 6572 7363 0400 0000  rl..headersc....
+00000120: 0000 0000 0000 0000 0400 0000 0200 0000  ................
+00000130: 4300 0000 731c 0000 007c 017c 005f 007c  C...s....|.|._.|
+00000140: 027c 005f 017c 037c 005f 0264 007c 005f  .|._.|.|._.d.|._
+00000150: 0364 0053 00a9 014e 2904 7205 0000 0072  .d.S...N).r....r
+00000160: 0600 0000 7207 0000 00da 0872 6573 706f  ....r......respo
+00000170: 6e73 6529 04da 0473 656c 6672 0500 0000  nse)...selfr....
+00000180: 7206 0000 0072 0700 0000 a900 720b 0000  r....r......r...
+00000190: 00fa 502f 776f 6f64 7065 636b 6572 2f73  ..P/woodpecker/s
+000001a0: 7263 2f63 6f64 6562 6572 672e 6f72 672f  rc/codeberg.org/
+000001b0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+000001c0: 7669 6e65 2f62 6f76 696e 652f 636c 6965  vine/bovine/clie
+000001d0: 6e74 732f 6576 656e 745f 736f 7572 6365  nts/event_source
+000001e0: 2e70 79da 085f 5f69 6e69 745f 5f09 0000  .py..__init__...
+000001f0: 0073 0800 0000 0603 0601 0601 0a01 7a14  .s............z.
+00000200: 4576 656e 7453 6f75 7263 652e 5f5f 696e  EventSource.__in
+00000210: 6974 5f5f da06 7265 7475 726e 4e63 0100  it__..returnNc..
+00000220: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00000230: 0000 c300 0000 737a 0000 0081 0174 006a  ......sz.....t.j
+00000240: 0164 0064 018d 017d 017c 006a 026a 037c  .d.d...}.|.j.j.|
+00000250: 006a 0464 0264 0369 017c 006a 05a5 017c  .j.d.d.i.|.j...|
+00000260: 0164 0464 058d 0449 0064 0048 007c 005f  .d.d...I.d.H.|._
+00000270: 067c 006a 0673 204a 0082 017c 006a 06a0  .|.j.s J...|.j..
+00000280: 07a1 0001 007c 006a 066a 0864 066b 0272  .....|.j.j.d.k.r
+00000290: 3b7c 006a 066a 0564 0719 007c 005f 047c  ;|.j.j.d...|._.|
+000002a0: 00a0 09a1 0049 0064 0048 0001 0064 0053  .....I.d.H...d.S
+000002b0: 0064 0053 0029 084e 2901 da05 746f 7461  .d.S.).N)...tota
+000002c0: 6cda 0641 6363 6570 747a 1174 6578 742f  l..Acceptz.text/
+000002d0: 6576 656e 742d 7374 7265 616d 4629 0372  event-streamF).r
+000002e0: 0700 0000 da07 7469 6d65 6f75 74da 0f61  ......timeout..a
+000002f0: 6c6c 6f77 5f72 6564 6972 6563 7473 692d  llow_redirectsi-
+00000300: 0100 00da 086c 6f63 6174 696f 6e29 0ada  .....location)..
+00000310: 0761 696f 6874 7470 da0d 436c 6965 6e74  .aiohttp..Client
+00000320: 5469 6d65 6f75 7472 0500 0000 da03 6765  Timeoutr......ge
+00000330: 7472 0600 0000 7207 0000 0072 0900 0000  tr....r....r....
+00000340: da10 7261 6973 655f 666f 725f 7374 6174  ..raise_for_stat
+00000350: 7573 da06 7374 6174 7573 da0f 6372 6561  us..status..crea
+00000360: 7465 5f72 6573 706f 6e73 6529 0272 0a00  te_response).r..
+00000370: 0000 7211 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00000380: 0072 0c00 0000 7219 0000 0011 0000 0073  .r....r........s
+00000390: 1c00 0000 0280 0c01 0602 0401 0c01 0201  ................
+000003a0: 0201 0efc 0a06 0a01 0c02 0e01 1201 04fe  ................
+000003b0: 7a1b 4576 656e 7453 6f75 7263 652e 6372  z.EventSource.cr
+000003c0: 6561 7465 5f72 6573 706f 6e73 6563 0100  eate_responsec..
+000003d0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+000003e0: 0000 4300 0000 7304 0000 007c 0053 0072  ..C...s....|.S.r
+000003f0: 0800 0000 720b 0000 0029 0172 0a00 0000  ....r....).r....
+00000400: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00000410: 095f 5f61 6974 6572 5f5f 2100 0000 7302  .__aiter__!...s.
+00000420: 0000 0004 017a 1545 7665 6e74 536f 7572  .....z.EventSour
+00000430: 6365 2e5f 5f61 6974 6572 5f5f 6301 0000  ce.__aiter__c...
+00000440: 0000 0000 0000 0000 0005 0000 0007 0000  ................
+00000450: 00c3 0000 0073 8a00 0000 8101 7c00 6a00  .....s......|.j.
+00000460: 6400 7500 720d 7c00 a001 a100 4900 6400  d.u.r.|.....I.d.
+00000470: 4800 0100 6401 7d01 7c00 6a00 7314 4a00  H...d.}.|.j.s.J.
+00000480: 8201 7c00 6a00 6a02 3200 7a29 3300 6400  ..|.j.j.2.z)3.d.
+00000490: 4800 5700 7d02 7c02 a003 6402 a101 7d03  H.W.}.|...d...}.
+000004a0: 7c03 6403 1900 6404 6b02 722a 7118 7c03  |.d...d.k.r*q.|.
+000004b0: 6405 6b02 723b 7404 a005 7c01 a101 7d04  d.k.r;t...|...}.
+000004c0: 7c04 6a06 723a 7c04 0200 0100 5300 7118  |.j.r:|.....S.q.
+000004d0: 7c01 9b00 7c03 9b00 9d02 7d01 7118 3600  |...|.....}.q.6.
+000004e0: 6400 5300 2906 4eda 007a 0575 7466 2d38  d.S.).N..z.utf-8
+000004f0: 7201 0000 00fa 013a da01 0a29 0772 0900  r......:...).r..
+00000500: 0000 7219 0000 00da 0763 6f6e 7465 6e74  ..r......content
+00000510: da06 6465 636f 6465 7203 0000 005a 0a70  ..decoder....Z.p
+00000520: 6172 7365 5f75 7466 38da 0464 6174 6129  arse_utf8..data)
+00000530: 0572 0a00 0000 5a08 746f 5f70 6172 7365  .r....Z.to_parse
+00000540: 5a0d 6c69 6e65 5f69 6e5f 6279 7465 73da  Z.line_in_bytes.
+00000550: 046c 696e 65da 0565 7665 6e74 720b 0000  .line..eventr...
+00000560: 0072 0b00 0000 720c 0000 00da 095f 5f61  .r....r......__a
+00000570: 6e65 7874 5f5f 2400 0000 7322 0000 0002  next__$...s"....
+00000580: 800a 010e 0104 020a 0214 020a 010c 0102  ................
+00000590: 0108 010a 0106 0108 0102 ff0e 0302 f704  ................
+000005a0: 0b7a 1545 7665 6e74 536f 7572 6365 2e5f  .z.EventSource._
+000005b0: 5f61 6e65 7874 5f5f 2902 720e 0000 004e  _anext__).r....N
+000005c0: 290c da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000005d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000005e0: 6e61 6d65 5f5f 7214 0000 00da 0d43 6c69  name__r......Cli
+000005f0: 656e 7453 6573 7369 6f6e da03 7374 7272  entSession..strr
+00000600: 0200 0000 720d 0000 0072 1900 0000 721a  ....r....r....r.
+00000610: 0000 0072 0300 0000 7223 0000 0072 0b00  ...r....r#...r..
+00000620: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+00000630: 0072 0400 0000 0800 0000 7318 0000 0008  .r........s.....
+00000640: 0002 0204 ff04 0102 ff02 0102 ff0a 010a  ................
+00000650: ff0a 0808 1016 0372 0400 0000 2906 da06  .......r....)...
+00000660: 7479 7069 6e67 7202 0000 0072 1400 0000  typingr....r....
+00000670: 5a0c 626f 7669 6e65 2e74 7970 6573 7203  Z.bovine.typesr.
+00000680: 0000 0072 0400 0000 720b 0000 0072 0b00  ...r....r....r..
+00000690: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
+000006a0: 6f64 756c 653e 0100 0000 7308 0000 000c  odule>....s.....
+000006b0: 0008 020c 0212 03                        .......
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/lookup_account.cpython-310.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/lookup_account.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 1303 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 1303 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6501 a005 6506 a101 5a07 6404 6502  ..e...e...Z.d.e.
 00000060: 6a08 6405 6509 6406 650a 6606 6407 6408  j.d.e.d.e.f.d.d.
 00000070: 8404 5a0b 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/moo_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 3176 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 680c 0000  o.........Adh...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 b90b 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 8400 5a0c 4700  m.Z...d.d...Z.G.
@@ -16,142 +16,144 @@
 000000f0: 4945 4e54 5f4e 414d 4529 01da 0b45 7665  IENT_NAME)...Eve
 00000100: 6e74 536f 7572 6365 6301 0000 0000 0000  ntSourcec.......
 00000110: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00000120: 0073 1400 0000 7400 7c00 8301 7d01 7c01  .s....t.|...}.|.
 00000130: 6a01 7c01 6a02 6602 5300 a901 4e29 0372  j.|.j.f.S...N).r
 00000140: 0200 0000 da06 6e65 746c 6f63 da04 7061  ......netloc..pa
 00000150: 7468 2902 da03 7572 6cda 0a70 6172 7365  th)...url..parse
-00000160: 645f 7572 6ca9 0072 0e00 0000 fa53 2f77  d_url..r.....S/w
+00000160: 645f 7572 6ca9 0072 0e00 0000 fa4c 2f77  d_url..r.....L/w
 00000170: 6f6f 6470 6563 6b65 722f 7372 632f 636f  oodpecker/src/co
 00000180: 6465 6265 7267 2e6f 7267 2f62 6f76 696e  deberg.org/bovin
 00000190: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
 000001a0: 626f 7669 6e65 2f63 6c69 656e 7473 2f6d  bovine/clients/m
-000001b0: 6f6f 5f61 7574 685f 636c 6965 6e74 2e70  oo_auth_client.p
-000001c0: 79da 1468 6f73 745f 7461 7267 6574 5f66  y..host_target_f
-000001d0: 726f 6d5f 7572 6c0d 0000 0073 0400 0000  rom_url....s....
-000001e0: 0801 0c01 7210 0000 0063 0000 0000 0000  ....r....c......
-000001f0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000200: 0000 733a 0000 0065 005a 0164 005a 0264  ..s:...e.Z.d.Z.d
-00000210: 0164 0284 005a 0369 0066 0164 0364 0484  .d...Z.i.f.d.d..
-00000220: 015a 0469 0064 0566 0264 0664 0784 015a  .Z.i.d.f.d.d...Z
-00000230: 0569 0066 0164 0864 0984 015a 0664 0553  .i.f.d.d...Z.d.S
-00000240: 0029 0ada 0d4d 6f6f 4175 7468 436c 6965  .)...MooAuthClie
-00000250: 6e74 6304 0000 0000 0000 0000 0000 0004  ntc.............
-00000260: 0000 0002 0000 0043 0000 0073 1600 0000  .......C...s....
-00000270: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
-00000280: 5f02 6400 5300 7209 0000 0029 03da 0773  _.d.S.r....)...s
-00000290: 6573 7369 6f6e da07 6469 645f 6b65 79da  ession..did_key.
-000002a0: 0b70 7269 7661 7465 5f6b 6579 2904 da04  .private_key)...
-000002b0: 7365 6c66 7212 0000 0072 1300 0000 7214  selfr....r....r.
-000002c0: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
-000002d0: 0000 da08 5f5f 696e 6974 5f5f 1300 0000  ....__init__....
-000002e0: 7306 0000 0006 0106 010a 017a 164d 6f6f  s..........z.Moo
-000002f0: 4175 7468 436c 6965 6e74 2e5f 5f69 6e69  AuthClient.__ini
-00000300: 745f 5f63 0300 0000 0000 0000 0000 0000  t__c............
-00000310: 0900 0000 0400 0000 c300 0000 738e 0000  ............s...
-00000320: 0081 0174 007c 0183 015c 027d 037d 0464  ...t.|...\.}.}.d
-00000330: 017d 0564 017d 0674 0183 007d 0774 027c  .}.d.}.t...}.t.|
-00000340: 0364 027c 0483 03a0 0364 037c 07a1 02a0  .d.|.....d.|....
-00000350: 047c 006a 05a1 017d 087c 057c 0264 043c  .|.j...}.|.|.d.<
-00000360: 007c 077c 0264 033c 007c 037c 0264 053c  .|.|.d.<.|.|.d.<
-00000370: 007c 067c 0264 063c 0064 077c 006a 069b  .|.|.d.<.d.|.j..
-00000380: 009d 027c 0264 083c 007c 087c 0264 093c  ...|.d.<.|.|.d.<
-00000390: 0074 077c 0264 0a3c 007c 006a 086a 097c  .t.|.d.<.|.j.j.|
-000003a0: 017c 0264 0b8d 0249 0064 0048 0053 0029  .|.d...I.d.H.S.)
-000003b0: 0c4e fa19 6170 706c 6963 6174 696f 6e2f  .N..application/
-000003c0: 6163 7469 7669 7479 2b6a 736f 6eda 0367  activity+json..g
-000003d0: 6574 da04 6461 7465 da06 6163 6365 7074  et..date..accept
-000003e0: da04 686f 7374 fa0c 636f 6e74 656e 742d  ..host..content-
-000003f0: 7479 7065 fa0b 4d6f 6f2d 4175 7468 2d31  type..Moo-Auth-1
-00000400: 20da 0d61 7574 686f 7269 7a61 7469 6f6e   ..authorization
-00000410: fa0f 782d 6d6f 6f2d 7369 676e 6174 7572  ..x-moo-signatur
-00000420: 65fa 0a75 7365 722d 6167 656e 74a9 01da  e..user-agent...
-00000430: 0768 6561 6465 7273 290a 7210 0000 0072  .headers).r....r
-00000440: 0500 0000 7204 0000 00da 0a77 6974 685f  ....r......with_
-00000450: 6669 656c 64da 0c65 6432 3535 3139 5f73  field..ed25519_s
-00000460: 6967 6e72 1400 0000 7213 0000 0072 0700  ignr....r....r..
-00000470: 0000 7212 0000 0072 1800 0000 2909 7215  ..r....r....).r.
-00000480: 0000 0072 0c00 0000 7222 0000 0072 1b00  ...r....r"...r..
-00000490: 0000 da06 7461 7267 6574 721a 0000 00da  ....targetr.....
-000004a0: 0c63 6f6e 7465 6e74 5f74 7970 65da 0b64  .content_type..d
-000004b0: 6174 655f 6865 6164 6572 da10 7369 676e  ate_header..sign
-000004c0: 6174 7572 655f 6865 6164 6572 720e 0000  ature_headerr...
-000004d0: 0072 0e00 0000 720f 0000 0072 1800 0000  .r....r....r....
-000004e0: 1900 0000 7322 0000 0002 800c 0104 0204  ....s"..........
-000004f0: 0106 010a 0308 0108 0102 fd08 0608 0108  ................
-00000500: 0108 0110 0108 0108 0116 027a 114d 6f6f  ...........z.Moo
-00000510: 4175 7468 436c 6965 6e74 2e67 6574 4e63  AuthClient.getNc
-00000520: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
-00000530: 0500 0000 c300 0000 73b0 0000 0081 0174  ........s......t
-00000540: 007c 0183 015c 027d 057d 0664 017d 077c  .|...\.}.}.d.}.|
-00000550: 0464 0075 0072 0f64 017d 0474 0183 007d  .d.u.r.d.}.t...}
-00000560: 0874 027c 0283 017d 0974 037c 0564 027c  .t.|...}.t.|.d.|
-00000570: 0683 03a0 0464 037c 08a1 02a0 0464 047c  .....d.|.....d.|
-00000580: 09a1 02a0 057c 006a 06a1 017d 0a7c 077c  .....|.j...}.|.|
-00000590: 0364 053c 007c 097c 0364 043c 007c 087c  .d.<.|.|.d.<.|.|
-000005a0: 0364 033c 007c 057c 0364 063c 007c 047c  .d.<.|.|.d.<.|.|
-000005b0: 0364 073c 0064 087c 006a 079b 009d 027c  .d.<.d.|.j.....|
-000005c0: 0364 093c 007c 0a7c 0364 0a3c 0074 087c  .d.<.|.|.d.<.t.|
-000005d0: 0364 0b3c 007c 006a 096a 0a7c 017c 027c  .d.<.|.j.j.|.|.|
-000005e0: 0364 0c8d 0349 0064 0048 0053 0029 0d4e  .d...I.d.H.S.).N
-000005f0: 7217 0000 00da 0470 6f73 7472 1900 0000  r......postr....
-00000600: da06 6469 6765 7374 721a 0000 0072 1b00  ..digestr....r..
-00000610: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00000620: 0072 1f00 0000 7220 0000 0029 02da 0464  .r....r ...)...d
-00000630: 6174 6172 2200 0000 290b 7210 0000 0072  atar"...).r....r
-00000640: 0500 0000 7203 0000 0072 0400 0000 7223  ....r....r....r#
-00000650: 0000 0072 2400 0000 7214 0000 0072 1300  ...r$...r....r..
-00000660: 0000 7207 0000 0072 1200 0000 7229 0000  ..r....r....r)..
-00000670: 0029 0b72 1500 0000 720c 0000 00da 0462  .).r....r......b
-00000680: 6f64 7972 2200 0000 7226 0000 0072 1b00  odyr"...r&...r..
-00000690: 0000 7225 0000 0072 1a00 0000 7227 0000  ..r%...r....r'..
-000006a0: 0072 2a00 0000 7228 0000 0072 0e00 0000  .r*...r(...r....
-000006b0: 720e 0000 0072 0f00 0000 7229 0000 0030  r....r....r)...0
-000006c0: 0000 0073 2a00 0000 0280 0c01 0401 0802  ...s*...........
-000006d0: 0401 0601 0802 0a03 0801 0801 0801 02fc  ................
-000006e0: 0807 0801 0802 0801 0801 1001 0801 0801  ................
-000006f0: 1802 7a12 4d6f 6f41 7574 6843 6c69 656e  ..z.MooAuthClien
-00000700: 742e 706f 7374 6303 0000 0000 0000 0000  t.postc.........
-00000710: 0000 0008 0000 0005 0000 0043 0000 0073  ...........C...s
-00000720: 7a00 0000 7400 7c01 8301 5c02 7d03 7d04  z...t.|...\.}.}.
-00000730: 7401 8300 7d05 6401 7d06 7402 7c03 6402  t...}.d.}.t.|.d.
-00000740: 7c04 8303 a003 6403 7c05 a102 a004 7c00  |.....d.|.....|.
-00000750: 6a05 a101 7d07 7c06 7c02 6404 3c00 7c05  j...}.|.|.d.<.|.
-00000760: 7c02 6403 3c00 7c03 7c02 6405 3c00 6406  |.d.<.|.|.d.<.d.
-00000770: 7c00 6a06 9b00 9d02 7c02 6407 3c00 7c07  |.j.....|.d.<.|.
-00000780: 7c02 6408 3c00 7407 7c02 6409 3c00 7408  |.d.<.t.|.d.<.t.
-00000790: 7c00 6a09 7c01 7c02 640a 8d03 5300 290b  |.j.|.|.d...S.).
-000007a0: 4e7a 1174 6578 742f 6576 656e 742d 7374  Nz.text/event-st
-000007b0: 7265 616d 7218 0000 0072 1900 0000 721a  reamr....r....r.
-000007c0: 0000 0072 1b00 0000 721d 0000 0072 1e00  ...r....r....r..
-000007d0: 0000 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-000007e0: 0029 0a72 1000 0000 7205 0000 0072 0400  .).r....r....r..
-000007f0: 0000 7223 0000 0072 2400 0000 7214 0000  ..r#...r$...r...
-00000800: 0072 1300 0000 7207 0000 0072 0800 0000  .r....r....r....
-00000810: 7212 0000 0029 0872 1500 0000 720c 0000  r....).r....r...
-00000820: 0072 2200 0000 721b 0000 0072 2500 0000  .r"...r....r%...
-00000830: 7227 0000 0072 1a00 0000 7228 0000 0072  r'...r....r(...r
-00000840: 0e00 0000 720e 0000 0072 0f00 0000 da0c  ....r....r......
-00000850: 6576 656e 745f 736f 7572 6365 4d00 0000  event_sourceM...
-00000860: 731c 0000 000c 0106 0104 010a 0208 0108  s...............
-00000870: 0102 fd08 0608 0108 0110 0108 0108 0110  ................
-00000880: 027a 1a4d 6f6f 4175 7468 436c 6965 6e74  .z.MooAuthClient
-00000890: 2e65 7665 6e74 5f73 6f75 7263 6529 07da  .event_source)..
-000008a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000008b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000008c0: 655f 5f72 1600 0000 7218 0000 0072 2900  e__r....r....r).
-000008d0: 0000 722d 0000 0072 0e00 0000 720e 0000  ..r-...r....r...
-000008e0: 0072 0e00 0000 720f 0000 0072 1100 0000  .r....r....r....
-000008f0: 1200 0000 730a 0000 0008 0008 010c 060e  ....s...........
-00000900: 1710 1d72 1100 0000 4e29 0eda 0c75 726c  ...r....N)...url
-00000910: 6c69 622e 7061 7273 6572 0200 0000 5a14  lib.parser....Z.
-00000920: 626f 7669 6e65 2e63 7279 7074 6f2e 6865  bovine.crypto.he
-00000930: 6c70 6572 7203 0000 005a 1c62 6f76 696e  lperr....Z.bovin
-00000940: 652e 6372 7970 746f 2e68 7474 705f 7369  e.crypto.http_si
-00000950: 676e 6174 7572 6572 0400 0000 5a11 626f  gnaturer....Z.bo
-00000960: 7669 6e65 2e75 7469 6c73 2e64 6174 6572  vine.utils.dater
-00000970: 0500 0000 da06 636f 6e73 7473 7207 0000  ......constsr...
-00000980: 0072 2d00 0000 7208 0000 0072 1000 0000  .r-...r....r....
-00000990: 7211 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-000009a0: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-000009b0: 6c65 3e01 0000 0073 1000 0000 0c00 0c02  le>....s........
-000009c0: 0c01 0c01 0c02 0c01 0805 1205            ............
+000001b0: 6f6f 5f61 7574 682e 7079 da14 686f 7374  oo_auth.py..host
+000001c0: 5f74 6172 6765 745f 6672 6f6d 5f75 726c  _target_from_url
+000001d0: 0b00 0000 7304 0000 0008 010c 0172 1000  ....s........r..
+000001e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000001f0: 0000 0003 0000 0040 0000 0073 3e00 0000  .......@...s>...
+00000200: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
+00000210: 8400 5a04 6900 6601 6404 6405 8401 5a05  ..Z.i.f.d.d...Z.
+00000220: 6900 6406 6602 6407 6408 8401 5a06 6900  i.d.f.d.d...Z.i.
+00000230: 6601 6409 640a 8401 5a07 6406 5300 290b  f.d.d...Z.d.S.).
+00000240: da0d 4d6f 6f41 7574 6843 6c69 656e 747a  ..MooAuthClientz
+00000250: 2a43 6c69 656e 7420 666f 7220 7573 696e  *Client for usin
+00000260: 6720 4d6f 6f2d 4175 7468 2d31 2061 7574  g Moo-Auth-1 aut
+00000270: 6865 6e74 6963 6174 696f 6e63 0400 0000  henticationc....
+00000280: 0000 0000 0000 0000 0400 0000 0200 0000  ................
+00000290: 4300 0000 7316 0000 007c 017c 005f 007c  C...s....|.|._.|
+000002a0: 027c 005f 017c 037c 005f 0264 0053 0072  .|._.|.|._.d.S.r
+000002b0: 0900 0000 2903 da07 7365 7373 696f 6eda  ....)...session.
+000002c0: 0764 6964 5f6b 6579 da0b 7072 6976 6174  .did_key..privat
+000002d0: 655f 6b65 7929 04da 0473 656c 6672 1200  e_key)...selfr..
+000002e0: 0000 7213 0000 0072 1400 0000 720e 0000  ..r....r....r...
+000002f0: 0072 0e00 0000 720f 0000 00da 085f 5f69  .r....r......__i
+00000300: 6e69 745f 5f13 0000 0073 0600 0000 0601  nit__....s......
+00000310: 0601 0a01 7a16 4d6f 6f41 7574 6843 6c69  ....z.MooAuthCli
+00000320: 656e 742e 5f5f 696e 6974 5f5f 6303 0000  ent.__init__c...
+00000330: 0000 0000 0000 0000 0008 0000 0004 0000  ................
+00000340: 00c3 0000 0073 8200 0000 8101 7400 7c01  .....s......t.|.
+00000350: 8301 5c02 7d03 7d04 6401 7d05 7401 8300  ..\.}.}.d.}.t...
+00000360: 7d06 7402 7c03 6402 7c04 8303 a003 6403  }.t.|.d.|.....d.
+00000370: 7c06 a102 a004 7c00 6a05 a101 7d07 7c05  |.....|.j...}.|.
+00000380: 7c02 6404 3c00 7c06 7c02 6403 3c00 7c03  |.d.<.|.|.d.<.|.
+00000390: 7c02 6405 3c00 6406 7c00 6a06 9b00 9d02  |.d.<.d.|.j.....
+000003a0: 7c02 6407 3c00 7c07 7c02 6408 3c00 7407  |.d.<.|.|.d.<.t.
+000003b0: 7c02 6409 3c00 7c00 6a08 6a09 7c01 7c02  |.d.<.|.j.j.|.|.
+000003c0: 640a 8d02 4900 6400 4800 5300 290b 4efa  d...I.d.H.S.).N.
+000003d0: 1961 7070 6c69 6361 7469 6f6e 2f61 6374  .application/act
+000003e0: 6976 6974 792b 6a73 6f6e da03 6765 74da  ivity+json..get.
+000003f0: 0464 6174 65da 0661 6363 6570 74da 0468  .date..accept..h
+00000400: 6f73 74fa 0b4d 6f6f 2d41 7574 682d 3120  ost..Moo-Auth-1 
+00000410: da0d 6175 7468 6f72 697a 6174 696f 6efa  ..authorization.
+00000420: 0f78 2d6d 6f6f 2d73 6967 6e61 7475 7265  .x-moo-signature
+00000430: fa0a 7573 6572 2d61 6765 6e74 a901 da07  ..user-agent....
+00000440: 6865 6164 6572 7329 0a72 1000 0000 7205  headers).r....r.
+00000450: 0000 0072 0400 0000 da0a 7769 7468 5f66  ...r......with_f
+00000460: 6965 6c64 da0c 6564 3235 3531 395f 7369  ield..ed25519_si
+00000470: 676e 7214 0000 0072 1300 0000 7207 0000  gnr....r....r...
+00000480: 0072 1200 0000 7218 0000 0029 0872 1500  .r....r....).r..
+00000490: 0000 720c 0000 0072 2100 0000 721b 0000  ..r....r!...r...
+000004a0: 00da 0674 6172 6765 7472 1a00 0000 da0b  ...targetr......
+000004b0: 6461 7465 5f68 6561 6465 72da 1073 6967  date_header..sig
+000004c0: 6e61 7475 7265 5f68 6561 6465 7272 0e00  nature_headerr..
+000004d0: 0000 720e 0000 0072 0f00 0000 7218 0000  ..r....r....r...
+000004e0: 0018 0000 0073 1e00 0000 0280 0c01 0402  .....s..........
+000004f0: 0601 0a03 0801 0801 02fd 0806 0801 0801  ................
+00000500: 1001 0801 0801 1602 7a11 4d6f 6f41 7574  ........z.MooAut
+00000510: 6843 6c69 656e 742e 6765 744e 6305 0000  hClient.getNc...
+00000520: 0000 0000 0000 0000 000b 0000 0005 0000  ................
+00000530: 00c3 0000 0073 b000 0000 8101 7400 7c01  .....s......t.|.
+00000540: 8301 5c02 7d05 7d06 6401 7d07 7c04 6400  ..\.}.}.d.}.|.d.
+00000550: 7500 720f 6401 7d04 7401 8300 7d08 7402  u.r.d.}.t...}.t.
+00000560: 7c02 8301 7d09 7403 7c05 6402 7c06 8303  |...}.t.|.d.|...
+00000570: a004 6403 7c08 a102 a004 6404 7c09 a102  ..d.|.....d.|...
+00000580: a005 7c00 6a06 a101 7d0a 7c07 7c03 6405  ..|.j...}.|.|.d.
+00000590: 3c00 7c09 7c03 6404 3c00 7c08 7c03 6403  <.|.|.d.<.|.|.d.
+000005a0: 3c00 7c05 7c03 6406 3c00 7c04 7c03 6407  <.|.|.d.<.|.|.d.
+000005b0: 3c00 6408 7c00 6a07 9b00 9d02 7c03 6409  <.d.|.j.....|.d.
+000005c0: 3c00 7c0a 7c03 640a 3c00 7408 7c03 640b  <.|.|.d.<.t.|.d.
+000005d0: 3c00 7c00 6a09 6a0a 7c01 7c02 7c03 640c  <.|.j.j.|.|.|.d.
+000005e0: 8d03 4900 6400 4800 5300 290d 4e72 1700  ..I.d.H.S.).Nr..
+000005f0: 0000 da04 706f 7374 7219 0000 00da 0664  ....postr......d
+00000600: 6967 6573 7472 1a00 0000 721b 0000 007a  igestr....r....z
+00000610: 0c63 6f6e 7465 6e74 2d74 7970 6572 1c00  .content-typer..
+00000620: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000630: 0029 02da 0464 6174 6172 2100 0000 290b  .)...datar!...).
+00000640: 7210 0000 0072 0500 0000 7203 0000 0072  r....r....r....r
+00000650: 0400 0000 7222 0000 0072 2300 0000 7214  ....r"...r#...r.
+00000660: 0000 0072 1300 0000 7207 0000 0072 1200  ...r....r....r..
+00000670: 0000 7227 0000 0029 0b72 1500 0000 720c  ..r'...).r....r.
+00000680: 0000 00da 0462 6f64 7972 2100 0000 da0c  .....bodyr!.....
+00000690: 636f 6e74 656e 745f 7479 7065 721b 0000  content_typer...
+000006a0: 0072 2400 0000 721a 0000 0072 2500 0000  .r$...r....r%...
+000006b0: 7228 0000 0072 2600 0000 720e 0000 0072  r(...r&...r....r
+000006c0: 0e00 0000 720f 0000 0072 2700 0000 2d00  ....r....r'...-.
+000006d0: 0000 732a 0000 0002 800c 0104 0108 0204  ..s*............
+000006e0: 0106 0108 020a 0308 0108 0108 0102 fc08  ................
+000006f0: 0708 0108 0208 0108 0110 0108 0108 0118  ................
+00000700: 027a 124d 6f6f 4175 7468 436c 6965 6e74  .z.MooAuthClient
+00000710: 2e70 6f73 7463 0300 0000 0000 0000 0000  .postc..........
+00000720: 0000 0800 0000 0500 0000 4300 0000 737a  ..........C...sz
+00000730: 0000 0074 007c 0183 015c 027d 037d 0474  ...t.|...\.}.}.t
+00000740: 0183 007d 0564 017d 0674 027c 0364 027c  ...}.d.}.t.|.d.|
+00000750: 0483 03a0 0364 037c 05a1 02a0 047c 006a  .....d.|.....|.j
+00000760: 05a1 017d 077c 067c 0264 043c 007c 057c  ...}.|.|.d.<.|.|
+00000770: 0264 033c 007c 037c 0264 053c 0064 067c  .d.<.|.|.d.<.d.|
+00000780: 006a 069b 009d 027c 0264 073c 007c 077c  .j.....|.d.<.|.|
+00000790: 0264 083c 0074 077c 0264 093c 0074 087c  .d.<.t.|.d.<.t.|
+000007a0: 006a 097c 017c 0264 0a8d 0353 0029 0b4e  .j.|.|.d...S.).N
+000007b0: 7a11 7465 7874 2f65 7665 6e74 2d73 7472  z.text/event-str
+000007c0: 6561 6d72 1800 0000 7219 0000 0072 1a00  eamr....r....r..
+000007d0: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+000007e0: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+000007f0: 290a 7210 0000 0072 0500 0000 7204 0000  ).r....r....r...
+00000800: 0072 2200 0000 7223 0000 0072 1400 0000  .r"...r#...r....
+00000810: 7213 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+00000820: 1200 0000 2908 7215 0000 0072 0c00 0000  ....).r....r....
+00000830: 7221 0000 0072 1b00 0000 7224 0000 0072  r!...r....r$...r
+00000840: 2500 0000 721a 0000 0072 2600 0000 720e  %...r....r&...r.
+00000850: 0000 0072 0e00 0000 720f 0000 00da 0c65  ...r....r......e
+00000860: 7665 6e74 5f73 6f75 7263 654a 0000 0073  vent_sourceJ...s
+00000870: 1c00 0000 0c01 0601 0401 0a02 0801 0801  ................
+00000880: 02fd 0806 0801 0801 1001 0801 0801 1002  ................
+00000890: 7a1a 4d6f 6f41 7574 6843 6c69 656e 742e  z.MooAuthClient.
+000008a0: 6576 656e 745f 736f 7572 6365 2908 da08  event_source)...
+000008b0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000008c0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000008d0: 5f5f da07 5f5f 646f 635f 5f72 1600 0000  __..__doc__r....
+000008e0: 7218 0000 0072 2700 0000 722c 0000 0072  r....r'...r,...r
+000008f0: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+00000900: 0000 0072 1100 0000 1000 0000 730c 0000  ...r........s...
+00000910: 0008 0004 0108 020c 050e 1510 1d72 1100  .............r..
+00000920: 0000 4e29 0eda 0c75 726c 6c69 622e 7061  ..N)...urllib.pa
+00000930: 7273 6572 0200 0000 5a14 626f 7669 6e65  rser....Z.bovine
+00000940: 2e63 7279 7074 6f2e 6865 6c70 6572 7203  .crypto.helperr.
+00000950: 0000 005a 1c62 6f76 696e 652e 6372 7970  ...Z.bovine.cryp
+00000960: 746f 2e68 7474 705f 7369 676e 6174 7572  to.http_signatur
+00000970: 6572 0400 0000 da11 626f 7669 6e65 2e75  er......bovine.u
+00000980: 7469 6c73 2e64 6174 6572 0500 0000 da06  tils.dater......
+00000990: 636f 6e73 7473 7207 0000 0072 2c00 0000  constsr....r,...
+000009a0: 7208 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+000009b0: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+000009c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000009d0: 0073 1000 0000 0c00 0c02 0c01 0c01 0c02  .s..............
+000009e0: 0c01 0803 1205                           ......
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 948 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 b403 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 b403 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6501 a006 6507  d.l.m.Z...e...e.
 00000060: a101 5a08 6404 6503 6a09 6405 650a 6406  ..Z.d.e.j.d.e.d.
 00000070: 650b 6606 6407 6408 8404 5a0c 6404 6503  e.f.d.d...Z.d.e.
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/signed_http.cpython-310.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 3278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 ce0c 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 ce0c 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
@@ -53,103 +53,103 @@
 00000340: 0072 1100 0000 290c 7209 0000 0072 0a00  .r....).r....r..
 00000350: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
 00000360: 00da 0a70 6172 7365 645f 7572 6c72 1400  ...parsed_urlr..
 00000370: 0000 da06 7461 7267 6574 7213 0000 00da  ....targetr.....
 00000380: 0c63 6f6e 7465 6e74 5f74 7970 65da 0b64  .content_type..d
 00000390: 6174 655f 6865 6164 6572 da10 7369 676e  ate_header..sign
 000003a0: 6174 7572 655f 6865 6164 6572 a900 7223  ature_header..r#
-000003b0: 0000 00fa 4f2f 776f 6f64 7065 636b 6572  ....O/woodpecker
+000003b0: 0000 00fa 572f 776f 6f64 7065 636b 6572  ....W/woodpecker
 000003c0: 2f73 7263 2f63 6f64 6562 6572 672e 6f72  /src/codeberg.or
 000003d0: 672f 626f 7669 6e65 2f62 6f76 696e 652f  g/bovine/bovine/
 000003e0: 626f 7669 6e65 2f62 6f76 696e 652f 636c  bovine/bovine/cl
 000003f0: 6965 6e74 732f 7369 676e 6564 5f68 7474  ients/signed_htt
-00000400: 702e 7079 da0a 7369 676e 6564 5f67 6574  p.py..signed_get
-00000410: 1000 0000 7328 0000 0002 8016 0708 0206  ....s(..........
-00000420: 0106 0104 0204 0106 010a 0308 0108 0108  ................
-00000430: 0102 fc08 0708 0108 0108 0108 0108 0114  ................
-00000440: 0172 2500 0000 6305 0000 0000 0000 0000  .r%...c.........
-00000450: 0000 000b 0000 0006 0000 0043 0000 0073  ...........C...s
-00000460: 8e00 0000 7400 a001 6401 7c01 9b00 6402  ....t...d.|...d.
-00000470: 7c03 9b00 9d04 a101 0100 7402 7c03 8301  |.........t.|...
-00000480: 7d05 7c05 6a03 7d06 7c05 6a04 7d07 6403  }.|.j.}.|.j.}.d.
-00000490: 7d08 7405 8300 7d09 7406 7c06 6404 7c07  }.t...}.t.|.d.|.
-000004a0: 8303 a007 6405 7c09 a102 a007 6406 7c08  ....d.|.....d.|.
-000004b0: a102 a006 7c01 7c02 a102 7d0a 7c08 7c04  ....|.|...}.|.|.
-000004c0: 6406 3c00 7c09 7c04 6405 3c00 7c06 7c04  d.<.|.|.d.<.|.|.
-000004d0: 6407 3c00 7c0a 7c04 6408 3c00 7408 7c04  d.<.|.|.d.<.t.|.
-000004e0: 6409 3c00 7409 7c00 7c03 7c04 640a 8d03  d.<.t.|.|.|.d...
-000004f0: 5300 290b 4e7a 1953 6967 6e65 6420 6576  S.).Nz.Signed ev
-00000500: 656e 7420 736f 7572 6365 2077 6974 6820  ent source with 
-00000510: 720f 0000 007a 1174 6578 742f 6576 656e  r....z.text/even
-00000520: 742d 7374 7265 616d 7211 0000 0072 1200  t-streamr....r..
-00000530: 0000 7213 0000 0072 1400 0000 7216 0000  ..r....r....r...
-00000540: 0072 1700 0000 7218 0000 0029 0a72 1900  .r....r....).r..
-00000550: 0000 721a 0000 0072 0200 0000 721b 0000  ..r....r....r...
-00000560: 0072 1c00 0000 7205 0000 0072 0400 0000  .r....r....r....
-00000570: 721d 0000 0072 0700 0000 7208 0000 0029  r....r....r....)
-00000580: 0b72 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000590: 720c 0000 0072 0d00 0000 721e 0000 0072  r....r....r....r
-000005a0: 1400 0000 721f 0000 0072 1300 0000 7221  ....r....r....r!
-000005b0: 0000 0072 2200 0000 7223 0000 0072 2300  ...r"...r#...r#.
-000005c0: 0000 7224 0000 00da 1373 6967 6e65 645f  ..r$.....signed_
-000005d0: 6576 656e 745f 736f 7572 6365 3100 0000  event_source1...
-000005e0: 7322 0000 0016 0708 0206 0106 0104 0206  s"..............
-000005f0: 010a 0308 0108 0108 0102 fc08 0708 0108  ................
-00000600: 0108 0108 010e 0172 2600 0000 da04 626f  .......r&.....bo
-00000610: 6479 6307 0000 0000 0000 0000 0000 000e  dyc.............
-00000620: 0000 0006 0000 00c3 0000 0073 c400 0000  ...........s....
-00000630: 8101 7400 a001 6401 7c01 9b00 6402 7c03  ..t...d.|...d.|.
-00000640: 9b00 9d04 a101 0100 7402 7c03 8301 7d07  ........t.|...}.
-00000650: 7c07 6a03 7d08 7c07 6a04 7d09 6403 7d0a  |.j.}.|.j.}.d.}.
-00000660: 7c06 6400 7500 721e 6403 7d06 7405 8300  |.d.u.r.d.}.t...
-00000670: 7d0b 7406 7c04 8301 7d0c 7407 7c08 6404  }.t.|...}.t.|.d.
-00000680: 7c09 8303 a008 6405 7c0b a102 a008 6406  |.....d.|.....d.
-00000690: 7c0c a102 a008 6407 7c06 a102 a007 7c01  |.....d.|.....|.
-000006a0: 7c02 a102 7d0d 7c0a 7c05 6408 3c00 7c0c  |...}.|.|.d.<.|.
-000006b0: 7c05 6406 3c00 7c0b 7c05 6405 3c00 7c08  |.d.<.|.|.d.<.|.
-000006c0: 7c05 6409 3c00 7c06 7c05 6407 3c00 7c0d  |.d.<.|.|.d.<.|.
-000006d0: 7c05 640a 3c00 7409 7c05 640b 3c00 7c00  |.d.<.t.|.d.<.|.
-000006e0: 6a0a 7c03 7c04 7c05 640c 8d03 4900 6400  j.|.|.|.d...I.d.
-000006f0: 4800 5300 290d 4e7a 1153 6967 6e65 6420  H.S.).Nz.Signed 
-00000700: 706f 7374 2077 6974 6820 720f 0000 0072  post with r....r
-00000710: 1000 0000 da04 706f 7374 7212 0000 00da  ......postr.....
-00000720: 0664 6967 6573 7472 1500 0000 7213 0000  .digestr....r...
-00000730: 0072 1400 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000740: 2902 da04 6461 7461 720d 0000 0029 0b72  )...datar....).r
-00000750: 1900 0000 721a 0000 0072 0200 0000 721b  ....r....r....r.
-00000760: 0000 0072 1c00 0000 7205 0000 0072 0300  ...r....r....r..
-00000770: 0000 7204 0000 0072 1d00 0000 7207 0000  ..r....r....r...
-00000780: 0072 2800 0000 290e 7209 0000 0072 0a00  .r(...).r....r..
-00000790: 0000 720b 0000 0072 0c00 0000 7227 0000  ..r....r....r'..
-000007a0: 0072 0d00 0000 7220 0000 0072 1e00 0000  .r....r ...r....
-000007b0: 7214 0000 0072 1f00 0000 7213 0000 0072  r....r....r....r
-000007c0: 2100 0000 7229 0000 0072 2200 0000 7223  !...r)...r"...r#
-000007d0: 0000 0072 2300 0000 7224 0000 00da 0b73  ...r#...r$.....s
-000007e0: 6967 6e65 645f 706f 7374 5000 0000 7330  igned_postP...s0
-000007f0: 0000 0002 8016 0908 0206 0106 0104 0208  ................
-00000800: 0204 0106 0108 020a 0308 0108 0108 0108  ................
-00000810: 0102 fb08 0808 0108 0108 0108 0108 0108  ................
-00000820: 0116 0272 2b00 0000 2918 da07 6c6f 6767  ...r+...)...logg
-00000830: 696e 67da 0c75 726c 6c69 622e 7061 7273  ing..urllib.pars
-00000840: 6572 0200 0000 da07 6169 6f68 7474 705a  er......aiohttpZ
-00000850: 1462 6f76 696e 652e 6372 7970 746f 2e68  .bovine.crypto.h
-00000860: 656c 7065 7272 0300 0000 5a1c 626f 7669  elperr....Z.bovi
-00000870: 6e65 2e63 7279 7074 6f2e 6874 7470 5f73  ne.crypto.http_s
-00000880: 6967 6e61 7475 7265 7204 0000 00da 1162  ignaturer......b
-00000890: 6f76 696e 652e 7574 696c 732e 6461 7465  ovine.utils.date
-000008a0: 7205 0000 00da 0663 6f6e 7374 7372 0700  r......constsr..
-000008b0: 0000 da0c 6576 656e 745f 736f 7572 6365  ....event_source
-000008c0: 7208 0000 00da 0967 6574 4c6f 6767 6572  r......getLogger
-000008d0: da08 5f5f 6e61 6d65 5f5f 7219 0000 00da  ..__name__r.....
-000008e0: 0d43 6c69 656e 7453 6573 7369 6f6e da03  .ClientSession..
-000008f0: 7374 72da 0464 6963 74da 0e43 6c69 656e  str..dict..Clien
-00000900: 7452 6573 706f 6e73 6572 2500 0000 7226  tResponser%...r&
-00000910: 0000 0072 2b00 0000 7223 0000 0072 2300  ...r+...r#...r#.
-00000920: 0000 7223 0000 0072 2400 0000 da08 3c6d  ..r#...r$.....<m
-00000930: 6f64 756c 653e 0100 0000 7368 0000 0008  odule>....sh....
-00000940: 000c 0108 020c 020c 010c 010c 020c 010a  ................
-00000950: 0202 0804 fb04 0102 ff02 0202 fe02 0302  ................
-00000960: fd02 0402 fc02 0502 fb04 060a fa02 2604  ..............&.
-00000970: fb04 0102 ff02 0202 fe02 0302 fd02 0402  ................
-00000980: fc02 050a fb02 2502 0104 f904 0102 ff02  ......%.........
-00000990: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
-000009a0: 0602 fa04 080e f8                        .......
+00000400: 705f 6d65 7468 6f64 732e 7079 da0a 7369  p_methods.py..si
+00000410: 676e 6564 5f67 6574 1000 0000 7328 0000  gned_get....s(..
+00000420: 0002 8016 0708 0206 0106 0104 0204 0106  ................
+00000430: 010a 0308 0108 0108 0102 fc08 0708 0108  ................
+00000440: 0108 0108 0108 0114 0172 2500 0000 6305  .........r%...c.
+00000450: 0000 0000 0000 0000 0000 000b 0000 0006  ................
+00000460: 0000 0043 0000 0073 8e00 0000 7400 a001  ...C...s....t...
+00000470: 6401 7c01 9b00 6402 7c03 9b00 9d04 a101  d.|...d.|.......
+00000480: 0100 7402 7c03 8301 7d05 7c05 6a03 7d06  ..t.|...}.|.j.}.
+00000490: 7c05 6a04 7d07 6403 7d08 7405 8300 7d09  |.j.}.d.}.t...}.
+000004a0: 7406 7c06 6404 7c07 8303 a007 6405 7c09  t.|.d.|.....d.|.
+000004b0: a102 a007 6406 7c08 a102 a006 7c01 7c02  ....d.|.....|.|.
+000004c0: a102 7d0a 7c08 7c04 6406 3c00 7c09 7c04  ..}.|.|.d.<.|.|.
+000004d0: 6405 3c00 7c06 7c04 6407 3c00 7c0a 7c04  d.<.|.|.d.<.|.|.
+000004e0: 6408 3c00 7408 7c04 6409 3c00 7409 7c00  d.<.t.|.d.<.t.|.
+000004f0: 7c03 7c04 640a 8d03 5300 290b 4e7a 1953  |.|.d...S.).Nz.S
+00000500: 6967 6e65 6420 6576 656e 7420 736f 7572  igned event sour
+00000510: 6365 2077 6974 6820 720f 0000 007a 1174  ce with r....z.t
+00000520: 6578 742f 6576 656e 742d 7374 7265 616d  ext/event-stream
+00000530: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000540: 1400 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00000550: 0000 0029 0a72 1900 0000 721a 0000 0072  ...).r....r....r
+00000560: 0200 0000 721b 0000 0072 1c00 0000 7205  ....r....r....r.
+00000570: 0000 0072 0400 0000 721d 0000 0072 0700  ...r....r....r..
+00000580: 0000 7208 0000 0029 0b72 0900 0000 720a  ..r....).r....r.
+00000590: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
+000005a0: 0000 721e 0000 0072 1400 0000 721f 0000  ..r....r....r...
+000005b0: 0072 1300 0000 7221 0000 0072 2200 0000  .r....r!...r"...
+000005c0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
+000005d0: 1373 6967 6e65 645f 6576 656e 745f 736f  .signed_event_so
+000005e0: 7572 6365 3100 0000 7322 0000 0016 0708  urce1...s"......
+000005f0: 0206 0106 0104 0206 010a 0308 0108 0108  ................
+00000600: 0102 fc08 0708 0108 0108 0108 010e 0172  ...............r
+00000610: 2600 0000 da04 626f 6479 6307 0000 0000  &.....bodyc.....
+00000620: 0000 0000 0000 000e 0000 0006 0000 00c3  ................
+00000630: 0000 0073 c400 0000 8101 7400 a001 6401  ...s......t...d.
+00000640: 7c01 9b00 6402 7c03 9b00 9d04 a101 0100  |...d.|.........
+00000650: 7402 7c03 8301 7d07 7c07 6a03 7d08 7c07  t.|...}.|.j.}.|.
+00000660: 6a04 7d09 6403 7d0a 7c06 6400 7500 721e  j.}.d.}.|.d.u.r.
+00000670: 6403 7d06 7405 8300 7d0b 7406 7c04 8301  d.}.t...}.t.|...
+00000680: 7d0c 7407 7c08 6404 7c09 8303 a008 6405  }.t.|.d.|.....d.
+00000690: 7c0b a102 a008 6406 7c0c a102 a008 6407  |.....d.|.....d.
+000006a0: 7c06 a102 a007 7c01 7c02 a102 7d0d 7c0a  |.....|.|...}.|.
+000006b0: 7c05 6408 3c00 7c0c 7c05 6406 3c00 7c0b  |.d.<.|.|.d.<.|.
+000006c0: 7c05 6405 3c00 7c08 7c05 6409 3c00 7c06  |.d.<.|.|.d.<.|.
+000006d0: 7c05 6407 3c00 7c0d 7c05 640a 3c00 7409  |.d.<.|.|.d.<.t.
+000006e0: 7c05 640b 3c00 7c00 6a0a 7c03 7c04 7c05  |.d.<.|.j.|.|.|.
+000006f0: 640c 8d03 4900 6400 4800 5300 290d 4e7a  d...I.d.H.S.).Nz
+00000700: 1153 6967 6e65 6420 706f 7374 2077 6974  .Signed post wit
+00000710: 6820 720f 0000 0072 1000 0000 da04 706f  h r....r......po
+00000720: 7374 7212 0000 00da 0664 6967 6573 7472  str......digestr
+00000730: 1500 0000 7213 0000 0072 1400 0000 7216  ....r....r....r.
+00000740: 0000 0072 1700 0000 2902 da04 6461 7461  ...r....)...data
+00000750: 720d 0000 0029 0b72 1900 0000 721a 0000  r....).r....r...
+00000760: 0072 0200 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000770: 7205 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
+00000780: 1d00 0000 7207 0000 0072 2800 0000 290e  ....r....r(...).
+00000790: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+000007a0: 0c00 0000 7227 0000 0072 0d00 0000 7220  ....r'...r....r 
+000007b0: 0000 0072 1e00 0000 7214 0000 0072 1f00  ...r....r....r..
+000007c0: 0000 7213 0000 0072 2100 0000 7229 0000  ..r....r!...r)..
+000007d0: 0072 2200 0000 7223 0000 0072 2300 0000  .r"...r#...r#...
+000007e0: 7224 0000 00da 0b73 6967 6e65 645f 706f  r$.....signed_po
+000007f0: 7374 5000 0000 7330 0000 0002 8016 0908  stP...s0........
+00000800: 0206 0106 0104 0208 0204 0106 0108 020a  ................
+00000810: 0308 0108 0108 0108 0102 fb08 0808 0108  ................
+00000820: 0108 0108 0108 0108 0116 0272 2b00 0000  ...........r+...
+00000830: 2918 da07 6c6f 6767 696e 67da 0c75 726c  )...logging..url
+00000840: 6c69 622e 7061 7273 6572 0200 0000 da07  lib.parser......
+00000850: 6169 6f68 7474 705a 1462 6f76 696e 652e  aiohttpZ.bovine.
+00000860: 6372 7970 746f 2e68 656c 7065 7272 0300  crypto.helperr..
+00000870: 0000 5a1c 626f 7669 6e65 2e63 7279 7074  ..Z.bovine.crypt
+00000880: 6f2e 6874 7470 5f73 6967 6e61 7475 7265  o.http_signature
+00000890: 7204 0000 00da 1162 6f76 696e 652e 7574  r......bovine.ut
+000008a0: 696c 732e 6461 7465 7205 0000 00da 0663  ils.dater......c
+000008b0: 6f6e 7374 7372 0700 0000 da0c 6576 656e  onstsr......even
+000008c0: 745f 736f 7572 6365 7208 0000 00da 0967  t_sourcer......g
+000008d0: 6574 4c6f 6767 6572 da08 5f5f 6e61 6d65  etLogger..__name
+000008e0: 5f5f 7219 0000 00da 0d43 6c69 656e 7453  __r......ClientS
+000008f0: 6573 7369 6f6e da03 7374 72da 0464 6963  ession..str..dic
+00000900: 74da 0e43 6c69 656e 7452 6573 706f 6e73  t..ClientRespons
+00000910: 6572 2500 0000 7226 0000 0072 2b00 0000  er%...r&...r+...
+00000920: 7223 0000 0072 2300 0000 7223 0000 0072  r#...r#...r#...r
+00000930: 2400 0000 da08 3c6d 6f64 756c 653e 0100  $.....<module>..
+00000940: 0000 7368 0000 0008 000c 0108 020c 020c  ..sh............
+00000950: 010c 010c 020c 010a 0202 0804 fb04 0102  ................
+00000960: ff02 0202 fe02 0302 fd02 0402 fc02 0502  ................
+00000970: fb04 060a fa02 2604 fb04 0102 ff02 0202  ......&.........
+00000980: fe02 0302 fd02 0402 fc02 050a fb02 2502  ..............%.
+00000990: 0104 f904 0102 ff02 0202 fe02 0302 fd02  ................
+000009a0: 0402 fc02 0502 fb02 0602 fa04 080e f8    ...............
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/signed_http.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1074 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,96 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 3204 0000  o.........Ad2...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 7e04 0000  o.......*.Nd~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a02 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000060: 0003 0000 0040 0000 0073 4000 0000 6500  .....@...s@...e.
-00000070: 5a01 6400 5a02 640c 6402 6403 8401 5a03  Z.d.Z.d.d.d...Z.
-00000080: 6404 6405 8400 5a04 6900 6601 6406 6407  d.d...Z.i.f.d.d.
-00000090: 8401 5a05 6900 6401 6602 6408 6409 8401  ..Z.i.d.f.d.d...
-000000a0: 5a06 640a 640b 8400 5a07 6401 5300 290d  Z.d.d...Z.d.S.).
-000000b0: da10 5369 676e 6564 4874 7470 436c 6965  ..SignedHttpClie
-000000c0: 6e74 4e63 0500 0000 0000 0000 0000 0000  ntNc............
-000000d0: 0500 0000 0200 0000 4300 0000 731c 0000  ........C...s...
-000000e0: 007c 017c 005f 007c 027c 005f 017c 037c  .|.|._.|.|._.|.|
-000000f0: 005f 027c 047c 005f 0364 0053 00a9 014e  ._.|.|._.d.S...N
-00000100: 2904 da07 7365 7373 696f 6eda 0e70 7562  )...session..pub
-00000110: 6c69 635f 6b65 795f 7572 6cda 0b70 7269  lic_key_url..pri
-00000120: 7661 7465 5f6b 6579 da0b 6163 636f 756e  vate_key..accoun
-00000130: 745f 7572 6c29 05da 0473 656c 6672 0400  t_url)...selfr..
-00000140: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
-00000150: 00a9 0072 0900 0000 fa56 2f77 6f6f 6470  ...r.....V/woodp
-00000160: 6563 6b65 722f 7372 632f 636f 6465 6265  ecker/src/codebe
-00000170: 7267 2e6f 7267 2f62 6f76 696e 652f 626f  rg.org/bovine/bo
-00000180: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
-00000190: 6e65 2f63 6c69 656e 7473 2f73 6967 6e65  ne/clients/signe
-000001a0: 645f 6874 7470 5f63 6c69 656e 742e 7079  d_http_client.py
-000001b0: da08 5f5f 696e 6974 5f5f 0500 0000 7308  ..__init__....s.
-000001c0: 0000 0006 0106 0106 010a 017a 1953 6967  ...........z.Sig
-000001d0: 6e65 6448 7474 7043 6c69 656e 742e 5f5f  nedHttpClient.__
-000001e0: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
-000001f0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-00000200: 0a00 0000 7c01 7c00 5f00 7c00 5300 7203  ....|.|._.|.S.r.
-00000210: 0000 0029 0172 0400 0000 2902 7208 0000  ...).r....).r...
-00000220: 0072 0400 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000230: 720a 0000 00da 0b73 6574 5f73 6573 7369  r......set_sessi
-00000240: 6f6e 0b00 0000 7304 0000 0006 0104 027a  on....s........z
-00000250: 1c53 6967 6e65 6448 7474 7043 6c69 656e  .SignedHttpClien
-00000260: 742e 7365 745f 7365 7373 696f 6e63 0300  t.set_sessionc..
-00000270: 0000 0000 0000 0000 0000 0300 0000 0700  ................
-00000280: 0000 c300 0000 7324 0000 0081 0174 006a  ......s$.....t.j
-00000290: 016a 02a0 037c 006a 047c 006a 057c 006a  .j...|.j.|.j.|.j
-000002a0: 067c 017c 02a1 0549 0064 0048 0053 0072  .|.|...I.d.H.S.r
-000002b0: 0300 0000 2907 da06 626f 7669 6e65 da07  ....)...bovine..
-000002c0: 636c 6965 6e74 73da 0b73 6967 6e65 645f  clients..signed_
-000002d0: 6874 7470 5a0a 7369 676e 6564 5f67 6574  httpZ.signed_get
-000002e0: 7204 0000 0072 0500 0000 7206 0000 0029  r....r....r....)
-000002f0: 0372 0800 0000 da03 7572 6cda 0768 6561  .r......url..hea
-00000300: 6465 7273 7209 0000 0072 0900 0000 720a  dersr....r....r.
-00000310: 0000 00da 0367 6574 1000 0000 7308 0000  .....get....s...
-00000320: 0002 8008 0110 010a ff7a 1453 6967 6e65  .........z.Signe
-00000330: 6448 7474 7043 6c69 656e 742e 6765 7463  dHttpClient.getc
-00000340: 0500 0000 0000 0000 0000 0000 0500 0000  ................
-00000350: 0900 0000 c300 0000 732a 0000 0081 0174  ........s*.....t
-00000360: 006a 016a 026a 037c 006a 047c 006a 057c  .j.j.j.|.j.|.j.|
-00000370: 006a 067c 017c 027c 037c 0464 018d 0749  .j.|.|.|.|.d...I
-00000380: 0064 0048 0053 0029 024e 2901 da0c 636f  .d.H.S.).N)...co
-00000390: 6e74 656e 745f 7479 7065 2907 720d 0000  ntent_type).r...
-000003a0: 0072 0e00 0000 720f 0000 005a 0b73 6967  .r....r....Z.sig
-000003b0: 6e65 645f 706f 7374 7204 0000 0072 0500  ned_postr....r..
-000003c0: 0000 7206 0000 0029 0572 0800 0000 7210  ..r....).r....r.
-000003d0: 0000 00da 0462 6f64 7972 1100 0000 7213  .....bodyr....r.
-000003e0: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
-000003f0: 0000 da04 706f 7374 1500 0000 7314 0000  ....post....s...
-00000400: 0002 8008 0104 0104 0104 0102 0102 0102  ................
-00000410: 0102 010c f97a 1553 6967 6e65 6448 7474  .....z.SignedHtt
-00000420: 7043 6c69 656e 742e 706f 7374 6302 0000  pClient.postc...
-00000430: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00000440: 0043 0000 0073 1a00 0000 7400 6a01 6a02  .C...s....t.j.j.
-00000450: a003 7c00 6a04 7c00 6a05 7c00 6a06 7c01  ..|.j.|.j.|.j.|.
-00000460: a104 5300 7203 0000 0029 0772 0d00 0000  ..S.r....).r....
-00000470: 720e 0000 0072 0f00 0000 5a13 7369 676e  r....r....Z.sign
-00000480: 6564 5f65 7665 6e74 5f73 6f75 7263 6572  ed_event_sourcer
-00000490: 0400 0000 7205 0000 0072 0600 0000 2902  ....r....r....).
-000004a0: 7208 0000 0072 1000 0000 7209 0000 0072  r....r....r....r
-000004b0: 0900 0000 720a 0000 00da 0c65 7665 6e74  ....r......event
-000004c0: 5f73 6f75 7263 6520 0000 0073 0600 0000  _source ...s....
-000004d0: 0801 0e01 04ff 7a1d 5369 676e 6564 4874  ......z.SignedHt
-000004e0: 7470 436c 6965 6e74 2e65 7665 6e74 5f73  tpClient.event_s
-000004f0: 6f75 7263 6572 0300 0000 2908 da08 5f5f  ourcer....)...__
-00000500: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000510: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000520: 720b 0000 0072 0c00 0000 7212 0000 0072  r....r....r....r
-00000530: 1500 0000 7216 0000 0072 0900 0000 7209  ....r....r....r.
-00000540: 0000 0072 0900 0000 720a 0000 0072 0200  ...r....r....r..
-00000550: 0000 0400 0000 730c 0000 0008 000a 0108  ......s.........
-00000560: 060c 050e 050c 0b72 0200 0000 2903 5a1a  .......r....).Z.
-00000570: 626f 7669 6e65 2e63 6c69 656e 7473 2e73  bovine.clients.s
-00000580: 6967 6e65 645f 6874 7470 720d 0000 0072  igned_httpr....r
-00000590: 0200 0000 7209 0000 0072 0900 0000 7209  ....r....r....r.
-000005a0: 0000 0072 0a00 0000 da08 3c6d 6f64 756c  ...r......<modul
-000005b0: 653e 0100 0000 7304 0000 0008 0012 03    e>....s........
+00000060: 0003 0000 0040 0000 0073 4400 0000 6500  .....@...sD...e.
+00000070: 5a01 6400 5a02 6401 5a03 640d 6403 6404  Z.d.Z.d.Z.d.d.d.
+00000080: 8401 5a04 6405 6406 8400 5a05 6900 6601  ..Z.d.d...Z.i.f.
+00000090: 6407 6408 8401 5a06 6900 6402 6602 6409  d.d...Z.i.d.f.d.
+000000a0: 640a 8401 5a07 640b 640c 8400 5a08 6402  d...Z.d.d...Z.d.
+000000b0: 5300 290e da10 5369 676e 6564 4874 7470  S.)...SignedHttp
+000000c0: 436c 6965 6e74 7a20 436c 6965 6e74 2066  Clientz Client f
+000000d0: 6f72 2075 7369 6e67 2048 5454 5020 5369  or using HTTP Si
+000000e0: 676e 6174 7572 6573 4e63 0500 0000 0000  gnaturesNc......
+000000f0: 0000 0000 0000 0500 0000 0200 0000 4300  ..............C.
+00000100: 0000 731c 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
+00000110: 005f 017c 037c 005f 027c 047c 005f 0364  ._.|.|._.|.|._.d
+00000120: 0053 00a9 014e 2904 da07 7365 7373 696f  .S...N)...sessio
+00000130: 6eda 0e70 7562 6c69 635f 6b65 795f 7572  n..public_key_ur
+00000140: 6cda 0b70 7269 7661 7465 5f6b 6579 da0b  l..private_key..
+00000150: 6163 636f 756e 745f 7572 6c29 05da 0473  account_url)...s
+00000160: 656c 6672 0400 0000 7205 0000 0072 0600  elfr....r....r..
+00000170: 0000 7207 0000 00a9 0072 0900 0000 fa4f  ..r......r.....O
+00000180: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
+00000190: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
+000001a0: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
+000001b0: 652f 626f 7669 6e65 2f63 6c69 656e 7473  e/bovine/clients
+000001c0: 2f73 6967 6e65 645f 6874 7470 2e70 79da  /signed_http.py.
+000001d0: 085f 5f69 6e69 745f 5f07 0000 0073 0800  .__init__....s..
+000001e0: 0000 0601 0601 0601 0a01 7a19 5369 676e  ..........z.Sign
+000001f0: 6564 4874 7470 436c 6965 6e74 2e5f 5f69  edHttpClient.__i
+00000200: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
+00000210: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000220: 0000 007c 017c 005f 007c 0053 0072 0300  ...|.|._.|.S.r..
+00000230: 0000 2901 7204 0000 0029 0272 0800 0000  ..).r....).r....
+00000240: 7204 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
+00000250: 0a00 0000 da0b 7365 745f 7365 7373 696f  ......set_sessio
+00000260: 6e0d 0000 0073 0400 0000 0601 0402 7a1c  n....s........z.
+00000270: 5369 676e 6564 4874 7470 436c 6965 6e74  SignedHttpClient
+00000280: 2e73 6574 5f73 6573 7369 6f6e 6303 0000  .set_sessionc...
+00000290: 0000 0000 0000 0000 0003 0000 0007 0000  ................
+000002a0: 00c3 0000 0073 2400 0000 8101 7400 6a01  .....s$.....t.j.
+000002b0: 6a02 a003 7c00 6a04 7c00 6a05 7c00 6a06  j...|.j.|.j.|.j.
+000002c0: 7c01 7c02 a105 4900 6400 4800 5300 7203  |.|...I.d.H.S.r.
+000002d0: 0000 0029 07da 0662 6f76 696e 65da 0763  ...)...bovine..c
+000002e0: 6c69 656e 7473 da13 7369 676e 6564 5f68  lients..signed_h
+000002f0: 7474 705f 6d65 7468 6f64 735a 0a73 6967  ttp_methodsZ.sig
+00000300: 6e65 645f 6765 7472 0400 0000 7205 0000  ned_getr....r...
+00000310: 0072 0600 0000 2903 7208 0000 00da 0375  .r....).r......u
+00000320: 726c da07 6865 6164 6572 7372 0900 0000  rl..headersr....
+00000330: 7209 0000 0072 0a00 0000 da03 6765 7412  r....r......get.
+00000340: 0000 0073 0800 0000 0280 0801 1001 0aff  ...s............
+00000350: 7a14 5369 676e 6564 4874 7470 436c 6965  z.SignedHttpClie
+00000360: 6e74 2e67 6574 6305 0000 0000 0000 0000  nt.getc.........
+00000370: 0000 0005 0000 0009 0000 00c3 0000 0073  ...............s
+00000380: 2a00 0000 8101 7400 6a01 6a02 6a03 7c00  *.....t.j.j.j.|.
+00000390: 6a04 7c00 6a05 7c00 6a06 7c01 7c02 7c03  j.|.j.|.j.|.|.|.
+000003a0: 7c04 6401 8d07 4900 6400 4800 5300 2902  |.d...I.d.H.S.).
+000003b0: 4e29 01da 0c63 6f6e 7465 6e74 5f74 7970  N)...content_typ
+000003c0: 6529 0772 0d00 0000 720e 0000 0072 0f00  e).r....r....r..
+000003d0: 0000 5a0b 7369 676e 6564 5f70 6f73 7472  ..Z.signed_postr
+000003e0: 0400 0000 7205 0000 0072 0600 0000 2905  ....r....r....).
+000003f0: 7208 0000 0072 1000 0000 da04 626f 6479  r....r......body
+00000400: 7211 0000 0072 1300 0000 7209 0000 0072  r....r....r....r
+00000410: 0900 0000 720a 0000 00da 0470 6f73 7417  ....r......post.
+00000420: 0000 0073 1400 0000 0280 0801 0401 0401  ...s............
+00000430: 0401 0201 0201 0201 0201 0cf9 7a15 5369  ............z.Si
+00000440: 676e 6564 4874 7470 436c 6965 6e74 2e70  gnedHttpClient.p
+00000450: 6f73 7463 0200 0000 0000 0000 0000 0000  ostc............
+00000460: 0200 0000 0600 0000 4300 0000 731a 0000  ........C...s...
+00000470: 0074 006a 016a 02a0 037c 006a 047c 006a  .t.j.j...|.j.|.j
+00000480: 057c 006a 067c 01a1 0453 0072 0300 0000  .|.j.|...S.r....
+00000490: 2907 720d 0000 0072 0e00 0000 720f 0000  ).r....r....r...
+000004a0: 005a 1373 6967 6e65 645f 6576 656e 745f  .Z.signed_event_
+000004b0: 736f 7572 6365 7204 0000 0072 0500 0000  sourcer....r....
+000004c0: 7206 0000 0029 0272 0800 0000 7210 0000  r....).r....r...
+000004d0: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+000004e0: da0c 6576 656e 745f 736f 7572 6365 2200  ..event_source".
+000004f0: 0000 7306 0000 0008 010e 0104 ff7a 1d53  ..s..........z.S
+00000500: 6967 6e65 6448 7474 7043 6c69 656e 742e  ignedHttpClient.
+00000510: 6576 656e 745f 736f 7572 6365 7203 0000  event_sourcer...
+00000520: 0029 09da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
+00000530: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000540: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000550: 720b 0000 0072 0c00 0000 7212 0000 0072  r....r....r....r
+00000560: 1500 0000 7216 0000 0072 0900 0000 7209  ....r....r....r.
+00000570: 0000 0072 0900 0000 720a 0000 0072 0200  ...r....r....r..
+00000580: 0000 0400 0000 730e 0000 0008 0004 010a  ......s.........
+00000590: 0208 060c 050e 050c 0b72 0200 0000 2903  .........r....).
+000005a0: 5a22 626f 7669 6e65 2e63 6c69 656e 7473  Z"bovine.clients
+000005b0: 2e73 6967 6e65 645f 6874 7470 5f6d 6574  .signed_http_met
+000005c0: 686f 6473 720d 0000 0072 0200 0000 7209  hodsr....r....r.
+000005d0: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+000005e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000005f0: 7304 0000 0008 0012 03                   s........
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 3f01 0000  o.........Ad?...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 3f01 0000  o.......*.Nd?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 8400 5a09 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0e66 6574 6368 5f6e  .....)...fetch_n
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1145 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 7904 0000  o.........Ady...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 8104 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a09  Z.m.Z...d.d.l.Z.
 00000060: 6400 6403 6c0a 6d0b 5a0b 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6405 6406  l.m.Z.m.Z...d.d.
@@ -120,12 +120,13 @@
 00000770: 7469 6f6e da07 7265 7772 6974 6572 1b00  tion..rewriter..
 00000780: 0000 da0d 756e 6974 7465 7374 2e6d 6f63  ....unittest.moc
 00000790: 6b72 0200 0000 7203 0000 0072 1700 0000  kr....r....r....
 000007a0: 5a1f 626f 7669 6e65 2e63 7279 7074 6f2e  Z.bovine.crypto.
 000007b0: 7369 676e 6174 7572 655f 6368 6563 6b65  signature_checke
 000007c0: 7272 0400 0000 da12 626f 7669 6e65 2e63  rr......bovine.c
 000007d0: 7279 7074 6f2e 7465 7374 7205 0000 0072  rypto.testr....r
-000007e0: 0600 0000 da0b 7369 676e 6564 5f68 7474  ......signed_htt
-000007f0: 7072 0800 0000 7236 0000 0072 3400 0000  pr....r6...r4...
-00000800: 7234 0000 0072 3400 0000 7235 0000 00da  r4...r4...r5....
-00000810: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
-00000820: 0000 2a00 0802 0c02 1001 0c02 0c03       ..*...........
+000007e0: 0600 0000 da13 7369 676e 6564 5f68 7474  ......signed_htt
+000007f0: 705f 6d65 7468 6f64 7372 0800 0000 7236  p_methodsr....r6
+00000800: 0000 0072 3400 0000 7234 0000 0072 3400  ...r4...r4...r4.
+00000810: 0000 7235 0000 00da 083c 6d6f 6475 6c65  ..r5.....<module
+00000820: 3e01 0000 0073 0c00 0000 2a00 0802 0c02  >....s....*.....
+00000830: 1001 0c02 0c03                           ......
```

### Comparing `bovine-0.1.2/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 529 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 1102 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0a02 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a08 6400 6403  Z...d.d.l.Z.d.d.
 00000060: 6c09 6d0a 5a0a 0100 6404 6405 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6406 6407 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
@@ -40,13 +40,12 @@
 00000270: 5f62 7569 6c74 696e 73da 195f 7079 7465  _builtins.._pyte
 00000280: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
 00000290: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
 000002a0: 0772 6577 7269 7465 da0a 4070 7974 6573  .rewrite..@pytes
 000002b0: 745f 6172 da0d 756e 6974 7465 7374 2e6d  t_ar..unittest.m
 000002c0: 6f63 6b72 0200 0000 7207 0000 00da 1262  ockr....r......b
 000002d0: 6f76 696e 652e 6372 7970 746f 2e74 6573  ovine.crypto.tes
-000002e0: 7472 0300 0000 da12 7369 676e 6564 5f68  tr......signed_h
-000002f0: 7474 705f 636c 6965 6e74 7205 0000 0072  ttp_clientr....r
-00000300: 1000 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
-00000310: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000320: 653e 0100 0000 730a 0000 0026 0008 020c  e>....s....&....
-00000330: 020c 020c 03                             .....
+000002e0: 7472 0300 0000 da0b 7369 676e 6564 5f68  tr......signed_h
+000002f0: 7474 7072 0500 0000 7210 0000 0072 0e00  ttpr....r....r..
+00000300: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000310: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000320: 0a00 0000 2600 0802 0c02 0c02 0c03       ....&.........
```

### Comparing `bovine-0.1.2/bovine/clients/lookup_account.py` & `bovine-0.1.3/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/clients/moo_auth_client.py` & `bovine-0.1.3/bovine/clients/moo_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,46 +3,43 @@
 from bovine.crypto.helper import content_digest_sha256
 from bovine.crypto.http_signature import build_signature
 from bovine.utils.date import get_gmt_now
 
 from .consts import BOVINE_CLIENT_NAME
 from .event_source import EventSource
 
-# from bovine.utils.crypto.did_key import private_key_to_ed25519
-
 
 def host_target_from_url(url):
     parsed_url = urlparse(url)
     return parsed_url.netloc, parsed_url.path
 
 
 class MooAuthClient:
+    """Client for using Moo-Auth-1 authentication"""
+
     def __init__(self, session, did_key, private_key):
         self.session = session
         self.did_key = did_key
         self.private_key = private_key
-        # self.private_key = private_key_to_ed25519(private_key)
 
     async def get(self, url, headers={}):
         host, target = host_target_from_url(url)
 
         accept = "application/activity+json"
-        content_type = "application/activity+json"
         date_header = get_gmt_now()
 
         signature_header = (
             build_signature(host, "get", target)
             .with_field("date", date_header)
             .ed25519_sign(self.private_key)
         )
 
         headers["accept"] = accept
         headers["date"] = date_header
         headers["host"] = host
-        headers["content-type"] = content_type
         headers["authorization"] = f"Moo-Auth-1 {self.did_key}"
         headers["x-moo-signature"] = signature_header
         headers["user-agent"] = BOVINE_CLIENT_NAME
 
         return await self.session.get(url, headers=headers)
 
     async def post(self, url, body, headers={}, content_type=None):
```

### Comparing `bovine-0.1.2/bovine/clients/nodeinfo.py` & `bovine-0.1.3/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/clients/signed_http.py` & `bovine-0.1.3/bovine/clients/signed_http_methods.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/clients/signed_http_client.py` & `bovine-0.1.3/bovine/clients/signed_http.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-import bovine.clients.signed_http
+import bovine.clients.signed_http_methods
 
 
 class SignedHttpClient:
+    """Client for using HTTP Signatures"""
+
     def __init__(self, session, public_key_url, private_key, account_url=None):
         self.session = session
         self.public_key_url = public_key_url
         self.private_key = private_key
         self.account_url = account_url
 
     def set_session(self, session):
         self.session = session
 
         return self
 
     async def get(self, url, headers={}):
-        return await bovine.clients.signed_http.signed_get(
+        return await bovine.clients.signed_http_methods.signed_get(
             self.session, self.public_key_url, self.private_key, url, headers
         )
 
     async def post(self, url, body, headers={}, content_type=None):
-        return await bovine.clients.signed_http.signed_post(
+        return await bovine.clients.signed_http_methods.signed_post(
             self.session,
             self.public_key_url,
             self.private_key,
             url,
             body,
             headers,
             content_type=content_type,
         )
 
     def event_source(self, url):
-        return bovine.clients.signed_http.signed_event_source(
+        return bovine.clients.signed_http_methods.signed_event_source(
             self.session, self.public_key_url, self.private_key, url
         )
```

### Comparing `bovine-0.1.2/bovine/clients/test_event_source.py` & `bovine-0.1.3/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/clients/test_signed_http.py` & `bovine-0.1.3/bovine/clients/test_signed_http.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest.mock import AsyncMock, MagicMock
 
 import aiohttp
 
 from bovine.crypto.signature_checker import SignatureChecker
 from bovine.crypto.test import private_key, public_key
 
-from .signed_http import signed_get
+from .signed_http_methods import signed_get
 
 
 async def test_signed_get():
     url = "https://test_domain/test_path"
     public_key_url = "public_key_url"
     session = AsyncMock(aiohttp.ClientSession)
     session.get = AsyncMock()
```

### Comparing `bovine-0.1.2/bovine/clients/test_signed_http_client.py` & `bovine-0.1.3/bovine/clients/test_signed_http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest.mock import AsyncMock
 
 import aiohttp
 
 from bovine.crypto.test import private_key
 
-from .signed_http_client import SignedHttpClient
+from .signed_http import SignedHttpClient
 
 
 async def test_activity_pub_client_get():
     session = AsyncMock(aiohttp.ClientSession)
     url = "https://test_domain/test_path"
     public_key_url = "public_key_url"
     session = AsyncMock(aiohttp.ClientSession)
```

### Comparing `bovine-0.1.2/bovine/crypto/__init__.py` & `bovine-0.1.3/bovine/crypto/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,24 +67,28 @@
     :param key_retriever:
         A function that returns the public key of the actor"""
 
     signature_checker = SignatureChecker(key_retriever)
     return signature_checker.validate_signature
 
 
-async def validate_moo_auth_signature(request, domain) -> Optional[str]:
+async def validate_moo_auth_signature(
+    request, domain
+) -> Tuple[Optional[str], Optional[str]]:
     """Validates the `Moo-Auth-1 <https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation>`_ signature of the request.
     Returns the did-key if the signature is valid.
 
     :param request:
         The request to validate the signature for.
     :param domain:
         The domain the request is made to.
 
-    :returns: On success the did key, on failure None
+    :returns:
+        On success the did key and domain, on failure None, None
+        When no domain is passed the did key and None is returned
     """  # noqa: E501
     didkey = request.headers["authorization"][11:]
     signature = request.headers["x-moo-signature"]
 
     dt = bovine.utils.date.parse_gmt(request.headers["date"])
     assert domain == request.headers["host"]
     assert bovine.utils.date.check_max_offset_now(dt)
@@ -96,19 +100,19 @@
             .with_field("host", request.headers["host"])
             .with_field("date", request.headers["date"])
         )
     else:
         raw_data = await request.get_data()
         digest = content_digest_sha256(raw_data)
         if digest != request.headers["digest"]:
-            return
+            return None, None
         http_signature = (
             HttpSignature()
             .with_field("(request-target)", "post " + request.path)
             .with_field("host", request.headers["host"])
             .with_field("date", request.headers["date"])
             .with_field("digest", request.headers["digest"])
         )
 
     if http_signature.ed25519_verify(didkey, signature):
-        return didkey
-    return None
+        return didkey, None
+    return None, None
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 3999 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,228 +1,235 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 9f0f 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 2d10 0000  o.......*.Nd-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0b 6406 6407 6c0c 6d0d 5a0d 6d0e 5a0e  Z.d.d.l.m.Z.m.Z.
 00000080: 6d0f 5a0f 0100 6406 6408 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
 00000090: 0100 6406 6409 6c12 6d13 5a13 0100 640a  ..d.d.l.m.Z...d.
 000000a0: 6514 6602 640b 640c 8404 5a15 640d 6514  e.f.d.d...Z.d.e.
 000000b0: 640a 6514 6604 640e 640f 8404 5a16 640a  d.e.f.d.d...Z.d.
 000000c0: 6502 6514 6514 6602 1900 6602 6410 6411  e.e.e.f...f.d.d.
-000000d0: 8404 5a17 6412 6413 8400 5a18 640a 6501  ..Z.d.d...Z.d.e.
-000000e0: 6514 1900 6602 6414 6415 8404 5a19 6405  e...f.d.d...Z.d.
-000000f0: 5300 2916 e900 0000 0029 02da 084f 7074  S.)......)...Opt
-00000100: 696f 6e61 6cda 0554 7570 6c65 2901 da0d  ional..Tuple)...
-00000110: 7365 7269 616c 697a 6174 696f 6e29 02da  serialization)..
-00000120: 0765 6432 3535 3139 da03 7273 6129 02da  .ed25519..rsa)..
-00000130: 096d 756c 7469 6261 7365 da0a 6d75 6c74  .multibase..mult
-00000140: 6963 6f64 6563 4ee9 0100 0000 2903 da15  icodecN.....)...
-00000150: 636f 6e74 656e 745f 6469 6765 7374 5f73  content_digest_s
-00000160: 6861 3235 36da 1670 7269 7661 7465 5f6b  ha256..private_k
-00000170: 6579 5f74 6f5f 6564 3235 3531 39da 1570  ey_to_ed25519..p
-00000180: 7562 6c69 635f 6b65 795f 746f 5f64 6964  ublic_key_to_did
-00000190: 5f6b 6579 2901 da0d 4874 7470 5369 676e  _key)...HttpSign
-000001a0: 6174 7572 6529 01da 1053 6967 6e61 7475  ature)...Signatu
-000001b0: 7265 4368 6563 6b65 72da 0672 6574 7572  reChecker..retur
-000001c0: 6e63 0000 0000 0000 0000 0000 0000 0300  nc..............
-000001d0: 0000 0500 0000 4300 0000 733e 0000 0074  ......C...s>...t
-000001e0: 006a 01a0 02a1 007d 007c 006a 0374 046a  .j.....}.|.j.t.j
-000001f0: 056a 0674 046a 076a 0674 04a0 08a1 0064  .j.t.j.j.t.....d
-00000200: 018d 037d 0174 09a0 0a64 027c 01a1 027d  ...}.t...d.|...}
-00000210: 0274 0ba0 0c7c 0264 03a1 0253 0029 047a  .t...|.d...S.).z
-00000220: 3a52 6574 7572 6e73 2061 206d 756c 7469  :Returns a multi
-00000230: 636f 6465 632f 6d75 6c74 6962 6173 6520  codec/multibase 
-00000240: 656e 636f 6465 6420 6564 3235 3531 3920  encoded ed25519 
-00000250: 7072 6976 6174 6520 6b65 79a9 03da 0865  private key....e
-00000260: 6e63 6f64 696e 67da 0666 6f72 6d61 745a  ncoding..formatZ
-00000270: 1465 6e63 7279 7074 696f 6e5f 616c 676f  .encryption_algo
-00000280: 7269 7468 6d7a 0c65 6432 3535 3139 2d70  rithmz.ed25519-p
-00000290: 7269 765a 0962 6173 6535 3862 7463 290d  rivZ.base58btc).
-000002a0: 7205 0000 005a 1145 6432 3535 3139 5072  r....Z.Ed25519Pr
-000002b0: 6976 6174 654b 6579 5a08 6765 6e65 7261  ivateKeyZ.genera
-000002c0: 7465 da0d 7072 6976 6174 655f 6279 7465  te..private_byte
-000002d0: 7372 0400 0000 da08 456e 636f 6469 6e67  sr......Encoding
-000002e0: 5a03 5261 77da 0d50 7269 7661 7465 466f  Z.Raw..PrivateFo
-000002f0: 726d 6174 da0c 4e6f 456e 6372 7970 7469  rmat..NoEncrypti
-00000300: 6f6e 7208 0000 00da 0477 7261 7072 0700  onr......wrapr..
-00000310: 0000 da06 656e 636f 6465 2903 da0b 7072  ....encode)...pr
-00000320: 6976 6174 655f 6b65 7972 1300 0000 da07  ivate_keyr......
-00000330: 7772 6170 7065 64a9 0072 1b00 0000 fa4b  wrapped..r.....K
-00000340: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
-00000350: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
-00000360: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
-00000370: 652f 626f 7669 6e65 2f63 7279 7074 6f2f  e/bovine/crypto/
-00000380: 5f5f 696e 6974 5f5f 2e70 79da 1c67 656e  __init__.py..gen
-00000390: 6572 6174 655f 6564 3235 3531 395f 7072  erate_ed25519_pr
-000003a0: 6976 6174 655f 6b65 790e 0000 0073 1000  ivate_key....s..
-000003b0: 0000 0a02 0402 0601 0601 0601 06fd 0c06  ................
-000003c0: 0c02 721d 0000 00da 0f70 7269 7661 7465  ..r......private
-000003d0: 5f6b 6579 5f73 7472 6301 0000 0000 0000  _key_strc.......
-000003e0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000003f0: 0073 1400 0000 7400 7c00 8301 7d01 7401  .s....t.|...}.t.
-00000400: 7c01 a002 a100 8301 5300 2901 7a9e 436f  |.......S.).z.Co
-00000410: 6d70 7574 6573 2070 7562 6c69 6320 6b65  mputes public ke
-00000420: 7920 696e 2064 6964 206b 6579 2066 6f72  y in did key for
-00000430: 6d20 6f66 2045 6432 3535 3139 2070 7269  m of Ed25519 pri
-00000440: 7661 7465 206b 6579 0a0a 2020 2020 3a70  vate key..    :p
-00000450: 6172 616d 2070 7269 7661 7465 5f6b 6579  aram private_key
-00000460: 5f73 7472 3a20 6d75 6c74 6962 6173 652f  _str: multibase/
-00000470: 6d75 6c74 6963 6f64 6563 2065 6e63 6f64  multicodec encod
-00000480: 6564 2045 6432 3535 3139 2070 7269 7661  ed Ed25519 priva
-00000490: 7465 206b 6579 0a0a 2020 2020 3a72 6574  te key..    :ret
-000004a0: 7572 6e3a 2064 6964 3a6b 6579 2903 720b  urn: did:key).r.
-000004b0: 0000 0072 0c00 0000 da0a 7075 626c 6963  ...r......public
-000004c0: 5f6b 6579 2902 721e 0000 0072 1900 0000  _key).r....r....
-000004d0: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-000004e0: 1670 7269 7661 7465 5f6b 6579 5f74 6f5f  .private_key_to_
-000004f0: 6469 645f 6b65 791d 0000 0073 0400 0000  did_key....s....
-00000500: 0807 0c02 7220 0000 0063 0000 0000 0000  ....r ...c......
-00000510: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-00000520: 0000 735c 0000 0074 006a 0164 0164 0264  ..s\...t.j.d.d.d
-00000530: 038d 027d 007c 006a 0274 036a 046a 0574  ...}.|.j.t.j.j.t
-00000540: 036a 066a 0774 03a0 08a1 0064 048d 037d  .j.j.t.....d...}
-00000550: 017c 00a0 09a1 007d 027c 026a 0a74 036a  .|.....}.|.j.t.j
-00000560: 046a 0574 036a 0b6a 0c64 058d 027d 037c  .j.t.j.j.d...}.|
-00000570: 03a0 0d64 06a1 017c 01a0 0d64 06a1 0166  ...d...|...d...f
-00000580: 0253 0029 077a 6b47 656e 6572 6174 6573  .S.).zkGenerates
-00000590: 2061 206e 6577 2070 6169 7220 6f66 2052   a new pair of R
-000005a0: 5341 2070 7562 6c69 6320 616e 6420 7072  SA public and pr
-000005b0: 6976 6174 6520 6b65 7973 2e0a 0a20 2020  ivate keys...   
-000005c0: 203a 7265 7475 726e 733a 2070 656d 2065   :returns: pem e
-000005d0: 6e63 6f64 6564 2070 7562 6c69 6320 616e  ncoded public an
-000005e0: 6420 7072 6976 6174 6520 6b65 790a 2020  d private key.  
-000005f0: 2020 6901 0001 0069 0008 0000 2902 5a0f    i....i....).Z.
-00000600: 7075 626c 6963 5f65 7870 6f6e 656e 745a  public_exponentZ
-00000610: 086b 6579 5f73 697a 6572 1000 0000 2902  .key_sizer....).
-00000620: 7211 0000 0072 1200 0000 7a05 7574 662d  r....r....z.utf-
-00000630: 3829 0e72 0600 0000 5a14 6765 6e65 7261  8).r....Z.genera
-00000640: 7465 5f70 7269 7661 7465 5f6b 6579 7213  te_private_keyr.
-00000650: 0000 0072 0400 0000 7214 0000 005a 0350  ...r....r....Z.P
-00000660: 454d 7215 0000 005a 0550 4b43 5338 7216  EMr....Z.PKCS8r.
-00000670: 0000 0072 1f00 0000 da0c 7075 626c 6963  ...r......public
-00000680: 5f62 7974 6573 5a0c 5075 626c 6963 466f  _bytesZ.PublicFo
-00000690: 726d 6174 5a14 5375 626a 6563 7450 7562  rmatZ.SubjectPub
-000006a0: 6c69 634b 6579 496e 666f da06 6465 636f  licKeyInfo..deco
-000006b0: 6465 2904 7219 0000 005a 0f70 7269 7661  de).r....Z.priva
-000006c0: 7465 5f6b 6579 5f70 656d 721f 0000 005a  te_key_pemr....Z
-000006d0: 0e70 7562 6c69 635f 6b65 795f 7065 6d72  .public_key_pemr
-000006e0: 1b00 0000 721b 0000 0072 1c00 0000 da1f  ....r....r......
-000006f0: 6765 6e65 7261 7465 5f72 7361 5f70 7562  generate_rsa_pub
-00000700: 6c69 635f 7072 6976 6174 655f 6b65 7929  lic_private_key)
-00000710: 0000 0073 1800 0000 0e06 0401 0601 0601  ...s............
-00000720: 0601 06fd 0806 0401 0601 0601 06fe 1405  ................
-00000730: 7223 0000 0063 0100 0000 0000 0000 0000  r#...c..........
-00000740: 0000 0200 0000 0200 0000 4300 0000 730e  ..........C...s.
-00000750: 0000 0074 007c 0083 017d 017c 016a 0153  ...t.|...}.|.j.S
-00000760: 0029 017a f243 7265 6174 6573 2061 2076  .).z.Creates a v
-00000770: 616c 6964 6174 655f 7369 676e 6174 7572  alidate_signatur
-00000780: 6520 6675 6e63 7469 6f6e 2e20 7661 6c69  e function. vali
-00000790: 6461 7465 5f73 6967 6e61 7475 7265 2074  date_signature t
-000007a0: 616b 6573 2074 6865 2072 6571 7565 7374  akes the request
-000007b0: 0a20 2020 2061 7320 7061 7261 6d65 7465  .    as paramete
-000007c0: 7220 616e 6420 7265 7475 726e 7320 7468  r and returns th
-000007d0: 6520 7075 626c 6963 206b 6579 2075 726c  e public key url
-000007e0: 2069 6620 7468 6520 6874 7470 2073 6967   if the http sig
-000007f0: 6e61 7475 7265 2069 7320 7661 6c69 642e  nature is valid.
-00000800: 0a0a 2020 2020 3a70 6172 616d 206b 6579  ..    :param key
-00000810: 5f72 6574 7269 6576 6572 3a0a 2020 2020  _retriever:.    
-00000820: 2020 2020 4120 6675 6e63 7469 6f6e 2074      A function t
-00000830: 6861 7420 7265 7475 726e 7320 7468 6520  hat returns the 
-00000840: 7075 626c 6963 206b 6579 206f 6620 7468  public key of th
-00000850: 6520 6163 746f 7229 0272 0e00 0000 5a12  e actor).r....Z.
-00000860: 7661 6c69 6461 7465 5f73 6967 6e61 7475  validate_signatu
-00000870: 7265 2902 5a0d 6b65 795f 7265 7472 6965  re).Z.key_retrie
-00000880: 7665 72da 1173 6967 6e61 7475 7265 5f63  ver..signature_c
-00000890: 6865 636b 6572 721b 0000 0072 1b00 0000  heckerr....r....
-000008a0: 721c 0000 00da 1d62 7569 6c64 5f76 616c  r......build_val
-000008b0: 6964 6174 655f 6874 7470 5f73 6967 6e61  idate_http_signa
-000008c0: 7475 7265 3f00 0000 7304 0000 0008 0706  ture?...s.......
-000008d0: 0172 2500 0000 6302 0000 0000 0000 0000  .r%...c.........
-000008e0: 0000 0008 0000 0005 0000 00c3 0000 0073  ...............s
-000008f0: 1001 0000 8101 7c00 6a00 6401 1900 6402  ......|.j.d...d.
-00000900: 6403 8502 1900 7d02 7c00 6a00 6404 1900  d.....}.|.j.d...
-00000910: 7d03 7401 6a02 6a03 a004 7c00 6a00 6405  }.t.j.j...|.j.d.
-00000920: 1900 a101 7d04 7c01 7c00 6a00 6406 1900  ....}.|.|.j.d...
-00000930: 6b02 7322 4a00 8201 7401 6a02 6a03 a005  k.s"J...t.j.j...
-00000940: 7c04 a101 732b 4a00 8201 7c00 6a06 a007  |...s+J...|.j...
-00000950: a100 6407 6b02 724b 7408 8300 a009 6408  ..d.k.rKt.....d.
-00000960: 6409 7c00 6a0a 1700 a102 a009 6406 7c00  d.|.j.......d.|.
-00000970: 6a00 6406 1900 a102 a009 6405 7c00 6a00  j.d.......d.|.j.
-00000980: 6405 1900 a102 7d05 6e33 7c00 a00b a100  d.....}.n3|.....
-00000990: 4900 6403 4800 7d06 740c 7c06 8301 7d07  I.d.H.}.t.|...}.
-000009a0: 7c07 7c00 6a00 640a 1900 6b03 725f 6403  |.|.j.d...k.r_d.
-000009b0: 5300 7408 8300 a009 6408 640b 7c00 6a0a  S.t.....d.d.|.j.
-000009c0: 1700 a102 a009 6406 7c00 6a00 6406 1900  ......d.|.j.d...
-000009d0: a102 a009 6405 7c00 6a00 6405 1900 a102  ....d.|.j.d.....
-000009e0: a009 640a 7c00 6a00 640a 1900 a102 7d05  ..d.|.j.d.....}.
-000009f0: 7c05 a00d 7c02 7c03 a102 7286 7c02 5300  |...|.|...r.|.S.
-00000a00: 6403 5300 290c 617a 0100 0056 616c 6964  d.S.).az...Valid
-00000a10: 6174 6573 2074 6865 2060 4d6f 6f2d 4175  ates the `Moo-Au
-00000a20: 7468 2d31 203c 6874 7470 733a 2f2f 626c  th-1 <https://bl
-00000a30: 6f67 2e6d 796d 6174 682e 726f 636b 732f  og.mymath.rocks/
-00000a40: 3230 3233 2d30 332d 3135 2f42 494e 315f  2023-03-15/BIN1_
-00000a50: 4d6f 6f5f 4175 7468 656e 7469 6361 7469  Moo_Authenticati
-00000a60: 6f6e 5f61 6e64 5f41 7574 686f 7269 6174  on_and_Authoriat
-00000a70: 696f 6e3e 605f 2073 6967 6e61 7475 7265  ion>`_ signature
-00000a80: 206f 6620 7468 6520 7265 7175 6573 742e   of the request.
-00000a90: 0a20 2020 2052 6574 7572 6e73 2074 6865  .    Returns the
-00000aa0: 2064 6964 2d6b 6579 2069 6620 7468 6520   did-key if the 
-00000ab0: 7369 676e 6174 7572 6520 6973 2076 616c  signature is val
-00000ac0: 6964 2e0a 0a20 2020 203a 7061 7261 6d20  id...    :param 
-00000ad0: 7265 7175 6573 743a 0a20 2020 2020 2020  request:.       
-00000ae0: 2054 6865 2072 6571 7565 7374 2074 6f20   The request to 
-00000af0: 7661 6c69 6461 7465 2074 6865 2073 6967  validate the sig
-00000b00: 6e61 7475 7265 2066 6f72 2e0a 2020 2020  nature for..    
-00000b10: 3a70 6172 616d 2064 6f6d 6169 6e3a 0a20  :param domain:. 
-00000b20: 2020 2020 2020 2054 6865 2064 6f6d 6169         The domai
-00000b30: 6e20 7468 6520 7265 7175 6573 7420 6973  n the request is
-00000b40: 206d 6164 6520 746f 2e0a 0a20 2020 203a   made to...    :
-00000b50: 7265 7475 726e 733a 204f 6e20 7375 6363  returns: On succ
-00000b60: 6573 7320 7468 6520 6469 6420 6b65 792c  ess the did key,
-00000b70: 206f 6e20 6661 696c 7572 6520 4e6f 6e65   on failure None
-00000b80: 0a20 2020 20da 0d61 7574 686f 7269 7a61  .    ..authoriza
-00000b90: 7469 6f6e e90b 0000 004e 7a0f 782d 6d6f  tion.....Nz.x-mo
-00000ba0: 6f2d 7369 676e 6174 7572 65da 0464 6174  o-signature..dat
-00000bb0: 65da 0468 6f73 74da 0367 6574 7a10 2872  e..host..getz.(r
-00000bc0: 6571 7565 7374 2d74 6172 6765 7429 7a04  equest-target)z.
-00000bd0: 6765 7420 da06 6469 6765 7374 7a05 706f  get ..digestz.po
-00000be0: 7374 2029 0eda 0768 6561 6465 7273 da06  st )...headers..
-00000bf0: 626f 7669 6e65 da05 7574 696c 7372 2800  bovine..utilsr(.
-00000c00: 0000 5a09 7061 7273 655f 676d 745a 1463  ..Z.parse_gmtZ.c
-00000c10: 6865 636b 5f6d 6178 5f6f 6666 7365 745f  heck_max_offset_
-00000c20: 6e6f 77da 066d 6574 686f 64da 056c 6f77  now..method..low
-00000c30: 6572 720d 0000 00da 0a77 6974 685f 6669  err......with_fi
-00000c40: 656c 64da 0470 6174 68da 0867 6574 5f64  eld..path..get_d
-00000c50: 6174 6172 0a00 0000 5a0e 6564 3235 3531  atar....Z.ed2551
-00000c60: 395f 7665 7269 6679 2908 da07 7265 7175  9_verify)...requ
-00000c70: 6573 74da 0664 6f6d 6169 6e5a 0664 6964  est..domainZ.did
-00000c80: 6b65 79da 0973 6967 6e61 7475 7265 da02  key..signature..
-00000c90: 6474 da0e 6874 7470 5f73 6967 6e61 7475  dt..http_signatu
-00000ca0: 7265 da08 7261 775f 6461 7461 722b 0000  re..raw_datar+..
-00000cb0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000cc0: da1b 7661 6c69 6461 7465 5f6d 6f6f 5f61  ..validate_moo_a
-00000cd0: 7574 685f 7369 676e 6174 7572 654a 0000  uth_signatureJ..
-00000ce0: 0073 3200 0000 0280 120b 0a01 1402 1201  .s2.............
-00000cf0: 1201 0e02 0402 0e01 0e01 0e01 04fc 0e07  ................
-00000d00: 0801 0e01 0401 0402 0e01 0e01 0e01 0e01  ................
-00000d10: 02fb 0c08 0401 0401 723a 0000 0029 1ada  ........r:...)..
-00000d20: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-00000d30: 005a 1e63 7279 7074 6f67 7261 7068 792e  .Z.cryptography.
-00000d40: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
-00000d50: 7372 0400 0000 5a29 6372 7970 746f 6772  sr....Z)cryptogr
-00000d60: 6170 6879 2e68 617a 6d61 742e 7072 696d  aphy.hazmat.prim
-00000d70: 6974 6976 6573 2e61 7379 6d6d 6574 7269  itives.asymmetri
-00000d80: 6372 0500 0000 7206 0000 005a 0c6d 756c  cr....r....Z.mul
-00000d90: 7469 666f 726d 6174 7372 0700 0000 7208  tiformatsr....r.
-00000da0: 0000 0072 2d00 0000 da06 6865 6c70 6572  ...r-.....helper
-00000db0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000dc0: 3800 0000 720d 0000 0072 2400 0000 720e  8...r....r$...r.
-00000dd0: 0000 00da 0373 7472 721d 0000 0072 2000  .....strr....r .
-00000de0: 0000 7223 0000 0072 2500 0000 723a 0000  ..r#...r%...r:..
-00000df0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
-00000e00: 721c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000e10: 0000 0073 1a00 0000 1000 0c02 1001 1001  ...s............
-00000e20: 0802 1402 0c01 0c01 0e03 120f 160c 0816  ................
-00000e30: 160b                                     ..
+000000d0: 8404 5a17 6412 6413 8400 5a18 640a 6502  ..Z.d.d...Z.d.e.
+000000e0: 6501 6514 1900 6501 6514 1900 6602 1900  e.e...e.e...f...
+000000f0: 6602 6414 6415 8404 5a19 6405 5300 2916  f.d.d...Z.d.S.).
+00000100: e900 0000 0029 02da 084f 7074 696f 6e61  .....)...Optiona
+00000110: 6cda 0554 7570 6c65 2901 da0d 7365 7269  l..Tuple)...seri
+00000120: 616c 697a 6174 696f 6e29 02da 0765 6432  alization)...ed2
+00000130: 3535 3139 da03 7273 6129 02da 096d 756c  5519..rsa)...mul
+00000140: 7469 6261 7365 da0a 6d75 6c74 6963 6f64  tibase..multicod
+00000150: 6563 4ee9 0100 0000 2903 da15 636f 6e74  ecN.....)...cont
+00000160: 656e 745f 6469 6765 7374 5f73 6861 3235  ent_digest_sha25
+00000170: 36da 1670 7269 7661 7465 5f6b 6579 5f74  6..private_key_t
+00000180: 6f5f 6564 3235 3531 39da 1570 7562 6c69  o_ed25519..publi
+00000190: 635f 6b65 795f 746f 5f64 6964 5f6b 6579  c_key_to_did_key
+000001a0: 2901 da0d 4874 7470 5369 676e 6174 7572  )...HttpSignatur
+000001b0: 6529 01da 1053 6967 6e61 7475 7265 4368  e)...SignatureCh
+000001c0: 6563 6b65 72da 0672 6574 7572 6e63 0000  ecker..returnc..
+000001d0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+000001e0: 0000 4300 0000 733e 0000 0074 006a 01a0  ..C...s>...t.j..
+000001f0: 02a1 007d 007c 006a 0374 046a 056a 0674  ...}.|.j.t.j.j.t
+00000200: 046a 076a 0674 04a0 08a1 0064 018d 037d  .j.j.t.....d...}
+00000210: 0174 09a0 0a64 027c 01a1 027d 0274 0ba0  .t...d.|...}.t..
+00000220: 0c7c 0264 03a1 0253 0029 047a 3a52 6574  .|.d...S.).z:Ret
+00000230: 7572 6e73 2061 206d 756c 7469 636f 6465  urns a multicode
+00000240: 632f 6d75 6c74 6962 6173 6520 656e 636f  c/multibase enco
+00000250: 6465 6420 6564 3235 3531 3920 7072 6976  ded ed25519 priv
+00000260: 6174 6520 6b65 79a9 03da 0865 6e63 6f64  ate key....encod
+00000270: 696e 67da 0666 6f72 6d61 745a 1465 6e63  ing..formatZ.enc
+00000280: 7279 7074 696f 6e5f 616c 676f 7269 7468  ryption_algorith
+00000290: 6d7a 0c65 6432 3535 3139 2d70 7269 765a  mz.ed25519-privZ
+000002a0: 0962 6173 6535 3862 7463 290d 7205 0000  .base58btc).r...
+000002b0: 005a 1145 6432 3535 3139 5072 6976 6174  .Z.Ed25519Privat
+000002c0: 654b 6579 5a08 6765 6e65 7261 7465 da0d  eKeyZ.generate..
+000002d0: 7072 6976 6174 655f 6279 7465 7372 0400  private_bytesr..
+000002e0: 0000 da08 456e 636f 6469 6e67 5a03 5261  ....EncodingZ.Ra
+000002f0: 77da 0d50 7269 7661 7465 466f 726d 6174  w..PrivateFormat
+00000300: da0c 4e6f 456e 6372 7970 7469 6f6e 7208  ..NoEncryptionr.
+00000310: 0000 00da 0477 7261 7072 0700 0000 da06  .....wrapr......
+00000320: 656e 636f 6465 2903 da0b 7072 6976 6174  encode)...privat
+00000330: 655f 6b65 7972 1300 0000 da07 7772 6170  e_keyr......wrap
+00000340: 7065 64a9 0072 1b00 0000 fa4b 2f77 6f6f  ped..r.....K/woo
+00000350: 6470 6563 6b65 722f 7372 632f 636f 6465  dpecker/src/code
+00000360: 6265 7267 2e6f 7267 2f62 6f76 696e 652f  berg.org/bovine/
+00000370: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+00000380: 7669 6e65 2f63 7279 7074 6f2f 5f5f 696e  vine/crypto/__in
+00000390: 6974 5f5f 2e70 79da 1c67 656e 6572 6174  it__.py..generat
+000003a0: 655f 6564 3235 3531 395f 7072 6976 6174  e_ed25519_privat
+000003b0: 655f 6b65 790e 0000 0073 1000 0000 0a02  e_key....s......
+000003c0: 0402 0601 0601 0601 06fd 0c06 0c02 721d  ..............r.
+000003d0: 0000 00da 0f70 7269 7661 7465 5f6b 6579  .....private_key
+000003e0: 5f73 7472 6301 0000 0000 0000 0000 0000  _strc...........
+000003f0: 0002 0000 0003 0000 0043 0000 0073 1400  .........C...s..
+00000400: 0000 7400 7c00 8301 7d01 7401 7c01 a002  ..t.|...}.t.|...
+00000410: a100 8301 5300 2901 7a9e 436f 6d70 7574  ....S.).z.Comput
+00000420: 6573 2070 7562 6c69 6320 6b65 7920 696e  es public key in
+00000430: 2064 6964 206b 6579 2066 6f72 6d20 6f66   did key form of
+00000440: 2045 6432 3535 3139 2070 7269 7661 7465   Ed25519 private
+00000450: 206b 6579 0a0a 2020 2020 3a70 6172 616d   key..    :param
+00000460: 2070 7269 7661 7465 5f6b 6579 5f73 7472   private_key_str
+00000470: 3a20 6d75 6c74 6962 6173 652f 6d75 6c74  : multibase/mult
+00000480: 6963 6f64 6563 2065 6e63 6f64 6564 2045  icodec encoded E
+00000490: 6432 3535 3139 2070 7269 7661 7465 206b  d25519 private k
+000004a0: 6579 0a0a 2020 2020 3a72 6574 7572 6e3a  ey..    :return:
+000004b0: 2064 6964 3a6b 6579 2903 720b 0000 0072   did:key).r....r
+000004c0: 0c00 0000 da0a 7075 626c 6963 5f6b 6579  ......public_key
+000004d0: 2902 721e 0000 0072 1900 0000 721b 0000  ).r....r....r...
+000004e0: 0072 1b00 0000 721c 0000 00da 1670 7269  .r....r......pri
+000004f0: 7661 7465 5f6b 6579 5f74 6f5f 6469 645f  vate_key_to_did_
+00000500: 6b65 791d 0000 0073 0400 0000 0807 0c02  key....s........
+00000510: 7220 0000 0063 0000 0000 0000 0000 0000  r ...c..........
+00000520: 0000 0400 0000 0500 0000 4300 0000 735c  ..........C...s\
+00000530: 0000 0074 006a 0164 0164 0264 038d 027d  ...t.j.d.d.d...}
+00000540: 007c 006a 0274 036a 046a 0574 036a 066a  .|.j.t.j.j.t.j.j
+00000550: 0774 03a0 08a1 0064 048d 037d 017c 00a0  .t.....d...}.|..
+00000560: 09a1 007d 027c 026a 0a74 036a 046a 0574  ...}.|.j.t.j.j.t
+00000570: 036a 0b6a 0c64 058d 027d 037c 03a0 0d64  .j.j.d...}.|...d
+00000580: 06a1 017c 01a0 0d64 06a1 0166 0253 0029  ...|...d...f.S.)
+00000590: 077a 6b47 656e 6572 6174 6573 2061 206e  .zkGenerates a n
+000005a0: 6577 2070 6169 7220 6f66 2052 5341 2070  ew pair of RSA p
+000005b0: 7562 6c69 6320 616e 6420 7072 6976 6174  ublic and privat
+000005c0: 6520 6b65 7973 2e0a 0a20 2020 203a 7265  e keys...    :re
+000005d0: 7475 726e 733a 2070 656d 2065 6e63 6f64  turns: pem encod
+000005e0: 6564 2070 7562 6c69 6320 616e 6420 7072  ed public and pr
+000005f0: 6976 6174 6520 6b65 790a 2020 2020 6901  ivate key.    i.
+00000600: 0001 0069 0008 0000 2902 5a0f 7075 626c  ...i....).Z.publ
+00000610: 6963 5f65 7870 6f6e 656e 745a 086b 6579  ic_exponentZ.key
+00000620: 5f73 697a 6572 1000 0000 2902 7211 0000  _sizer....).r...
+00000630: 0072 1200 0000 7a05 7574 662d 3829 0e72  .r....z.utf-8).r
+00000640: 0600 0000 5a14 6765 6e65 7261 7465 5f70  ....Z.generate_p
+00000650: 7269 7661 7465 5f6b 6579 7213 0000 0072  rivate_keyr....r
+00000660: 0400 0000 7214 0000 005a 0350 454d 7215  ....r....Z.PEMr.
+00000670: 0000 005a 0550 4b43 5338 7216 0000 0072  ...Z.PKCS8r....r
+00000680: 1f00 0000 da0c 7075 626c 6963 5f62 7974  ......public_byt
+00000690: 6573 5a0c 5075 626c 6963 466f 726d 6174  esZ.PublicFormat
+000006a0: 5a14 5375 626a 6563 7450 7562 6c69 634b  Z.SubjectPublicK
+000006b0: 6579 496e 666f da06 6465 636f 6465 2904  eyInfo..decode).
+000006c0: 7219 0000 005a 0f70 7269 7661 7465 5f6b  r....Z.private_k
+000006d0: 6579 5f70 656d 721f 0000 005a 0e70 7562  ey_pemr....Z.pub
+000006e0: 6c69 635f 6b65 795f 7065 6d72 1b00 0000  lic_key_pemr....
+000006f0: 721b 0000 0072 1c00 0000 da1f 6765 6e65  r....r......gene
+00000700: 7261 7465 5f72 7361 5f70 7562 6c69 635f  rate_rsa_public_
+00000710: 7072 6976 6174 655f 6b65 7929 0000 0073  private_key)...s
+00000720: 1800 0000 0e06 0401 0601 0601 0601 06fd  ................
+00000730: 0806 0401 0601 0601 06fe 1405 7223 0000  ............r#..
+00000740: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000750: 0000 0200 0000 4300 0000 730e 0000 0074  ......C...s....t
+00000760: 007c 0083 017d 017c 016a 0153 0029 017a  .|...}.|.j.S.).z
+00000770: f243 7265 6174 6573 2061 2076 616c 6964  .Creates a valid
+00000780: 6174 655f 7369 676e 6174 7572 6520 6675  ate_signature fu
+00000790: 6e63 7469 6f6e 2e20 7661 6c69 6461 7465  nction. validate
+000007a0: 5f73 6967 6e61 7475 7265 2074 616b 6573  _signature takes
+000007b0: 2074 6865 2072 6571 7565 7374 0a20 2020   the request.   
+000007c0: 2061 7320 7061 7261 6d65 7465 7220 616e   as parameter an
+000007d0: 6420 7265 7475 726e 7320 7468 6520 7075  d returns the pu
+000007e0: 626c 6963 206b 6579 2075 726c 2069 6620  blic key url if 
+000007f0: 7468 6520 6874 7470 2073 6967 6e61 7475  the http signatu
+00000800: 7265 2069 7320 7661 6c69 642e 0a0a 2020  re is valid...  
+00000810: 2020 3a70 6172 616d 206b 6579 5f72 6574    :param key_ret
+00000820: 7269 6576 6572 3a0a 2020 2020 2020 2020  riever:.        
+00000830: 4120 6675 6e63 7469 6f6e 2074 6861 7420  A function that 
+00000840: 7265 7475 726e 7320 7468 6520 7075 626c  returns the publ
+00000850: 6963 206b 6579 206f 6620 7468 6520 6163  ic key of the ac
+00000860: 746f 7229 0272 0e00 0000 5a12 7661 6c69  tor).r....Z.vali
+00000870: 6461 7465 5f73 6967 6e61 7475 7265 2902  date_signature).
+00000880: 5a0d 6b65 795f 7265 7472 6965 7665 72da  Z.key_retriever.
+00000890: 1173 6967 6e61 7475 7265 5f63 6865 636b  .signature_check
+000008a0: 6572 721b 0000 0072 1b00 0000 721c 0000  err....r....r...
+000008b0: 00da 1d62 7569 6c64 5f76 616c 6964 6174  ...build_validat
+000008c0: 655f 6874 7470 5f73 6967 6e61 7475 7265  e_http_signature
+000008d0: 3f00 0000 7304 0000 0008 0706 0172 2500  ?...s........r%.
+000008e0: 0000 6302 0000 0000 0000 0000 0000 0008  ..c.............
+000008f0: 0000 0005 0000 00c3 0000 0073 1401 0000  ...........s....
+00000900: 8101 7c00 6a00 6401 1900 6402 6403 8502  ..|.j.d...d.d...
+00000910: 1900 7d02 7c00 6a00 6404 1900 7d03 7401  ..}.|.j.d...}.t.
+00000920: 6a02 6a03 a004 7c00 6a00 6405 1900 a101  j.j...|.j.d.....
+00000930: 7d04 7c01 7c00 6a00 6406 1900 6b02 7322  }.|.|.j.d...k.s"
+00000940: 4a00 8201 7401 6a02 6a03 a005 7c04 a101  J...t.j.j...|...
+00000950: 732b 4a00 8201 7c00 6a06 a007 a100 6407  s+J...|.j.....d.
+00000960: 6b02 724b 7408 8300 a009 6408 6409 7c00  k.rKt.....d.d.|.
+00000970: 6a0a 1700 a102 a009 6406 7c00 6a00 6406  j.......d.|.j.d.
+00000980: 1900 a102 a009 6405 7c00 6a00 6405 1900  ......d.|.j.d...
+00000990: a102 7d05 6e33 7c00 a00b a100 4900 6403  ..}.n3|.....I.d.
+000009a0: 4800 7d06 740c 7c06 8301 7d07 7c07 7c00  H.}.t.|...}.|.|.
+000009b0: 6a00 640a 1900 6b03 725f 640b 5300 7408  j.d...k.r_d.S.t.
+000009c0: 8300 a009 6408 640c 7c00 6a0a 1700 a102  ....d.d.|.j.....
+000009d0: a009 6406 7c00 6a00 6406 1900 a102 a009  ..d.|.j.d.......
+000009e0: 6405 7c00 6a00 6405 1900 a102 a009 640a  d.|.j.d.......d.
+000009f0: 7c00 6a00 640a 1900 a102 7d05 7c05 a00d  |.j.d.....}.|...
+00000a00: 7c02 7c03 a102 7288 7c02 6403 6602 5300  |.|...r.|.d.f.S.
+00000a10: 640b 5300 290d 61d5 0100 0056 616c 6964  d.S.).a....Valid
+00000a20: 6174 6573 2074 6865 2060 4d6f 6f2d 4175  ates the `Moo-Au
+00000a30: 7468 2d31 203c 6874 7470 733a 2f2f 626c  th-1 <https://bl
+00000a40: 6f67 2e6d 796d 6174 682e 726f 636b 732f  og.mymath.rocks/
+00000a50: 3230 3233 2d30 332d 3135 2f42 494e 315f  2023-03-15/BIN1_
+00000a60: 4d6f 6f5f 4175 7468 656e 7469 6361 7469  Moo_Authenticati
+00000a70: 6f6e 5f61 6e64 5f41 7574 686f 7269 6174  on_and_Authoriat
+00000a80: 696f 6e3e 605f 2073 6967 6e61 7475 7265  ion>`_ signature
+00000a90: 206f 6620 7468 6520 7265 7175 6573 742e   of the request.
+00000aa0: 0a20 2020 2052 6574 7572 6e73 2074 6865  .    Returns the
+00000ab0: 2064 6964 2d6b 6579 2069 6620 7468 6520   did-key if the 
+00000ac0: 7369 676e 6174 7572 6520 6973 2076 616c  signature is val
+00000ad0: 6964 2e0a 0a20 2020 203a 7061 7261 6d20  id...    :param 
+00000ae0: 7265 7175 6573 743a 0a20 2020 2020 2020  request:.       
+00000af0: 2054 6865 2072 6571 7565 7374 2074 6f20   The request to 
+00000b00: 7661 6c69 6461 7465 2074 6865 2073 6967  validate the sig
+00000b10: 6e61 7475 7265 2066 6f72 2e0a 2020 2020  nature for..    
+00000b20: 3a70 6172 616d 2064 6f6d 6169 6e3a 0a20  :param domain:. 
+00000b30: 2020 2020 2020 2054 6865 2064 6f6d 6169         The domai
+00000b40: 6e20 7468 6520 7265 7175 6573 7420 6973  n the request is
+00000b50: 206d 6164 6520 746f 2e0a 0a20 2020 203a   made to...    :
+00000b60: 7265 7475 726e 733a 0a20 2020 2020 2020  returns:.       
+00000b70: 204f 6e20 7375 6363 6573 7320 7468 6520   On success the 
+00000b80: 6469 6420 6b65 7920 616e 6420 646f 6d61  did key and doma
+00000b90: 696e 2c20 6f6e 2066 6169 6c75 7265 204e  in, on failure N
+00000ba0: 6f6e 652c 204e 6f6e 650a 2020 2020 2020  one, None.      
+00000bb0: 2020 5768 656e 206e 6f20 646f 6d61 696e    When no domain
+00000bc0: 2069 7320 7061 7373 6564 2074 6865 2064   is passed the d
+00000bd0: 6964 206b 6579 2061 6e64 204e 6f6e 6520  id key and None 
+00000be0: 6973 2072 6574 7572 6e65 640a 2020 2020  is returned.    
+00000bf0: da0d 6175 7468 6f72 697a 6174 696f 6ee9  ..authorization.
+00000c00: 0b00 0000 4e7a 0f78 2d6d 6f6f 2d73 6967  ....Nz.x-moo-sig
+00000c10: 6e61 7475 7265 da04 6461 7465 da04 686f  nature..date..ho
+00000c20: 7374 da03 6765 747a 1028 7265 7175 6573  st..getz.(reques
+00000c30: 742d 7461 7267 6574 297a 0467 6574 20da  t-target)z.get .
+00000c40: 0664 6967 6573 7429 024e 4e7a 0570 6f73  .digest).NNz.pos
+00000c50: 7420 290e da07 6865 6164 6572 73da 0662  t )...headers..b
+00000c60: 6f76 696e 65da 0575 7469 6c73 7228 0000  ovine..utilsr(..
+00000c70: 00da 0970 6172 7365 5f67 6d74 da14 6368  ...parse_gmt..ch
+00000c80: 6563 6b5f 6d61 785f 6f66 6673 6574 5f6e  eck_max_offset_n
+00000c90: 6f77 da06 6d65 7468 6f64 da05 6c6f 7765  ow..method..lowe
+00000ca0: 7272 0d00 0000 da0a 7769 7468 5f66 6965  rr......with_fie
+00000cb0: 6c64 da04 7061 7468 da08 6765 745f 6461  ld..path..get_da
+00000cc0: 7461 720a 0000 005a 0e65 6432 3535 3139  tar....Z.ed25519
+00000cd0: 5f76 6572 6966 7929 08da 0772 6571 7565  _verify)...reque
+00000ce0: 7374 da06 646f 6d61 696e 5a06 6469 646b  st..domainZ.didk
+00000cf0: 6579 da09 7369 676e 6174 7572 65da 0264  ey..signature..d
+00000d00: 74da 0e68 7474 705f 7369 676e 6174 7572  t..http_signatur
+00000d10: 65da 0872 6177 5f64 6174 6172 2b00 0000  e..raw_datar+...
+00000d20: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00000d30: 1b76 616c 6964 6174 655f 6d6f 6f5f 6175  .validate_moo_au
+00000d40: 7468 5f73 6967 6e61 7475 7265 4a00 0000  th_signatureJ...
+00000d50: 7332 0000 0002 8012 0f0a 0114 0212 0112  s2..............
+00000d60: 010e 0204 020e 010e 010e 0104 fc0e 0708  ................
+00000d70: 010e 0104 0104 020e 010e 010e 010e 0102  ................
+00000d80: fb0c 0808 0104 0172 3c00 0000 291a da06  .......r<...)...
+00000d90: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
+00000da0: 5a1e 6372 7970 746f 6772 6170 6879 2e68  Z.cryptography.h
+00000db0: 617a 6d61 742e 7072 696d 6974 6976 6573  azmat.primitives
+00000dc0: 7204 0000 005a 2963 7279 7074 6f67 7261  r....Z)cryptogra
+00000dd0: 7068 792e 6861 7a6d 6174 2e70 7269 6d69  phy.hazmat.primi
+00000de0: 7469 7665 732e 6173 796d 6d65 7472 6963  tives.asymmetric
+00000df0: 7205 0000 0072 0600 0000 5a0c 6d75 6c74  r....r....Z.mult
+00000e00: 6966 6f72 6d61 7473 7207 0000 0072 0800  iformatsr....r..
+00000e10: 0000 722d 0000 00da 0668 656c 7065 7272  ..r-.....helperr
+00000e20: 0a00 0000 720b 0000 0072 0c00 0000 723a  ....r....r....r:
+00000e30: 0000 0072 0d00 0000 7224 0000 0072 0e00  ...r....r$...r..
+00000e40: 0000 da03 7374 7272 1d00 0000 7220 0000  ....strr....r ..
+00000e50: 0072 2300 0000 7225 0000 0072 3c00 0000  .r#...r%...r<...
+00000e60: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00000e70: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000e80: 0000 731e 0000 0010 000c 0210 0110 0108  ..s.............
+00000e90: 0214 020c 010c 010e 0312 0f16 0c08 1602  ................
+00000ea0: 0b12 020e fe                             .....
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/helper.cpython-310.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2664 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 680a 0000  o.........Adh...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 680a 0000  o.......*.Ndh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/http_signature.cpython-310.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/http_signature.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 4008 0000  o.........Ad@...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 4008 0000  o.......*.Nd@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6405  d.l.m.Z.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6500 a00c 650d a101 5a0e 6407 6408  ..e...e...Z.d.d.
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 7e0b 0000  o.........Ad~...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 7e0b 0000  o.......*.Nd~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c04 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6404 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 f204 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 f204 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6500 a001 6502 a101 5a03  d.l.Z.e...e...Z.
 00000040: 4700 6402 6403 8400 6403 8302 5a04 6404  G.d.d...d...Z.d.
 00000050: 6405 8400 5a05 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000060: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
 00000070: 0000 0003 0000 0040 0000 0073 2800 0000  .......@...s(...
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/test.cpython-310.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/test.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 2199 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 9708 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 9708 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5300 2903 61c4 0100  Z.d.Z.d.S.).a...
 00000040: 000a 2d2d 2d2d 2d42 4547 494e 2050 5542  ..-----BEGIN PUB
 00000050: 4c49 4320 4b45 592d 2d2d 2d2d 0a4d 4949  LIC KEY-----.MII
 00000060: 4249 6a41 4e42 676b 7168 6b69 4739 7730  BIjANBgkqhkiG9w0
 00000070: 4241 5145 4641 414f 4341 5138 414d 4949  BAQEFAAOCAQ8AMII
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 4989 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 7d13 0000  o.........Ad}...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 8313 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 6d09 5a09 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  l.m.Z.m.Z.m.Z.m.
 00000070: 5a0e 0100 6403 6405 6c0f 6d10 5a10 0100  Z...d.d.l.m.Z...
@@ -127,238 +127,238 @@
 000007e0: 6d61 7436 721e 0000 0072 1e00 0000 721f  mat6r....r....r.
 000007f0: 0000 00da 1b74 6573 745f 7072 6976 6174  .....test_privat
 00000800: 655f 6b65 795f 746f 5f64 6964 5f6b 6579  e_key_to_did_key
 00000810: 1600 0000 7306 0000 0004 0108 027c 0272  ....s........|.r
 00000820: 2e00 0000 7a26 626f 7669 6e65 2e75 7469  ....z&bovine.uti
 00000830: 6c73 2e64 6174 652e 6368 6563 6b5f 6d61  ls.date.check_ma
 00000840: 785f 6f66 6673 6574 5f6e 6f77 6301 0000  x_offset_nowc...
-00000850: 0000 0000 0000 0000 0007 0000 0008 0000  ................
-00000860: 00c3 0000 0073 ac00 0000 8101 6401 7c00  .....s......d.|.
+00000850: 0000 0000 0000 0000 0008 0000 0008 0000  ................
+00000860: 00c3 0000 0073 b000 0000 8101 6401 7c00  .....s......d.|.
 00000870: 5f00 7401 6402 6403 6404 6405 6406 6407  _.t.d.d.d.d.d.d.
 00000880: 6408 9c04 6409 8d03 7d01 7402 7c01 6405  d...d...}.t.|.d.
-00000890: 8302 4900 6400 4800 7d02 640a 7d03 7c02  ..I.d.H.}.d.}.|.
-000008a0: 7c03 6b02 7d04 7c04 7350 7403 a004 640b  |.k.}.|.sPt...d.
-000008b0: 7c04 6601 640c 7c02 7c03 6602 a104 640d  |.f.d.|.|.f...d.
-000008c0: 7405 a006 a100 7600 7335 7403 a007 7c02  t.....v.s5t...|.
-000008d0: a101 723a 7403 a008 7c02 a101 6e01 640d  ..r:t...|...n.d.
-000008e0: 7403 a008 7c03 a101 640e 9c02 1600 7d05  t...|...d.....}.
-000008f0: 640f 6410 7c05 6901 1600 7d06 7409 7403  d.d.|.i...}.t.t.
-00000900: a00a 7c06 a101 8301 8201 6400 0400 7d04  ..|.......d...}.
-00000910: 7d03 6400 5300 2911 4e54 da03 6765 74fa  }.d.S.).NT..get.
-00000920: 112f 7061 7468 2f74 6f2f 7265 736f 7572  ./path/to/resour
-00000930: 6365 fa1d 5765 642c 2031 3520 4d61 7220  ce..Wed, 15 Mar 
-00000940: 3230 3233 2031 373a 3238 3a31 3520 474d  2023 17:28:15 GM
-00000950: 54fa 0a6d 7968 6f73 742e 746c 64fa 434d  T..myhost.tld.CM
-00000960: 6f6f 2d41 7574 682d 3120 6469 643a 6b65  oo-Auth-1 did:ke
-00000970: 793a 7a36 4d6b 656b 7743 3652 3962 6a39  y:z6MkekwC6R9bj9
-00000980: 4572 546f 4237 4169 5a4a 6679 4353 4468  ErToB7AiZJfyCSDh
-00000990: 615a 6531 5578 6844 6243 714a 7268 7170  aZe1UxhDbCqJrhqp
-000009a0: 5335 5a59 7a35 6168 6448 4362 5039 614a  S5ZYz5ahdHCbP9aJ
-000009b0: 4573 4474 7647 314d 455a 7078 507a 7576  EsDtvG1MEZpxPzuv
-000009c0: 474b 5963 6458 644b 764d 7135 594c 3231  GKYcdXdKvMq5YL21
-000009d0: 5a32 756d 786a 7331 536f 7043 5932 4170  Z2umxjs1SopCY2Ap
-000009e0: 3876 5a78 566a 5445 6636 6459 6247 7542  8vZxVjTEf6dYbGuB
-000009f0: 376d 7467 6367 5579 4e64 424c 6529 04da  7mtgcgUyNdBLe)..
-00000a00: 0464 6174 65da 0468 6f73 74da 0d61 7574  .date..host..aut
-00000a10: 686f 7269 7a61 7469 6f6e fa0f 782d 6d6f  horization..x-mo
-00000a20: 6f2d 7369 676e 6174 7572 6529 03da 066d  o-signature)...m
-00000a30: 6574 686f 64da 0470 6174 68da 0768 6561  ethod..path..hea
-00000a40: 6465 7273 7221 0000 0072 2200 0000 7224  dersr!...r"...r$
-00000a50: 0000 00da 0672 6573 756c 7472 2600 0000  .....resultr&...
-00000a60: 7228 0000 0072 2900 0000 290b da0c 7265  r(...r)...)...re
-00000a70: 7475 726e 5f76 616c 7565 7203 0000 0072  turn_valuer....r
-00000a80: 0900 0000 7214 0000 0072 2a00 0000 7212  ....r....r*...r.
-00000a90: 0000 0072 1300 0000 7215 0000 0072 1600  ...r....r....r..
-00000aa0: 0000 7217 0000 0072 1800 0000 a907 da0b  ..r....r........
-00000ab0: 6d6f 636b 5f6f 6666 7365 74da 0772 6571  mock_offset..req
-00000ac0: 7565 7374 723b 0000 0072 2b00 0000 721a  uestr;...r+...r.
-00000ad0: 0000 0072 2c00 0000 722d 0000 0072 1e00  ...r,...r-...r..
-00000ae0: 0000 721e 0000 0072 1f00 0000 da24 7465  ..r....r.....$te
-00000af0: 7374 5f76 616c 6964 6174 655f 6d6f 6f5f  st_validate_moo_
-00000b00: 6175 7468 5f73 6967 6e61 7475 7265 5f67  auth_signature_g
-00000b10: 6574 1e00 0000 731a 0000 0002 8006 0402  et....s.........
-00000b20: 0202 0102 0102 0202 0102 0102 0104 fc06  ................
-00000b30: fd10 0b7c 0272 4000 0000 6301 0000 0000  ...|.r@...c.....
-00000b40: 0000 0000 0000 0007 0000 0009 0000 00c3  ................
-00000b50: 0000 0073 b600 0000 8101 6401 7c00 5f00  ...s......d.|._.
-00000b60: 7401 6402 6403 6404 6405 6406 6407 6408  t.d.d.d.d.d.d.d.
-00000b70: 6409 9c05 7402 640a 640b 8d01 640c 8d04  d...t.d.d...d...
-00000b80: 7d01 7403 7c01 6405 8302 4900 6400 4800  }.t.|.d...I.d.H.
-00000b90: 7d02 640d 7d03 7c02 7c03 6b02 7d04 7c04  }.d.}.|.|.k.}.|.
-00000ba0: 7355 7404 a005 640e 7c04 6601 640f 7c02  sUt...d.|.f.d.|.
-00000bb0: 7c03 6602 a104 6410 7406 a007 a100 7600  |.f...d.t.....v.
-00000bc0: 733a 7404 a008 7c02 a101 723f 7404 a009  s:t...|...r?t...
-00000bd0: 7c02 a101 6e01 6410 7404 a009 7c03 a101  |...n.d.t...|...
-00000be0: 6411 9c02 1600 7d05 6412 6413 7c05 6901  d.....}.d.d.|.i.
-00000bf0: 1600 7d06 740a 7404 a00b 7c06 a101 8301  ..}.t.t...|.....
-00000c00: 8201 6400 0400 7d04 7d03 6400 5300 2914  ..d...}.}.d.S.).
-00000c10: 4e54 da04 706f 7374 7230 0000 0072 3100  NT..postr0...r1.
-00000c20: 0000 7232 0000 0072 3300 0000 fa34 7368  ..r2...r3....4sh
-00000c30: 612d 3235 363d 4d49 4c62 356c 5544 4436  a-256=MILb5lUDD6
-00000c40: 5a30 7044 5378 6867 786a 2b68 4d42 4577  Z0pDSxhgxj+hMBEw
-00000c50: 3075 547a 5033 6732 7155 4a47 484d 7039  0uTzP3g2qUJGHMp9
-00000c60: 6b3d 5a59 7a34 7650 6b4a 616f 6153 5651  k=ZYz4vPkJaoaSVQ
-00000c70: 7035 4472 4d62 3845 7643 616a 4a63 6572  p5DrMb8EvCajJcer
-00000c80: 5733 3672 7379 5744 454c 5457 5133 6359  W36rsyWDELTWQ3cY
-00000c90: 6d61 6f6e 6e47 6662 3857 4869 7748 3534  maonnGfb8WHiwH54
-00000ca0: 4253 6869 6443 636d 706f 7948 6a61 6e56  BShidCcmpoyHjanV
-00000cb0: 5259 4e72 5858 586b 6134 6a41 6e29 0572  RYNrXXXka4jAn).r
-00000cc0: 3400 0000 7235 0000 0072 3600 0000 da06  4...r5...r6.....
-00000cd0: 6469 6765 7374 7237 0000 00fa 107b 2263  digestr7.....{"c
-00000ce0: 6f77 7322 3a20 2267 6f6f 6422 7da9 0172  ows": "good"}..r
-00000cf0: 3c00 0000 2904 7238 0000 0072 3900 0000  <...).r8...r9...
-00000d00: 723a 0000 00da 0867 6574 5f64 6174 6172  r:.....get_datar
-00000d10: 2100 0000 7222 0000 0072 2400 0000 723b  !...r"...r$...r;
-00000d20: 0000 0072 2600 0000 7228 0000 0072 2900  ...r&...r(...r).
-00000d30: 0000 290c 723c 0000 0072 0300 0000 7202  ..).r<...r....r.
-00000d40: 0000 0072 0900 0000 7214 0000 0072 2a00  ...r....r....r*.
-00000d50: 0000 7212 0000 0072 1300 0000 7215 0000  ..r....r....r...
-00000d60: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000d70: 723d 0000 0072 1e00 0000 721e 0000 0072  r=...r....r....r
-00000d80: 1f00 0000 da25 7465 7374 5f76 616c 6964  .....%test_valid
-00000d90: 6174 655f 6d6f 6f5f 6175 7468 5f73 6967  ate_moo_auth_sig
-00000da0: 6e61 7475 7265 5f70 6f73 7434 0000 0073  nature_post4...s
-00000db0: 1e00 0000 0280 0604 0202 0201 0201 0202  ................
-00000dc0: 0201 0201 0201 0201 04fb 0807 06f6 100d  ................
-00000dd0: 7c02 7247 0000 0063 0100 0000 0000 0000  |.rG...c........
-00000de0: 0000 0000 0600 0000 0800 0000 c300 0000  ................
-00000df0: 736a 0000 0081 0164 0164 0284 007d 0164  sj.....d.d...}.d
-00000e00: 037c 005f 0074 017c 0183 017d 0274 0264  .|._.t.|...}.t.d
-00000e10: 0464 0564 0664 0764 0864 0964 0a9c 0364  .d.d.d.d.d.d...d
-00000e20: 0b8d 047d 037c 027c 0383 0149 0064 0048  ...}.|.|...I.d.H
-00000e30: 007d 047c 0473 3164 0c64 0d74 03a0 047c  .}.|.s1d.d.t...|
-00000e40: 04a1 0169 0116 007d 0574 0574 03a0 067c  ...i...}.t.t...|
-00000e50: 05a1 0183 0182 0164 007d 0464 0053 0029  .......d.}.d.S.)
-00000e60: 0e4e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
-00000e70: 0000 0002 0000 00d3 0000 00f3 0a00 0000  ................
-00000e80: 8101 7400 6401 6602 5300 a902 4eda 056f  ..t.d.f.S...N..o
-00000e90: 776e 6572 720a 0000 00a9 01da 0375 726c  wnerr........url
-00000ea0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-00000eb0: 0d6b 6579 5f72 6574 7269 6576 6572 4e00  .key_retrieverN.
-00000ec0: 0000 f304 0000 0002 8008 017a 3974 6573  ...........z9tes
-00000ed0: 745f 6275 696c 645f 7661 6c69 6461 7465  t_build_validate
-00000ee0: 5f68 7474 705f 7369 676e 6174 7572 652e  _http_signature.
-00000ef0: 3c6c 6f63 616c 733e 2e6b 6579 5f72 6574  <locals>.key_ret
-00000f00: 7269 6576 6572 5472 2f00 0000 7230 0000  rieverTr/...r0..
-00000f10: 00fa 2368 7474 7073 3a2f 2f6d 7968 6f73  ..#https://myhos
-00000f20: 742e 746c 642f 7061 7468 2f74 6f2f 7265  t.tld/path/to/re
-00000f30: 736f 7572 6365 7231 0000 0072 3200 0000  sourcer1...r2...
-00000f40: 61af 0100 006b 6579 4964 3d22 6b65 795f  a....keyId="key_
-00000f50: 6964 222c 616c 676f 7269 7468 6d3d 2272  id",algorithm="r
-00000f60: 7361 2d73 6861 3235 3622 2c68 6561 6465  sa-sha256",heade
-00000f70: 7273 3d22 2872 6571 7565 7374 2d74 6172  rs="(request-tar
-00000f80: 6765 7429 2068 6f73 7420 6461 7465 222c  get) host date",
-00000f90: 7369 676e 6174 7572 653d 2262 7767 4133  signature="bwgA3
-00000fa0: 5561 6a70 447a 4d30 3777 4d2b 4d55 6b70  UajpDzM07wM+MUkp
-00000fb0: 4748 532f 6d41 6868 5475 2b57 4469 424c  GHS/mAhhTu+WDiBL
-00000fc0: 3148 3238 4a37 3632 6a55 5575 6767 7a50  1H28J762jUUuggzP
-00000fd0: 3857 6535 2b49 3057 4879 7053 4243 5774  8We5+I0WHypSBCWt
-00000fe0: 384c 6170 3241 6259 7147 3650 6654 7364  8Lap2AbYqG6PfTsd
-00000ff0: 4645 626b 3856 5765 7758 3334 6e37 2f4c  FEbk8VWewX34n7/L
-00001000: 5553 4d2f 574a 6541 3841 4643 456e 4859  USM/WJeA8AFCEnHY
-00001010: 5064 3872 5269 6234 6430 2b6b 5156 2b55  Pd8rRib4d0+kQV+U
-00001020: 3441 6939 3937 5855 7873 3278 6932 4172  4Ai997XUxs2xi2Ar
-00001030: 754e 646b 4236 534e 4d6b 5362 6e51 4c6f  uNdkB6SNMkSbnQLo
-00001040: 426a 5954 3474 7a47 6166 3249 3178 5a75  BjYT4tzGaf2I1xZu
-00001050: 716a 4431 4876 7657 3078 6131 6f2f 6e50  qjD1HvvW0xa1o/nP
-00001060: 7434 4735 6b6a 3074 566d 6744 7272 6765  t4G5kj0tVmgDrrge
-00001070: 4b4c 3268 554a 3231 5564 4863 5844 4e46  KL2hUJ21UdHcXDNF
-00001080: 7739 514a 5766 2f4f 364b 7945 6d62 756d  w9QJWf/O6KyEmbum
-00001090: 7670 704b 4746 5566 6470 4b53 6833 6e32  vppKGFUfdpKSh3n2
-000010a0: 2f66 5037 4f34 4278 7161 6443 624d 596a  /fP7O4BxqadCbMYj
-000010b0: 306f 4444 4f46 3148 3350 6136 4756 3945  0oDDOF1H3Pa6GV9E
-000010c0: 6649 6553 5858 4c53 3954 6679 5070 6b58  fIeSXXLS9TfyPpkX
-000010d0: 7762 5772 4e70 7a55 425a 5132 6852 477a  wbWrNpzUBZQ2hRGz
-000010e0: 5832 6a53 2f4a 4568 7053 4e53 5671 7636  X2jS/JEhpSNSVqv6
-000010f0: 413d 3d22 2903 7234 0000 0072 3500 0000  A==").r4...r5...
-00001100: da09 7369 676e 6174 7572 6529 0472 3800  ..signature).r8.
-00001110: 0000 7239 0000 0072 4c00 0000 723a 0000  ..r9...rL...r:..
-00001120: 00fa 0e61 7373 6572 7420 2528 7079 3129  ...assert %(py1)
-00001130: 73da 0370 7931 2907 723c 0000 0072 0600  s..py1).r<...r..
-00001140: 0000 7203 0000 0072 1400 0000 7216 0000  ..r....r....r...
-00001150: 0072 1700 0000 7218 0000 00a9 0672 3e00  .r....r......r>.
-00001160: 0000 724d 0000 005a 1776 616c 6964 6174  ..rM...Z.validat
-00001170: 655f 6874 7470 5f73 6967 6e61 7475 7265  e_http_signature
-00001180: 723f 0000 00da 0b40 7079 5f61 7373 6572  r?.....@py_asser
-00001190: 7430 5a0b 4070 795f 666f 726d 6174 3272  t0Z.@py_format2r
-000011a0: 1e00 0000 721e 0000 0072 1f00 0000 da22  ....r....r....."
-000011b0: 7465 7374 5f62 7569 6c64 5f76 616c 6964  test_build_valid
-000011c0: 6174 655f 6874 7470 5f73 6967 6e61 7475  ate_http_signatu
-000011d0: 7265 4c00 0000 731c 0000 0002 8008 0206  reL...s.........
-000011e0: 0308 0202 0202 0102 0102 0102 0202 0102  ................
-000011f0: 0104 fd06 fc3a 0b72 5500 0000 6301 0000  .....:.rU...c...
-00001200: 0000 0000 0000 0000 0006 0000 0009 0000  ................
-00001210: 00c3 0000 0073 7400 0000 8101 6401 6402  .....st.....d.d.
-00001220: 8400 7d01 6403 7c00 5f00 7401 7c01 8301  ..}.d.|._.t.|...
-00001230: 7d02 7402 6404 6405 6406 6407 6408 6409  }.t.d.d.d.d.d.d.
-00001240: 640a 640b 9c04 7403 640c 640d 8d01 640e  d.d...t.d.d...d.
-00001250: 8d05 7d03 7c02 7c03 8301 4900 6400 4800  ..}.|.|...I.d.H.
-00001260: 7d04 7c04 7336 640f 6410 7404 a005 7c04  }.|.s6d.d.t...|.
-00001270: a101 6901 1600 7d05 7406 7404 a007 7c05  ..i...}.t.t...|.
-00001280: a101 8301 8201 6400 7d04 6400 5300 2911  ......d.}.d.S.).
-00001290: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
-000012a0: 0000 0200 0000 d300 0000 7248 0000 0072  ..........rH...r
-000012b0: 4900 0000 720a 0000 0072 4b00 0000 721e  I...r....rK...r.
-000012c0: 0000 0072 1e00 0000 721f 0000 0072 4d00  ...r....r....rM.
-000012d0: 0000 6500 0000 724e 0000 007a 3e74 6573  ..e...rN...z>tes
-000012e0: 745f 6275 696c 645f 7661 6c69 6461 7465  t_build_validate
-000012f0: 5f68 7474 705f 7369 676e 6174 7572 655f  _http_signature_
-00001300: 706f 7374 2e3c 6c6f 6361 6c73 3e2e 6b65  post.<locals>.ke
-00001310: 795f 7265 7472 6965 7665 7254 7241 0000  y_retrieverTrA..
-00001320: 0072 3000 0000 724f 0000 0072 3100 0000  .r0...rO...r1...
-00001330: 7232 0000 0072 4200 0000 61b6 0100 006b  r2...rB...a....k
-00001340: 6579 4964 3d22 6b65 795f 6964 222c 616c  eyId="key_id",al
-00001350: 676f 7269 7468 6d3d 2272 7361 2d73 6861  gorithm="rsa-sha
-00001360: 3235 3622 2c68 6561 6465 7273 3d22 2872  256",headers="(r
-00001370: 6571 7565 7374 2d74 6172 6765 7429 2068  equest-target) h
-00001380: 6f73 7420 6461 7465 2064 6967 6573 7422  ost date digest"
-00001390: 2c73 6967 6e61 7475 7265 3d22 5170 654c  ,signature="QpeL
-000013a0: 4d45 682f 5a30 3039 4467 5963 534f 6b72  MEh/Z009DgYcSOkr
-000013b0: 734b 7239 7a57 3757 7537 5557 5451 3339  sKr9zW7Wu7UWTQ39
-000013c0: 3871 7675 6543 7a61 454c 2f48 7872 7639  8qvueCzaEL/Hxrv9
-000013d0: 4334 3255 2b57 592f 4f33 3478 2f33 3835  C42U+WY/O34x/385
-000013e0: 6c54 2b7a 3149 3342 6b36 714d 5a54 4441  lT+z1I3Bk6qMZTDA
-000013f0: 5a53 6d4b 4759 4235 6c5a 4a56 4264 4332  ZSmKGYB5lZJVBdC2
-00001400: 3061 3444 2b2b 487a 4979 4536 3264 3643  0a4D++HzIyE62d6C
-00001410: 7671 5573 5177 4976 346f 642f 684f 6d6d  vqUsQwIv4od/hOmm
-00001420: 4f51 3348 4b49 3639 4d55 4f73 4e72 4c79  OQ3HKI69MUOsNrLy
-00001430: 6a49 5178 5561 4c53 427a 316d 2f77 6b4c  jIQxUaLSBz1m/wkL
-00001440: 7638 694d 7268 3951 7755 4c6c 7154 4f38  v8iMrh9QwULlqTO8
-00001450: 5748 566a 534a 6c67 5677 6c6c 5274 4f4f  WHVjSJlgVwllRtOO
-00001460: 636d 3377 7a6f 2f63 7232 5879 466a 3467  cm3wzo/cr2XyFj4g
-00001470: 4238 4355 6433 6147 3364 717a 4366 4f4f  B8CUd3aG3dqzCfOO
-00001480: 6f4e 5176 5568 4d44 6c78 5037 5571 426e  oNQvUhMDlxP7UqBn
-00001490: 476f 4636 706e 596e 546e 4a55 5353 4864  GoF6pnYnTnJUSSHd
-000014a0: 6365 5762 4530 3954 7158 4c6d 4148 7a61  ceWbE09TqXLmAHza
-000014b0: 7559 4753 6461 4852 5333 5852 2f53 6a65  uYGSdaHRS3XR/Sje
-000014c0: 3745 5439 5561 4f67 4848 6350 4a48 494e  7ET9UaOgHHcPJHIN
-000014d0: 2b34 6a72 4270 4470 3247 4d36 396a 6f58  +4jrBpDp2GM69joX
-000014e0: 576b 5a77 6845 3047 4f6c 3971 334b 4253  WkZwhE0GOl9q3KBS
-000014f0: 4b41 3d3d 2229 0472 3400 0000 7235 0000  KA==").r4...r5..
-00001500: 0072 4300 0000 7250 0000 0072 4400 0000  .rC...rP...rD...
-00001510: 7245 0000 0029 0572 3800 0000 7239 0000  rE...).r8...r9..
-00001520: 0072 4c00 0000 723a 0000 0072 4600 0000  .rL...r:...rF...
-00001530: 7251 0000 0072 5200 0000 2908 723c 0000  rQ...rR...).r<..
-00001540: 0072 0600 0000 7203 0000 0072 0200 0000  .r....r....r....
-00001550: 7214 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00001560: 1800 0000 7253 0000 0072 1e00 0000 721e  ....rS...r....r.
-00001570: 0000 0072 1f00 0000 da27 7465 7374 5f62  ...r.....'test_b
-00001580: 7569 6c64 5f76 616c 6964 6174 655f 6874  uild_validate_ht
-00001590: 7470 5f73 6967 6e61 7475 7265 5f70 6f73  tp_signature_pos
-000015a0: 7463 0000 0073 2000 0000 0280 0802 0603  tc...s .........
-000015b0: 0802 0202 0201 0201 0201 0202 0201 0201  ................
-000015c0: 0201 04fc 0806 06f6 3a0d 7256 0000 0029  ........:.rV...)
-000015d0: 17da 0862 7569 6c74 696e 7372 1200 0000  ...builtinsr....
-000015e0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-000015f0: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-00001600: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-00001610: 1400 0000 da0d 756e 6974 7465 7374 2e6d  ......unittest.m
-00001620: 6f63 6b72 0200 0000 7203 0000 0072 0400  ockr....r....r..
-00001630: 0000 da00 7206 0000 0072 0700 0000 7208  ....r....r....r.
-00001640: 0000 0072 0900 0000 da04 7465 7374 720b  ...r......testr.
-00001650: 0000 0072 2000 0000 722e 0000 0072 4000  ...r ...r....r@.
-00001660: 0000 7247 0000 0072 5500 0000 7256 0000  ..rG...rU...rV..
-00001670: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
-00001680: 721f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00001690: 0000 0073 1a00 0000 2e00 1802 0c06 0803  ...s............
-000016a0: 080a 0608 0a01 0615 0a01 0617 0a01 0616  ................
-000016b0: 0e01                                     ..
+00000890: 8302 4900 6400 4800 5c02 7d02 7d03 640a  ..I.d.H.\.}.}.d.
+000008a0: 7d04 7c02 7c04 6b02 7d05 7c05 7352 7403  }.|.|.k.}.|.sRt.
+000008b0: a004 640b 7c05 6601 640c 7c02 7c04 6602  ..d.|.f.d.|.|.f.
+000008c0: a104 640d 7405 a006 a100 7600 7337 7403  ..d.t.....v.s7t.
+000008d0: a007 7c02 a101 723c 7403 a008 7c02 a101  ..|...r<t...|...
+000008e0: 6e01 640d 7403 a008 7c04 a101 640e 9c02  n.d.t...|...d...
+000008f0: 1600 7d06 640f 6410 7c06 6901 1600 7d07  ..}.d.d.|.i...}.
+00000900: 7409 7403 a00a 7c07 a101 8301 8201 6400  t.t...|.......d.
+00000910: 0400 7d05 7d04 6400 5300 2911 4e54 da03  ..}.}.d.S.).NT..
+00000920: 6765 74fa 112f 7061 7468 2f74 6f2f 7265  get../path/to/re
+00000930: 736f 7572 6365 fa1d 5765 642c 2031 3520  source..Wed, 15 
+00000940: 4d61 7220 3230 3233 2031 373a 3238 3a31  Mar 2023 17:28:1
+00000950: 3520 474d 54fa 0a6d 7968 6f73 742e 746c  5 GMT..myhost.tl
+00000960: 64fa 434d 6f6f 2d41 7574 682d 3120 6469  d.CMoo-Auth-1 di
+00000970: 643a 6b65 793a 7a36 4d6b 656b 7743 3652  d:key:z6MkekwC6R
+00000980: 3962 6a39 4572 546f 4237 4169 5a4a 6679  9bj9ErToB7AiZJfy
+00000990: 4353 4468 615a 6531 5578 6844 6243 714a  CSDhaZe1UxhDbCqJ
+000009a0: 7268 7170 5335 5a59 7a35 6168 6448 4362  rhqpS5ZYz5ahdHCb
+000009b0: 5039 614a 4573 4474 7647 314d 455a 7078  P9aJEsDtvG1MEZpx
+000009c0: 507a 7576 474b 5963 6458 644b 764d 7135  PzuvGKYcdXdKvMq5
+000009d0: 594c 3231 5a32 756d 786a 7331 536f 7043  YL21Z2umxjs1SopC
+000009e0: 5932 4170 3876 5a78 566a 5445 6636 6459  Y2Ap8vZxVjTEf6dY
+000009f0: 6247 7542 376d 7467 6367 5579 4e64 424c  bGuB7mtgcgUyNdBL
+00000a00: 6529 04da 0464 6174 65da 0468 6f73 74da  e)...date..host.
+00000a10: 0d61 7574 686f 7269 7a61 7469 6f6e fa0f  .authorization..
+00000a20: 782d 6d6f 6f2d 7369 676e 6174 7572 6529  x-moo-signature)
+00000a30: 03da 066d 6574 686f 64da 0470 6174 68da  ...method..path.
+00000a40: 0768 6561 6465 7273 7221 0000 0072 2200  .headersr!...r".
+00000a50: 0000 7224 0000 00da 0672 6573 756c 7472  ..r$.....resultr
+00000a60: 2600 0000 7228 0000 0072 2900 0000 290b  &...r(...r)...).
+00000a70: da0c 7265 7475 726e 5f76 616c 7565 7203  ..return_valuer.
+00000a80: 0000 0072 0900 0000 7214 0000 0072 2a00  ...r....r....r*.
+00000a90: 0000 7212 0000 0072 1300 0000 7215 0000  ..r....r....r...
+00000aa0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000ab0: a908 da0b 6d6f 636b 5f6f 6666 7365 74da  ....mock_offset.
+00000ac0: 0772 6571 7565 7374 723b 0000 00da 015f  .requestr;....._
+00000ad0: 722b 0000 0072 1a00 0000 722c 0000 0072  r+...r....r,...r
+00000ae0: 2d00 0000 721e 0000 0072 1e00 0000 721f  -...r....r....r.
+00000af0: 0000 00da 2474 6573 745f 7661 6c69 6461  ....$test_valida
+00000b00: 7465 5f6d 6f6f 5f61 7574 685f 7369 676e  te_moo_auth_sign
+00000b10: 6174 7572 655f 6765 741e 0000 0073 1a00  ature_get....s..
+00000b20: 0000 0280 0604 0202 0201 0201 0202 0201  ................
+00000b30: 0201 0201 04fc 06fd 140b 7c02 7241 0000  ..........|.rA..
+00000b40: 0063 0100 0000 0000 0000 0000 0000 0800  .c..............
+00000b50: 0000 0900 0000 c300 0000 73ba 0000 0081  ..........s.....
+00000b60: 0164 017c 005f 0074 0164 0264 0364 0464  .d.|._.t.d.d.d.d
+00000b70: 0564 0664 0764 0864 099c 0574 0264 0a64  .d.d.d.d...t.d.d
+00000b80: 0b8d 0164 0c8d 047d 0174 037c 0164 0583  ...d...}.t.|.d..
+00000b90: 0249 0064 0048 005c 027d 027d 0364 0d7d  .I.d.H.\.}.}.d.}
+00000ba0: 047c 027c 046b 027d 057c 0573 5774 04a0  .|.|.k.}.|.sWt..
+00000bb0: 0564 0e7c 0566 0164 0f7c 027c 0466 02a1  .d.|.f.d.|.|.f..
+00000bc0: 0464 1074 06a0 07a1 0076 0073 3c74 04a0  .d.t.....v.s<t..
+00000bd0: 087c 02a1 0172 4174 04a0 097c 02a1 016e  .|...rAt...|...n
+00000be0: 0164 1074 04a0 097c 04a1 0164 119c 0216  .d.t...|...d....
+00000bf0: 007d 0664 1264 137c 0669 0116 007d 0774  .}.d.d.|.i...}.t
+00000c00: 0a74 04a0 0b7c 07a1 0183 0182 0164 0004  .t...|.......d..
+00000c10: 007d 057d 0464 0053 0029 144e 54da 0470  .}.}.d.S.).NT..p
+00000c20: 6f73 7472 3000 0000 7231 0000 0072 3200  ostr0...r1...r2.
+00000c30: 0000 7233 0000 00fa 3473 6861 2d32 3536  ..r3....4sha-256
+00000c40: 3d4d 494c 6235 6c55 4444 365a 3070 4453  =MILb5lUDD6Z0pDS
+00000c50: 7868 6778 6a2b 684d 4245 7730 7554 7a50  xhgxj+hMBEw0uTzP
+00000c60: 3367 3271 554a 4748 4d70 396b 3d5a 597a  3g2qUJGHMp9k=ZYz
+00000c70: 3476 506b 4a61 6f61 5356 5170 3544 724d  4vPkJaoaSVQp5DrM
+00000c80: 6238 4576 4361 6a4a 6365 7257 3336 7273  b8EvCajJcerW36rs
+00000c90: 7957 4445 4c54 5751 3363 596d 616f 6e6e  yWDELTWQ3cYmaonn
+00000ca0: 4766 6238 5748 6977 4835 3442 5368 6964  Gfb8WHiwH54BShid
+00000cb0: 4363 6d70 6f79 486a 616e 5652 594e 7258  CcmpoyHjanVRYNrX
+00000cc0: 5858 6b61 346a 416e 2905 7234 0000 0072  XXka4jAn).r4...r
+00000cd0: 3500 0000 7236 0000 00da 0664 6967 6573  5...r6.....diges
+00000ce0: 7472 3700 0000 fa10 7b22 636f 7773 223a  tr7.....{"cows":
+00000cf0: 2022 676f 6f64 227d a901 723c 0000 0029   "good"}..r<...)
+00000d00: 0472 3800 0000 7239 0000 0072 3a00 0000  .r8...r9...r:...
+00000d10: da08 6765 745f 6461 7461 7221 0000 0072  ..get_datar!...r
+00000d20: 2200 0000 7224 0000 0072 3b00 0000 7226  "...r$...r;...r&
+00000d30: 0000 0072 2800 0000 7229 0000 0029 0c72  ...r(...r)...).r
+00000d40: 3c00 0000 7203 0000 0072 0200 0000 7209  <...r....r....r.
+00000d50: 0000 0072 1400 0000 722a 0000 0072 1200  ...r....r*...r..
+00000d60: 0000 7213 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000d70: 0072 1700 0000 7218 0000 0072 3d00 0000  .r....r....r=...
+00000d80: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
+00000d90: 2574 6573 745f 7661 6c69 6461 7465 5f6d  %test_validate_m
+00000da0: 6f6f 5f61 7574 685f 7369 676e 6174 7572  oo_auth_signatur
+00000db0: 655f 706f 7374 3400 0000 731e 0000 0002  e_post4...s.....
+00000dc0: 8006 0402 0202 0102 0102 0202 0102 0102  ................
+00000dd0: 0102 0104 fb08 0706 f614 0d7c 0272 4800  ...........|.rH.
+00000de0: 0000 6301 0000 0000 0000 0000 0000 0006  ..c.............
+00000df0: 0000 0008 0000 00c3 0000 0073 6a00 0000  ...........sj...
+00000e00: 8101 6401 6402 8400 7d01 6403 7c00 5f00  ..d.d...}.d.|._.
+00000e10: 7401 7c01 8301 7d02 7402 6404 6405 6406  t.|...}.t.d.d.d.
+00000e20: 6407 6408 6409 640a 9c03 640b 8d04 7d03  d.d.d.d...d...}.
+00000e30: 7c02 7c03 8301 4900 6400 4800 7d04 7c04  |.|...I.d.H.}.|.
+00000e40: 7331 640c 640d 7403 a004 7c04 a101 6901  s1d.d.t...|...i.
+00000e50: 1600 7d05 7405 7403 a006 7c05 a101 8301  ..}.t.t...|.....
+00000e60: 8201 6400 7d04 6400 5300 290e 4e63 0100  ..d.}.d.S.).Nc..
+00000e70: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000e80: 0000 d300 0000 f30a 0000 0081 0174 0064  .............t.d
+00000e90: 0166 0253 00a9 024e da05 6f77 6e65 7272  .f.S...N..ownerr
+00000ea0: 0a00 0000 a901 da03 7572 6c72 1e00 0000  ........urlr....
+00000eb0: 721e 0000 0072 1f00 0000 da0d 6b65 795f  r....r......key_
+00000ec0: 7265 7472 6965 7665 724e 0000 00f3 0400  retrieverN......
+00000ed0: 0000 0280 0801 7a39 7465 7374 5f62 7569  ......z9test_bui
+00000ee0: 6c64 5f76 616c 6964 6174 655f 6874 7470  ld_validate_http
+00000ef0: 5f73 6967 6e61 7475 7265 2e3c 6c6f 6361  _signature.<loca
+00000f00: 6c73 3e2e 6b65 795f 7265 7472 6965 7665  ls>.key_retrieve
+00000f10: 7254 722f 0000 0072 3000 0000 fa23 6874  rTr/...r0....#ht
+00000f20: 7470 733a 2f2f 6d79 686f 7374 2e74 6c64  tps://myhost.tld
+00000f30: 2f70 6174 682f 746f 2f72 6573 6f75 7263  /path/to/resourc
+00000f40: 6572 3100 0000 7232 0000 0061 af01 0000  er1...r2...a....
+00000f50: 6b65 7949 643d 226b 6579 5f69 6422 2c61  keyId="key_id",a
+00000f60: 6c67 6f72 6974 686d 3d22 7273 612d 7368  lgorithm="rsa-sh
+00000f70: 6132 3536 222c 6865 6164 6572 733d 2228  a256",headers="(
+00000f80: 7265 7175 6573 742d 7461 7267 6574 2920  request-target) 
+00000f90: 686f 7374 2064 6174 6522 2c73 6967 6e61  host date",signa
+00000fa0: 7475 7265 3d22 6277 6741 3355 616a 7044  ture="bwgA3UajpD
+00000fb0: 7a4d 3037 774d 2b4d 556b 7047 4853 2f6d  zM07wM+MUkpGHS/m
+00000fc0: 4168 6854 752b 5744 6942 4c31 4832 384a  AhhTu+WDiBL1H28J
+00000fd0: 3736 326a 5555 7567 677a 5038 5765 352b  762jUUuggzP8We5+
+00000fe0: 4930 5748 7970 5342 4357 7438 4c61 7032  I0WHypSBCWt8Lap2
+00000ff0: 4162 5971 4736 5066 5473 6446 4562 6b38  AbYqG6PfTsdFEbk8
+00001000: 5657 6577 5833 346e 372f 4c55 534d 2f57  VWewX34n7/LUSM/W
+00001010: 4a65 4138 4146 4345 6e48 5950 6438 7252  JeA8AFCEnHYPd8rR
+00001020: 6962 3464 302b 6b51 562b 5534 4169 3939  ib4d0+kQV+U4Ai99
+00001030: 3758 5578 7332 7869 3241 7275 4e64 6b42  7XUxs2xi2AruNdkB
+00001040: 3653 4e4d 6b53 626e 514c 6f42 6a59 5434  6SNMkSbnQLoBjYT4
+00001050: 747a 4761 6632 4931 785a 7571 6a44 3148  tzGaf2I1xZuqjD1H
+00001060: 7676 5730 7861 316f 2f6e 5074 3447 356b  vvW0xa1o/nPt4G5k
+00001070: 6a30 7456 6d67 4472 7267 654b 4c32 6855  j0tVmgDrrgeKL2hU
+00001080: 4a32 3155 6448 6358 444e 4677 3951 4a57  J21UdHcXDNFw9QJW
+00001090: 662f 4f36 4b79 456d 6275 6d76 7070 4b47  f/O6KyEmbumvppKG
+000010a0: 4655 6664 704b 5368 336e 322f 6650 374f  FUfdpKSh3n2/fP7O
+000010b0: 3442 7871 6164 4362 4d59 6a30 6f44 444f  4BxqadCbMYj0oDDO
+000010c0: 4631 4833 5061 3647 5639 4566 4965 5358  F1H3Pa6GV9EfIeSX
+000010d0: 584c 5339 5466 7950 706b 5877 6257 724e  XLS9TfyPpkXwbWrN
+000010e0: 707a 5542 5a51 3268 5247 7a58 326a 532f  pzUBZQ2hRGzX2jS/
+000010f0: 4a45 6870 534e 5356 7176 3641 3d3d 2229  JEhpSNSVqv6A==")
+00001100: 0372 3400 0000 7235 0000 00da 0973 6967  .r4...r5.....sig
+00001110: 6e61 7475 7265 2904 7238 0000 0072 3900  nature).r8...r9.
+00001120: 0000 724d 0000 0072 3a00 0000 fa0e 6173  ..rM...r:.....as
+00001130: 7365 7274 2025 2870 7931 2973 da03 7079  sert %(py1)s..py
+00001140: 3129 0772 3c00 0000 7206 0000 0072 0300  1).r<...r....r..
+00001150: 0000 7214 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001160: 0072 1800 0000 a906 723e 0000 0072 4e00  .r......r>...rN.
+00001170: 0000 5a17 7661 6c69 6461 7465 5f68 7474  ..Z.validate_htt
+00001180: 705f 7369 676e 6174 7572 6572 3f00 0000  p_signaturer?...
+00001190: da0b 4070 795f 6173 7365 7274 305a 0b40  ..@py_assert0Z.@
+000011a0: 7079 5f66 6f72 6d61 7432 721e 0000 0072  py_format2r....r
+000011b0: 1e00 0000 721f 0000 00da 2274 6573 745f  ....r....."test_
+000011c0: 6275 696c 645f 7661 6c69 6461 7465 5f68  build_validate_h
+000011d0: 7474 705f 7369 676e 6174 7572 654c 0000  ttp_signatureL..
+000011e0: 0073 1c00 0000 0280 0802 0603 0802 0202  .s..............
+000011f0: 0201 0201 0201 0202 0201 0201 04fd 06fc  ................
+00001200: 3a0b 7256 0000 0063 0100 0000 0000 0000  :.rV...c........
+00001210: 0000 0000 0600 0000 0900 0000 c300 0000  ................
+00001220: 7374 0000 0081 0164 0164 0284 007d 0164  st.....d.d...}.d
+00001230: 037c 005f 0074 017c 0183 017d 0274 0264  .|._.t.|...}.t.d
+00001240: 0464 0564 0664 0764 0864 0964 0a64 0b9c  .d.d.d.d.d.d.d..
+00001250: 0474 0364 0c64 0d8d 0164 0e8d 057d 037c  .t.d.d...d...}.|
+00001260: 027c 0383 0149 0064 0048 007d 047c 0473  .|...I.d.H.}.|.s
+00001270: 3664 0f64 1074 04a0 057c 04a1 0169 0116  6d.d.t...|...i..
+00001280: 007d 0574 0674 04a0 077c 05a1 0183 0182  .}.t.t...|......
+00001290: 0164 007d 0464 0053 0029 114e 6301 0000  .d.}.d.S.).Nc...
+000012a0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+000012b0: 00d3 0000 0072 4900 0000 724a 0000 0072  .....rI...rJ...r
+000012c0: 0a00 0000 724c 0000 0072 1e00 0000 721e  ....rL...r....r.
+000012d0: 0000 0072 1f00 0000 724e 0000 0065 0000  ...r....rN...e..
+000012e0: 0072 4f00 0000 7a3e 7465 7374 5f62 7569  .rO...z>test_bui
+000012f0: 6c64 5f76 616c 6964 6174 655f 6874 7470  ld_validate_http
+00001300: 5f73 6967 6e61 7475 7265 5f70 6f73 742e  _signature_post.
+00001310: 3c6c 6f63 616c 733e 2e6b 6579 5f72 6574  <locals>.key_ret
+00001320: 7269 6576 6572 5472 4200 0000 7230 0000  rieverTrB...r0..
+00001330: 0072 5000 0000 7231 0000 0072 3200 0000  .rP...r1...r2...
+00001340: 7243 0000 0061 b601 0000 6b65 7949 643d  rC...a....keyId=
+00001350: 226b 6579 5f69 6422 2c61 6c67 6f72 6974  "key_id",algorit
+00001360: 686d 3d22 7273 612d 7368 6132 3536 222c  hm="rsa-sha256",
+00001370: 6865 6164 6572 733d 2228 7265 7175 6573  headers="(reques
+00001380: 742d 7461 7267 6574 2920 686f 7374 2064  t-target) host d
+00001390: 6174 6520 6469 6765 7374 222c 7369 676e  ate digest",sign
+000013a0: 6174 7572 653d 2251 7065 4c4d 4568 2f5a  ature="QpeLMEh/Z
+000013b0: 3030 3944 6759 6353 4f6b 7273 4b72 397a  009DgYcSOkrsKr9z
+000013c0: 5737 5775 3755 5754 5133 3938 7176 7565  W7Wu7UWTQ398qvue
+000013d0: 437a 6145 4c2f 4878 7276 3943 3432 552b  CzaEL/Hxrv9C42U+
+000013e0: 5759 2f4f 3334 782f 3338 356c 542b 7a31  WY/O34x/385lT+z1
+000013f0: 4933 426b 3671 4d5a 5444 415a 536d 4b47  I3Bk6qMZTDAZSmKG
+00001400: 5942 356c 5a4a 5642 6443 3230 6134 442b  YB5lZJVBdC20a4D+
+00001410: 2b48 7a49 7945 3632 6436 4376 7155 7351  +HzIyE62d6CvqUsQ
+00001420: 7749 7634 6f64 2f68 4f6d 6d4f 5133 484b  wIv4od/hOmmOQ3HK
+00001430: 4936 394d 554f 734e 724c 796a 4951 7855  I69MUOsNrLyjIQxU
+00001440: 614c 5342 7a31 6d2f 776b 4c76 3869 4d72  aLSBz1m/wkLv8iMr
+00001450: 6839 5177 554c 6c71 544f 3857 4856 6a53  h9QwULlqTO8WHVjS
+00001460: 4a6c 6756 776c 6c52 744f 4f63 6d33 777a  JlgVwllRtOOcm3wz
+00001470: 6f2f 6372 3258 7946 6a34 6742 3843 5564  o/cr2XyFj4gB8CUd
+00001480: 3361 4733 6471 7a43 664f 4f6f 4e51 7655  3aG3dqzCfOOoNQvU
+00001490: 684d 446c 7850 3755 7142 6e47 6f46 3670  hMDlxP7UqBnGoF6p
+000014a0: 6e59 6e54 6e4a 5553 5348 6463 6557 6245  nYnTnJUSSHdceWbE
+000014b0: 3039 5471 584c 6d41 487a 6175 5947 5364  09TqXLmAHzauYGSd
+000014c0: 6148 5253 3358 522f 536a 6537 4554 3955  aHRS3XR/Sje7ET9U
+000014d0: 614f 6748 4863 504a 4849 4e2b 346a 7242  aOgHHcPJHIN+4jrB
+000014e0: 7044 7032 474d 3639 6a6f 5857 6b5a 7768  pDp2GM69joXWkZwh
+000014f0: 4530 474f 6c39 7133 4b42 534b 413d 3d22  E0GOl9q3KBSKA=="
+00001500: 2904 7234 0000 0072 3500 0000 7244 0000  ).r4...r5...rD..
+00001510: 0072 5100 0000 7245 0000 0072 4600 0000  .rQ...rE...rF...
+00001520: 2905 7238 0000 0072 3900 0000 724d 0000  ).r8...r9...rM..
+00001530: 0072 3a00 0000 7247 0000 0072 5200 0000  .r:...rG...rR...
+00001540: 7253 0000 0029 0872 3c00 0000 7206 0000  rS...).r<...r...
+00001550: 0072 0300 0000 7202 0000 0072 1400 0000  .r....r....r....
+00001560: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00001570: 5400 0000 721e 0000 0072 1e00 0000 721f  T...r....r....r.
+00001580: 0000 00da 2774 6573 745f 6275 696c 645f  ....'test_build_
+00001590: 7661 6c69 6461 7465 5f68 7474 705f 7369  validate_http_si
+000015a0: 676e 6174 7572 655f 706f 7374 6300 0000  gnature_postc...
+000015b0: 7320 0000 0002 8008 0206 0308 0202 0202  s ..............
+000015c0: 0102 0102 0102 0202 0102 0102 0104 fc08  ................
+000015d0: 0606 f63a 0d72 5700 0000 2917 da08 6275  ...:.rW...)...bu
+000015e0: 696c 7469 6e73 7212 0000 00da 195f 7079  iltinsr......_py
+000015f0: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
+00001600: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
+00001610: 6eda 0772 6577 7269 7465 7214 0000 00da  n..rewriter.....
+00001620: 0d75 6e69 7474 6573 742e 6d6f 636b 7202  .unittest.mockr.
+00001630: 0000 0072 0300 0000 7204 0000 00da 0072  ...r....r......r
+00001640: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
+00001650: 0000 00da 0474 6573 7472 0b00 0000 7220  .....testr....r 
+00001660: 0000 0072 2e00 0000 7241 0000 0072 4800  ...r....rA...rH.
+00001670: 0000 7256 0000 0072 5700 0000 721e 0000  ..rV...rW...r...
+00001680: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00001690: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
+000016a0: 0000 002e 0018 020c 0608 0308 0a06 080a  ................
+000016b0: 0106 150a 0106 170a 0106 160e 01         .............
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 896 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 8003 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 8003 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6403 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6406 6407  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 5081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 d913 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 d913 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6402 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6402 6405  l.m.Z.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 0100 6406 6407 8400 5a0e  l.m.Z...d.d...Z.
```

### Comparing `bovine-0.1.2/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 b704 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 b704 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
 00000060: 8400 5a09 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0953 6967 6e61 7475  .....)...Signatu
```

### Comparing `bovine-0.1.2/bovine/crypto/helper.py` & `bovine-0.1.3/bovine/crypto/helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/crypto/http_signature.py` & `bovine-0.1.3/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/crypto/signature_checker.py` & `bovine-0.1.3/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/crypto/signature_parser.py` & `bovine-0.1.3/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/crypto/test.py` & `bovine-0.1.3/bovine/crypto/test.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/crypto/test_crypto.py` & `bovine-0.1.3/bovine/crypto/test_crypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             "date": "Wed, 15 Mar 2023 17:28:15 GMT",
             "host": "myhost.tld",
             "authorization": "Moo-Auth-1 did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5",  # noqa F501
             "x-moo-signature": "z5ahdHCbP9aJEsDtvG1MEZpxPzuvGKYcdXdKvMq5YL21Z2umxjs1SopCY2Ap8vZxVjTEf6dYbGuB7mtgcgUyNdBLe",  # noqa F501
         },
     )
 
-    result = await validate_moo_auth_signature(request, "myhost.tld")
+    result, _ = await validate_moo_auth_signature(request, "myhost.tld")
 
     assert result == "did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5"
 
 
 @patch("bovine.utils.date.check_max_offset_now")
 async def test_validate_moo_auth_signature_post(mock_offset):
     # https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation#appendix-test-data
@@ -64,15 +64,15 @@
             "authorization": "Moo-Auth-1 did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5",  # noqa F501
             "digest": "sha-256=MILb5lUDD6Z0pDSxhgxj+hMBEw0uTzP3g2qUJGHMp9k=",
             "x-moo-signature": "z4vPkJaoaSVQp5DrMb8EvCajJcerW36rsyWDELTWQ3cYmaonnGfb8WHiwH54BShidCcmpoyHjanVRYNrXXXka4jAn",  # noqa F501
         },
         get_data=AsyncMock(return_value='{"cows": "good"}'),
     )
 
-    result = await validate_moo_auth_signature(request, "myhost.tld")
+    result, _ = await validate_moo_auth_signature(request, "myhost.tld")
 
     assert result == "did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5"
 
 
 @patch("bovine.utils.date.check_max_offset_now")
 async def test_build_validate_http_signature(mock_offset):
     async def key_retriever(url):
```

### Comparing `bovine-0.1.2/bovine/crypto/test_helper.py` & `bovine-0.1.3/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/crypto/test_http_signature.py` & `bovine-0.1.3/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/crypto/test_signature_parser.py` & `bovine-0.1.3/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/msg.py` & `bovine-0.1.3/bovine/msg.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/types.py` & `bovine-0.1.3/bovine/types.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/utils/__init__.py` & `bovine-0.1.3/bovine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.3/bovine/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 9b02 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 9b02 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6503 6403 6503 6404 6503 6405 6504 6608  e.d.e.d.e.d.e.f.
 00000050: 6406 6407 8404 5a05 6408 6503 6405 6502  d.d...Z.d.e.d.e.
 00000060: 6503 6501 6503 1900 6602 1900 6604 6409  e.e.e...f...f.d.
 00000070: 640a 8404 5a06 640b 5300 290c e900 0000  d...Z.d.S.).....
```

### Comparing `bovine-0.1.2/bovine/utils/__pycache__/date.cpython-310.pyc` & `bovine-0.1.3/bovine/utils/__pycache__/date.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 0702 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 0702 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d00 5a00 6d01 5a01 6d02 5a02  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6505 6602 6404 6405 8404 5a06 6406 6505  e.f.d.d...Z.d.e.
 00000060: 6403 6500 6604 6407 6408 8404 5a07 640f  d.e.f.d.d...Z.d.
 00000070: 640a 6500 640b 6508 6403 6509 6606 640c  d.e.d.e.d.e.f.d.
```

### Comparing `bovine-0.1.2/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,216 +1,217 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 e102 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 f902 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
+00000020: 0003 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 6d08 5a08 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100  l.m.Z.m.Z.m.Z...
-00000070: 6405 6406 8400 5a0d 6407 6408 8400 5a0e  d.d...Z.d.d...Z.
-00000080: 6409 640a 8400 5a0f 6401 5300 290b e900  d.d...Z.d.S.)...
-00000090: 0000 004e 2903 da08 6461 7465 7469 6d65  ...N)...datetime
-000000a0: da09 7469 6d65 6465 6c74 61da 0874 696d  ..timedelta..tim
-000000b0: 657a 6f6e 65e9 0100 0000 2903 da14 6368  ezone.....)...ch
-000000c0: 6563 6b5f 6d61 785f 6f66 6673 6574 5f6e  eck_max_offset_n
-000000d0: 6f77 da0b 6765 745f 676d 745f 6e6f 77da  ow..get_gmt_now.
-000000e0: 0970 6172 7365 5f67 6d74 6300 0000 0000  .parse_gmtc.....
-000000f0: 0000 0000 0000 0005 0000 0007 0000 0043  ...............C
-00000100: 0000 0073 8200 0000 7400 8300 7d00 6401  ...s....t...}.d.
-00000110: 7d01 7c01 7c00 7600 7d02 7c02 733b 7401  }.|.|.v.}.|.s;t.
-00000120: a002 6402 7c02 6601 6403 7c01 7c00 6602  ..d.|.f.d.|.|.f.
-00000130: a104 7401 a003 7c01 a101 6404 7404 a005  ..t...|...d.t...
-00000140: a100 7600 7324 7401 a006 7c00 a101 7229  ..v.s$t...|...r)
-00000150: 7401 a003 7c00 a101 6e01 6404 6405 9c02  t...|...n.d.d...
-00000160: 1600 7d03 6406 6407 7c03 6901 1600 7d04  ..}.d.d.|.i...}.
-00000170: 7407 7401 a008 7c04 a101 8301 8201 6400  t.t...|.......d.
-00000180: 0400 7d01 7d02 6400 5300 2908 4eda 0347  ..}.}.d.S.).N..G
-00000190: 4d54 2901 da02 696e 2901 7a12 2528 7079  MT)...in).z.%(py
-000001a0: 3129 7320 696e 2025 2870 7933 2973 da0b  1)s in %(py3)s..
-000001b0: 6461 7465 5f73 7472 696e 6729 02da 0370  date_string)...p
-000001c0: 7931 da03 7079 337a 0e61 7373 6572 7420  y1..py3z.assert 
-000001d0: 2528 7079 3529 73da 0370 7935 2909 7207  %(py5)s..py5).r.
-000001e0: 0000 00da 0a40 7079 7465 7374 5f61 72da  .....@pytest_ar.
-000001f0: 115f 6361 6c6c 5f72 6570 7263 6f6d 7061  ._call_reprcompa
-00000200: 7265 da09 5f73 6166 6572 6570 72da 0c40  re.._saferepr..@
-00000210: 7079 5f62 7569 6c74 696e 73da 066c 6f63  py_builtins..loc
-00000220: 616c 73da 185f 7368 6f75 6c64 5f72 6570  als.._should_rep
-00000230: 725f 676c 6f62 616c 5f6e 616d 65da 0e41  r_global_name..A
-00000240: 7373 6572 7469 6f6e 4572 726f 72da 135f  ssertionError.._
-00000250: 666f 726d 6174 5f65 7870 6c61 6e61 7469  format_explanati
-00000260: 6f6e 2905 720b 0000 00da 0b40 7079 5f61  on).r......@py_a
-00000270: 7373 6572 7430 da0b 4070 795f 6173 7365  ssert0..@py_asse
-00000280: 7274 32da 0b40 7079 5f66 6f72 6d61 7434  rt2..@py_format4
-00000290: da0b 4070 795f 666f 726d 6174 36a9 0072  ..@py_format6..r
-000002a0: 1b00 0000 fa4b 2f77 6f6f 6470 6563 6b65  .....K/woodpecke
-000002b0: 722f 7372 632f 636f 6465 6265 7267 2e6f  r/src/codeberg.o
-000002c0: 7267 2f62 6f76 696e 652f 626f 7669 6e65  rg/bovine/bovine
-000002d0: 2f62 6f76 696e 652f 626f 7669 6e65 2f75  /bovine/bovine/u
-000002e0: 7469 6c73 2f74 6573 745f 6461 7465 2e70  tils/test_date.p
-000002f0: 79da 1074 6573 745f 6765 745f 676d 745f  y..test_get_gmt_
-00000300: 6e6f 7706 0000 0073 0400 0000 0601 7c02  now....s......|.
-00000310: 721d 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000320: 0000 0b00 0000 0800 0000 4300 0000 7388  ..........C...s.
-00000330: 0100 0074 0083 007d 0074 017c 0083 017d  ...t...}.t.|...}
-00000340: 0174 026a 0374 046a 0564 018d 017d 027c  .t.j.t.j.d...}.|
-00000350: 017c 026b 017d 037c 0373 5174 06a0 0764  .|.k.}.|.sQt...d
-00000360: 027c 0366 0164 037c 017c 0266 02a1 0464  .|.f.d.|.|.f...d
-00000370: 0474 08a0 09a1 0076 0073 2974 06a0 0a7c  .t.....v.s)t...|
-00000380: 01a1 0172 2e74 06a0 0b7c 01a1 016e 0164  ...r.t...|...n.d
-00000390: 0464 0574 08a0 09a1 0076 0073 3a74 06a0  .d.t.....v.s:t..
-000003a0: 0a7c 02a1 0172 3f74 06a0 0b7c 02a1 016e  .|...r?t...|...n
-000003b0: 0164 0564 069c 0216 007d 0464 0764 087c  .d.d.....}.d.d.|
-000003c0: 0469 0116 007d 0574 0c74 06a0 0d7c 05a1  .i...}.t.t...|..
-000003d0: 0183 0182 0164 007d 0364 097d 0674 0e7c  .....d.}.d.}.t.|
-000003e0: 0664 0a8d 017d 077c 027c 0718 007d 087c  .d...}.|.|...}.|
-000003f0: 017c 086b 057d 037c 0373 ba74 06a0 0764  .|.k.}.|.s.t...d
-00000400: 0b7c 0366 0164 0c7c 017c 0866 02a1 0464  .|.f.d.|.|.f...d
-00000410: 0474 08a0 09a1 0076 0073 7974 06a0 0a7c  .t.....v.syt...|
-00000420: 01a1 0172 7e74 06a0 0b7c 01a1 016e 0164  ...r~t...|...n.d
-00000430: 0464 0574 08a0 09a1 0076 0073 8a74 06a0  .d.t.....v.s.t..
-00000440: 0a7c 02a1 0172 8f74 06a0 0b7c 02a1 016e  .|...r.t...|...n
-00000450: 0164 0564 0d74 08a0 09a1 0076 0073 9b74  .d.d.t.....v.s.t
-00000460: 06a0 0a74 0ea1 0172 a074 06a0 0b74 0ea1  ...t...r.t...t..
-00000470: 016e 0164 0d74 06a0 0b7c 06a1 0174 06a0  .n.d.t...|...t..
-00000480: 0b7c 07a1 0164 0e9c 0516 007d 0964 0f64  .|...d.....}.d.d
-00000490: 107c 0969 0116 007d 0a74 0c74 06a0 0d7c  .|.i...}.t.t...|
-000004a0: 0aa1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
-000004b0: 0604 007d 077d 0864 0053 0029 114e a901  ...}.}.d.S.).N..
-000004c0: da02 747a 2901 fa02 3c3d 2901 7a12 2528  ..tz)...<=).z.%(
-000004d0: 7079 3029 7320 3c3d 2025 2870 7932 2973  py0)s <= %(py2)s
-000004e0: da06 7061 7273 6564 da03 6e6f 7729 02da  ..parsed..now)..
-000004f0: 0370 7930 da03 7079 327a 0e61 7373 6572  .py0..py2z.asser
-00000500: 7420 2528 7079 3429 73da 0370 7934 e905  t %(py4)s..py4..
-00000510: 0000 0029 01da 0773 6563 6f6e 6473 2901  ...)...seconds).
-00000520: fa02 3e3d 2901 7a44 2528 7079 3029 7320  ..>=).zD%(py0)s 
-00000530: 3e3d 2028 2528 7079 3229 7320 2d20 2528  >= (%(py2)s - %(
-00000540: 7079 3729 730a 7b25 2870 7937 2973 203d  py7)s.{%(py7)s =
-00000550: 2025 2870 7933 2973 2873 6563 6f6e 6473   %(py3)s(seconds
-00000560: 3d25 2870 7935 2973 290a 7d29 7203 0000  =%(py5)s).})r...
-00000570: 0029 0572 2300 0000 7224 0000 0072 0d00  .).r#...r$...r..
-00000580: 0000 720e 0000 00da 0370 7937 7a0f 6173  ..r......py7z.as
-00000590: 7365 7274 2025 2870 7931 3029 73da 0470  sert %(py10)s..p
-000005a0: 7931 3029 0f72 0700 0000 7208 0000 0072  y10).r....r....r
-000005b0: 0200 0000 7222 0000 0072 0400 0000 da03  ....r"...r......
-000005c0: 7574 6372 0f00 0000 7210 0000 0072 1200  utcr....r....r..
-000005d0: 0000 7213 0000 0072 1400 0000 7211 0000  ..r....r....r...
-000005e0: 0072 1500 0000 7216 0000 0072 0300 0000  .r....r....r....
-000005f0: 290b 720b 0000 0072 2100 0000 7222 0000  ).r....r!...r"..
-00000600: 00da 0b40 7079 5f61 7373 6572 7431 da0b  ...@py_assert1..
-00000610: 4070 795f 666f 726d 6174 33da 0b40 7079  @py_format3..@py
-00000620: 5f66 6f72 6d61 7435 da0b 4070 795f 6173  _format5..@py_as
-00000630: 7365 7274 34da 0b40 7079 5f61 7373 6572  sert4..@py_asser
-00000640: 7436 da0b 4070 795f 6173 7365 7274 38da  t6..@py_assert8.
-00000650: 0b40 7079 5f66 6f72 6d61 7439 da0c 4070  .@py_format9..@p
-00000660: 795f 666f 726d 6174 3131 721b 0000 0072  y_format11r....r
-00000670: 1b00 0000 721c 0000 00da 0e74 6573 745f  ....r......test_
-00000680: 7061 7273 655f 676d 740c 0000 0073 0a00  parse_gmt....s..
-00000690: 0000 0601 0802 0e01 8a02 e201 7234 0000  ............r4..
-000006a0: 0063 0000 0000 0000 0000 0000 0000 0800  .c..............
-000006b0: 0000 0900 0000 4300 0000 735e 0300 0074  ......C...s^...t
-000006c0: 006a 0174 026a 0364 018d 017d 0064 027d  .j.t.j.d...}.d.}
-000006d0: 0174 047c 0164 038d 017d 027c 007c 0218  .t.|.d...}.|.|..
-000006e0: 007d 0374 057c 0383 017d 047c 0473 6364  .}.t.|...}.|.scd
-000006f0: 0464 0574 06a0 07a1 0076 0073 2474 08a0  .d.t.....v.s$t..
-00000700: 0974 05a1 0172 2974 08a0 0a74 05a1 016e  .t...r)t...t...n
-00000710: 0164 0564 0674 06a0 07a1 0076 0073 3574  .d.d.t.....v.s5t
-00000720: 08a0 097c 00a1 0172 3a74 08a0 0a7c 00a1  ...|...r:t...|..
-00000730: 016e 0164 0664 0774 06a0 07a1 0076 0073  .n.d.d.t.....v.s
-00000740: 4674 08a0 0974 04a1 0172 4b74 08a0 0a74  Ft...t...rKt...t
-00000750: 04a1 016e 0164 0774 08a0 0a7c 01a1 0174  ...n.d.t...|...t
-00000760: 08a0 0a7c 02a1 0174 08a0 0a7c 04a1 0164  ...|...t...|...d
-00000770: 089c 0616 007d 0574 0b74 08a0 0c7c 05a1  .....}.t.t...|..
-00000780: 0183 0182 0164 0004 007d 0104 007d 0204  .....d...}...}..
-00000790: 007d 037d 0464 027d 0174 047c 0164 038d  .}.}.d.}.t.|.d..
-000007a0: 017d 027c 007c 0217 007d 0374 057c 0383  .}.|.|...}.t.|..
-000007b0: 017d 047c 0473 c764 0964 0574 06a0 07a1  .}.|.s.d.d.t....
-000007c0: 0076 0073 8874 08a0 0974 05a1 0172 8d74  .v.s.t...t...r.t
-000007d0: 08a0 0a74 05a1 016e 0164 0564 0674 06a0  ...t...n.d.d.t..
-000007e0: 07a1 0076 0073 9974 08a0 097c 00a1 0172  ...v.s.t...|...r
-000007f0: 9e74 08a0 0a7c 00a1 016e 0164 0664 0774  .t...|...n.d.d.t
-00000800: 06a0 07a1 0076 0073 aa74 08a0 0974 04a1  .....v.s.t...t..
-00000810: 0172 af74 08a0 0a74 04a1 016e 0164 0774  .r.t...t...n.d.t
-00000820: 08a0 0a7c 01a1 0174 08a0 0a7c 02a1 0174  ...|...t...|...t
-00000830: 08a0 0a7c 04a1 0164 089c 0616 007d 0574  ...|...d.....}.t
-00000840: 0b74 08a0 0c7c 05a1 0183 0182 0164 0004  .t...|.......d..
-00000850: 007d 0104 007d 0204 007d 037d 0464 0a7d  .}...}...}.}.d.}
-00000860: 0174 047c 0164 038d 017d 027c 007c 0218  .t.|.d...}.|.|..
-00000870: 007d 0374 057c 0383 017d 047c 040c 007d  .}.t.|...}.|...}
-00000880: 067c 0690 0173 3364 0b64 0574 06a0 07a1  .|...s3d.d.t....
-00000890: 0076 0073 f074 08a0 0974 05a1 0172 f574  .v.s.t...t...r.t
-000008a0: 08a0 0a74 05a1 016e 0164 0564 0674 06a0  ...t...n.d.d.t..
-000008b0: 07a1 0076 0090 0173 0374 08a0 097c 00a1  ...v...s.t...|..
-000008c0: 0190 0172 0874 08a0 0a7c 00a1 016e 0164  ...r.t...|...n.d
-000008d0: 0664 0774 06a0 07a1 0076 0090 0173 1674  .d.t.....v...s.t
-000008e0: 08a0 0974 04a1 0190 0172 1b74 08a0 0a74  ...t.....r.t...t
-000008f0: 04a1 016e 0164 0774 08a0 0a7c 01a1 0174  ...n.d.t...|...t
-00000900: 08a0 0a7c 02a1 0174 08a0 0a7c 04a1 0164  ...|...t...|...d
-00000910: 089c 0616 007d 0774 0b74 08a0 0c7c 07a1  .....}.t.t...|..
-00000920: 0183 0182 0164 0004 007d 0104 007d 0204  .....d...}...}..
-00000930: 007d 0304 007d 047d 0664 0a7d 0174 047c  .}...}.}.d.}.t.|
-00000940: 0164 038d 017d 027c 007c 0217 007d 0374  .d...}.|.|...}.t
-00000950: 057c 0383 017d 047c 040c 007d 067c 0690  .|...}.|...}.|..
-00000960: 0173 a364 0c64 0574 06a0 07a1 0076 0090  .s.d.d.t.....v..
-00000970: 0173 6074 08a0 0974 05a1 0190 0172 6574  .s`t...t.....ret
-00000980: 08a0 0a74 05a1 016e 0164 0564 0674 06a0  ...t...n.d.d.t..
-00000990: 07a1 0076 0090 0173 7374 08a0 097c 00a1  ...v...sst...|..
-000009a0: 0190 0172 7874 08a0 0a7c 00a1 016e 0164  ...rxt...|...n.d
-000009b0: 0664 0774 06a0 07a1 0076 0090 0173 8674  .d.t.....v...s.t
-000009c0: 08a0 0974 04a1 0190 0172 8b74 08a0 0a74  ...t.....r.t...t
-000009d0: 04a1 016e 0164 0774 08a0 0a7c 01a1 0174  ...n.d.t...|...t
-000009e0: 08a0 0a7c 02a1 0174 08a0 0a7c 04a1 0164  ...|...t...|...d
-000009f0: 089c 0616 007d 0774 0b74 08a0 0c7c 07a1  .....}.t.t...|..
-00000a00: 0183 0182 0164 0004 007d 0104 007d 0204  .....d...}...}..
-00000a10: 007d 0304 007d 047d 0664 0053 0029 0d4e  .}...}.}.d.S.).N
-00000a20: 721e 0000 00e9 0400 0000 2901 da07 6d69  r.........)...mi
-00000a30: 6e75 7465 737a 5e61 7373 6572 7420 2528  nutesz^assert %(
-00000a40: 7079 3929 730a 7b25 2870 7939 2973 203d  py9)s.{%(py9)s =
-00000a50: 2025 2870 7930 2973 2828 2528 7079 3129   %(py0)s((%(py1)
-00000a60: 7320 2d20 2528 7079 3629 730a 7b25 2870  s - %(py6)s.{%(p
-00000a70: 7936 2973 203d 2025 2870 7932 2973 286d  y6)s = %(py2)s(m
-00000a80: 696e 7574 6573 3d25 2870 7934 2973 290a  inutes=%(py4)s).
-00000a90: 7d29 290a 7d72 0600 0000 7222 0000 0072  })).}r....r"...r
-00000aa0: 0300 0000 2906 7223 0000 0072 0c00 0000  ....).r#...r....
-00000ab0: 7224 0000 0072 2500 0000 da03 7079 36da  r$...r%.....py6.
-00000ac0: 0370 7939 7a5e 6173 7365 7274 2025 2870  .py9z^assert %(p
-00000ad0: 7939 2973 0a7b 2528 7079 3929 7320 3d20  y9)s.{%(py9)s = 
-00000ae0: 2528 7079 3029 7328 2825 2870 7931 2973  %(py0)s((%(py1)s
-00000af0: 202b 2025 2870 7936 2973 0a7b 2528 7079   + %(py6)s.{%(py
-00000b00: 3629 7320 3d20 2528 7079 3229 7328 6d69  6)s = %(py2)s(mi
-00000b10: 6e75 7465 733d 2528 7079 3429 7329 0a7d  nutes=%(py4)s).}
-00000b20: 2929 0a7d e906 0000 007a 6261 7373 6572  )).}.....zbasser
-00000b30: 7420 6e6f 7420 2528 7079 3929 730a 7b25  t not %(py9)s.{%
-00000b40: 2870 7939 2973 203d 2025 2870 7930 2973  (py9)s = %(py0)s
-00000b50: 2828 2528 7079 3129 7320 2d20 2528 7079  ((%(py1)s - %(py
-00000b60: 3629 730a 7b25 2870 7936 2973 203d 2025  6)s.{%(py6)s = %
-00000b70: 2870 7932 2973 286d 696e 7574 6573 3d25  (py2)s(minutes=%
-00000b80: 2870 7934 2973 290a 7d29 290a 7d7a 6261  (py4)s).})).}zba
-00000b90: 7373 6572 7420 6e6f 7420 2528 7079 3929  ssert not %(py9)
-00000ba0: 730a 7b25 2870 7939 2973 203d 2025 2870  s.{%(py9)s = %(p
-00000bb0: 7930 2973 2828 2528 7079 3129 7320 2b20  y0)s((%(py1)s + 
-00000bc0: 2528 7079 3629 730a 7b25 2870 7936 2973  %(py6)s.{%(py6)s
-00000bd0: 203d 2025 2870 7932 2973 286d 696e 7574   = %(py2)s(minut
-00000be0: 6573 3d25 2870 7934 2973 290a 7d29 290a  es=%(py4)s).})).
-00000bf0: 7d29 0d72 0200 0000 7222 0000 0072 0400  }).r....r"...r..
-00000c00: 0000 722b 0000 0072 0300 0000 7206 0000  ..r+...r....r...
-00000c10: 0072 1200 0000 7213 0000 0072 0f00 0000  .r....r....r....
-00000c20: 7214 0000 0072 1100 0000 7215 0000 0072  r....r....r....r
-00000c30: 1600 0000 2908 7222 0000 00da 0b40 7079  ....).r".....@py
-00000c40: 5f61 7373 6572 7433 da0b 4070 795f 6173  _assert3..@py_as
-00000c50: 7365 7274 35da 0b40 7079 5f61 7373 6572  sert5..@py_asser
-00000c60: 7437 7231 0000 00da 0c40 7079 5f66 6f72  t7r1.....@py_for
-00000c70: 6d61 7431 305a 0c40 7079 5f61 7373 6572  mat10Z.@py_asser
-00000c80: 7431 3072 3300 0000 721b 0000 0072 1b00  t10r3...r....r..
-00000c90: 0000 721c 0000 00da 1974 6573 745f 6368  ..r......test_ch
-00000ca0: 6563 6b5f 6d61 785f 6f66 6673 6574 5f6e  eck_max_offset_n
-00000cb0: 6f77 1600 0000 730a 0000 000e 01c8 02c8  ow....s.........
-00000cc0: 01dc 01e4 0172 3e00 0000 2910 da08 6275  .....r>...)...bu
-00000cd0: 696c 7469 6e73 7212 0000 00da 195f 7079  iltinsr......_py
-00000ce0: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
-00000cf0: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
-00000d00: 6eda 0772 6577 7269 7465 720f 0000 0072  n..rewriter....r
-00000d10: 0200 0000 7203 0000 0072 0400 0000 da04  ....r....r......
-00000d20: 6461 7465 7206 0000 0072 0700 0000 7208  dater....r....r.
-00000d30: 0000 0072 1d00 0000 7234 0000 0072 3e00  ...r....r4...r>.
-00000d40: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
-00000d50: 0072 1c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000d60: 0100 0000 730a 0000 002e 0014 0208 0308  ....s...........
-00000d70: 060c 0a                                  ...
+00000070: 640c 6406 6407 8404 5a0d 640c 6408 6409  d.d.d...Z.d.d.d.
+00000080: 8404 5a0e 640c 640a 640b 8404 5a0f 6401  ..Z.d.d.d...Z.d.
+00000090: 5300 290d e900 0000 004e 2903 da08 6461  S.)......N)...da
+000000a0: 7465 7469 6d65 da09 7469 6d65 6465 6c74  tetime..timedelt
+000000b0: 61da 0874 696d 657a 6f6e 65e9 0100 0000  a..timezone.....
+000000c0: 2903 da14 6368 6563 6b5f 6d61 785f 6f66  )...check_max_of
+000000d0: 6673 6574 5f6e 6f77 da0b 6765 745f 676d  fset_now..get_gm
+000000e0: 745f 6e6f 77da 0970 6172 7365 5f67 6d74  t_now..parse_gmt
+000000f0: da06 7265 7475 726e 6300 0000 0000 0000  ..returnc.......
+00000100: 0000 0000 0005 0000 0007 0000 0043 0000  .............C..
+00000110: 0073 8200 0000 7400 8300 7d00 6401 7d01  .s....t...}.d.}.
+00000120: 7c01 7c00 7600 7d02 7c02 733b 7401 a002  |.|.v.}.|.s;t...
+00000130: 6402 7c02 6601 6403 7c01 7c00 6602 a104  d.|.f.d.|.|.f...
+00000140: 7401 a003 7c01 a101 6404 7404 a005 a100  t...|...d.t.....
+00000150: 7600 7324 7401 a006 7c00 a101 7229 7401  v.s$t...|...r)t.
+00000160: a003 7c00 a101 6e01 6404 6405 9c02 1600  ..|...n.d.d.....
+00000170: 7d03 6406 6407 7c03 6901 1600 7d04 7407  }.d.d.|.i...}.t.
+00000180: 7401 a008 7c04 a101 8301 8201 6400 0400  t...|.......d...
+00000190: 7d01 7d02 6400 5300 2908 4eda 0347 4d54  }.}.d.S.).N..GMT
+000001a0: 2901 da02 696e 2901 7a12 2528 7079 3129  )...in).z.%(py1)
+000001b0: 7320 696e 2025 2870 7933 2973 da0b 6461  s in %(py3)s..da
+000001c0: 7465 5f73 7472 696e 6729 02da 0370 7931  te_string)...py1
+000001d0: da03 7079 337a 0e61 7373 6572 7420 2528  ..py3z.assert %(
+000001e0: 7079 3529 73da 0370 7935 2909 7207 0000  py5)s..py5).r...
+000001f0: 00da 0a40 7079 7465 7374 5f61 72da 115f  ...@pytest_ar.._
+00000200: 6361 6c6c 5f72 6570 7263 6f6d 7061 7265  call_reprcompare
+00000210: da09 5f73 6166 6572 6570 72da 0c40 7079  .._saferepr..@py
+00000220: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
+00000230: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
+00000240: 676c 6f62 616c 5f6e 616d 65da 0e41 7373  global_name..Ass
+00000250: 6572 7469 6f6e 4572 726f 72da 135f 666f  ertionError.._fo
+00000260: 726d 6174 5f65 7870 6c61 6e61 7469 6f6e  rmat_explanation
+00000270: 2905 720c 0000 00da 0b40 7079 5f61 7373  ).r......@py_ass
+00000280: 6572 7430 da0b 4070 795f 6173 7365 7274  ert0..@py_assert
+00000290: 32da 0b40 7079 5f66 6f72 6d61 7434 da0b  2..@py_format4..
+000002a0: 4070 795f 666f 726d 6174 36a9 0072 1c00  @py_format6..r..
+000002b0: 0000 fa4b 2f77 6f6f 6470 6563 6b65 722f  ...K/woodpecker/
+000002c0: 7372 632f 636f 6465 6265 7267 2e6f 7267  src/codeberg.org
+000002d0: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
+000002e0: 6f76 696e 652f 626f 7669 6e65 2f75 7469  ovine/bovine/uti
+000002f0: 6c73 2f74 6573 745f 6461 7465 2e70 79da  ls/test_date.py.
+00000300: 1074 6573 745f 6765 745f 676d 745f 6e6f  .test_get_gmt_no
+00000310: 7706 0000 0073 0400 0000 0601 7c02 721e  w....s......|.r.
+00000320: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000330: 0b00 0000 0800 0000 4300 0000 7388 0100  ........C...s...
+00000340: 0074 0083 007d 0074 017c 0083 017d 0174  .t...}.t.|...}.t
+00000350: 026a 0374 046a 0564 018d 017d 027c 017c  .j.t.j.d...}.|.|
+00000360: 026b 017d 037c 0373 5174 06a0 0764 027c  .k.}.|.sQt...d.|
+00000370: 0366 0164 037c 017c 0266 02a1 0464 0474  .f.d.|.|.f...d.t
+00000380: 08a0 09a1 0076 0073 2974 06a0 0a7c 01a1  .....v.s)t...|..
+00000390: 0172 2e74 06a0 0b7c 01a1 016e 0164 0464  .r.t...|...n.d.d
+000003a0: 0574 08a0 09a1 0076 0073 3a74 06a0 0a7c  .t.....v.s:t...|
+000003b0: 02a1 0172 3f74 06a0 0b7c 02a1 016e 0164  ...r?t...|...n.d
+000003c0: 0564 069c 0216 007d 0464 0764 087c 0469  .d.....}.d.d.|.i
+000003d0: 0116 007d 0574 0c74 06a0 0d7c 05a1 0183  ...}.t.t...|....
+000003e0: 0182 0164 007d 0364 097d 0674 0e7c 0664  ...d.}.d.}.t.|.d
+000003f0: 0a8d 017d 077c 027c 0718 007d 087c 017c  ...}.|.|...}.|.|
+00000400: 086b 057d 037c 0373 ba74 06a0 0764 0b7c  .k.}.|.s.t...d.|
+00000410: 0366 0164 0c7c 017c 0866 02a1 0464 0474  .f.d.|.|.f...d.t
+00000420: 08a0 09a1 0076 0073 7974 06a0 0a7c 01a1  .....v.syt...|..
+00000430: 0172 7e74 06a0 0b7c 01a1 016e 0164 0464  .r~t...|...n.d.d
+00000440: 0574 08a0 09a1 0076 0073 8a74 06a0 0a7c  .t.....v.s.t...|
+00000450: 02a1 0172 8f74 06a0 0b7c 02a1 016e 0164  ...r.t...|...n.d
+00000460: 0564 0d74 08a0 09a1 0076 0073 9b74 06a0  .d.t.....v.s.t..
+00000470: 0a74 0ea1 0172 a074 06a0 0b74 0ea1 016e  .t...r.t...t...n
+00000480: 0164 0d74 06a0 0b7c 06a1 0174 06a0 0b7c  .d.t...|...t...|
+00000490: 07a1 0164 0e9c 0516 007d 0964 0f64 107c  ...d.....}.d.d.|
+000004a0: 0969 0116 007d 0a74 0c74 06a0 0d7c 0aa1  .i...}.t.t...|..
+000004b0: 0183 0182 0164 0004 007d 0304 007d 0604  .....d...}...}..
+000004c0: 007d 077d 0864 0053 0029 114e a901 da02  .}.}.d.S.).N....
+000004d0: 747a 2901 fa02 3c3d 2901 7a12 2528 7079  tz)...<=).z.%(py
+000004e0: 3029 7320 3c3d 2025 2870 7932 2973 da06  0)s <= %(py2)s..
+000004f0: 7061 7273 6564 da03 6e6f 7729 02da 0370  parsed..now)...p
+00000500: 7930 da03 7079 327a 0e61 7373 6572 7420  y0..py2z.assert 
+00000510: 2528 7079 3429 73da 0370 7934 e905 0000  %(py4)s..py4....
+00000520: 0029 01da 0773 6563 6f6e 6473 2901 fa02  .)...seconds)...
+00000530: 3e3d 2901 7a44 2528 7079 3029 7320 3e3d  >=).zD%(py0)s >=
+00000540: 2028 2528 7079 3229 7320 2d20 2528 7079   (%(py2)s - %(py
+00000550: 3729 730a 7b25 2870 7937 2973 203d 2025  7)s.{%(py7)s = %
+00000560: 2870 7933 2973 2873 6563 6f6e 6473 3d25  (py3)s(seconds=%
+00000570: 2870 7935 2973 290a 7d29 7203 0000 0029  (py5)s).})r....)
+00000580: 0572 2400 0000 7225 0000 0072 0e00 0000  .r$...r%...r....
+00000590: 720f 0000 00da 0370 7937 7a0f 6173 7365  r......py7z.asse
+000005a0: 7274 2025 2870 7931 3029 73da 0470 7931  rt %(py10)s..py1
+000005b0: 3029 0f72 0700 0000 7208 0000 0072 0200  0).r....r....r..
+000005c0: 0000 7223 0000 0072 0400 0000 da03 7574  ..r#...r......ut
+000005d0: 6372 1000 0000 7211 0000 0072 1300 0000  cr....r....r....
+000005e0: 7214 0000 0072 1500 0000 7212 0000 0072  r....r....r....r
+000005f0: 1600 0000 7217 0000 0072 0300 0000 290b  ....r....r....).
+00000600: 720c 0000 0072 2200 0000 7223 0000 00da  r....r"...r#....
+00000610: 0b40 7079 5f61 7373 6572 7431 da0b 4070  .@py_assert1..@p
+00000620: 795f 666f 726d 6174 33da 0b40 7079 5f66  y_format3..@py_f
+00000630: 6f72 6d61 7435 da0b 4070 795f 6173 7365  ormat5..@py_asse
+00000640: 7274 34da 0b40 7079 5f61 7373 6572 7436  rt4..@py_assert6
+00000650: da0b 4070 795f 6173 7365 7274 38da 0b40  ..@py_assert8..@
+00000660: 7079 5f66 6f72 6d61 7439 da0c 4070 795f  py_format9..@py_
+00000670: 666f 726d 6174 3131 721c 0000 0072 1c00  format11r....r..
+00000680: 0000 721d 0000 00da 0e74 6573 745f 7061  ..r......test_pa
+00000690: 7273 655f 676d 740c 0000 0073 0a00 0000  rse_gmt....s....
+000006a0: 0601 0802 0e01 8a02 e201 7235 0000 0063  ..........r5...c
+000006b0: 0000 0000 0000 0000 0000 0000 0800 0000  ................
+000006c0: 0900 0000 4300 0000 735e 0300 0074 006a  ....C...s^...t.j
+000006d0: 0174 026a 0364 018d 017d 0064 027d 0174  .t.j.d...}.d.}.t
+000006e0: 047c 0164 038d 017d 027c 007c 0218 007d  .|.d...}.|.|...}
+000006f0: 0374 057c 0383 017d 047c 0473 6364 0464  .t.|...}.|.scd.d
+00000700: 0574 06a0 07a1 0076 0073 2474 08a0 0974  .t.....v.s$t...t
+00000710: 05a1 0172 2974 08a0 0a74 05a1 016e 0164  ...r)t...t...n.d
+00000720: 0564 0674 06a0 07a1 0076 0073 3574 08a0  .d.t.....v.s5t..
+00000730: 097c 00a1 0172 3a74 08a0 0a7c 00a1 016e  .|...r:t...|...n
+00000740: 0164 0664 0774 06a0 07a1 0076 0073 4674  .d.d.t.....v.sFt
+00000750: 08a0 0974 04a1 0172 4b74 08a0 0a74 04a1  ...t...rKt...t..
+00000760: 016e 0164 0774 08a0 0a7c 01a1 0174 08a0  .n.d.t...|...t..
+00000770: 0a7c 02a1 0174 08a0 0a7c 04a1 0164 089c  .|...t...|...d..
+00000780: 0616 007d 0574 0b74 08a0 0c7c 05a1 0183  ...}.t.t...|....
+00000790: 0182 0164 0004 007d 0104 007d 0204 007d  ...d...}...}...}
+000007a0: 037d 0464 027d 0174 047c 0164 038d 017d  .}.d.}.t.|.d...}
+000007b0: 027c 007c 0217 007d 0374 057c 0383 017d  .|.|...}.t.|...}
+000007c0: 047c 0473 c764 0964 0574 06a0 07a1 0076  .|.s.d.d.t.....v
+000007d0: 0073 8874 08a0 0974 05a1 0172 8d74 08a0  .s.t...t...r.t..
+000007e0: 0a74 05a1 016e 0164 0564 0674 06a0 07a1  .t...n.d.d.t....
+000007f0: 0076 0073 9974 08a0 097c 00a1 0172 9e74  .v.s.t...|...r.t
+00000800: 08a0 0a7c 00a1 016e 0164 0664 0774 06a0  ...|...n.d.d.t..
+00000810: 07a1 0076 0073 aa74 08a0 0974 04a1 0172  ...v.s.t...t...r
+00000820: af74 08a0 0a74 04a1 016e 0164 0774 08a0  .t...t...n.d.t..
+00000830: 0a7c 01a1 0174 08a0 0a7c 02a1 0174 08a0  .|...t...|...t..
+00000840: 0a7c 04a1 0164 089c 0616 007d 0574 0b74  .|...d.....}.t.t
+00000850: 08a0 0c7c 05a1 0183 0182 0164 0004 007d  ...|.......d...}
+00000860: 0104 007d 0204 007d 037d 0464 0a7d 0174  ...}...}.}.d.}.t
+00000870: 047c 0164 038d 017d 027c 007c 0218 007d  .|.d...}.|.|...}
+00000880: 0374 057c 0383 017d 047c 040c 007d 067c  .t.|...}.|...}.|
+00000890: 0690 0173 3364 0b64 0574 06a0 07a1 0076  ...s3d.d.t.....v
+000008a0: 0073 f074 08a0 0974 05a1 0172 f574 08a0  .s.t...t...r.t..
+000008b0: 0a74 05a1 016e 0164 0564 0674 06a0 07a1  .t...n.d.d.t....
+000008c0: 0076 0090 0173 0374 08a0 097c 00a1 0190  .v...s.t...|....
+000008d0: 0172 0874 08a0 0a7c 00a1 016e 0164 0664  .r.t...|...n.d.d
+000008e0: 0774 06a0 07a1 0076 0090 0173 1674 08a0  .t.....v...s.t..
+000008f0: 0974 04a1 0190 0172 1b74 08a0 0a74 04a1  .t.....r.t...t..
+00000900: 016e 0164 0774 08a0 0a7c 01a1 0174 08a0  .n.d.t...|...t..
+00000910: 0a7c 02a1 0174 08a0 0a7c 04a1 0164 089c  .|...t...|...d..
+00000920: 0616 007d 0774 0b74 08a0 0c7c 07a1 0183  ...}.t.t...|....
+00000930: 0182 0164 0004 007d 0104 007d 0204 007d  ...d...}...}...}
+00000940: 0304 007d 047d 0664 0a7d 0174 047c 0164  ...}.}.d.}.t.|.d
+00000950: 038d 017d 027c 007c 0217 007d 0374 057c  ...}.|.|...}.t.|
+00000960: 0383 017d 047c 040c 007d 067c 0690 0173  ...}.|...}.|...s
+00000970: a364 0c64 0574 06a0 07a1 0076 0090 0173  .d.d.t.....v...s
+00000980: 6074 08a0 0974 05a1 0190 0172 6574 08a0  `t...t.....ret..
+00000990: 0a74 05a1 016e 0164 0564 0674 06a0 07a1  .t...n.d.d.t....
+000009a0: 0076 0090 0173 7374 08a0 097c 00a1 0190  .v...sst...|....
+000009b0: 0172 7874 08a0 0a7c 00a1 016e 0164 0664  .rxt...|...n.d.d
+000009c0: 0774 06a0 07a1 0076 0090 0173 8674 08a0  .t.....v...s.t..
+000009d0: 0974 04a1 0190 0172 8b74 08a0 0a74 04a1  .t.....r.t...t..
+000009e0: 016e 0164 0774 08a0 0a7c 01a1 0174 08a0  .n.d.t...|...t..
+000009f0: 0a7c 02a1 0174 08a0 0a7c 04a1 0164 089c  .|...t...|...d..
+00000a00: 0616 007d 0774 0b74 08a0 0c7c 07a1 0183  ...}.t.t...|....
+00000a10: 0182 0164 0004 007d 0104 007d 0204 007d  ...d...}...}...}
+00000a20: 0304 007d 047d 0664 0053 0029 0d4e 721f  ...}.}.d.S.).Nr.
+00000a30: 0000 00e9 0400 0000 2901 da07 6d69 6e75  ........)...minu
+00000a40: 7465 737a 5e61 7373 6572 7420 2528 7079  tesz^assert %(py
+00000a50: 3929 730a 7b25 2870 7939 2973 203d 2025  9)s.{%(py9)s = %
+00000a60: 2870 7930 2973 2828 2528 7079 3129 7320  (py0)s((%(py1)s 
+00000a70: 2d20 2528 7079 3629 730a 7b25 2870 7936  - %(py6)s.{%(py6
+00000a80: 2973 203d 2025 2870 7932 2973 286d 696e  )s = %(py2)s(min
+00000a90: 7574 6573 3d25 2870 7934 2973 290a 7d29  utes=%(py4)s).})
+00000aa0: 290a 7d72 0600 0000 7223 0000 0072 0300  ).}r....r#...r..
+00000ab0: 0000 2906 7224 0000 0072 0d00 0000 7225  ..).r$...r....r%
+00000ac0: 0000 0072 2600 0000 da03 7079 36da 0370  ...r&.....py6..p
+00000ad0: 7939 7a5e 6173 7365 7274 2025 2870 7939  y9z^assert %(py9
+00000ae0: 2973 0a7b 2528 7079 3929 7320 3d20 2528  )s.{%(py9)s = %(
+00000af0: 7079 3029 7328 2825 2870 7931 2973 202b  py0)s((%(py1)s +
+00000b00: 2025 2870 7936 2973 0a7b 2528 7079 3629   %(py6)s.{%(py6)
+00000b10: 7320 3d20 2528 7079 3229 7328 6d69 6e75  s = %(py2)s(minu
+00000b20: 7465 733d 2528 7079 3429 7329 0a7d 2929  tes=%(py4)s).}))
+00000b30: 0a7d e906 0000 007a 6261 7373 6572 7420  .}.....zbassert 
+00000b40: 6e6f 7420 2528 7079 3929 730a 7b25 2870  not %(py9)s.{%(p
+00000b50: 7939 2973 203d 2025 2870 7930 2973 2828  y9)s = %(py0)s((
+00000b60: 2528 7079 3129 7320 2d20 2528 7079 3629  %(py1)s - %(py6)
+00000b70: 730a 7b25 2870 7936 2973 203d 2025 2870  s.{%(py6)s = %(p
+00000b80: 7932 2973 286d 696e 7574 6573 3d25 2870  y2)s(minutes=%(p
+00000b90: 7934 2973 290a 7d29 290a 7d7a 6261 7373  y4)s).})).}zbass
+00000ba0: 6572 7420 6e6f 7420 2528 7079 3929 730a  ert not %(py9)s.
+00000bb0: 7b25 2870 7939 2973 203d 2025 2870 7930  {%(py9)s = %(py0
+00000bc0: 2973 2828 2528 7079 3129 7320 2b20 2528  )s((%(py1)s + %(
+00000bd0: 7079 3629 730a 7b25 2870 7936 2973 203d  py6)s.{%(py6)s =
+00000be0: 2025 2870 7932 2973 286d 696e 7574 6573   %(py2)s(minutes
+00000bf0: 3d25 2870 7934 2973 290a 7d29 290a 7d29  =%(py4)s).})).})
+00000c00: 0d72 0200 0000 7223 0000 0072 0400 0000  .r....r#...r....
+00000c10: 722c 0000 0072 0300 0000 7206 0000 0072  r,...r....r....r
+00000c20: 1300 0000 7214 0000 0072 1000 0000 7215  ....r....r....r.
+00000c30: 0000 0072 1200 0000 7216 0000 0072 1700  ...r....r....r..
+00000c40: 0000 2908 7223 0000 00da 0b40 7079 5f61  ..).r#.....@py_a
+00000c50: 7373 6572 7433 da0b 4070 795f 6173 7365  ssert3..@py_asse
+00000c60: 7274 35da 0b40 7079 5f61 7373 6572 7437  rt5..@py_assert7
+00000c70: 7232 0000 00da 0c40 7079 5f66 6f72 6d61  r2.....@py_forma
+00000c80: 7431 305a 0c40 7079 5f61 7373 6572 7431  t10Z.@py_assert1
+00000c90: 3072 3400 0000 721c 0000 0072 1c00 0000  0r4...r....r....
+00000ca0: 721d 0000 00da 1974 6573 745f 6368 6563  r......test_chec
+00000cb0: 6b5f 6d61 785f 6f66 6673 6574 5f6e 6f77  k_max_offset_now
+00000cc0: 1600 0000 730a 0000 000e 01c8 02c8 01dc  ....s...........
+00000cd0: 01e4 0172 3f00 0000 2902 7209 0000 004e  ...r?...).r....N
+00000ce0: 2910 da08 6275 696c 7469 6e73 7213 0000  )...builtinsr...
+00000cf0: 00da 195f 7079 7465 7374 2e61 7373 6572  ..._pytest.asser
+00000d00: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
+00000d10: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
+00000d20: 7210 0000 0072 0200 0000 7203 0000 0072  r....r....r....r
+00000d30: 0400 0000 da04 6461 7465 7206 0000 0072  ......dater....r
+00000d40: 0700 0000 7208 0000 0072 1e00 0000 7235  ....r....r....r5
+00000d50: 0000 0072 3f00 0000 721c 0000 0072 1c00  ...r?...r....r..
+00000d60: 0000 721c 0000 0072 1d00 0000 da08 3c6d  ..r....r......<m
+00000d70: 6f64 756c 653e 0100 0000 730a 0000 002e  odule>....s.....
+00000d80: 0014 020a 030a 060e 0a                   .........
```

### Comparing `bovine-0.1.2/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 c401 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 c401 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1670 6172 7365 5f66 6564 6976 6572 7365  .parse_fediverse
```

### Comparing `bovine-0.1.2/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 191 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 bf00 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 bf00 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1777 6562 6669 6e67 6572 5f72 6573 706f  .webfinger_respo
```

### Comparing `bovine-0.1.2/bovine/utils/date.py` & `bovine-0.1.3/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.2/bovine/utils/msg/__init__.py` & `bovine-0.1.3/bovine/utils/msg/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import aiohttp
+
 from bovine import BovineClient
 from bovine.clients import lookup_account_with_webfinger
 
 from .validation import validate_tos
 
 
 def validate(args):
@@ -10,15 +12,15 @@
         exit(1)
 
     if len(args.to) == 0 and not args.public:
         print("Specify at least one recipient")
         exit(1)
 
 
-async def resolve(session, to):
+async def resolve(session: aiohttp.ClientSession, to: str) -> str:
     if "@" in to:
         return await lookup_account_with_webfinger(session, to)
 
     return to
 
 
 async def process(args):
```

### Comparing `bovine-0.1.2/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.3/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 1159 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,113 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 8704 0000  o.........Ad....
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 ba04 0000  o.......*.Nd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6405 6406 8400 5a06 6407 6408 8400  ..d.d...Z.d.d...
-00000060: 5a07 6409 640a 8400 5a08 640b 5300 290c  Z.d.d...Z.d.S.).
-00000070: e900 0000 0029 01da 0c42 6f76 696e 6543  .....)...BovineC
-00000080: 6c69 656e 74a9 01da 1d6c 6f6f 6b75 705f  lient....lookup_
-00000090: 6163 636f 756e 745f 7769 7468 5f77 6562  account_with_web
-000000a0: 6669 6e67 6572 e901 0000 0029 01da 0c76  finger.....)...v
-000000b0: 616c 6964 6174 655f 746f 7363 0100 0000  alidate_tosc....
-000000c0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000000d0: 4300 0000 734a 0000 0074 007c 006a 0183  C...sJ...t.|.j..
-000000e0: 0173 0d74 0264 0183 0101 0074 0364 0283  .s.t.d.....t.d..
-000000f0: 0101 0074 047c 006a 0183 0164 036b 0272  ...t.|.j...d.k.r
-00000100: 217c 006a 0573 2374 0264 0483 0101 0074  !|.j.s#t.d.....t
-00000110: 0364 0283 0101 0064 0053 0064 0053 0064  .d.....d.S.d.S.d
-00000120: 0053 0029 054e 7a12 496e 7661 6c69 6420  .S.).Nz.Invalid 
-00000130: 7265 6369 7069 656e 7473 7205 0000 0072  recipientsr....r
-00000140: 0100 0000 7a1e 5370 6563 6966 7920 6174  ....z.Specify at
-00000150: 206c 6561 7374 206f 6e65 2072 6563 6970   least one recip
-00000160: 6965 6e74 2906 7206 0000 00da 0274 6fda  ient).r......to.
-00000170: 0570 7269 6e74 da04 6578 6974 da03 6c65  .print..exit..le
-00000180: 6eda 0670 7562 6c69 6329 01da 0461 7267  n..public)...arg
-00000190: 73a9 0072 0d00 0000 fa4e 2f77 6f6f 6470  s..r.....N/woodp
-000001a0: 6563 6b65 722f 7372 632f 636f 6465 6265  ecker/src/codebe
-000001b0: 7267 2e6f 7267 2f62 6f76 696e 652f 626f  rg.org/bovine/bo
-000001c0: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
-000001d0: 6e65 2f75 7469 6c73 2f6d 7367 2f5f 5f69  ne/utils/msg/__i
-000001e0: 6e69 745f 5f2e 7079 da08 7661 6c69 6461  nit__.py..valida
-000001f0: 7465 0700 0000 730e 0000 000a 0108 0108  te....s.........
-00000200: 0114 0208 010c 0108 fe72 0f00 0000 6302  .........r....c.
-00000210: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000220: 0000 00c3 0000 0073 1e00 0000 8101 6401  .......s......d.
-00000230: 7c01 7600 720d 7400 7c00 7c01 8302 4900  |.v.r.t.|.|...I.
-00000240: 6400 4800 5300 7c01 5300 2902 4efa 0140  d.H.S.|.S.).N..@
-00000250: 7203 0000 0029 02da 0773 6573 7369 6f6e  r....)...session
-00000260: 7207 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000270: 0e00 0000 da07 7265 736f 6c76 6511 0000  ......resolve...
-00000280: 0073 0800 0000 0280 0801 1001 0402 7212  .s............r.
-00000290: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000002a0: 0500 0000 0900 0000 8300 0000 73d8 0000  ............s...
-000002b0: 0081 0174 007c 006a 017c 006a 0264 019c  ...t.|.j.|.j.d..
-000002c0: 0283 0134 0049 0064 0048 009a 5189 0087  ...4.I.d.H..Q...
-000002d0: 0066 0164 0264 0384 087c 006a 0344 0083  .f.d.d...|.j.D..
-000002e0: 0149 0064 0048 007d 0187 0066 0164 0464  .I.d.H.}...f.d.d
-000002f0: 0384 087c 0144 0083 0149 0064 0048 007d  ...|.D...I.d.H.}
-00000300: 0264 0564 0384 007c 0244 0083 017d 0288  .d.d...|.D...}..
-00000310: 006a 046a 0574 067c 0183 017c 027c 006a  .j.j.t.|...|.|.j
-00000320: 0764 068d 037d 037c 006a 0872 427c 03a0  .d...}.|.j.rB|..
-00000330: 09a1 007d 0388 006a 0aa0 0b7c 03a0 0ca1  ...}...j...|....
-00000340: 00a1 01a0 0ca1 007d 0488 00a0 0d7c 04a1  .......}.....|..
-00000350: 0149 0064 0048 0001 0057 0064 0004 0004  .I.d.H...W.d....
-00000360: 0083 0349 0064 0048 0001 0064 0053 0031  ...I.d.H...d.S.1
-00000370: 0049 0064 0048 0073 6577 0101 0001 0001  .I.d.H.sew......
-00000380: 0059 0001 0064 0053 0029 074e 2902 da04  .Y...d.S.).N)...
-00000390: 686f 7374 da0b 7072 6976 6174 655f 6b65  host..private_ke
-000003a0: 7963 0100 0000 0000 0000 0000 0000 0200  yc..............
-000003b0: 0000 0500 0000 9300 0000 7320 0000 0081  ..........s ....
-000003c0: 0167 007c 005d 0b7d 0174 0088 006a 017c  .g.|.].}.t...j.|
-000003d0: 0183 0249 0064 0048 0091 0271 0353 00a9  ...I.d.H...q.S..
-000003e0: 014e 2902 7212 0000 0072 1100 0000 2902  .N).r....r....).
-000003f0: da02 2e30 7207 0000 00a9 01da 0663 6c69  ...0r........cli
-00000400: 656e 7472 0d00 0000 720e 0000 00da 0a3c  entr....r......<
-00000410: 6c69 7374 636f 6d70 3e1a 0000 0073 0400  listcomp>....s..
-00000420: 0000 0280 1e00 7a1b 7072 6f63 6573 732e  ......z.process.
-00000430: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000440: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-00000450: 0200 0000 0500 0000 9300 0000 7320 0000  ............s ..
-00000460: 0081 0167 007c 005d 0b7d 0188 006a 00a0  ...g.|.].}...j..
-00000470: 017c 01a1 0149 0064 0048 0091 0271 0353  .|...I.d.H...q.S
-00000480: 0072 1500 0000 2902 da0e 6f62 6a65 6374  .r....)...object
-00000490: 5f66 6163 746f 7279 da15 6d65 6e74 696f  _factory..mentio
-000004a0: 6e5f 666f 725f 6163 746f 725f 7572 6929  n_for_actor_uri)
-000004b0: 0272 1600 0000 5a09 7265 6369 7069 656e  .r....Z.recipien
-000004c0: 7472 1700 0000 720d 0000 0072 0e00 0000  tr....r....r....
-000004d0: 7219 0000 001c 0000 0073 0a00 0000 0280  r........s......
-000004e0: 0600 0202 10ff 06ff 6301 0000 0000 0000  ........c.......
-000004f0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00000500: 0073 1400 0000 6700 7c00 5d06 7d01 7c01  .s....g.|.].}.|.
-00000510: a000 a100 9102 7102 5300 720d 0000 0029  ......q.S.r....)
-00000520: 01da 0562 7569 6c64 2902 7216 0000 00da  ...build).r.....
-00000530: 016d 720d 0000 0072 0d00 0000 720e 0000  .mr....r....r...
-00000540: 0072 1900 0000 2000 0000 7302 0000 0014  .r.... ...s.....
-00000550: 0029 0372 0700 0000 da03 7461 67da 0763  .).r......tag..c
-00000560: 6f6e 7465 6e74 290e 7202 0000 0072 1300  ontent).r....r..
-00000570: 0000 da06 7365 6372 6574 7207 0000 0072  ....secretr....r
-00000580: 1a00 0000 da04 6e6f 7465 da03 7365 74da  ......note..set.
-00000590: 076d 6573 7361 6765 720b 0000 00da 0961  .messager......a
-000005a0: 735f 7075 626c 6963 da10 6163 7469 7669  s_public..activi
-000005b0: 7479 5f66 6163 746f 7279 da06 6372 6561  ty_factory..crea
-000005c0: 7465 721c 0000 00da 0e73 656e 645f 746f  ter......send_to
-000005d0: 5f6f 7574 626f 7829 0572 0c00 0000 da0a  _outbox).r......
-000005e0: 7265 6369 7069 656e 7473 5a08 6d65 6e74  recipientsZ.ment
-000005f0: 696f 6e73 7221 0000 0072 2600 0000 720d  ionsr!...r&...r.
-00000600: 0000 0072 1700 0000 720e 0000 00da 0770  ...r....r......p
-00000610: 726f 6365 7373 1800 0000 731e 0000 0002  rocess....s.....
-00000620: 801c 011a 010a 0202 020c fe0e 0406 020c  ................
-00000630: 0106 ff06 0408 0114 0212 022e ee72 2900  .............r).
-00000640: 0000 4e29 09da 0662 6f76 696e 6572 0200  ..N)...boviner..
-00000650: 0000 da0e 626f 7669 6e65 2e63 6c69 656e  ....bovine.clien
-00000660: 7473 7204 0000 00da 0a76 616c 6964 6174  tsr......validat
-00000670: 696f 6e72 0600 0000 720f 0000 0072 1200  ionr....r....r..
-00000680: 0000 7229 0000 0072 0d00 0000 720d 0000  ..r)...r....r...
-00000690: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
-000006a0: 6475 6c65 3e01 0000 0073 0c00 0000 0c00  dule>....s......
-000006b0: 0c01 0c02 0803 080a 0c07                 ..........
+00000020: 0006 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
+00000050: 6405 6c05 6d06 5a06 0100 6406 6407 8400  d.l.m.Z...d.d...
+00000060: 5a07 6408 6500 6a08 6409 6509 640a 6509  Z.d.e.j.d.e.d.e.
+00000070: 6606 640b 640c 8404 5a0a 640d 640e 8400  f.d.d...Z.d.d...
+00000080: 5a0b 6401 5300 290f e900 0000 004e 2901  Z.d.S.)......N).
+00000090: da0c 426f 7669 6e65 436c 6965 6e74 a901  ..BovineClient..
+000000a0: da1d 6c6f 6f6b 7570 5f61 6363 6f75 6e74  ..lookup_account
+000000b0: 5f77 6974 685f 7765 6266 696e 6765 72e9  _with_webfinger.
+000000c0: 0100 0000 2901 da0c 7661 6c69 6461 7465  ....)...validate
+000000d0: 5f74 6f73 6301 0000 0000 0000 0000 0000  _tosc...........
+000000e0: 0001 0000 0002 0000 0043 0000 0073 4a00  .........C...sJ.
+000000f0: 0000 7400 7c00 6a01 8301 730d 7402 6401  ..t.|.j...s.t.d.
+00000100: 8301 0100 7403 6402 8301 0100 7404 7c00  ....t.d.....t.|.
+00000110: 6a01 8301 6403 6b02 7221 7c00 6a05 7323  j...d.k.r!|.j.s#
+00000120: 7402 6404 8301 0100 7403 6402 8301 0100  t.d.....t.d.....
+00000130: 6400 5300 6400 5300 6400 5300 2905 4e7a  d.S.d.S.d.S.).Nz
+00000140: 1249 6e76 616c 6964 2072 6563 6970 6965  .Invalid recipie
+00000150: 6e74 7372 0500 0000 7201 0000 007a 1e53  ntsr....r....z.S
+00000160: 7065 6369 6679 2061 7420 6c65 6173 7420  pecify at least 
+00000170: 6f6e 6520 7265 6369 7069 656e 7429 0672  one recipient).r
+00000180: 0600 0000 da02 746f da05 7072 696e 74da  ......to..print.
+00000190: 0465 7869 74da 036c 656e da06 7075 626c  .exit..len..publ
+000001a0: 6963 2901 da04 6172 6773 a900 720d 0000  ic)...args..r...
+000001b0: 00fa 4e2f 776f 6f64 7065 636b 6572 2f73  ..N/woodpecker/s
+000001c0: 7263 2f63 6f64 6562 6572 672e 6f72 672f  rc/codeberg.org/
+000001d0: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
+000001e0: 7669 6e65 2f62 6f76 696e 652f 7574 696c  vine/bovine/util
+000001f0: 732f 6d73 672f 5f5f 696e 6974 5f5f 2e70  s/msg/__init__.p
+00000200: 79da 0876 616c 6964 6174 6509 0000 0073  y..validate....s
+00000210: 0e00 0000 0a01 0801 0801 1402 0801 0c01  ................
+00000220: 08fe 720f 0000 00da 0773 6573 7369 6f6e  ..r......session
+00000230: 7207 0000 00da 0672 6574 7572 6e63 0200  r......returnc..
+00000240: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000250: 0000 c300 0000 731e 0000 0081 0164 017c  ......s......d.|
+00000260: 0176 0072 0d74 007c 007c 0183 0249 0064  .v.r.t.|.|...I.d
+00000270: 0048 0053 007c 0153 0029 024e fa01 4072  .H.S.|.S.).N..@r
+00000280: 0300 0000 2902 7210 0000 0072 0700 0000  ....).r....r....
+00000290: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+000002a0: 0772 6573 6f6c 7665 1300 0000 7308 0000  .resolve....s...
+000002b0: 0002 8008 0110 0104 0272 1300 0000 6301  .........r....c.
+000002c0: 0000 0000 0000 0000 0000 0005 0000 0009  ................
+000002d0: 0000 0083 0000 0073 d800 0000 8101 7400  .......s......t.
+000002e0: 7c00 6a01 7c00 6a02 6401 9c02 8301 3400  |.j.|.j.d.....4.
+000002f0: 4900 6400 4800 9a51 8900 8700 6601 6402  I.d.H..Q....f.d.
+00000300: 6403 8408 7c00 6a03 4400 8301 4900 6400  d...|.j.D...I.d.
+00000310: 4800 7d01 8700 6601 6404 6403 8408 7c01  H.}...f.d.d...|.
+00000320: 4400 8301 4900 6400 4800 7d02 6405 6403  D...I.d.H.}.d.d.
+00000330: 8400 7c02 4400 8301 7d02 8800 6a04 6a05  ..|.D...}...j.j.
+00000340: 7406 7c01 8301 7c02 7c00 6a07 6406 8d03  t.|...|.|.j.d...
+00000350: 7d03 7c00 6a08 7242 7c03 a009 a100 7d03  }.|.j.rB|.....}.
+00000360: 8800 6a0a a00b 7c03 a00c a100 a101 a00c  ..j...|.........
+00000370: a100 7d04 8800 a00d 7c04 a101 4900 6400  ..}.....|...I.d.
+00000380: 4800 0100 5700 6400 0400 0400 8303 4900  H...W.d.......I.
+00000390: 6400 4800 0100 6400 5300 3100 4900 6400  d.H...d.S.1.I.d.
+000003a0: 4800 7365 7701 0100 0100 0100 5900 0100  H.sew.......Y...
+000003b0: 6400 5300 2907 4e29 02da 0468 6f73 74da  d.S.).N)...host.
+000003c0: 0b70 7269 7661 7465 5f6b 6579 6301 0000  .private_keyc...
+000003d0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+000003e0: 0093 0000 0073 2000 0000 8101 6700 7c00  .....s .....g.|.
+000003f0: 5d0b 7d01 7400 8800 6a01 7c01 8302 4900  ].}.t...j.|...I.
+00000400: 6400 4800 9102 7103 5300 a901 4e29 0272  d.H...q.S...N).r
+00000410: 1300 0000 7210 0000 0029 02da 022e 3072  ....r....)....0r
+00000420: 0700 0000 a901 da06 636c 6965 6e74 720d  ........clientr.
+00000430: 0000 0072 0e00 0000 da0a 3c6c 6973 7463  ...r......<listc
+00000440: 6f6d 703e 1c00 0000 7304 0000 0002 801e  omp>....s.......
+00000450: 007a 1b70 726f 6365 7373 2e3c 6c6f 6361  .z.process.<loca
+00000460: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
+00000470: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00000480: 0000 0093 0000 0073 2000 0000 8101 6700  .......s .....g.
+00000490: 7c00 5d0b 7d01 8800 6a00 a001 7c01 a101  |.].}...j...|...
+000004a0: 4900 6400 4800 9102 7103 5300 7216 0000  I.d.H...q.S.r...
+000004b0: 0029 02da 0e6f 626a 6563 745f 6661 6374  .)...object_fact
+000004c0: 6f72 79da 156d 656e 7469 6f6e 5f66 6f72  ory..mention_for
+000004d0: 5f61 6374 6f72 5f75 7269 2902 7217 0000  _actor_uri).r...
+000004e0: 005a 0972 6563 6970 6965 6e74 7218 0000  .Z.recipientr...
+000004f0: 0072 0d00 0000 720e 0000 0072 1a00 0000  .r....r....r....
+00000500: 1e00 0000 730a 0000 0002 8006 0002 0210  ....s...........
+00000510: ff06 ff63 0100 0000 0000 0000 0000 0000  ...c............
+00000520: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
+00000530: 0067 007c 005d 067d 017c 01a0 00a1 0091  .g.|.].}.|......
+00000540: 0271 0253 0072 0d00 0000 2901 da05 6275  .q.S.r....)...bu
+00000550: 696c 6429 0272 1700 0000 da01 6d72 0d00  ild).r......mr..
+00000560: 0000 720d 0000 0072 0e00 0000 721a 0000  ..r....r....r...
+00000570: 0022 0000 0073 0200 0000 1400 2903 7207  ."...s......).r.
+00000580: 0000 00da 0374 6167 da07 636f 6e74 656e  .....tag..conten
+00000590: 7429 0e72 0200 0000 7214 0000 00da 0673  t).r....r......s
+000005a0: 6563 7265 7472 0700 0000 721b 0000 00da  ecretr....r.....
+000005b0: 046e 6f74 65da 0373 6574 da07 6d65 7373  .note..set..mess
+000005c0: 6167 6572 0b00 0000 da09 6173 5f70 7562  ager......as_pub
+000005d0: 6c69 63da 1061 6374 6976 6974 795f 6661  lic..activity_fa
+000005e0: 6374 6f72 79da 0663 7265 6174 6572 1d00  ctory..creater..
+000005f0: 0000 da0e 7365 6e64 5f74 6f5f 6f75 7462  ....send_to_outb
+00000600: 6f78 2905 720c 0000 00da 0a72 6563 6970  ox).r......recip
+00000610: 6965 6e74 735a 086d 656e 7469 6f6e 7372  ientsZ.mentionsr
+00000620: 2200 0000 7227 0000 0072 0d00 0000 7218  "...r'...r....r.
+00000630: 0000 0072 0e00 0000 da07 7072 6f63 6573  ...r......proces
+00000640: 731a 0000 0073 1e00 0000 0280 1c01 1a01  s....s..........
+00000650: 0a02 0202 0cfe 0e04 0602 0c01 06ff 0604  ................
+00000660: 0801 1402 1202 2eee 722a 0000 0029 0cda  ........r*...)..
+00000670: 0761 696f 6874 7470 da06 626f 7669 6e65  .aiohttp..bovine
+00000680: 7202 0000 00da 0e62 6f76 696e 652e 636c  r......bovine.cl
+00000690: 6965 6e74 7372 0400 0000 da0a 7661 6c69  ientsr......vali
+000006a0: 6461 7469 6f6e 7206 0000 0072 0f00 0000  dationr....r....
+000006b0: da0d 436c 6965 6e74 5365 7373 696f 6eda  ..ClientSession.
+000006c0: 0373 7472 7213 0000 0072 2a00 0000 720d  .strr....r*...r.
+000006d0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+000006e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000006f0: 730e 0000 0008 000c 020c 010c 0208 0318  s...............
+00000700: 0a0c 07                                  ...
```

### Comparing `bovine-0.1.2/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.3/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:27:12 2023 UTC, .py size: 557 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,121 +1,123 @@
-00000000: 6f0d 0d0a 0000 0000 8013 4164 2d02 0000  o.........Ad-...
+00000000: 6f0d 0d0a 0000 0000 2a9f 4e64 5702 0000  o.......*.NdW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
+00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
-00000060: 6404 6405 8400 5a0a 6406 6407 8400 5a0b  d.d...Z.d.d...Z.
-00000070: 6506 6a0c a00d 6408 6409 640a 6702 a102  e.j...d.d.d.g...
-00000080: 640b 640c 8400 8301 5a0e 6506 6a0c a00d  d.d.....Z.e.j...
-00000090: 6408 640d 640e 6702 a102 640f 6410 8400  d.d.d.g...d.d...
-000000a0: 8301 5a0f 6401 5300 2911 e900 0000 004e  ..Z.d.S.)......N
-000000b0: e901 0000 0029 02da 0b76 616c 6964 6174  .....)...validat
-000000c0: 655f 746f da0c 7661 6c69 6461 7465 5f74  e_to..validate_t
-000000d0: 6f73 6300 0000 0000 0000 0000 0000 0003  osc.............
-000000e0: 0000 0006 0000 0043 0000 0073 6600 0000  .......C...sf...
-000000f0: 6400 7d00 7400 7c00 8301 7d01 7c01 732d  d.}.t.|...}.|.s-
-00000100: 6401 6402 7401 a002 a100 7600 7314 7403  d.d.t.....v.s.t.
-00000110: a004 7400 a101 7219 7403 a005 7400 a101  ..t...r.t...t...
-00000120: 6e01 6402 7403 a005 7c00 a101 7403 a005  n.d.t...|...t...
-00000130: 7c01 a101 6403 9c03 1600 7d02 7406 7403  |...d.....}.t.t.
-00000140: a007 7c02 a101 8301 8201 6400 0400 7d00  ..|.......d...}.
-00000150: 7d01 6400 5300 2904 4efa 2c61 7373 6572  }.d.S.).N.,asser
-00000160: 7420 2528 7079 3429 730a 7b25 2870 7934  t %(py4)s.{%(py4
-00000170: 2973 203d 2025 2870 7930 2973 2825 2870  )s = %(py0)s(%(p
-00000180: 7932 2973 290a 7d72 0400 0000 a903 da03  y2)s).}r........
-00000190: 7079 30da 0370 7932 da03 7079 34a9 0872  py0..py2..py4..r
-000001a0: 0400 0000 da0c 4070 795f 6275 696c 7469  ......@py_builti
-000001b0: 6e73 da06 6c6f 6361 6c73 da0a 4070 7974  ns..locals..@pyt
-000001c0: 6573 745f 6172 da18 5f73 686f 756c 645f  est_ar.._should_
-000001d0: 7265 7072 5f67 6c6f 6261 6c5f 6e61 6d65  repr_global_name
-000001e0: da09 5f73 6166 6572 6570 72da 0e41 7373  .._saferepr..Ass
-000001f0: 6572 7469 6f6e 4572 726f 72da 135f 666f  ertionError.._fo
-00000200: 726d 6174 5f65 7870 6c61 6e61 7469 6f6e  rmat_explanation
-00000210: a903 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
-00000220: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
-00000230: 795f 666f 726d 6174 35a9 0072 1600 0000  y_format5..r....
-00000240: fa55 2f77 6f6f 6470 6563 6b65 722f 7372  .U/woodpecker/sr
-00000250: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
-00000260: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-00000270: 696e 652f 626f 7669 6e65 2f75 7469 6c73  ine/bovine/utils
-00000280: 2f6d 7367 2f74 6573 745f 7661 6c69 6461  /msg/test_valida
-00000290: 7469 6f6e 2e70 79da 1674 6573 745f 7661  tion.py..test_va
-000002a0: 6c69 6461 7465 5f74 6f73 5f6e 6f6e 6506  lidate_tos_none.
-000002b0: 0000 0073 0200 0000 6601 7218 0000 0063  ...s....f.r....c
-000002c0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000002d0: 0600 0000 4300 0000 7368 0000 0064 0167  ....C...sh...d.g
-000002e0: 017d 0074 007c 0083 017d 017c 0173 2e64  .}.t.|...}.|.s.d
-000002f0: 0264 0374 01a0 02a1 0076 0073 1574 03a0  .d.t.....v.s.t..
-00000300: 0474 00a1 0172 1a74 03a0 0574 00a1 016e  .t...r.t...t...n
-00000310: 0164 0374 03a0 057c 00a1 0174 03a0 057c  .d.t...|...t...|
-00000320: 01a1 0164 049c 0316 007d 0274 0674 03a0  ...d.....}.t.t..
-00000330: 077c 02a1 0183 0182 0164 0004 007d 007d  .|.......d...}.}
-00000340: 0164 0053 0029 054e 7a0e 616c 7973 7373  .d.S.).Nz.alysss
-00000350: 6140 6265 6e2e 6465 7205 0000 0072 0400  a@ben.der....r..
-00000360: 0000 7206 0000 0072 0a00 0000 7212 0000  ..r....r....r...
-00000370: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000380: da11 7465 7374 5f76 616c 6964 6174 655f  ..test_validate_
-00000390: 746f 730a 0000 0073 0200 0000 6801 7219  tos....s....h.r.
-000003a0: 0000 00da 0972 6563 6970 6965 6e74 7a21  .....recipientz!
-000003b0: 6874 7470 733a 2f2f 6368 6174 7479 2e65  https://chatty.e
-000003c0: 7861 6d70 6c65 2e63 6f6d 2f61 6c79 7373  xample.com/alyss
-000003d0: 617a 1161 6c79 7373 6140 6368 6174 7479  az.alyssa@chatty
-000003e0: 2e63 6f6d 6301 0000 0000 0000 0000 0000  .comc...........
-000003f0: 0003 0000 0006 0000 0043 0000 0073 7800  .........C...sx.
-00000400: 0000 7400 7c00 8301 7d01 7c01 7338 6401  ..t.|...}.|.s8d.
-00000410: 6402 7401 a002 a100 7600 7312 7403 a004  d.t.....v.s.t...
-00000420: 7400 a101 7217 7403 a005 7400 a101 6e01  t...r.t...t...n.
-00000430: 6402 6403 7401 a002 a100 7600 7323 7403  d.d.t.....v.s#t.
-00000440: a004 7c00 a101 7228 7403 a005 7c00 a101  ..|...r(t...|...
-00000450: 6e01 6403 7403 a005 7c01 a101 6404 9c03  n.d.t...|...d...
-00000460: 1600 7d02 7406 7403 a007 7c02 a101 8301  ..}.t.t...|.....
-00000470: 8201 6400 7d01 6400 5300 2905 4e7a 2c61  ..d.}.d.S.).Nz,a
-00000480: 7373 6572 7420 2528 7079 3329 730a 7b25  ssert %(py3)s.{%
-00000490: 2870 7933 2973 203d 2025 2870 7930 2973  (py3)s = %(py0)s
-000004a0: 2825 2870 7931 2973 290a 7d72 0300 0000  (%(py1)s).}r....
-000004b0: 721a 0000 00a9 0372 0700 0000 da03 7079  r......r......py
-000004c0: 31da 0370 7933 a908 7203 0000 0072 0b00  1..py3..r....r..
-000004d0: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-000004e0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-000004f0: 2903 721a 0000 00da 0b40 7079 5f61 7373  ).r......@py_ass
-00000500: 6572 7432 da0b 4070 795f 666f 726d 6174  ert2..@py_format
-00000510: 3472 1600 0000 7216 0000 0072 1700 0000  4r....r....r....
-00000520: da15 7465 7374 5f76 616c 6964 6174 655f  ..test_validate_
-00000530: 746f 5f74 7275 650e 0000 0073 0200 0000  to_true....s....
-00000540: 7804 7221 0000 007a 2068 7474 703a 2f2f  x.r!...z http://
-00000550: 6368 6174 7479 2e65 7861 6d70 6c65 2e63  chatty.example.c
-00000560: 6f6d 2f61 6c79 7373 617a 1061 6c79 7373  om/alyssaz.alyss
-00000570: 6163 6861 7474 792e 636f 6d63 0100 0000  achatty.comc....
-00000580: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00000590: 4300 0000 7382 0000 0074 007c 0083 017d  C...s....t.|...}
-000005a0: 017c 010c 007d 027c 0273 3b64 0164 0274  .|...}.|.s;d.d.t
-000005b0: 01a0 02a1 0076 0073 1574 03a0 0474 00a1  .....v.s.t...t..
-000005c0: 0172 1a74 03a0 0574 00a1 016e 0164 0264  .r.t...t...n.d.d
-000005d0: 0374 01a0 02a1 0076 0073 2674 03a0 047c  .t.....v.s&t...|
-000005e0: 00a1 0172 2b74 03a0 057c 00a1 016e 0164  ...r+t...|...n.d
-000005f0: 0374 03a0 057c 01a1 0164 049c 0316 007d  .t...|...d.....}
-00000600: 0374 0674 03a0 077c 03a1 0183 0182 0164  .t.t...|.......d
-00000610: 0004 007d 017d 0264 0053 0029 054e 7a30  ...}.}.d.S.).Nz0
-00000620: 6173 7365 7274 206e 6f74 2025 2870 7933  assert not %(py3
-00000630: 2973 0a7b 2528 7079 3329 7320 3d20 2528  )s.{%(py3)s = %(
-00000640: 7079 3029 7328 2528 7079 3129 7329 0a7d  py0)s(%(py1)s).}
-00000650: 7203 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000660: 1e00 0000 2904 721a 0000 0072 1f00 0000  ....).r....r....
-00000670: da0b 4070 795f 6173 7365 7274 3472 1500  ..@py_assert4r..
-00000680: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000690: 00da 1674 6573 745f 7661 6c69 6461 7465  ...test_validate
-000006a0: 5f74 6f5f 6661 6c73 6515 0000 0073 0200  _to_false....s..
-000006b0: 0000 8204 7223 0000 0029 10da 0862 7569  ....r#...)...bui
-000006c0: 6c74 696e 7372 0b00 0000 da19 5f70 7974  ltinsr......_pyt
-000006d0: 6573 742e 6173 7365 7274 696f 6e2e 7265  est.assertion.re
-000006e0: 7772 6974 65da 0961 7373 6572 7469 6f6e  write..assertion
-000006f0: da07 7265 7772 6974 6572 0d00 0000 da06  ..rewriter......
-00000700: 7079 7465 7374 da0a 7661 6c69 6461 7469  pytest..validati
-00000710: 6f6e 7203 0000 0072 0400 0000 7218 0000  onr....r....r...
-00000720: 0072 1900 0000 da04 6d61 726b da0b 7061  .r......mark..pa
-00000730: 7261 6d65 7472 697a 6572 2100 0000 7223  rametrizer!...r#
-00000740: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-00000750: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000760: 3e01 0000 0073 1800 0000 2200 1002 0803  >....s....".....
-00000770: 0804 0604 0801 02ff 0a03 0604 0801 02ff  ................
-00000780: 0e03                                     ..
+00000060: 6412 6405 6406 8404 5a0a 6412 6407 6408  d.d.d...Z.d.d.d.
+00000070: 8404 5a0b 6506 6a0c a00d 6409 640a 640b  ..Z.e.j...d.d.d.
+00000080: 6702 a102 6409 650e 6404 6401 6604 640c  g...d.e.d.d.f.d.
+00000090: 640d 8404 8301 5a0f 6506 6a0c a00d 6409  d.....Z.e.j...d.
+000000a0: 640e 640f 6702 a102 6409 650e 6404 6401  d.d.g...d.e.d.d.
+000000b0: 6604 6410 6411 8404 8301 5a10 6401 5300  f.d.d.....Z.d.S.
+000000c0: 2913 e900 0000 004e e901 0000 0029 02da  )......N.....)..
+000000d0: 0b76 616c 6964 6174 655f 746f da0c 7661  .validate_to..va
+000000e0: 6c69 6461 7465 5f74 6f73 da06 7265 7475  lidate_tos..retu
+000000f0: 726e 6300 0000 0000 0000 0000 0000 0003  rnc.............
+00000100: 0000 0006 0000 0043 0000 0073 6600 0000  .......C...sf...
+00000110: 6400 7d00 7400 7c00 8301 7d01 7c01 732d  d.}.t.|...}.|.s-
+00000120: 6401 6402 7401 a002 a100 7600 7314 7403  d.d.t.....v.s.t.
+00000130: a004 7400 a101 7219 7403 a005 7400 a101  ..t...r.t...t...
+00000140: 6e01 6402 7403 a005 7c00 a101 7403 a005  n.d.t...|...t...
+00000150: 7c01 a101 6403 9c03 1600 7d02 7406 7403  |...d.....}.t.t.
+00000160: a007 7c02 a101 8301 8201 6400 0400 7d00  ..|.......d...}.
+00000170: 7d01 6400 5300 2904 4efa 2c61 7373 6572  }.d.S.).N.,asser
+00000180: 7420 2528 7079 3429 730a 7b25 2870 7934  t %(py4)s.{%(py4
+00000190: 2973 203d 2025 2870 7930 2973 2825 2870  )s = %(py0)s(%(p
+000001a0: 7932 2973 290a 7d72 0400 0000 a903 da03  y2)s).}r........
+000001b0: 7079 30da 0370 7932 da03 7079 34a9 0872  py0..py2..py4..r
+000001c0: 0400 0000 da0c 4070 795f 6275 696c 7469  ......@py_builti
+000001d0: 6e73 da06 6c6f 6361 6c73 da0a 4070 7974  ns..locals..@pyt
+000001e0: 6573 745f 6172 da18 5f73 686f 756c 645f  est_ar.._should_
+000001f0: 7265 7072 5f67 6c6f 6261 6c5f 6e61 6d65  repr_global_name
+00000200: da09 5f73 6166 6572 6570 72da 0e41 7373  .._saferepr..Ass
+00000210: 6572 7469 6f6e 4572 726f 72da 135f 666f  ertionError.._fo
+00000220: 726d 6174 5f65 7870 6c61 6e61 7469 6f6e  rmat_explanation
+00000230: a903 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
+00000240: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
+00000250: 795f 666f 726d 6174 35a9 0072 1700 0000  y_format5..r....
+00000260: fa55 2f77 6f6f 6470 6563 6b65 722f 7372  .U/woodpecker/sr
+00000270: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
+00000280: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
+00000290: 696e 652f 626f 7669 6e65 2f75 7469 6c73  ine/bovine/utils
+000002a0: 2f6d 7367 2f74 6573 745f 7661 6c69 6461  /msg/test_valida
+000002b0: 7469 6f6e 2e70 79da 1674 6573 745f 7661  tion.py..test_va
+000002c0: 6c69 6461 7465 5f74 6f73 5f6e 6f6e 6506  lidate_tos_none.
+000002d0: 0000 0073 0200 0000 6601 7219 0000 0063  ...s....f.r....c
+000002e0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000002f0: 0600 0000 4300 0000 7368 0000 0064 0167  ....C...sh...d.g
+00000300: 017d 0074 007c 0083 017d 017c 0173 2e64  .}.t.|...}.|.s.d
+00000310: 0264 0374 01a0 02a1 0076 0073 1574 03a0  .d.t.....v.s.t..
+00000320: 0474 00a1 0172 1a74 03a0 0574 00a1 016e  .t...r.t...t...n
+00000330: 0164 0374 03a0 057c 00a1 0174 03a0 057c  .d.t...|...t...|
+00000340: 01a1 0164 049c 0316 007d 0274 0674 03a0  ...d.....}.t.t..
+00000350: 077c 02a1 0183 0182 0164 0004 007d 007d  .|.......d...}.}
+00000360: 0164 0053 0029 054e 7a0e 616c 7973 7373  .d.S.).Nz.alysss
+00000370: 6140 6265 6e2e 6465 7206 0000 0072 0400  a@ben.der....r..
+00000380: 0000 7207 0000 0072 0b00 0000 7213 0000  ..r....r....r...
+00000390: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+000003a0: da11 7465 7374 5f76 616c 6964 6174 655f  ..test_validate_
+000003b0: 746f 730a 0000 0073 0200 0000 6801 721a  tos....s....h.r.
+000003c0: 0000 00da 0972 6563 6970 6965 6e74 7a21  .....recipientz!
+000003d0: 6874 7470 733a 2f2f 6368 6174 7479 2e65  https://chatty.e
+000003e0: 7861 6d70 6c65 2e63 6f6d 2f61 6c79 7373  xample.com/alyss
+000003f0: 617a 1161 6c79 7373 6140 6368 6174 7479  az.alyssa@chatty
+00000400: 2e63 6f6d 6301 0000 0000 0000 0000 0000  .comc...........
+00000410: 0003 0000 0006 0000 0043 0000 0073 7800  .........C...sx.
+00000420: 0000 7400 7c00 8301 7d01 7c01 7338 6401  ..t.|...}.|.s8d.
+00000430: 6402 7401 a002 a100 7600 7312 7403 a004  d.t.....v.s.t...
+00000440: 7400 a101 7217 7403 a005 7400 a101 6e01  t...r.t...t...n.
+00000450: 6402 6403 7401 a002 a100 7600 7323 7403  d.d.t.....v.s#t.
+00000460: a004 7c00 a101 7228 7403 a005 7c00 a101  ..|...r(t...|...
+00000470: 6e01 6403 7403 a005 7c01 a101 6404 9c03  n.d.t...|...d...
+00000480: 1600 7d02 7406 7403 a007 7c02 a101 8301  ..}.t.t...|.....
+00000490: 8201 6400 7d01 6400 5300 2905 4e7a 2c61  ..d.}.d.S.).Nz,a
+000004a0: 7373 6572 7420 2528 7079 3329 730a 7b25  ssert %(py3)s.{%
+000004b0: 2870 7933 2973 203d 2025 2870 7930 2973  (py3)s = %(py0)s
+000004c0: 2825 2870 7931 2973 290a 7d72 0300 0000  (%(py1)s).}r....
+000004d0: 721b 0000 00a9 0372 0800 0000 da03 7079  r......r......py
+000004e0: 31da 0370 7933 a908 7203 0000 0072 0c00  1..py3..r....r..
+000004f0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000500: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000510: 2903 721b 0000 00da 0b40 7079 5f61 7373  ).r......@py_ass
+00000520: 6572 7432 da0b 4070 795f 666f 726d 6174  ert2..@py_format
+00000530: 3472 1700 0000 7217 0000 0072 1800 0000  4r....r....r....
+00000540: da15 7465 7374 5f76 616c 6964 6174 655f  ..test_validate_
+00000550: 746f 5f74 7275 650e 0000 0073 0200 0000  to_true....s....
+00000560: 7804 7222 0000 007a 2068 7474 703a 2f2f  x.r"...z http://
+00000570: 6368 6174 7479 2e65 7861 6d70 6c65 2e63  chatty.example.c
+00000580: 6f6d 2f61 6c79 7373 617a 1061 6c79 7373  om/alyssaz.alyss
+00000590: 6163 6861 7474 792e 636f 6d63 0100 0000  achatty.comc....
+000005a0: 0000 0000 0000 0000 0400 0000 0600 0000  ................
+000005b0: 4300 0000 7382 0000 0074 007c 0083 017d  C...s....t.|...}
+000005c0: 017c 010c 007d 027c 0273 3b64 0164 0274  .|...}.|.s;d.d.t
+000005d0: 01a0 02a1 0076 0073 1574 03a0 0474 00a1  .....v.s.t...t..
+000005e0: 0172 1a74 03a0 0574 00a1 016e 0164 0264  .r.t...t...n.d.d
+000005f0: 0374 01a0 02a1 0076 0073 2674 03a0 047c  .t.....v.s&t...|
+00000600: 00a1 0172 2b74 03a0 057c 00a1 016e 0164  ...r+t...|...n.d
+00000610: 0374 03a0 057c 01a1 0164 049c 0316 007d  .t...|...d.....}
+00000620: 0374 0674 03a0 077c 03a1 0183 0182 0164  .t.t...|.......d
+00000630: 0004 007d 017d 0264 0053 0029 054e 7a30  ...}.}.d.S.).Nz0
+00000640: 6173 7365 7274 206e 6f74 2025 2870 7933  assert not %(py3
+00000650: 2973 0a7b 2528 7079 3329 7320 3d20 2528  )s.{%(py3)s = %(
+00000660: 7079 3029 7328 2528 7079 3129 7329 0a7d  py0)s(%(py1)s).}
+00000670: 7203 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00000680: 1f00 0000 2904 721b 0000 0072 2000 0000  ....).r....r ...
+00000690: da0b 4070 795f 6173 7365 7274 3472 1600  ..@py_assert4r..
+000006a0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+000006b0: 00da 1674 6573 745f 7661 6c69 6461 7465  ...test_validate
+000006c0: 5f74 6f5f 6661 6c73 6515 0000 0073 0200  _to_false....s..
+000006d0: 0000 8204 7224 0000 0029 0272 0500 0000  ....r$...).r....
+000006e0: 4e29 11da 0862 7569 6c74 696e 7372 0c00  N)...builtinsr..
+000006f0: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
+00000700: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
+00000710: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
+00000720: 6572 0e00 0000 da06 7079 7465 7374 da0a  er......pytest..
+00000730: 7661 6c69 6461 7469 6f6e 7203 0000 0072  validationr....r
+00000740: 0400 0000 7219 0000 0072 1a00 0000 da04  ....r....r......
+00000750: 6d61 726b da0b 7061 7261 6d65 7472 697a  mark..parametriz
+00000760: 65da 0373 7472 7222 0000 0072 2400 0000  e..strr"...r$...
+00000770: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00000780: 1800 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000790: 0000 7318 0000 0022 0010 020a 030a 0406  ..s...."........
+000007a0: 0408 0102 ff14 0306 0408 0102 ff18 03    ...............
```

### Comparing `bovine-0.1.2/bovine/utils/msg/test_validation.py` & `bovine-0.1.3/bovine/utils/msg/test_validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pytest
 
 from .validation import validate_to, validate_tos
 
 
-def test_validate_tos_none():
+def test_validate_tos_none() -> None:
     assert validate_tos(None)
 
 
-def test_validate_tos():
+def test_validate_tos() -> None:
     assert validate_tos(["alysssa@ben.de"])
 
 
 @pytest.mark.parametrize(
     "recipient", ["https://chatty.example.com/alyssa", "alyssa@chatty.com"]
 )
-def test_validate_to_true(recipient):
+def test_validate_to_true(recipient: str) -> None:
     assert validate_to(recipient)
 
 
 @pytest.mark.parametrize(
     "recipient", ["http://chatty.example.com/alyssa", "alyssachatty.com"]
 )
-def test_validate_to_false(recipient):
+def test_validate_to_false(recipient: str) -> None:
     assert not validate_to(recipient)
```

### Comparing `bovine-0.1.2/bovine/utils/test_date.py` & `bovine-0.1.3/bovine/utils/test_date.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from datetime import datetime, timedelta, timezone
 
 from .date import check_max_offset_now, get_gmt_now, parse_gmt
 
 
-def test_get_gmt_now():
+def test_get_gmt_now() -> None:
     date_string = get_gmt_now()
 
     assert "GMT" in date_string
 
 
-def test_parse_gmt():
+def test_parse_gmt() -> None:
     date_string = get_gmt_now()
 
     parsed = parse_gmt(date_string)
     now = datetime.now(tz=timezone.utc)
 
     assert parsed <= now
     assert parsed >= now - timedelta(seconds=5)
 
 
-def test_check_max_offset_now():
+def test_check_max_offset_now() -> None:
     now = datetime.now(tz=timezone.utc)
 
     assert check_max_offset_now(now - timedelta(minutes=4))
     assert check_max_offset_now(now + timedelta(minutes=4))
     assert not check_max_offset_now(now - timedelta(minutes=6))
     assert not check_max_offset_now(now + timedelta(minutes=6))
```

### Comparing `bovine-0.1.2/pyproject.toml` & `bovine-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "bovine"
-version = "0.1.2"
-description = "Core functionality of bovine needed to build FediVerse applications"
+version = "0.1.3"
+description = "Core functionality of bovine needed to build fediverse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
 repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
 
@@ -13,14 +13,15 @@
 python = "^3.10"
 aiohttp = "^3.8.3"
 cryptography = "^39.0.0"
 python-dateutil = "^2.8.2"
 tomli = "^2.0.1"
 multiformats = "^0.2.1"
 bleach = "^6.0.0"
+aiodns = "^3.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `bovine-0.1.2/PKG-INFO` & `bovine-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: bovine
-Version: 0.1.2
-Summary: Core functionality of bovine needed to build FediVerse applications
+Version: 0.1.3
+Summary: Core functionality of bovine needed to build fediverse applications
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: bleach (>=6.0.0,<7.0.0)
 Requires-Dist: cryptography (>=39.0.0,<40.0.0)
 Requires-Dist: multiformats (>=0.2.1,<0.3.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://bovine.readthedocs.io/en/latest/
```

