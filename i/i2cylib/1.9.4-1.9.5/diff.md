# Comparing `tmp/i2cylib-1.9.4.tar.gz` & `tmp/i2cylib-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cylib-1.9.4.tar", last modified: Sat Jun 11 08:37:52 2022, max compression
+gzip compressed data, was "dist\i2cylib-1.9.5.tar", last modified: Sun Jun 12 07:26:36 2022, max compression
```

## Comparing `i2cylib-1.9.4.tar` & `i2cylib-1.9.5.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.606736 i2cylib-1.9.4/
--rw-rw-rw-   0        0        0     1504 2022-06-11 08:37:52.604193 i2cylib-1.9.4/PKG-INFO
--rw-rw-rw-   0        0        0      644 2022-02-13 10:19:27.000000 i2cylib-1.9.4/README.md
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.178408 i2cylib-1.9.4/i2cylib/
--rw-rw-rw-   0        0        0      429 2022-06-02 04:51:47.000000 i2cylib-1.9.4/i2cylib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.233557 i2cylib-1.9.4/i2cylib/crypto/
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.247748 i2cylib-1.9.4/i2cylib/crypto/I2En/
--rw-rw-rw-   0        0        0      167 2021-09-27 07:24:40.000000 i2cylib-1.9.4/i2cylib/crypto/I2En/__init__.py
--rw-rw-rw-   0        0        0     5747 2022-01-26 16:35:41.000000 i2cylib-1.9.4/i2cylib/crypto/I2En/icen.py
--rw-rw-rw-   0        0        0      198 2022-02-11 12:52:24.000000 i2cylib-1.9.4/i2cylib/crypto/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.258504 i2cylib-1.9.4/i2cylib/crypto/iccode/
--rw-rw-rw-   0        0        0      151 2021-09-09 15:56:57.000000 i2cylib-1.9.4/i2cylib/crypto/iccode/__init__.py
--rw-rw-rw-   0        0        0     6897 2021-09-28 08:01:13.000000 i2cylib-1.9.4/i2cylib/crypto/iccode/iccode.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.275155 i2cylib-1.9.4/i2cylib/crypto/keygen/
--rw-rw-rw-   0        0        0      176 2021-09-09 15:56:54.000000 i2cylib-1.9.4/i2cylib/crypto/keygen/__init__.py
--rw-rw-rw-   0        0        0     2819 2022-05-22 06:51:19.000000 i2cylib-1.9.4/i2cylib/crypto/keygen/dynkey.py
--rw-rw-rw-   0        0        0     1366 2021-09-09 15:56:55.000000 i2cylib-1.9.4/i2cylib/crypto/keygen/time_key.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.286932 i2cylib-1.9.4/i2cylib/crypto/utils/
--rw-rw-rw-   0        0        0      174 2022-02-11 12:52:36.000000 i2cylib-1.9.4/i2cylib/crypto/utils/__init__.py
--rw-rw-rw-   0        0        0      826 2022-01-28 11:34:44.000000 i2cylib-1.9.4/i2cylib/crypto/utils/operators.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.292138 i2cylib-1.9.4/i2cylib/database/
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.313477 i2cylib-1.9.4/i2cylib/database/I2DB/
--rw-rw-rw-   0        0        0      188 2022-02-11 12:53:10.000000 i2cylib-1.9.4/i2cylib/database/I2DB/__init__.py
--rw-rw-rw-   0        0        0    22042 2022-02-07 17:01:26.000000 i2cylib-1.9.4/i2cylib/database/I2DB/i2cydbclient.py
--rw-rw-rw-   0        0        0    12825 2022-02-07 17:01:26.000000 i2cylib-1.9.4/i2cylib/database/I2DB/i2cydbserver.py
--rw-rw-rw-   0        0        0      174 2022-02-11 12:53:31.000000 i2cylib-1.9.4/i2cylib/database/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.332982 i2cylib-1.9.4/i2cylib/database/sqlite/
--rw-rw-rw-   0        0        0      155 2021-09-09 15:56:52.000000 i2cylib-1.9.4/i2cylib/database/sqlite/__init__.py
--rw-rw-rw-   0        0        0    21518 2021-10-01 11:29:41.000000 i2cylib-1.9.4/i2cylib/database/sqlite/sqlitedb.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.344193 i2cylib-1.9.4/i2cylib/engineering/
--rw-rw-rw-   0        0        0      167 2022-02-11 12:53:39.000000 i2cylib-1.9.4/i2cylib/engineering/__init__.py
--rw-rw-rw-   0        0        0     8784 2022-06-11 08:36:53.000000 i2cylib-1.9.4/i2cylib/engineering/pid.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.350236 i2cylib-1.9.4/i2cylib/filesystem/
--rw-rw-rw-   0        0        0      154 2022-02-11 12:53:59.000000 i2cylib-1.9.4/i2cylib/filesystem/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.360831 i2cylib-1.9.4/i2cylib/filesystem/icfat64/
--rw-rw-rw-   0        0        0      152 2022-02-11 12:54:01.000000 i2cylib-1.9.4/i2cylib/filesystem/icfat64/__init__.py
--rw-rw-rw-   0        0        0    34616 2022-02-04 11:22:59.000000 i2cylib-1.9.4/i2cylib/filesystem/icfat64/icfat.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.367869 i2cylib-1.9.4/i2cylib/network/
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.378164 i2cylib-1.9.4/i2cylib/network/I2Pipe/
--rw-rw-rw-   0        0        0      168 2022-02-11 12:54:16.000000 i2cylib-1.9.4/i2cylib/network/I2Pipe/__init__.py
--rw-rw-rw-   0        0        0     1300 2022-02-07 10:47:38.000000 i2cylib-1.9.4/i2cylib/network/I2Pipe/pipe.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.390514 i2cylib-1.9.4/i2cylib/network/I2Scan/
--rw-rw-rw-   0        0        0      147 2021-12-26 16:01:30.000000 i2cylib-1.9.4/i2cylib/network/I2Scan/__init__.py
--rw-rw-rw-   0        0        0    13383 2022-02-13 07:43:30.000000 i2cylib-1.9.4/i2cylib/network/I2Scan/i2scan.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.410194 i2cylib-1.9.4/i2cylib/network/I2TCP/
--rw-rw-rw-   0        0        0      194 2022-02-07 17:10:58.000000 i2cylib-1.9.4/i2cylib/network/I2TCP/__init__.py
--rw-rw-rw-   0        0        0     9917 2022-05-26 09:19:54.000000 i2cylib-1.9.4/i2cylib/network/I2TCP/client.py
--rw-rw-rw-   0        0        0     9985 2022-05-23 07:58:16.000000 i2cylib-1.9.4/i2cylib/network/I2TCP/server.py
--rw-rw-rw-   0        0        0     2329 2022-05-22 18:34:31.000000 i2cylib-1.9.4/i2cylib/network/I2TCP/test.py
--rw-rw-rw-   0        0        0      180 2022-02-12 15:02:25.000000 i2cylib-1.9.4/i2cylib/network/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.427145 i2cylib-1.9.4/i2cylib/network/i2tcp_basic/
--rw-rw-rw-   0        0        0      184 2022-01-26 15:05:08.000000 i2cylib-1.9.4/i2cylib/network/i2tcp_basic/__init__.py
--rw-rw-rw-   0        0        0    14362 2022-05-26 09:19:48.000000 i2cylib-1.9.4/i2cylib/network/i2tcp_basic/base_client.py
--rw-rw-rw-   0        0        0    23733 2022-05-26 09:19:50.000000 i2cylib-1.9.4/i2cylib/network/i2tcp_basic/base_server.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.433166 i2cylib-1.9.4/i2cylib/serial/
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.443308 i2cylib-1.9.4/i2cylib/serial/HTprot/
--rw-rw-rw-   0        0        0      173 2022-05-31 12:14:28.000000 i2cylib-1.9.4/i2cylib/serial/HTprot/__init__.py
--rw-rw-rw-   0        0        0     4885 2022-05-31 12:19:13.000000 i2cylib-1.9.4/i2cylib/serial/HTprot/htsocket.py
--rw-rw-rw-   0        0        0      169 2022-05-31 12:14:28.000000 i2cylib-1.9.4/i2cylib/serial/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.448316 i2cylib-1.9.4/i2cylib/utils/
--rw-rw-rw-   0        0        0      347 2022-05-12 08:38:15.000000 i2cylib-1.9.4/i2cylib/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.463532 i2cylib-1.9.4/i2cylib/utils/args/
--rw-rw-rw-   0        0        0      181 2021-09-09 15:57:07.000000 i2cylib-1.9.4/i2cylib/utils/args/__init__.py
--rw-rw-rw-   0        0        0      946 2021-09-09 15:57:08.000000 i2cylib-1.9.4/i2cylib/utils/args/decode_args.py
--rw-rw-rw-   0        0        0      716 2022-05-18 09:10:01.000000 i2cylib-1.9.4/i2cylib/utils/args/get_args.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.479185 i2cylib-1.9.4/i2cylib/utils/bytes/
--rw-rw-rw-   0        0        0      191 2021-09-09 15:57:12.000000 i2cylib-1.9.4/i2cylib/utils/bytes/__init__.py
--rw-rw-rw-   0        0        0     2081 2021-09-09 15:57:13.000000 i2cylib-1.9.4/i2cylib/utils/bytes/data_transform.py
--rw-rw-rw-   0        0        0      301 2021-09-09 15:57:13.000000 i2cylib-1.9.4/i2cylib/utils/bytes/random_bytesgen.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.492248 i2cylib-1.9.4/i2cylib/utils/delay/
--rw-rw-rw-   0        0        0      155 2021-09-09 15:57:19.000000 i2cylib-1.9.4/i2cylib/utils/delay/__init__.py
--rw-rw-rw-   0        0        0     2000 2021-09-09 15:57:18.000000 i2cylib-1.9.4/i2cylib/utils/delay/normal_delay.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.508097 i2cylib-1.9.4/i2cylib/utils/files/
--rw-rw-rw-   0        0        0      185 2021-09-09 15:57:10.000000 i2cylib-1.9.4/i2cylib/utils/files/__init__.py
--rw-rw-rw-   0        0        0      455 2021-09-09 15:57:11.000000 i2cylib-1.9.4/i2cylib/utils/files/hash_file.py
--rw-rw-rw-   0        0        0      419 2021-09-09 15:57:10.000000 i2cylib-1.9.4/i2cylib/utils/files/import_scripts.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.518376 i2cylib-1.9.4/i2cylib/utils/logger/
--rw-rw-rw-   0        0        0      151 2021-09-09 15:57:19.000000 i2cylib-1.9.4/i2cylib/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     4203 2022-05-22 06:51:19.000000 i2cylib-1.9.4/i2cylib/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.535134 i2cylib-1.9.4/i2cylib/utils/os/
--rw-rw-rw-   0        0        0      187 2021-09-09 15:57:08.000000 i2cylib-1.9.4/i2cylib/utils/os/__init__.py
--rw-rw-rw-   0        0        0      995 2022-01-06 19:35:23.000000 i2cylib-1.9.4/i2cylib/utils/os/linux_hddtemp.py
--rw-rw-rw-   0        0        0      537 2021-09-09 15:57:09.000000 i2cylib-1.9.4/i2cylib/utils/os/win_tasklist.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.561583 i2cylib-1.9.4/i2cylib/utils/path/
--rw-rw-rw-   0        0        0      207 2021-09-09 15:57:15.000000 i2cylib-1.9.4/i2cylib/utils/path/__init__.py
--rw-rw-rw-   0        0        0      423 2021-09-09 15:57:17.000000 i2cylib-1.9.4/i2cylib/utils/path/path_fixer.py
--rw-rw-rw-   0        0        0      393 2021-09-09 15:57:16.000000 i2cylib-1.9.4/i2cylib/utils/path/read_path.py
--rw-rw-rw-   0        0        0     1122 2021-09-09 15:57:16.000000 i2cylib-1.9.4/i2cylib/utils/path/scan_path.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.573776 i2cylib-1.9.4/i2cylib/utils/stdout/
--rw-rw-rw-   0        0        0      149 2021-09-09 15:57:21.000000 i2cylib-1.9.4/i2cylib/utils/stdout/__init__.py
--rw-rw-rw-   0        0        0     1695 2021-09-09 15:57:20.000000 i2cylib-1.9.4/i2cylib/utils/stdout/echo.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.584160 i2cylib-1.9.4/i2cylib/utils/string/
--rw-rw-rw-   0        0        0      155 2021-09-09 15:57:14.000000 i2cylib-1.9.4/i2cylib/utils/string/__init__.py
--rw-rw-rw-   0        0        0     1039 2021-09-09 15:57:14.000000 i2cylib-1.9.4/i2cylib/utils/string/text_match.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.596743 i2cylib-1.9.4/i2cylib/utils/time/
--rw-rw-rw-   0        0        0      153 2021-09-09 15:57:11.000000 i2cylib-1.9.4/i2cylib/utils/time/__init__.py
--rw-rw-rw-   0        0        0      401 2021-09-09 15:57:12.000000 i2cylib-1.9.4/i2cylib/utils/time/trf_time.py
-drwxrwxrwx   0        0        0        0 2022-06-11 08:37:52.227069 i2cylib-1.9.4/i2cylib.egg-info/
--rw-rw-rw-   0        0        0     1504 2022-06-11 08:37:51.000000 i2cylib-1.9.4/i2cylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2330 2022-06-11 08:37:51.000000 i2cylib-1.9.4/i2cylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-11 08:37:51.000000 i2cylib-1.9.4/i2cylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2022-06-11 08:37:51.000000 i2cylib-1.9.4/i2cylib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2022-06-11 08:37:51.000000 i2cylib-1.9.4/i2cylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-06-11 08:37:51.000000 i2cylib-1.9.4/i2cylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-09-09 15:54:19.000000 i2cylib-1.9.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-06-11 08:37:52.607779 i2cylib-1.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1400 2022-06-11 08:37:41.000000 i2cylib-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.885491 i2cylib-1.9.5/
+-rw-rw-rw-   0        0        0     1504 2022-06-12 07:26:36.884498 i2cylib-1.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2022-02-13 10:19:27.000000 i2cylib-1.9.5/README.md
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.724786 i2cylib-1.9.5/i2cylib/
+-rw-rw-rw-   0        0        0      429 2022-06-02 04:51:47.000000 i2cylib-1.9.5/i2cylib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.765954 i2cylib-1.9.5/i2cylib/crypto/
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.769425 i2cylib-1.9.5/i2cylib/crypto/I2En/
+-rw-rw-rw-   0        0        0      167 2021-09-27 07:24:40.000000 i2cylib-1.9.5/i2cylib/crypto/I2En/__init__.py
+-rw-rw-rw-   0        0        0     5747 2022-01-26 16:35:41.000000 i2cylib-1.9.5/i2cylib/crypto/I2En/icen.py
+-rw-rw-rw-   0        0        0      198 2022-02-11 12:52:24.000000 i2cylib-1.9.5/i2cylib/crypto/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.772898 i2cylib-1.9.5/i2cylib/crypto/iccode/
+-rw-rw-rw-   0        0        0      151 2021-09-09 15:56:57.000000 i2cylib-1.9.5/i2cylib/crypto/iccode/__init__.py
+-rw-rw-rw-   0        0        0     6897 2021-09-28 08:01:13.000000 i2cylib-1.9.5/i2cylib/crypto/iccode/iccode.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.778850 i2cylib-1.9.5/i2cylib/crypto/keygen/
+-rw-rw-rw-   0        0        0      176 2021-09-09 15:56:54.000000 i2cylib-1.9.5/i2cylib/crypto/keygen/__init__.py
+-rw-rw-rw-   0        0        0     2819 2022-05-22 06:51:19.000000 i2cylib-1.9.5/i2cylib/crypto/keygen/dynkey.py
+-rw-rw-rw-   0        0        0     1366 2021-09-09 15:56:55.000000 i2cylib-1.9.5/i2cylib/crypto/keygen/time_key.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.782818 i2cylib-1.9.5/i2cylib/crypto/utils/
+-rw-rw-rw-   0        0        0      174 2022-02-11 12:52:36.000000 i2cylib-1.9.5/i2cylib/crypto/utils/__init__.py
+-rw-rw-rw-   0        0        0      826 2022-01-28 11:34:44.000000 i2cylib-1.9.5/i2cylib/crypto/utils/operators.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.784802 i2cylib-1.9.5/i2cylib/database/
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.790259 i2cylib-1.9.5/i2cylib/database/I2DB/
+-rw-rw-rw-   0        0        0      188 2022-02-11 12:53:10.000000 i2cylib-1.9.5/i2cylib/database/I2DB/__init__.py
+-rw-rw-rw-   0        0        0    22042 2022-02-07 17:01:26.000000 i2cylib-1.9.5/i2cylib/database/I2DB/i2cydbclient.py
+-rw-rw-rw-   0        0        0    12825 2022-02-07 17:01:26.000000 i2cylib-1.9.5/i2cylib/database/I2DB/i2cydbserver.py
+-rw-rw-rw-   0        0        0      174 2022-02-11 12:53:31.000000 i2cylib-1.9.5/i2cylib/database/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.793730 i2cylib-1.9.5/i2cylib/database/sqlite/
+-rw-rw-rw-   0        0        0      155 2021-09-09 15:56:52.000000 i2cylib-1.9.5/i2cylib/database/sqlite/__init__.py
+-rw-rw-rw-   0        0        0    21518 2021-10-01 11:29:41.000000 i2cylib-1.9.5/i2cylib/database/sqlite/sqlitedb.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.797700 i2cylib-1.9.5/i2cylib/engineering/
+-rw-rw-rw-   0        0        0      167 2022-02-11 12:53:39.000000 i2cylib-1.9.5/i2cylib/engineering/__init__.py
+-rw-rw-rw-   0        0        0     8784 2022-06-12 07:20:01.000000 i2cylib-1.9.5/i2cylib/engineering/pid.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.799682 i2cylib-1.9.5/i2cylib/filesystem/
+-rw-rw-rw-   0        0        0      154 2022-02-11 12:53:59.000000 i2cylib-1.9.5/i2cylib/filesystem/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.803650 i2cylib-1.9.5/i2cylib/filesystem/icfat64/
+-rw-rw-rw-   0        0        0      152 2022-02-11 12:54:01.000000 i2cylib-1.9.5/i2cylib/filesystem/icfat64/__init__.py
+-rw-rw-rw-   0        0        0    34616 2022-02-04 11:22:59.000000 i2cylib-1.9.5/i2cylib/filesystem/icfat64/icfat.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.806130 i2cylib-1.9.5/i2cylib/network/
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.810595 i2cylib-1.9.5/i2cylib/network/I2Pipe/
+-rw-rw-rw-   0        0        0      168 2022-02-11 12:54:16.000000 i2cylib-1.9.5/i2cylib/network/I2Pipe/__init__.py
+-rw-rw-rw-   0        0        0     1300 2022-02-07 10:47:38.000000 i2cylib-1.9.5/i2cylib/network/I2Pipe/pipe.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.814562 i2cylib-1.9.5/i2cylib/network/I2Scan/
+-rw-rw-rw-   0        0        0      147 2021-12-26 16:01:30.000000 i2cylib-1.9.5/i2cylib/network/I2Scan/__init__.py
+-rw-rw-rw-   0        0        0    13383 2022-02-13 07:43:30.000000 i2cylib-1.9.5/i2cylib/network/I2Scan/i2scan.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.821538 i2cylib-1.9.5/i2cylib/network/I2TCP/
+-rw-rw-rw-   0        0        0      194 2022-02-07 17:10:58.000000 i2cylib-1.9.5/i2cylib/network/I2TCP/__init__.py
+-rw-rw-rw-   0        0        0     9917 2022-05-26 09:19:54.000000 i2cylib-1.9.5/i2cylib/network/I2TCP/client.py
+-rw-rw-rw-   0        0        0     9985 2022-05-23 07:58:16.000000 i2cylib-1.9.5/i2cylib/network/I2TCP/server.py
+-rw-rw-rw-   0        0        0     2329 2022-05-22 18:34:31.000000 i2cylib-1.9.5/i2cylib/network/I2TCP/test.py
+-rw-rw-rw-   0        0        0      180 2022-02-12 15:02:25.000000 i2cylib-1.9.5/i2cylib/network/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.826962 i2cylib-1.9.5/i2cylib/network/i2tcp_basic/
+-rw-rw-rw-   0        0        0      184 2022-01-26 15:05:08.000000 i2cylib-1.9.5/i2cylib/network/i2tcp_basic/__init__.py
+-rw-rw-rw-   0        0        0    14362 2022-05-26 09:19:48.000000 i2cylib-1.9.5/i2cylib/network/i2tcp_basic/base_client.py
+-rw-rw-rw-   0        0        0    23733 2022-05-26 09:19:50.000000 i2cylib-1.9.5/i2cylib/network/i2tcp_basic/base_server.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.828978 i2cylib-1.9.5/i2cylib/serial/
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.833410 i2cylib-1.9.5/i2cylib/serial/HTprot/
+-rw-rw-rw-   0        0        0      173 2022-05-31 12:14:28.000000 i2cylib-1.9.5/i2cylib/serial/HTprot/__init__.py
+-rw-rw-rw-   0        0        0     5047 2022-06-12 07:25:25.000000 i2cylib-1.9.5/i2cylib/serial/HTprot/htsocket.py
+-rw-rw-rw-   0        0        0      169 2022-05-31 12:14:28.000000 i2cylib-1.9.5/i2cylib/serial/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.835394 i2cylib-1.9.5/i2cylib/utils/
+-rw-rw-rw-   0        0        0      347 2022-05-12 08:38:15.000000 i2cylib-1.9.5/i2cylib/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.841345 i2cylib-1.9.5/i2cylib/utils/args/
+-rw-rw-rw-   0        0        0      181 2021-09-09 15:57:07.000000 i2cylib-1.9.5/i2cylib/utils/args/__init__.py
+-rw-rw-rw-   0        0        0      946 2021-09-09 15:57:08.000000 i2cylib-1.9.5/i2cylib/utils/args/decode_args.py
+-rw-rw-rw-   0        0        0      716 2022-05-18 09:10:01.000000 i2cylib-1.9.5/i2cylib/utils/args/get_args.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.850273 i2cylib-1.9.5/i2cylib/utils/bytes/
+-rw-rw-rw-   0        0        0      191 2021-09-09 15:57:12.000000 i2cylib-1.9.5/i2cylib/utils/bytes/__init__.py
+-rw-rw-rw-   0        0        0     2081 2021-09-09 15:57:13.000000 i2cylib-1.9.5/i2cylib/utils/bytes/data_transform.py
+-rw-rw-rw-   0        0        0      301 2021-09-09 15:57:13.000000 i2cylib-1.9.5/i2cylib/utils/bytes/random_bytesgen.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.853747 i2cylib-1.9.5/i2cylib/utils/delay/
+-rw-rw-rw-   0        0        0      155 2021-09-09 15:57:19.000000 i2cylib-1.9.5/i2cylib/utils/delay/__init__.py
+-rw-rw-rw-   0        0        0     2000 2021-09-09 15:57:18.000000 i2cylib-1.9.5/i2cylib/utils/delay/normal_delay.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.859698 i2cylib-1.9.5/i2cylib/utils/files/
+-rw-rw-rw-   0        0        0      185 2021-09-09 15:57:10.000000 i2cylib-1.9.5/i2cylib/utils/files/__init__.py
+-rw-rw-rw-   0        0        0      455 2021-09-09 15:57:11.000000 i2cylib-1.9.5/i2cylib/utils/files/hash_file.py
+-rw-rw-rw-   0        0        0      419 2021-09-09 15:57:10.000000 i2cylib-1.9.5/i2cylib/utils/files/import_scripts.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.863170 i2cylib-1.9.5/i2cylib/utils/logger/
+-rw-rw-rw-   0        0        0      151 2021-09-09 15:57:19.000000 i2cylib-1.9.5/i2cylib/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     4203 2022-05-22 06:51:19.000000 i2cylib-1.9.5/i2cylib/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.867633 i2cylib-1.9.5/i2cylib/utils/os/
+-rw-rw-rw-   0        0        0      187 2021-09-09 15:57:08.000000 i2cylib-1.9.5/i2cylib/utils/os/__init__.py
+-rw-rw-rw-   0        0        0      995 2022-01-06 19:35:23.000000 i2cylib-1.9.5/i2cylib/utils/os/linux_hddtemp.py
+-rw-rw-rw-   0        0        0      537 2021-09-09 15:57:09.000000 i2cylib-1.9.5/i2cylib/utils/os/win_tasklist.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.873585 i2cylib-1.9.5/i2cylib/utils/path/
+-rw-rw-rw-   0        0        0      207 2021-09-09 15:57:15.000000 i2cylib-1.9.5/i2cylib/utils/path/__init__.py
+-rw-rw-rw-   0        0        0      423 2021-09-09 15:57:17.000000 i2cylib-1.9.5/i2cylib/utils/path/path_fixer.py
+-rw-rw-rw-   0        0        0      393 2021-09-09 15:57:16.000000 i2cylib-1.9.5/i2cylib/utils/path/read_path.py
+-rw-rw-rw-   0        0        0     1122 2021-09-09 15:57:16.000000 i2cylib-1.9.5/i2cylib/utils/path/scan_path.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.877059 i2cylib-1.9.5/i2cylib/utils/stdout/
+-rw-rw-rw-   0        0        0      149 2021-09-09 15:57:21.000000 i2cylib-1.9.5/i2cylib/utils/stdout/__init__.py
+-rw-rw-rw-   0        0        0     1695 2021-09-09 15:57:20.000000 i2cylib-1.9.5/i2cylib/utils/stdout/echo.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.880035 i2cylib-1.9.5/i2cylib/utils/string/
+-rw-rw-rw-   0        0        0      155 2021-09-09 15:57:14.000000 i2cylib-1.9.5/i2cylib/utils/string/__init__.py
+-rw-rw-rw-   0        0        0     1039 2021-09-09 15:57:14.000000 i2cylib-1.9.5/i2cylib/utils/string/text_match.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.883010 i2cylib-1.9.5/i2cylib/utils/time/
+-rw-rw-rw-   0        0        0      153 2021-09-09 15:57:11.000000 i2cylib-1.9.5/i2cylib/utils/time/__init__.py
+-rw-rw-rw-   0        0        0      401 2021-09-09 15:57:12.000000 i2cylib-1.9.5/i2cylib/utils/time/trf_time.py
+drwxrwxrwx   0        0        0        0 2022-06-12 07:26:36.763971 i2cylib-1.9.5/i2cylib.egg-info/
+-rw-rw-rw-   0        0        0     1504 2022-06-12 07:26:36.000000 i2cylib-1.9.5/i2cylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2330 2022-06-12 07:26:36.000000 i2cylib-1.9.5/i2cylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-12 07:26:36.000000 i2cylib-1.9.5/i2cylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2022-06-12 07:26:36.000000 i2cylib-1.9.5/i2cylib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2022-06-12 07:26:36.000000 i2cylib-1.9.5/i2cylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-06-12 07:26:36.000000 i2cylib-1.9.5/i2cylib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-09-09 15:54:19.000000 i2cylib-1.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-06-12 07:26:36.885491 i2cylib-1.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2022-06-12 07:26:30.000000 i2cylib-1.9.5/setup.py
```

### Comparing `i2cylib-1.9.4/PKG-INFO` & `i2cylib-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cylib
-Version: 1.9.4
+Version: 1.9.5
 Summary: A Python library contains a lot of useful functions and tools
 Home-page: https://github.com/i2cy/i2cylib
 Author: I2cy Cloud
 Author-email: i2cy@outlook.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/i2cy/i2cylib/issues
 Project-URL: Source Code, https://github.com/i2cy/i2cylib
