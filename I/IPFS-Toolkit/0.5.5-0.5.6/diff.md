# Comparing `tmp/IPFS-Toolkit-0.5.5.tar.gz` & `tmp/IPFS-Toolkit-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPFS-Toolkit-0.5.5.tar", last modified: Sat Apr 29 06:23:00 2023, max compression
+gzip compressed data, was "IPFS-Toolkit-0.5.6.tar", last modified: Sun Apr 30 17:50:39 2023, max compression
```

## Comparing `IPFS-Toolkit-0.5.5.tar` & `IPFS-Toolkit-0.5.6.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7983 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/IPFS_API.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12925 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/IPFS_DataTransmission.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1368 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/IPFS_LNS.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.474612 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)    12580 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/PKG-INFO
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)     1337 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)        1 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)       64 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/requires.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)      105 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/top_level.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12580 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/PKG-INFO
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    17995 2023-04-29 06:15:14.000000 IPFS-Toolkit-0.5.5/ipfs_api.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14844 2023-04-29 05:16:35.000000 IPFS-Toolkit-0.5.5/ipfs_cli.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    74398 2023-04-23 14:44:42.000000 IPFS-Toolkit-0.5.5/ipfs_datatransmission.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     5291 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfs_lns.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/ipfshttpclient2/
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      417 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/__init__.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10097 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/__init__.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    12665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/base.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1755 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/bitswap.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2045 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/block.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1783 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/bootstrap.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2159 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/config.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/dag.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6294 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/dht.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14839 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/files.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     3431 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/key.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6230 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/miscellaneous.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4125 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/name.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    11246 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/object.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3400 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/p2p.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     8698 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/pin.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10038 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/pubsub.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2366 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/repo.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6087 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/swarm.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5684 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/unstable.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7884 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/encoding.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5622 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/exceptions.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    25493 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/filescanner.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1361 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/http.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19985 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/http_common.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6139 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/http_httpx.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6600 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/http_requests.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    19796 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/multipart.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     9483 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/requests_wrapper.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4749 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/utils.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      551 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/version.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/pyproject.toml
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/setup.cfg
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1499 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/setup.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/tests/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5345 2023-04-29 06:20:36.000000 IPFS-Toolkit-0.5.5/tests/test_with_docker.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1547 2023-04-29 06:17:33.000000 IPFS-Toolkit-0.5.5/tests/test_without_docker.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7983 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/IPFS_API.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12925 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/IPFS_DataTransmission.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1368 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/IPFS_LNS.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.546781 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)    12580 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)     1357 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)        1 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)       64 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/requires.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)      105 2023-04-30 17:50:39.000000 IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12580 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/PKG-INFO
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    19575 2023-04-30 14:11:24.000000 IPFS-Toolkit-0.5.6/ipfs_api.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14844 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.6/ipfs_cli.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    74398 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.6/ipfs_datatransmission.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     5291 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfs_lns.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.546781 IPFS-Toolkit-0.5.6/ipfshttpclient2/
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      417 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/__init__.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10097 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/__init__.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    12665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/base.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1755 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/bitswap.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2045 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/block.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1783 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/bootstrap.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2159 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/config.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/dag.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6294 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/dht.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14839 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/files.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     3431 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/key.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6230 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/miscellaneous.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4125 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/name.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    11246 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/object.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3400 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/p2p.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     8698 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/pin.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10038 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/pubsub.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2366 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/repo.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7484 2023-04-30 14:02:37.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/swarm.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5684 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/client/unstable.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7884 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/encoding.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5622 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/exceptions.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    25493 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/filescanner.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1361 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/http.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19985 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/http_common.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6139 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/http_httpx.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6600 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/http_requests.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    19796 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/multipart.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     9483 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/requests_wrapper.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4749 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/utils.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      551 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/ipfshttpclient2/version.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.6/pyproject.toml
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/setup.cfg
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1499 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.6/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-30 17:50:39.550781 IPFS-Toolkit-0.5.6/tests/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3128 2023-04-30 17:44:05.000000 IPFS-Toolkit-0.5.6/tests/test_peers.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5345 2023-04-30 17:45:34.000000 IPFS-Toolkit-0.5.6/tests/test_with_docker.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1547 2023-04-30 17:46:18.000000 IPFS-Toolkit-0.5.6/tests/test_without_docker.py
```

### Comparing `IPFS-Toolkit-0.5.5/IPFS_API.py` & `IPFS-Toolkit-0.5.6/IPFS_API.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/IPFS_DataTransmission.py` & `IPFS-Toolkit-0.5.6/IPFS_DataTransmission.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/IPFS_LNS.py` & `IPFS-Toolkit-0.5.6/IPFS_LNS.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/PKG-INFO` & `IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFS-Toolkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: A set of tools  for working with IPFS in Python: a programmer-friendly API wrapper, P2P data-transmission machinery, and accelerated connections to known peers
 Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup#IPFS-Toolkit
 Author: emendir
 License: UNKNOWN
 Project-URL: Github, https://github.com/emendir/IPFS-Toolkit-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/SOURCES.txt` & `IPFS-Toolkit-0.5.6/IPFS_Toolkit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,9 +39,10 @@
 ipfshttpclient2/client/object.py
 ipfshttpclient2/client/p2p.py
 ipfshttpclient2/client/pin.py
 ipfshttpclient2/client/pubsub.py
 ipfshttpclient2/client/repo.py
 ipfshttpclient2/client/swarm.py
 ipfshttpclient2/client/unstable.py
