# Comparing `tmp/jc-1.9.2.tar.gz` & `tmp/jc-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jc-1.9.2.tar", last modified: Fri Mar 13 00:10:26 2020, max compression
+gzip compressed data, was "dist/jc-1.9.3.tar", last modified: Fri Mar 27 00:17:02 2020, max compression
```

## Comparing `jc-1.9.2.tar` & `jc-1.9.3.tar`

### file list

```diff
@@ -1,604 +1,610 @@
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:26.000000 jc-1.9.2/
--rw-r--r--   0 kbrazil    (501) staff       (20)       21 2020-02-08 20:39:18.000000 jc-1.9.2/MANIFEST.in
--rw-r--r--   0 kbrazil    (501) staff       (20)    68515 2020-03-13 00:10:26.000000 jc-1.9.2/PKG-INFO
--rwxr-xr-x   0 kbrazil    (501) staff       (20)    49028 2020-03-12 15:24:33.000000 jc-1.9.2/README.md
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:25.000000 jc-1.9.2/jc/
--rw-r--r--   0 kbrazil    (501) staff       (20)     2538 2019-11-17 20:00:19.000000 jc-1.9.2/jc/__init__.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     8326 2020-03-13 00:09:29.000000 jc-1.9.2/jc/cli.py
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:25.000000 jc-1.9.2/jc/parsers/
--rw-r--r--   0 kbrazil    (501) staff       (20)        0 2019-11-07 14:51:38.000000 jc-1.9.2/jc/parsers/__init__.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3598 2020-03-11 20:47:39.000000 jc-1.9.2/jc/parsers/airport.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4366 2020-03-11 20:47:39.000000 jc-1.9.2/jc/parsers/airport_s.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     5000 2020-03-13 00:09:29.000000 jc-1.9.2/jc/parsers/arp.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     6868 2020-03-08 21:54:48.000000 jc-1.9.2/jc/parsers/blkid.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     6756 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/crontab.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     7055 2020-02-08 20:42:01.000000 jc-1.9.2/jc/parsers/crontab_u.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3193 2020-03-03 19:47:13.000000 jc-1.9.2/jc/parsers/csv.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     5176 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/df.py
--rw-r--r--   0 kbrazil    (501) staff       (20)    15625 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/dig.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3751 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/du.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2782 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/env.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2933 2020-03-12 15:51:46.000000 jc-1.9.2/jc/parsers/file.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1802 2020-03-08 21:54:48.000000 jc-1.9.2/jc/parsers/foo.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3037 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/free.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4098 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/fstab.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3976 2020-03-03 19:47:13.000000 jc-1.9.2/jc/parsers/group.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3230 2020-03-03 19:47:13.000000 jc-1.9.2/jc/parsers/gshadow.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2807 2020-03-11 20:47:39.000000 jc-1.9.2/jc/parsers/history.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3258 2020-02-06 01:00:38.000000 jc-1.9.2/jc/parsers/hosts.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     5595 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/id.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     7611 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/ifconfig.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2418 2020-02-06 01:00:38.000000 jc-1.9.2/jc/parsers/ini.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     7465 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/iptables.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4885 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/jobs.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4425 2020-03-03 19:47:13.000000 jc-1.9.2/jc/parsers/last.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     8829 2020-03-08 21:54:48.000000 jc-1.9.2/jc/parsers/ls.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     9105 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/lsblk.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3844 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/lsmod.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     5434 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/lsof.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3729 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/mount.py
--rw-r--r--   0 kbrazil    (501) staff       (20)    16129 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/netstat.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     6787 2020-03-11 20:47:39.000000 jc-1.9.2/jc/parsers/ntpq.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4055 2020-03-03 19:47:13.000000 jc-1.9.2/jc/parsers/passwd.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2658 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/pip_list.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3444 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/pip_show.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     6793 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/ps.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4085 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/route.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4306 2020-03-03 19:47:13.000000 jc-1.9.2/jc/parsers/shadow.py
--rw-r--r--   0 kbrazil    (501) staff       (20)    11491 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/ss.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     8255 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/stat.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2940 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/systemctl.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3483 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/systemctl_lj.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2675 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/systemctl_ls.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2585 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/systemctl_luf.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3432 2020-03-11 20:47:39.000000 jc-1.9.2/jc/parsers/timedatectl.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3225 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/uname.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4041 2019-12-17 20:12:32.000000 jc-1.9.2/jc/parsers/universal.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3243 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/uptime.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4345 2020-02-14 02:27:17.000000 jc-1.9.2/jc/parsers/w.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     7850 2020-03-03 19:47:13.000000 jc-1.9.2/jc/parsers/who.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2747 2020-02-06 01:00:38.000000 jc-1.9.2/jc/parsers/xml.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3045 2020-02-06 01:00:38.000000 jc-1.9.2/jc/parsers/yaml.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1471 2019-12-17 20:12:32.000000 jc-1.9.2/jc/utils.py
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:25.000000 jc-1.9.2/jc.egg-info/
--rw-r--r--   0 kbrazil    (501) staff       (20)    68515 2020-03-13 00:10:25.000000 jc-1.9.2/jc.egg-info/PKG-INFO
--rw-r--r--   0 kbrazil    (501) staff       (20)    21252 2020-03-13 00:10:25.000000 jc-1.9.2/jc.egg-info/SOURCES.txt
--rw-r--r--   0 kbrazil    (501) staff       (20)        1 2020-03-13 00:10:25.000000 jc-1.9.2/jc.egg-info/dependency_links.txt
--rw-r--r--   0 kbrazil    (501) staff       (20)       36 2020-03-13 00:10:25.000000 jc-1.9.2/jc.egg-info/entry_points.txt
--rw-r--r--   0 kbrazil    (501) staff       (20)       61 2020-03-13 00:10:25.000000 jc-1.9.2/jc.egg-info/requires.txt
--rw-r--r--   0 kbrazil    (501) staff       (20)        9 2020-03-13 00:10:25.000000 jc-1.9.2/jc.egg-info/top_level.txt
--rw-r--r--   0 kbrazil    (501) staff       (20)       38 2020-03-13 00:10:26.000000 jc-1.9.2/setup.cfg
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     1007 2020-03-13 00:09:29.000000 jc-1.9.2/setup.py
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:25.000000 jc-1.9.2/tests/
--rw-r--r--   0 kbrazil    (501) staff       (20)        0 2019-10-31 15:07:28.000000 jc-1.9.2/tests/__init__.py
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:25.000000 jc-1.9.2/tests/fixtures/
--rw-r--r--   0 kbrazil    (501) staff       (20)     8196 2019-12-12 21:25:13.000000 jc-1.9.2/tests/fixtures/.DS_Store
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:25.000000 jc-1.9.2/tests/fixtures/centos-7.7/
--rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2019-12-12 00:35:58.000000 jc-1.9.2/tests/fixtures/centos-7.7/.DS_Store
--rw-r--r--   0 kbrazil    (501) staff       (20)      350 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/arp-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      173 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/arp-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      236 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/arp-v.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      274 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/arp-v.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      236 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/arp.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      243 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/arp.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      764 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-multi.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      618 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-multi.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      987 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-udev-multi.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      838 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-udev-multi.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      488 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-udev.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      413 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-udev.out
--rw-r--r--   0 kbrazil    (501) staff       (20)       99 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid-sda2.json
--rw-r--r--   0 kbrazil    (501) staff       (20)       77 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid-sda2.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      392 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      307 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/blkid.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      399 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/centos-7.7/crontab-u.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      163 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/centos-7.7/crontab-u.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1940 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/centos-7.7/crontab.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1564 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/crontab.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      836 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/df-h.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      444 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/df-h.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      904 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/df.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      524 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/df.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      462 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/dig-aaaa.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      556 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/dig-aaaa.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      464 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/dig-x.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      547 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/dig-x.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1005 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/dig.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1052 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/dig.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   365319 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/du.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   250940 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/du.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2932 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/env.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2331 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/env.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1490 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/centos-7.7/file.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1264 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/centos-7.7/file.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      177 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/free-h.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      204 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/free-h.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      194 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/free.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      204 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/free.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      423 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/fstab.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      488 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/fstab.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2701 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/group.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      509 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/group.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3106 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/gshadow.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      407 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/gshadow.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    47552 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/centos-7.7/history.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    25967 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/history.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      223 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/hosts.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      193 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/hosts.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      267 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/centos-7.7/id.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      129 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/centos-7.7/id.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1598 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/ifconfig.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1259 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/ifconfig.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     7469 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter-line-numbers.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     6643 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter-line-numbers.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    10625 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter-nv.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     9064 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter-nv.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     7749 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     6762 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1938 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-mangle.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2399 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-mangle.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3211 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-nat.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     3484 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-nat.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1386 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-raw.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1616 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/iptables-raw.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      306 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/jobs.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      164 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/jobs.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     9189 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/last-w.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     5452 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/last-w.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     8934 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/last.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     5197 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/last.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      511 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/lastb.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      346 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/lastb.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1281 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-R-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      542 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-R-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   315329 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-R.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    72565 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-R.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2776 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-al.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1070 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-al.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   773278 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-alR.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   281708 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-alR.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2776 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-alh.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1071 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-alh.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    97675 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-glob.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    22048 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-glob.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1183 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-l-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      583 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-l-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2576 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-lR-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1209 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-lR-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      498 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      260 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      409 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls.json
--rw-r--r--   0 kbrazil    (501) staff       (20)       85 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/ls.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4102 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsblk-allcols.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2502 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsblk-allcols.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      698 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsblk.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      332 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsblk.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     6655 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsmod.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     4161 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsmod.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   618317 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsof-sudo.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   363073 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsof-sudo.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   126050 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsof.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    70567 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/lsof.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4848 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/mount.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2711 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/mount.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     7020 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat-l.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     3499 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat-l.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    17621 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat-p.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    10407 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat-p.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    29188 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat-sudo-aeep.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    14986 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat-sudo-aeep.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     8734 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat-sudo-lnp.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     4402 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat-sudo-lnp.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    15637 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     8068 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/netstat.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      713 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/centos-7.7/ntpq-p.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      474 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/centos-7.7/ntpq-p.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      700 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/centos-7.7/ntpq-pn.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      474 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/centos-7.7/ntpq-pn.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2747 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/passwd.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      961 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/passwd.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      905 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/pip-list.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      616 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/pip-list.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1129 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/pip-show.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      974 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/centos-7.7/pip-show.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    20936 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/ps-axu.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     9932 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/ps-axu.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    14630 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/ps-ef.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     8168 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/ps-ef.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      442 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/route-vn.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      338 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/route-vn.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      437 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/route.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      338 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/route.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3206 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/shadow.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      740 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/shadow.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    29301 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/ss-sudo-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    17945 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/ss-sudo-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   322074 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/stat.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   295777 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/stat.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1439 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/systemctl-ls.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1159 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/systemctl-ls.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    14574 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/systemctl-luf.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    13499 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/systemctl-luf.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    31968 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/systemctl.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    38560 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/systemctl.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      276 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/centos-7.7/timedatectl.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      554 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/centos-7.7/timedatectl.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      276 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/uname-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      122 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/uname-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      103 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/uptime.json
--rw-r--r--   0 kbrazil    (501) staff       (20)       62 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/uptime.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      287 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/centos-7.7/w.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      266 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/centos-7.7/w.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      549 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/who-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      364 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/who-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      155 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/who.json
--rw-r--r--   0 kbrazil    (501) staff       (20)       93 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/centos-7.7/who.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3397 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/create_fixtures.sh
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:25.000000 jc-1.9.2/tests/fixtures/generic/
--rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2020-03-02 22:16:03.000000 jc-1.9.2/tests/fixtures/generic/.DS_Store
--rw-r--r--   0 kbrazil    (501) staff       (20)      849 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-biostats.csv
--rw-r--r--   0 kbrazil    (501) staff       (20)     1566 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-biostats.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     8402 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-cities.csv
--rw-r--r--   0 kbrazil    (501) staff       (20)    18398 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-cities.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2391 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-deniro.csv
--rw-r--r--   0 kbrazil    (501) staff       (20)     5146 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-deniro.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1117 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-example.csv
--rw-r--r--   0 kbrazil    (501) staff       (20)     1588 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-example.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   558246 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-flyrna.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   205281 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-flyrna.tsv
--rw-r--r--   0 kbrazil    (501) staff       (20)   556670 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-flyrna2.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   203705 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-flyrna2.tsv
--rw-r--r--   0 kbrazil    (501) staff       (20)      158 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-homes-pipe.csv
--rw-r--r--   0 kbrazil    (501) staff       (20)      274 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-homes-pipe.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2125 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-homes.csv
--rw-r--r--   0 kbrazil    (501) staff       (20)     6798 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-homes.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    53816 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-insurance.csv
--rw-r--r--   0 kbrazil    (501) staff       (20)   229722 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/generic/csv-insurance.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     4705 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/ini-iptelserver.ini
--rw-r--r--   0 kbrazil    (501) staff       (20)     1486 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/ini-iptelserver.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      171 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/ini-test.ini
--rw-r--r--   0 kbrazil    (501) staff       (20)      270 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/ini-test.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     3294 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/xml-cd_catalog.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     5077 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/xml-cd_catalog.xml
--rw-r--r--   0 kbrazil    (501) staff       (20)      811 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/xml-foodmenu.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1102 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/xml-foodmenu.xml
--rw-r--r--   0 kbrazil    (501) staff       (20)      333 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/yaml-istio-sc.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      305 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/yaml-istio-sc.yaml
--rw-r--r--   0 kbrazil    (501) staff       (20)     3178 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/yaml-istio-sidecar.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     3681 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/generic/yaml-istio-sidecar.yaml
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:25.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/
--rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2019-12-06 21:09:19.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/.DS_Store
--rw-r--r--   0 kbrazil    (501) staff       (20)     1669 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/arp-a.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     1036 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/arp-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1151 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/df-h.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      908 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/df-h.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1196 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/df.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      992 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/df.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      439 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/dig-aaaa.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      537 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/dig-aaaa.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      442 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/dig-x.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      529 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/dig-x.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1272 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/dig.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     1188 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/dig.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   221050 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/du.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)   166687 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/du.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3791 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ifconfig.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     1571 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ifconfig.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3791 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ifconfig2.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     1571 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ifconfig2.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4259 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ls-al.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     1851 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ls-al.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4296 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ls-alh.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     1882 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ls-alh.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      533 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ls.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      175 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ls.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      224 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/pip-list.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      168 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/pip-list.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1028 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/pip-show.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      867 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/pip-show.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    53632 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ps-axu.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)    32255 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ps-axu.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    38291 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ps-ef.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)    25921 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/ps-ef.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      233 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/uname-a.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      142 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/uname-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      102 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/uptime.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)       57 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/uptime.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      627 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/w.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      458 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.11.6/w.out
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:26.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/
--rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2019-12-16 21:35:29.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/.DS_Store
--rw-r--r--   0 kbrazil    (501) staff       (20)      307 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/airport-I.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      348 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/airport-I.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2152 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/airport-s.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1423 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/airport-s.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1541 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/arp-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      968 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/arp-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2582 2020-03-13 00:09:29.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/arp-a2.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1597 2020-03-13 00:09:29.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/arp-a2.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1686 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/df-h.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1276 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/df-h.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1764 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/df.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1384 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/df.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      438 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/dig-aaaa.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      536 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/dig-aaaa.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      442 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/dig-x.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      529 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/dig-x.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1266 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/dig.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1182 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/dig.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   296296 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/du.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   222287 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/du.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3589 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/file.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2890 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/file.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4715 2020-03-12 15:24:33.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/file2.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     4780 2020-03-12 15:24:33.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/file2.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     9646 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/group.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2823 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/group.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      759 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/id.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      386 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/id.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    10823 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ifconfig.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     3779 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ifconfig.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    11375 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ifconfig2.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     3979 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ifconfig2.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    45274 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/last.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    25827 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/last.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      852 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-R-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      278 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-R-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   469418 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-R.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   133787 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-R.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4653 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-al.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     2111 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-al.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   959674 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-alR.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   364578 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-alR.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4684 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-alh.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)     2111 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-alh.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    91499 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-glob.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    19369 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-glob.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1162 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-l-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      583 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-l-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   355547 2020-03-08 21:54:48.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-lR-empty-folder.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   128740 2020-03-08 21:54:48.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-lR-empty-folder.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1450 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-lR-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      656 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-lR-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      498 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      260 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      585 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      193 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ls.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      672 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/mount.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      349 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/mount.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      841 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/mount2.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      464 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/mount2.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    14855 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/passwd.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     6804 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/passwd.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      224 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/pip-list.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      168 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/pip-list.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1067 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/pip-show.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      910 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/pip-show.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    99173 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ps-axu.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    60107 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ps-axu.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    71162 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ps-ef.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    48758 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/ps-ef.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      221 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/uname-a.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      131 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/uname-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      110 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/uptime.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)       65 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/uptime.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      836 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/w.json
--rwxr-xr-x   0 kbrazil    (501) staff       (20)      570 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/w.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      659 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/who-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      419 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/who-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      251 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/who.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      128 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/osx-10.14.6/who.out
-drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-13 00:10:26.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/
--rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2020-02-18 21:08:44.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/.DS_Store
--rw-r--r--   0 kbrazil    (501) staff       (20)      351 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/arp-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      174 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/arp-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      237 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/arp-v.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      274 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/arp-v.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      237 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/arp.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      243 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/arp.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      818 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-multi.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      717 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-multi.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      962 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-udev-multi.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      832 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-udev-multi.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      547 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-udev.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      478 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-udev.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      142 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-sda2.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      115 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-sda2.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      986 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      675 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      939 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/crontab-u.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      752 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/crontab-u.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2261 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/df-h.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1004 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/df-h.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2372 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/df.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1194 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/df.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      458 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/dig-aaaa.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      532 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/dig-aaaa.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      460 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/dig-x.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      523 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/dig-x.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1306 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/dig.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1156 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/dig.out
--rw-r--r--   0 kbrazil    (501) staff       (20)  1560353 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/du.json
--rw-r--r--   0 kbrazil    (501) staff       (20)  1136984 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/du.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2651 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/env.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2125 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/env.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1093 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/file.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      729 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/file.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      177 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/free-h.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      204 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/free-h.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      195 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/free.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      204 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/free.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      268 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/fstab.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      120 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/fstab.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3705 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/group.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      721 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/group.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4279 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/gshadow.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      606 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/gshadow.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    22782 2020-02-06 01:00:38.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/history.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    12844 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/history.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      365 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/hosts.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      272 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/hosts.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1090 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ifconfig.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      894 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ifconfig.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      847 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter-line-numbers.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1025 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter-line-numbers.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2363 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter-nv.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2763 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter-nv.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1730 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2035 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      141 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-mangle.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      468 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-mangle.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      106 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-nat.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      375 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-nat.out
--rw-r--r--   0 kbrazil    (501) staff       (20)       39 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-raw.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      187 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-raw.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      306 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/jobs.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      164 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/jobs.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1852 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/last-w.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1073 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/last-w.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1845 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/last.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1066 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/last.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      125 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lastb.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      111 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lastb.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1114 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-R-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      471 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-R-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   298654 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-R.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    62421 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-R.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3950 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-al.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1744 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-al.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   772252 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-alR.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   262651 2020-02-19 15:07:23.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-alR.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3942 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-alh.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1567 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-alh.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    66907 2020-02-19 15:07:24.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-glob.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    13721 2020-02-19 15:07:24.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-glob.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1176 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-l-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      576 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-l-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2089 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-lR-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      984 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-lR-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      498 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-newlines.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      260 2020-02-27 19:25:11.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-newlines.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      622 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      162 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ls.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    11397 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsblk-allcols.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     7364 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsblk-allcols.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2114 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsblk.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      812 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsblk.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     6744 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsmod.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     4251 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsmod.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   526695 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsof-sudo.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   342863 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsof-sudo.out
--rw-r--r--   0 kbrazil    (501) staff       (20)   194044 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsof.json
--rw-r--r--   0 kbrazil    (501) staff       (20)   132043 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/lsof.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     6547 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/mount.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     3708 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/mount.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     5079 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-l.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2606 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-l.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    14711 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-p.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     8706 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-p.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    22957 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-sudo-aeep.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    12016 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-sudo-aeep.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     6259 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-sudo-lnp.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     3236 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-sudo-lnp.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    12550 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     6711 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3333 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-p.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1659 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-p.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3832 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-p2.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1896 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-p2.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     3314 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-pn.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1659 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-pn.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     1659 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ntqp-p.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4116 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/passwd.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1565 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/passwd.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2638 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-list-legacy.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     1041 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-list-legacy.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2638 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-list.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2360 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-list.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      874 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-show.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      730 2019-12-17 20:12:32.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-show.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    31390 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ps-axu.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    14127 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ps-axu.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    21583 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ps-ef.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    11355 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ps-ef.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      447 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/route-vn.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      336 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/route-vn.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      439 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/route.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      336 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/route.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     4330 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/shadow.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      939 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/shadow.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    23277 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ss-sudo-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    25599 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/ss-sudo-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    73147 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/stat.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    60023 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/stat.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      270 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-lj.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      244 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-lj.out
--rw-r--r--   0 kbrazil    (501) staff       (20)     2431 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-ls.json
--rw-r--r--   0 kbrazil    (501) staff       (20)     2072 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-ls.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    18756 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-luf.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    17734 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-luf.out
--rw-r--r--   0 kbrazil    (501) staff       (20)    47895 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl.json
--rw-r--r--   0 kbrazil    (501) staff       (20)    76059 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      274 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/timedatectl.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      350 2020-03-11 20:47:39.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/timedatectl.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      268 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/uname-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      114 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/uname-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      109 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/uptime.json
--rw-r--r--   0 kbrazil    (501) staff       (20)       70 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/uptime.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      292 2019-11-17 20:00:19.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/w.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      274 2019-10-31 15:07:28.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/w.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      452 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/who-a.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      355 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/who-a.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      155 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/who.json
--rw-r--r--   0 kbrazil    (501) staff       (20)      140 2020-03-03 19:47:13.000000 jc-1.9.2/tests/fixtures/ubuntu-18.04/who.out
--rw-r--r--   0 kbrazil    (501) staff       (20)      862 2020-03-11 20:47:39.000000 jc-1.9.2/tests/test_airport.py
--rw-r--r--   0 kbrazil    (501) staff       (20)      866 2020-03-11 20:47:39.000000 jc-1.9.2/tests/test_airport_s.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     5350 2020-03-13 00:09:29.000000 jc-1.9.2/tests/test_arp.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     6590 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_blkid.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1134 2020-03-11 20:47:39.000000 jc-1.9.2/tests/test_cli.py
--rw-r--r--   0 kbrazil    (501) staff       (20)      837 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_crontab.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1498 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_crontab_u.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     5383 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_csv.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4669 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_df.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3656 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_dig.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2415 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_du.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1350 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_env.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2547 2020-03-12 15:24:33.000000 jc-1.9.2/tests/test_file.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2517 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_free.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1406 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_fstab.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1982 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_group.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1444 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_gshadow.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1426 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_history.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1406 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_hosts.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1329 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_id.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3845 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_ifconfig.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1404 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_ini.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     8341 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_iptables.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1369 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_jobs.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4237 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_last.py
--rw-r--r--   0 kbrazil    (501) staff       (20)    20734 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_ls.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3084 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_lsblk.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1388 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_lsmod.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2563 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_lsof.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2536 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_mount.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     6474 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_netstat.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3178 2020-03-11 20:47:39.000000 jc-1.9.2/tests/test_ntpq.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2012 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_passwd.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3303 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_pip_list.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2637 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_pip_show.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     4805 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_ps.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2570 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_route.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1425 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_shadow.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1445 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_ss.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1383 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_stat.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1470 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_systemctl.py
--rw-r--r--   0 kbrazil    (501) staff       (20)      907 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_systemctl_lj.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1547 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_systemctl_ls.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1564 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_systemctl_luf.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1502 2020-03-11 20:47:39.000000 jc-1.9.2/tests/test_timedatectl.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2586 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_uname.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2563 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_uptime.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     2370 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_w.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     3599 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_who.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1429 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_xml.py
--rw-r--r--   0 kbrazil    (501) staff       (20)     1473 2020-03-08 21:54:48.000000 jc-1.9.2/tests/test_yaml.py
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:02.000000 jc-1.9.3/
+-rw-r--r--   0 kbrazil    (501) staff       (20)       21 2020-02-08 20:39:18.000000 jc-1.9.3/MANIFEST.in
+-rw-r--r--   0 kbrazil    (501) staff       (20)    68515 2020-03-27 00:17:02.000000 jc-1.9.3/PKG-INFO
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)    49028 2020-03-12 15:24:33.000000 jc-1.9.3/README.md
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:01.000000 jc-1.9.3/jc/
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2538 2019-11-17 20:00:19.000000 jc-1.9.3/jc/__init__.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8326 2020-03-27 00:16:11.000000 jc-1.9.3/jc/cli.py
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:01.000000 jc-1.9.3/jc/parsers/
+-rw-r--r--   0 kbrazil    (501) staff       (20)        0 2019-11-07 14:51:38.000000 jc-1.9.3/jc/parsers/__init__.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3598 2020-03-11 20:47:39.000000 jc-1.9.3/jc/parsers/airport.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4366 2020-03-11 20:47:39.000000 jc-1.9.3/jc/parsers/airport_s.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5000 2020-03-13 00:09:29.000000 jc-1.9.3/jc/parsers/arp.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6868 2020-03-08 21:54:48.000000 jc-1.9.3/jc/parsers/blkid.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6756 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/crontab.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     7055 2020-02-08 20:42:01.000000 jc-1.9.3/jc/parsers/crontab_u.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3193 2020-03-03 19:47:13.000000 jc-1.9.3/jc/parsers/csv.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5176 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/df.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)    17105 2020-03-27 00:16:11.000000 jc-1.9.3/jc/parsers/dig.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3751 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/du.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2782 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/env.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2933 2020-03-12 15:51:46.000000 jc-1.9.3/jc/parsers/file.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1802 2020-03-08 21:54:48.000000 jc-1.9.3/jc/parsers/foo.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3037 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/free.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4098 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/fstab.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3976 2020-03-03 19:47:13.000000 jc-1.9.3/jc/parsers/group.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3230 2020-03-03 19:47:13.000000 jc-1.9.3/jc/parsers/gshadow.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2807 2020-03-11 20:47:39.000000 jc-1.9.3/jc/parsers/history.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3258 2020-02-06 01:00:38.000000 jc-1.9.3/jc/parsers/hosts.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5595 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/id.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     7611 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/ifconfig.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2418 2020-02-06 01:00:38.000000 jc-1.9.3/jc/parsers/ini.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     7465 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/iptables.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4885 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/jobs.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4425 2020-03-03 19:47:13.000000 jc-1.9.3/jc/parsers/last.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8829 2020-03-08 21:54:48.000000 jc-1.9.3/jc/parsers/ls.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     9105 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/lsblk.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3844 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/lsmod.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5434 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/lsof.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3729 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/mount.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)    16129 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/netstat.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6787 2020-03-11 20:47:39.000000 jc-1.9.3/jc/parsers/ntpq.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4055 2020-03-03 19:47:13.000000 jc-1.9.3/jc/parsers/passwd.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2658 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/pip_list.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3444 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/pip_show.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6793 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/ps.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4085 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/route.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4306 2020-03-03 19:47:13.000000 jc-1.9.3/jc/parsers/shadow.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)    11491 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/ss.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8255 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/stat.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2940 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/systemctl.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3483 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/systemctl_lj.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2675 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/systemctl_ls.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2585 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/systemctl_luf.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3432 2020-03-11 20:47:39.000000 jc-1.9.3/jc/parsers/timedatectl.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3225 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/uname.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4041 2019-12-17 20:12:32.000000 jc-1.9.3/jc/parsers/universal.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3243 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/uptime.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4345 2020-02-14 02:27:17.000000 jc-1.9.3/jc/parsers/w.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     7850 2020-03-03 19:47:13.000000 jc-1.9.3/jc/parsers/who.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2747 2020-02-06 01:00:38.000000 jc-1.9.3/jc/parsers/xml.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3045 2020-02-06 01:00:38.000000 jc-1.9.3/jc/parsers/yaml.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1471 2019-12-17 20:12:32.000000 jc-1.9.3/jc/utils.py
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:01.000000 jc-1.9.3/jc.egg-info/
+-rw-r--r--   0 kbrazil    (501) staff       (20)    68515 2020-03-27 00:17:01.000000 jc-1.9.3/jc.egg-info/PKG-INFO
+-rw-r--r--   0 kbrazil    (501) staff       (20)    21495 2020-03-27 00:17:01.000000 jc-1.9.3/jc.egg-info/SOURCES.txt
+-rw-r--r--   0 kbrazil    (501) staff       (20)        1 2020-03-27 00:17:01.000000 jc-1.9.3/jc.egg-info/dependency_links.txt
+-rw-r--r--   0 kbrazil    (501) staff       (20)       36 2020-03-27 00:17:01.000000 jc-1.9.3/jc.egg-info/entry_points.txt
+-rw-r--r--   0 kbrazil    (501) staff       (20)       61 2020-03-27 00:17:01.000000 jc-1.9.3/jc.egg-info/requires.txt
+-rw-r--r--   0 kbrazil    (501) staff       (20)        9 2020-03-27 00:17:01.000000 jc-1.9.3/jc.egg-info/top_level.txt
+-rw-r--r--   0 kbrazil    (501) staff       (20)       38 2020-03-27 00:17:02.000000 jc-1.9.3/setup.cfg
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     1007 2020-03-27 00:16:11.000000 jc-1.9.3/setup.py
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:01.000000 jc-1.9.3/tests/
+-rw-r--r--   0 kbrazil    (501) staff       (20)        0 2019-10-31 15:07:28.000000 jc-1.9.3/tests/__init__.py
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:01.000000 jc-1.9.3/tests/fixtures/
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8196 2019-12-12 21:25:13.000000 jc-1.9.3/tests/fixtures/.DS_Store
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:02.000000 jc-1.9.3/tests/fixtures/centos-7.7/
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2019-12-12 00:35:58.000000 jc-1.9.3/tests/fixtures/centos-7.7/.DS_Store
+-rw-r--r--   0 kbrazil    (501) staff       (20)      350 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/arp-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      173 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/arp-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      236 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/arp-v.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      274 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/arp-v.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      236 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/arp.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      243 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/arp.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      764 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-multi.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      618 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-multi.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      987 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-udev-multi.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      838 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-udev-multi.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      488 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-udev.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      413 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-udev.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)       99 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid-sda2.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)       77 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid-sda2.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      392 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      307 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/blkid.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      399 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/centos-7.7/crontab-u.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      163 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/centos-7.7/crontab-u.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1940 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/centos-7.7/crontab.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1564 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/crontab.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      836 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/df-h.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      444 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/df-h.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      904 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/df.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      524 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/df.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      462 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/dig-aaaa.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      556 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/dig-aaaa.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5984 2020-03-27 00:16:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/dig-axfr.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3548 2020-03-27 00:16:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/dig-axfr.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      464 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/dig-x.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      547 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/dig-x.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1005 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/dig.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1052 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/dig.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   365319 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/du.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   250940 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/du.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2932 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/env.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2331 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/env.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1490 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/centos-7.7/file.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1264 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/centos-7.7/file.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      177 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/free-h.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      204 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/free-h.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      194 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/free.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      204 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/free.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      423 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/fstab.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      488 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/fstab.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2701 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/group.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      509 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/group.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3106 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/gshadow.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      407 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/gshadow.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    47552 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/centos-7.7/history.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    25967 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/history.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      223 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/hosts.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      193 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/hosts.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      267 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/centos-7.7/id.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      129 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/centos-7.7/id.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1598 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/ifconfig.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1259 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/ifconfig.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     7469 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter-line-numbers.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6643 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter-line-numbers.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    10625 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter-nv.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     9064 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter-nv.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     7749 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6762 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1938 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-mangle.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2399 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-mangle.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3211 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-nat.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3484 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-nat.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1386 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-raw.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1616 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/iptables-raw.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      306 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/jobs.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      164 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/jobs.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     9189 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/last-w.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5452 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/last-w.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8934 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/last.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5197 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/last.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      511 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/lastb.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      346 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/lastb.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1281 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-R-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      542 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-R-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   315329 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-R.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    72565 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-R.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2776 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-al.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1070 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-al.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   773278 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-alR.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   281708 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-alR.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2776 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-alh.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1071 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-alh.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    97675 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-glob.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    22048 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-glob.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1183 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-l-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      583 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-l-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2576 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-lR-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1209 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-lR-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      498 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      260 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      409 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)       85 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/ls.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4102 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsblk-allcols.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2502 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsblk-allcols.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      698 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsblk.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      332 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsblk.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6655 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsmod.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4161 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsmod.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   618317 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsof-sudo.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   363073 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsof-sudo.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   126050 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsof.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    70567 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/lsof.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4848 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/mount.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2711 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/mount.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     7020 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat-l.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3499 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat-l.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    17621 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat-p.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    10407 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat-p.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    29188 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat-sudo-aeep.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    14986 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat-sudo-aeep.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8734 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat-sudo-lnp.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4402 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat-sudo-lnp.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    15637 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8068 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/netstat.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      713 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/centos-7.7/ntpq-p.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      474 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/centos-7.7/ntpq-p.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      700 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/centos-7.7/ntpq-pn.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      474 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/centos-7.7/ntpq-pn.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2747 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/passwd.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      961 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/passwd.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      905 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/pip-list.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      616 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/pip-list.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1129 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/pip-show.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      974 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/centos-7.7/pip-show.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    20936 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/ps-axu.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     9932 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/ps-axu.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    14630 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/ps-ef.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8168 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/ps-ef.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      442 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/route-vn.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      338 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/route-vn.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      437 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/route.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      338 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/route.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3206 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/shadow.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      740 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/shadow.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    29301 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/ss-sudo-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    17945 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/ss-sudo-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   322074 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/stat.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   295777 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/stat.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1439 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/systemctl-ls.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1159 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/systemctl-ls.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    14574 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/systemctl-luf.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    13499 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/systemctl-luf.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    31968 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/systemctl.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    38560 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/systemctl.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      276 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/centos-7.7/timedatectl.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      554 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/centos-7.7/timedatectl.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      276 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/uname-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      122 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/uname-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      103 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/uptime.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)       62 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/uptime.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      287 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/centos-7.7/w.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      266 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/centos-7.7/w.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      549 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/who-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      364 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/who-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      155 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/who.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)       93 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/centos-7.7/who.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3397 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/create_fixtures.sh
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:02.000000 jc-1.9.3/tests/fixtures/generic/
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2020-03-02 22:16:03.000000 jc-1.9.3/tests/fixtures/generic/.DS_Store
+-rw-r--r--   0 kbrazil    (501) staff       (20)      849 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-biostats.csv
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1566 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-biostats.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8402 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-cities.csv
+-rw-r--r--   0 kbrazil    (501) staff       (20)    18398 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-cities.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2391 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-deniro.csv
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5146 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-deniro.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1117 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-example.csv
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1588 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-example.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   558246 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-flyrna.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   205281 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-flyrna.tsv
+-rw-r--r--   0 kbrazil    (501) staff       (20)   556670 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-flyrna2.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   203705 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-flyrna2.tsv
+-rw-r--r--   0 kbrazil    (501) staff       (20)      158 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-homes-pipe.csv
+-rw-r--r--   0 kbrazil    (501) staff       (20)      274 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-homes-pipe.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2125 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-homes.csv
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6798 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-homes.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    53816 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-insurance.csv
+-rw-r--r--   0 kbrazil    (501) staff       (20)   229722 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/generic/csv-insurance.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4705 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/ini-iptelserver.ini
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1486 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/ini-iptelserver.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      171 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/ini-test.ini
+-rw-r--r--   0 kbrazil    (501) staff       (20)      270 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/ini-test.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3294 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/xml-cd_catalog.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5077 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/xml-cd_catalog.xml
+-rw-r--r--   0 kbrazil    (501) staff       (20)      811 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/xml-foodmenu.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1102 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/xml-foodmenu.xml
+-rw-r--r--   0 kbrazil    (501) staff       (20)      333 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/yaml-istio-sc.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      305 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/yaml-istio-sc.yaml
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3178 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/yaml-istio-sidecar.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3681 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/generic/yaml-istio-sidecar.yaml
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:02.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2019-12-06 21:09:19.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/.DS_Store
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1669 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/arp-a.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     1036 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/arp-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1151 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/df-h.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      908 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/df-h.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1196 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/df.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      992 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/df.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      439 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/dig-aaaa.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      537 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/dig-aaaa.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      442 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/dig-x.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      529 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/dig-x.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1272 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/dig.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     1188 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/dig.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   221050 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/du.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)   166687 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/du.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3791 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ifconfig.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     1571 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ifconfig.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3791 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ifconfig2.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     1571 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ifconfig2.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4259 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ls-al.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     1851 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ls-al.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4296 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ls-alh.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     1882 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ls-alh.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      533 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ls.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      175 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ls.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      224 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/pip-list.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      168 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/pip-list.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1028 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/pip-show.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      867 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/pip-show.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    53632 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ps-axu.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)    32255 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ps-axu.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    38291 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ps-ef.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)    25921 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/ps-ef.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      233 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/uname-a.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      142 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/uname-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      102 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/uptime.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)       57 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/uptime.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      627 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/w.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      458 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.11.6/w.out
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:02.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2019-12-16 21:35:29.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/.DS_Store
+-rw-r--r--   0 kbrazil    (501) staff       (20)      307 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/airport-I.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      348 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/airport-I.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2152 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/airport-s.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1423 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/airport-s.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1541 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/arp-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      968 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/arp-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2582 2020-03-13 00:09:29.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/arp-a2.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1597 2020-03-13 00:09:29.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/arp-a2.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1686 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/df-h.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1276 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/df-h.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1764 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/df.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1384 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/df.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      438 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/dig-aaaa.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      536 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/dig-aaaa.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5984 2020-03-27 00:16:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/dig-axfr.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3511 2020-03-27 00:16:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/dig-axfr.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      442 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/dig-x.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      529 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/dig-x.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1266 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/dig.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1182 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/dig.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   296296 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/du.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   222287 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/du.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3589 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/file.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2890 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/file.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4715 2020-03-12 15:24:33.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/file2.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4780 2020-03-12 15:24:33.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/file2.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     9646 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/group.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2823 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/group.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      759 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/id.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      386 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/id.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    10823 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ifconfig.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     3779 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ifconfig.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    11375 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ifconfig2.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3979 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ifconfig2.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    45274 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/last.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    25827 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/last.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      852 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-R-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      278 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-R-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   469418 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-R.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   133787 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-R.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4653 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-al.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     2111 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-al.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   959674 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-alR.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   364578 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-alR.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4684 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-alh.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)     2111 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-alh.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    91499 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-glob.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    19369 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-glob.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1162 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-l-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      583 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-l-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   355547 2020-03-08 21:54:48.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-lR-empty-folder.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   128740 2020-03-08 21:54:48.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-lR-empty-folder.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1450 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-lR-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      656 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-lR-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      498 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      260 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      585 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      193 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ls.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      672 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/mount.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      349 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/mount.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      841 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/mount2.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      464 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/mount2.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    14855 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/passwd.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6804 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/passwd.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      224 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/pip-list.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      168 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/pip-list.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1067 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/pip-show.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      910 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/pip-show.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    99173 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ps-axu.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    60107 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ps-axu.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    71162 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ps-ef.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    48758 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/ps-ef.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      221 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/uname-a.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      131 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/uname-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      110 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/uptime.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)       65 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/uptime.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      836 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/w.json
+-rwxr-xr-x   0 kbrazil    (501) staff       (20)      570 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/w.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      659 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/who-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      419 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/who-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      251 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/who.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      128 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/osx-10.14.6/who.out
+drwxr-xr-x   0 kbrazil    (501) staff       (20)        0 2020-03-27 00:17:02.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6148 2020-02-18 21:08:44.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/.DS_Store
+-rw-r--r--   0 kbrazil    (501) staff       (20)      351 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/arp-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      174 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/arp-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      237 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/arp-v.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      274 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/arp-v.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      237 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/arp.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      243 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/arp.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      818 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-multi.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      717 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-multi.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      962 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-udev-multi.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      832 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-udev-multi.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      547 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-udev.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      478 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-udev.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      142 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-sda2.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      115 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-sda2.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      986 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      675 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      939 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/crontab-u.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      752 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/crontab-u.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2261 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/df-h.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1004 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/df-h.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2372 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/df.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1194 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/df.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      458 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/dig-aaaa.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      532 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/dig-aaaa.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5984 2020-03-27 00:16:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/dig-axfr.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3529 2020-03-27 00:16:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/dig-axfr.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      460 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/dig-x.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      523 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/dig-x.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1306 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/dig.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1156 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/dig.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)  1560353 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/du.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)  1136984 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/du.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2651 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/env.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2125 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/env.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1093 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/file.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      729 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/file.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      177 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/free-h.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      204 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/free-h.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      195 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/free.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      204 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/free.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      268 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/fstab.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      120 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/fstab.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3705 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/group.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      721 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/group.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4279 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/gshadow.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      606 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/gshadow.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    22782 2020-02-06 01:00:38.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/history.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    12844 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/history.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      365 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/hosts.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      272 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/hosts.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1090 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ifconfig.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      894 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ifconfig.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      847 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter-line-numbers.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1025 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter-line-numbers.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2363 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter-nv.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2763 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter-nv.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1730 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2035 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      141 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-mangle.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      468 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-mangle.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      106 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-nat.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      375 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-nat.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)       39 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-raw.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      187 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-raw.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      306 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/jobs.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      164 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/jobs.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1852 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/last-w.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1073 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/last-w.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1845 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/last.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1066 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/last.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      125 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lastb.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      111 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lastb.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1114 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-R-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      471 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-R-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   298654 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-R.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    62421 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-R.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3950 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-al.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1744 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-al.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   772252 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-alR.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   262651 2020-02-19 15:07:23.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-alR.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3942 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-alh.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1567 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-alh.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    66907 2020-02-19 15:07:24.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-glob.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    13721 2020-02-19 15:07:24.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-glob.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1176 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-l-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      576 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-l-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2089 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-lR-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      984 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-lR-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      498 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-newlines.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      260 2020-02-27 19:25:11.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-newlines.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      622 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      162 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ls.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    11397 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsblk-allcols.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     7364 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsblk-allcols.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2114 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsblk.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      812 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsblk.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6744 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsmod.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4251 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsmod.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   526695 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsof-sudo.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   342863 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsof-sudo.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)   194044 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsof.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)   132043 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/lsof.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6547 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/mount.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3708 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/mount.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5079 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-l.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2606 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-l.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    14711 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-p.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8706 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-p.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    22957 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-sudo-aeep.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    12016 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-sudo-aeep.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6259 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-sudo-lnp.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3236 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-sudo-lnp.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    12550 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6711 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3333 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-p.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1659 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-p.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3832 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-p2.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1896 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-p2.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3314 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-pn.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1659 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-pn.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1659 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ntqp-p.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4116 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/passwd.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1565 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/passwd.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2638 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-list-legacy.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1041 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-list-legacy.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2638 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-list.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2360 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-list.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      874 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-show.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      730 2019-12-17 20:12:32.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-show.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    31390 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ps-axu.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    14127 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ps-axu.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    21583 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ps-ef.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    11355 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ps-ef.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      447 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/route-vn.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      336 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/route-vn.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      439 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/route.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      336 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/route.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4330 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/shadow.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      939 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/shadow.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    23277 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ss-sudo-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    25599 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/ss-sudo-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    73147 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/stat.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    60023 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/stat.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      270 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-lj.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      244 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-lj.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2431 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-ls.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2072 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-ls.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    18756 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-luf.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    17734 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-luf.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)    47895 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)    76059 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      274 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/timedatectl.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      350 2020-03-11 20:47:39.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/timedatectl.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      268 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/uname-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      114 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/uname-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      109 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/uptime.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)       70 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/uptime.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      292 2019-11-17 20:00:19.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/w.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      274 2019-10-31 15:07:28.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/w.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      452 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/who-a.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      355 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/who-a.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      155 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/who.json
+-rw-r--r--   0 kbrazil    (501) staff       (20)      140 2020-03-03 19:47:13.000000 jc-1.9.3/tests/fixtures/ubuntu-18.04/who.out
+-rw-r--r--   0 kbrazil    (501) staff       (20)      862 2020-03-11 20:47:39.000000 jc-1.9.3/tests/test_airport.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)      866 2020-03-11 20:47:39.000000 jc-1.9.3/tests/test_airport_s.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5350 2020-03-13 00:09:29.000000 jc-1.9.3/tests/test_arp.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6590 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_blkid.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1134 2020-03-11 20:47:39.000000 jc-1.9.3/tests/test_cli.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)      837 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_crontab.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1498 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_crontab_u.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     5383 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_csv.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4669 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_df.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8845 2020-03-27 00:16:11.000000 jc-1.9.3/tests/test_dig.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2415 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_du.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1350 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_env.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2547 2020-03-12 15:24:33.000000 jc-1.9.3/tests/test_file.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2517 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_free.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1406 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_fstab.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1982 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_group.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1444 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_gshadow.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1426 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_history.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1406 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_hosts.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1329 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_id.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3845 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_ifconfig.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1404 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_ini.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     8341 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_iptables.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1369 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_jobs.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4237 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_last.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)    20734 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_ls.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3084 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_lsblk.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1388 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_lsmod.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2563 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_lsof.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2536 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_mount.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     6474 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_netstat.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3178 2020-03-11 20:47:39.000000 jc-1.9.3/tests/test_ntpq.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2012 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_passwd.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3303 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_pip_list.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2637 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_pip_show.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     4805 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_ps.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2570 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_route.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1425 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_shadow.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1445 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_ss.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1383 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_stat.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1470 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_systemctl.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)      907 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_systemctl_lj.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1547 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_systemctl_ls.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1564 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_systemctl_luf.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1502 2020-03-11 20:47:39.000000 jc-1.9.3/tests/test_timedatectl.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2586 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_uname.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2563 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_uptime.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     2370 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_w.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     3599 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_who.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1429 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_xml.py
+-rw-r--r--   0 kbrazil    (501) staff       (20)     1473 2020-03-08 21:54:48.000000 jc-1.9.3/tests/test_yaml.py
```

### Comparing `jc-1.9.2/PKG-INFO` & `jc-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jc
-Version: 1.9.2
+Version: 1.9.3
 Summary: This tool serializes the output of popular command line tools and filetypes to structured JSON output.
 Home-page: https://github.com/kellyjonbrazil/jc
 Author: Kelly Brazil
 Author-email: kellyjonbrazil@gmail.com
 License: MIT
 Description: # JC
         JSON CLI output utility
