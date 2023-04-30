# Comparing `tmp/sleuren-1.0.4.tar.gz` & `tmp/sleuren-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleuren-1.0.4.tar", last modified: Tue Apr  4 20:29:25 2023, max compression
+gzip compressed data, was "sleuren-1.0.5.tar", last modified: Sun Apr 30 14:37:00 2023, max compression
```

## Comparing `sleuren-1.0.4.tar` & `sleuren-1.0.5.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:29:25.478360 sleuren-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-04 20:29:16.000000 sleuren-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-04 20:29:25.478360 sleuren-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-04 20:29:16.000000 sleuren-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 20:29:25.478360 sleuren-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-04 20:29:16.000000 sleuren-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:29:25.470359 sleuren-1.0.4/sleuren/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:29:25.478360 sleuren-1.0.4/sleuren/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/apt-updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/asterisk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/bitninja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/cloudlinux-dbgov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/cloudlinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/cpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/cpu_freq.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/dirsize.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/diskinodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/diskstatus-nvme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/diskstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4138 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/diskusage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/exim.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/haproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/httpd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5227 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/iostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/janus.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/kamailio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/litespeed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/loadavg.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/mailq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/mdstat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/megacli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/memcached.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/openvpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/phpfpm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/plesk-cgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/powerdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/redis_stat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/sleeper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/unbound.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/vms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/wp-toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/plugins/yum-updates.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren/sleuren.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:29:25.474359 sleuren-1.0.4/sleuren.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-04 20:29:25.000000 sleuren-1.0.4/sleuren.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-04 20:29:25.000000 sleuren-1.0.4/sleuren.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:29:25.000000 sleuren-1.0.4/sleuren.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-04 20:29:25.000000 sleuren-1.0.4/sleuren.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 20:29:25.000000 sleuren-1.0.4/sleuren.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 20:29:25.000000 sleuren-1.0.4/sleuren.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-04 20:29:16.000000 sleuren-1.0.4/sleuren.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:37:00.469946 sleuren-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-30 14:36:51.000000 sleuren-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-30 14:37:00.469946 sleuren-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-30 14:36:51.000000 sleuren-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:37:00.469946 sleuren-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-30 14:36:51.000000 sleuren-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:37:00.461946 sleuren-1.0.5/sleuren/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:37:00.469946 sleuren-1.0.5/sleuren/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/apt-updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/asterisk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/bitninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/cloudlinux-dbgov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/cloudlinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/cpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/cpu_freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/dirsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/diskinodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/diskstatus-nvme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/diskstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4138 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/diskusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/exim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/haproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/httpd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5227 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/iostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/janus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/kamailio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/litespeed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/loadavg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/loggedin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/mailq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/mdstat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/megacli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/memcached.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/openvpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/phpfpm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/plesk-cgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/powerdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/redis_stat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/sleeper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/unbound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/vms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/wp-toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/plugins/yum-updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren/sleuren.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:37:00.461946 sleuren-1.0.5/sleuren.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-30 14:37:00.000000 sleuren-1.0.5/sleuren.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-30 14:37:00.000000 sleuren-1.0.5/sleuren.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:37:00.000000 sleuren-1.0.5/sleuren.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-30 14:37:00.000000 sleuren-1.0.5/sleuren.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 14:37:00.000000 sleuren-1.0.5/sleuren.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 14:37:00.000000 sleuren-1.0.5/sleuren.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-30 14:36:51.000000 sleuren-1.0.5/sleuren.ini
```

### Comparing `sleuren-1.0.4/LICENSE` & `sleuren-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/PKG-INFO` & `sleuren-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleuren
-Version: 1.0.4
+Version: 1.0.5
 Summary: Server monitoring agent
 Home-page: https://github.com/sleuren/agent
 Author: sleuren
 Author-email: hello@sleuren.com
 Maintainer: sleuren
 Maintainer-email: hello@sleuren.com
 License: MIT