+tests/test_peers.py
 tests/test_with_docker.py
 tests/test_without_docker.py
```

### Comparing `IPFS-Toolkit-0.5.5/PKG-INFO` & `IPFS-Toolkit-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFS-Toolkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: A set of tools  for working with IPFS in Python: a programmer-friendly API wrapper, P2P data-transmission machinery, and accelerated connections to known peers
 Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup#IPFS-Toolkit
 Author: emendir
 License: UNKNOWN
 Project-URL: Github, https://github.com/emendir/IPFS-Toolkit-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IPFS-Toolkit-0.5.5/ipfs_api.py` & `IPFS-Toolkit-0.5.6/ipfs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This is a wrapper for the ipfshttpclient module to make it easier to interact with the Interplanetary File System (IPFS)
 # process running on the computer.
 # To use it you must have IPFS running on your computer.
 # This wrapper uses a custom updated version of the ipfshttpclient.
 
 
+from termcolor import colored
 import time
 from threading import Event
 import shutil
 import tempfile
 # import sys
 from subprocess import Popen, PIPE
 # import subprocess
@@ -192,15 +193,15 @@
     """Returns this IPFS node's peer ID.
     Returns:
         str: the peer ID of this node
     """
     return http_client.id().get("Addresses")
 
 
-def list_peer_multiaddrs():
+def list_peers():
     """Returns a list of the IPFS multiaddresses of the other nodes
     this node is connected to.
     Returns:
         list(str): a list of the IPFS multiaddresses of the other nodes
         this node is connected to
     """
     proc = Popen(['ipfs', 'swarm', 'peers'], stdout=PIPE)
@@ -208,14 +209,53 @@
     peers = []
     for line in proc.stdout:
         peers.append(line.decode('utf-8').strip("\n"))
 
     return peers
 
 