```

### Comparing `jc-1.9.2/README.md` & `jc-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/__init__.py` & `jc-1.9.3/jc/__init__.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/cli.py` & `jc-1.9.3/jc/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import textwrap
 import signal
 import json
 import jc.utils
 
 
 class info():
-    version = '1.9.2'
+    version = '1.9.3'
     description = 'jc cli output JSON conversion tool'
     author = 'Kelly Brazil'
     author_email = 'kellyjonbrazil@gmail.com'
 
 
 __version__ = info.version
```

### Comparing `jc-1.9.2/jc/parsers/airport.py` & `jc-1.9.3/jc/parsers/airport.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/airport_s.py` & `jc-1.9.3/jc/parsers/airport_s.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/arp.py` & `jc-1.9.3/jc/parsers/arp.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/blkid.py` & `jc-1.9.3/jc/parsers/blkid.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/crontab.py` & `jc-1.9.3/jc/parsers/crontab.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/crontab_u.py` & `jc-1.9.3/jc/parsers/crontab_u.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/csv.py` & `jc-1.9.3/jc/parsers/csv.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/df.py` & `jc-1.9.3/jc/parsers/df.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/dig.py` & `jc-1.9.3/jc/parsers/dig.py`

 * *Files 26% similar despite different names*

```diff
@@ -320,15 +320,15 @@
       }
     ]
 """
 import jc.utils
 
 
 class info():
-    version = '1.0'
+    version = '1.1'
     description = 'dig command parser'
     author = 'Kelly Brazil'
     author_email = 'kellyjonbrazil@gmail.com'
 
     # compatible options: linux, darwin, cygwin, win32, aix, freebsd
     compatible = ['linux', 'aix', 'freebsd', 'darwin']
     magic_commands = ['dig']
@@ -398,14 +398,22 @@
             if key in entry:
                 try:
                     key_int = int(entry[key])
                     entry[key] = key_int
                 except (ValueError):
                     entry[key] = None
 
+        if 'axfr' in entry:
+            for ax in entry['axfr']:
+                try:
+                    ttl_int = int(ax['ttl'])
+                    ax['ttl'] = ttl_int
+                except (ValueError):
+                    ax['ttl'] = None
+
         if 'answer' in entry:
             for ans in entry['answer']:
                 try:
                     ttl_int = int(ans['ttl'])
                     ans['ttl'] = ttl_int
                 except (ValueError):
                     ans['ttl'] = None
@@ -503,14 +511,32 @@
 
     return {'name': answer_name,
             'class': answer_class,
             'type': answer_type,
             'ttl': answer_ttl,
             'data': answer_data}
 
+def parse_axfr(axfr):
+    #; <<>> DiG 9.11.14-3-Debian <<>> @81.4.108.41 axfr zonetransfer.me +nocookie
+    #; (1 server found)
+    #;; global options: +cmd
+    #zonetransfer.me. 7200 IN A 5.196.105.14
+    axfr = axfr.split(maxsplit=4)
+    axfr_name = axfr[0]
+    axfr_ttl = axfr[1]
+    axfr_class = axfr[2]
+    axfr_type = axfr[3]
+    axfr_data = axfr[4]
+
+    return {'name': axfr_name,
+            'ttl': axfr_ttl,
+            'class': axfr_class,
+            'type': axfr_type,
+            'data': axfr_data}
+
 
 def parse(data, raw=False, quiet=False):
     """
     Main text parsing function
 
     Parameters:
 