```

### Comparing `i2cylib-1.9.4/README.md` & `i2cylib-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/crypto/I2En/icen.py` & `i2cylib-1.9.5/i2cylib/crypto/I2En/icen.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/crypto/iccode/iccode.py` & `i2cylib-1.9.5/i2cylib/crypto/iccode/iccode.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/crypto/keygen/dynkey.py` & `i2cylib-1.9.5/i2cylib/crypto/keygen/dynkey.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/crypto/keygen/time_key.py` & `i2cylib-1.9.5/i2cylib/crypto/keygen/time_key.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/crypto/utils/operators.py` & `i2cylib-1.9.5/i2cylib/crypto/utils/operators.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/database/I2DB/i2cydbclient.py` & `i2cylib-1.9.5/i2cylib/database/I2DB/i2cydbclient.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/database/I2DB/i2cydbserver.py` & `i2cylib-1.9.5/i2cylib/database/I2DB/i2cydbserver.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/database/sqlite/sqlitedb.py` & `i2cylib-1.9.5/i2cylib/database/sqlite/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/engineering/pid.py` & `i2cylib-1.9.5/i2cylib/engineering/pid.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/filesystem/icfat64/icfat.py` & `i2cylib-1.9.5/i2cylib/filesystem/icfat64/icfat.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/network/I2Pipe/pipe.py` & `i2cylib-1.9.5/i2cylib/network/I2Pipe/pipe.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/network/I2Scan/i2scan.py` & `i2cylib-1.9.5/i2cylib/network/I2Scan/i2scan.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/network/I2TCP/client.py` & `i2cylib-1.9.5/i2cylib/network/I2TCP/client.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/network/I2TCP/server.py` & `i2cylib-1.9.5/i2cylib/network/I2TCP/server.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/network/I2TCP/test.py` & `i2cylib-1.9.5/i2cylib/network/I2TCP/test.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/network/i2tcp_basic/base_client.py` & `i2cylib-1.9.5/i2cylib/network/i2tcp_basic/base_client.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/network/i2tcp_basic/base_server.py` & `i2cylib-1.9.5/i2cylib/network/i2tcp_basic/base_server.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/serial/HTprot/htsocket.py` & `i2cylib-1.9.5/i2cylib/serial/HTprot/htsocket.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 # Author: i2cy(i2cy@outlook.com)
 # Project: I2cyLib
 # Filename: htsocket
 # Created on: 2022/5/31