+def list_peer_multiaddrs():
+    print(colored("IPFS_API: DEPRECATED: This function (ifps_api.list_peer_multiaddrs) has been renamed to ipfs_api.list_peers to avoid confusion with the new get_peer_multiaddrs function.", "yellow"))
+    return list_peers()
+
+
+def get_peer_multiaddrs(peer_id):
+    """Returns the multiaddresses (without the IPFS CID) via which we can reach
+    the specified peer.
+    Append /p2p/PEER_ID to these multiaddress parts to turn them into complete
+    multiaddresses.
+
+    Args:
+        peer_id (str): the IPFS ID of the peer to lookup
+
+    Returns:
+        list(str): the multiaddresses (without the IPFS CID) via which we can
+        reach the given peer
+    """
+    try:
+        response = http_client.dht.findpeer(peer_id)
+        return response.get("Responses")[0].get("Addrs")
+    except:
+        return []
+
+
+def connect_to_peer(multiaddr):
+    """Tries to connect to a peer given its multiaddress.
+    Returns:
+        bool: success
+    """
+    try:
+        response = http_client.swarm.connect(multiaddr)
+        if response.get("Strings")[0][-7:] == "success":
+            return True
+        return False
+    except:
+        return False
+
+
 def find_peer(peer_id: str):
     """Try to connect to the specified IPFS node.
     Args:
         peer_id (str): the IPFS peer ID of the node to connect to
     Returns:
         str: the multiaddress of the connected node
     """
@@ -471,28 +511,36 @@
     while data[-1] == 61 and data[-1]:
         data = data[:-1]
     data = b'u' + data
     return data
 
 
 def wait_till_ipfs_is_running(timeout_sec=None):
+    """Waits till it can connect to the local IPFS daemon's HTTP-interface.
+    Args:
+        timeout_sec (int): maximum time to wait for. If this duration is,
+                            exceeded, a TimeoutError is raised.
+    """
     count = 0
     while True:
         try:
             if is_ipfs_running():
                 return
         except ipfshttpclient.exceptions.ConnectionError as error:
             pass
         time.sleep(1)
         count += 1
         if timeout_sec and count == timeout_sec:
             raise TimeoutError()
 
 
 def try_run_ipfs():
+    """Tries to use the IPFS CLI to run the local IPFS daemon with PubSub,
+    like manually executing `ipfs daemon --enable-pubsub-experiment`
+    """
     from ipfs_cli import try_run_ipfs as _try_run_ipfs
     _try_run_ipfs()
 
 
 if LIBERROR:    # if not all modules needed for the ipfs_http_client library were loaded
     print("Falling back to IPFS CLI because our HTTP client isn't working;\nNot all modules required by the http-connection could be loaded.")
     from ipfs_cli import *
```

### Comparing `IPFS-Toolkit-0.5.5/ipfs_cli.py` & `IPFS-Toolkit-0.5.6/ipfs_cli.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfs_datatransmission.py` & `IPFS-Toolkit-0.5.6/ipfs_datatransmission.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfs_lns.py` & `IPFS-Toolkit-0.5.6/ipfs_lns.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/__init__.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/__init__.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/base.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/base.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/bitswap.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/bitswap.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/block.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/block.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/bootstrap.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/bootstrap.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/config.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/config.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/dag.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/dag.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/dht.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/dht.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/files.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/files.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/key.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/key.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/miscellaneous.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/name.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/name.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/object.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/object.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/p2p.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/p2p.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/pin.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/pin.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/pubsub.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/pubsub.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/repo.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/repo.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/unstable.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/client/unstable.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/encoding.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/encoding.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/exceptions.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/exceptions.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/filescanner.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/filescanner.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/http.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/http.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/http_common.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/http_common.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/http_httpx.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/http_httpx.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/http_requests.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/http_requests.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/multipart.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/multipart.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/requests_wrapper.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/utils.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/utils.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/ipfshttpclient2/version.py` & `IPFS-Toolkit-0.5.6/ipfshttpclient2/version.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/setup.py` & `IPFS-Toolkit-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/tests/test_with_docker.py` & `IPFS-Toolkit-0.5.6/tests/test_with_docker.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.5/tests/test_without_docker.py` & `IPFS-Toolkit-0.5.6/tests/test_without_docker.py`

 * *Files identical despite different names*