@@ -530,85 +556,108 @@
     cleandata = data.splitlines()
     # remove blank lines
     cleandata = list(filter(None, cleandata))
 
     question = False
     authority = False
     answer = False
+    axfr = False
 
     output_entry = {}
     for line in cleandata:
 
-        if line.find(';; ->>HEADER<<-') == 0:
+        if line.startswith('; <<>> ') and line.lower().find(' axfr ') != -1:
+            question = False
+            authority = False
+            answer = False
+            axfr = True
+            axfr_list = []
+            continue
+
+        if line.find(';') == -1 and axfr:
+            axfr_list.append(parse_axfr(line))
+            output_entry.update({'axfr': axfr_list})
+            continue
+
+        if line.startswith(';; ->>HEADER<<-'):
             output_entry = {}
             output_entry.update(parse_header(line))
             continue
 
-        if line.find(';; flags:') == 0:
+        if line.startswith(';; flags:'):
             output_entry.update(parse_flags_line(line))
             continue
 
-        if line.find(';; QUESTION SECTION:') == 0:
+        if line.startswith(';; QUESTION SECTION:'):
             question = True
             authority = False
             answer = False
+            axfr = False
             continue
 
         if question:
             output_entry['question'] = parse_question(line)
             question = False
             authority = False
             answer = False
