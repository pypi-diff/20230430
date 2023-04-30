# Comparing `tmp/dkimpy-1.1.2.tar.gz` & `tmp/dkimpy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkimpy-1.1.2.tar", last modified: Sun Apr  9 13:34:23 2023, max compression
+gzip compressed data, was "dkimpy-1.1.3.tar", last modified: Sun Apr 30 14:12:18 2023, max compression
```

## Comparing `dkimpy-1.1.2.tar` & `dkimpy-1.1.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.106676 dkimpy-1.1.2/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    13427 2023-04-09 13:33:30.000000 dkimpy-1.1.2/ChangeLog
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      979 2020-04-06 04:06:13.000000 dkimpy-1.1.2/LICENSE
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      200 2020-04-06 04:27:45.000000 dkimpy-1.1.2/MANIFEST.in
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    10824 2023-04-09 13:34:23.106676 dkimpy-1.1.2/PKG-INFO
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     7905 2023-03-31 17:07:31.000000 dkimpy-1.1.2/README.md
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.094675 dkimpy-1.1.2/dkim/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    57849 2023-03-31 17:04:51.000000 dkimpy-1.1.2/dkim/__init__.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      139 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/__main__.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2570 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/arcsign.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1774 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/arcverify.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4300 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/asn1.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4829 2023-02-28 04:59:06.000000 dkimpy-1.1.2/dkim/asyncsupport.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4610 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/canonicalization.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8173 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/crypto.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3628 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/dkimsign.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1951 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/dkimverify.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4688 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/dknewkey.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2982 2020-08-08 20:55:43.000000 dkimpy-1.1.2/dkim/dnsplug.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.094675 dkimpy-1.1.2/dkim/tests/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1769 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/__init__.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.102676 dkimpy-1.1.2/dkim/tests/data/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/1024_testkey.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      212 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/1024_testkey_wo_markers.pub.rsa.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/1024_testkey_wo_markers.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1679 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1704 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey_PKCS8.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey_PKCS8.key.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      384 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey_wo_markers.pub.rsa.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/2048_testkey_wo_markers.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      251 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/badk.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/badversion.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       58 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/ed25519test.dns
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/ed25519test.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/ed25519test.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      588 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/ed25519test2.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       67 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/eximtest.dns
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4444 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/message.mbox
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      269 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/rfc6376.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1069 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/rfc6376.signed.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      708 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/rfc6376.signed.rsa.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      275 2022-12-05 20:53:17.000000 dkimpy-1.1.2/dkim/tests/data/rfc6376.w1258.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/rfc8032_7_1.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      778 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/data/test.message.baddomain
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test.private
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1104 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test2.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test2.private
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      233 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test2.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test_bad.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      219 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test_extra.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      164 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/data/test_nofrom.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      250 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/data/test_tlsrpt.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     5300 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/test_arc.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6045 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/test_canonicalization.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6786 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/test_crypto.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    23644 2023-02-25 20:35:32.000000 dkimpy-1.1.2/dkim/tests/test_dkim.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    12866 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/test_dkim_ed25519.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4426 2022-12-05 21:05:46.000000 dkimpy-1.1.2/dkim/tests/test_dkim_generate.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2022-12-02 02:29:32.000000 dkimpy-1.1.2/dkim/tests/test_dkim_rsavariants.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11980 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/test_dkim_tlsrpt.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1557 2020-04-06 04:27:45.000000 dkimpy-1.1.2/dkim/tests/test_dnsplug.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3432 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/tests/test_util.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2501 2020-04-06 04:06:13.000000 dkimpy-1.1.2/dkim/util.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.102676 dkimpy-1.1.2/dkimpy.egg-info/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    10824 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/PKG-INFO
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1986 2023-04-09 13:34:23.000000 dkimpy-1.1.2/dkimpy.egg-info/SOURCES.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/dependency_links.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      173 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/entry_points.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2020-04-06 12:14:30.000000 dkimpy-1.1.2/dkimpy.egg-info/not-zip-safe
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       84 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/requires.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        5 2023-04-09 13:34:22.000000 dkimpy-1.1.2/dkimpy.egg-info/top_level.txt
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-09 13:34:23.106676 dkimpy-1.1.2/man/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4392 2020-04-06 04:06:13.000000 dkimpy-1.1.2/man/arcsign.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4152 2020-04-06 04:06:13.000000 dkimpy-1.1.2/man/arcverify.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4957 2020-04-06 04:06:13.000000 dkimpy-1.1.2/man/dkimsign.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4273 2022-12-02 02:29:32.000000 dkimpy-1.1.2/man/dkimverify.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2020-04-06 04:06:13.000000 dkimpy-1.1.2/man/dknewkey.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       38 2023-04-09 13:34:23.106676 dkimpy-1.1.2/setup.cfg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3387 2023-03-31 17:07:05.000000 dkimpy-1.1.2/setup.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      268 2020-04-06 04:06:13.000000 dkimpy-1.1.2/test.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-30 14:12:18.992257 dkimpy-1.1.3/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    13825 2023-04-30 14:11:53.000000 dkimpy-1.1.3/ChangeLog
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      979 2020-04-06 04:06:13.000000 dkimpy-1.1.3/LICENSE
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      200 2020-04-06 04:27:45.000000 dkimpy-1.1.3/MANIFEST.in
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11065 2023-04-30 14:12:18.992257 dkimpy-1.1.3/PKG-INFO
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8122 2023-04-30 14:11:53.000000 dkimpy-1.1.3/README.md
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-30 14:12:18.980257 dkimpy-1.1.3/dkim/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    58005 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/__init__.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      139 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/__main__.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2570 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/arcsign.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1774 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/arcverify.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4300 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/asn1.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4829 2023-04-30 13:58:34.000000 dkimpy-1.1.3/dkim/asyncsupport.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4610 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/canonicalization.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8173 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/crypto.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3628 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/dkimsign.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1951 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/dkimverify.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4737 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/dknewkey.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2982 2020-08-08 20:55:43.000000 dkimpy-1.1.3/dkim/dnsplug.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-30 14:12:18.984257 dkimpy-1.1.3/dkim/tests/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1769 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/tests/__init__.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-30 14:12:18.988257 dkimpy-1.1.3/dkim/tests/data/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/data/1024_testkey.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      212 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/data/1024_testkey_wo_markers.pub.rsa.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/data/1024_testkey_wo_markers.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1679 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/data/2048_testkey.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1704 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/tests/data/2048_testkey_PKCS8.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/tests/data/2048_testkey_PKCS8.key.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      384 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/data/2048_testkey_wo_markers.pub.rsa.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/data/2048_testkey_wo_markers.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      251 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/badk.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/badversion.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       58 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/ed25519test.dns
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/ed25519test.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/ed25519test.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      588 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/ed25519test2.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       67 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/eximtest.dns
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4444 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/message.mbox
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      269 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/rfc6376.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1069 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/rfc6376.signed.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      708 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/rfc6376.signed.rsa.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      275 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/tests/data/rfc6376.w1258.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/rfc8032_7_1.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      778 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/tests/data/test.message.baddomain
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test.private
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1104 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test2.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test2.private
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      233 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test2.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test_bad.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      219 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test_extra.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      164 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/data/test_nofrom.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      250 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/data/test_tlsrpt.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     5300 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/test_arc.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6045 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/test_canonicalization.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6786 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/test_crypto.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    23644 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/tests/test_dkim.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    12866 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/test_dkim_ed25519.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4476 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/tests/test_dkim_generate.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2023-04-30 14:11:53.000000 dkimpy-1.1.3/dkim/tests/test_dkim_rsavariants.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11980 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/test_dkim_tlsrpt.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1557 2020-04-06 04:27:45.000000 dkimpy-1.1.3/dkim/tests/test_dnsplug.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3432 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/tests/test_util.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2501 2020-04-06 04:06:13.000000 dkimpy-1.1.3/dkim/util.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-30 14:12:18.988257 dkimpy-1.1.3/dkimpy.egg-info/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11065 2023-04-30 14:12:18.000000 dkimpy-1.1.3/dkimpy.egg-info/PKG-INFO
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1986 2023-04-30 14:12:18.000000 dkimpy-1.1.3/dkimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2023-04-30 14:12:18.000000 dkimpy-1.1.3/dkimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      173 2023-04-30 14:12:18.000000 dkimpy-1.1.3/dkimpy.egg-info/entry_points.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2020-04-06 12:14:30.000000 dkimpy-1.1.3/dkimpy.egg-info/not-zip-safe
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       84 2023-04-30 14:12:18.000000 dkimpy-1.1.3/dkimpy.egg-info/requires.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        5 2023-04-30 14:12:18.000000 dkimpy-1.1.3/dkimpy.egg-info/top_level.txt
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-04-30 14:12:18.992257 dkimpy-1.1.3/man/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4392 2020-04-06 04:06:13.000000 dkimpy-1.1.3/man/arcsign.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4152 2020-04-06 04:06:13.000000 dkimpy-1.1.3/man/arcverify.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4957 2020-04-06 04:06:13.000000 dkimpy-1.1.3/man/dkimsign.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4273 2023-04-30 14:11:53.000000 dkimpy-1.1.3/man/dkimverify.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2020-04-06 04:06:13.000000 dkimpy-1.1.3/man/dknewkey.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       38 2023-04-30 14:12:18.992257 dkimpy-1.1.3/setup.cfg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3387 2023-04-30 14:11:53.000000 dkimpy-1.1.3/setup.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      268 2020-04-06 04:06:13.000000 dkimpy-1.1.3/test.py
```

### Comparing `dkimpy-1.1.2/ChangeLog` & `dkimpy-1.1.3/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2023-04-30 Version 1.1.3
+   - Catch nacl.exceptions.ValueError and raise KeyFormatError, similar to how
+     RSA key errors are treated (LP: #2018021)
+   - Create ed25519 key files with secure permissions to avoid risk of
+     insecure chmode call/race condition (Thanks to Hanno Böck for the report
+     and the suggested fix) (LP: #2017430)
+   - Properly cleanup temporary directories in tests
+
 2023-04-09 Version 1.1.2
    - Verify correct AMS header is used for ARC seal verification (André Cruz)
 
 2023-03-09 Version 1.1.1
     - Document dropping of Python 2 support (dropped as of 1.1.0) (LP:
       #20086738)
     - Fix traceback when attempting to verify an unsigned message using
```

### Comparing `dkimpy-1.1.2/LICENSE` & `dkimpy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/PKG-INFO` & `dkimpy-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkimpy
-Version: 1.1.2
+Version: 1.1.3
 Summary: DKIM (DomainKeys Identified Mail), ARC (Authenticated Receive Chain), and TLSRPT (TLS Report) email signing and verification
 Home-page: https://launchpad.net/dkimpy
 Author: Scott Kitterman
 Author-email: scott@kitterman.com
 License: BSD-like
 Description: dkimpy - DKIM (DomainKeys Identified Mail)
         https://launchpad.net/dkimpy/
@@ -17,15 +17,15 @@
         dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
         signing and verification.  Basic DKIM requirements are defined in RFC 6376:
         
         https://tools.ietf.org/html/rfc6376
         
         # VERSION
         
-        This is dkimpy 1.1.2.
+        This is dkimpy 1.1.3.
         
         # REQUIREMENTS
         
         Dependencies will be automatically included for normal DKIM usage.  The
         extras_requires feature 'ed25519' will add the dependencies needed for signing
         and verifying using the new DCRUP ed25519-sha256 algorithm.  The
         extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
@@ -156,15 +156,18 @@
         ## DKIM SCRIPTS
         
         Three helper programs are also supplied: dknewkey, dkimsign and
         dkimverify
         
         dknewkey is s script that produces private and public key pairs suitable
         for use with DKIM.  Note that the private key file format used for ed25519 is
-        not standardized (there is no standard) and is unique to dkimpy.
+        not standardized (there is no standard) and is unique to dkimpy.  Creation of
+        keys should be done in a secure environment.  If an unauthorized entity gains
+        access to current private keys they can generate signed email that will pass
+        DKIM checkes and will be difficult to repudiate.
         
         dkimsign is a filter that reads an RFC822 message on standard input, and
         writes the same message on standard output with a DKIM-Signature line
         prepended. The signing options are specified on the command line:
         
         dkimsign selector domain privatekeyfile [identity]
```

### Comparing `dkimpy-1.1.2/README.md` & `dkimpy-1.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
 signing and verification.  Basic DKIM requirements are defined in RFC 6376:
 
 https://tools.ietf.org/html/rfc6376
 
 # VERSION
 
-This is dkimpy 1.1.2.
+This is dkimpy 1.1.3.
 
 # REQUIREMENTS
 
 Dependencies will be automatically included for normal DKIM usage.  The
 extras_requires feature 'ed25519' will add the dependencies needed for signing
 and verifying using the new DCRUP ed25519-sha256 algorithm.  The
 extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
@@ -148,15 +148,18 @@
 ## DKIM SCRIPTS
 
 Three helper programs are also supplied: dknewkey, dkimsign and
 dkimverify
 
 dknewkey is s script that produces private and public key pairs suitable
 for use with DKIM.  Note that the private key file format used for ed25519 is
-not standardized (there is no standard) and is unique to dkimpy.
+not standardized (there is no standard) and is unique to dkimpy.  Creation of
+keys should be done in a secure environment.  If an unauthorized entity gains
+access to current private keys they can generate signed email that will pass
+DKIM checkes and will be difficult to repudiate.
 
 dkimsign is a filter that reads an RFC822 message on standard input, and
 writes the same message on standard output with a DKIM-Signature line
 prepended. The signing options are specified on the command line:
 
 dkimsign selector domain privatekeyfile [identity]
```

### Comparing `dkimpy-1.1.2/dkim/__init__.py` & `dkimpy-1.1.3/dkim/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,26 +464,28 @@
       pass
   try:
       if pub[b'k'] == b'ed25519':
           try:
               pk = nacl.signing.VerifyKey(pub[b'p'], encoder=nacl.encoding.Base64Encoder)
           except NameError:
               raise NaClNotFoundError('pynacl module required for ed25519 signing, see README.md')
+          except nacl.exceptions.ValueError as e:
+              raise KeyFormatError("could not parse ed25519 public key (%s): %s" % (pub[b'p'],e))
           keysize = 256
           ktag = b'ed25519'
   except KeyError:
       pub[b'k'] = b'rsa'
   if pub[b'k'] == b'rsa':
       try:
           pk = parse_public_key(base64.b64decode(pub[b'p']))
           keysize = bitsize(pk['modulus'])
       except KeyError:
-          raise KeyFormatError("incomplete public key: %s" % s)
+          raise KeyFormatError("incomplete RSA public key: %s" % s)
       except (TypeError,UnparsableKeyError) as e:
-          raise KeyFormatError("could not parse public key (%s): %s" % (pub[b'p'],e))
+          raise KeyFormatError("could not parse RSA public key (%s): %s" % (pub[b'p'],e))
       ktag = b'rsa'
   if pub[b'k'] != b'rsa' and pub[b'k'] != b'ed25519':
       raise KeyFormatError('unknown algorithm in k= tag: {0}'.format(pub[b'k']))
   seqtlsrpt = False
   try:
       # Ignore unknown service types, RFC 6376 3.6.1
       if pub[b's'] != b'*' and pub[b's'] != b'email' and pub[b's'] != b'tlsrpt':
```

### Comparing `dkimpy-1.1.2/dkim/arcsign.py` & `dkimpy-1.1.3/dkim/arcsign.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/arcverify.py` & `dkimpy-1.1.3/dkim/arcverify.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/asn1.py` & `dkimpy-1.1.3/dkim/asn1.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/asyncsupport.py` & `dkimpy-1.1.3/dkim/asyncsupport.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/canonicalization.py` & `dkimpy-1.1.3/dkim/canonicalization.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/crypto.py` & `dkimpy-1.1.3/dkim/crypto.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/dkimsign.py` & `dkimpy-1.1.3/dkim/dkimsign.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/dkimverify.py` & `dkimpy-1.1.3/dkim/dkimverify.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/dknewkey.py` & `dkimpy-1.1.3/dkim/dknewkey.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,18 +60,20 @@
     import nacl.signing # Yes, pep-8, but let's not make everyone install nacl
     import nacl.encoding
     import os
     skg = nacl.signing.SigningKey(seed=os.urandom(32))
     if verbose:
         eprint('generating ' + private_key_file)
     priv_key = skg.generate()
+    if os.name == 'posix':
+        old_umask = os.umask(0o077)
     with open(private_key_file, 'w') as pkf:
         pkf.write(priv_key.encode(encoder=nacl.encoding.Base64Encoder).decode("utf-8"))
     if os.name == 'posix':
-        os.chmod(private_key_file, 0o600)
+        os.umask(old_umask)
     return(priv_key)
 
 def ExtractRSADnsPublicKey(private_key_file, dns_file, verbose=True):
   """ Given a key, extract the bit we should place in DNS.
   """
   if verbose:
     eprint('extracting ' + private_key_file)
```

### Comparing `dkimpy-1.1.2/dkim/dnsplug.py` & `dkimpy-1.1.3/dkim/dnsplug.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/__init__.py` & `dkimpy-1.1.3/dkim/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/1024_testkey.key` & `dkimpy-1.1.3/dkim/tests/data/1024_testkey.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/2048_testkey.key` & `dkimpy-1.1.3/dkim/tests/data/2048_testkey.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/2048_testkey_PKCS8.key` & `dkimpy-1.1.3/dkim/tests/data/2048_testkey_PKCS8.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/ed25519test2.msg` & `dkimpy-1.1.3/dkim/tests/data/ed25519test2.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/message.mbox` & `dkimpy-1.1.3/dkim/tests/data/message.mbox`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/rfc6376.signed.msg` & `dkimpy-1.1.3/dkim/tests/data/rfc6376.signed.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/rfc6376.signed.rsa.msg` & `dkimpy-1.1.3/dkim/tests/data/rfc6376.signed.rsa.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/test.message.baddomain` & `dkimpy-1.1.3/dkim/tests/data/test.message.baddomain`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/test.private` & `dkimpy-1.1.3/dkim/tests/data/test.private`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/test2.message` & `dkimpy-1.1.3/dkim/tests/data/test2.message`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/data/test2.private` & `dkimpy-1.1.3/dkim/tests/data/test2.private`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_arc.py` & `dkimpy-1.1.3/dkim/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_canonicalization.py` & `dkimpy-1.1.3/dkim/tests/test_canonicalization.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_crypto.py` & `dkimpy-1.1.3/dkim/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_dkim.py` & `dkimpy-1.1.3/dkim/tests/test_dkim.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_dkim_ed25519.py` & `dkimpy-1.1.3/dkim/tests/test_dkim_ed25519.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_dkim_generate.py` & `dkimpy-1.1.3/dkim/tests/test_dkim_generate.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         for header_algo in (b"simple", b"relaxed"):
             for body_algo in (b"simple", b"relaxed"):
                 sig = dkim.sign(
                     self.message, b"test", b"example.com", rsakey,
                     canonicalize=(header_algo, body_algo))
                 res = dkim.verify(sig + self.message, dnsfunc=self.dnsfuncRSA)
                 self.assertTrue(res)
+        tmpdir.cleanup()
 
 
     def test_generate_verifies_Ed25519_key(self):
         #Create temporary dir
         tmpdir = tempfile.TemporaryDirectory()
         keydir = tmpdir.name
         ed25519_key_file = os.path.join(keydir, "dkim.ed25519.key")
@@ -78,14 +79,15 @@
             for body_algo in (b"simple", b"relaxed"):
                 sig = dkim.sign(
                     self.message, b"test1", b"example.com", ed25519key,
                     signature_algorithm=b'ed25519-sha256',
                     canonicalize=(header_algo, body_algo))
                 res = dkim.verify(sig + self.message, dnsfunc=self.dnsfuncED25519)
                 self.assertTrue(res)
+        tmpdir.cleanup()
 
 
     def dnsfuncRSA(self, domain, timeout=5):
         _dns_responses = {
             'test._domainkey.example.com.': read_data(self.rsa_dns_key_file),
         }
         try:
```

### Comparing `dkimpy-1.1.2/dkim/tests/test_dkim_rsavariants.py` & `dkimpy-1.1.3/dkim/tests/test_dkim_rsavariants.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_dkim_tlsrpt.py` & `dkimpy-1.1.3/dkim/tests/test_dkim_tlsrpt.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_dnsplug.py` & `dkimpy-1.1.3/dkim/tests/test_dnsplug.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/tests/test_util.py` & `dkimpy-1.1.3/dkim/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkim/util.py` & `dkimpy-1.1.3/dkim/util.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/dkimpy.egg-info/PKG-INFO` & `dkimpy-1.1.3/dkimpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkimpy
-Version: 1.1.2
+Version: 1.1.3
 Summary: DKIM (DomainKeys Identified Mail), ARC (Authenticated Receive Chain), and TLSRPT (TLS Report) email signing and verification
 Home-page: https://launchpad.net/dkimpy
 Author: Scott Kitterman
 Author-email: scott@kitterman.com
 License: BSD-like
 Description: dkimpy - DKIM (DomainKeys Identified Mail)
         https://launchpad.net/dkimpy/
@@ -17,15 +17,15 @@
         dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
         signing and verification.  Basic DKIM requirements are defined in RFC 6376:
         
         https://tools.ietf.org/html/rfc6376
         
         # VERSION
         
-        This is dkimpy 1.1.2.
+        This is dkimpy 1.1.3.
         
         # REQUIREMENTS
         
         Dependencies will be automatically included for normal DKIM usage.  The
         extras_requires feature 'ed25519' will add the dependencies needed for signing
         and verifying using the new DCRUP ed25519-sha256 algorithm.  The
         extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
@@ -156,15 +156,18 @@
         ## DKIM SCRIPTS
         
         Three helper programs are also supplied: dknewkey, dkimsign and
         dkimverify
         
         dknewkey is s script that produces private and public key pairs suitable
         for use with DKIM.  Note that the private key file format used for ed25519 is
-        not standardized (there is no standard) and is unique to dkimpy.
+        not standardized (there is no standard) and is unique to dkimpy.  Creation of
+        keys should be done in a secure environment.  If an unauthorized entity gains
+        access to current private keys they can generate signed email that will pass
+        DKIM checkes and will be difficult to repudiate.
         
         dkimsign is a filter that reads an RFC822 message on standard input, and
         writes the same message on standard output with a DKIM-Signature line
         prepended. The signing options are specified on the command line:
         
         dkimsign selector domain privatekeyfile [identity]
```

### Comparing `dkimpy-1.1.2/dkimpy.egg-info/SOURCES.txt` & `dkimpy-1.1.3/dkimpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/man/arcsign.1` & `dkimpy-1.1.3/man/arcsign.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/man/arcverify.1` & `dkimpy-1.1.3/man/arcverify.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/man/dkimsign.1` & `dkimpy-1.1.3/man/dkimsign.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/man/dkimverify.1` & `dkimpy-1.1.3/man/dkimverify.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/man/dknewkey.1` & `dkimpy-1.1.3/man/dknewkey.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.2/setup.py` & `dkimpy-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # This has been modified from the original software.
 # Copyright (c) 2011,2012,2018 Scott Kitterman <scott@kitterman.com>
 
 from setuptools import setup
 import os
 import sys
 
-version = "1.1.2"
+version = "1.1.3"
 
 kw = {}  # Work-around for lack of 'or' requires in setuptools.
 try:
     import DNS
     kw['install_requires'] = ['Py3DNS']
 except ImportError:  # If PyDNS is not installed, prefer dnspython
     kw['install_requires'] = ['dnspython>=1.16.0']
```