+import time
 
 import serial
 from i2cylib.utils.logger.logger import *
 
 
 class HTSocket:
 
@@ -23,14 +24,15 @@
         """
 
         self.head = head
         self.baudrate = baudrate
         self.port = port
         self.client = None
         self.timeout = timeout
+        self.__lock = False
 
     def connect(self, port=None, baudrate=None, timeout=None):
         """
         connect to the target
 
         :param port: int or None
         :param baudrate: int or None
@@ -92,14 +94,18 @@
 
         t = time.time()
         ret = None
         data = self.__pack(addr, data, send_length=send_length)
 
         # print(data)
 
+        while self.__lock:
+            time.sleep(0.001)
+        self.__lock = True
+
         while True:
             ret = self.client.write(data)
 
             if check:
                 if time.time() - t > 2 * self.timeout:
                     ret = False
                     break
@@ -107,14 +113,16 @@
                 if fb == b"OK":
                     break
             else:
                 break
 
             time.sleep(0.05)
 
+        self.__lock = False
+
         return ret
 
     def recv(self, addr, length=None):
         """
         serial receive function
 
         :param addr: bytes
```

### Comparing `i2cylib-1.9.4/i2cylib/utils/args/decode_args.py` & `i2cylib-1.9.5/i2cylib/utils/args/decode_args.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/args/get_args.py` & `i2cylib-1.9.5/i2cylib/utils/args/get_args.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/bytes/data_transform.py` & `i2cylib-1.9.5/i2cylib/utils/bytes/data_transform.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/delay/normal_delay.py` & `i2cylib-1.9.5/i2cylib/utils/delay/normal_delay.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/logger/logger.py` & `i2cylib-1.9.5/i2cylib/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/os/linux_hddtemp.py` & `i2cylib-1.9.5/i2cylib/utils/os/linux_hddtemp.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/os/win_tasklist.py` & `i2cylib-1.9.5/i2cylib/utils/os/win_tasklist.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/path/scan_path.py` & `i2cylib-1.9.5/i2cylib/utils/path/scan_path.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/stdout/echo.py` & `i2cylib-1.9.5/i2cylib/utils/stdout/echo.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib/utils/string/text_match.py` & `i2cylib-1.9.5/i2cylib/utils/string/text_match.py`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/i2cylib.egg-info/PKG-INFO` & `i2cylib-1.9.5/i2cylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cylib
-Version: 1.9.4
+Version: 1.9.5
 Summary: A Python library contains a lot of useful functions and tools
 Home-page: https://github.com/i2cy/i2cylib
 Author: I2cy Cloud
 Author-email: i2cy@outlook.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/i2cy/i2cylib/issues
 Project-URL: Source Code, https://github.com/i2cy/i2cylib
```

### Comparing `i2cylib-1.9.4/i2cylib.egg-info/SOURCES.txt` & `i2cylib-1.9.5/i2cylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i2cylib-1.9.4/setup.py` & `i2cylib-1.9.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# Author: i2cy(i2cy@outlook.com)
-# Filename: setup
-# Created on: 2021/3/6
-
-import setuptools
-
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="i2cylib",  # Replace with your own username
-    version="1.9.4",
-    author="I2cy Cloud",
-    author_email="i2cy@outlook.com",
-    description="A Python library contains a lot of useful functions and tools",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/i2cy/i2cylib",
-    project_urls={
-        "Bug Tracker": "https://github.com/i2cy/i2cylib/issues",
-        "Source Code": "https://github.com/i2cy/i2cylib",
-        "Documentation": "https://github.com/i2cy/I2cylib/wiki/API-Document"
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    install_requires=[
-        'numpy',
-        'tqdm',
-        'rsa',
-        'pyserial'
-    ],
-    packages=setuptools.find_packages(),
-    python_requires=">=3.6",
-    entry_points={'console_scripts':
-        [
-            "i2cydbserver = i2cylib.database.I2DB.i2cydbserver:main",
-            "i2en = i2cylib.crypto.I2En.icen:main",
-            "i2scan = i2cylib.network.I2Scan.i2scan:main"
-        ]
-    }
-)
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# Author: i2cy(i2cy@outlook.com)
+# Filename: setup
+# Created on: 2021/3/6
+
+import setuptools
+
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+ 
+setuptools.setup(
+    name="i2cylib",  # Replace with your own username
+    version="1.9.5",
+    author="I2cy Cloud",
+    author_email="i2cy@outlook.com",
+    description="A Python library contains a lot of useful functions and tools",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/i2cy/i2cylib",
+    project_urls={
+        "Bug Tracker": "https://github.com/i2cy/i2cylib/issues",
+        "Source Code": "https://github.com/i2cy/i2cylib",
+        "Documentation": "https://github.com/i2cy/I2cylib/wiki/API-Document"
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=[
+        'numpy',
+        'tqdm',
+        'rsa',
+        'pyserial'
+    ],
+    packages=setuptools.find_packages(),
+    python_requires=">=3.6",
+    entry_points={'console_scripts':
+        [
+            "i2cydbserver = i2cylib.database.I2DB.i2cydbserver:main",
+            "i2en = i2cylib.crypto.I2En.icen:main",
+            "i2scan = i2cylib.network.I2Scan.i2scan:main"
+        ]
+    }
+)
```