+            axfr = False
             continue
 
-        if line.find(';; AUTHORITY SECTION:') == 0:
+        if line.startswith(';; AUTHORITY SECTION:'):
             question = False
             authority = True
             answer = False
+            axfr = False
             authority_list = []
             continue
 
         if line.find(';') == -1 and authority:
             authority_list.append(parse_authority(line))
             output_entry.update({'authority': authority_list})
             continue
 
-        if line.find(';; ANSWER SECTION:') == 0:
+        if line.startswith(';; ANSWER SECTION:'):
             question = False
             authority = False
             answer = True
+            axfr = False
             answer_list = []
             continue
 
         if line.find(';') == -1 and answer:
             answer_list.append(parse_answer(line))
             output_entry.update({'answer': answer_list})
             continue
 
         # footer consists of 4 lines
         # footer line 1
-        if line.find(';; Query time:') == 0:
+        if line.startswith(';; Query time:'):
             output_entry.update({'query_time': line.split(':')[1].lstrip()})
             continue
 
         # footer line 2
-        if line.find(';; SERVER:') == 0:
+        if line.startswith(';; SERVER:'):
             output_entry.update({'server': line.split(':')[1].lstrip()})
             continue
 
         # footer line 3
-        if line.find(';; WHEN:') == 0:
+        if line.startswith(';; WHEN:'):
             output_entry.update({'when': line.split(':', maxsplit=1)[1].lstrip()})
             continue
 
         # footer line 4 (last line)
