# Comparing `tmp/tonsdk-1.0.7.tar.gz` & `tmp/tonsdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonsdk-1.0.7.tar", last modified: Sun Sep 18 15:48:18 2022, max compression
+gzip compressed data, was "tonsdk-1.0.9.tar", last modified: Wed Nov 16 07:38:47 2022, max compression
```

## Comparing `tonsdk-1.0.7.tar` & `tonsdk-1.0.9.tar`

### file list

```diff
@@ -1,78 +1,85 @@
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.409261 tonsdk-1.0.7/
--rw-r--r--   0 akkireev   (501) staff       (20)    11357 2022-08-23 05:56:48.000000 tonsdk-1.0.7/LICENSE
--rw-r--r--   0 akkireev   (501) staff       (20)     7422 2022-09-18 15:48:18.409442 tonsdk-1.0.7/PKG-INFO
--rw-r--r--   0 akkireev   (501) staff       (20)     6509 2022-08-29 08:29:45.000000 tonsdk-1.0.7/README.md
--rw-r--r--   0 akkireev   (501) staff       (20)       89 2022-08-22 06:24:22.000000 tonsdk-1.0.7/pyproject.toml
--rw-r--r--   0 akkireev   (501) staff       (20)     1201 2022-09-18 15:48:18.410198 tonsdk-1.0.7/setup.cfg
--rw-r--r--   0 akkireev   (501) staff       (20)       37 2022-08-22 06:24:22.000000 tonsdk-1.0.7/setup.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.377936 tonsdk-1.0.7/tonsdk/
--rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)      352 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/_exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.382685 tonsdk-1.0.7/tonsdk/boc/
--rw-r--r--   0 akkireev   (501) staff       (20)      145 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/boc/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4896 2022-08-23 16:38:23.000000 tonsdk-1.0.7/tonsdk/boc/_bit_string.py
--rw-r--r--   0 akkireev   (501) staff       (20)    11121 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/boc/_cell.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.383387 tonsdk-1.0.7/tonsdk/contract/
--rw-r--r--   0 akkireev   (501) staff       (20)     5127 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.384288 tonsdk-1.0.7/tonsdk/contract/token/
--rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-09-18 15:46:05.000000 tonsdk-1.0.7/tonsdk/contract/token/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.385614 tonsdk-1.0.7/tonsdk/contract/token/ft/
--rw-r--r--   0 akkireev   (501) staff       (20)      134 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/token/ft/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3241 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/token/ft/jetton_minter.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3155 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/token/ft/jetton_wallet.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.388656 tonsdk-1.0.7/tonsdk/contract/token/nft/
--rw-r--r--   0 akkireev   (501) staff       (20)      167 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/token/nft/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4473 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/token/nft/nft_collection.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2638 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/token/nft/nft_item.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1975 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/token/nft/nft_sale.py
--rw-r--r--   0 akkireev   (501) staff       (20)      889 2022-08-22 06:23:56.000000 tonsdk-1.0.7/tonsdk/contract/token/nft/nft_utils.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.391434 tonsdk-1.0.7/tonsdk/contract/wallet/
--rw-r--r--   0 akkireev   (501) staff       (20)     2891 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/wallet/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4212 2022-09-18 15:46:05.000000 tonsdk-1.0.7/tonsdk/contract/wallet/_wallet_contract.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1373 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/wallet/_wallet_contract_v2.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1933 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/wallet/_wallet_contract_v3.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4622 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/contract/wallet/_wallet_contract_v4.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.394867 tonsdk-1.0.7/tonsdk/crypto/
--rw-r--r--   0 akkireev   (501) staff       (20)      322 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/crypto/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)      609 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/crypto/_keystore.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1845 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/crypto/_mnemonic.py
--rw-r--r--   0 akkireev   (501) staff       (20)       26 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/crypto/_settings.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1023 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/crypto/_utils.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.396061 tonsdk-1.0.7/tonsdk/crypto/bip39/
--rw-r--r--   0 akkireev   (501) staff       (20)       68 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/crypto/bip39/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)    19268 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/crypto/bip39/_english.py
--rw-r--r--   0 akkireev   (501) staff       (20)      138 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/crypto/exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.399109 tonsdk-1.0.7/tonsdk/provider/
--rw-r--r--   0 akkireev   (501) staff       (20)      495 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/provider/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3977 2022-08-22 19:28:07.000000 tonsdk-1.0.7/tonsdk/provider/_address.py
--rw-r--r--   0 akkireev   (501) staff       (20)      147 2022-08-22 19:28:07.000000 tonsdk-1.0.7/tonsdk/provider/_exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.400446 tonsdk-1.0.7/tonsdk/provider/_toncenter/
--rw-r--r--   0 akkireev   (501) staff       (20)      124 2022-08-22 19:28:07.000000 tonsdk-1.0.7/tonsdk/provider/_toncenter/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2374 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/provider/_toncenter/_client.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.401646 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/
--rw-r--r--   0 akkireev   (501) staff       (20)      196 2022-08-22 19:28:07.000000 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.403189 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_async/
--rw-r--r--   0 akkireev   (501) staff       (20)      153 2022-08-22 19:28:07.000000 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_async/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)    31396 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_async/_client.py
--rw-r--r--   0 akkireev   (501) staff       (20)     6163 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_async/_wrapper.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.404631 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_sync/
--rw-r--r--   0 akkireev   (501) staff       (20)      141 2022-08-22 19:28:07.000000 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_sync/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4535 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_sync/_client.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2074 2022-08-22 19:28:07.000000 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_sync/_wrapper.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4442 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_utils.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.405377 tonsdk-1.0.7/tonsdk/provider/_utils/
--rw-r--r--   0 akkireev   (501) staff       (20)     1245 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/provider/_utils/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4803 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/provider/_wallet.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.408594 tonsdk-1.0.7/tonsdk/utils/
--rw-r--r--   0 akkireev   (501) staff       (20)      667 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/utils/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4808 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/utils/_address.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3004 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/utils/_currency.py
--rw-r--r--   0 akkireev   (501) staff       (20)      134 2022-08-04 10:29:39.000000 tonsdk-1.0.7/tonsdk/utils/_exceptions.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4200 2022-08-29 07:57:29.000000 tonsdk-1.0.7/tonsdk/utils/_utils.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-09-18 15:48:18.380853 tonsdk-1.0.7/tonsdk.egg-info/
--rw-r--r--   0 akkireev   (501) staff       (20)     7422 2022-09-18 15:48:18.000000 tonsdk-1.0.7/tonsdk.egg-info/PKG-INFO
--rw-r--r--   0 akkireev   (501) staff       (20)     1866 2022-09-18 15:48:18.000000 tonsdk-1.0.7/tonsdk.egg-info/SOURCES.txt
--rw-r--r--   0 akkireev   (501) staff       (20)        1 2022-09-18 15:48:18.000000 tonsdk-1.0.7/tonsdk.egg-info/dependency_links.txt
--rw-r--r--   0 akkireev   (501) staff       (20)        1 2022-08-22 20:11:48.000000 tonsdk-1.0.7/tonsdk.egg-info/not-zip-safe
--rw-r--r--   0 akkireev   (501) staff       (20)       14 2022-09-18 15:48:18.000000 tonsdk-1.0.7/tonsdk.egg-info/requires.txt
--rw-r--r--   0 akkireev   (501) staff       (20)        7 2022-09-18 15:48:18.000000 tonsdk-1.0.7/tonsdk.egg-info/top_level.txt
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.502847 tonsdk-1.0.9/
+-rw-r--r--   0 akkireev   (501) staff       (20)    11357 2022-08-23 05:56:48.000000 tonsdk-1.0.9/LICENSE
+-rw-r--r--   0 akkireev   (501) staff       (20)     7422 2022-11-16 07:38:47.503080 tonsdk-1.0.9/PKG-INFO
+-rw-r--r--   0 akkireev   (501) staff       (20)     6509 2022-08-29 08:29:45.000000 tonsdk-1.0.9/README.md
+-rw-r--r--   0 akkireev   (501) staff       (20)       89 2022-08-22 06:24:22.000000 tonsdk-1.0.9/pyproject.toml
+-rw-r--r--   0 akkireev   (501) staff       (20)     1201 2022-11-16 07:38:47.504605 tonsdk-1.0.9/setup.cfg
+-rw-r--r--   0 akkireev   (501) staff       (20)       37 2022-08-22 06:24:22.000000 tonsdk-1.0.9/setup.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.466720 tonsdk-1.0.9/tonsdk/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-08-04 10:29:39.000000 tonsdk-1.0.9/tonsdk/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      352 2022-08-04 10:29:39.000000 tonsdk-1.0.9/tonsdk/_exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.473190 tonsdk-1.0.9/tonsdk/boc/
+-rw-r--r--   0 akkireev   (501) staff       (20)      300 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/boc/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4965 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/boc/_bit_string.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1918 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/boc/_builder.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    11203 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/boc/_cell.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1309 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/boc/_dict_builder.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.474450 tonsdk-1.0.9/tonsdk/boc/dict/
+-rw-r--r--   0 akkireev   (501) staff       (20)       94 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/boc/dict/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      356 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/boc/dict/find_common_prefix.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4193 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/boc/dict/serialize_dict.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.475105 tonsdk-1.0.9/tonsdk/contract/
+-rw-r--r--   0 akkireev   (501) staff       (20)     5127 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.475886 tonsdk-1.0.9/tonsdk/contract/token/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-09-18 15:46:05.000000 tonsdk-1.0.9/tonsdk/contract/token/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.477985 tonsdk-1.0.9/tonsdk/contract/token/ft/
+-rw-r--r--   0 akkireev   (501) staff       (20)      134 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/token/ft/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3241 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/token/ft/jetton_minter.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3155 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/token/ft/jetton_wallet.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.480699 tonsdk-1.0.9/tonsdk/contract/token/nft/
+-rw-r--r--   0 akkireev   (501) staff       (20)      167 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/token/nft/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4473 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/token/nft/nft_collection.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2638 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/token/nft/nft_item.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1975 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/token/nft/nft_sale.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      889 2022-08-22 06:23:56.000000 tonsdk-1.0.9/tonsdk/contract/token/nft/nft_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.484389 tonsdk-1.0.9/tonsdk/contract/wallet/
+-rw-r--r--   0 akkireev   (501) staff       (20)     3087 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/contract/wallet/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     5239 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/contract/wallet/_highload_wallet_contract.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4212 2022-09-18 15:46:05.000000 tonsdk-1.0.9/tonsdk/contract/wallet/_wallet_contract.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1373 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/wallet/_wallet_contract_v2.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1933 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/wallet/_wallet_contract_v3.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4622 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/contract/wallet/_wallet_contract_v4.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.488864 tonsdk-1.0.9/tonsdk/crypto/
+-rw-r--r--   0 akkireev   (501) staff       (20)      322 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/crypto/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      609 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/crypto/_keystore.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1845 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/crypto/_mnemonic.py
+-rw-r--r--   0 akkireev   (501) staff       (20)       26 2022-08-04 10:29:39.000000 tonsdk-1.0.9/tonsdk/crypto/_settings.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1023 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/crypto/_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.490566 tonsdk-1.0.9/tonsdk/crypto/bip39/
+-rw-r--r--   0 akkireev   (501) staff       (20)       68 2022-08-04 10:29:39.000000 tonsdk-1.0.9/tonsdk/crypto/bip39/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    19268 2022-08-04 10:29:39.000000 tonsdk-1.0.9/tonsdk/crypto/bip39/_english.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      138 2022-08-04 10:29:39.000000 tonsdk-1.0.9/tonsdk/crypto/exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.493704 tonsdk-1.0.9/tonsdk/provider/
+-rw-r--r--   0 akkireev   (501) staff       (20)      495 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/provider/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3977 2022-08-22 19:28:07.000000 tonsdk-1.0.9/tonsdk/provider/_address.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      147 2022-08-22 19:28:07.000000 tonsdk-1.0.9/tonsdk/provider/_exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.494757 tonsdk-1.0.9/tonsdk/provider/_toncenter/
+-rw-r--r--   0 akkireev   (501) staff       (20)      124 2022-08-22 19:28:07.000000 tonsdk-1.0.9/tonsdk/provider/_toncenter/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2374 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/provider/_toncenter/_client.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.495678 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/
+-rw-r--r--   0 akkireev   (501) staff       (20)      196 2022-08-22 19:28:07.000000 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.497135 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_async/
+-rw-r--r--   0 akkireev   (501) staff       (20)      153 2022-08-22 19:28:07.000000 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_async/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    31396 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_async/_client.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     6163 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_async/_wrapper.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.498692 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_sync/
+-rw-r--r--   0 akkireev   (501) staff       (20)      141 2022-08-22 19:28:07.000000 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_sync/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4535 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_sync/_client.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2074 2022-08-22 19:28:07.000000 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_sync/_wrapper.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4442 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.499281 tonsdk-1.0.9/tonsdk/provider/_utils/
+-rw-r--r--   0 akkireev   (501) staff       (20)     1245 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/provider/_utils/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4803 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/provider/_wallet.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.502486 tonsdk-1.0.9/tonsdk/utils/
+-rw-r--r--   0 akkireev   (501) staff       (20)      667 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/utils/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4808 2022-08-29 07:57:29.000000 tonsdk-1.0.9/tonsdk/utils/_address.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3004 2022-08-04 10:29:39.000000 tonsdk-1.0.9/tonsdk/utils/_currency.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      134 2022-08-04 10:29:39.000000 tonsdk-1.0.9/tonsdk/utils/_exceptions.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4204 2022-11-16 07:38:08.000000 tonsdk-1.0.9/tonsdk/utils/_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2022-11-16 07:38:47.470536 tonsdk-1.0.9/tonsdk.egg-info/
+-rw-r--r--   0 akkireev   (501) staff       (20)     7422 2022-11-16 07:38:47.000000 tonsdk-1.0.9/tonsdk.egg-info/PKG-INFO
+-rw-r--r--   0 akkireev   (501) staff       (20)     2069 2022-11-16 07:38:47.000000 tonsdk-1.0.9/tonsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 akkireev   (501) staff       (20)        1 2022-11-16 07:38:47.000000 tonsdk-1.0.9/tonsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 akkireev   (501) staff       (20)        1 2022-08-22 20:11:48.000000 tonsdk-1.0.9/tonsdk.egg-info/not-zip-safe
+-rw-r--r--   0 akkireev   (501) staff       (20)       14 2022-11-16 07:38:47.000000 tonsdk-1.0.9/tonsdk.egg-info/requires.txt
+-rw-r--r--   0 akkireev   (501) staff       (20)        7 2022-11-16 07:38:47.000000 tonsdk-1.0.9/tonsdk.egg-info/top_level.txt
```

### Comparing `tonsdk-1.0.7/LICENSE` & `tonsdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/PKG-INFO` & `tonsdk-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonsdk
-Version: 1.0.7
+Version: 1.0.9
 Summary: Python SDK for TON
 Author: tonfactory.org
 License: Apache 2.0
 Project-URL: Github, https://github.com/tonfactory/tonsdk
 Keywords: TON,TON SDK,TON utils,TON tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `tonsdk-1.0.7/README.md` & `tonsdk-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/setup.cfg` & `tonsdk-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tonsdk
-version = 1.0.7
+version = 1.0.9
 description = Python SDK for TON
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = TON, TON SDK, TON utils, TON tools
 license = Apache 2.0
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `tonsdk-1.0.7/tonsdk/boc/_bit_string.py` & `tonsdk-1.0.9/tonsdk/boc/_bit_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,7 +165,10 @@
         if amount == 0:
             self.write_uint(0, 4)
         else:
             amount = int(amount)
             l = math.ceil(len(hex(amount)[2:]) / 2)  # ? [2:] removes 0x
             self.write_uint(l, 4)
             self.write_uint(amount, l * 8)