```

### Comparing `sleuren-1.0.4/README.md` & `sleuren-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/setup.py` & `sleuren-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     install_requires = ['psutil==5.6.7', 'netifaces', 'configparser==3.5.0', 'future']
 else:
     install_requires = ['psutil', 'netifaces', 'configparser', 'future']
 
 
 setuptools.setup(
     name='sleuren',
-    version='1.0.4',
+    version='1.0.5',
     description='Server monitoring agent',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/sleuren/agent',
     author='sleuren',
     author_email='hello@sleuren.com',
     maintainer='sleuren',
```

### Comparing `sleuren-1.0.4/sleuren/plugins/apt-updates.py` & `sleuren-1.0.5/sleuren/plugins/apt-updates.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/asterisk.py` & `sleuren-1.0.5/sleuren/plugins/asterisk.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/bitninja.py` & `sleuren-1.0.5/sleuren/plugins/bitninja.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/cloudlinux-dbgov.py` & `sleuren-1.0.5/sleuren/plugins/cloudlinux-dbgov.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/cloudlinux.py` & `sleuren-1.0.5/sleuren/plugins/cloudlinux.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/cpanel.py` & `sleuren-1.0.5/sleuren/plugins/cpanel.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/cpu.py` & `sleuren-1.0.5/sleuren/plugins/cpu.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/cpu_freq.py` & `sleuren-1.0.5/sleuren/plugins/cpu_freq.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/dirsize.py` & `sleuren-1.0.5/sleuren/plugins/dirsize.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/diskinodes.py` & `sleuren-1.0.5/sleuren/plugins/diskinodes.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/diskstatus-nvme.py` & `sleuren-1.0.5/sleuren/plugins/diskstatus-nvme.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/diskstatus.py` & `sleuren-1.0.5/sleuren/plugins/diskstatus.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/diskusage.py` & `sleuren-1.0.5/sleuren/plugins/diskusage.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/docker.py` & `sleuren-1.0.5/sleuren/plugins/docker.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/elasticsearch.py` & `sleuren-1.0.5/sleuren/plugins/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/gpu.py` & `sleuren-1.0.5/sleuren/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/haproxy.py` & `sleuren-1.0.5/sleuren/plugins/haproxy.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/httpd.py` & `sleuren-1.0.5/sleuren/plugins/httpd.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/iostat.py` & `sleuren-1.0.5/sleuren/plugins/iostat.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/janus.py` & `sleuren-1.0.5/sleuren/plugins/janus.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/kamailio.py` & `sleuren-1.0.5/sleuren/plugins/kamailio.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/litespeed.py` & `sleuren-1.0.5/sleuren/plugins/litespeed.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/mailq.py` & `sleuren-1.0.5/sleuren/plugins/mailq.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/mdstat.py` & `sleuren-1.0.5/sleuren/plugins/mdstat.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/megacli.py` & `sleuren-1.0.5/sleuren/plugins/megacli.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/memcached.py` & `sleuren-1.0.5/sleuren/plugins/memcached.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/memory.py` & `sleuren-1.0.5/sleuren/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/minecraft.py` & `sleuren-1.0.5/sleuren/plugins/minecraft.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/mongodb.py` & `sleuren-1.0.5/sleuren/plugins/mongodb.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/mysql.py` & `sleuren-1.0.5/sleuren/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/network.py` & `sleuren-1.0.5/sleuren/plugins/network.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/nginx.py` & `sleuren-1.0.5/sleuren/plugins/nginx.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/openvpn.py` & `sleuren-1.0.5/sleuren/plugins/openvpn.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/phpfpm.py` & `sleuren-1.0.5/sleuren/plugins/phpfpm.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/ping.py` & `sleuren-1.0.5/sleuren/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/plesk-cgroups.py` & `sleuren-1.0.5/sleuren/plugins/plesk-cgroups.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/plugins.py` & `sleuren-1.0.5/sleuren/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/powerdns.py` & `sleuren-1.0.5/sleuren/plugins/powerdns.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/process.py` & `sleuren-1.0.5/sleuren/plugins/process.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/rabbitmq.py` & `sleuren-1.0.5/sleuren/plugins/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/redis_stat.py` & `sleuren-1.0.5/sleuren/plugins/redis_stat.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/system.py` & `sleuren-1.0.5/sleuren/plugins/system.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/temp.py` & `sleuren-1.0.5/sleuren/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/unbound.py` & `sleuren-1.0.5/sleuren/plugins/unbound.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/vms.py` & `sleuren-1.0.5/sleuren/plugins/vms.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/wp-toolkit.py` & `sleuren-1.0.5/sleuren/plugins/wp-toolkit.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/plugins/yum-updates.py` & `sleuren-1.0.5/sleuren/plugins/yum-updates.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.4/sleuren/sleuren.py` & `sleuren-1.0.5/sleuren/sleuren.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; tab-width: 4; indent-tabs: nil; -*-
 from __future__ import print_function
 import bz2
 import sys
+
 if sys.version_info >= (3,):
     try:
         from past.builtins import basestring
     except ImportError:
         basestring = str
     import configparser
     import http.client
@@ -16,14 +17,15 @@
     import ConfigParser
     import httplib
     import StringIO
     from Queue import Queue, Empty
 
 import glob
 import imp
+
 try:
     import json
 except ImportError:
     import simplejson as json
 import logging
 import os
 import pickle
@@ -40,15 +42,15 @@
     from urllib.request import urlopen, Request
     from urllib.error import HTTPError
 except ImportError:
     from urlparse import urlparse
     from urllib import urlencode
     from urllib2 import urlopen, Request, HTTPError
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 __FILEABSDIRNAME__ = os.path.dirname(os.path.abspath(__file__))
 
 ini_files = (
     os.path.join('/etc', 'sleuren.ini'),
     os.path.join('/etc', 'sleuren-token.ini'),
     os.path.join(os.path.dirname(__FILEABSDIRNAME__), 'sleuren.ini'),
     os.path.join(os.path.dirname(__FILEABSDIRNAME__), 'sleuren-token.ini'),
@@ -58,14 +60,15 @@
 
 if sys.platform == 'win32':
     ini_files = (
         os.path.join(__FILEABSDIRNAME__, 'sleuren.ini'),
         os.path.join(__FILEABSDIRNAME__, 'sleuren-token.ini'),
     )
 
+
 def info():
     '''
     Return string with info about sleuren:
         - version
         - plugins enabled
         - absolute path to plugin directory
         - server id from configuration file
@@ -76,49 +79,49 @@
     plugins_enabled = agent._get_plugins(state='enabled')
 
     return '\n'.join((
         'Version: %s' % __version__,
         'Plugins enabled: %s' % ', '.join(plugins_enabled),
         'Plugins directory: %s' % plugins_path,
         'Server: %s' % agent.config.get('agent', 'server'),
-        'User: %s' % agent.config.get('agent', 'user'),
+        'User: %s' % agent.config.get('agent', 'project'),
     ))
 
 
 def hello(proto='https'):
-    user_id = sys.argv[1]
+    project = sys.argv[1]
     agent = Agent(dry_instance=True)
     if len(sys.argv) > 2:
         token_filename = sys.argv[2]
     else:
         token_filename = os.path.join(__FILEABSDIRNAME__, 'sleuren-token.ini')
     if len(sys.argv) > 3:
         unique_id = sys.argv[3]
     else:
         unique_id = ''
-    if '_' in user_id:
-        server_id = user_id.split('_')[1]
-        user_id = user_id.split('_')[0]
+    if '_' in project:
+        server_id = project.split('_')[1]
+        project = project.split('_')[0]
     else:
         try:
             hostname = os.uname()[1]
         except AttributeError:
             hostname = socket.getfqdn()
         server_id = urlopen(
-            proto + '://' + agent.config.get('data', 'api_host') + '/api/hello',
+            proto + '://' + agent.config.get('data', 'api_host') + '/hello',
             data=urlencode({
-                    'user': user_id,
-                    'hostname': hostname,
-                    'unique_id': unique_id
+                'project': project,
+                'hostname': hostname,
+                'unique_id': unique_id
             }).encode("utf-8")
-           ).read().decode()
+        ).read().decode()
     if len(server_id) == 36:
         print('Got server_id: %s' % server_id)
-        open(token_filename, 'w').\
-            write('[DEFAULT]\nuser=%s\nserver=%s\n' % (user_id, server_id))
+        open(token_filename, 'w'). \
+            write('[DEFAULT]\nproject=%s\nserver=%s\n' % (project, server_id))
     else:
         print('Could not retrieve server_id: %s' % server_id)
 
 
 # def run_agent():
 #     Agent().run()
 
@@ -205,18 +208,18 @@
             'logging_level': logging.INFO,
             'threads': 100,
             'ttl': 60,
             'interval': 60,
             'plugins': os.path.join(__FILEABSDIRNAME__, 'plugins'),
             'enabled': 'no',
             'subprocess': 'no',
-            'user': '',
+            'project': '',
             'server': '',
-            'api_host': 'api.sleuren.com',
-            'api_path': '/api/agent',
+            'api_host': 'agent.sleuren.com',
+            'api_path': '/events',
             'log_file': '/var/log/sleuren.log',
             'log_file_mode': 'a',
             'max_cached_collections': 10,
         }
         sections = [
             'agent',
             'execution',
@@ -261,15 +264,16 @@
         else:
             log_file_mode = 'a'
 
         if log_file == '-':
             logging.basicConfig(level=level)  # Log to sys.stderr by default
         else:
             try:
-                logging.basicConfig(filename=log_file, filemode=log_file_mode, level=level, format="%(asctime)-15s  %(levelname)s    %(message)s")
+                logging.basicConfig(filename=log_file, filemode=log_file_mode, level=level,
+                                    format="%(asctime)-15s  %(levelname)s    %(message)s")
             except IOError as e:
                 logging.basicConfig(level=level)
                 logging.info('IOError: %s', e)
                 logging.info('Drop logging to stderr')
 
         logging.info('Agent logging_level %i', level)
 
@@ -308,16 +312,16 @@
                         logging.error('import_plugin:%s', name)
 
     def _subprocess_execution(self, task):
         '''
         Execute /task/ in a subprocess
         '''
         process = subprocess.Popen((sys.executable, task),
-            stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-            universal_newlines=True)
+                                   stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+                                   universal_newlines=True)
         logging.debug('%s:process:%i', threading.currentThread(), process.pid)
         interval = self.config.getint('execution', 'interval')
         name = _plugin_name(task)
         ttl = self.config.getint(name, 'ttl')
         ticks = ttl / interval or 1
         process.poll()
         while process.returncode is None and ticks > 0:
@@ -327,15 +331,15 @@
             process.poll()
         if process.returncode is None:
             logging.error('%s:kill:%i', threading.currentThread(), process.pid)
             os.kill(process.pid, signal.SIGTERM)
         stdout, stderr = process.communicate()
         if process.returncode != 0 or stderr:
             logging.error('%s:%s:%s:%s', threading.currentThread(),
-                task, process.returncode, stderr)
+                          task, process.returncode, stderr)
         if stdout:
             ret = pickle.loads(stdout)
         else:
             ret = None
         return ret
 
     def _execution(self):
@@ -380,37 +384,36 @@
                 'name': name,
                 'interval': interval,
                 'payload': payload,
             })
         self.cemetery.put(threading.currentThread())
         self.hire.release()
 
-
     def _data(self):
         '''
         Take and collect data, send and clean if needed
         '''
         logging.info('%s', threading.currentThread())
         api_host = self.config.get('data', 'api_host')
         api_path = self.config.get('data', 'api_path')
         max_age = self.config.getint('agent', 'max_data_age')
         max_span = self.config.getint('agent', 'max_data_span')
         server = self.config.get('agent', 'server')
-        user = self.config.get('agent', 'user')
+        project = self.config.get('agent', 'project')
         interval = self.config.getint('data', 'interval')
         max_cached_collections = self.config.get('agent', 'max_cached_collections')
         cached_collections = []
         collection = []
         while True:
             loop_ts = time.time()
             if self.shutdown:
                 logging.info('%s:shutdown', threading.currentThread())
                 break
             logging.debug('%s:data_queue:%i:collection:%i',
-                threading.currentThread(), self.data.qsize(), len(collection))
+                          threading.currentThread(), self.data.qsize(), len(collection))
             while self.data.qsize():
                 try:
                     collection.append(self.data.get_nowait())
                 except Exception as e:
                     logging.error('Data queue error: %s' % e)
             if collection:
                 first_ts = min((e['ts'] for e in collection))
@@ -424,49 +427,49 @@
                 elif now - first_ts >= max_age:
                     logging.warning('Max data age')
                     send = True
                     clean = True
                 if send:
                     headers = {
                         "Content-type": "application/json",
-                        "Authorization": "ApiKey %s:%s" % (user, server),
+                        "Authorization": "ApiKey %s:%s" % (project, server),
                     }
                     logging.debug('collection: %s',
-                        json.dumps(collection, indent=2, sort_keys=True))
-                    if not (server and user):
-                        logging.warning('Empty server or user, nowhere to send.')
+                                  json.dumps(collection, indent=2, sort_keys=True))
+                    if not (server and project):
+                        logging.warning('Empty server or project, nowhere to send.')
                         clean = True
                     else:
 
                         try:
                             if sys.version_info >= (3,):
                                 connection = http.client.HTTPSConnection(api_host, timeout=15)
                             else:
                                 connection = httplib.HTTPSConnection(api_host, timeout=15)
 
                             # Trying to send cached collections if any
                             if cached_collections:
                                 logging.info('Sending cached collections: %i', len(cached_collections))
                                 while cached_collections:
                                     connection.request('PUT', '%s?version=%s' % (api_path, __version__),
-                                            cached_collections[0],
-                                            headers=headers)
+                                                       cached_collections[0],
+                                                       headers=headers)
                                     response = connection.getresponse()
                                     response.read()
                                     if response.status == 200:
                                         del cached_collections[0]  # Remove just sent collection
                                         logging.debug('Successful response: %s', response.status)
                                     else:
                                         raise ValueError('Unsuccessful response: %s' % response.status)
                                 logging.info('All cached collections sent')
 
                             # Send recent collection (reuse existing connection)
                             connection.request('PUT', '%s?version=%s' % (api_path, __version__),
-                                   bz2.compress(str(json.dumps(collection) + "\n").encode()),
-                                    headers=headers)
+                                               bz2.compress(str(json.dumps(collection) + "\n").encode()),
+                                               headers=headers)
                             response = connection.getresponse()
                             response.read()
 
                             if response.status == 200:
                                 logging.debug('Successful response: %s', response.status)
                                 clean = True
                             else:
@@ -475,17 +478,17 @@
                             logging.error('Failed to submit collection: %s' % e)
 
                             # Store recent collection in cached_collections if send failed
                             if max_cached_collections > 0:
                                 if len(cached_collections) >= max_cached_collections:
                                     del cached_collections[0]  # Remove oldest collection
                                     logging.info('Reach max_cached_collections (%s): oldest cached collection dropped',
-                                        max_cached_collections)
+                                                 max_cached_collections)
                                 logging.info('Cache current collection to resend next time')
-                                cached_collections.append(bz2.compress(str(json.dumps(collection)+"\n").encode()))
+                                cached_collections.append(bz2.compress(str(json.dumps(collection) + "\n").encode()))
                                 collection = []
                         finally:
                             connection.close()
                     if clean:
                         collection = []
             sleep_interval = interval - (time.time() - loop_ts)
             if sleep_interval > 0:
@@ -527,30 +530,28 @@
                     plugins.append(plugin_name)
             elif state == 'disabled':
                 if not self.config.getboolean(plugin_name, 'enabled'):
                     plugins.append(plugin_name)
 
         return plugins
 
-
     def _rip(self):
         '''
         Join with dead workers
         Workaround for https://bugs.python.org/issue37788
         '''
         logging.debug('cemetery:%i', self.cemetery.qsize())
         while True:
             try:
                 thread = self.cemetery.get_nowait()
             except Empty:
                 break
             logging.debug('joining:%s', thread)
             thread.join()
 
-
     def run(self):
         '''
         Start all the worker threads
         '''
         logging.info('Agent main loop')
         interval = self.config.getfloat('agent', 'interval')
         self.hire = threading.Semaphore(
@@ -592,15 +593,15 @@
                         self.metrics.put({
                             'ts': now,
                             'name': 'agent_internal',
                             'payload': {
                                 'threads_capping':
                                     self.config.getint('execution', 'threads')}
                         })
-                sleep_interval = .5-(time.time()-now)
+                sleep_interval = .5 - (time.time() - now)
                 if sleep_interval > 0:
                     time.sleep(sleep_interval)
                 else:
                     logging.warning('not enough time to start worker threads')
                     time.sleep(.1)
 
         except KeyboardInterrupt:
@@ -610,27 +611,28 @@
             wait_for = True
             while wait_for:
                 all_threads = threading.enumerate()
                 logging.info('Remaining threads: %s', all_threads)
                 wait_for = [
                     thread for thread in all_threads
                     if not thread.isDaemon() and
-                    not isinstance(thread, threading._MainThread)
+                       not isinstance(thread, threading._MainThread)
                 ]
                 if not wait_for:
                     logging.info('Bye!')
                     sys.exit(0)
                 self.shutdown = True
                 logging.info('Waiting for %i threads to exit', len(wait_for))
                 for thread in wait_for:
                     logging.info('Joining with %s/%f', thread, interval)
                     thread.join(interval)
         except Exception as e:
             logging.error('Worker error: %s' % e)
 
+
 def main():
     if len(sys.argv) > 1:
         if sys.argv[1].startswith('--'):
             sys.argv[1] = sys.argv[1][2:]
 
         if sys.argv[1] == 'help':
             print('\n'.join((
@@ -658,8 +660,8 @@
             print('Invalid option:', sys.argv[1], file=sys.stderr)
             sys.exit(1)
     else:
         Agent().run()
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `sleuren-1.0.4/sleuren.egg-info/PKG-INFO` & `sleuren-1.0.5/sleuren.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleuren
-Version: 1.0.4
+Version: 1.0.5
 Summary: Server monitoring agent
 Home-page: https://github.com/sleuren/agent
 Author: sleuren
 Author-email: hello@sleuren.com
 Maintainer: sleuren
 Maintainer-email: hello@sleuren.com
 License: MIT
```

### Comparing `sleuren-1.0.4/sleuren.egg-info/SOURCES.txt` & `sleuren-1.0.5/sleuren.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 sleuren/plugins/haproxy.py
 sleuren/plugins/httpd.py
 sleuren/plugins/iostat.py
 sleuren/plugins/janus.py
 sleuren/plugins/kamailio.py
 sleuren/plugins/litespeed.py
 sleuren/plugins/loadavg.py
+sleuren/plugins/loggedin.py
 sleuren/plugins/mailq.py
 sleuren/plugins/mdstat.py
 sleuren/plugins/megacli.py
 sleuren/plugins/memcached.py
 sleuren/plugins/memory.py
 sleuren/plugins/minecraft.py
 sleuren/plugins/mongodb.py
```