-        if line.find(';; MSG SIZE  rcvd:') == 0:
+        if line.startswith(';; MSG SIZE  rcvd:'):
             output_entry.update({'rcvd': line.split(':')[1].lstrip()})
 
             if output_entry:
                 raw_output.append(output_entry)
+        elif line.startswith(';; XFR size:'):
+            output_entry.update({'size': line.split(':')[1].lstrip()})
+
+            if output_entry:
+                raw_output.append(output_entry)
 
     raw_output = list(filter(None, raw_output))
     if raw:
         return raw_output
     else:
         return process(raw_output)
```

### Comparing `jc-1.9.2/jc/parsers/du.py` & `jc-1.9.3/jc/parsers/du.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/env.py` & `jc-1.9.3/jc/parsers/env.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/file.py` & `jc-1.9.3/jc/parsers/file.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/foo.py` & `jc-1.9.3/jc/parsers/foo.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/free.py` & `jc-1.9.3/jc/parsers/free.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/fstab.py` & `jc-1.9.3/jc/parsers/fstab.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/group.py` & `jc-1.9.3/jc/parsers/group.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/gshadow.py` & `jc-1.9.3/jc/parsers/gshadow.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/history.py` & `jc-1.9.3/jc/parsers/history.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/hosts.py` & `jc-1.9.3/jc/parsers/hosts.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/id.py` & `jc-1.9.3/jc/parsers/id.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/ifconfig.py` & `jc-1.9.3/jc/parsers/ifconfig.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/ini.py` & `jc-1.9.3/jc/parsers/ini.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/iptables.py` & `jc-1.9.3/jc/parsers/iptables.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/jobs.py` & `jc-1.9.3/jc/parsers/jobs.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/last.py` & `jc-1.9.3/jc/parsers/last.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/ls.py` & `jc-1.9.3/jc/parsers/ls.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/lsblk.py` & `jc-1.9.3/jc/parsers/lsblk.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/lsmod.py` & `jc-1.9.3/jc/parsers/lsmod.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/lsof.py` & `jc-1.9.3/jc/parsers/lsof.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/mount.py` & `jc-1.9.3/jc/parsers/mount.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/netstat.py` & `jc-1.9.3/jc/parsers/netstat.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/ntpq.py` & `jc-1.9.3/jc/parsers/ntpq.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/passwd.py` & `jc-1.9.3/jc/parsers/passwd.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/pip_list.py` & `jc-1.9.3/jc/parsers/pip_list.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/pip_show.py` & `jc-1.9.3/jc/parsers/pip_show.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/ps.py` & `jc-1.9.3/jc/parsers/ps.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/route.py` & `jc-1.9.3/jc/parsers/route.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/shadow.py` & `jc-1.9.3/jc/parsers/shadow.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/ss.py` & `jc-1.9.3/jc/parsers/ss.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/stat.py` & `jc-1.9.3/jc/parsers/stat.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/systemctl.py` & `jc-1.9.3/jc/parsers/systemctl.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/systemctl_lj.py` & `jc-1.9.3/jc/parsers/systemctl_lj.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/systemctl_ls.py` & `jc-1.9.3/jc/parsers/systemctl_ls.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/systemctl_luf.py` & `jc-1.9.3/jc/parsers/systemctl_luf.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/timedatectl.py` & `jc-1.9.3/jc/parsers/timedatectl.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/uname.py` & `jc-1.9.3/jc/parsers/uname.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/universal.py` & `jc-1.9.3/jc/parsers/universal.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/uptime.py` & `jc-1.9.3/jc/parsers/uptime.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/w.py` & `jc-1.9.3/jc/parsers/w.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/who.py` & `jc-1.9.3/jc/parsers/who.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/xml.py` & `jc-1.9.3/jc/parsers/xml.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/parsers/yaml.py` & `jc-1.9.3/jc/parsers/yaml.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc/utils.py` & `jc-1.9.3/jc/utils.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/jc.egg-info/PKG-INFO` & `jc-1.9.3/jc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jc
-Version: 1.9.2
+Version: 1.9.3
 Summary: This tool serializes the output of popular command line tools and filetypes to structured JSON output.
 Home-page: https://github.com/kellyjonbrazil/jc
 Author: Kelly Brazil
 Author-email: kellyjonbrazil@gmail.com
 License: MIT
 Description: # JC
         JSON CLI output utility