+
+    def write_coins(self, amount):
+        self.write_grams(amount)
```

### Comparing `tonsdk-1.0.7/tonsdk/boc/_cell.py` & `tonsdk-1.0.9/tonsdk/boc/_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,17 @@
         self.bits = BitString(1023)
         self.refs = []
         self.is_exotic = False
 
     def __repr__(self):
         return "<Cell refs_num: %d, %s>" % (len(self.refs), repr(self.bits))
 
+    def __bool__(self):
+        return bool(self.bits.cursor) or bool(self.refs)
+
     def bytes_hash(self):
         return sha256(self.bytes_repr()).digest()
 
     def bytes_repr(self):
         repr_array = list()
         repr_array.append(self.get_data_with_descriptors())
         for r in self.refs:
```

### Comparing `tonsdk-1.0.7/tonsdk/contract/__init__.py` & `tonsdk-1.0.9/tonsdk/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/token/ft/jetton_minter.py` & `tonsdk-1.0.9/tonsdk/contract/token/ft/jetton_minter.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/token/ft/jetton_wallet.py` & `tonsdk-1.0.9/tonsdk/contract/token/ft/jetton_wallet.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/token/nft/nft_collection.py` & `tonsdk-1.0.9/tonsdk/contract/token/nft/nft_collection.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/token/nft/nft_item.py` & `tonsdk-1.0.9/tonsdk/contract/token/nft/nft_item.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/token/nft/nft_sale.py` & `tonsdk-1.0.9/tonsdk/contract/token/nft/nft_sale.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/token/nft/nft_utils.py` & `tonsdk-1.0.9/tonsdk/contract/token/nft/nft_utils.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/wallet/__init__.py` & `tonsdk-1.0.9/tonsdk/contract/wallet/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,74 +2,77 @@
 from typing import List, Optional, Tuple
 
 from ._wallet_contract import SendModeEnum
 from ._wallet_contract import WalletContract
 from ._wallet_contract_v2 import WalletV2ContractR1, WalletV2ContractR2
 from ._wallet_contract_v3 import WalletV3ContractR1, WalletV3ContractR2
 from ._wallet_contract_v4 import WalletV4ContractR1, WalletV4ContractR2
+from ._highload_wallet_contract import HighloadWalletV2Contract
 from ...crypto import mnemonic_new, mnemonic_to_wallet_key, mnemonic_is_valid
 from ...crypto.exceptions import InvalidMnemonicsError
 
 
 class WalletVersionEnum(str, Enum):
     v2r1 = 'v2r1'
     v2r2 = 'v2r2'
     v3r1 = 'v3r1'
     v3r2 = 'v3r2'
     v4r1 = 'v4r1'
     v4r2 = 'v4r2'
+    hv2 = 'hv2'
 
 
 class Wallets:
     default_version = WalletVersionEnum.v3r2
     ALL = {
         WalletVersionEnum.v2r1: WalletV2ContractR1,
         WalletVersionEnum.v2r2: WalletV2ContractR2,
         WalletVersionEnum.v3r1: WalletV3ContractR1,
         WalletVersionEnum.v3r2: WalletV3ContractR2,
         WalletVersionEnum.v4r1: WalletV4ContractR1,
         WalletVersionEnum.v4r2: WalletV4ContractR2,
+        WalletVersionEnum.hv2: HighloadWalletV2Contract
     }
 
     @classmethod
     def create(cls, version: WalletVersionEnum, workchain: int,
-               password: Optional[str] = None) -> Tuple[List[str], bytes, bytes, WalletContract]:
+               password: Optional[str] = None, **kwargs) -> Tuple[List[str], bytes, bytes, WalletContract]:
         """
         :rtype: (List[str](mnemonics), bytes(public_key), bytes(private_key), WalletContract(wallet))
         """
         mnemonics = mnemonic_new(password=password)
         pub_k, priv_k = mnemonic_to_wallet_key(mnemonics)
         wallet = cls.ALL[version](
-            public_key=pub_k, private_key=priv_k, wc=workchain)
+            public_key=pub_k, private_key=priv_k, wc=workchain, **kwargs)
 
         return mnemonics, pub_k, priv_k, wallet
 
     @classmethod
     def from_mnemonics(cls, mnemonics: List[str], version: WalletVersionEnum = default_version,
-                       workchain: int = 0) -> Tuple[List[str], bytes, bytes, WalletContract]:
+                       workchain: int = 0, **kwargs) -> Tuple[List[str], bytes, bytes, WalletContract]:
         """
         :rtype: (List[str](mnemonics), bytes(public_key), bytes(private_key), WalletContract(wallet))
         """
         if not mnemonic_is_valid(mnemonics):
             raise InvalidMnemonicsError()
 
         pub_k, priv_k = mnemonic_to_wallet_key(mnemonics)
         wallet = cls.ALL[version](
-            public_key=pub_k, private_key=priv_k, wc=workchain)
+            public_key=pub_k, private_key=priv_k, wc=workchain, **kwargs)
 
         return mnemonics, pub_k, priv_k, wallet
 
     @classmethod
     def to_addr_pk(cls, mnemonics: WalletContract, version: WalletVersionEnum = default_version,
-                   workchain: int = 0) -> Tuple[bytes, bytes]:
+                   workchain: int = 0, **kwargs) -> Tuple[bytes, bytes]:
         """
         :rtype: (bytes(addr), bytes(pk)
         """
         _mnemonics, _pub_k, priv_k, wallet = cls.from_mnemonics(
-            mnemonics, version, workchain)
+            mnemonics, version, workchain, **kwargs)
 
         return wallet.address.to_buffer(), priv_k[:32]
 
 
 __all__ = [
     'WalletV2ContractR1',
     'WalletV2ContractR2',
```

### Comparing `tonsdk-1.0.7/tonsdk/contract/wallet/_wallet_contract.py` & `tonsdk-1.0.9/tonsdk/contract/wallet/_wallet_contract.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/wallet/_wallet_contract_v2.py` & `tonsdk-1.0.9/tonsdk/contract/wallet/_wallet_contract_v2.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/wallet/_wallet_contract_v3.py` & `tonsdk-1.0.9/tonsdk/contract/wallet/_wallet_contract_v3.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/contract/wallet/_wallet_contract_v4.py` & `tonsdk-1.0.9/tonsdk/contract/wallet/_wallet_contract_v4.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/crypto/_keystore.py` & `tonsdk-1.0.9/tonsdk/crypto/_keystore.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/crypto/_mnemonic.py` & `tonsdk-1.0.9/tonsdk/crypto/_mnemonic.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/crypto/_utils.py` & `tonsdk-1.0.9/tonsdk/crypto/_utils.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/crypto/bip39/_english.py` & `tonsdk-1.0.9/tonsdk/crypto/bip39/_english.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_address.py` & `tonsdk-1.0.9/tonsdk/provider/_address.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_toncenter/_client.py` & `tonsdk-1.0.9/tonsdk/provider/_toncenter/_client.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_async/_client.py` & `tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_async/_client.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_async/_wrapper.py` & `tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_async/_wrapper.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_sync/_client.py` & `tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_sync/_client.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_sync/_wrapper.py` & `tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_sync/_wrapper.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_tonlibjson/_utils.py` & `tonsdk-1.0.9/tonsdk/provider/_tonlibjson/_utils.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_utils/__init__.py` & `tonsdk-1.0.9/tonsdk/provider/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/provider/_wallet.py` & `tonsdk-1.0.9/tonsdk/provider/_wallet.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/utils/__init__.py` & `tonsdk-1.0.9/tonsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/utils/_address.py` & `tonsdk-1.0.9/tonsdk/utils/_address.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/utils/_currency.py` & `tonsdk-1.0.9/tonsdk/utils/_currency.py`

 * *Files identical despite different names*

### Comparing `tonsdk-1.0.7/tonsdk/utils/_utils.py` & `tonsdk-1.0.9/tonsdk/utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def move_to_end(index_hashmap, topological_order_arr, target):
     target_index = index_hashmap[target]
     for _hash in index_hashmap:
         if index_hashmap[_hash] > target_index:
             index_hashmap[_hash] -= 1
     index_hashmap[target] = len(topological_order_arr) - 1
-    data = topological_order_arr[target_index]
+    data = topological_order_arr.pop(target_index)
     topological_order_arr.append(data)
     for sub_cell in data[1].refs:
         topological_order_arr, index_hashmap = move_to_end(index_hashmap, topological_order_arr, sub_cell.bytes_hash())
     return [topological_order_arr, index_hashmap]
 
 
 def tree_walk(cell, topological_order_arr, index_hashmap, parent_hash=None):
```

### Comparing `tonsdk-1.0.7/tonsdk.egg-info/PKG-INFO` & `tonsdk-1.0.9/tonsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonsdk
-Version: 1.0.7
+Version: 1.0.9
 Summary: Python SDK for TON
 Author: tonfactory.org
 License: Apache 2.0
 Project-URL: Github, https://github.com/tonfactory/tonsdk
 Keywords: TON,TON SDK,TON utils,TON tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `tonsdk-1.0.7/tonsdk.egg-info/SOURCES.txt` & `tonsdk-1.0.9/tonsdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,32 @@
 tonsdk.egg-info/SOURCES.txt
 tonsdk.egg-info/dependency_links.txt
 tonsdk.egg-info/not-zip-safe
 tonsdk.egg-info/requires.txt
 tonsdk.egg-info/top_level.txt
 tonsdk/boc/__init__.py
 tonsdk/boc/_bit_string.py
+tonsdk/boc/_builder.py
 tonsdk/boc/_cell.py
+tonsdk/boc/_dict_builder.py
+tonsdk/boc/dict/__init__.py
+tonsdk/boc/dict/find_common_prefix.py
+tonsdk/boc/dict/serialize_dict.py
 tonsdk/contract/__init__.py
 tonsdk/contract/token/__init__.py
 tonsdk/contract/token/ft/__init__.py
 tonsdk/contract/token/ft/jetton_minter.py
 tonsdk/contract/token/ft/jetton_wallet.py
 tonsdk/contract/token/nft/__init__.py
 tonsdk/contract/token/nft/nft_collection.py
 tonsdk/contract/token/nft/nft_item.py
 tonsdk/contract/token/nft/nft_sale.py
 tonsdk/contract/token/nft/nft_utils.py
 tonsdk/contract/wallet/__init__.py
+tonsdk/contract/wallet/_highload_wallet_contract.py
 tonsdk/contract/wallet/_wallet_contract.py
 tonsdk/contract/wallet/_wallet_contract_v2.py
 tonsdk/contract/wallet/_wallet_contract_v3.py
 tonsdk/contract/wallet/_wallet_contract_v4.py
 tonsdk/crypto/__init__.py
 tonsdk/crypto/_keystore.py
 tonsdk/crypto/_mnemonic.py
```