```

### Comparing `jc-1.9.2/jc.egg-info/SOURCES.txt` & `jc-1.9.3/jc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,16 @@
 tests/fixtures/centos-7.7/crontab.out
 tests/fixtures/centos-7.7/df-h.json
 tests/fixtures/centos-7.7/df-h.out
 tests/fixtures/centos-7.7/df.json
 tests/fixtures/centos-7.7/df.out
 tests/fixtures/centos-7.7/dig-aaaa.json
 tests/fixtures/centos-7.7/dig-aaaa.out
+tests/fixtures/centos-7.7/dig-axfr.json
+tests/fixtures/centos-7.7/dig-axfr.out
 tests/fixtures/centos-7.7/dig-x.json
 tests/fixtures/centos-7.7/dig-x.out
 tests/fixtures/centos-7.7/dig.json
 tests/fixtures/centos-7.7/dig.out
 tests/fixtures/centos-7.7/du.json
 tests/fixtures/centos-7.7/du.out
 tests/fixtures/centos-7.7/env.json
@@ -357,14 +359,16 @@
 tests/fixtures/osx-10.14.6/arp-a2.out
 tests/fixtures/osx-10.14.6/df-h.json
 tests/fixtures/osx-10.14.6/df-h.out
 tests/fixtures/osx-10.14.6/df.json
 tests/fixtures/osx-10.14.6/df.out
 tests/fixtures/osx-10.14.6/dig-aaaa.json
 tests/fixtures/osx-10.14.6/dig-aaaa.out
+tests/fixtures/osx-10.14.6/dig-axfr.json
+tests/fixtures/osx-10.14.6/dig-axfr.out
 tests/fixtures/osx-10.14.6/dig-x.json
 tests/fixtures/osx-10.14.6/dig-x.out
 tests/fixtures/osx-10.14.6/dig.json
 tests/fixtures/osx-10.14.6/dig.out
 tests/fixtures/osx-10.14.6/du.json
 tests/fixtures/osx-10.14.6/du.out
 tests/fixtures/osx-10.14.6/file.json
@@ -448,14 +452,16 @@
 tests/fixtures/ubuntu-18.04/crontab-u.out
 tests/fixtures/ubuntu-18.04/df-h.json
 tests/fixtures/ubuntu-18.04/df-h.out
 tests/fixtures/ubuntu-18.04/df.json
 tests/fixtures/ubuntu-18.04/df.out
 tests/fixtures/ubuntu-18.04/dig-aaaa.json
 tests/fixtures/ubuntu-18.04/dig-aaaa.out
+tests/fixtures/ubuntu-18.04/dig-axfr.json
+tests/fixtures/ubuntu-18.04/dig-axfr.out
 tests/fixtures/ubuntu-18.04/dig-x.json
 tests/fixtures/ubuntu-18.04/dig-x.out
 tests/fixtures/ubuntu-18.04/dig.json
 tests/fixtures/ubuntu-18.04/dig.out
 tests/fixtures/ubuntu-18.04/du.json
 tests/fixtures/ubuntu-18.04/du.out
 tests/fixtures/ubuntu-18.04/env.json
```

### Comparing `jc-1.9.2/setup.py` & `jc-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='jc',
-    version='1.9.2',
+    version='1.9.3',
     author='Kelly Brazil',
     author_email='kellyjonbrazil@gmail.com',
     description='This tool serializes the output of popular command line tools and filetypes to structured JSON output.',
     install_requires=[
         'ifconfig-parser>=0.0.5',
         'ruamel.yaml>=0.15.0',
         'xmltodict>=0.12.0'
```

### Comparing `jc-1.9.2/tests/fixtures/.DS_Store` & `jc-1.9.3/tests/fixtures/.DS_Store`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/.DS_Store` & `jc-1.9.3/tests/fixtures/centos-7.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-multi.json` & `jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-multi.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-multi.out` & `jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-multi.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-udev-multi.json` & `jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-udev-multi.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/blkid-ip-udev-multi.out` & `jc-1.9.3/tests/fixtures/centos-7.7/blkid-ip-udev-multi.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/crontab.json` & `jc-1.9.3/tests/fixtures/centos-7.7/crontab.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/crontab.out` & `jc-1.9.3/tests/fixtures/centos-7.7/crontab.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/df-h.json` & `jc-1.9.3/tests/fixtures/centos-7.7/df-h.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/df.json` & `jc-1.9.3/tests/fixtures/centos-7.7/df.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/df.out` & `jc-1.9.3/tests/fixtures/centos-7.7/df.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/dig-aaaa.out` & `jc-1.9.3/tests/fixtures/centos-7.7/dig-aaaa.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/dig-x.out` & `jc-1.9.3/tests/fixtures/centos-7.7/dig-x.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/dig.json` & `jc-1.9.3/tests/fixtures/centos-7.7/dig.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/dig.out` & `jc-1.9.3/tests/fixtures/centos-7.7/dig.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/du.json` & `jc-1.9.3/tests/fixtures/centos-7.7/du.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/du.out` & `jc-1.9.3/tests/fixtures/centos-7.7/du.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/env.json` & `jc-1.9.3/tests/fixtures/centos-7.7/env.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/env.out` & `jc-1.9.3/tests/fixtures/centos-7.7/env.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/file.json` & `jc-1.9.3/tests/fixtures/centos-7.7/file.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/file.out` & `jc-1.9.3/tests/fixtures/centos-7.7/file.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/group.json` & `jc-1.9.3/tests/fixtures/centos-7.7/group.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/gshadow.json` & `jc-1.9.3/tests/fixtures/centos-7.7/gshadow.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/history.json` & `jc-1.9.3/tests/fixtures/centos-7.7/history.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/history.out` & `jc-1.9.3/tests/fixtures/centos-7.7/history.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ifconfig.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ifconfig.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ifconfig.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ifconfig.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter-line-numbers.json` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter-line-numbers.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter-line-numbers.out` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter-line-numbers.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter-nv.json` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter-nv.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter-nv.out` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter-nv.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter.json` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-filter.out` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-filter.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-mangle.json` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-mangle.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-mangle.out` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-mangle.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-nat.json` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-nat.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-nat.out` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-nat.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-raw.json` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-raw.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/iptables-raw.out` & `jc-1.9.3/tests/fixtures/centos-7.7/iptables-raw.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/last-w.json` & `jc-1.9.3/tests/fixtures/centos-7.7/last-w.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/last-w.out` & `jc-1.9.3/tests/fixtures/centos-7.7/last-w.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/last.json` & `jc-1.9.3/tests/fixtures/centos-7.7/last.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/last.out` & `jc-1.9.3/tests/fixtures/centos-7.7/last.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-R-newlines.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-R-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-R-newlines.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-R-newlines.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-R.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-R.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-R.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-R.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-al.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-al.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-al.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-al.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-alR.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-alR.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-alR.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-alR.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-alh.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-alh.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-alh.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-alh.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-glob.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-glob.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-glob.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-glob.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-l-newlines.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-l-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-l-newlines.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-l-newlines.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-lR-newlines.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-lR-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ls-lR-newlines.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ls-lR-newlines.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsblk-allcols.json` & `jc-1.9.3/tests/fixtures/centos-7.7/lsblk-allcols.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsblk-allcols.out` & `jc-1.9.3/tests/fixtures/centos-7.7/lsblk-allcols.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsblk.json` & `jc-1.9.3/tests/fixtures/centos-7.7/lsblk.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsmod.json` & `jc-1.9.3/tests/fixtures/centos-7.7/lsmod.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsmod.out` & `jc-1.9.3/tests/fixtures/centos-7.7/lsmod.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsof-sudo.json` & `jc-1.9.3/tests/fixtures/centos-7.7/lsof-sudo.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsof-sudo.out` & `jc-1.9.3/tests/fixtures/centos-7.7/lsof-sudo.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsof.json` & `jc-1.9.3/tests/fixtures/centos-7.7/lsof.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/lsof.out` & `jc-1.9.3/tests/fixtures/centos-7.7/lsof.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/mount.json` & `jc-1.9.3/tests/fixtures/centos-7.7/mount.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/mount.out` & `jc-1.9.3/tests/fixtures/centos-7.7/mount.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat-l.json` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat-l.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat-l.out` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat-l.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat-p.json` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat-p.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat-p.out` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat-p.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat-sudo-aeep.json` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat-sudo-aeep.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat-sudo-aeep.out` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat-sudo-aeep.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat-sudo-lnp.json` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat-sudo-lnp.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat-sudo-lnp.out` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat-sudo-lnp.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat.json` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/netstat.out` & `jc-1.9.3/tests/fixtures/centos-7.7/netstat.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ntpq-p.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ntpq-p.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ntpq-pn.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ntpq-pn.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/passwd.json` & `jc-1.9.3/tests/fixtures/centos-7.7/passwd.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/passwd.out` & `jc-1.9.3/tests/fixtures/centos-7.7/passwd.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/pip-list.json` & `jc-1.9.3/tests/fixtures/centos-7.7/pip-list.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/pip-list.out` & `jc-1.9.3/tests/fixtures/centos-7.7/pip-list.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/pip-show.json` & `jc-1.9.3/tests/fixtures/centos-7.7/pip-show.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/pip-show.out` & `jc-1.9.3/tests/fixtures/centos-7.7/pip-show.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ps-axu.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ps-axu.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ps-axu.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ps-axu.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ps-ef.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ps-ef.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ps-ef.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ps-ef.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/shadow.json` & `jc-1.9.3/tests/fixtures/centos-7.7/shadow.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/shadow.out` & `jc-1.9.3/tests/fixtures/centos-7.7/shadow.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ss-sudo-a.json` & `jc-1.9.3/tests/fixtures/centos-7.7/ss-sudo-a.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/ss-sudo-a.out` & `jc-1.9.3/tests/fixtures/centos-7.7/ss-sudo-a.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/stat.json` & `jc-1.9.3/tests/fixtures/centos-7.7/stat.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/stat.out` & `jc-1.9.3/tests/fixtures/centos-7.7/stat.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/systemctl-ls.json` & `jc-1.9.3/tests/fixtures/centos-7.7/systemctl-ls.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/systemctl-ls.out` & `jc-1.9.3/tests/fixtures/centos-7.7/systemctl-ls.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/systemctl-luf.json` & `jc-1.9.3/tests/fixtures/centos-7.7/systemctl-luf.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/systemctl-luf.out` & `jc-1.9.3/tests/fixtures/centos-7.7/systemctl-luf.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/systemctl.json` & `jc-1.9.3/tests/fixtures/centos-7.7/systemctl.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/systemctl.out` & `jc-1.9.3/tests/fixtures/centos-7.7/systemctl.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/timedatectl.out` & `jc-1.9.3/tests/fixtures/centos-7.7/timedatectl.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/centos-7.7/who-a.json` & `jc-1.9.3/tests/fixtures/centos-7.7/who-a.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/create_fixtures.sh` & `jc-1.9.3/tests/fixtures/create_fixtures.sh`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/.DS_Store` & `jc-1.9.3/tests/fixtures/generic/.DS_Store`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-biostats.csv` & `jc-1.9.3/tests/fixtures/generic/csv-biostats.csv`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-biostats.json` & `jc-1.9.3/tests/fixtures/generic/csv-biostats.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-cities.csv` & `jc-1.9.3/tests/fixtures/generic/csv-cities.csv`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-cities.json` & `jc-1.9.3/tests/fixtures/generic/csv-cities.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-deniro.csv` & `jc-1.9.3/tests/fixtures/generic/csv-deniro.csv`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-deniro.json` & `jc-1.9.3/tests/fixtures/generic/csv-deniro.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-example.csv` & `jc-1.9.3/tests/fixtures/generic/csv-example.csv`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-example.json` & `jc-1.9.3/tests/fixtures/generic/csv-example.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-flyrna.json` & `jc-1.9.3/tests/fixtures/generic/csv-flyrna.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-flyrna.tsv` & `jc-1.9.3/tests/fixtures/generic/csv-flyrna.tsv`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-flyrna2.json` & `jc-1.9.3/tests/fixtures/generic/csv-flyrna2.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-flyrna2.tsv` & `jc-1.9.3/tests/fixtures/generic/csv-flyrna2.tsv`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-homes.csv` & `jc-1.9.3/tests/fixtures/generic/csv-homes.csv`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-homes.json` & `jc-1.9.3/tests/fixtures/generic/csv-homes.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-insurance.csv` & `jc-1.9.3/tests/fixtures/generic/csv-insurance.csv`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/csv-insurance.json` & `jc-1.9.3/tests/fixtures/generic/csv-insurance.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/ini-iptelserver.ini` & `jc-1.9.3/tests/fixtures/generic/ini-iptelserver.ini`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/ini-iptelserver.json` & `jc-1.9.3/tests/fixtures/generic/ini-iptelserver.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/xml-cd_catalog.json` & `jc-1.9.3/tests/fixtures/generic/xml-cd_catalog.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/xml-cd_catalog.xml` & `jc-1.9.3/tests/fixtures/generic/xml-cd_catalog.xml`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/xml-foodmenu.json` & `jc-1.9.3/tests/fixtures/generic/xml-foodmenu.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/xml-foodmenu.xml` & `jc-1.9.3/tests/fixtures/generic/xml-foodmenu.xml`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/yaml-istio-sidecar.json` & `jc-1.9.3/tests/fixtures/generic/yaml-istio-sidecar.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/generic/yaml-istio-sidecar.yaml` & `jc-1.9.3/tests/fixtures/generic/yaml-istio-sidecar.yaml`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/.DS_Store` & `jc-1.9.3/tests/fixtures/osx-10.11.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/arp-a.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/arp-a.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/arp-a.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/arp-a.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/df-h.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/df-h.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/df-h.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/df-h.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/df.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/df.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/df.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/df.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/dig-aaaa.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/dig-aaaa.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/dig-x.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/dig-x.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/dig.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/dig.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/dig.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/dig.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/du.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/du.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/du.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/du.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ifconfig.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ifconfig.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ifconfig.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ifconfig.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ifconfig2.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ifconfig2.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ifconfig2.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ifconfig2.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ls-al.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ls-al.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ls-al.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ls-al.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ls-alh.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ls-alh.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ls-alh.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ls-alh.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ls.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ls.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/pip-show.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/pip-show.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/pip-show.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/pip-show.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ps-axu.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ps-axu.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ps-axu.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ps-axu.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ps-ef.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ps-ef.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/ps-ef.out` & `jc-1.9.3/tests/fixtures/osx-10.11.6/ps-ef.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.11.6/w.json` & `jc-1.9.3/tests/fixtures/osx-10.11.6/w.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/.DS_Store` & `jc-1.9.3/tests/fixtures/osx-10.14.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/airport-s.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/airport-s.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/airport-s.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/airport-s.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/arp-a.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/arp-a.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/arp-a.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/arp-a.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/arp-a2.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/arp-a2.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/arp-a2.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/arp-a2.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/df-h.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/df-h.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/df-h.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/df-h.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/df.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/df.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/df.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/df.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/dig-aaaa.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/dig-aaaa.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/dig-x.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/dig-x.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/dig.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/dig.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/dig.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/dig.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/du.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/du.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/du.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/du.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/file.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/file.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/file.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/file.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/file2.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/file2.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/file2.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/file2.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/group.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/group.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/group.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/group.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/id.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/id.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ifconfig.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ifconfig.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ifconfig.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ifconfig.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ifconfig2.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ifconfig2.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ifconfig2.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ifconfig2.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/last.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/last.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/last.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/last.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-R-newlines.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-R-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-R.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-R.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-R.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-R.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-al.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-al.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-al.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-al.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-alR.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-alR.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-alR.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-alR.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-alh.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-alh.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-alh.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-alh.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-glob.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-glob.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-glob.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-glob.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-l-newlines.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-l-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-l-newlines.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-l-newlines.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-lR-empty-folder.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-lR-empty-folder.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-lR-empty-folder.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-lR-empty-folder.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-lR-newlines.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-lR-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls-lR-newlines.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls-lR-newlines.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ls.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ls.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/mount.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/mount.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/mount2.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/mount2.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/passwd.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/passwd.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/passwd.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/passwd.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/pip-show.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/pip-show.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/pip-show.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/pip-show.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ps-axu.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ps-axu.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ps-axu.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ps-axu.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ps-ef.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ps-ef.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/ps-ef.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/ps-ef.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/w.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/w.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/w.out` & `jc-1.9.3/tests/fixtures/osx-10.14.6/w.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/osx-10.14.6/who-a.json` & `jc-1.9.3/tests/fixtures/osx-10.14.6/who-a.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/.DS_Store` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/.DS_Store`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-multi.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-multi.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-multi.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-multi.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-udev-multi.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-udev-multi.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-udev-multi.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-udev-multi.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid-ip-udev.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid-ip-udev.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/blkid.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/blkid.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/crontab-u.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/crontab-u.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/crontab-u.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/crontab-u.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/df-h.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/df-h.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/df-h.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/df-h.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/df.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/df.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/df.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/df.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/dig-aaaa.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/dig-aaaa.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/dig-x.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/dig-x.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/dig.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/dig.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/dig.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/dig.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/du.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/du.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/du.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/du.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/env.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/env.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/env.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/env.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/file.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/file.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/file.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/file.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/group.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/group.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/group.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/group.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/gshadow.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/gshadow.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/gshadow.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/gshadow.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/history.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/history.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/history.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/history.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ifconfig.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ifconfig.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ifconfig.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ifconfig.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter-line-numbers.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter-line-numbers.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter-line-numbers.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter-line-numbers.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter-nv.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter-nv.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter-nv.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter-nv.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/iptables-filter.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/iptables-filter.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/last-w.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/last-w.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/last-w.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/last-w.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/last.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/last.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/last.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/last.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-R-newlines.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-R-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-R.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-R.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-R.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-R.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-al.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-al.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-al.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-al.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-alR.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-alR.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-alR.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-alR.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-alh.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-alh.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-alh.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-alh.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-glob.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-glob.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-glob.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-glob.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-l-newlines.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-l-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-l-newlines.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-l-newlines.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-lR-newlines.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-lR-newlines.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls-lR-newlines.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls-lR-newlines.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ls.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ls.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsblk-allcols.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsblk-allcols.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsblk-allcols.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsblk-allcols.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsblk.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsblk.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsblk.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsblk.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsmod.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsmod.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsmod.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsmod.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsof-sudo.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsof-sudo.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsof-sudo.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsof-sudo.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsof.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsof.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/lsof.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/lsof.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/mount.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/mount.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/mount.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/mount.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-l.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-l.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-l.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-l.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-p.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-p.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-p.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-p.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-sudo-aeep.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-sudo-aeep.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-sudo-aeep.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-sudo-aeep.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-sudo-lnp.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-sudo-lnp.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat-sudo-lnp.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat-sudo-lnp.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/netstat.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/netstat.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-p.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-p.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-p.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-p.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-p2.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-p2.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-p2.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-p2.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-pn.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-pn.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ntpq-pn.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ntpq-pn.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ntqp-p.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ntqp-p.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/passwd.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/passwd.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/passwd.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/passwd.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-list-legacy.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-list-legacy.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-list-legacy.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-list-legacy.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-list.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-list.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-list.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-list.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-show.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-show.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/pip-show.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/pip-show.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ps-axu.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ps-axu.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ps-axu.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ps-axu.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ps-ef.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ps-ef.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ps-ef.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ps-ef.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/shadow.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/shadow.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/shadow.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/shadow.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ss-sudo-a.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ss-sudo-a.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/ss-sudo-a.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/ss-sudo-a.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/stat.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/stat.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/stat.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/stat.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-ls.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-ls.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-ls.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-ls.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-luf.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-luf.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl-luf.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl-luf.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl.json` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl.json`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/fixtures/ubuntu-18.04/systemctl.out` & `jc-1.9.3/tests/fixtures/ubuntu-18.04/systemctl.out`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_airport.py` & `jc-1.9.3/tests/test_airport.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_airport_s.py` & `jc-1.9.3/tests/test_airport_s.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_arp.py` & `jc-1.9.3/tests/test_arp.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_blkid.py` & `jc-1.9.3/tests/test_blkid.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_cli.py` & `jc-1.9.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_crontab.py` & `jc-1.9.3/tests/test_crontab.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_crontab_u.py` & `jc-1.9.3/tests/test_crontab_u.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_csv.py` & `jc-1.9.3/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_df.py` & `jc-1.9.3/tests/test_df.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_dig.py` & `jc-1.9.3/tests/test_who.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 import os
 import json
 import unittest
-import jc.parsers.dig
+import jc.parsers.who
 
 THIS_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 class MyTests(unittest.TestCase):
 
     def setUp(self):
         # input
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/dig.out'), 'r', encoding='utf-8') as f:
-            self.centos_7_7_dig = f.read()
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/who.out'), 'r', encoding='utf-8') as f:
+            self.centos_7_7_who = f.read()
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/dig.out'), 'r', encoding='utf-8') as f:
-            self.ubuntu_18_4_dig = f.read()
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/who.out'), 'r', encoding='utf-8') as f:
+            self.ubuntu_18_4_who = f.read()
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/dig-x.out'), 'r', encoding='utf-8') as f:
-            self.centos_7_7_dig_x = f.read()
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/osx-10.14.6/who.out'), 'r', encoding='utf-8') as f:
+            self.osx_10_14_6_who = f.read()
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/dig-x.out'), 'r', encoding='utf-8') as f:
-            self.ubuntu_18_4_dig_x = f.read()
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/who-a.out'), 'r', encoding='utf-8') as f:
+            self.centos_7_7_who_a = f.read()
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/dig-aaaa.out'), 'r', encoding='utf-8') as f:
-            self.centos_7_7_dig_aaaa = f.read()
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/who-a.out'), 'r', encoding='utf-8') as f:
+            self.ubuntu_18_4_who_a = f.read()
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/dig-aaaa.out'), 'r', encoding='utf-8') as f:
-            self.ubuntu_18_4_dig_aaaa = f.read()
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/osx-10.14.6/who-a.out'), 'r', encoding='utf-8') as f:
+            self.osx_10_14_6_who_a = f.read()
 
         # output
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/dig.json'), 'r', encoding='utf-8') as f:
-            self.centos_7_7_dig_json = json.loads(f.read())
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/who.json'), 'r', encoding='utf-8') as f:
+            self.centos_7_7_who_json = json.loads(f.read())
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/dig.json'), 'r', encoding='utf-8') as f:
-            self.ubuntu_18_4_dig_json = json.loads(f.read())
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/who.json'), 'r', encoding='utf-8') as f:
+            self.ubuntu_18_4_who_json = json.loads(f.read())
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/dig-x.json'), 'r', encoding='utf-8') as f:
-            self.centos_7_7_dig_x_json = json.loads(f.read())
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/osx-10.14.6/who.json'), 'r', encoding='utf-8') as f:
+            self.osx_10_14_6_who_json = json.loads(f.read())
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/dig-x.json'), 'r', encoding='utf-8') as f:
-            self.ubuntu_18_4_dig_x_json = json.loads(f.read())
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/who-a.json'), 'r', encoding='utf-8') as f:
+            self.centos_7_7_who_a_json = json.loads(f.read())
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/centos-7.7/dig-aaaa.json'), 'r', encoding='utf-8') as f:
-            self.centos_7_7_dig_aaaa_json = json.loads(f.read())
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/who-a.json'), 'r', encoding='utf-8') as f:
+            self.ubuntu_18_4_who_a_json = json.loads(f.read())
 
-        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/ubuntu-18.04/dig-aaaa.json'), 'r', encoding='utf-8') as f:
-            self.ubuntu_18_4_dig_aaaa_json = json.loads(f.read())
+        with open(os.path.join(THIS_DIR, os.pardir, 'tests/fixtures/osx-10.14.6/who-a.json'), 'r', encoding='utf-8') as f:
+            self.osx_10_14_6_who_a_json = json.loads(f.read())
 
-    def test_dig_centos_7_7(self):
+    def test_who_centos_7_7(self):
         """
-        Test 'dig' on Centos 7.7
+        Test 'who' on Centos 7.7
         """
-        self.assertEqual(jc.parsers.dig.parse(self.centos_7_7_dig, quiet=True), self.centos_7_7_dig_json)
+        self.assertEqual(jc.parsers.who.parse(self.centos_7_7_who, quiet=True), self.centos_7_7_who_json)
 
-    def test_dig_ubuntu_18_4(self):
+    def test_who_ubuntu_18_4(self):
         """
-        Test 'dig' on Ubuntu 18.4
+        Test 'who' on Ubuntu 18.4
         """
-        self.assertEqual(jc.parsers.dig.parse(self.ubuntu_18_4_dig, quiet=True), self.ubuntu_18_4_dig_json)
+        self.assertEqual(jc.parsers.who.parse(self.ubuntu_18_4_who, quiet=True), self.ubuntu_18_4_who_json)
 
-    def test_dig_x_centos_7_7(self):
+    def test_who_osx_10_14_6(self):
         """
-        Test 'dig -x' on Centos 7.7
+        Test 'who' on OSX 10.14.6
         """
-        self.assertEqual(jc.parsers.dig.parse(self.centos_7_7_dig_x, quiet=True), self.centos_7_7_dig_x_json)
+        self.assertEqual(jc.parsers.who.parse(self.osx_10_14_6_who, quiet=True), self.osx_10_14_6_who_json)
 
-    def test_dig_x_ubuntu_18_4(self):
+    def test_who_a_centos_7_7(self):
         """
-        Test 'dig -x' on Ubuntu 18.4
+        Test 'who -a' on Centos 7.7
         """
-        self.assertEqual(jc.parsers.dig.parse(self.ubuntu_18_4_dig_x, quiet=True), self.ubuntu_18_4_dig_x_json)
+        self.assertEqual(jc.parsers.who.parse(self.centos_7_7_who_a, quiet=True), self.centos_7_7_who_a_json)
 
-    def test_dig_aaaa_centos_7_7(self):
+    def test_who_a_ubuntu_18_4(self):
         """
-        Test 'dig AAAA' on Centos 7.7
+        Test 'who -a' on Ubuntu 18.4
         """
-        self.assertEqual(jc.parsers.dig.parse(self.centos_7_7_dig_aaaa, quiet=True), self.centos_7_7_dig_aaaa_json)
+        self.assertEqual(jc.parsers.who.parse(self.ubuntu_18_4_who_a, quiet=True), self.ubuntu_18_4_who_a_json)
 
-    def test_dig_aaaa_ubuntu_18_4(self):
+    def test_who_a_osx_10_14_6(self):
         """
-        Test 'dig AAAA' on Ubuntu 18.4
+        Test 'who -a' on OSX 10.14.6
         """
-        self.assertEqual(jc.parsers.dig.parse(self.ubuntu_18_4_dig_aaaa, quiet=True), self.ubuntu_18_4_dig_aaaa_json)
+        self.assertEqual(jc.parsers.who.parse(self.osx_10_14_6_who_a, quiet=True), self.osx_10_14_6_who_a_json)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `jc-1.9.2/tests/test_du.py` & `jc-1.9.3/tests/test_du.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_env.py` & `jc-1.9.3/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_file.py` & `jc-1.9.3/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_free.py` & `jc-1.9.3/tests/test_free.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_fstab.py` & `jc-1.9.3/tests/test_fstab.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_group.py` & `jc-1.9.3/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_gshadow.py` & `jc-1.9.3/tests/test_gshadow.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_history.py` & `jc-1.9.3/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_hosts.py` & `jc-1.9.3/tests/test_hosts.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_id.py` & `jc-1.9.3/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_ifconfig.py` & `jc-1.9.3/tests/test_ifconfig.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_ini.py` & `jc-1.9.3/tests/test_ini.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_iptables.py` & `jc-1.9.3/tests/test_iptables.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_jobs.py` & `jc-1.9.3/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_last.py` & `jc-1.9.3/tests/test_last.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_ls.py` & `jc-1.9.3/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_lsblk.py` & `jc-1.9.3/tests/test_lsblk.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_lsmod.py` & `jc-1.9.3/tests/test_lsmod.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_lsof.py` & `jc-1.9.3/tests/test_lsof.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_mount.py` & `jc-1.9.3/tests/test_mount.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_netstat.py` & `jc-1.9.3/tests/test_netstat.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_ntpq.py` & `jc-1.9.3/tests/test_ntpq.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_passwd.py` & `jc-1.9.3/tests/test_passwd.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_pip_list.py` & `jc-1.9.3/tests/test_pip_list.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_pip_show.py` & `jc-1.9.3/tests/test_pip_show.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_ps.py` & `jc-1.9.3/tests/test_ps.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_route.py` & `jc-1.9.3/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_shadow.py` & `jc-1.9.3/tests/test_shadow.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_ss.py` & `jc-1.9.3/tests/test_ss.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_stat.py` & `jc-1.9.3/tests/test_stat.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_systemctl.py` & `jc-1.9.3/tests/test_systemctl.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_systemctl_lj.py` & `jc-1.9.3/tests/test_systemctl_lj.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_systemctl_ls.py` & `jc-1.9.3/tests/test_systemctl_ls.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_systemctl_luf.py` & `jc-1.9.3/tests/test_systemctl_luf.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_timedatectl.py` & `jc-1.9.3/tests/test_timedatectl.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_uname.py` & `jc-1.9.3/tests/test_uname.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_uptime.py` & `jc-1.9.3/tests/test_uptime.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_w.py` & `jc-1.9.3/tests/test_w.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_xml.py` & `jc-1.9.3/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `jc-1.9.2/tests/test_yaml.py` & `jc-1.9.3/tests/test_yaml.py`

 * *Files identical despite different names*

