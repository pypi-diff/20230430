# Comparing `tmp/portage-3.0.46.tar.gz` & `tmp/portage-3.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portage-3.0.46.tar", last modified: Fri Apr  7 09:56:10 2023, max compression
+gzip compressed data, was "portage-3.0.47.tar", last modified: Sun Apr 30 04:11:56 2023, max compression
```

## Comparing `portage-3.0.46.tar` & `portage-3.0.47.tar`

### file list

```diff
@@ -1,941 +1,942 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:35.927469 portage-3.0.46/.portage_not_installed
--rw-r--r--   0 root         (0) root         (0)     6944 2023-03-21 03:50:18.057424 portage-3.0.46/DEVELOPING
--rw-r--r--   0 root         (0) root         (0)    18092 2021-11-12 08:15:35.927469 portage-3.0.46/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4474 2023-04-07 09:56:10.598322 portage-3.0.46/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1864 2021-11-12 08:15:35.927469 portage-3.0.46/TEST-NOTES
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.571655 portage-3.0.46/bin/
--rwxr-xr-x   0 root         (0) root         (0)     3262 2023-03-21 23:52:40.754842 portage-3.0.46/bin/archive-conf
--rwxr-xr-x   0 root         (0) root         (0)     1443 2023-03-20 03:14:35.108827 portage-3.0.46/bin/bashrc-functions.sh
--rwxr-xr-x   0 root         (0) root         (0)     4457 2023-03-21 23:52:40.598174 portage-3.0.46/bin/binhost-snapshot
--rwxr-xr-x   0 root         (0) root         (0)       51 2021-11-12 08:15:35.934136 portage-3.0.46/bin/cgroup-release-agent
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.934136 portage-3.0.46/bin/chmod-lite -> ebuild-pyhelper
--rwxr-xr-x   0 root         (0) root         (0)      951 2023-03-21 03:35:23.553538 portage-3.0.46/bin/chmod-lite.py
--rwxr-xr-x   0 root         (0) root         (0)     5891 2023-03-21 03:35:23.553538 portage-3.0.46/bin/chpathtool.py
--rwxr-xr-x   0 root         (0) root         (0)     1421 2023-03-21 03:35:23.553538 portage-3.0.46/bin/clean_locks
--rwxr-xr-x   0 root         (0) root         (0)    19929 2023-03-21 23:52:40.598174 portage-3.0.46/bin/dispatch-conf
--rwxr-xr-x   0 root         (0) root         (0)     8895 2023-03-21 03:35:23.556871 portage-3.0.46/bin/dohtml.py
--rwxr-xr-x   0 root         (0) root         (0)    20007 2023-03-21 03:35:23.550205 portage-3.0.46/bin/doins.py
--rwxr-xr-x   0 root         (0) root         (0)     6078 2023-03-21 03:35:23.550205 portage-3.0.46/bin/eapi.sh
--rwxr-xr-x   0 root         (0) root         (0)     4310 2023-03-20 03:14:35.108827 portage-3.0.46/bin/eapi7-ver-funcs.sh
--rwxr-xr-x   0 root         (0) root         (0)    15468 2023-03-21 23:52:40.598174 portage-3.0.46/bin/ebuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.571655 portage-3.0.46/bin/ebuild-helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.571655 portage-3.0.46/bin/ebuild-helpers/bsd/
--rwxr-xr-x   0 root         (0) root         (0)      639 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/bsd/sed
--rwxr-xr-x   0 root         (0) root         (0)      200 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/die
--rwxr-xr-x   0 root         (0) root         (0)     1052 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/dobin
--rwxr-xr-x   0 root         (0) root         (0)      515 2022-09-10 09:45:01.063717 portage-3.0.46/bin/ebuild-helpers/doconfd
--rwxr-xr-x   0 root         (0) root         (0)      359 2022-09-10 09:45:01.057050 portage-3.0.46/bin/ebuild-helpers/dodir
--rwxr-xr-x   0 root         (0) root         (0)      888 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/dodoc
--rwxr-xr-x   0 root         (0) root         (0)      513 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/doenvd
--rwxr-xr-x   0 root         (0) root         (0)      955 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/doexe
--rwxr-xr-x   0 root         (0) root         (0)      531 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/dohard
--rwxr-xr-x   0 root         (0) root         (0)      632 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/doheader
--rwxr-xr-x   0 root         (0) root         (0)      782 2022-09-10 09:45:01.063717 portage-3.0.46/bin/ebuild-helpers/dohtml
--rwxr-xr-x   0 root         (0) root         (0)      722 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/doinfo
--rwxr-xr-x   0 root         (0) root         (0)      485 2022-09-10 09:45:01.063717 portage-3.0.46/bin/ebuild-helpers/doinitd
--rwxr-xr-x   0 root         (0) root         (0)     3034 2022-09-10 09:45:01.057050 portage-3.0.46/bin/ebuild-helpers/doins
--rwxr-xr-x   0 root         (0) root         (0)     1441 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/dolib
--rwxr-xr-x   0 root         (0) root         (0)      189 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/dolib.a
--rwxr-xr-x   0 root         (0) root         (0)      189 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/dolib.so
--rwxr-xr-x   0 root         (0) root         (0)     1553 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/doman
--rwxr-xr-x   0 root         (0) root         (0)     1219 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/domo
--rwxr-xr-x   0 root         (0) root         (0)     1056 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/dosbin
--rwxr-xr-x   0 root         (0) root         (0)      818 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/dosed
--rwxr-xr-x   0 root         (0) root         (0)     2366 2022-09-10 09:45:01.063717 portage-3.0.46/bin/ebuild-helpers/dosym
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.46/bin/ebuild-helpers/eerror -> elog
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.46/bin/ebuild-helpers/einfo -> elog
--rwxr-xr-x   0 root         (0) root         (0)      204 2022-09-10 09:45:01.053717 portage-3.0.46/bin/ebuild-helpers/elog
--rwxr-xr-x   0 root         (0) root         (0)      894 2022-09-10 09:45:01.053717 portage-3.0.46/bin/ebuild-helpers/emake
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.46/bin/ebuild-helpers/eqawarn -> elog
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.46/bin/ebuild-helpers/ewarn -> elog
--rwxr-xr-x   0 root         (0) root         (0)      792 2022-09-10 09:45:01.057050 portage-3.0.46/bin/ebuild-helpers/fowners
--rwxr-xr-x   0 root         (0) root         (0)      850 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/fperms
--rwxr-xr-x   0 root         (0) root         (0)      490 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/keepdir
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newbin -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newconfd -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newdoc -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newenvd -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newexe -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newheader -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newinitd -> newins
--rwxr-xr-x   0 root         (0) root         (0)     1201 2023-02-03 18:03:13.730194 portage-3.0.46/bin/ebuild-helpers/newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newlib.a -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newlib.so -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newman -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/newsbin -> newins
--rwxr-xr-x   0 root         (0) root         (0)      359 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/nonfatal
--rwxr-xr-x   0 root         (0) root         (0)      739 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/portageq
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/prepall
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.46/bin/ebuild-helpers/prepalldocs
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.46/bin/ebuild-helpers/prepallinfo
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.46/bin/ebuild-helpers/prepallman
--rwxr-xr-x   0 root         (0) root         (0)      383 2022-09-10 09:45:01.057050 portage-3.0.46/bin/ebuild-helpers/prepallstrip
--rwxr-xr-x   0 root         (0) root         (0)      843 2023-04-07 09:45:46.551215 portage-3.0.46/bin/ebuild-helpers/prepinfo
--rwxr-xr-x   0 root         (0) root         (0)      364 2023-04-07 09:45:46.551215 portage-3.0.46/bin/ebuild-helpers/prepman
--rwxr-xr-x   0 root         (0) root         (0)      375 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/prepstrip
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.571655 portage-3.0.46/bin/ebuild-helpers/unprivileged/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-helpers/unprivileged/chgrp -> chown
--rwxr-xr-x   0 root         (0) root         (0)     1178 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/unprivileged/chown
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.571655 portage-3.0.46/bin/ebuild-helpers/xattr/
--rwxr-xr-x   0 root         (0) root         (0)     1369 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ebuild-helpers/xattr/install
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.46/bin/ebuild-ipc -> ebuild-pyhelper
--rwxr-xr-x   0 root         (0) root         (0)    10684 2023-03-21 23:52:40.598174 portage-3.0.46/bin/ebuild-ipc.py
--rwxr-xr-x   0 root         (0) root         (0)      616 2022-09-10 09:45:01.057050 portage-3.0.46/bin/ebuild-pyhelper
--rwxr-xr-x   0 root         (0) root         (0)    26114 2023-03-21 03:35:23.556871 portage-3.0.46/bin/ebuild.sh
--rwxr-xr-x   0 root         (0) root         (0)     6481 2022-12-24 02:35:49.845990 portage-3.0.46/bin/ecompress
--rwxr-xr-x   0 root         (0) root         (0)     1746 2022-09-10 09:45:01.060384 portage-3.0.46/bin/ecompress-file
--rwxr-xr-x   0 root         (0) root         (0)    53990 2023-03-21 23:52:40.598174 portage-3.0.46/bin/egencache
--rwxr-xr-x   0 root         (0) root         (0)     1857 2023-03-21 03:35:23.556871 portage-3.0.46/bin/emaint
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-03-21 23:52:40.598174 portage-3.0.46/bin/emerge
--rwxr-xr-x   0 root         (0) root         (0)    15950 2022-09-10 09:45:01.063717 portage-3.0.46/bin/emerge-webrsync
--rwxr-xr-x   0 root         (0) root         (0)      634 2022-09-10 09:45:01.053717 portage-3.0.46/bin/emirrordist
--rwxr-xr-x   0 root         (0) root         (0)     1048 2023-03-21 03:35:23.556871 portage-3.0.46/bin/env-update
--rwxr-xr-x   0 root         (0) root         (0)    17296 2023-03-21 03:35:23.556871 portage-3.0.46/bin/estrip
--rwxr-xr-x   0 root         (0) root         (0)    23454 2023-03-21 03:50:18.057424 portage-3.0.46/bin/etc-update
--rwxr-xr-x   0 root         (0) root         (0)     6045 2023-03-21 03:35:23.556871 portage-3.0.46/bin/filter-bash-environment.py
--rwxr-xr-x   0 root         (0) root         (0)     1601 2023-03-21 03:35:23.556871 portage-3.0.46/bin/fixpackages
--rwxr-xr-x   0 root         (0) root         (0)    15636 2023-03-21 23:52:40.601508 portage-3.0.46/bin/glsa-check
--rwxr-xr-x   0 root         (0) root         (0)     2166 2023-03-21 03:35:23.556871 portage-3.0.46/bin/gpkg-helper.py
--rwxr-xr-x   0 root         (0) root         (0)     2476 2022-12-24 02:35:49.845990 portage-3.0.46/bin/gpkg-sign
--rwxr-xr-x   0 root         (0) root         (0)     2918 2023-03-20 03:14:35.108827 portage-3.0.46/bin/helper-functions.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/bin/install-qa-check.d/
--rwxr-xr-x   0 root         (0) root         (0)      444 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/05double-D
--rwxr-xr-x   0 root         (0) root         (0)     4302 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/05prefix
--rwxr-xr-x   0 root         (0) root         (0)     5559 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/10executable-issues
--rwxr-xr-x   0 root         (0) root         (0)     3591 2023-03-21 03:35:23.550205 portage-3.0.46/bin/install-qa-check.d/10ignored-flags
--rwxr-xr-x   0 root         (0) root         (0)      406 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/20deprecated-directories
--rwxr-xr-x   0 root         (0) root         (0)      835 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/20runtime-directories
--rwxr-xr-x   0 root         (0) root         (0)     3306 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/60bash-completion
--rwxr-xr-x   0 root         (0) root         (0)     1443 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/60openrc
--rwxr-xr-x   0 root         (0) root         (0)     5508 2023-03-21 03:35:23.550205 portage-3.0.46/bin/install-qa-check.d/60pkgconfig
--rwxr-xr-x   0 root         (0) root         (0)      668 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/60pngfix
--rwxr-xr-x   0 root         (0) root         (0)      687 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/60systemd
--rwxr-xr-x   0 root         (0) root         (0)      442 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/60udev
--rwxr-xr-x   0 root         (0) root         (0)     5556 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/80libraries
--rwxr-xr-x   0 root         (0) root         (0)     1417 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/80multilib-strict
--rwxr-xr-x   0 root         (0) root         (0)     1918 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/90bad-bin-group-write
--rwxr-xr-x   0 root         (0) root         (0)     1566 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/90bad-bin-owner
--rwxr-xr-x   0 root         (0) root         (0)      654 2023-03-20 03:14:35.108827 portage-3.0.46/bin/install-qa-check.d/90cmake-warnings
--rwxr-xr-x   0 root         (0) root         (0)     3333 2023-03-21 03:50:18.057424 portage-3.0.46/bin/install-qa-check.d/90config-impl-decl
--rwxr-xr-x   0 root         (0) root         (0)     7866 2023-03-21 03:35:23.550205 portage-3.0.46/bin/install-qa-check.d/90gcc-warnings
--rwxr-xr-x   0 root         (0) root         (0)     1042 2023-03-20 03:14:35.112161 portage-3.0.46/bin/install-qa-check.d/90world-writable
--rwxr-xr-x   0 root         (0) root         (0)     1518 2023-03-20 03:14:35.112161 portage-3.0.46/bin/install-qa-check.d/95empty-dirs
--rwxr-xr-x   0 root         (0) root         (0)     6314 2023-03-21 23:52:40.601508 portage-3.0.46/bin/install.py
--rwxr-xr-x   0 root         (0) root         (0)    18552 2023-03-21 03:50:18.057424 portage-3.0.46/bin/isolated-functions.sh
--rwxr-xr-x   0 root         (0) root         (0)      903 2023-03-21 03:35:23.553538 portage-3.0.46/bin/lock-helper.py
--rwxr-xr-x   0 root         (0) root         (0)    20244 2023-04-07 09:45:46.551215 portage-3.0.46/bin/misc-functions.sh
--rwxr-xr-x   0 root         (0) root         (0)    34584 2023-03-20 03:14:35.112161 portage-3.0.46/bin/phase-functions.sh
--rwxr-xr-x   0 root         (0) root         (0)    33794 2023-03-21 03:35:23.553538 portage-3.0.46/bin/phase-helpers.sh
--rwxr-xr-x   0 root         (0) root         (0)     5723 2023-03-21 03:35:23.556871 portage-3.0.46/bin/pid-ns-init
--rwxr-xr-x   0 root         (0) root         (0)    51197 2023-03-21 23:52:40.601508 portage-3.0.46/bin/portageq
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/bin/postinst-qa-check.d/
--rwxr-xr-x   0 root         (0) root         (0)     5236 2023-03-20 03:14:35.112161 portage-3.0.46/bin/postinst-qa-check.d/50xdg-utils
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/bin/preinst-qa-check.d/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.947469 portage-3.0.46/bin/preinst-qa-check.d/50xdg-utils -> ../postinst-qa-check.d/50xdg-utils
--rwxr-xr-x   0 root         (0) root         (0)    16731 2023-03-21 23:52:40.601508 portage-3.0.46/bin/quickpkg
--rwxr-xr-x   0 root         (0) root         (0)     4992 2023-03-21 03:35:23.556871 portage-3.0.46/bin/regenworld
--rwxr-xr-x   0 root         (0) root         (0)     4533 2023-03-21 03:50:18.057424 portage-3.0.46/bin/save-ebuild-env.sh
--rwxr-xr-x   0 root         (0) root         (0)     1339 2022-09-10 09:45:01.060384 portage-3.0.46/bin/shelve-utils
--rwxr-xr-x   0 root         (0) root         (0)     8140 2023-03-21 03:35:23.556871 portage-3.0.46/bin/socks5-server.py
--rwxr-xr-x   0 root         (0) root         (0)     4784 2023-03-21 23:52:40.601508 portage-3.0.46/bin/xattr-helper.py
--rwxr-xr-x   0 root         (0) root         (0)     1825 2023-03-21 03:35:23.550205 portage-3.0.46/bin/xpak-helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/cnf/
--rw-r--r--   0 root         (0) root         (0)     1718 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.alpha.diff
--rw-r--r--   0 root         (0) root         (0)     2319 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.amd64-fbsd.diff
--rw-r--r--   0 root         (0) root         (0)     2309 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.amd64.diff
--rw-r--r--   0 root         (0) root         (0)     1592 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.arm.diff
--rw-r--r--   0 root         (0) root         (0)     1580 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.arm64.diff
--rw-r--r--   0 root         (0) root         (0)     2465 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.hppa.diff
--rw-r--r--   0 root         (0) root         (0)      663 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.ia64.diff
--rw-r--r--   0 root         (0) root         (0)     2192 2023-03-21 03:35:23.550205 portage-3.0.46/cnf/make.conf.example.loong.diff
--rw-r--r--   0 root         (0) root         (0)      900 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.m68k.diff
--rw-r--r--   0 root         (0) root         (0)     1383 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.mips.diff
--rw-r--r--   0 root         (0) root         (0)     3541 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.ppc.diff
--rw-r--r--   0 root         (0) root         (0)     2361 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.ppc64.diff
--rw-r--r--   0 root         (0) root         (0)     2332 2022-09-10 09:44:56.963689 portage-3.0.46/cnf/make.conf.example.riscv.diff
--rw-r--r--   0 root         (0) root         (0)      656 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.s390.diff
--rw-r--r--   0 root         (0) root         (0)     1257 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.sh.diff
--rw-r--r--   0 root         (0) root         (0)      728 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.sparc-fbsd.diff
--rw-r--r--   0 root         (0) root         (0)     2129 2021-12-09 09:19:33.760140 portage-3.0.46/cnf/make.conf.example.sparc.diff
--rw-r--r--   0 root         (0) root         (0)     2507 2021-12-09 09:19:33.763473 portage-3.0.46/cnf/make.conf.example.x86-fbsd.diff
--rw-r--r--   0 root         (0) root         (0)     3759 2021-12-09 09:19:33.763473 portage-3.0.46/cnf/make.conf.example.x86.diff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/doc/api/
--rw-r--r--   0 root         (0) root         (0)     1141 2021-11-12 08:15:35.954135 portage-3.0.46/doc/api/Makefile
--rw-r--r--   0 root         (0) root         (0)     2372 2023-03-21 03:35:23.550205 portage-3.0.46/doc/api/conf.py
--rw-r--r--   0 root         (0) root         (0)      217 2021-11-12 08:15:35.954135 portage-3.0.46/doc/api/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/doc/config/
--rw-r--r--   0 root         (0) root         (0)     1900 2021-11-12 08:15:35.954135 portage-3.0.46/doc/config/bashrc.docbook
--rw-r--r--   0 root         (0) root         (0)    26214 2021-11-12 08:15:35.954135 portage-3.0.46/doc/config/sets.docbook
--rw-r--r--   0 root         (0) root         (0)       85 2021-11-12 08:15:35.954135 portage-3.0.46/doc/config.docbook
--rw-r--r--   0 root         (0) root         (0)      257 2021-11-12 08:15:35.954135 portage-3.0.46/doc/custom.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/doc/dependency_resolution/
--rw-r--r--   0 root         (0) root         (0)     3281 2021-11-12 08:15:35.957468 portage-3.0.46/doc/dependency_resolution/decision_making.docbook
--rw-r--r--   0 root         (0) root         (0)     4154 2021-11-12 08:15:35.957468 portage-3.0.46/doc/dependency_resolution/package_modeling.docbook
--rw-r--r--   0 root         (0) root         (0)     3451 2021-11-12 08:15:35.957468 portage-3.0.46/doc/dependency_resolution/task_scheduling.docbook
--rw-r--r--   0 root         (0) root         (0)      200 2021-11-12 08:15:35.954135 portage-3.0.46/doc/dependency_resolution.docbook
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/doc/package/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/doc/package/ebuild/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.574988 portage-3.0.46/doc/package/ebuild/eapi/
--rw-r--r--   0 root         (0) root         (0)      487 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/eapi/0.docbook
--rw-r--r--   0 root         (0) root         (0)     1598 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/eapi/1.docbook
--rw-r--r--   0 root         (0) root         (0)     8299 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/eapi/2.docbook
--rw-r--r--   0 root         (0) root         (0)     2938 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/eapi/3.docbook
--rw-r--r--   0 root         (0) root         (0)     3112 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/eapi/4-slot-abi.docbook
--rw-r--r--   0 root         (0) root         (0)    14690 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/eapi/4.docbook
--rw-r--r--   0 root         (0) root         (0)     8044 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/eapi/5.docbook
--rw-r--r--   0 root         (0) root         (0)     1725 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/helper_functions.docbook
--rw-r--r--   0 root         (0) root         (0)     2780 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package/ebuild/phases.docbook
--rw-r--r--   0 root         (0) root         (0)      364 2022-09-10 09:45:01.060384 portage-3.0.46/doc/package/ebuild.docbook
--rw-r--r--   0 root         (0) root         (0)       76 2021-11-12 08:15:35.957468 portage-3.0.46/doc/package.docbook
--rw-r--r--   0 root         (0) root         (0)     2194 2022-09-10 09:45:01.060384 portage-3.0.46/doc/portage.docbook
--rw-r--r--   0 root         (0) root         (0)    19579 2021-11-12 08:15:35.960802 portage-3.0.46/doc/qa.docbook
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.561655 portage-3.0.46/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.578322 portage-3.0.46/lib/_emerge/
--rw-r--r--   0 root         (0) root         (0)      816 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/AbstractDepPriority.py
--rw-r--r--   0 root         (0) root         (0)    18460 2023-03-21 03:50:18.057424 portage-3.0.46/lib/_emerge/AbstractEbuildProcess.py
--rw-r--r--   0 root         (0) root         (0)     3723 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/AbstractPollTask.py
--rw-r--r--   0 root         (0) root         (0)    10471 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/AsynchronousLock.py
--rw-r--r--   0 root         (0) root         (0)     7090 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/AsynchronousTask.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/AtomArg.py
--rw-r--r--   0 root         (0) root         (0)    21241 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/Binpkg.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/BinpkgEnvExtractor.py
--rw-r--r--   0 root         (0) root         (0)     5494 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/BinpkgExtractorAsync.py
--rw-r--r--   0 root         (0) root         (0)     9584 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/BinpkgFetcher.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/BinpkgPrefetcher.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/BinpkgVerifier.py
--rw-r--r--   0 root         (0) root         (0)      483 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/Blocker.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/BlockerCache.py
--rw-r--r--   0 root         (0) root         (0)     5325 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/BlockerDB.py
--rw-r--r--   0 root         (0) root         (0)      355 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/BlockerDepPriority.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/CompositeTask.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/DepPriority.py
--rw-r--r--   0 root         (0) root         (0)     1564 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/DepPriorityNormalRange.py
--rw-r--r--   0 root         (0) root         (0)     3647 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/DepPrioritySatisfiedRange.py
--rw-r--r--   0 root         (0) root         (0)      878 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/Dependency.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/DependencyArg.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/EbuildBinpkg.py
--rw-r--r--   0 root         (0) root         (0)    23204 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/EbuildBuild.py
--rw-r--r--   0 root         (0) root         (0)     5749 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/EbuildBuildDir.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/EbuildExecuter.py
--rw-r--r--   0 root         (0) root         (0)    14395 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/EbuildFetcher.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/EbuildFetchonly.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/EbuildIpcDaemon.py
--rw-r--r--   0 root         (0) root         (0)     3258 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/EbuildMerge.py
--rw-r--r--   0 root         (0) root         (0)     7597 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/EbuildMetadataPhase.py
--rw-r--r--   0 root         (0) root         (0)    22622 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/EbuildPhase.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/EbuildProcess.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/EbuildSpawnProcess.py
--rw-r--r--   0 root         (0) root         (0)    12786 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/FakeVartree.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/FifoIpcDaemon.py
--rw-r--r--   0 root         (0) root         (0)     9113 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/JobStatusDisplay.py
--rw-r--r--   0 root         (0) root         (0)     4823 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/MergeListItem.py
--rw-r--r--   0 root         (0) root         (0)     6121 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/MetadataRegen.py
--rw-r--r--   0 root         (0) root         (0)     2424 2022-09-10 09:45:01.063717 portage-3.0.46/lib/_emerge/MiscFunctionsProcess.py
--rw-r--r--   0 root         (0) root         (0)    31019 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/Package.py
--rw-r--r--   0 root         (0) root         (0)      735 2022-09-10 09:44:56.967023 portage-3.0.46/lib/_emerge/PackageArg.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/PackageMerge.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/PackagePhase.py
--rw-r--r--   0 root         (0) root         (0)     5870 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/PackageUninstall.py
--rw-r--r--   0 root         (0) root         (0)     4651 2022-09-10 09:44:56.967023 portage-3.0.46/lib/_emerge/PackageVirtualDbapi.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/PipeReader.py
--rw-r--r--   0 root         (0) root         (0)     6630 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/PollScheduler.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-09-10 09:44:56.967023 portage-3.0.46/lib/_emerge/ProgressHandler.py
--rw-r--r--   0 root         (0) root         (0)     1227 2022-09-10 09:44:56.967023 portage-3.0.46/lib/_emerge/RootConfig.py
--rw-r--r--   0 root         (0) root         (0)    85615 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/Scheduler.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/SequentialTaskQueue.py
--rw-r--r--   0 root         (0) root         (0)      421 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/SetArg.py
--rw-r--r--   0 root         (0) root         (0)    10190 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/SpawnProcess.py
--rw-r--r--   0 root         (0) root         (0)     3167 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/SubProcess.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/Task.py
--rw-r--r--   0 root         (0) root         (0)     1538 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/TaskSequence.py
--rw-r--r--   0 root         (0) root         (0)      455 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/UninstallFailure.py
--rw-r--r--   0 root         (0) root         (0)     1326 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/UnmergeDepPriority.py
--rw-r--r--   0 root         (0) root         (0)     3555 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/UseFlagDisplay.py
--rw-r--r--   0 root         (0) root         (0)     2995 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/UserQuery.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:35.977468 portage-3.0.46/lib/_emerge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1165 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/_find_deep_system_runtime_deps.py
--rw-r--r--   0 root         (0) root         (0)      442 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/_flush_elog_mod_echo.py
--rw-r--r--   0 root         (0) root         (0)   149373 2023-03-21 03:50:18.060757 portage-3.0.46/lib/_emerge/actions.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/chk_updated_cfg_files.py
--rw-r--r--   0 root         (0) root         (0)      498 2022-09-10 09:44:56.963689 portage-3.0.46/lib/_emerge/clear_caches.py
--rw-r--r--   0 root         (0) root         (0)      586 2023-02-03 18:03:13.733528 portage-3.0.46/lib/_emerge/countdown.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/create_depgraph_params.py
--rw-r--r--   0 root         (0) root         (0)     5191 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/create_world_atom.py
--rw-r--r--   0 root         (0) root         (0)   499558 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/depgraph.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/emergelog.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/getloadavg.py
--rw-r--r--   0 root         (0) root         (0)     3425 2022-09-10 09:44:56.970356 portage-3.0.46/lib/_emerge/help.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/is_valid_package_atom.py
--rw-r--r--   0 root         (0) root         (0)    42164 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/main.py
--rw-r--r--   0 root         (0) root         (0)     5614 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/post_emerge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.578322 portage-3.0.46/lib/_emerge/resolver/
--rw-r--r--   0 root         (0) root         (0)     3198 2022-09-10 09:44:56.970356 portage-3.0.46/lib/_emerge/resolver/DbapiProvidesIndex.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:35.980801 portage-3.0.46/lib/_emerge/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11328 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/resolver/backtracking.py
--rw-r--r--   0 root         (0) root         (0)    11932 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/resolver/circular_dependency.py
--rw-r--r--   0 root         (0) root         (0)    39548 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/resolver/output.py
--rw-r--r--   0 root         (0) root         (0)    20756 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/resolver/output_helpers.py
--rw-r--r--   0 root         (0) root         (0)    15636 2023-03-21 03:35:23.550205 portage-3.0.46/lib/_emerge/resolver/package_tracker.py
--rw-r--r--   0 root         (0) root         (0)    59893 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/resolver/slot_collision.py
--rw-r--r--   0 root         (0) root         (0)    20976 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/search.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/show_invalid_depstring_notice.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-03-21 03:35:23.553538 portage-3.0.46/lib/_emerge/stdout_spinner.py
--rw-r--r--   0 root         (0) root         (0)    26564 2023-03-21 03:35:23.556871 portage-3.0.46/lib/_emerge/unmerge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.578322 portage-3.0.46/lib/portage/
--rw-r--r--   0 root         (0) root         (0)    25908 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.578322 portage-3.0.46/lib/portage/_compat_upgrade/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.007468 portage-3.0.46/lib/portage/_compat_upgrade/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/_compat_upgrade/binpkg_compression.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_compat_upgrade/binpkg_multi_instance.py
--rw-r--r--   0 root         (0) root         (0)     4288 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_compat_upgrade/default_locations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.578322 portage-3.0.46/lib/portage/_emirrordist/
--rw-r--r--   0 root         (0) root         (0)     5376 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_emirrordist/Config.py
--rw-r--r--   0 root         (0) root         (0)     7223 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_emirrordist/ContentDB.py
--rw-r--r--   0 root         (0) root         (0)     4631 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_emirrordist/DeletionIterator.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_emirrordist/DeletionTask.py
--rw-r--r--   0 root         (0) root         (0)    11176 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_emirrordist/FetchIterator.py
--rw-r--r--   0 root         (0) root         (0)    25443 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_emirrordist/FetchTask.py
--rw-r--r--   0 root         (0) root         (0)     9145 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_emirrordist/MirrorDistTask.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.007468 portage-3.0.46/lib/portage/_emirrordist/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16082 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/_emirrordist/main.py
--rw-r--r--   0 root         (0) root         (0)    10222 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_global_updates.py
--rw-r--r--   0 root         (0) root         (0)     2550 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/_legacy_globals.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_selinux.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.578322 portage-3.0.46/lib/portage/_sets/
--rw-r--r--   0 root         (0) root         (0)     1719 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_sets/ProfilePackageSet.py
--rw-r--r--   0 root         (0) root         (0)    14268 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/_sets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8205 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_sets/base.py
--rw-r--r--   0 root         (0) root         (0)    22035 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_sets/dbapi.py
--rw-r--r--   0 root         (0) root         (0)    15573 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_sets/files.py
--rw-r--r--   0 root         (0) root         (0)     3603 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/_sets/libs.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_sets/profiles.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_sets/security.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/_sets/shell.py
--rw-r--r--   0 root         (0) root         (0)     2576 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/binpkg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.578322 portage-3.0.46/lib/portage/binrepo/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.014134 portage-3.0.46/lib/portage/binrepo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4554 2023-02-03 18:03:13.730194 portage-3.0.46/lib/portage/binrepo/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/cache/
--rw-r--r--   0 root         (0) root         (0)      101 2021-11-12 08:15:36.014134 portage-3.0.46/lib/portage/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3167 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/cache/anydbm.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/cache/cache_errors.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/cache/ebuild_xattr.py
--rw-r--r--   0 root         (0) root         (0)     5286 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/cache/flat_hash.py
--rw-r--r--   0 root         (0) root         (0)     3197 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/cache/fs_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/cache/index/
--rw-r--r--   0 root         (0) root         (0)      562 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/cache/index/IndexStreamIterator.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.017468 portage-3.0.46/lib/portage/cache/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/cache/index/pkg_desc_index.py
--rw-r--r--   0 root         (0) root         (0)    11957 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/cache/mappings.py
--rw-r--r--   0 root         (0) root         (0)     5844 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/cache/metadata.py
--rw-r--r--   0 root         (0) root         (0)    11820 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/cache/sql_template.py
--rw-r--r--   0 root         (0) root         (0)    13390 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/cache/sqlite.py
--rw-r--r--   0 root         (0) root         (0)    13272 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/cache/template.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/cache/volatile.py
--rw-r--r--   0 root         (0) root         (0)    16566 2023-04-07 09:45:44.114534 portage-3.0.46/lib/portage/checksum.py
--rw-r--r--   0 root         (0) root         (0)     8879 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/const.py
--rw-r--r--   0 root         (0) root         (0)    11470 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/cvstree.py
--rw-r--r--   0 root         (0) root         (0)    11537 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/dbapi/
--rw-r--r--   0 root         (0) root         (0)      643 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/dbapi/DummyTree.py
--rw-r--r--   0 root         (0) root         (0)     5690 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/dbapi/IndexedPortdb.py
--rw-r--r--   0 root         (0) root         (0)     3743 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/dbapi/IndexedVardb.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/dbapi/_ContentsCaseSensitivityManager.py
--rw-r--r--   0 root         (0) root         (0)    10128 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/dbapi/_MergeProcess.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/dbapi/_SyncfsProcess.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/dbapi/_VdbMetadataDelta.py
--rw-r--r--   0 root         (0) root         (0)    16769 2023-04-07 09:45:48.221225 portage-3.0.46/lib/portage/dbapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2545 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/dbapi/_expand_new_virt.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/dbapi/_similar_name_search.py
--rw-r--r--   0 root         (0) root         (0)    90388 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/dbapi/bintree.py
--rw-r--r--   0 root         (0) root         (0)     4184 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/dbapi/cpv_expand.py
--rw-r--r--   0 root         (0) root         (0)     1889 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/dbapi/dep_expand.py
--rw-r--r--   0 root         (0) root         (0)    64264 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/dbapi/porttree.py
--rw-r--r--   0 root         (0) root         (0)   252193 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/dbapi/vartree.py
--rw-r--r--   0 root         (0) root         (0)     7587 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/dbapi/virtual.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/dep/
--rw-r--r--   0 root         (0) root         (0)   107693 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/dep/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/dep/_dnf.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/dep/_slot_operator.py
--rw-r--r--   0 root         (0) root         (0)    42498 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/dep/dep_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/dep/soname/
--rw-r--r--   0 root         (0) root         (0)     1925 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/dep/soname/SonameAtom.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.030801 portage-3.0.46/lib/portage/dep/soname/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5080 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/dep/soname/multilib_category.py
--rw-r--r--   0 root         (0) root         (0)     1491 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/dep/soname/parse.py
--rw-r--r--   0 root         (0) root         (0)    14093 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/dispatch_conf.py
--rw-r--r--   0 root         (0) root         (0)     8092 2023-01-10 15:35:29.386865 portage-3.0.46/lib/portage/eapi.py
--rw-r--r--   0 root         (0) root         (0)     6757 2022-09-10 09:45:01.057050 portage-3.0.46/lib/portage/eclass_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/elog/
--rw-r--r--   0 root         (0) root         (0)     6879 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/elog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      613 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/elog/filtering.py
--rw-r--r--   0 root         (0) root         (0)     6065 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/elog/messages.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-02-03 18:03:13.736861 portage-3.0.46/lib/portage/elog/mod_custom.py
--rw-r--r--   0 root         (0) root         (0)     2204 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/elog/mod_echo.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/elog/mod_mail.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/elog/mod_mail_summary.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/elog/mod_save.py
--rw-r--r--   0 root         (0) root         (0)     3580 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/elog/mod_save_summary.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/elog/mod_syslog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/
--rw-r--r--   0 root         (0) root         (0)      163 2021-11-12 08:15:36.037467 portage-3.0.46/lib/portage/emaint/__init__.py
--rw-r--r--   0 root         (0) root         (0)      762 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/defaults.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/emaint/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/
--rw-r--r--   0 root         (0) root         (0)      173 2021-11-12 08:15:36.037467 portage-3.0.46/lib/portage/emaint/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/binhost/
--rw-r--r--   0 root         (0) root         (0)      524 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/modules/binhost/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6358 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/emaint/modules/binhost/binhost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/config/
--rw-r--r--   0 root         (0) root         (0)      534 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/modules/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/emaint/modules/config/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/logs/
--rw-r--r--   0 root         (0) root         (0)     1629 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/modules/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/emaint/modules/logs/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/merges/
--rw-r--r--   0 root         (0) root         (0)     1417 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/modules/merges/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9834 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/emaint/modules/merges/merges.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/move/
--rw-r--r--   0 root         (0) root         (0)      851 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/modules/move/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7693 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/emaint/modules/move/move.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/resume/
--rw-r--r--   0 root         (0) root         (0)      566 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/modules/resume/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/emaint/modules/resume/resume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/sync/
--rw-r--r--   0 root         (0) root         (0)     2145 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/modules/sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18469 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/emaint/modules/sync/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/emaint/modules/world/
--rw-r--r--   0 root         (0) root         (0)      502 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/emaint/modules/world/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/emaint/modules/world/world.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/env/
--rw-r--r--   0 root         (0) root         (0)       52 2021-11-12 08:15:36.044134 portage-3.0.46/lib/portage/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/env/config.py
--rw-r--r--   0 root         (0) root         (0)    10311 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/env/loaders.py
--rw-r--r--   0 root         (0) root         (0)      578 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/env/validators.py
--rw-r--r--   0 root         (0) root         (0)     6616 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/exception.py
--rw-r--r--   0 root         (0) root         (0)    31465 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/getbinpkg.py
--rw-r--r--   0 root         (0) root         (0)    31099 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/glsa.py
--rw-r--r--   0 root         (0) root         (0)     3637 2022-09-10 09:45:01.060384 portage-3.0.46/lib/portage/gpg.py
--rw-r--r--   0 root         (0) root         (0)    80663 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/gpkg.py
--rw-r--r--   0 root         (0) root         (0)     1550 2022-09-10 09:45:01.060384 portage-3.0.46/lib/portage/localization.py
--rw-r--r--   0 root         (0) root         (0)    28153 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/locks.py
--rw-r--r--   0 root         (0) root         (0)     6187 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/mail.py
--rw-r--r--   0 root         (0) root         (0)    31108 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/manifest.py
--rw-r--r--   0 root         (0) root         (0)     8221 2023-02-03 18:03:13.736861 portage-3.0.46/lib/portage/metadata.py
--rw-r--r--   0 root         (0) root         (0)     8568 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/module.py
--rw-r--r--   0 root         (0) root         (0)    18485 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/news.py
--rw-r--r--   0 root         (0) root         (0)    29784 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/package/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.047467 portage-3.0.46/lib/portage/package/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/package/ebuild/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.050800 portage-3.0.46/lib/portage/package/ebuild/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/package/ebuild/_config/
--rw-r--r--   0 root         (0) root         (0)    13005 2023-02-03 18:03:13.730194 portage-3.0.46/lib/portage/package/ebuild/_config/KeywordsManager.py
--rw-r--r--   0 root         (0) root         (0)     9192 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/_config/LicenseManager.py
--rw-r--r--   0 root         (0) root         (0)    16684 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/_config/LocationsManager.py
--rw-r--r--   0 root         (0) root         (0)    13915 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/package/ebuild/_config/MaskManager.py
--rw-r--r--   0 root         (0) root         (0)    21565 2023-02-03 18:03:13.730194 portage-3.0.46/lib/portage/package/ebuild/_config/UseManager.py
--rw-r--r--   0 root         (0) root         (0)     8443 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/package/ebuild/_config/VirtualsManager.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.050800 portage-3.0.46/lib/portage/package/ebuild/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      770 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/package/ebuild/_config/env_var_validation.py
--rw-r--r--   0 root         (0) root         (0)     4694 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/package/ebuild/_config/features_set.py
--rw-r--r--   0 root         (0) root         (0)     2272 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/package/ebuild/_config/helper.py
--rw-r--r--   0 root         (0) root         (0)     9457 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/package/ebuild/_config/special_env_vars.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/package/ebuild/_ipc/
--rw-r--r--   0 root         (0) root         (0)      829 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/_ipc/ExitCommand.py
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/_ipc/IpcCommand.py
--rw-r--r--   0 root         (0) root         (0)     5193 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/package/ebuild/_ipc/QueryCommand.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.054134 portage-3.0.46/lib/portage/package/ebuild/_ipc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/_metadata_invalid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/package/ebuild/_parallel_manifest/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py
--rw-r--r--   0 root         (0) root         (0)     7859 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.057467 portage-3.0.46/lib/portage/package/ebuild/_parallel_manifest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4987 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/package/ebuild/_spawn_nofetch.py
--rw-r--r--   0 root         (0) root         (0)   133992 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/config.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/package/ebuild/deprecated_profile_check.py
--rw-r--r--   0 root         (0) root         (0)     6732 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/package/ebuild/digestcheck.py
--rw-r--r--   0 root         (0) root         (0)     9424 2023-03-21 03:35:23.550205 portage-3.0.46/lib/portage/package/ebuild/digestgen.py
--rw-r--r--   0 root         (0) root         (0)   111662 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/package/ebuild/doebuild.py
--rw-r--r--   0 root         (0) root         (0)    79658 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/package/ebuild/fetch.py
--rw-r--r--   0 root         (0) root         (0)     4689 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/package/ebuild/getmaskingreason.py
--rw-r--r--   0 root         (0) root         (0)     6556 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/package/ebuild/getmaskingstatus.py
--rw-r--r--   0 root         (0) root         (0)    19287 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/package/ebuild/prepare_build_dirs.py
--rw-r--r--   0 root         (0) root         (0)     1004 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/package/ebuild/profile_iuse.py
--rw-r--r--   0 root         (0) root         (0)    41702 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/process.py
--rw-r--r--   0 root         (0) root         (0)     1573 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.581655 portage-3.0.46/lib/portage/proxy/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.060800 portage-3.0.46/lib/portage/proxy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7832 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/proxy/lazyimport.py
--rw-r--r--   0 root         (0) root         (0)     2857 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/proxy/objectproxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/repository/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.064134 portage-3.0.46/lib/portage/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62136 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/repository/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/repository/storage/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.064134 portage-3.0.46/lib/portage/repository/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3951 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/repository/storage/hardlink_quarantine.py
--rw-r--r--   0 root         (0) root         (0)    10940 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/repository/storage/hardlink_rcu.py
--rw-r--r--   0 root         (0) root         (0)     1153 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/repository/storage/inplace.py
--rw-r--r--   0 root         (0) root         (0)     2675 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/repository/storage/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/sync/
--rw-r--r--   0 root         (0) root         (0)     1589 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3015 2023-02-03 18:03:13.733528 portage-3.0.46/lib/portage/sync/config_checks.py
--rw-r--r--   0 root         (0) root         (0)    14745 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/sync/controller.py
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/sync/getaddrinfo_validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/sync/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.067467 portage-3.0.46/lib/portage/sync/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/sync/modules/cvs/
--rw-r--r--   0 root         (0) root         (0)     1650 2023-02-03 18:03:13.733528 portage-3.0.46/lib/portage/sync/modules/cvs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-02-03 18:03:13.730194 portage-3.0.46/lib/portage/sync/modules/cvs/cvs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/sync/modules/git/
--rw-r--r--   0 root         (0) root         (0)     2722 2023-02-03 18:03:13.730194 portage-3.0.46/lib/portage/sync/modules/git/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20049 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/sync/modules/git/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/sync/modules/mercurial/
--rw-r--r--   0 root         (0) root         (0)     1403 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/sync/modules/mercurial/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6125 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/sync/modules/mercurial/mercurial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/sync/modules/rsync/
--rw-r--r--   0 root         (0) root         (0)     1287 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/sync/modules/rsync/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33953 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/sync/modules/rsync/rsync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/sync/modules/svn/
--rw-r--r--   0 root         (0) root         (0)     1037 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/sync/modules/svn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2759 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/sync/modules/svn/svn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/sync/modules/webrsync/
--rw-r--r--   0 root         (0) root         (0)     1648 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/sync/modules/webrsync/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5092 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/sync/modules/webrsync/webrsync.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/sync/old_tree_timestamp.py
--rw-r--r--   0 root         (0) root         (0)    13139 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/sync/syncbase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/.gnupg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/.gnupg/openpgp-revocs.d/
--rw-r--r--   0 root         (0) root         (0)     1850 2022-09-10 09:45:01.063717 portage-3.0.46/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev
--rw-r--r--   0 root         (0) root         (0)     1852 2022-09-10 09:45:01.063717 portage-3.0.46/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/.gnupg/private-keys-v1.d/
--rw-r--r--   0 root         (0) root         (0)     2055 2022-09-10 09:45:01.057050 portage-3.0.46/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key
--rw-r--r--   0 root         (0) root         (0)     2055 2022-09-10 09:45:01.060384 portage-3.0.46/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key
--rw-r--r--   0 root         (0) root         (0)     2774 2022-09-10 09:45:01.060384 portage-3.0.46/lib/portage/tests/.gnupg/pubring.kbx
--rw-r--r--   0 root         (0) root         (0)     1360 2022-09-10 09:45:01.060384 portage-3.0.46/lib/portage/tests/.gnupg/trustdb.gpg
--rw-r--r--   0 root         (0) root         (0)    11871 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/bin/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.46/lib/portage/tests/bin/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.46/lib/portage/tests/bin/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2658 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/bin/setup_env.py
--rw-r--r--   0 root         (0) root         (0)      547 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/bin/test_dobin.py
--rw-r--r--   0 root         (0) root         (0)      565 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/bin/test_dodir.py
--rw-r--r--   0 root         (0) root         (0)    13013 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/bin/test_doins.py
--rw-r--r--   0 root         (0) root         (0)     9192 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/bin/test_eapi7_ver_funcs.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/bin/test_filter_bash_env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/dbapi/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.074133 portage-3.0.46/lib/portage/tests/dbapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.46/lib/portage/tests/dbapi/__test__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dbapi/test_auxdb.py
--rw-r--r--   0 root         (0) root         (0)     6521 2023-02-03 18:03:13.730194 portage-3.0.46/lib/portage/tests/dbapi/test_bintree.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/dbapi/test_fakedbapi.py
--rw-r--r--   0 root         (0) root         (0)     9409 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/dbapi/test_portdb_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/dep/
--rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.077467 portage-3.0.46/lib/portage/tests/dep/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.077467 portage-3.0.46/lib/portage/tests/dep/__test__.py
--rw-r--r--   0 root         (0) root         (0)    24520 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/dep/testAtom.py
--rw-r--r--   0 root         (0) root         (0)     9752 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/dep/testCheckRequiredUse.py
--rw-r--r--   0 root         (0) root         (0)      779 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/dep/testExtendedAtomDict.py
--rw-r--r--   0 root         (0) root         (0)     3769 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/dep/testExtractAffectingUSE.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/dep/testStandalone.py
--rw-r--r--   0 root         (0) root         (0)     4452 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/dep/test_best_match_to_list.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_dep_getcpv.py
--rw-r--r--   0 root         (0) root         (0)      988 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_dep_getrepo.py
--rw-r--r--   0 root         (0) root         (0)      934 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_dep_getslot.py
--rw-r--r--   0 root         (0) root         (0)     1402 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_dep_getusedeps.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_dnf_convert.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_get_operator.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_get_required_use_flags.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_isjustname.py
--rw-r--r--   0 root         (0) root         (0)    11660 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_isvalidatom.py
--rw-r--r--   0 root         (0) root         (0)    11132 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_match_from_list.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_overlap_dnf.py
--rw-r--r--   0 root         (0) root         (0)     2661 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_paren_reduce.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/dep/test_soname_atom_pickle.py
--rw-r--r--   0 root         (0) root         (0)    27656 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/dep/test_use_reduce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/ebuild/
--rw-r--r--   0 root         (0) root         (0)      107 2021-11-12 08:15:36.080800 portage-3.0.46/lib/portage/tests/ebuild/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.080800 portage-3.0.46/lib/portage/tests/ebuild/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/ebuild/test_array_fromfile_eof.py
--rw-r--r--   0 root         (0) root         (0)    14001 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/ebuild/test_config.py
--rw-r--r--   0 root         (0) root         (0)     5947 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py
--rw-r--r--   0 root         (0) root         (0)     5167 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/ebuild/test_doebuild_spawn.py
--rw-r--r--   0 root         (0) root         (0)    35283 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/ebuild/test_fetch.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/ebuild/test_ipc_daemon.py
--rw-r--r--   0 root         (0) root         (0)     5211 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/ebuild/test_shell_quote.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/ebuild/test_spawn.py
--rw-r--r--   0 root         (0) root         (0)     4479 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/ebuild/test_use_expand_incremental.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/emerge/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.080800 portage-3.0.46/lib/portage/tests/emerge/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.080800 portage-3.0.46/lib/portage/tests/emerge/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1877 2022-12-24 02:35:49.845990 portage-3.0.46/lib/portage/tests/emerge/test_actions.py
--rw-r--r--   0 root         (0) root         (0)    10290 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/emerge/test_config_protect.py
--rw-r--r--   0 root         (0) root         (0)     6335 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py
--rw-r--r--   0 root         (0) root         (0)     6615 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/emerge/test_emerge_slot_abi.py
--rw-r--r--   0 root         (0) root         (0)     1320 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/emerge/test_global_updates.py
--rw-r--r--   0 root         (0) root         (0)    26423 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/emerge/test_simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/env/
--rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/env/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/env/config/
--rw-r--r--   0 root         (0) root         (0)      176 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/env/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/env/config/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/env/config/test_PackageKeywordsFile.py
--rw-r--r--   0 root         (0) root         (0)      818 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/env/config/test_PackageMaskFile.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/env/config/test_PackageUseFile.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/env/config/test_PortageModulesFile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.584988 portage-3.0.46/lib/portage/tests/glsa/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/glsa/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/glsa/__test__.py
--rw-r--r--   0 root         (0) root         (0)     7173 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/glsa/test_security_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.588322 portage-3.0.46/lib/portage/tests/gpkg/
--rw-r--r--   0 root         (0) root         (0)      102 2022-09-10 09:45:01.057050 portage-3.0.46/lib/portage/tests/gpkg/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-10 09:45:01.057050 portage-3.0.46/lib/portage/tests/gpkg/__test__.py
--rw-r--r--   0 root         (0) root         (0)    13833 2022-09-20 03:21:13.396002 portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_checksum.py
--rw-r--r--   0 root         (0) root         (0)    15728 2022-09-20 03:21:13.396002 portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_gpg.py
--rw-r--r--   0 root         (0) root         (0)     1899 2022-09-20 03:21:13.396002 portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_metadata_update.py
--rw-r--r--   0 root         (0) root         (0)     5288 2022-09-20 03:21:13.396002 portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_metadata_url.py
--rw-r--r--   0 root         (0) root         (0)    14745 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_path.py
--rw-r--r--   0 root         (0) root         (0)     1868 2022-09-20 03:21:13.396002 portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_size.py
--rw-r--r--   0 root         (0) root         (0)     3305 2022-09-20 03:21:13.396002 portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.588322 portage-3.0.46/lib/portage/tests/lafilefixer/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/lafilefixer/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/lafilefixer/__test__.py
--rw-r--r--   0 root         (0) root         (0)     6338 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/lafilefixer/test_lafilefixer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.588322 portage-3.0.46/lib/portage/tests/lazyimport/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/lazyimport/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.46/lib/portage/tests/lazyimport/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py
--rw-r--r--   0 root         (0) root         (0)      596 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/lazyimport/test_preload_portage_submodules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.588322 portage-3.0.46/lib/portage/tests/lint/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.46/lib/portage/tests/lint/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.46/lib/portage/tests/lint/__test__.py
--rw-r--r--   0 root         (0) root         (0)      214 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/lint/metadata.py
--rw-r--r--   0 root         (0) root         (0)     2345 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/lint/test_bash_syntax.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/lint/test_compile_modules.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/lint/test_import_modules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.588322 portage-3.0.46/lib/portage/tests/locks/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.087467 portage-3.0.46/lib/portage/tests/locks/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.46/lib/portage/tests/locks/__test__.py
--rw-r--r--   0 root         (0) root         (0)     7850 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/locks/test_asynchronous_lock.py
--rw-r--r--   0 root         (0) root         (0)     2763 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/locks/test_lock_nonblock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.588322 portage-3.0.46/lib/portage/tests/news/
--rw-r--r--   0 root         (0) root         (0)      170 2021-11-12 08:15:36.087467 portage-3.0.46/lib/portage/tests/news/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.46/lib/portage/tests/news/__test__.py
--rw-r--r--   0 root         (0) root         (0)    14363 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/news/test_NewsItem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.588322 portage-3.0.46/lib/portage/tests/process/
--rw-r--r--   0 root         (0) root         (0)      107 2021-11-12 08:15:36.087467 portage-3.0.46/lib/portage/tests/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.46/lib/portage/tests/process/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2016 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/process/test_AsyncFunction.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/process/test_PipeLogger.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/process/test_PopenProcess.py
--rw-r--r--   0 root         (0) root         (0)     2366 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/process/test_PopenProcessBlockingIO.py
--rw-r--r--   0 root         (0) root         (0)     3737 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/process/test_poll.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/process/test_spawn_fail_e2big.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-03-21 03:50:18.060757 portage-3.0.46/lib/portage/tests/process/test_spawn_warn_large_env.py
--rw-r--r--   0 root         (0) root         (0)     1178 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/process/test_unshare_net.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/resolver/
--rw-r--r--   0 root         (0) root         (0)    42502 2023-03-21 03:50:18.064091 portage-3.0.46/lib/portage/tests/resolver/ResolverPlayground.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.46/lib/portage/tests/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.104133 portage-3.0.46/lib/portage/tests/resolver/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/resolver/binpkg_multi_instance/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.46/lib/portage/tests/resolver/binpkg_multi_instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.46/lib/portage/tests/resolver/binpkg_multi_instance/__test__.py
--rw-r--r--   0 root         (0) root         (0)     5585 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py
--rw-r--r--   0 root         (0) root         (0)     3747 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/resolver/soname/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/resolver/soname/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/resolver/soname/__test__.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_autounmask.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_depclean.py
--rw-r--r--   0 root         (0) root         (0)     8528 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_downgrade.py
--rw-r--r--   0 root         (0) root         (0)     3840 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_or_choices.py
--rw-r--r--   0 root         (0) root         (0)     3305 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_reinstall.py
--rw-r--r--   0 root         (0) root         (0)     3338 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_skip_update.py
--rw-r--r--   0 root         (0) root         (0)    12877 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_slot_conflict_update.py
--rw-r--r--   0 root         (0) root         (0)     2944 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_soname_provided.py
--rw-r--r--   0 root         (0) root         (0)     2778 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/soname/test_unsatisfiable.py
--rw-r--r--   0 root         (0) root         (0)     3354 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/soname/test_unsatisfied.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py
--rw-r--r--   0 root         (0) root         (0)    28432 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_autounmask.py
--rw-r--r--   0 root         (0) root         (0)     2732 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_autounmask_binpkg_use.py
--rw-r--r--   0 root         (0) root         (0)     2176 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_autounmask_keep_keywords.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_autounmask_multilib_use.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_autounmask_parent.py
--rw-r--r--   0 root         (0) root         (0)     2573 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_autounmask_use_backtrack.py
--rw-r--r--   0 root         (0) root         (0)     3743 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_autounmask_use_breakage.py
--rw-r--r--   0 root         (0) root         (0)     1830 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py
--rw-r--r--   0 root         (0) root         (0)     5786 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/resolver/test_backtracking.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_bdeps.py
--rw-r--r--   0 root         (0) root         (0)     4927 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py
--rw-r--r--   0 root         (0) root         (0)     4231 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/resolver/test_blocker.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_changed_deps.py
--rw-r--r--   0 root         (0) root         (0)     7899 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_circular_choices.py
--rw-r--r--   0 root         (0) root         (0)     3341 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_circular_choices_rust.py
--rw-r--r--   0 root         (0) root         (0)     4832 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_circular_dependencies.py
--rw-r--r--   0 root         (0) root         (0)     4948 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_complete_graph.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py
--rw-r--r--   0 root         (0) root         (0)     9959 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_depclean.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_depclean_order.py
--rw-r--r--   0 root         (0) root         (0)     2443 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_depclean_slot_unavailable.py
--rw-r--r--   0 root         (0) root         (0)    13128 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_depth.py
--rw-r--r--   0 root         (0) root         (0)     3329 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_disjunctive_depend_order.py
--rw-r--r--   0 root         (0) root         (0)     9983 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_eapi.py
--rw-r--r--   0 root         (0) root         (0)     2658 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_features_test_use.py
--rw-r--r--   0 root         (0) root         (0)     3379 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py
--rw-r--r--   0 root         (0) root         (0)     3457 2022-09-10 09:45:01.057050 portage-3.0.46/lib/portage/tests/resolver/test_installkernel.py
--rw-r--r--   0 root         (0) root         (0)    11063 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_keywords.py
--rw-r--r--   0 root         (0) root         (0)    31088 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_merge_order.py
--rw-r--r--   0 root         (0) root         (0)     1234 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_multirepo.py
--rw-r--r--   0 root         (0) root         (0)     1772 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/resolver/test_multislot.py
--rw-r--r--   0 root         (0) root         (0)     1554 2022-09-10 09:44:56.963689 portage-3.0.46/lib/portage/tests/resolver/test_old_dep_chain_display.py
--rw-r--r--   0 root         (0) root         (0)     1142 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_onlydeps.py
--rw-r--r--   0 root         (0) root         (0)     1527 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_onlydeps_circular.py
--rw-r--r--   0 root         (0) root         (0)     5933 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_onlydeps_ideps.py
--rw-r--r--   0 root         (0) root         (0)     2552 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_onlydeps_minimal.py
--rw-r--r--   0 root         (0) root         (0)    25072 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_or_choices.py
--rw-r--r--   0 root         (0) root         (0)     2716 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_or_downgrade_installed.py
--rw-r--r--   0 root         (0) root         (0)     6850 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_or_upgrade_installed.py
--rw-r--r--   0 root         (0) root         (0)     3911 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_output.py
--rw-r--r--   0 root         (0) root         (0)     9049 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_package_tracker.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_profile_default_eapi.py
--rw-r--r--   0 root         (0) root         (0)     3353 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_profile_package_set.py
--rw-r--r--   0 root         (0) root         (0)     6911 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     2409 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py
--rw-r--r--   0 root         (0) root         (0)    11792 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_required_use.py
--rw-r--r--   0 root         (0) root         (0)     2640 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_simple.py
--rw-r--r--   0 root         (0) root         (0)    18128 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_abi.py
--rw-r--r--   0 root         (0) root         (0)     8790 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_abi_downgrade.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_change_without_revbump.py
--rw-r--r--   0 root         (0) root         (0)    13393 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_collisions.py
--rw-r--r--   0 root         (0) root         (0)     1990 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     1432 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_mask_update.py
--rw-r--r--   0 root         (0) root         (0)    14826 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     7910 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_update.py
--rw-r--r--   0 root         (0) root         (0)     2491 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_update_virt.py
--rw-r--r--   0 root         (0) root         (0)     5024 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_autounmask.py
--rw-r--r--   0 root         (0) root         (0)     7642 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_bdeps.py
--rw-r--r--   0 root         (0) root         (0)     4350 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_complete_graph.py
--rw-r--r--   0 root         (0) root         (0)     4694 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py
--rw-r--r--   0 root         (0) root         (0)     4366 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_missed_update.py
--rw-r--r--   0 root         (0) root         (0)     3719 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_required_use.py
--rw-r--r--   0 root         (0) root         (0)     9190 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py
--rw-r--r--   0 root         (0) root         (0)     3974 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_unsolved.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py
--rw-r--r--   0 root         (0) root         (0)     3584 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/tests/resolver/test_targetroot.py
--rw-r--r--   0 root         (0) root         (0)     1571 2022-09-10 09:45:01.060384 portage-3.0.46/lib/portage/tests/resolver/test_unecessary_slot_upgrade.py
--rw-r--r--   0 root         (0) root         (0)    11321 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/tests/resolver/test_unmerge_order.py
--rw-r--r--   0 root         (0) root         (0)     3843 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_update.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_use_dep_defaults.py
--rw-r--r--   0 root         (0) root         (0)     5326 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_useflags.py
--rw-r--r--   0 root         (0) root         (0)     9976 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_virtual_minimize_children.py
--rw-r--r--   0 root         (0) root         (0)     9326 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/resolver/test_virtual_slot.py
--rw-r--r--   0 root         (0) root         (0)     2910 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/resolver/test_with_test_deps.py
--rwxr-xr-x   0 root         (0) root         (0)     2100 2023-03-21 03:50:18.064091 portage-3.0.46/lib/portage/tests/runTests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/sets/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sets/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sets/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/sets/base/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sets/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sets/base/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/sets/base/testInternalPackageSet.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/sets/base/testVariableSet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/sets/files/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sets/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sets/files/__test__.py
--rw-r--r--   0 root         (0) root         (0)      992 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/sets/files/testConfigFileSet.py
--rw-r--r--   0 root         (0) root         (0)      829 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/sets/files/testStaticFileSet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/sets/shell/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sets/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sets/shell/__test__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/sets/shell/testShell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/sync/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/sync/__test__.py
--rw-r--r--   0 root         (0) root         (0)    16481 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/sync/test_sync_local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/unicode/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/unicode/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.46/lib/portage/tests/unicode/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2294 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/unicode/test_string_format.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/update/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.110799 portage-3.0.46/lib/portage/tests/update/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.110799 portage-3.0.46/lib/portage/tests/update/__test__.py
--rw-r--r--   0 root         (0) root         (0)     4462 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/update/test_move_ent.py
--rw-r--r--   0 root         (0) root         (0)     5444 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/update/test_move_slot_ent.py
--rw-r--r--   0 root         (0) root         (0)    11460 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/update/test_update_dbentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/util/
--rw-r--r--   0 root         (0) root         (0)      170 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/util/dyn_libs/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/dyn_libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/dyn_libs/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1389 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/util/dyn_libs/test_soname_deps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/util/eventloop/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/eventloop/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/eventloop/__test__.py
--rw-r--r--   0 root         (0) root         (0)      826 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/eventloop/test_call_soon_fifo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/util/file_copy/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/file_copy/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/file_copy/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/file_copy/test_copyfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.591655 portage-3.0.46/lib/portage/tests/util/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.46/lib/portage/tests/util/futures/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/tests/util/futures/asyncio/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.46/lib/portage/tests/util/futures/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.46/lib/portage/tests/util/futures/asyncio/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_child_watcher.py
--rw-r--r--   0 root         (0) root         (0)     2025 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py
--rw-r--r--   0 root         (0) root         (0)     5394 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py
--rw-r--r--   0 root         (0) root         (0)      795 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py
--rw-r--r--   0 root         (0) root         (0)     1394 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py
--rw-r--r--   0 root         (0) root         (0)     6912 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py
--rw-r--r--   0 root         (0) root         (0)     7135 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/futures/test_compat_coroutine.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/futures/test_done_callback.py
--rw-r--r--   0 root         (0) root         (0)     1565 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/util/futures/test_done_callback_after_exit.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/futures/test_iter_completed.py
--rw-r--r--   0 root         (0) root         (0)    10828 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/futures/test_retry.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-03-21 03:50:18.064091 portage-3.0.46/lib/portage/tests/util/test_checksum.py
--rw-r--r--   0 root         (0) root         (0)    11345 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/test_digraph.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/test_file_copier.py
--rw-r--r--   0 root         (0) root         (0)     3534 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/test_getconfig.py
--rw-r--r--   0 root         (0) root         (0)      315 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/util/test_grabdict.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/test_install_mask.py
--rw-r--r--   0 root         (0) root         (0)     1120 2022-12-24 02:35:49.845990 portage-3.0.46/lib/portage/tests/util/test_manifest.py
--rw-r--r--   0 root         (0) root         (0)    10489 2022-09-10 09:45:01.057050 portage-3.0.46/lib/portage/tests/util/test_mtimedb.py
--rw-r--r--   0 root         (0) root         (0)      440 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/test_normalizedPath.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-04-02 19:17:09.550903 portage-3.0.46/lib/portage/tests/util/test_shelve.py
--rw-r--r--   0 root         (0) root         (0)     6638 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/test_socks5.py
--rw-r--r--   0 root         (0) root         (0)      832 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/util/test_stackDictList.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/tests/util/test_stackDicts.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/test_stackLists.py
--rw-r--r--   0 root         (0) root         (0)      897 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/tests/util/test_uniqueArray.py
--rw-r--r--   0 root         (0) root         (0)     3347 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/test_varExpand.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/test_whirlpool.py
--rw-r--r--   0 root         (0) root         (0)     6243 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/util/test_xattr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/tests/versions/
--rw-r--r--   0 root         (0) root         (0)      174 2021-11-12 08:15:36.117466 portage-3.0.46/lib/portage/tests/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.46/lib/portage/tests/versions/__test__.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/versions/test_cpv_sort_key.py
--rw-r--r--   0 root         (0) root         (0)     3026 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/versions/test_vercmp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/tests/xpak/
--rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.117466 portage-3.0.46/lib/portage/tests/xpak/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.46/lib/portage/tests/xpak/__test__.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/tests/xpak/test_decodeint.py
--rw-r--r--   0 root         (0) root         (0)    17014 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/
--rw-r--r--   0 root         (0) root         (0)     3063 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/ExtractKernelVersion.py
--rw-r--r--   0 root         (0) root         (0)     2141 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/SlotObject.py
--rw-r--r--   0 root         (0) root         (0)    68707 2023-03-21 03:50:18.064091 portage-3.0.46/lib/portage/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/_async/
--rw-r--r--   0 root         (0) root         (0)     2609 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/_async/AsyncFunction.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/_async/AsyncScheduler.py
--rw-r--r--   0 root         (0) root         (0)      963 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/_async/AsyncTaskFuture.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/_async/BuildLogger.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/_async/FileCopier.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/_async/FileDigester.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_async/ForkProcess.py
--rw-r--r--   0 root         (0) root         (0)     7527 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_async/PipeLogger.py
--rw-r--r--   0 root         (0) root         (0)     2676 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_async/PipeReaderBlockingIO.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_async/PopenProcess.py
--rw-r--r--   0 root         (0) root         (0)     4501 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_async/SchedulerInterface.py
--rw-r--r--   0 root         (0) root         (0)      644 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/util/_async/TaskScheduler.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.127466 portage-3.0.46/lib/portage/util/_async/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1360 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/util/_async/run_main_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     4347 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/_compare_files.py
--rw-r--r--   0 root         (0) root         (0)     1219 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/_ctypes.py
--rw-r--r--   0 root         (0) root         (0)     2654 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/_desktop_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/_dyn_libs/
--rw-r--r--   0 root         (0) root         (0)    41425 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_dyn_libs/LinkageMapELF.py
--rw-r--r--   0 root         (0) root         (0)     2877 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/_dyn_libs/NeededEntry.py
--rw-r--r--   0 root         (0) root         (0)     9385 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.130799 portage-3.0.46/lib/portage/util/_dyn_libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3834 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_dyn_libs/display_preserved_libs.py
--rw-r--r--   0 root         (0) root         (0)     1070 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/util/_dyn_libs/dyn_libs.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_dyn_libs/soname_deps.py
--rw-r--r--   0 root         (0) root         (0)     3722 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_dyn_libs/soname_deps_qa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/_eventloop/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.134132 portage-3.0.46/lib/portage/util/_eventloop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5849 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/util/_eventloop/asyncio_event_loop.py
--rw-r--r--   0 root         (0) root         (0)      213 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/util/_eventloop/global_event_loop.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_get_vm_info.py
--rw-r--r--   0 root         (0) root         (0)     5956 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/_info_files.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/_path.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/_pty.py
--rw-r--r--   0 root         (0) root         (0)     4032 2022-09-10 09:45:01.060384 portage-3.0.46/lib/portage/util/_urlopen.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/_xattr.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/backoff.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/bin_entry_point.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3464 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/compression_probe.py
--rw-r--r--   0 root         (0) root         (0)     2403 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/configparser.py
--rw-r--r--   0 root         (0) root         (0)     2180 2022-12-24 02:35:49.845990 portage-3.0.46/lib/portage/util/cpuinfo.py
--rw-r--r--   0 root         (0) root         (0)    12975 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/digraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/elf/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.137466 portage-3.0.46/lib/portage/util/elf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/elf/constants.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/elf/header.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/endian/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.137466 portage-3.0.46/lib/portage/util/endian/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1303 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/endian/decode.py
--rw-r--r--   0 root         (0) root         (0)    15592 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/env_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/file_copy/
--rw-r--r--   0 root         (0) root         (0)      909 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/file_copy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2118 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/formatter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/futures/
--rw-r--r--   0 root         (0) root         (0)      180 2022-09-10 09:44:56.967023 portage-3.0.46/lib/portage/util/futures/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/futures/_asyncio/
--rw-r--r--   0 root         (0) root         (0)     9758 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/futures/_asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/futures/_asyncio/streams.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/futures/_sync_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/futures/compat_coroutine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/futures/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.140799 portage-3.0.46/lib/portage/util/futures/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4306 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/futures/executor/fork.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/futures/extendedfutures.py
--rw-r--r--   0 root         (0) root         (0)      516 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/util/futures/futures.py
--rw-r--r--   0 root         (0) root         (0)     6868 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/futures/iter_completed.py
--rw-r--r--   0 root         (0) root         (0)     6297 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/util/futures/retry.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/futures/unix_events.py
--rw-r--r--   0 root         (0) root         (0)     1584 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/hooks.py
--rw-r--r--   0 root         (0) root         (0)     6549 2022-09-10 09:45:01.060384 portage-3.0.46/lib/portage/util/install_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/util/iterators/
--rw-r--r--   0 root         (0) root         (0)     2996 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/iterators/MultiIterGroupBy.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.144132 portage-3.0.46/lib/portage/util/iterators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7349 2022-09-10 09:45:01.063717 portage-3.0.46/lib/portage/util/lafilefixer.py
--rw-r--r--   0 root         (0) root         (0)     4814 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/listdir.py
--rw-r--r--   0 root         (0) root         (0)     4339 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/locale.py
--rw-r--r--   0 root         (0) root         (0)    13909 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/movefile.py
--rw-r--r--   0 root         (0) root         (0)     4258 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/mtimedb.py
--rw-r--r--   0 root         (0) root         (0)     2990 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/netlink.py
--rw-r--r--   0 root         (0) root         (0)     1336 2022-09-10 09:44:56.970356 portage-3.0.46/lib/portage/util/path.py
--rw-r--r--   0 root         (0) root         (0)     1527 2022-09-10 09:45:01.057050 portage-3.0.46/lib/portage/util/shelve.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/socks5.py
--rw-r--r--   0 root         (0) root         (0)    58416 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/util/whirlpool.py
--rw-r--r--   0 root         (0) root         (0)     4506 2023-03-21 03:35:23.553538 portage-3.0.46/lib/portage/util/writeable_check.py
--rw-r--r--   0 root         (0) root         (0)    19275 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/lib/portage/xml/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.147466 portage-3.0.46/lib/portage/xml/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16789 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/xml/metadata.py
--rw-r--r--   0 root         (0) root         (0)    19413 2023-03-21 03:35:23.556871 portage-3.0.46/lib/portage/xpak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/misc/
--rwxr-xr-x   0 root         (0) root         (0)    24116 2023-02-03 18:03:13.736861 portage-3.0.46/misc/emerge-delta-webrsync
--rwxr-xr-x   0 root         (0) root         (0)    29953 2023-04-07 09:54:54.254527 portage-3.0.46/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 09:56:10.594988 portage-3.0.46/src/
--rw-r--r--   0 root         (0) root         (0)    71291 2023-03-21 03:35:23.556871 portage-3.0.46/src/portage_util__whirlpool.c
--rw-r--r--   0 root         (0) root         (0)    13384 2023-03-21 03:35:23.556871 portage-3.0.46/src/portage_util_file_copy_reflink_linux.c
--rw-r--r--   0 root         (0) root         (0)     1276 2023-03-21 03:35:23.556871 portage-3.0.46/src/portage_util_libc.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:35.927469 portage-3.0.47/.portage_not_installed
+-rw-r--r--   0 root         (0) root         (0)     6944 2023-03-21 03:50:18.057424 portage-3.0.47/DEVELOPING
+-rw-r--r--   0 root         (0) root         (0)    18092 2021-11-12 08:15:35.927469 portage-3.0.47/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-04-30 04:11:56.749078 portage-3.0.47/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1864 2021-11-12 08:15:35.927469 portage-3.0.47/TEST-NOTES
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.722411 portage-3.0.47/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     3262 2023-03-21 23:52:40.754842 portage-3.0.47/bin/archive-conf
+-rwxr-xr-x   0 root         (0) root         (0)     1443 2023-04-07 10:38:37.709109 portage-3.0.47/bin/bashrc-functions.sh
+-rwxr-xr-x   0 root         (0) root         (0)     4457 2023-03-21 23:52:40.598174 portage-3.0.47/bin/binhost-snapshot
+-rwxr-xr-x   0 root         (0) root         (0)       51 2021-11-12 08:15:35.934136 portage-3.0.47/bin/cgroup-release-agent
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.934136 portage-3.0.47/bin/chmod-lite -> ebuild-pyhelper
+-rwxr-xr-x   0 root         (0) root         (0)      951 2023-03-21 03:35:23.553538 portage-3.0.47/bin/chmod-lite.py
+-rwxr-xr-x   0 root         (0) root         (0)     5891 2023-03-21 03:35:23.553538 portage-3.0.47/bin/chpathtool.py
+-rwxr-xr-x   0 root         (0) root         (0)     1421 2023-03-21 03:35:23.553538 portage-3.0.47/bin/clean_locks
+-rwxr-xr-x   0 root         (0) root         (0)    19951 2023-04-29 04:41:18.541267 portage-3.0.47/bin/dispatch-conf
+-rwxr-xr-x   0 root         (0) root         (0)     8895 2023-04-29 04:41:16.537917 portage-3.0.47/bin/dohtml.py
+-rwxr-xr-x   0 root         (0) root         (0)    20007 2023-04-07 10:38:37.709109 portage-3.0.47/bin/doins.py
+-rwxr-xr-x   0 root         (0) root         (0)     6078 2023-04-07 10:38:37.709109 portage-3.0.47/bin/eapi.sh
+-rwxr-xr-x   0 root         (0) root         (0)     4310 2023-04-07 10:38:37.709109 portage-3.0.47/bin/eapi7-ver-funcs.sh
+-rwxr-xr-x   0 root         (0) root         (0)    15468 2023-03-21 23:52:40.598174 portage-3.0.47/bin/ebuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/ebuild-helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/ebuild-helpers/bsd/
+-rwxr-xr-x   0 root         (0) root         (0)      639 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/bsd/sed
+-rwxr-xr-x   0 root         (0) root         (0)      200 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/die
+-rwxr-xr-x   0 root         (0) root         (0)     1049 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/dobin
+-rwxr-xr-x   0 root         (0) root         (0)      515 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doconfd
+-rwxr-xr-x   0 root         (0) root         (0)      359 2022-09-10 09:45:01.057050 portage-3.0.47/bin/ebuild-helpers/dodir
+-rwxr-xr-x   0 root         (0) root         (0)      885 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/dodoc
+-rwxr-xr-x   0 root         (0) root         (0)      513 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doenvd
+-rwxr-xr-x   0 root         (0) root         (0)      952 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doexe
+-rwxr-xr-x   0 root         (0) root         (0)      531 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/dohard
+-rwxr-xr-x   0 root         (0) root         (0)      632 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doheader
+-rwxr-xr-x   0 root         (0) root         (0)      782 2022-09-10 09:45:01.063717 portage-3.0.47/bin/ebuild-helpers/dohtml
+-rwxr-xr-x   0 root         (0) root         (0)      722 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/doinfo
+-rwxr-xr-x   0 root         (0) root         (0)      485 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doinitd
+-rwxr-xr-x   0 root         (0) root         (0)     3034 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doins
+-rwxr-xr-x   0 root         (0) root         (0)     1438 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/dolib
+-rwxr-xr-x   0 root         (0) root         (0)      189 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/dolib.a
+-rwxr-xr-x   0 root         (0) root         (0)      189 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/dolib.so
+-rwxr-xr-x   0 root         (0) root         (0)     1553 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/doman
+-rwxr-xr-x   0 root         (0) root         (0)     1216 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/domo
+-rwxr-xr-x   0 root         (0) root         (0)     1053 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/dosbin
+-rwxr-xr-x   0 root         (0) root         (0)      818 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/dosed
+-rwxr-xr-x   0 root         (0) root         (0)     2366 2022-09-10 09:45:01.063717 portage-3.0.47/bin/ebuild-helpers/dosym
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.47/bin/ebuild-helpers/eerror -> elog
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.47/bin/ebuild-helpers/einfo -> elog
+-rwxr-xr-x   0 root         (0) root         (0)      204 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/elog
+-rwxr-xr-x   0 root         (0) root         (0)      894 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/emake
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.47/bin/ebuild-helpers/eqawarn -> elog
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.47/bin/ebuild-helpers/ewarn -> elog
+-rwxr-xr-x   0 root         (0) root         (0)      792 2022-09-10 09:45:01.057050 portage-3.0.47/bin/ebuild-helpers/fowners
+-rwxr-xr-x   0 root         (0) root         (0)      850 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/fperms
+-rwxr-xr-x   0 root         (0) root         (0)      490 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/keepdir
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newbin -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newconfd -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newdoc -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newenvd -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newexe -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newheader -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newinitd -> newins
+-rwxr-xr-x   0 root         (0) root         (0)     1201 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newlib.a -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newlib.so -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newman -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newsbin -> newins
+-rwxr-xr-x   0 root         (0) root         (0)      359 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/nonfatal
+-rwxr-xr-x   0 root         (0) root         (0)      739 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/portageq
+-rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/prepall
+-rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/prepalldocs
+-rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/prepallinfo
+-rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/prepallman
+-rwxr-xr-x   0 root         (0) root         (0)      383 2022-09-10 09:45:01.057050 portage-3.0.47/bin/ebuild-helpers/prepallstrip
+-rwxr-xr-x   0 root         (0) root         (0)      843 2023-04-09 06:49:46.512769 portage-3.0.47/bin/ebuild-helpers/prepinfo
+-rwxr-xr-x   0 root         (0) root         (0)      364 2023-04-09 06:49:46.512769 portage-3.0.47/bin/ebuild-helpers/prepman
+-rwxr-xr-x   0 root         (0) root         (0)      375 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/prepstrip
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/ebuild-helpers/unprivileged/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/unprivileged/chgrp -> chown
+-rwxr-xr-x   0 root         (0) root         (0)     1178 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/unprivileged/chown
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/ebuild-helpers/xattr/
+-rwxr-xr-x   0 root         (0) root         (0)     1369 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/xattr/install
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-ipc -> ebuild-pyhelper
+-rwxr-xr-x   0 root         (0) root         (0)    10684 2023-03-21 23:52:40.598174 portage-3.0.47/bin/ebuild-ipc.py
+-rwxr-xr-x   0 root         (0) root         (0)      616 2022-09-10 09:45:01.057050 portage-3.0.47/bin/ebuild-pyhelper
+-rwxr-xr-x   0 root         (0) root         (0)    26114 2023-03-21 03:35:23.556871 portage-3.0.47/bin/ebuild.sh
+-rwxr-xr-x   0 root         (0) root         (0)     6481 2022-12-24 02:35:49.845990 portage-3.0.47/bin/ecompress
+-rwxr-xr-x   0 root         (0) root         (0)     1746 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ecompress-file
+-rwxr-xr-x   0 root         (0) root         (0)    53990 2023-03-21 23:52:40.598174 portage-3.0.47/bin/egencache
+-rwxr-xr-x   0 root         (0) root         (0)     1857 2023-03-21 03:35:23.556871 portage-3.0.47/bin/emaint
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-03-21 23:52:40.598174 portage-3.0.47/bin/emerge
+-rwxr-xr-x   0 root         (0) root         (0)    18798 2023-04-09 07:25:51.408246 portage-3.0.47/bin/emerge-webrsync
+-rwxr-xr-x   0 root         (0) root         (0)      634 2022-09-10 09:45:01.053717 portage-3.0.47/bin/emirrordist
+-rwxr-xr-x   0 root         (0) root         (0)     1048 2023-03-21 03:35:23.556871 portage-3.0.47/bin/env-update
+-rwxr-xr-x   0 root         (0) root         (0)    17296 2023-03-21 03:35:23.556871 portage-3.0.47/bin/estrip
+-rwxr-xr-x   0 root         (0) root         (0)    23454 2023-03-21 03:50:18.057424 portage-3.0.47/bin/etc-update
+-rwxr-xr-x   0 root         (0) root         (0)     6045 2023-03-21 03:35:23.556871 portage-3.0.47/bin/filter-bash-environment.py
+-rwxr-xr-x   0 root         (0) root         (0)     1601 2023-03-21 03:35:23.556871 portage-3.0.47/bin/fixpackages
+-rwxr-xr-x   0 root         (0) root         (0)    15636 2023-03-21 23:52:40.601508 portage-3.0.47/bin/glsa-check
+-rwxr-xr-x   0 root         (0) root         (0)     2166 2023-03-21 03:35:23.556871 portage-3.0.47/bin/gpkg-helper.py
+-rwxr-xr-x   0 root         (0) root         (0)     2476 2022-12-24 02:35:49.845990 portage-3.0.47/bin/gpkg-sign
+-rwxr-xr-x   0 root         (0) root         (0)     2918 2023-04-07 10:38:37.709109 portage-3.0.47/bin/helper-functions.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/install-qa-check.d/
+-rwxr-xr-x   0 root         (0) root         (0)      444 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/05double-D
+-rwxr-xr-x   0 root         (0) root         (0)     4302 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/05prefix
+-rwxr-xr-x   0 root         (0) root         (0)     5559 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/10executable-issues
+-rwxr-xr-x   0 root         (0) root         (0)     3591 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/10ignored-flags
+-rwxr-xr-x   0 root         (0) root         (0)      406 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/20deprecated-directories
+-rwxr-xr-x   0 root         (0) root         (0)      835 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/20runtime-directories
+-rwxr-xr-x   0 root         (0) root         (0)     3306 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60bash-completion
+-rwxr-xr-x   0 root         (0) root         (0)     1443 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60openrc
+-rwxr-xr-x   0 root         (0) root         (0)     5508 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60pkgconfig
+-rwxr-xr-x   0 root         (0) root         (0)      668 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60pngfix
+-rwxr-xr-x   0 root         (0) root         (0)      687 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60systemd
+-rwxr-xr-x   0 root         (0) root         (0)      442 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60udev
+-rwxr-xr-x   0 root         (0) root         (0)     5556 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/80libraries
+-rwxr-xr-x   0 root         (0) root         (0)     1417 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/80multilib-strict
+-rwxr-xr-x   0 root         (0) root         (0)     1918 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90bad-bin-group-write
+-rwxr-xr-x   0 root         (0) root         (0)     1566 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90bad-bin-owner
+-rwxr-xr-x   0 root         (0) root         (0)      654 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90cmake-warnings
+-rwxr-xr-x   0 root         (0) root         (0)     3333 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90config-impl-decl
+-rwxr-xr-x   0 root         (0) root         (0)     1277 2023-04-23 20:49:21.036042 portage-3.0.47/bin/install-qa-check.d/90cython-dep
+-rwxr-xr-x   0 root         (0) root         (0)     8300 2023-04-09 06:49:46.512769 portage-3.0.47/bin/install-qa-check.d/90gcc-warnings
+-rwxr-xr-x   0 root         (0) root         (0)     1042 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90world-writable
+-rwxr-xr-x   0 root         (0) root         (0)     1518 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/95empty-dirs
+-rwxr-xr-x   0 root         (0) root         (0)     6314 2023-03-21 23:52:40.601508 portage-3.0.47/bin/install.py
+-rwxr-xr-x   0 root         (0) root         (0)    18552 2023-04-07 10:38:37.712442 portage-3.0.47/bin/isolated-functions.sh
+-rwxr-xr-x   0 root         (0) root         (0)      903 2023-03-21 03:35:23.553538 portage-3.0.47/bin/lock-helper.py
+-rwxr-xr-x   0 root         (0) root         (0)    20244 2023-04-09 06:49:46.512769 portage-3.0.47/bin/misc-functions.sh
+-rwxr-xr-x   0 root         (0) root         (0)    34584 2023-04-29 04:41:16.537917 portage-3.0.47/bin/phase-functions.sh
+-rwxr-xr-x   0 root         (0) root         (0)    33858 2023-04-29 04:41:16.537917 portage-3.0.47/bin/phase-helpers.sh
+-rwxr-xr-x   0 root         (0) root         (0)     5723 2023-04-07 10:38:37.712442 portage-3.0.47/bin/pid-ns-init
+-rwxr-xr-x   0 root         (0) root         (0)    51197 2023-03-21 23:52:40.601508 portage-3.0.47/bin/portageq
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/postinst-qa-check.d/
+-rwxr-xr-x   0 root         (0) root         (0)     5236 2023-04-07 10:38:37.712442 portage-3.0.47/bin/postinst-qa-check.d/50xdg-utils
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/preinst-qa-check.d/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.947469 portage-3.0.47/bin/preinst-qa-check.d/50xdg-utils -> ../postinst-qa-check.d/50xdg-utils
+-rwxr-xr-x   0 root         (0) root         (0)    16731 2023-03-21 23:52:40.601508 portage-3.0.47/bin/quickpkg
+-rwxr-xr-x   0 root         (0) root         (0)     4992 2023-03-21 03:35:23.556871 portage-3.0.47/bin/regenworld
+-rwxr-xr-x   0 root         (0) root         (0)     4535 2023-04-29 04:41:16.541251 portage-3.0.47/bin/save-ebuild-env.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1339 2022-09-10 09:45:01.060384 portage-3.0.47/bin/shelve-utils
+-rwxr-xr-x   0 root         (0) root         (0)     8140 2023-04-07 10:38:37.712442 portage-3.0.47/bin/socks5-server.py
+-rwxr-xr-x   0 root         (0) root         (0)     4784 2023-03-21 23:52:40.601508 portage-3.0.47/bin/xattr-helper.py
+-rwxr-xr-x   0 root         (0) root         (0)     1825 2023-03-21 03:35:23.550205 portage-3.0.47/bin/xpak-helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/cnf/
+-rw-r--r--   0 root         (0) root         (0)     1718 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.alpha.diff
+-rw-r--r--   0 root         (0) root         (0)     2319 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.amd64-fbsd.diff
+-rw-r--r--   0 root         (0) root         (0)     2309 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.amd64.diff
+-rw-r--r--   0 root         (0) root         (0)     1592 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.arm.diff
+-rw-r--r--   0 root         (0) root         (0)     1580 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.arm64.diff
+-rw-r--r--   0 root         (0) root         (0)     2465 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.hppa.diff
+-rw-r--r--   0 root         (0) root         (0)      663 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.ia64.diff
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-03-21 03:35:23.550205 portage-3.0.47/cnf/make.conf.example.loong.diff
+-rw-r--r--   0 root         (0) root         (0)      900 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.m68k.diff
+-rw-r--r--   0 root         (0) root         (0)     1383 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.mips.diff
+-rw-r--r--   0 root         (0) root         (0)     3541 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.ppc.diff
+-rw-r--r--   0 root         (0) root         (0)     2361 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.ppc64.diff
+-rw-r--r--   0 root         (0) root         (0)     2332 2022-09-10 09:44:56.963689 portage-3.0.47/cnf/make.conf.example.riscv.diff
+-rw-r--r--   0 root         (0) root         (0)      656 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.s390.diff
+-rw-r--r--   0 root         (0) root         (0)     1257 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.sh.diff
+-rw-r--r--   0 root         (0) root         (0)      728 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.sparc-fbsd.diff
+-rw-r--r--   0 root         (0) root         (0)     2129 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.sparc.diff
+-rw-r--r--   0 root         (0) root         (0)     2507 2021-12-09 09:19:33.763473 portage-3.0.47/cnf/make.conf.example.x86-fbsd.diff
+-rw-r--r--   0 root         (0) root         (0)     3759 2021-12-09 09:19:33.763473 portage-3.0.47/cnf/make.conf.example.x86.diff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/api/
+-rw-r--r--   0 root         (0) root         (0)     1141 2021-11-12 08:15:35.954135 portage-3.0.47/doc/api/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-03-21 03:35:23.550205 portage-3.0.47/doc/api/conf.py
+-rw-r--r--   0 root         (0) root         (0)      217 2021-11-12 08:15:35.954135 portage-3.0.47/doc/api/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/config/
+-rw-r--r--   0 root         (0) root         (0)     1900 2021-11-12 08:15:35.954135 portage-3.0.47/doc/config/bashrc.docbook
+-rw-r--r--   0 root         (0) root         (0)    26214 2021-11-12 08:15:35.954135 portage-3.0.47/doc/config/sets.docbook
+-rw-r--r--   0 root         (0) root         (0)       85 2021-11-12 08:15:35.954135 portage-3.0.47/doc/config.docbook
+-rw-r--r--   0 root         (0) root         (0)      257 2021-11-12 08:15:35.954135 portage-3.0.47/doc/custom.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/dependency_resolution/
+-rw-r--r--   0 root         (0) root         (0)     3281 2021-11-12 08:15:35.957468 portage-3.0.47/doc/dependency_resolution/decision_making.docbook
+-rw-r--r--   0 root         (0) root         (0)     4154 2021-11-12 08:15:35.957468 portage-3.0.47/doc/dependency_resolution/package_modeling.docbook
+-rw-r--r--   0 root         (0) root         (0)     3451 2021-11-12 08:15:35.957468 portage-3.0.47/doc/dependency_resolution/task_scheduling.docbook
+-rw-r--r--   0 root         (0) root         (0)      200 2021-11-12 08:15:35.954135 portage-3.0.47/doc/dependency_resolution.docbook
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/package/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/package/ebuild/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.729078 portage-3.0.47/doc/package/ebuild/eapi/
+-rw-r--r--   0 root         (0) root         (0)      487 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/0.docbook
+-rw-r--r--   0 root         (0) root         (0)     1598 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/1.docbook
+-rw-r--r--   0 root         (0) root         (0)     8299 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/2.docbook
+-rw-r--r--   0 root         (0) root         (0)     2938 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/3.docbook
+-rw-r--r--   0 root         (0) root         (0)     3112 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/4-slot-abi.docbook
+-rw-r--r--   0 root         (0) root         (0)    14690 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/4.docbook
+-rw-r--r--   0 root         (0) root         (0)     8044 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/5.docbook
+-rw-r--r--   0 root         (0) root         (0)     1725 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/helper_functions.docbook
+-rw-r--r--   0 root         (0) root         (0)     2780 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/phases.docbook
+-rw-r--r--   0 root         (0) root         (0)      364 2022-09-10 09:45:01.060384 portage-3.0.47/doc/package/ebuild.docbook
+-rw-r--r--   0 root         (0) root         (0)       76 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package.docbook
+-rw-r--r--   0 root         (0) root         (0)     2194 2022-09-10 09:45:01.060384 portage-3.0.47/doc/portage.docbook
+-rw-r--r--   0 root         (0) root         (0)    19579 2021-11-12 08:15:35.960802 portage-3.0.47/doc/qa.docbook
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.712411 portage-3.0.47/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.729078 portage-3.0.47/lib/_emerge/
+-rw-r--r--   0 root         (0) root         (0)      816 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/AbstractDepPriority.py
+-rw-r--r--   0 root         (0) root         (0)    18460 2023-03-21 03:50:18.057424 portage-3.0.47/lib/_emerge/AbstractEbuildProcess.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/AbstractPollTask.py
+-rw-r--r--   0 root         (0) root         (0)    10471 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/AsynchronousLock.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/AsynchronousTask.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/AtomArg.py
+-rw-r--r--   0 root         (0) root         (0)    21241 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/Binpkg.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgEnvExtractor.py
+-rw-r--r--   0 root         (0) root         (0)     5494 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgExtractorAsync.py
+-rw-r--r--   0 root         (0) root         (0)     9584 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgFetcher.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgPrefetcher.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgVerifier.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/Blocker.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/BlockerCache.py
+-rw-r--r--   0 root         (0) root         (0)     5325 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/BlockerDB.py
+-rw-r--r--   0 root         (0) root         (0)      355 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/BlockerDepPriority.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/CompositeTask.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/DepPriority.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/DepPriorityNormalRange.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/DepPrioritySatisfiedRange.py
+-rw-r--r--   0 root         (0) root         (0)      878 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/Dependency.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/DependencyArg.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildBinpkg.py
+-rw-r--r--   0 root         (0) root         (0)    23204 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildBuild.py
+-rw-r--r--   0 root         (0) root         (0)     5749 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildBuildDir.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildExecuter.py
+-rw-r--r--   0 root         (0) root         (0)    14395 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildFetcher.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildFetchonly.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildIpcDaemon.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/EbuildMerge.py
+-rw-r--r--   0 root         (0) root         (0)     7597 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/EbuildMetadataPhase.py
+-rw-r--r--   0 root         (0) root         (0)    22622 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildPhase.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildProcess.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildSpawnProcess.py
+-rw-r--r--   0 root         (0) root         (0)    12786 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/FakeVartree.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/FifoIpcDaemon.py
+-rw-r--r--   0 root         (0) root         (0)     9113 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/JobStatusDisplay.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/MergeListItem.py
+-rw-r--r--   0 root         (0) root         (0)     6121 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/MetadataRegen.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2022-09-10 09:45:01.063717 portage-3.0.47/lib/_emerge/MiscFunctionsProcess.py
+-rw-r--r--   0 root         (0) root         (0)    31019 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/Package.py
+-rw-r--r--   0 root         (0) root         (0)      735 2022-09-10 09:44:56.967023 portage-3.0.47/lib/_emerge/PackageArg.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PackageMerge.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PackagePhase.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PackageUninstall.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2022-09-10 09:44:56.967023 portage-3.0.47/lib/_emerge/PackageVirtualDbapi.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PipeReader.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PollScheduler.py
+-rw-r--r--   0 root         (0) root         (0)      603 2022-09-10 09:44:56.967023 portage-3.0.47/lib/_emerge/ProgressHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2022-09-10 09:44:56.967023 portage-3.0.47/lib/_emerge/RootConfig.py
+-rw-r--r--   0 root         (0) root         (0)    85615 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/Scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/SequentialTaskQueue.py
+-rw-r--r--   0 root         (0) root         (0)      421 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/SetArg.py
+-rw-r--r--   0 root         (0) root         (0)    10190 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/SpawnProcess.py
+-rw-r--r--   0 root         (0) root         (0)     3167 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/SubProcess.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/Task.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/TaskSequence.py
+-rw-r--r--   0 root         (0) root         (0)      455 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/UninstallFailure.py
+-rw-r--r--   0 root         (0) root         (0)     1326 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/UnmergeDepPriority.py
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/UseFlagDisplay.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/UserQuery.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:35.977468 portage-3.0.47/lib/_emerge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/_find_deep_system_runtime_deps.py
+-rw-r--r--   0 root         (0) root         (0)      442 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/_flush_elog_mod_echo.py
+-rw-r--r--   0 root         (0) root         (0)   149373 2023-03-21 03:50:18.060757 portage-3.0.47/lib/_emerge/actions.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/chk_updated_cfg_files.py
+-rw-r--r--   0 root         (0) root         (0)      498 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/clear_caches.py
+-rw-r--r--   0 root         (0) root         (0)      586 2023-02-03 18:03:13.733528 portage-3.0.47/lib/_emerge/countdown.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/create_depgraph_params.py
+-rw-r--r--   0 root         (0) root         (0)     5191 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/create_world_atom.py
+-rw-r--r--   0 root         (0) root         (0)   499558 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/depgraph.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/emergelog.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/getloadavg.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2022-09-10 09:44:56.970356 portage-3.0.47/lib/_emerge/help.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/is_valid_package_atom.py
+-rw-r--r--   0 root         (0) root         (0)    42164 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/main.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/post_emerge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.729078 portage-3.0.47/lib/_emerge/resolver/
+-rw-r--r--   0 root         (0) root         (0)     3198 2022-09-10 09:44:56.970356 portage-3.0.47/lib/_emerge/resolver/DbapiProvidesIndex.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:35.980801 portage-3.0.47/lib/_emerge/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11328 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/backtracking.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/circular_dependency.py
+-rw-r--r--   0 root         (0) root         (0)    39548 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/output.py
+-rw-r--r--   0 root         (0) root         (0)    20756 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/output_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    15636 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/package_tracker.py
+-rw-r--r--   0 root         (0) root         (0)    59893 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/resolver/slot_collision.py
+-rw-r--r--   0 root         (0) root         (0)    20976 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/search.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/show_invalid_depstring_notice.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/stdout_spinner.py
+-rw-r--r--   0 root         (0) root         (0)    26564 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/unmerge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/
+-rw-r--r--   0 root         (0) root         (0)    25908 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/_compat_upgrade/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.007468 portage-3.0.47/lib/portage/_compat_upgrade/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/_compat_upgrade/binpkg_compression.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_compat_upgrade/binpkg_multi_instance.py
+-rw-r--r--   0 root         (0) root         (0)     4288 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_compat_upgrade/default_locations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/_emirrordist/
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_emirrordist/Config.py
+-rw-r--r--   0 root         (0) root         (0)     7223 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_emirrordist/ContentDB.py
+-rw-r--r--   0 root         (0) root         (0)     4631 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_emirrordist/DeletionIterator.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_emirrordist/DeletionTask.py
+-rw-r--r--   0 root         (0) root         (0)    11176 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_emirrordist/FetchIterator.py
+-rw-r--r--   0 root         (0) root         (0)    25443 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_emirrordist/FetchTask.py
+-rw-r--r--   0 root         (0) root         (0)     9145 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_emirrordist/MirrorDistTask.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.007468 portage-3.0.47/lib/portage/_emirrordist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16082 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/_emirrordist/main.py
+-rw-r--r--   0 root         (0) root         (0)    10222 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_global_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/_legacy_globals.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_selinux.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/_sets/
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_sets/ProfilePackageSet.py
+-rw-r--r--   0 root         (0) root         (0)    14268 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/_sets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8205 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_sets/base.py
+-rw-r--r--   0 root         (0) root         (0)    22035 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_sets/dbapi.py
+-rw-r--r--   0 root         (0) root         (0)    15573 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_sets/files.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_sets/libs.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_sets/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_sets/security.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_sets/shell.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/binpkg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/binrepo/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.014134 portage-3.0.47/lib/portage/binrepo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4554 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/binrepo/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/cache/
+-rw-r--r--   0 root         (0) root         (0)      101 2021-11-12 08:15:36.014134 portage-3.0.47/lib/portage/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3167 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/anydbm.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/cache_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/ebuild_xattr.py
+-rw-r--r--   0 root         (0) root         (0)     5286 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/flat_hash.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/fs_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/cache/index/
+-rw-r--r--   0 root         (0) root         (0)      562 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/index/IndexStreamIterator.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.017468 portage-3.0.47/lib/portage/cache/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/index/pkg_desc_index.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/mappings.py
+-rw-r--r--   0 root         (0) root         (0)     5844 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    11820 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/sql_template.py
+-rw-r--r--   0 root         (0) root         (0)    13390 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)    13272 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/template.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/volatile.py
+-rw-r--r--   0 root         (0) root         (0)    16566 2023-04-07 09:45:44.114534 portage-3.0.47/lib/portage/checksum.py
+-rw-r--r--   0 root         (0) root         (0)     8879 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/const.py
+-rw-r--r--   0 root         (0) root         (0)    11470 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/cvstree.py
+-rw-r--r--   0 root         (0) root         (0)    11537 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/dbapi/
+-rw-r--r--   0 root         (0) root         (0)      643 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/dbapi/DummyTree.py
+-rw-r--r--   0 root         (0) root         (0)     5690 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dbapi/IndexedPortdb.py
+-rw-r--r--   0 root         (0) root         (0)     3743 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/dbapi/IndexedVardb.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dbapi/_ContentsCaseSensitivityManager.py
+-rw-r--r--   0 root         (0) root         (0)    10128 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/dbapi/_MergeProcess.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/dbapi/_SyncfsProcess.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/dbapi/_VdbMetadataDelta.py
+-rw-r--r--   0 root         (0) root         (0)    16769 2023-04-09 06:49:46.516103 portage-3.0.47/lib/portage/dbapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/dbapi/_expand_new_virt.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/dbapi/_similar_name_search.py
+-rw-r--r--   0 root         (0) root         (0)    90388 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dbapi/bintree.py
+-rw-r--r--   0 root         (0) root         (0)     4184 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/dbapi/cpv_expand.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/dbapi/dep_expand.py
+-rw-r--r--   0 root         (0) root         (0)    64264 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dbapi/porttree.py
+-rw-r--r--   0 root         (0) root         (0)   252193 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dbapi/vartree.py
+-rw-r--r--   0 root         (0) root         (0)     7587 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dbapi/virtual.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/dep/
+-rw-r--r--   0 root         (0) root         (0)   107693 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/_dnf.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/_slot_operator.py
+-rw-r--r--   0 root         (0) root         (0)    42498 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/dep_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/dep/soname/
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/soname/SonameAtom.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.030801 portage-3.0.47/lib/portage/dep/soname/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/dep/soname/multilib_category.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/dep/soname/parse.py
+-rw-r--r--   0 root         (0) root         (0)    14093 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dispatch_conf.py
+-rw-r--r--   0 root         (0) root         (0)     8092 2023-01-10 15:35:29.386865 portage-3.0.47/lib/portage/eapi.py
+-rw-r--r--   0 root         (0) root         (0)     6757 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/eclass_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/elog/
+-rw-r--r--   0 root         (0) root         (0)     6879 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/elog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      613 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/elog/filtering.py
+-rw-r--r--   0 root         (0) root         (0)     6065 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/elog/messages.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-02-03 18:03:13.736861 portage-3.0.47/lib/portage/elog/mod_custom.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/elog/mod_echo.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/elog/mod_mail.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/elog/mod_mail_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/elog/mod_save.py
+-rw-r--r--   0 root         (0) root         (0)     3580 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/elog/mod_save_summary.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/elog/mod_syslog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/
+-rw-r--r--   0 root         (0) root         (0)      163 2021-11-12 08:15:36.037467 portage-3.0.47/lib/portage/emaint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      762 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/
+-rw-r--r--   0 root         (0) root         (0)      173 2021-11-12 08:15:36.037467 portage-3.0.47/lib/portage/emaint/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/binhost/
+-rw-r--r--   0 root         (0) root         (0)      524 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/binhost/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/modules/binhost/binhost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/config/
+-rw-r--r--   0 root         (0) root         (0)      534 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/modules/config/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/logs/
+-rw-r--r--   0 root         (0) root         (0)     1629 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/modules/logs/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/merges/
+-rw-r--r--   0 root         (0) root         (0)     1417 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/merges/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/modules/merges/merges.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/emaint/modules/move/
+-rw-r--r--   0 root         (0) root         (0)      851 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/move/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7693 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/emaint/modules/move/move.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/emaint/modules/resume/
+-rw-r--r--   0 root         (0) root         (0)      566 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/resume/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/emaint/modules/resume/resume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/emaint/modules/sync/
+-rw-r--r--   0 root         (0) root         (0)     2145 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18469 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/emaint/modules/sync/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/emaint/modules/world/
+-rw-r--r--   0 root         (0) root         (0)      502 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/world/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/emaint/modules/world/world.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/env/
+-rw-r--r--   0 root         (0) root         (0)       52 2021-11-12 08:15:36.044134 portage-3.0.47/lib/portage/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/env/config.py
+-rw-r--r--   0 root         (0) root         (0)    10311 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/env/loaders.py
+-rw-r--r--   0 root         (0) root         (0)      578 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/env/validators.py
+-rw-r--r--   0 root         (0) root         (0)     6616 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/exception.py
+-rw-r--r--   0 root         (0) root         (0)    31465 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/getbinpkg.py
+-rw-r--r--   0 root         (0) root         (0)    31099 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/glsa.py
+-rw-r--r--   0 root         (0) root         (0)     3637 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/gpg.py
+-rw-r--r--   0 root         (0) root         (0)    80663 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/gpkg.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/localization.py
+-rw-r--r--   0 root         (0) root         (0)    28153 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/locks.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/mail.py
+-rw-r--r--   0 root         (0) root         (0)    31108 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/manifest.py
+-rw-r--r--   0 root         (0) root         (0)     8221 2023-02-03 18:03:13.736861 portage-3.0.47/lib/portage/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     8568 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/module.py
+-rw-r--r--   0 root         (0) root         (0)    18485 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/news.py
+-rw-r--r--   0 root         (0) root         (0)    29784 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.047467 portage-3.0.47/lib/portage/package/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/ebuild/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.050800 portage-3.0.47/lib/portage/package/ebuild/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/ebuild/_config/
+-rw-r--r--   0 root         (0) root         (0)    13005 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/package/ebuild/_config/KeywordsManager.py
+-rw-r--r--   0 root         (0) root         (0)     9192 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_config/LicenseManager.py
+-rw-r--r--   0 root         (0) root         (0)    16684 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_config/LocationsManager.py
+-rw-r--r--   0 root         (0) root         (0)    13915 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/MaskManager.py
+-rw-r--r--   0 root         (0) root         (0)    21565 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/package/ebuild/_config/UseManager.py
+-rw-r--r--   0 root         (0) root         (0)     8443 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/VirtualsManager.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.050800 portage-3.0.47/lib/portage/package/ebuild/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      770 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/env_var_validation.py
+-rw-r--r--   0 root         (0) root         (0)     4694 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/features_set.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/helper.py
+-rw-r--r--   0 root         (0) root         (0)     9457 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/package/ebuild/_config/special_env_vars.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/ebuild/_ipc/
+-rw-r--r--   0 root         (0) root         (0)      829 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_ipc/ExitCommand.py
+-rw-r--r--   0 root         (0) root         (0)      212 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_ipc/IpcCommand.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/package/ebuild/_ipc/QueryCommand.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.054134 portage-3.0.47/lib/portage/package/ebuild/_ipc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_metadata_invalid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.057467 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_spawn_nofetch.py
+-rw-r--r--   0 root         (0) root         (0)   133992 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/config.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/deprecated_profile_check.py
+-rw-r--r--   0 root         (0) root         (0)     6732 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/package/ebuild/digestcheck.py
+-rw-r--r--   0 root         (0) root         (0)     9424 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/package/ebuild/digestgen.py
+-rw-r--r--   0 root         (0) root         (0)   111579 2023-04-29 04:41:37.948089 portage-3.0.47/lib/portage/package/ebuild/doebuild.py
+-rw-r--r--   0 root         (0) root         (0)    79658 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/package/ebuild/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     4689 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/package/ebuild/getmaskingreason.py
+-rw-r--r--   0 root         (0) root         (0)     6556 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/package/ebuild/getmaskingstatus.py
+-rw-r--r--   0 root         (0) root         (0)    19287 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/package/ebuild/prepare_build_dirs.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/package/ebuild/profile_iuse.py
+-rw-r--r--   0 root         (0) root         (0)    41702 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/process.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/proxy/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.060800 portage-3.0.47/lib/portage/proxy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7832 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/proxy/lazyimport.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/proxy/objectproxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/repository/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.064134 portage-3.0.47/lib/portage/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62136 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/repository/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/repository/storage/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.064134 portage-3.0.47/lib/portage/repository/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3951 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/repository/storage/hardlink_quarantine.py
+-rw-r--r--   0 root         (0) root         (0)    10940 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/repository/storage/hardlink_rcu.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/repository/storage/inplace.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/repository/storage/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/
+-rw-r--r--   0 root         (0) root         (0)     1589 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2023-02-03 18:03:13.733528 portage-3.0.47/lib/portage/sync/config_checks.py
+-rw-r--r--   0 root         (0) root         (0)    14745 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/sync/controller.py
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/sync/getaddrinfo_validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.067467 portage-3.0.47/lib/portage/sync/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/cvs/
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-02-03 18:03:13.733528 portage-3.0.47/lib/portage/sync/modules/cvs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/sync/modules/cvs/cvs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/git/
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/sync/modules/git/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20049 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/sync/modules/git/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/mercurial/
+-rw-r--r--   0 root         (0) root         (0)     1403 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/sync/modules/mercurial/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6125 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/sync/modules/mercurial/mercurial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/rsync/
+-rw-r--r--   0 root         (0) root         (0)     1287 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/sync/modules/rsync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33953 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/sync/modules/rsync/rsync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/svn/
+-rw-r--r--   0 root         (0) root         (0)     1037 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/sync/modules/svn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/sync/modules/svn/svn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/webrsync/
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-04-09 06:51:34.556710 portage-3.0.47/lib/portage/sync/modules/webrsync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-04-09 06:51:34.716710 portage-3.0.47/lib/portage/sync/modules/webrsync/webrsync.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/sync/old_tree_timestamp.py
+-rw-r--r--   0 root         (0) root         (0)    13139 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/sync/syncbase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/.gnupg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/
+-rw-r--r--   0 root         (0) root         (0)     1850 2022-09-10 09:45:01.063717 portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev
+-rw-r--r--   0 root         (0) root         (0)     1852 2022-09-10 09:45:01.063717 portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/
+-rw-r--r--   0 root         (0) root         (0)     2055 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key
+-rw-r--r--   0 root         (0) root         (0)     2055 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key
+-rw-r--r--   0 root         (0) root         (0)     2774 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/tests/.gnupg/pubring.kbx
+-rw-r--r--   0 root         (0) root         (0)     1360 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/tests/.gnupg/trustdb.gpg
+-rw-r--r--   0 root         (0) root         (0)    11871 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/bin/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.47/lib/portage/tests/bin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.47/lib/portage/tests/bin/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/bin/setup_env.py
+-rw-r--r--   0 root         (0) root         (0)      547 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/bin/test_dobin.py
+-rw-r--r--   0 root         (0) root         (0)      565 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/bin/test_dodir.py
+-rw-r--r--   0 root         (0) root         (0)    13013 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/bin/test_doins.py
+-rw-r--r--   0 root         (0) root         (0)     9192 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/bin/test_eapi7_ver_funcs.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/bin/test_filter_bash_env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/dbapi/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.074133 portage-3.0.47/lib/portage/tests/dbapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.47/lib/portage/tests/dbapi/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dbapi/test_auxdb.py
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/tests/dbapi/test_bintree.py
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dbapi/test_fakedbapi.py
+-rw-r--r--   0 root         (0) root         (0)     9409 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dbapi/test_portdb_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/dep/
+-rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.077467 portage-3.0.47/lib/portage/tests/dep/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.077467 portage-3.0.47/lib/portage/tests/dep/__test__.py
+-rw-r--r--   0 root         (0) root         (0)    24520 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dep/testAtom.py
+-rw-r--r--   0 root         (0) root         (0)     9752 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/dep/testCheckRequiredUse.py
+-rw-r--r--   0 root         (0) root         (0)      779 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/dep/testExtendedAtomDict.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/dep/testExtractAffectingUSE.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dep/testStandalone.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/dep/test_best_match_to_list.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dep_getcpv.py
+-rw-r--r--   0 root         (0) root         (0)      988 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dep_getrepo.py
+-rw-r--r--   0 root         (0) root         (0)      934 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dep_getslot.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dep_getusedeps.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dnf_convert.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_get_operator.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_get_required_use_flags.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_isjustname.py
+-rw-r--r--   0 root         (0) root         (0)    11660 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_isvalidatom.py
+-rw-r--r--   0 root         (0) root         (0)    11132 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_match_from_list.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_overlap_dnf.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_paren_reduce.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_soname_atom_pickle.py
+-rw-r--r--   0 root         (0) root         (0)    27656 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dep/test_use_reduce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/ebuild/
+-rw-r--r--   0 root         (0) root         (0)      107 2021-11-12 08:15:36.080800 portage-3.0.47/lib/portage/tests/ebuild/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.080800 portage-3.0.47/lib/portage/tests/ebuild/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_array_fromfile_eof.py
+-rw-r--r--   0 root         (0) root         (0)    14001 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     5947 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py
+-rw-r--r--   0 root         (0) root         (0)     5167 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_doebuild_spawn.py
+-rw-r--r--   0 root         (0) root         (0)    35283 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_fetch.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_ipc_daemon.py
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_shell_quote.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/ebuild/test_spawn.py
+-rw-r--r--   0 root         (0) root         (0)     4479 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/ebuild/test_use_expand_incremental.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/emerge/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.080800 portage-3.0.47/lib/portage/tests/emerge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.080800 portage-3.0.47/lib/portage/tests/emerge/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2022-12-24 02:35:49.845990 portage-3.0.47/lib/portage/tests/emerge/test_actions.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/emerge/test_config_protect.py
+-rw-r--r--   0 root         (0) root         (0)     6335 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/emerge/test_emerge_slot_abi.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/emerge/test_global_updates.py
+-rw-r--r--   0 root         (0) root         (0)    26423 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/emerge/test_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/env/
+-rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/env/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/env/config/
+-rw-r--r--   0 root         (0) root         (0)      176 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/env/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/env/config/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/env/config/test_PackageKeywordsFile.py
+-rw-r--r--   0 root         (0) root         (0)      818 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/env/config/test_PackageMaskFile.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/env/config/test_PackageUseFile.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/env/config/test_PortageModulesFile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/glsa/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/glsa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/glsa/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/glsa/test_security_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/gpkg/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/gpkg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/gpkg/__test__.py
+-rw-r--r--   0 root         (0) root         (0)    13833 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_checksum.py
+-rw-r--r--   0 root         (0) root         (0)    15728 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_gpg.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_metadata_update.py
+-rw-r--r--   0 root         (0) root         (0)     5288 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_metadata_url.py
+-rw-r--r--   0 root         (0) root         (0)    14745 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_path.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_size.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/lafilefixer/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/lafilefixer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/lafilefixer/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     6338 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/lafilefixer/test_lafilefixer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/lazyimport/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/lazyimport/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/lazyimport/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py
+-rw-r--r--   0 root         (0) root         (0)      596 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/lazyimport/test_preload_portage_submodules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/lint/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/lint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/lint/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      214 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/lint/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/lint/test_bash_syntax.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/lint/test_compile_modules.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/lint/test_import_modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/locks/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/locks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/locks/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/locks/test_asynchronous_lock.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/locks/test_lock_nonblock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/news/
+-rw-r--r--   0 root         (0) root         (0)      170 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/news/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/news/__test__.py
+-rw-r--r--   0 root         (0) root         (0)    14363 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/news/test_NewsItem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/process/
+-rw-r--r--   0 root         (0) root         (0)      107 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/process/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/process/test_AsyncFunction.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_PipeLogger.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_PopenProcess.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_PopenProcessBlockingIO.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_poll.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_spawn_fail_e2big.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/tests/process/test_spawn_warn_large_env.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_unshare_net.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/resolver/
+-rw-r--r--   0 root         (0) root         (0)    42502 2023-03-21 03:50:18.064091 portage-3.0.47/lib/portage/tests/resolver/ResolverPlayground.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.47/lib/portage/tests/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.104133 portage-3.0.47/lib/portage/tests/resolver/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     5585 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py
+-rw-r--r--   0 root         (0) root         (0)     3747 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/resolver/soname/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/resolver/soname/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/resolver/soname/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_autounmask.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_depclean.py
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_downgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_or_choices.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_reinstall.py
+-rw-r--r--   0 root         (0) root         (0)     3338 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_skip_update.py
+-rw-r--r--   0 root         (0) root         (0)    12877 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_slot_conflict_update.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_soname_provided.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_unsatisfiable.py
+-rw-r--r--   0 root         (0) root         (0)     3354 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/soname/test_unsatisfied.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py
+-rw-r--r--   0 root         (0) root         (0)    28432 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_binpkg_use.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_keep_keywords.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_multilib_use.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_parent.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_backtrack.py
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_breakage.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_backtracking.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_bdeps.py
+-rw-r--r--   0 root         (0) root         (0)     4927 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py
+-rw-r--r--   0 root         (0) root         (0)     4231 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_blocker.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_changed_deps.py
+-rw-r--r--   0 root         (0) root         (0)     7899 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_circular_choices.py
+-rw-r--r--   0 root         (0) root         (0)     3341 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_circular_choices_rust.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_circular_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)     4948 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_complete_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py
+-rw-r--r--   0 root         (0) root         (0)     9959 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_depclean.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_depclean_order.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_depclean_slot_unavailable.py
+-rw-r--r--   0 root         (0) root         (0)    13128 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_depth.py
+-rw-r--r--   0 root         (0) root         (0)     3329 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_disjunctive_depend_order.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_eapi.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_features_test_use.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/resolver/test_installkernel.py
+-rw-r--r--   0 root         (0) root         (0)    11063 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_keywords.py
+-rw-r--r--   0 root         (0) root         (0)    31088 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_merge_order.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_multirepo.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_multislot.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_old_dep_chain_display.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_onlydeps.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_circular.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_ideps.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_minimal.py
+-rw-r--r--   0 root         (0) root         (0)    25072 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_or_choices.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_or_downgrade_installed.py
+-rw-r--r--   0 root         (0) root         (0)     6850 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_or_upgrade_installed.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_output.py
+-rw-r--r--   0 root         (0) root         (0)     9049 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_package_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_profile_default_eapi.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_profile_package_set.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py
+-rw-r--r--   0 root         (0) root         (0)    11792 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_required_use.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_simple.py
+-rw-r--r--   0 root         (0) root         (0)    18128 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_abi.py
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_abi_downgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_change_without_revbump.py
+-rw-r--r--   0 root         (0) root         (0)    13393 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_collisions.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_mask_update.py
+-rw-r--r--   0 root         (0) root         (0)    14826 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     7910 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_update.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_update_virt.py
+-rw-r--r--   0 root         (0) root         (0)     5024 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_autounmask.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_bdeps.py
+-rw-r--r--   0 root         (0) root         (0)     4350 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_complete_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4694 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py
+-rw-r--r--   0 root         (0) root         (0)     4366 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_missed_update.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_required_use.py
+-rw-r--r--   0 root         (0) root         (0)     9190 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_unsolved.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/tests/resolver/test_targetroot.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/tests/resolver/test_unecessary_slot_upgrade.py
+-rw-r--r--   0 root         (0) root         (0)    11321 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/tests/resolver/test_unmerge_order.py
+-rw-r--r--   0 root         (0) root         (0)     3843 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_update.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_use_dep_defaults.py
+-rw-r--r--   0 root         (0) root         (0)     5326 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_useflags.py
+-rw-r--r--   0 root         (0) root         (0)     9976 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_virtual_minimize_children.py
+-rw-r--r--   0 root         (0) root         (0)     9326 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_virtual_slot.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_with_test_deps.py
+-rwxr-xr-x   0 root         (0) root         (0)     2100 2023-03-21 03:50:18.064091 portage-3.0.47/lib/portage/tests/runTests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sets/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sets/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/base/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/sets/base/testInternalPackageSet.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/sets/base/testVariableSet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sets/files/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/files/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/sets/files/testConfigFileSet.py
+-rw-r--r--   0 root         (0) root         (0)      829 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/sets/files/testStaticFileSet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sets/shell/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/shell/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/sets/shell/testShell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sync/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sync/__test__.py
+-rw-r--r--   0 root         (0) root         (0)    16481 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/sync/test_sync_local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/unicode/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/unicode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/unicode/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/unicode/test_string_format.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/update/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.110799 portage-3.0.47/lib/portage/tests/update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.110799 portage-3.0.47/lib/portage/tests/update/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     4462 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/update/test_move_ent.py
+-rw-r--r--   0 root         (0) root         (0)     5444 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/update/test_move_slot_ent.py
+-rw-r--r--   0 root         (0) root         (0)    11460 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/update/test_update_dbentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/
+-rw-r--r--   0 root         (0) root         (0)      170 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/dyn_libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/dyn_libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/dyn_libs/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/dyn_libs/test_soname_deps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/eventloop/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/eventloop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/eventloop/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      826 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/eventloop/test_call_soon_fifo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/file_copy/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/file_copy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/file_copy/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/file_copy/test_copyfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/futures/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/futures/asyncio/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/util/futures/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/util/futures/asyncio/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_child_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py
+-rw-r--r--   0 root         (0) root         (0)      795 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py
+-rw-r--r--   0 root         (0) root         (0)     7135 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/test_compat_coroutine.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/test_done_callback.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/futures/test_done_callback_after_exit.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/test_iter_completed.py
+-rw-r--r--   0 root         (0) root         (0)    10828 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/test_retry.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-03-21 03:50:18.064091 portage-3.0.47/lib/portage/tests/util/test_checksum.py
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_digraph.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_file_copier.py
+-rw-r--r--   0 root         (0) root         (0)     3534 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_getconfig.py
+-rw-r--r--   0 root         (0) root         (0)      315 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/test_grabdict.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_install_mask.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2022-12-24 02:35:49.845990 portage-3.0.47/lib/portage/tests/util/test_manifest.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/util/test_mtimedb.py
+-rw-r--r--   0 root         (0) root         (0)      440 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_normalizedPath.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-09 06:49:46.516103 portage-3.0.47/lib/portage/tests/util/test_shelve.py
+-rw-r--r--   0 root         (0) root         (0)     6638 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_socks5.py
+-rw-r--r--   0 root         (0) root         (0)      832 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/test_stackDictList.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_stackDicts.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_stackLists.py
+-rw-r--r--   0 root         (0) root         (0)      897 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/test_uniqueArray.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_varExpand.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_whirlpool.py
+-rw-r--r--   0 root         (0) root         (0)     6243 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_xattr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/versions/
+-rw-r--r--   0 root         (0) root         (0)      174 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/versions/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/versions/test_cpv_sort_key.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/versions/test_vercmp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/xpak/
+-rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/xpak/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/xpak/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      427 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/xpak/test_decodeint.py
+-rw-r--r--   0 root         (0) root         (0)    17014 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/util/
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/ExtractKernelVersion.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/SlotObject.py
+-rw-r--r--   0 root         (0) root         (0)    68707 2023-03-21 03:50:18.064091 portage-3.0.47/lib/portage/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/_async/
+-rw-r--r--   0 root         (0) root         (0)     2609 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_async/AsyncFunction.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_async/AsyncScheduler.py
+-rw-r--r--   0 root         (0) root         (0)      963 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_async/AsyncTaskFuture.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_async/BuildLogger.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_async/FileCopier.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_async/FileDigester.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/ForkProcess.py
+-rw-r--r--   0 root         (0) root         (0)     7527 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/PipeLogger.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/PipeReaderBlockingIO.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/PopenProcess.py
+-rw-r--r--   0 root         (0) root         (0)     4501 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/SchedulerInterface.py
+-rw-r--r--   0 root         (0) root         (0)      644 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_async/TaskScheduler.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.127466 portage-3.0.47/lib/portage/util/_async/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_async/run_main_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_compare_files.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_ctypes.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_desktop_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/_dyn_libs/
+-rw-r--r--   0 root         (0) root         (0)    41425 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/LinkageMapELF.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_dyn_libs/NeededEntry.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.130799 portage-3.0.47/lib/portage/util/_dyn_libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/display_preserved_libs.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_dyn_libs/dyn_libs.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/soname_deps.py
+-rw-r--r--   0 root         (0) root         (0)     3722 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/soname_deps_qa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/_eventloop/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.134132 portage-3.0.47/lib/portage/util/_eventloop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5849 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_eventloop/asyncio_event_loop.py
+-rw-r--r--   0 root         (0) root         (0)      213 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_eventloop/global_event_loop.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_get_vm_info.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_info_files.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_path.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_pty.py
+-rw-r--r--   0 root         (0) root         (0)     4032 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/util/_urlopen.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_xattr.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/bin_entry_point.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/compression_probe.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/configparser.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2022-12-24 02:35:49.845990 portage-3.0.47/lib/portage/util/cpuinfo.py
+-rw-r--r--   0 root         (0) root         (0)    12975 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/digraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/elf/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.137466 portage-3.0.47/lib/portage/util/elf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/elf/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/elf/header.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/endian/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.137466 portage-3.0.47/lib/portage/util/endian/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/endian/decode.py
+-rw-r--r--   0 root         (0) root         (0)    15592 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/env_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/file_copy/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/file_copy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/formatter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/futures/
+-rw-r--r--   0 root         (0) root         (0)      180 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/futures/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/futures/_asyncio/
+-rw-r--r--   0 root         (0) root         (0)     9758 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/futures/_asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/futures/_asyncio/streams.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/futures/_sync_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/compat_coroutine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/futures/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.140799 portage-3.0.47/lib/portage/util/futures/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/executor/fork.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/extendedfutures.py
+-rw-r--r--   0 root         (0) root         (0)      516 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/futures/futures.py
+-rw-r--r--   0 root         (0) root         (0)     6868 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/iter_completed.py
+-rw-r--r--   0 root         (0) root         (0)     6297 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/futures/retry.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/unix_events.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     6549 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/util/install_mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/iterators/
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/iterators/MultiIterGroupBy.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.144132 portage-3.0.47/lib/portage/util/iterators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7349 2022-09-10 09:45:01.063717 portage-3.0.47/lib/portage/util/lafilefixer.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/listdir.py
+-rw-r--r--   0 root         (0) root         (0)     4339 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/locale.py
+-rw-r--r--   0 root         (0) root         (0)    13909 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/movefile.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/mtimedb.py
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/netlink.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/util/shelve.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/socks5.py
+-rw-r--r--   0 root         (0) root         (0)    58416 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/whirlpool.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/writeable_check.py
+-rw-r--r--   0 root         (0) root         (0)    19275 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/xml/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.147466 portage-3.0.47/lib/portage/xml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16789 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/xml/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    19413 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/xpak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/misc/
+-rwxr-xr-x   0 root         (0) root         (0)    24116 2023-02-03 18:03:13.736861 portage-3.0.47/misc/emerge-delta-webrsync
+-rwxr-xr-x   0 root         (0) root         (0)    29953 2023-04-30 04:10:22.598516 portage-3.0.47/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/src/
+-rw-r--r--   0 root         (0) root         (0)    71291 2023-03-21 03:35:23.556871 portage-3.0.47/src/portage_util__whirlpool.c
+-rw-r--r--   0 root         (0) root         (0)    13384 2023-03-21 03:35:23.556871 portage-3.0.47/src/portage_util_file_copy_reflink_linux.c
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-03-21 03:35:23.556871 portage-3.0.47/src/portage_util_libc.c
```

### Comparing `portage-3.0.46/DEVELOPING` & `portage-3.0.47/DEVELOPING`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/LICENSE` & `portage-3.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/PKG-INFO` & `portage-3.0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portage
-Version: 3.0.46
+Version: 3.0.47
 Summary: Portage is the package management and distribution system for Gentoo
 Home-page: https://wiki.gentoo.org/wiki/Project:Portage
 Author: Gentoo Portage Development Team
 Author-email: dev-portage@gentoo.org
 License: GPLV2
 Project-URL: Release Notes, https://gitweb.gentoo.org/proj/portage.git/plain/NEWS
 Project-URL: Documentation, https://wiki.gentoo.org/wiki/Handbook:AMD64/Working/Portage
```

### Comparing `portage-3.0.46/TEST-NOTES` & `portage-3.0.47/TEST-NOTES`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/archive-conf` & `portage-3.0.47/bin/archive-conf`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/bashrc-functions.sh` & `portage-3.0.47/bin/bashrc-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/binhost-snapshot` & `portage-3.0.47/bin/binhost-snapshot`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/chmod-lite.py` & `portage-3.0.47/bin/chmod-lite.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/chpathtool.py` & `portage-3.0.47/bin/chpathtool.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/clean_locks` & `portage-3.0.47/bin/clean_locks`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/dispatch-conf` & `portage-3.0.47/bin/dispatch-conf`

 * *Files 0% similar despite different names*

```diff
@@ -115,16 +115,17 @@
 
         if "log-file" in self.options:
             if os.path.isfile(self.options["log-file"]):
                 shutil.copy(self.options["log-file"], self.options["log-file"] + ".old")
             if os.path.isfile(self.options["log-file"]) or not os.path.exists(
                 self.options["log-file"]
             ):
+                old_umask = os.umask(0o077)
                 open(self.options["log-file"], "w").close()  # Truncate it
-                os.chmod(self.options["log-file"], 0o600)
+                os.umask(old_umask)
 
         pager = self.options.get("pager")
         if pager is None or not cmd_var_is_valid(pager):
             pager = os.environ.get("PAGER")
             if pager is None or not cmd_var_is_valid(pager):
                 pager = "cat"
```

### Comparing `portage-3.0.46/bin/dohtml.py` & `portage-3.0.47/bin/dohtml.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,16 +148,16 @@
                 self.PF = normalize_path(self.PF)
         if os.environ.get("EAPI", "0") in ("0", "1", "2"):
             self.ED = os.environ.get("D", "")
         else:
             self.ED = os.environ.get("ED", "")
         if self.ED:
             self.ED = normalize_path(self.ED)
-        if "_E_DOCDESTTREE_" in os.environ:
-            self.DOCDESTTREE = os.environ["_E_DOCDESTTREE_"]
+        if "__E_DOCDESTTREE" in os.environ:
+            self.DOCDESTTREE = os.environ["__E_DOCDESTTREE"]
             if self.DOCDESTTREE:
                 self.DOCDESTTREE = normalize_path(self.DOCDESTTREE)
 
         self.allowed_exts = ["css", "gif", "htm", "html", "jpeg", "jpg", "js", "png"]
         self.allowed_files = []
         self.disallowed_dirs = ["CVS"]
         self.recurse = False
```

### Comparing `portage-3.0.46/bin/doins.py` & `portage-3.0.47/bin/doins.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/eapi.sh` & `portage-3.0.47/bin/eapi.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/eapi7-ver-funcs.sh` & `portage-3.0.47/bin/eapi7-ver-funcs.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild` & `portage-3.0.47/bin/ebuild`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/bsd/sed` & `portage-3.0.47/bin/ebuild-helpers/bsd/sed`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/dobin` & `portage-3.0.47/bin/ebuild-helpers/dobin`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2018 Gentoo Foundation
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if [[ $# -lt 1 ]] ; then
 	__helpers_die "${0##*/}: at least one argument needed"
 	exit 1
@@ -14,26 +14,26 @@
 fi
 
 if ! ___eapi_has_DESTTREE_INSDESTTREE; then
 	[[ -n ${DESTTREE} ]] &&
 		die "${0##*/}: \${DESTTREE} has been banned for EAPI '${EAPI}'; use 'into' instead"
 else
 	# backwards compatibility
-	_E_DESTTREE_=${DESTTREE}
+	__E_DESTTREE=${DESTTREE}
 fi
 
-if [[ ! -d ${ED%/}/${_E_DESTTREE_#/}/bin ]] ; then
-	install -d "${ED%/}/${_E_DESTTREE_#/}/bin" || { __helpers_die "${0##*/}: failed to install ${ED%/}/${_E_DESTTREE_#/}/bin"; exit 2; }
+if [[ ! -d ${ED%/}/${__E_DESTTREE#/}/bin ]] ; then
+	install -d "${ED%/}/${__E_DESTTREE#/}/bin" || { __helpers_die "${0##*/}: failed to install ${ED%/}/${__E_DESTTREE#/}/bin"; exit 2; }
 fi
 
 ret=0
 
 for x in "$@" ; do
 	if [[ -e ${x} ]] ; then
-		install -m0755 -o ${PORTAGE_INST_UID:-0} -g ${PORTAGE_INST_GID:-0} "${x}" "${ED%/}/${_E_DESTTREE_#/}/bin"
+		install -m0755 -o ${PORTAGE_INST_UID:-0} -g ${PORTAGE_INST_GID:-0} "${x}" "${ED%/}/${__E_DESTTREE#/}/bin"
 	else
 		echo "!!! ${0##*/}: ${x} does not exist" 1>&2
 		false
 	fi
 	((ret|=$?))
 done
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/doconfd` & `portage-3.0.47/bin/ebuild-helpers/doconfd`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env bash
-# Copyright 1999-2021 Gentoo Authors
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if [[ $# -lt 1 ]] ; then
 	__helpers_die "${0##*/}: at least one argument needed"
 	exit 1
 fi
 
-export _E_INSDESTTREE_='/etc/conf.d/'
+export __E_INSDESTTREE='/etc/conf.d/'
 if ___eapi_has_DESTTREE_INSDESTTREE; then
-	export INSDESTTREE=${_E_INSDESTTREE_}
+	export INSDESTTREE=${__E_INSDESTTREE}
 fi
 
 if ! ___eapi_doconfd_respects_insopts; then
 	export INSOPTIONS=-m0644
 	export DIROPTIONS=""
 fi
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/dodoc` & `portage-3.0.47/bin/ebuild-helpers/dodoc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2018 Gentoo Foundation
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if ___eapi_dodoc_supports_-r; then
 	__PORTAGE_HELPER='dodoc' exec doins "$@"
 fi
@@ -13,15 +13,15 @@
 	exit 1
 fi
 
 if ! ___eapi_has_prefix_variables; then
 	ED=${D}
 fi
 
-dir="${ED%/}/usr/share/doc/${PF}/${_E_DOCDESTTREE_#/}"
+dir="${ED%/}/usr/share/doc/${PF}/${__E_DOCDESTTREE#/}"
 if [ ! -d "${dir}" ] ; then
 	install -d "${dir}"
 fi
 
 ret=0
 for x in "$@" ; do
 	if [ -d "${x}" ] ; then
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/doenvd` & `portage-3.0.47/bin/ebuild-helpers/doenvd`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env bash
-# Copyright 1999-2021 Gentoo Authors
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if [[ $# -lt 1 ]] ; then
 	__helpers_die "${0##*/}: at least one argument needed"
 	exit 1
 fi
 
-export _E_INSDESTTREE_='/etc/env.d/'
+export __E_INSDESTTREE='/etc/env.d/'
 if ___eapi_has_DESTTREE_INSDESTTREE; then
-	export INSDESTTREE=${_E_INSDESTTREE_}
+	export INSDESTTREE=${__E_INSDESTTREE}
 fi
 
 if ! ___eapi_doenvd_respects_insopts; then
 	export INSOPTIONS=-m0644
 	export DIROPTIONS=""
 fi
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/doexe` & `portage-3.0.47/bin/ebuild-helpers/doexe`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env bash
-# Copyright 1999-2018 Gentoo Foundation
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if [[ $# -lt 1 ]] ; then
 	__helpers_die "${0##*/}: at least one argument needed"
 	exit 1
 fi
 
 if ! ___eapi_has_prefix_variables; then
 	ED=${D}
 fi
 
-if [[ ! -d ${ED%/}/${_E_EXEDESTTREE_#/} ]] ; then
-	install -d "${ED%/}/${_E_EXEDESTTREE_#/}"
+if [[ ! -d ${ED%/}/${__E_EXEDESTTREE#/} ]] ; then
+	install -d "${ED%/}/${__E_EXEDESTTREE#/}"
 fi
 
 TMP=$(mktemp -d "${T}/.doexe_tmp_XXXXXX")
 
 ret=0
 
 for x in "$@" ; do
@@ -29,15 +29,15 @@
 		__vecho "doexe: warning, skipping directory ${x}"
 		continue
 	else
 		mysrc="${x}"
 	fi
 
 	if [ -e "${mysrc}" ] ; then
-		install ${EXEOPTIONS} "${mysrc}" "${ED%/}/${_E_EXEDESTTREE_#/}"
+		install ${EXEOPTIONS} "${mysrc}" "${ED%/}/${__E_EXEDESTTREE#/}"
 	else
 		echo "!!! ${0##*/}: ${mysrc} does not exist" 1>&2
 		false
 	fi
 	((ret|=$?))
 done
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/dohard` & `portage-3.0.47/bin/ebuild-helpers/dohard`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/doheader` & `portage-3.0.47/bin/ebuild-helpers/doheader`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env bash
-# Copyright 1999-2021 Gentoo Authors
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if ! ___eapi_has_doheader; then
 	die "${0##*/} is not supported in EAPI ${EAPI}"
 fi
 
 if [[ $# -lt 1 ]] || [[ $1 == -r && $# -lt 2 ]] ; then
 	__helpers_die "${0##*/}: at least one argument needed"
 	exit 1
 fi
 
-export _E_INSDESTTREE_='/usr/include/'
+export __E_INSDESTTREE='/usr/include/'
 if ___eapi_has_DESTTREE_INSDESTTREE; then
-	export INSDESTTREE=${_E_INSDESTTREE_}
+	export INSDESTTREE=${__E_INSDESTTREE}
 fi
 
 if ! ___eapi_doheader_respects_insopts; then
 	export INSOPTIONS=-m0644
 	export DIROPTIONS=""
 fi
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/dohtml` & `portage-3.0.47/bin/ebuild-helpers/dohtml`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/doinfo` & `portage-3.0.47/bin/ebuild-helpers/doinfo`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/doins` & `portage-3.0.47/bin/ebuild-helpers/doins`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2019 Gentoo Authors
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 helper=${__PORTAGE_HELPER:-${0##*/}}
 
 if [[ ${helper} == dodoc ]] ; then
@@ -12,22 +12,22 @@
 		# when DOC is defined but empty, so simply return
 		# sucessfully in this case.
 		eqawarn "QA Notice: dodoc called with no arguments"
 		exit 0
 	fi
 	export INSOPTIONS=-m0644
 	export DIROPTIONS=""
-	export _E_INSDESTTREE_=usr/share/doc/${PF}/${_E_DOCDESTTREE_}
+	export __E_INSDESTTREE=usr/share/doc/${PF}/${__E_DOCDESTTREE}
 else
 	if ! ___eapi_has_DESTTREE_INSDESTTREE; then
 		[[ -n ${INSDESTTREE} ]] &&
 			die "${0##*/}: \${INSDESTTREE} has been banned for EAPI '${EAPI}'; use 'into' instead"
 	else
 		# backwards compatibility
-		_E_INSDESTTREE_=${INSDESTTREE}
+		__E_INSDESTTREE=${INSDESTTREE}
 	fi
 fi
 
 if [ $# -lt 1 ] ; then
 	__helpers_die "${helper}: at least one argument needed"
 	exit 1
 fi
@@ -38,28 +38,28 @@
 	shift
 fi
 
 if ! ___eapi_has_prefix_variables; then
 	export ED="${D}"
 fi
 
-if [[ ${_E_INSDESTTREE_#${D}} != "${_E_INSDESTTREE_}" ]]; then
+if [[ ${__E_INSDESTTREE#${D}} != "${__E_INSDESTTREE}" ]]; then
 	__vecho "-------------------------------------------------------" 1>&2
 	__vecho "You should not use \${D} or \${ED} with helpers." 1>&2
-	__vecho "  --> ${_E_INSDESTTREE_}" 1>&2
+	__vecho "  --> ${__E_INSDESTTREE}" 1>&2
 	__vecho "-------------------------------------------------------" 1>&2
 	__helpers_die "${helper} used with \${D} or \${ED}"
 	exit 1
 fi
 if [[ -n ${EPREFIX} && \
-		${_E_INSDESTTREE_#${EPREFIX}} != "${_E_INSDESTTREE_}" ]]
+		${__E_INSDESTTREE#${EPREFIX}} != "${__E_INSDESTTREE}" ]]
 then
 	__vecho "-------------------------------------------------------" 1>&2
 	__vecho "You should not use \${EPREFIX} with helpers." 1>&2
-	__vecho "  --> ${_E_INSDESTTREE_}" 1>&2
+	__vecho "  --> ${__E_INSDESTTREE}" 1>&2
 	__vecho "-------------------------------------------------------" 1>&2
 	__helpers_die "${helper} used with \${EPREFIX}"
 	exit 1
 fi
 
 if ___eapi_doins_and_newins_preserve_symlinks; then
 	DOINS_ARGS+=( --preserve_symlinks )
@@ -90,15 +90,15 @@
 		--enable_copy_xattr
 		"--xattr_exclude=${PORTAGE_XATTR_EXCLUDE}"
 	)
 fi
 
 DOINS_ARGS+=(
 	"--helper=${helper}"
-	"--dest=${ED%/}/${_E_INSDESTTREE_#/}"
+	"--dest=${ED%/}/${__E_INSDESTTREE#/}"
 )
 
 # Explicitly set PYTHONPATH to non empty.
 # If PYTHONPATH is empty (not unset), it means "add current working directory
 # to the import path" if the Python is prior to 3.4, which would cause
 # unexpected import. See also #469338.
 PYTHONPATH=${PORTAGE_PYTHONPATH:-${PORTAGE_PYM_PATH}} \
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/dolib` & `portage-3.0.47/bin/ebuild-helpers/dolib`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2018 Gentoo Foundation
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if [[ -z ${PORTAGE_INTERNAL_DOLIB} ]] && ! ___eapi_has_dolib_libopts; then
 	die "'${0##*/}' has been banned for EAPI '${EAPI}'"
 	exit 1
@@ -14,27 +14,27 @@
 fi
 
 if ! ___eapi_has_DESTTREE_INSDESTTREE; then
 	[[ -n ${DESTTREE} ]] &&
 		die "${0##*/}: \${DESTTREE} has been banned for EAPI '${EAPI}'; use 'into' instead"
 else
 	# backwards compatibility
-	_E_DESTTREE_=${DESTTREE}
+	__E_DESTTREE=${DESTTREE}
 fi
 
 # Setup ABI cruft
 LIBDIR_VAR="LIBDIR_${ABI}"
 if [[ -n ${ABI} && -n ${!LIBDIR_VAR} ]] ; then
 	CONF_LIBDIR=${!LIBDIR_VAR}
 fi
 unset LIBDIR_VAR
 
 # We need this to default to lib so that things dont break
 CONF_LIBDIR=${CONF_LIBDIR:-lib}
-libdir="${ED%/}/${_E_DESTTREE_#/}/${CONF_LIBDIR}"
+libdir="${ED%/}/${__E_DESTTREE#/}/${CONF_LIBDIR}"
 
 if [[ $# -lt 1 ]] ; then
 	__helpers_die "${0##*/}: at least one argument needed"
 	exit 1
 fi
 if [[ ! -d ${libdir} ]] ; then
 	install -d "${libdir}" || { __helpers_die "${0##*/}: failed to install ${libdir}"; exit 1; }
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/doman` & `portage-3.0.47/bin/ebuild-helpers/doman`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/domo` & `portage-3.0.47/bin/ebuild-helpers/domo`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2018 Gentoo Foundation
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 mynum=${#}
 if [ ${mynum} -lt 1 ] ; then
 	__helpers_die "${0}: at least one argument needed"
@@ -15,32 +15,32 @@
 fi
 
 if ! ___eapi_has_DESTTREE_INSDESTTREE; then
 	[[ -n ${DESTTREE} ]] &&
 		die "${0##*/}: \${DESTTREE} has been banned for EAPI '${EAPI}'; use 'into' instead"
 else
 	# backwards compatibility
-	_E_DESTTREE_=${DESTTREE}
+	__E_DESTTREE=${DESTTREE}
 fi
 
 # newer EAPIs force /usr consistently with other /usr/share helpers
 if ! ___eapi_domo_respects_into; then
-	_E_DESTTREE_=/usr
+	__E_DESTTREE=/usr
 fi
 
-if [ ! -d "${ED%/}/${_E_DESTTREE_#/}/share/locale" ] ; then
-	install -d "${ED%/}/${_E_DESTTREE_#/}/share/locale/"
+if [ ! -d "${ED%/}/${__E_DESTTREE#/}/share/locale" ] ; then
+	install -d "${ED%/}/${__E_DESTTREE#/}/share/locale/"
 fi
 
 ret=0
 
 for x in "$@" ; do
 	if [ -e "${x}" ] ; then
 		mytiny="${x##*/}"
-		mydir="${ED%/}/${_E_DESTTREE_#/}/share/locale/${mytiny%.*}/LC_MESSAGES"
+		mydir="${ED%/}/${__E_DESTTREE#/}/share/locale/${mytiny%.*}/LC_MESSAGES"
 		if [ ! -d "${mydir}" ] ; then
 			install -d "${mydir}"
 		fi
 		install -m0644 "${x}" "${mydir}/${MOPREFIX}.mo"
 	else
 		echo "!!! ${0##*/}: ${x} does not exist" 1>&2
 		false
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/dosbin` & `portage-3.0.47/bin/ebuild-helpers/dosbin`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2018 Gentoo Foundation
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if [[ $# -lt 1 ]] ; then
 	__helpers_die "${0##*/}: at least one argument needed"
 	exit 1
@@ -14,26 +14,26 @@
 fi
 
 if ! ___eapi_has_DESTTREE_INSDESTTREE; then
 	[[ -n ${DESTTREE} ]] &&
 		die "${0##*/}: \${DESTTREE} has been banned for EAPI '${EAPI}'; use 'into' instead"
 else
 	# backwards compatibility
-	_E_DESTTREE_=${DESTTREE}
+	__E_DESTTREE=${DESTTREE}
 fi
 
-if [[ ! -d ${ED%/}/${_E_DESTTREE_#/}/sbin ]] ; then
-	install -d "${ED%/}/${_E_DESTTREE_#/}/sbin" || { __helpers_die "${0##*/}: failed to install ${ED%/}/${_E_DESTTREE_#/}/sbin"; exit 2; }
+if [[ ! -d ${ED%/}/${__E_DESTTREE#/}/sbin ]] ; then
+	install -d "${ED%/}/${__E_DESTTREE#/}/sbin" || { __helpers_die "${0##*/}: failed to install ${ED%/}/${__E_DESTTREE#/}/sbin"; exit 2; }
 fi
 
 ret=0
 
 for x in "$@" ; do
 	if [[ -e ${x} ]] ; then
-		install -m0755 -o ${PORTAGE_INST_UID:-0} -g ${PORTAGE_INST_GID:-0} "${x}" "${ED%/}/${_E_DESTTREE_#/}/sbin"
+		install -m0755 -o ${PORTAGE_INST_UID:-0} -g ${PORTAGE_INST_GID:-0} "${x}" "${ED%/}/${__E_DESTTREE#/}/sbin"
 	else
 		echo "!!! ${0##*/}: ${x} does not exist" 1>&2
 		false
 	fi
 	((ret|=$?))
 done
```

### Comparing `portage-3.0.46/bin/ebuild-helpers/dosed` & `portage-3.0.47/bin/ebuild-helpers/dosed`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/dosym` & `portage-3.0.47/bin/ebuild-helpers/dosym`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/emake` & `portage-3.0.47/bin/ebuild-helpers/emake`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/fowners` & `portage-3.0.47/bin/ebuild-helpers/fowners`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/fperms` & `portage-3.0.47/bin/ebuild-helpers/fperms`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/newins` & `portage-3.0.47/bin/ebuild-helpers/newins`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/portageq` & `portage-3.0.47/bin/ebuild-helpers/portageq`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/prepinfo` & `portage-3.0.47/bin/ebuild-helpers/prepinfo`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/unprivileged/chown` & `portage-3.0.47/bin/ebuild-helpers/unprivileged/chown`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-helpers/xattr/install` & `portage-3.0.47/bin/ebuild-helpers/xattr/install`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-ipc.py` & `portage-3.0.47/bin/ebuild-ipc.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild-pyhelper` & `portage-3.0.47/bin/ebuild-pyhelper`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ebuild.sh` & `portage-3.0.47/bin/ebuild.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ecompress` & `portage-3.0.47/bin/ecompress`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/ecompress-file` & `portage-3.0.47/bin/ecompress-file`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/egencache` & `portage-3.0.47/bin/egencache`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/emaint` & `portage-3.0.47/bin/emaint`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/emerge` & `portage-3.0.47/bin/emerge`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/emerge-webrsync` & `portage-3.0.47/bin/emerge-webrsync`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2014 Gentoo Foundation
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 # Author: Karl Trygve Kalleberg <karltk@gentoo.org>
 # Rewritten from the old, Perl-based emerge-webrsync script
 # Author: Alon Bar-Lev <alon.barlev@gmail.com>
 # Major rewrite from Karl's scripts.
 
 # TODO:
@@ -20,35 +20,70 @@
 # Alternative (legacy) PORTAGE_GPG_DIR configuration:
 # gpg key import
 # KEY_ID=0x96D8BF6D
 # gpg --homedir /etc/portage/gnupg --keyserver subkeys.pgp.net --recv-keys ${KEY_ID}
 # gpg --homedir /etc/portage/gnupg --edit-key ${KEY_ID} trust
 #
 
-# Only echo if in verbose mode
-vvecho() { [[ ${do_verbose} -eq 1 ]] && echo "$@" ; }
-# Only echo if not in verbose mode
-nvecho() { [[ ${do_verbose} -eq 0 ]] && echo "$@" ; }
-# warning echos
-wecho() { echo "${argv0##*/}: warning: $*" 1>&2 ; }
-# error echos
-eecho() { echo "${argv0##*/}: error: $*" 1>&2 ; }
+# Opportunistically use gentoo-functions for nicer output
+functions_script="${EPREFIX:-/}/lib/gentoo/functions.sh"
+source "${functions_script}" || {
+	echo "${argv0}: Could not source ${functions_script}!" 1>&2
+
+	ebegin() {
+		printf '%s*%s %s ... ' "${GOOD}" "${NORMAL}" "$*"
+	}
+
+	eend() {
+		local r=${1:-0}
+		shift
+		if [[ $r -eq 0 ]] ; then
+			printf '[ %sok%s ]\n' "${GOOD}" "${NORMAL}"
+		else
+			printf '%s [ %s!!%s ]\n' "$*" "${BAD}" "${NORMAL}"
+		fi
+		return "${r}"
+	}
+
+	einfo() {
+		echo "${argv0##*/}: $*"
+	}
+
+	ewarn() {
+		echo "${argv0##*/}: warning: $*" 1>&2
+	}
+
+	eerror() {
+		echo "${argv0##*/}: error: $*" 1>&2
+	}
+
+}
+
+# Only echo if in normal mode
+vvecho() { [[ ${PORTAGE_QUIET} != 1 ]] && echo "$@" ; }
+# Only echo if in quiet mode
+nvecho() { [[ ${PORTAGE_QUIET} == 1 ]] && echo "$@" ; }
+
+# Unfortunately, gentoo-functions doesn't yet have a die() (bug #878505)
+die() {
+	eerror "$@"
+	exit 1
+}
 
 argv0=$0
 
 # Use portageq from the same directory/prefix as the current script, so
 # that we don't have to rely on PATH including the current EPREFIX.
 scriptpath=${BASH_SOURCE[0]}
-if [ -x "${scriptpath%/*}/portageq" ]; then
+if [[ -x "${scriptpath%/*}/portageq" ]]; then
 	portageq=${scriptpath%/*}/portageq
 elif type -P portageq > /dev/null ; then
 	portageq=portageq
 else
-	eecho "could not find 'portageq'; aborting"
-	exit 1
+	die "could not find 'portageq'; aborting"
 fi
 
 eval "$("${portageq}" envvar -v DISTDIR EPREFIX FEATURES \
 	FETCHCOMMAND GENTOO_MIRRORS \
 	PORTAGE_BIN_PATH PORTAGE_CONFIGROOT PORTAGE_GPG_DIR \
 	PORTAGE_NICENESS PORTAGE_REPOSITORIES PORTAGE_RSYNC_EXTRA_OPTS \
 	PORTAGE_RSYNC_OPTS PORTAGE_TEMP_GPG_DIR PORTAGE_TMPDIR \
@@ -56,61 +91,82 @@
 export http_proxy ftp_proxy
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 repo_name=gentoo
 repo_location=$(__repo_attr "${repo_name}" location)
 if [[ -z ${repo_location} ]]; then
-	eecho "Repository '${repo_name}' not found"
-	exit 1
+	die "Repository '${repo_name}' not found"
 fi
 repo_sync_type=$(__repo_attr "${repo_name}" sync-type)
 
 # If PORTAGE_NICENESS is overriden via the env then it will
 # still pass through the portageq call and override properly.
-if [ -n "${PORTAGE_NICENESS}" ]; then
-	renice ${PORTAGE_NICENESS} $$ > /dev/null
+if [[ -n "${PORTAGE_NICENESS}" ]]; then
+	renice "${PORTAGE_NICENESS}" $$ > /dev/null
 fi
 
-do_verbose=0
 do_debug=0
 keep=false
 
-has webrsync-gpg ${FEATURES} && webrsync_gpg=1 || webrsync_gpg=0
-
-if [[ ${webrsync_gpg} -eq 1 ]]; then
-	wecho "FEATURES=webrsync-gpg is deprecated, see the make.conf(5) man page."
-fi
+handle_pgp_setup() {
+	has webrsync-gpg ${FEATURES} && webrsync_gpg=1 || webrsync_gpg=0
 
-if [[ -n ${PORTAGE_TEMP_GPG_DIR} ]] ||
-	has $(__repo_attr "${repo_name}" sync-webrsync-verify-signature |
-	LC_ALL=C tr '[:upper:]' '[:lower:]') true yes; then
-
-	# If FEATURES=webrsync-gpg is enabled then allow direct emerge-webrsync
-	# calls for backward compatibility (this triggers a deprecation warning
-	# above). Since direct emerge-webrsync calls do not use gemato for secure
-	# key refresh, this behavior will not be supported in a future release.
-	if [[ ! ( -d ${PORTAGE_GPG_DIR} && ${webrsync_gpg} -eq 1 ) &&
-		-z ${PORTAGE_TEMP_GPG_DIR} ]]; then
-		eecho "Do not call ${argv0##*/} directly, instead call emerge --sync or emaint sync."
-		exit 1
+	if [[ ${webrsync_gpg} -eq 1 ]]; then
+		ewarn "FEATURES=webrsync-gpg is deprecated, see the make.conf(5) man page."
 	fi
 
-	WEBSYNC_VERIFY_SIGNATURE=1
-elif has webrsync-gpg ${FEATURES}; then
-	WEBSYNC_VERIFY_SIGNATURE=1
-else
-	WEBSYNC_VERIFY_SIGNATURE=0
-fi
+	repo_has_webrsync_verify=$(
+		has $(__repo_attr "${repo_name}" sync-webrsync-verify-signature	| LC_ALL=C tr '[:upper:]' '[:lower:]') true yes
+	)
+
+	# WEBRSYNC_VERIFY_SIGNATURE=0: disable PGP verification
+	# WEBRSYNC_VERIFY_SIGNATURE=1: use gemato for verification, fallback to regular gpg
+	# WEBRSYNC_VERIFY_SIGNATURE=2: use legacy FEATURES="webrsync-gpg"
+	WEBRSYNC_VERIFY_SIGNATURE=1
+
+	if [[ -n ${PORTAGE_TEMP_GPG_DIR} ]] || [[ ${repo_has_webrsync_verify} -eq 1 ]]; then
+		# If FEATURES=webrsync-gpg is enabled then allow direct emerge-webrsync
+		# calls for backward compatibility (this triggers a deprecation warning
+		# above). Since direct emerge-webrsync calls do not use gemato for secure
+		# key refresh, this behavior will not be supported in a future release.
+		if [[ ! ( -d ${PORTAGE_GPG_DIR} && ${webrsync_gpg} -eq 1 ) && -z ${PORTAGE_TEMP_GPG_DIR} ]]; then
+			die "Do not call ${argv0##*/} directly, instead call emerge --sync or emaint sync."
+		fi
 
-[[ -n ${PORTAGE_TEMP_GPG_DIR} ]] && PORTAGE_GPG_DIR=${PORTAGE_TEMP_GPG_DIR}
-if [ ${WEBSYNC_VERIFY_SIGNATURE} != 0 -a -z "${PORTAGE_GPG_DIR}" ]; then
-	eecho "please set PORTAGE_GPG_DIR in make.conf"
-	exit 1
-fi
+		WEBRSYNC_VERIFY_SIGNATURE=2
+	elif has webrsync-gpg ${FEATURES}; then
+		WEBRSYNC_VERIFY_SIGNATURE=2
+	elif [[ -n ${no_pgp_verify} ]]; then
+		WEBRSYNC_VERIFY_SIGNATURE=0
+	fi
+
+	case "${WEBRSYNC_VERIFY_SIGNATURE}" in
+		0)
+			[[ ${PORTAGE_QUIET} -eq 1 ]] || ewarn "PGP verification method: disabled"
+			;;
+		1)
+			[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "PGP verification method: gemato"
+			;;
+		2)
+			ewarn "PGP verification method: legacy FEATURES=webrsync-gpg"
+			;;
+		*)
+			die "Unknown WEBRSYNC_VERIFY_SIGNATURE state: \${WEBRSYNC_VERIFY_SIGNATURE}=${WEBRSYNC_VERIFY_SIGNATURE}"
+			;;
+	esac
+
+	if [[ -n ${PORTAGE_TEMP_GPG_DIR} ]]; then
+		PORTAGE_GPG_DIR=${PORTAGE_TEMP_GPG_DIR}
+	fi
+
+	if [[ ${WEBRSYNC_VERIFY_SIGNATURE} == 2 && -z "${PORTAGE_GPG_DIR}" ]]; then
+		die "Please set PORTAGE_GPG_DIR in make.conf!"
+	fi
+}
 
 do_tar() {
 	local file=$1
 	shift
 	local decompressor
 
 	case ${file} in
@@ -129,17 +185,17 @@
 }
 
 get_date_part() {
 	local utc_time_in_secs="$1"
 	local part="$2"
 
 	if [[ ${USERLAND} == BSD ]] ; then
-		date -r ${utc_time_in_secs} -u +"${part}"
+		date -r "${utc_time_in_secs}" -u +"${part}"
 	else
-		date -d @${utc_time_in_secs} -u +"${part}"
+		date -d "@${utc_time_in_secs}" -u +"${part}"
 	fi
 }
 
 get_utc_second_from_string() {
 	local s="$1"
 
 	if [[ ${USERLAND} == BSD ]] ; then
@@ -147,38 +203,38 @@
 		# digits are inherited from the current system clock time.
 		date -juf "%Y%m%d%H%M.%S" "${s}0000.00" +"%s"
 	else
 		date -d "${s:0:4}-${s:4:2}-${s:6:2}" -u +"%s"
 	fi
 }
 
-get_portage_timestamp() {
+get_repository_timestamp() {
 	local portage_current_timestamp=0
 
-	if [ -f "${repo_location}/metadata/timestamp.x" ]; then
+	if [[ -f "${repo_location}/metadata/timestamp.x" ]]; then
 		portage_current_timestamp=$(cut -f 1 -d " " "${repo_location}/metadata/timestamp.x" )
 	fi
 
 	echo "${portage_current_timestamp}"
 }
 
 fetch_file() {
 	local URI="$1"
 	local FILE="$2"
 	local opts
 
-	if [ "${FETCHCOMMAND/wget/}" != "${FETCHCOMMAND}" ]; then
+	if [[ "${FETCHCOMMAND/wget/}" != "${FETCHCOMMAND}" ]]; then
 		opts="--continue $(nvecho -q)"
-	elif [ "${FETCHCOMMAND/curl/}" != "${FETCHCOMMAND}" ]; then
+	elif [[ "${FETCHCOMMAND/curl/}" != "${FETCHCOMMAND}" ]]; then
 		opts="--continue-at - $(nvecho -s -f)"
 	else
 		rm -f "${DISTDIR}/${FILE}"
 	fi
 
-	__vecho "Fetching file ${FILE} ..."
+	[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "Fetching file ${FILE} ..."
 	# Already set DISTDIR=
 	eval "${FETCHCOMMAND} ${opts}"
 
 	if [[ $? -eq 0 && -s ${DISTDIR}/${FILE} ]] ; then
 		return 0
 	else
 		rm -f "${DISTDIR}/${FILE}"
@@ -187,60 +243,102 @@
 }
 
 check_file_digest() {
 	local digest="$1"
 	local file="$2"
 	local r=1
 
-	__vecho "Checking digest ..."
+	[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "Checking digest ..."
 
 	if type -P md5sum > /dev/null; then
 		local md5sum_output=$(md5sum "${file}")
 		local digest_content=$(< "${digest}")
-		[ "${md5sum_output%%[[:space:]]*}" = "${digest_content%%[[:space:]]*}" ] && r=0
+		[[ "${md5sum_output%%[[:space:]]*}" = "${digest_content%%[[:space:]]*}" ]] && r=0
 	elif type -P md5 > /dev/null; then
-		[ "$(md5 -q "${file}")" == "$(cut -d ' ' -f 1 "${digest}")" ] && r=0
+		[[ "$(md5 -q "${file}")" == "$(cut -d ' ' -f 1 "${digest}")" ]] && r=0
 	else
-		eecho "cannot check digest: no suitable md5/md5sum binaries found"
+		die "cannot check digest: no suitable md5/md5sum binaries found"
 	fi
 
 	return "${r}"
 }
 
-check_file_signature() {
+check_file_signature_gemato() {
 	local signature="$1"
 	local file="$2"
 	local r=1
-	local gnupg_status line
 
-	if [ ${WEBSYNC_VERIFY_SIGNATURE} != 0 ]; then
-		__vecho "Checking signature ..."
+	if type -P gemato > /dev/null; then
+		local gemato_args=(
+			openpgp-verify-detached
+			-K /usr/share/openpgp-keys/gentoo-release.asc
+		)
+
+		[[ ${PORTAGE_QUIET} == 1 ]] && gemato_args+=( --quiet )
+		[[ ${do_debug} == 1 ]] && gemato_args+=( --debug )
+
+		gemato "${gemato_args[@]}" "${signature}" "${file}"
+		r=$?
+
+		if [[ ${r} -ne 0 ]]; then
+			# Exit early since it's typically inappropriate to
+			# try other mirrors in this case (it may indicate
+			# a keyring problem).
+			die "signature verification failed"
+		fi
+	fi
 
-		if type -P gpg > /dev/null; then
-			if gnupg_status=$(gpg --homedir "${PORTAGE_GPG_DIR}" --batch \
-				--status-fd 1 --verify "${signature}" "${file}"); then
-				while read -r line; do
-					if [[ ${line} == "[GNUPG:] GOODSIG"* ]]; then
-						r=0
-						break
-					fi
-				done <<< "${gnupg_status}"
-			fi
+	return "${r}"
+}
 
-			if [[ ${r} -ne 0 ]]; then
-				# Exit early since it's typically inappropriate to
-				# try other mirrors in this case (it may indicate
-				# a keyring problem).
-				eecho "signature verification failed"
-				exit 1
-			fi
-		else
-			eecho "cannot check signature: gpg binary not found"
-			exit 1
+check_file_signature_gpg_unwrapped() {
+	local signature="$1"
+	local file="$2"
+
+	if type -P gpg > /dev/null; then
+		if gnupg_status=$(gpg --homedir "${PORTAGE_GPG_DIR}" --batch \
+			--status-fd 1 --verify "${signature}" "${file}"); then
+			while read -r line; do
+				if [[ ${line} == "[GNUPG:] GOODSIG"* ]]; then
+					r=0
+					break
+				fi
+			done <<< "${gnupg_status}"
 		fi
+
+		if [[ ${r} -ne 0 ]]; then
+			# Exit early since it's typically inappropriate to
+			# try other mirrors in this case (it may indicate
+			# a keyring problem).
+			die "signature verification failed"
+		fi
+	else
+		die "cannot check signature: gpg binary not found"
+	fi
+}
+
+check_file_signature() {
+	local signature="$1"
+	local file="$2"
+	local r=1
+	local gnupg_status line
+
+	if [[ ${WEBRSYNC_VERIFY_SIGNATURE} != 0 ]]; then
+		[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "Checking signature ..."
+
+		case ${WEBRSYNC_VERIFY_SIGNATURE} in
+			1)
+				check_file_signature_gemato "${signature}" "${file}"
+				r=$?
+				;;
+			2)
+				check_file_signature_gpg_unwrapped "${signature}" "${file}"
+				r=$?
+				;;
+		esac
 	else
 		r=0
 	fi
 
 	return "${r}"
 }
 
@@ -249,15 +347,15 @@
 
 	do_tar "${file}" --to-stdout -f - --wildcards -x '*/metadata/timestamp.x' | cut -f 1 -d " "
 }
 
 sync_local() {
 	local file="$1"
 
-	__vecho "Syncing local tree ..."
+	[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "Syncing local repository ..."
 
 	local ownership="portage:portage"
 	if has usersync ${FEATURES} ; then
 		case "${USERLAND}" in
 			BSD)
 				ownership=$(stat -f '%Su:%Sg' "${repo_location}")
 				;;
@@ -270,45 +368,48 @@
 	if type -P tarsync > /dev/null ; then
 		local chown_opts="-o ${ownership%:*} -g ${ownership#*:}"
 		chown ${ownership} "${repo_location}" > /dev/null 2>&1 || chown_opts=""
 
 		if ! tarsync $(vvecho -v) -s 1 ${chown_opts} \
 			-e /distfiles -e /packages -e /local "${file}" "${repo_location}"; then
 
-			eecho "tarsync failed; tarball is corrupt? (${file})"
+			eerror "tarsync failed; tarball is corrupt? (${file})"
 			return 1
 		fi
 	else
 		if ! do_tar "${file}" -x --strip-components=1 -f -; then
-			eecho "tar failed to extract the image. tarball is corrupt? (${file})"
+			eerror "tar failed to extract the image. tarball is corrupt? (${file})"
 			return 1
 		fi
 
 		# Free disk space
 		${keep} || rm -f "${file}"
 
-		local rsync_opts="${PORTAGE_RSYNC_OPTS} ${PORTAGE_RSYNC_EXTRA_OPTS}"
+		local rsync_opts="${PORTAGE_RSYNC_OPTS} ${PORTAGE_RSYNC_EXTRA_OPTS} $(nvecho -q)"
 		if chown ${ownership} . > /dev/null 2>&1; then
 			chown -R ${ownership} .
 			rsync_opts+=" --owner --group"
 		fi
 
 		chmod 755 .
-		rsync ${rsync_opts} . "${repo_location%%/}"
+		rsync ${rsync_opts} . "${repo_location%%/}" || {
+			eerror "rsync failed: $?"
+			die "Aborting because of rsync failure"
+		}
 
-		__vecho "Cleaning up ..."
+		[[ ${PORTAGE_QUIET} == 1 ]] || einfo "Cleaning up ..."
 	fi
 
 	if has metadata-transfer ${FEATURES} ; then
-		__vecho "Updating cache ..."
+		einfo "Updating cache ..."
 		emerge --metadata
 	fi
 
-	local post_sync=${PORTAGE_CONFIGROOT}etc/portage/bin/post_sync
-	[ -x "${post_sync}" ] && "${post_sync}"
+	local post_sync=${PORTAGE_CONFIGROOT%/}/etc/portage/bin/post_sync
+	[[ -x "${post_sync}" ]] && "${post_sync}"
 
 	# --quiet suppresses output if there are no relevant news items
 	has news ${FEATURES} && emerge --check-news --quiet
 	return 0
 }
 
 do_snapshot() {
@@ -322,150 +423,157 @@
 	local have_files=0
 	local mirror
 
 	local compressions=""
 
 	type -P xzcat > /dev/null && compressions="${compressions} ${repo_name}:xz portage:xz"
 	type -P bzcat > /dev/null && compressions="${compressions} ${repo_name}:bz2 portage:bz2"
-	type -P  zcat > /dev/null && compressions="${compressions} ${repo_name}:gz portage:gz"
-
+	type -P zcat > /dev/null && compressions="${compressions} ${repo_name}:gz portage:gz"
 	if [[ -z ${compressions} ]] ; then
-		eecho "unable to locate any decompressors (xzcat or bzcat or zcat)"
-		exit 1
+		die "unable to locate any decompressors (xzcat or bzcat or zcat)"
 	fi
 
 	for mirror in ${GENTOO_MIRRORS} ; do
 		mirror=${mirror%/}
-		__vecho "Trying to retrieve ${date} snapshot from ${mirror} ..."
+		[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "Trying to retrieve ${date} snapshot from ${mirror} ..."
 
 		for compression in ${compressions} ; do
 			local name=${compression%%:*}
+
 			compression=${compression#*:}
+
 			local file="${name}-${date}.tar.${compression}"
 			local digest="${file}.md5sum"
 			local signature="${file}.gpgsig"
 
-			if [ -s "${DISTDIR}/${file}" -a -s "${DISTDIR}/${digest}" -a -s "${DISTDIR}/${signature}" ] ; then
+			if [[ -s "${DISTDIR}/${file}" && -s "${DISTDIR}/${digest}" && -s "${DISTDIR}/${signature}" ]] ; then
 				check_file_digest "${DISTDIR}/${digest}" "${DISTDIR}/${file}" && \
 				check_file_signature "${DISTDIR}/${signature}" "${DISTDIR}/${file}" && \
 				have_files=1
 			fi
 
-			if [ ${have_files} -eq 0 ] ; then
+			if [[ ${have_files} -eq 0 ]] ; then
 				fetch_file "${mirror}/snapshots/${digest}" "${digest}" && \
-				fetch_file "${mirror}/snapshots/${signature}" "${signature}" && \
-				fetch_file "${mirror}/snapshots/${file}" "${file}" && \
-				check_file_digest "${DISTDIR}/${digest}" "${DISTDIR}/${file}" && \
-				check_file_signature "${DISTDIR}/${signature}" "${DISTDIR}/${file}" && \
+					fetch_file "${mirror}/snapshots/${signature}" "${signature}" && \
+					fetch_file "${mirror}/snapshots/${file}" "${file}" && \
+					check_file_digest "${DISTDIR}/${digest}" "${DISTDIR}/${file}" && \
+					check_file_signature "${DISTDIR}/${signature}" "${DISTDIR}/${file}" && \
+
 				have_files=1
 			fi
 
 			#
 			# If timestamp is invalid
 			# we want to try and retrieve
 			# from a different mirror
 			#
-			if [ ${have_files} -eq 1 ]; then
-				__vecho "Getting snapshot timestamp ..."
-				local snapshot_timestamp=$(get_snapshot_timestamp "${DISTDIR}/${file}")
-
-				if [ ${ignore_timestamp} == 0 ]; then
-					if [ ${snapshot_timestamp} -lt $(get_portage_timestamp) ]; then
-						wecho "portage is newer than snapshot"
+			if [[ ${have_files} -eq 1 ]]; then
+				[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "Getting snapshot timestamp ..."
+
+				local snapshot_timestamp
+				snapshot_timestamp=$(get_snapshot_timestamp "${DISTDIR}/${file}")
+
+				if [[ ${ignore_timestamp} == 0 ]]; then
+					if [[ ${snapshot_timestamp} -lt $(get_repository_timestamp) ]]; then
+						ewarn "Repository (age) is newer than fetched snapshot"
 						have_files=0
 					fi
 				else
-					local utc_seconds=$(get_utc_second_from_string "${date}")
+					local utc_seconds
+					utc_seconds=$(get_utc_second_from_string "${date}")
 
-					#
-					# Check that this snapshot
-					# is what it claims to be ...
-					#
-					if [ ${snapshot_timestamp} -lt ${utc_seconds} ] || \
-						[ ${snapshot_timestamp} -gt $((${utc_seconds}+ 2*86400)) ]; then
+					# Check that this snapshot is what the age it claims to be
+					if [[ ${snapshot_timestamp} -lt ${utc_seconds} || \
+						${snapshot_timestamp} -gt $((${utc_seconds}+ 2*86400)) ]]; then
 
-						wecho "snapshot timestamp is not in acceptable period"
+						ewarn "Snapshot timestamp is not within acceptable period!"
 						have_files=0
 					fi
 				fi
 			fi
 
-			if [ ${have_files} -eq 1 ]; then
+			if [[ ${have_files} -eq 1 ]]; then
 				break
 			else
-				#
 				# Remove files and use a different mirror
-				#
 				rm -f "${DISTDIR}/${file}" "${DISTDIR}/${digest}" "${DISTDIR}/${signature}"
 			fi
 		done
 
-		[ ${have_files} -eq 1 ] && break
+		[[ ${have_files} -eq 1 ]] && break
 	done
 
-	if [ ${have_files} -eq 1 ]; then
+	if [[ ${have_files} -eq 1 ]]; then
 		sync_local "${DISTDIR}/${file}" && r=0
 	else
-		__vecho "${date} snapshot was not found"
+		ewarn "${date} snapshot was not found"
 	fi
 
 	${keep} || rm -f "${DISTDIR}/${file}" "${DISTDIR}/${digest}" "${DISTDIR}/${signature}"
 	return "${r}"
 }
 
 do_latest_snapshot() {
 	local attempts=0
 	local r=1
 
-	__vecho "Fetching most recent snapshot ..."
+	[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "Fetching most recent snapshot ..."
 
 	# The snapshot for a given day is generated at 00:45 UTC on the following
 	# day, so the current day's snapshot (going by UTC time) hasn't been
 	# generated yet.  Therefore, always start by looking for the previous day's
 	# snapshot (for attempts=1, subtract 1 day from the current UTC time).
 
 	# Timestamps that differ by less than 2 hours
 	# are considered to be approximately equal.
 	local min_time_diff=$(( 2 * 60 * 60 ))
 
-	local existing_timestamp=$(get_portage_timestamp)
+	local existing_timestamp
 	local timestamp_difference
 	local timestamp_problem
 	local approx_snapshot_time
-	local start_time=$(get_utc_date_in_seconds)
-	local start_hour=$(get_date_part ${start_time} "%H")
+	local start_time
+	local start_hour
+	local snapshot_date
+	local snapshot_date_seconds
+
+	existing_timestamp=$(get_repository_timestamp)
+	start_time=$(get_utc_date_in_seconds)
+	start_hour=$(get_date_part "${start_time}" "%H")
 
 	# Daily snapshots are created at 00:45 and are not
 	# available until after 01:00. Don't waste time trying
 	# to fetch a snapshot before it's been created.
-	if [ ${start_hour} -lt 1 ] ; then
+	if [[ ${start_hour} -lt 1 ]] ; then
 		(( start_time -= 86400 ))
 	fi
-	local snapshot_date=$(get_date_part ${start_time} "%Y%m%d")
-	local snapshot_date_seconds=$(get_utc_second_from_string ${snapshot_date})
 
-	while (( ${attempts} <  40 )) ; do
+	snapshot_date=$(get_date_part "${start_time}" "%Y%m%d")
+	snapshot_date_seconds=$(get_utc_second_from_string "${snapshot_date}")
+
+	while (( ${attempts} < 40 )) ; do
 		(( attempts++ ))
 		(( snapshot_date_seconds -= 86400 ))
 		# snapshots are created at 00:45
 		(( approx_snapshot_time = snapshot_date_seconds + 86400 + 2700 ))
 		(( timestamp_difference = existing_timestamp - approx_snapshot_time ))
-		[ ${timestamp_difference} -lt 0 ] && (( timestamp_difference = -1 * timestamp_difference ))
-		snapshot_date=$(get_date_part ${snapshot_date_seconds} "%Y%m%d")
+
+		[[ ${timestamp_difference} -lt 0 ]] && (( timestamp_difference = -1 * timestamp_difference ))
+		snapshot_date=$(get_date_part "${snapshot_date_seconds}" "%Y%m%d")
 
 		timestamp_problem=""
-		if [ ${timestamp_difference} -eq 0 ]; then
+		if [[ ${timestamp_difference} -eq 0 ]]; then
 			timestamp_problem="is identical to"
-		elif [ ${timestamp_difference} -lt ${min_time_diff} ]; then
+		elif [[ ${timestamp_difference} -lt ${min_time_diff} ]]; then
 			timestamp_problem="is possibly identical to"
-		elif [ ${approx_snapshot_time} -lt ${existing_timestamp} ] ; then
+		elif [[ ${approx_snapshot_time} -lt ${existing_timestamp} ]] ; then
 			timestamp_problem="is newer than"
 		fi
 
-		if [ -n "${timestamp_problem}" ]; then
+		if [[ -n "${timestamp_problem}" ]]; then
 			ewarn "Latest snapshot date: ${snapshot_date}"
 			ewarn
 			ewarn "Approximate snapshot timestamp: ${approx_snapshot_time}"
 			ewarn "       Current local timestamp: ${existing_timestamp}"
 			ewarn
 			echo -e "The current local timestamp" \
 				"${timestamp_problem} the" \
@@ -492,17 +600,18 @@
 
 usage() {
 	cat <<-EOF
 	Usage: $0 [options]
 
 	Options:
 	  --revert=yyyymmdd   Revert to snapshot
+	  --no-pgp-verify     Disable PGP verification of snapshot
 	  -k, --keep          Keep snapshots in DISTDIR (don't delete)
 	  -q, --quiet         Only output errors
-	  -v, --verbose       Enable verbose output
+	  -v, --verbose       Enable verbose output (no-op)
 	  -x, --debug         Enable debug output
 	  -h, --help          This help screen (duh!)
 	EOF
 	if [[ -n $* ]] ; then
 		printf "\nError: %s\n" "$*" 1>&2
 		exit 1
 	else
@@ -516,55 +625,55 @@
 
 	for arg in "$@" ; do
 		local v=${arg#*=}
 		case ${arg} in
 			-h|--help)    usage ;;
 			-k|--keep)    keep=true ;;
 			-q|--quiet)   PORTAGE_QUIET=1 ;;
-			-v|--verbose) do_verbose=1 ;;
+			-v|--verbose) unset PORTAGE_QUIET ;;
 			-x|--debug)   do_debug=1 ;;
 			--revert=*)   revert_date=${v} ;;
+			--no-pgp-verify) no_pgp_verify=1 ;;
 			*)            usage "Invalid option '${arg}'" ;;
 		esac
 	done
 
+	handle_pgp_setup
+
 	[[ -d ${repo_location} ]] || mkdir -p "${repo_location}"
 	if [[ ! -w ${repo_location} ]] ; then
-		eecho "Repository '${repo_name}' is not writable: ${repo_location}"
-		exit 1
+		die "Repository '${repo_name}' is not writable: ${repo_location}"
 	fi
 
 	[[ -d ${PORTAGE_TMPDIR}/portage ]] || mkdir -p "${PORTAGE_TMPDIR}/portage"
 	TMPDIR=$(mktemp -d "${PORTAGE_TMPDIR}/portage/webrsync-XXXXXX")
 	if [[ ! -w ${TMPDIR} ]] ; then
-		eecho "TMPDIR is not writable: ${TMPDIR}"
-		exit 1
+		die "TMPDIR is not writable: ${TMPDIR}"
 	fi
-	trap 'cd / ; rm -rf "${TMPDIR}"' EXIT
+	trap 'set -u ; cd / ; rm -rf "${TMPDIR}"' EXIT
 	cd "${TMPDIR}" || exit 1
 
 	${keep} || DISTDIR=${TMPDIR}
-	[ ! -d "${DISTDIR}" ] && mkdir -p "${DISTDIR}"
+	[[ ! -d "${DISTDIR}" ]] && mkdir -p "${DISTDIR}"
 
 	if ${keep} && [[ ! -w ${DISTDIR} ]] ; then
-		eecho "DISTDIR is not writable: ${DISTDIR}"
-		exit 1
+		die "DISTDIR is not writable: ${DISTDIR}"
 	fi
 
 	# This is a sanity check to help prevent people like funtoo users
 	# from accidentally wiping out their git tree.
-	if [[ -n ${repo_sync_type} &&  ${repo_sync_type} != rsync && ${repo_sync_type} != webrsync ]] ; then
-		echo "The current sync-type attribute of repository 'gentoo' is not set to 'rsync' or 'webrsync':" >&2
-		echo >&2
-		echo "  sync-type=${repo_sync_type}" >&2
-		echo >&2
-		echo "If you intend to use emerge-webrsync then please" >&2
-		echo "adjust sync-type and sync-uri attributes to refer to rsync." >&2
-		echo "emerge-webrsync exiting due to abnormal sync-type setting." >&2
-		exit 1
+	if [[ -n ${repo_sync_type} && ${repo_sync_type} != rsync && ${repo_sync_type} != webrsync ]] ; then
+		eerror "The current sync-type attribute of repository 'gentoo' is not set to 'rsync' or 'webrsync':"
+		eerror
+		eerror "  sync-type=${repo_sync_type}"
+		eerror
+		eerror "If you intend to use emerge-webrsync then please"
+		eerror "adjust sync-type and sync-uri attributes to refer to rsync."
+		eerror "emerge-webrsync exiting due to abnormal sync-type setting."
+		die
 	fi
 
 	[[ ${do_debug} -eq 1 ]] && set -x
 
 	if [[ -n ${revert_date} ]] ; then
 		do_snapshot 1 "${revert_date}"
 	else
```

### Comparing `portage-3.0.46/bin/emirrordist` & `portage-3.0.47/bin/emirrordist`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/env-update` & `portage-3.0.47/bin/env-update`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/estrip` & `portage-3.0.47/bin/estrip`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/etc-update` & `portage-3.0.47/bin/etc-update`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/filter-bash-environment.py` & `portage-3.0.47/bin/filter-bash-environment.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/fixpackages` & `portage-3.0.47/bin/fixpackages`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/glsa-check` & `portage-3.0.47/bin/glsa-check`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/gpkg-helper.py` & `portage-3.0.47/bin/gpkg-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/gpkg-sign` & `portage-3.0.47/bin/gpkg-sign`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/helper-functions.sh` & `portage-3.0.47/bin/helper-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/05prefix` & `portage-3.0.47/bin/install-qa-check.d/05prefix`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/10executable-issues` & `portage-3.0.47/bin/install-qa-check.d/10executable-issues`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/10ignored-flags` & `portage-3.0.47/bin/install-qa-check.d/10ignored-flags`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/20runtime-directories` & `portage-3.0.47/bin/install-qa-check.d/20runtime-directories`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/60bash-completion` & `portage-3.0.47/bin/install-qa-check.d/60bash-completion`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/60openrc` & `portage-3.0.47/bin/install-qa-check.d/60openrc`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/60pkgconfig` & `portage-3.0.47/bin/install-qa-check.d/60pkgconfig`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/60pngfix` & `portage-3.0.47/bin/install-qa-check.d/60pngfix`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/60systemd` & `portage-3.0.47/bin/install-qa-check.d/60systemd`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/80libraries` & `portage-3.0.47/bin/install-qa-check.d/80libraries`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/80multilib-strict` & `portage-3.0.47/bin/install-qa-check.d/80multilib-strict`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/90bad-bin-group-write` & `portage-3.0.47/bin/install-qa-check.d/90bad-bin-group-write`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/90bad-bin-owner` & `portage-3.0.47/bin/install-qa-check.d/90bad-bin-owner`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/90cmake-warnings` & `portage-3.0.47/bin/install-qa-check.d/90cmake-warnings`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/90config-impl-decl` & `portage-3.0.47/bin/install-qa-check.d/90config-impl-decl`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/90gcc-warnings` & `portage-3.0.47/bin/install-qa-check.d/90gcc-warnings`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 			reset_debug=1
 		fi
 
 		local m msgs=(
 			# only will and does, no might :)
 			'warning: .*will.*\[-Wstrict-aliasing\]'
 			'warning: .*does.*\[-Wstrict-aliasing\]'
+			'warning: .*\[-Wrestrict\]'
 			# strict aliasing violation in C++ (Clang)
 			'warning: .*\[-Wundefined-reinterpret-cast\]'
 
 			# implicit declaration of function ‘...’
 			'warning: .*\[-Wimplicit-function-declaration\]'
 			# with -Wall, goes in pair with -Wimplicit-function-declaration
 			# but without -Wall, we need to assert for it alone
@@ -40,14 +41,16 @@
 			'warning: .*\[-Warray-bounds\]'
 			# attempt to free a non-heap object
 			'warning: .*\[-Wfree-nonheap-object\]'
 			# those three do not have matching -W flags, it seems
 			'warning: .*will always overflow destination buffer'
 			# compile-time part of FORTIFY_SOURCE
 			'warning: .*\[-Wstringop-overflow\]'
+			'warning: .*\[-Wstringop-overread\]'
+			'warning: .*\[-Wstringop-truncation\]'
 			# clang-only, equivalent of -Wstringop-overflow
 			'warning: .*\[-Wfortify-source\]'
 			'warning: .*assuming pointer wraparound does not occur'
 			'warning: .*escape sequence out of range'
 
 			# all clang
 			'warning: .*\[-Wstrlcpy-strlcat-size\]'
@@ -82,14 +85,15 @@
 
 			# -Wformat
 			# TODO: comment out some time in future for time_t & LFS preparedness
 			#'warning: .*\[-Wformat=\]'
 			# -Wformat variants
 			'warning: .*too few arguments for format'
 			'warning: .*missing sentinel in function call.*\[-Wformat=\]'
+			'warning: .*\[-Wformat-truncation\]'
 			# format ... expects a matching ... argument
 			# (iow, too few arguments for format in new wording :))
 			'warning: .*matching.*\[-Wformat=\]'
 
 			# function returns address of local variable
 			'warning: .*\[-Wreturn-local-addr\]'
 			# missing return at end of function, or non-void return in a void function
@@ -100,27 +104,35 @@
 			# iteration invokes undefined behavior
 			'warning: .*\[-Waggressive-loop-optimizations\]'
 			# conversion between pointers that have incompatible types
 			'warning: .*\[-Wincompatible-pointer-types\]'
 			# more specific form of -Wincompatible-pointer-types (Clang)
 			'warning: .*\[-Wincompatible-function-pointer-types\]'
 			# these will fail with CFI (https://reviews.llvm.org/D134831)
+			# (gcc lacks -strict)
+			#'warning: .*\[-Wcast-function-type\]'
 			'warning: .*\[-Wcast-function-type-strict\]'
 			# using wrong deallocator, e.g. using free() on object allocated using my_malloc()
 			# when my_malloc() is annotated as needing my_free().
 			'warning: .*\[-Wmismatched-dealloc\]'
 			# clobbered: Warn for variables that might be changed by longjmp or vfork
 			# (This warning is also enabled by -Wextra.)
 			'warning: .*\[-Wclobbered\]'
 			# LTO type mismatch (https://wiki.gentoo.org/wiki/Project:Toolchain/LTO)
 			'warning: .*\[-Wlto-type-mismatch\]'
 			# ODR (https://wiki.gentoo.org/wiki/Project:Toolchain/LTO)
 			'warning: .*\[-Wodr\]'
 			# warning: argument value A will result in undefined behaviour (Clang)
 			'warning: .*\[-Wargument-undefined-behaviour\]'
+			'warning: .*\[-Wnull-dereference\]'
+
+			# general sensible warnings (will be rejected by modern compilers soon)
+			'warning: .*\[-Wmain\]'
+			'warning: .*\[-Wimplicit-int\]'
+			'warning: .*\[-Wstring-compare\]'
 
 			# this may be valid code :/
 			#': warning: multi-character character constant'
 			# need to check these two ...
 			#': warning: assuming signed overflow does not occur when'
 			#': warning: comparison with string literal results in unspecified behav'
 			# yacc/lex likes to trigger this one
```

### Comparing `portage-3.0.46/bin/install-qa-check.d/90world-writable` & `portage-3.0.47/bin/install-qa-check.d/90world-writable`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install-qa-check.d/95empty-dirs` & `portage-3.0.47/bin/install-qa-check.d/95empty-dirs`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/install.py` & `portage-3.0.47/bin/install.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/isolated-functions.sh` & `portage-3.0.47/bin/isolated-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/lock-helper.py` & `portage-3.0.47/bin/lock-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/misc-functions.sh` & `portage-3.0.47/bin/misc-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/phase-functions.sh` & `portage-3.0.47/bin/phase-functions.sh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2021 Gentoo Authors
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 # Hardcoded bash lists are needed for backward compatibility with
 # <portage-2.1.4 since they assume that a newly installed version
 # of ebuild.sh will work for pkg_postinst, pkg_prerm, and pkg_postrm
 # when portage is upgrading itself.
 
@@ -601,19 +601,19 @@
 	# Reset exeinto(), docinto(), insinto(), and into() state variables
 	# in case the user is running the install phase multiple times
 	# consecutively via the ebuild command.
 	if ___eapi_has_DESTTREE_INSDESTTREE; then
 		export DESTTREE=/usr
 		export INSDESTTREE=""
 	else
-		export _E_DESTTREE_=/usr
-		export _E_INSDESTTREE_=""
+		export __E_DESTTREE=/usr
+		export __E_INSDESTTREE=""
 	fi
-	export _E_EXEDESTTREE_=""
-	export _E_DOCDESTTREE_=""
+	export __E_EXEDESTTREE=""
+	export __E_DOCDESTTREE=""
 
 	__ebuild_phase src_install
 	>> "${PORTAGE_BUILDDIR}/.installed" || \
 		die "Failed to create ${PORTAGE_BUILDDIR}/.installed"
 	__vecho ">>> Completed installing ${CATEGORY}/${PF} into ${D}"
 	__vecho
 	__ebuild_phase post_src_install
```

### Comparing `portage-3.0.46/bin/phase-helpers.sh` & `portage-3.0.47/bin/phase-helpers.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env bash
-# Copyright 1999-2021 Gentoo Authors
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 if ___eapi_has_DESTTREE_INSDESTTREE; then
 	export DESTTREE=/usr
 	export INSDESTTREE=""
 else
-	export _E_DESTTREE_=/usr
-	export _E_INSDESTTREE_=""
+	export __E_DESTTREE=/usr
+	export __E_INSDESTTREE=""
 fi
-export _E_EXEDESTTREE_=""
-export _E_DOCDESTTREE_=""
+export __E_EXEDESTTREE=""
+export __E_DOCDESTTREE=""
 export INSOPTIONS="-m0644"
 export EXEOPTIONS="-m0755"
 export LIBOPTIONS="-m0644"
 export DIROPTIONS="-m0755"
 export MOPREFIX=${PN}
 # Do not compress files which are smaller than this (in bytes), bug #169260
 export PORTAGE_DOCOMPRESS_SIZE_LIMIT="128"
@@ -22,90 +22,90 @@
 declare -a PORTAGE_DOCOMPRESS_SKIP=( /usr/share/doc/${PF}/html )
 declare -a PORTAGE_DOSTRIP=( / )
 has strip ${PORTAGE_RESTRICT} && PORTAGE_DOSTRIP=()
 declare -a PORTAGE_DOSTRIP_SKIP=()
 
 into() {
 	if [[ "$1" == "/" ]]; then
-		export _E_DESTTREE_=""
+		export __E_DESTTREE=""
 	else
-		export _E_DESTTREE_=$1
+		export __E_DESTTREE=$1
 		if ! ___eapi_has_prefix_variables; then
 			local ED=${D}
 		fi
-		if [[ ! -d "${ED%/}/${_E_DESTTREE_#/}" ]]; then
-			install -d "${ED%/}/${_E_DESTTREE_#/}"
+		if [[ ! -d "${ED%/}/${__E_DESTTREE#/}" ]]; then
+			install -d "${ED%/}/${__E_DESTTREE#/}"
 
 			local ret=$?
 			if [[ ${ret} -ne 0 ]] ; then
 				__helpers_die "${FUNCNAME[0]} failed"
 				return ${ret}
 			fi
 		fi
 	fi
 
 	if ___eapi_has_DESTTREE_INSDESTTREE; then
-		export DESTTREE=${_E_DESTTREE_}
+		export DESTTREE=${__E_DESTTREE}
 	fi
 }
 
 insinto() {
 	if [[ "${1}" == "/" ]]; then
-		export _E_INSDESTTREE_=""
+		export __E_INSDESTTREE=""
 	else
-		export _E_INSDESTTREE_=${1}
+		export __E_INSDESTTREE=${1}
 		if ! ___eapi_has_prefix_variables; then
 			local ED=${D}
 		fi
-		if [[ ! -d "${ED%/}/${_E_INSDESTTREE_#/}" ]]; then
-			install -d "${ED%/}/${_E_INSDESTTREE_#/}"
+		if [[ ! -d "${ED%/}/${__E_INSDESTTREE#/}" ]]; then
+			install -d "${ED%/}/${__E_INSDESTTREE#/}"
 
 			local ret=$?
 			if [[ ${ret} -ne 0 ]] ; then
 				__helpers_die "${FUNCNAME[0]} failed"
 				return ${ret}
 			fi
 		fi
 	fi
 
 	if ___eapi_has_DESTTREE_INSDESTTREE; then
-		export INSDESTTREE=${_E_INSDESTTREE_}
+		export INSDESTTREE=${__E_INSDESTTREE}
 	fi
 }
 
 exeinto() {
 	if [[ "${1}" == "/" ]]; then
-		export _E_EXEDESTTREE_=""
+		export __E_EXEDESTTREE=""
 	else
-		export _E_EXEDESTTREE_="${1}"
+		export __E_EXEDESTTREE="${1}"
 		if ! ___eapi_has_prefix_variables; then
 			local ED=${D}
 		fi
-		if [[ ! -d "${ED%/}/${_E_EXEDESTTREE_#/}" ]]; then
-			install -d "${ED%/}/${_E_EXEDESTTREE_#/}"
+		if [[ ! -d "${ED%/}/${__E_EXEDESTTREE#/}" ]]; then
+			install -d "${ED%/}/${__E_EXEDESTTREE#/}"
 
 			local ret=$?
 			if [[ ${ret} -ne 0 ]] ; then
 				__helpers_die "${FUNCNAME[0]} failed"
 				return ${ret}
 			fi
 		fi
 	fi
 }
 
 docinto() {
 	if [[ "${1}" == "/" ]]; then
-		export _E_DOCDESTTREE_=""
+		export __E_DOCDESTTREE=""
 	else
-		export _E_DOCDESTTREE_="${1}"
+		export __E_DOCDESTTREE="${1}"
 		if ! ___eapi_has_prefix_variables; then
 			local ED=${D}
 		fi
-		if [[ ! -d "${ED%/}/usr/share/doc/${PF}/${_E_DOCDESTTREE_#/}" ]]; then
-			install -d "${ED%/}/usr/share/doc/${PF}/${_E_DOCDESTTREE_#/}"
+		if [[ ! -d "${ED%/}/usr/share/doc/${PF}/${__E_DOCDESTTREE#/}" ]]; then
+			install -d "${ED%/}/usr/share/doc/${PF}/${__E_DOCDESTTREE#/}"
 			local ret=$?
 			if [[ ${ret} -ne 0 ]] ; then
 				__helpers_die "${FUNCNAME[0]} failed"
 				return ${ret}
 			fi
 		fi
 	fi
@@ -639,21 +639,23 @@
 			if ___eapi_econf_passes_--datarootdir; then
 				if [[ ${conf_help} == *--datarootdir* ]]; then
 					conf_args+=( --datarootdir="${EPREFIX}"/usr/share )
 				fi
 			fi
 
 			if ___eapi_econf_passes_--disable-dependency-tracking; then
-				if [[ ${conf_help} == *--disable-dependency-tracking* ]]; then
+				if [[ ${conf_help} == \
+						*--disable-dependency-tracking[^A-Za-z0-9+_.-]* ]]; then
 					conf_args+=( --disable-dependency-tracking )
 				fi
 			fi
 
 			if ___eapi_econf_passes_--disable-silent-rules; then
-				if [[ ${conf_help} == *--disable-silent-rules* ]]; then
+				if [[ ${conf_help} == \
+						*--disable-silent-rules[^A-Za-z0-9+_.-]* ]]; then
 					conf_args+=( --disable-silent-rules )
 				fi
 			fi
 
 			if ___eapi_econf_passes_--disable-static; then
 				if [[ ${conf_help} == *--enable-shared[^A-Za-z0-9+_.-]* &&
 						${conf_help} == *--enable-static[^A-Za-z0-9+_.-]* ]]; then
@@ -668,15 +670,15 @@
 
 				if [[ ${conf_help} == *--htmldir* ]]; then
 					conf_args+=( --htmldir="${EPREFIX}"/usr/share/doc/${PF}/html )
 				fi
 			fi
 
 			if ___eapi_econf_passes_--with-sysroot; then
-				if [[ ${conf_help} == *--with-sysroot* ]]; then
+				if [[ ${conf_help} == *--with-sysroot[^A-Za-z0-9+_.-]* ]]; then
 					conf_args+=( --with-sysroot="${ESYSROOT:-/}" )
 				fi
 			fi
 		fi
 
 		# If the profile defines a location to install libs to aside from default, pass it on.
 		# If the ebuild passes in --libdir, they're responsible for the conf_libdir fun.
```

### Comparing `portage-3.0.46/bin/pid-ns-init` & `portage-3.0.47/bin/pid-ns-init`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/portageq` & `portage-3.0.47/bin/portageq`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/postinst-qa-check.d/50xdg-utils` & `portage-3.0.47/bin/postinst-qa-check.d/50xdg-utils`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/quickpkg` & `portage-3.0.47/bin/quickpkg`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/regenworld` & `portage-3.0.47/bin/regenworld`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/save-ebuild-env.sh` & `portage-3.0.47/bin/save-ebuild-env.sh`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # --exclude-init-phases causes pkg_nofetch and src_* phase functions to
 # be excluded from the output. These function are not needed for installation
 # or removal of the packages, and can therefore be safely excluded.
 #
 __save_ebuild_env() {
 	(
 	if has --exclude-init-phases $* ; then
-		unset S _E_DESTTREE _E_INSDESTTREE _E_DOCDESTTREE_ _E_EXEDESTTREE_ \
+		unset S __E_DESTTREE __E_INSDESTTREE __E_DOCDESTTREE __E_EXEDESTTREE \
 			PORTAGE_DOCOMPRESS_SIZE_LIMIT PORTAGE_DOCOMPRESS \
 			PORTAGE_DOCOMPRESS_SKIP PORTAGE_DOSTRIP PORTAGE_DOSTRIP_SKIP
 		if [[ -n ${PYTHONPATH} &&
 			${PYTHONPATH%%:*} -ef ${PORTAGE_PYM_PATH} ]] ; then
 			if [[ ${PYTHONPATH} == *:* ]] ; then
 				export PYTHONPATH=${PYTHONPATH#*:}
 			else
```

### Comparing `portage-3.0.46/bin/shelve-utils` & `portage-3.0.47/bin/shelve-utils`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/socks5-server.py` & `portage-3.0.47/bin/socks5-server.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/xattr-helper.py` & `portage-3.0.47/bin/xattr-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/bin/xpak-helper.py` & `portage-3.0.47/bin/xpak-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.alpha.diff` & `portage-3.0.47/cnf/make.conf.example.alpha.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.amd64-fbsd.diff` & `portage-3.0.47/cnf/make.conf.example.amd64-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.amd64.diff` & `portage-3.0.47/cnf/make.conf.example.amd64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.arm.diff` & `portage-3.0.47/cnf/make.conf.example.arm.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.arm64.diff` & `portage-3.0.47/cnf/make.conf.example.arm64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.hppa.diff` & `portage-3.0.47/cnf/make.conf.example.hppa.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.ia64.diff` & `portage-3.0.47/cnf/make.conf.example.ia64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.loong.diff` & `portage-3.0.47/cnf/make.conf.example.loong.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.m68k.diff` & `portage-3.0.47/cnf/make.conf.example.m68k.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.mips.diff` & `portage-3.0.47/cnf/make.conf.example.mips.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.ppc.diff` & `portage-3.0.47/cnf/make.conf.example.ppc.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.ppc64.diff` & `portage-3.0.47/cnf/make.conf.example.ppc64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.riscv.diff` & `portage-3.0.47/cnf/make.conf.example.riscv.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.s390.diff` & `portage-3.0.47/cnf/make.conf.example.s390.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.sh.diff` & `portage-3.0.47/cnf/make.conf.example.sh.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.sparc-fbsd.diff` & `portage-3.0.47/cnf/make.conf.example.sparc-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.sparc.diff` & `portage-3.0.47/cnf/make.conf.example.sparc.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.x86-fbsd.diff` & `portage-3.0.47/cnf/make.conf.example.x86-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/cnf/make.conf.example.x86.diff` & `portage-3.0.47/cnf/make.conf.example.x86.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/api/Makefile` & `portage-3.0.47/doc/api/Makefile`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/api/conf.py` & `portage-3.0.47/doc/api/conf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/config/bashrc.docbook` & `portage-3.0.47/doc/config/bashrc.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/config/sets.docbook` & `portage-3.0.47/doc/config/sets.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/dependency_resolution/decision_making.docbook` & `portage-3.0.47/doc/dependency_resolution/decision_making.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/dependency_resolution/package_modeling.docbook` & `portage-3.0.47/doc/dependency_resolution/package_modeling.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/dependency_resolution/task_scheduling.docbook` & `portage-3.0.47/doc/dependency_resolution/task_scheduling.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/package/ebuild/eapi/1.docbook` & `portage-3.0.47/doc/package/ebuild/eapi/1.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/package/ebuild/eapi/2.docbook` & `portage-3.0.47/doc/package/ebuild/eapi/2.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/package/ebuild/eapi/3.docbook` & `portage-3.0.47/doc/package/ebuild/eapi/3.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/package/ebuild/eapi/4-slot-abi.docbook` & `portage-3.0.47/doc/package/ebuild/eapi/4-slot-abi.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/package/ebuild/eapi/4.docbook` & `portage-3.0.47/doc/package/ebuild/eapi/4.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/package/ebuild/eapi/5.docbook` & `portage-3.0.47/doc/package/ebuild/eapi/5.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/package/ebuild/helper_functions.docbook` & `portage-3.0.47/doc/package/ebuild/helper_functions.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/package/ebuild/phases.docbook` & `portage-3.0.47/doc/package/ebuild/phases.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/portage.docbook` & `portage-3.0.47/doc/portage.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/doc/qa.docbook` & `portage-3.0.47/doc/qa.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/AbstractDepPriority.py` & `portage-3.0.47/lib/_emerge/AbstractDepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/AbstractEbuildProcess.py` & `portage-3.0.47/lib/_emerge/AbstractEbuildProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/AbstractPollTask.py` & `portage-3.0.47/lib/_emerge/AbstractPollTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/AsynchronousLock.py` & `portage-3.0.47/lib/_emerge/AsynchronousLock.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/AsynchronousTask.py` & `portage-3.0.47/lib/_emerge/AsynchronousTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/Binpkg.py` & `portage-3.0.47/lib/_emerge/Binpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/BinpkgEnvExtractor.py` & `portage-3.0.47/lib/_emerge/BinpkgEnvExtractor.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/BinpkgExtractorAsync.py` & `portage-3.0.47/lib/_emerge/BinpkgExtractorAsync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/BinpkgFetcher.py` & `portage-3.0.47/lib/_emerge/BinpkgFetcher.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/BinpkgPrefetcher.py` & `portage-3.0.47/lib/_emerge/BinpkgPrefetcher.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/BinpkgVerifier.py` & `portage-3.0.47/lib/_emerge/BinpkgVerifier.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/BlockerCache.py` & `portage-3.0.47/lib/_emerge/BlockerCache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/BlockerDB.py` & `portage-3.0.47/lib/_emerge/BlockerDB.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/CompositeTask.py` & `portage-3.0.47/lib/_emerge/CompositeTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/DepPriority.py` & `portage-3.0.47/lib/_emerge/DepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/DepPriorityNormalRange.py` & `portage-3.0.47/lib/_emerge/DepPriorityNormalRange.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/DepPrioritySatisfiedRange.py` & `portage-3.0.47/lib/_emerge/DepPrioritySatisfiedRange.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/Dependency.py` & `portage-3.0.47/lib/_emerge/Dependency.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/DependencyArg.py` & `portage-3.0.47/lib/_emerge/DependencyArg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildBinpkg.py` & `portage-3.0.47/lib/_emerge/EbuildBinpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildBuild.py` & `portage-3.0.47/lib/_emerge/EbuildBuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildBuildDir.py` & `portage-3.0.47/lib/_emerge/EbuildBuildDir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildExecuter.py` & `portage-3.0.47/lib/_emerge/EbuildExecuter.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildFetcher.py` & `portage-3.0.47/lib/_emerge/EbuildFetcher.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildFetchonly.py` & `portage-3.0.47/lib/_emerge/EbuildFetchonly.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildIpcDaemon.py` & `portage-3.0.47/lib/_emerge/EbuildIpcDaemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildMerge.py` & `portage-3.0.47/lib/_emerge/EbuildMerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildMetadataPhase.py` & `portage-3.0.47/lib/_emerge/EbuildMetadataPhase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildPhase.py` & `portage-3.0.47/lib/_emerge/EbuildPhase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildProcess.py` & `portage-3.0.47/lib/_emerge/EbuildProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/EbuildSpawnProcess.py` & `portage-3.0.47/lib/_emerge/EbuildSpawnProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/FakeVartree.py` & `portage-3.0.47/lib/_emerge/FakeVartree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/FifoIpcDaemon.py` & `portage-3.0.47/lib/_emerge/FifoIpcDaemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/JobStatusDisplay.py` & `portage-3.0.47/lib/_emerge/JobStatusDisplay.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/MergeListItem.py` & `portage-3.0.47/lib/_emerge/MergeListItem.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/MetadataRegen.py` & `portage-3.0.47/lib/_emerge/MetadataRegen.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/MiscFunctionsProcess.py` & `portage-3.0.47/lib/_emerge/MiscFunctionsProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/Package.py` & `portage-3.0.47/lib/_emerge/Package.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/PackageArg.py` & `portage-3.0.47/lib/_emerge/PackageArg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/PackageMerge.py` & `portage-3.0.47/lib/_emerge/PackageMerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/PackagePhase.py` & `portage-3.0.47/lib/_emerge/PackagePhase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/PackageUninstall.py` & `portage-3.0.47/lib/_emerge/PackageUninstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/PackageVirtualDbapi.py` & `portage-3.0.47/lib/_emerge/PackageVirtualDbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/PipeReader.py` & `portage-3.0.47/lib/_emerge/PipeReader.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/PollScheduler.py` & `portage-3.0.47/lib/_emerge/PollScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/ProgressHandler.py` & `portage-3.0.47/lib/_emerge/ProgressHandler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/RootConfig.py` & `portage-3.0.47/lib/_emerge/RootConfig.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/Scheduler.py` & `portage-3.0.47/lib/_emerge/Scheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/SequentialTaskQueue.py` & `portage-3.0.47/lib/_emerge/SequentialTaskQueue.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/SpawnProcess.py` & `portage-3.0.47/lib/_emerge/SpawnProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/SubProcess.py` & `portage-3.0.47/lib/_emerge/SubProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/Task.py` & `portage-3.0.47/lib/_emerge/Task.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/TaskSequence.py` & `portage-3.0.47/lib/_emerge/TaskSequence.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/UnmergeDepPriority.py` & `portage-3.0.47/lib/_emerge/UnmergeDepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/UseFlagDisplay.py` & `portage-3.0.47/lib/_emerge/UseFlagDisplay.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/UserQuery.py` & `portage-3.0.47/lib/_emerge/UserQuery.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/_find_deep_system_runtime_deps.py` & `portage-3.0.47/lib/_emerge/_find_deep_system_runtime_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/actions.py` & `portage-3.0.47/lib/_emerge/actions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/chk_updated_cfg_files.py` & `portage-3.0.47/lib/_emerge/chk_updated_cfg_files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/countdown.py` & `portage-3.0.47/lib/_emerge/countdown.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/create_depgraph_params.py` & `portage-3.0.47/lib/_emerge/create_depgraph_params.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/create_world_atom.py` & `portage-3.0.47/lib/_emerge/create_world_atom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/depgraph.py` & `portage-3.0.47/lib/_emerge/depgraph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/emergelog.py` & `portage-3.0.47/lib/_emerge/emergelog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/getloadavg.py` & `portage-3.0.47/lib/_emerge/getloadavg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/help.py` & `portage-3.0.47/lib/_emerge/help.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/is_valid_package_atom.py` & `portage-3.0.47/lib/_emerge/is_valid_package_atom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/main.py` & `portage-3.0.47/lib/_emerge/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/post_emerge.py` & `portage-3.0.47/lib/_emerge/post_emerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/resolver/DbapiProvidesIndex.py` & `portage-3.0.47/lib/_emerge/resolver/DbapiProvidesIndex.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/resolver/backtracking.py` & `portage-3.0.47/lib/_emerge/resolver/backtracking.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/resolver/circular_dependency.py` & `portage-3.0.47/lib/_emerge/resolver/circular_dependency.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/resolver/output.py` & `portage-3.0.47/lib/_emerge/resolver/output.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/resolver/output_helpers.py` & `portage-3.0.47/lib/_emerge/resolver/output_helpers.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/resolver/package_tracker.py` & `portage-3.0.47/lib/_emerge/resolver/package_tracker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/resolver/slot_collision.py` & `portage-3.0.47/lib/_emerge/resolver/slot_collision.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/search.py` & `portage-3.0.47/lib/_emerge/search.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/show_invalid_depstring_notice.py` & `portage-3.0.47/lib/_emerge/show_invalid_depstring_notice.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/stdout_spinner.py` & `portage-3.0.47/lib/_emerge/stdout_spinner.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/_emerge/unmerge.py` & `portage-3.0.47/lib/_emerge/unmerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/__init__.py` & `portage-3.0.47/lib/portage/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_compat_upgrade/binpkg_compression.py` & `portage-3.0.47/lib/portage/_compat_upgrade/binpkg_compression.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_compat_upgrade/binpkg_multi_instance.py` & `portage-3.0.47/lib/portage/_compat_upgrade/binpkg_multi_instance.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_compat_upgrade/default_locations.py` & `portage-3.0.47/lib/portage/_compat_upgrade/default_locations.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_emirrordist/Config.py` & `portage-3.0.47/lib/portage/_emirrordist/Config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_emirrordist/ContentDB.py` & `portage-3.0.47/lib/portage/_emirrordist/ContentDB.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_emirrordist/DeletionIterator.py` & `portage-3.0.47/lib/portage/_emirrordist/DeletionIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_emirrordist/DeletionTask.py` & `portage-3.0.47/lib/portage/_emirrordist/DeletionTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_emirrordist/FetchIterator.py` & `portage-3.0.47/lib/portage/_emirrordist/FetchIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_emirrordist/FetchTask.py` & `portage-3.0.47/lib/portage/_emirrordist/FetchTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_emirrordist/MirrorDistTask.py` & `portage-3.0.47/lib/portage/_emirrordist/MirrorDistTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_emirrordist/main.py` & `portage-3.0.47/lib/portage/_emirrordist/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_global_updates.py` & `portage-3.0.47/lib/portage/_global_updates.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_legacy_globals.py` & `portage-3.0.47/lib/portage/_legacy_globals.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_selinux.py` & `portage-3.0.47/lib/portage/_selinux.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/ProfilePackageSet.py` & `portage-3.0.47/lib/portage/_sets/ProfilePackageSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/__init__.py` & `portage-3.0.47/lib/portage/_sets/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/base.py` & `portage-3.0.47/lib/portage/_sets/base.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/dbapi.py` & `portage-3.0.47/lib/portage/_sets/dbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/files.py` & `portage-3.0.47/lib/portage/_sets/files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/libs.py` & `portage-3.0.47/lib/portage/_sets/libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/profiles.py` & `portage-3.0.47/lib/portage/_sets/profiles.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/security.py` & `portage-3.0.47/lib/portage/_sets/security.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/_sets/shell.py` & `portage-3.0.47/lib/portage/_sets/shell.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/binpkg.py` & `portage-3.0.47/lib/portage/binpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/binrepo/config.py` & `portage-3.0.47/lib/portage/binrepo/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/anydbm.py` & `portage-3.0.47/lib/portage/cache/anydbm.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/cache_errors.py` & `portage-3.0.47/lib/portage/cache/cache_errors.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/ebuild_xattr.py` & `portage-3.0.47/lib/portage/cache/ebuild_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/flat_hash.py` & `portage-3.0.47/lib/portage/cache/flat_hash.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/fs_template.py` & `portage-3.0.47/lib/portage/cache/fs_template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/index/IndexStreamIterator.py` & `portage-3.0.47/lib/portage/cache/index/IndexStreamIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/index/pkg_desc_index.py` & `portage-3.0.47/lib/portage/cache/index/pkg_desc_index.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/mappings.py` & `portage-3.0.47/lib/portage/cache/mappings.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/metadata.py` & `portage-3.0.47/lib/portage/cache/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/sql_template.py` & `portage-3.0.47/lib/portage/cache/sql_template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/sqlite.py` & `portage-3.0.47/lib/portage/cache/sqlite.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/template.py` & `portage-3.0.47/lib/portage/cache/template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cache/volatile.py` & `portage-3.0.47/lib/portage/cache/volatile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/checksum.py` & `portage-3.0.47/lib/portage/checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/const.py` & `portage-3.0.47/lib/portage/const.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/cvstree.py` & `portage-3.0.47/lib/portage/cvstree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/data.py` & `portage-3.0.47/lib/portage/data.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/DummyTree.py` & `portage-3.0.47/lib/portage/dbapi/DummyTree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/IndexedPortdb.py` & `portage-3.0.47/lib/portage/dbapi/IndexedPortdb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/IndexedVardb.py` & `portage-3.0.47/lib/portage/dbapi/IndexedVardb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/_ContentsCaseSensitivityManager.py` & `portage-3.0.47/lib/portage/dbapi/_ContentsCaseSensitivityManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/_MergeProcess.py` & `portage-3.0.47/lib/portage/dbapi/_MergeProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/_SyncfsProcess.py` & `portage-3.0.47/lib/portage/dbapi/_SyncfsProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/_VdbMetadataDelta.py` & `portage-3.0.47/lib/portage/dbapi/_VdbMetadataDelta.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/__init__.py` & `portage-3.0.47/lib/portage/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/_expand_new_virt.py` & `portage-3.0.47/lib/portage/dbapi/_expand_new_virt.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/_similar_name_search.py` & `portage-3.0.47/lib/portage/dbapi/_similar_name_search.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/bintree.py` & `portage-3.0.47/lib/portage/dbapi/bintree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/cpv_expand.py` & `portage-3.0.47/lib/portage/dbapi/cpv_expand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/dep_expand.py` & `portage-3.0.47/lib/portage/dbapi/dep_expand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/porttree.py` & `portage-3.0.47/lib/portage/dbapi/porttree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/vartree.py` & `portage-3.0.47/lib/portage/dbapi/vartree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dbapi/virtual.py` & `portage-3.0.47/lib/portage/dbapi/virtual.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/debug.py` & `portage-3.0.47/lib/portage/debug.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dep/__init__.py` & `portage-3.0.47/lib/portage/dep/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dep/_dnf.py` & `portage-3.0.47/lib/portage/dep/_dnf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dep/_slot_operator.py` & `portage-3.0.47/lib/portage/dep/_slot_operator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dep/dep_check.py` & `portage-3.0.47/lib/portage/dep/dep_check.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dep/soname/SonameAtom.py` & `portage-3.0.47/lib/portage/dep/soname/SonameAtom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dep/soname/multilib_category.py` & `portage-3.0.47/lib/portage/dep/soname/multilib_category.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dep/soname/parse.py` & `portage-3.0.47/lib/portage/dep/soname/parse.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/dispatch_conf.py` & `portage-3.0.47/lib/portage/dispatch_conf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/eapi.py` & `portage-3.0.47/lib/portage/eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/eclass_cache.py` & `portage-3.0.47/lib/portage/eclass_cache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/__init__.py` & `portage-3.0.47/lib/portage/elog/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/filtering.py` & `portage-3.0.47/lib/portage/elog/filtering.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/messages.py` & `portage-3.0.47/lib/portage/elog/messages.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/mod_custom.py` & `portage-3.0.47/lib/portage/elog/mod_custom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/mod_echo.py` & `portage-3.0.47/lib/portage/elog/mod_echo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/mod_mail.py` & `portage-3.0.47/lib/portage/elog/mod_mail.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/mod_mail_summary.py` & `portage-3.0.47/lib/portage/elog/mod_mail_summary.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/mod_save.py` & `portage-3.0.47/lib/portage/elog/mod_save.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/mod_save_summary.py` & `portage-3.0.47/lib/portage/elog/mod_save_summary.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/elog/mod_syslog.py` & `portage-3.0.47/lib/portage/elog/mod_syslog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/defaults.py` & `portage-3.0.47/lib/portage/emaint/defaults.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/main.py` & `portage-3.0.47/lib/portage/emaint/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/binhost/__init__.py` & `portage-3.0.47/lib/portage/emaint/modules/binhost/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/binhost/binhost.py` & `portage-3.0.47/lib/portage/emaint/modules/binhost/binhost.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/config/__init__.py` & `portage-3.0.47/lib/portage/emaint/modules/config/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/config/config.py` & `portage-3.0.47/lib/portage/emaint/modules/config/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/logs/__init__.py` & `portage-3.0.47/lib/portage/emaint/modules/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/logs/logs.py` & `portage-3.0.47/lib/portage/emaint/modules/logs/logs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/merges/__init__.py` & `portage-3.0.47/lib/portage/emaint/modules/merges/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/merges/merges.py` & `portage-3.0.47/lib/portage/emaint/modules/merges/merges.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/move/__init__.py` & `portage-3.0.47/lib/portage/emaint/modules/move/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/move/move.py` & `portage-3.0.47/lib/portage/emaint/modules/move/move.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/resume/__init__.py` & `portage-3.0.47/lib/portage/emaint/modules/resume/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/resume/resume.py` & `portage-3.0.47/lib/portage/emaint/modules/resume/resume.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/sync/__init__.py` & `portage-3.0.47/lib/portage/emaint/modules/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/sync/sync.py` & `portage-3.0.47/lib/portage/emaint/modules/sync/sync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/emaint/modules/world/world.py` & `portage-3.0.47/lib/portage/emaint/modules/world/world.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/env/config.py` & `portage-3.0.47/lib/portage/env/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/env/loaders.py` & `portage-3.0.47/lib/portage/env/loaders.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/env/validators.py` & `portage-3.0.47/lib/portage/env/validators.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/exception.py` & `portage-3.0.47/lib/portage/exception.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/getbinpkg.py` & `portage-3.0.47/lib/portage/getbinpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/glsa.py` & `portage-3.0.47/lib/portage/glsa.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/gpg.py` & `portage-3.0.47/lib/portage/gpg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/gpkg.py` & `portage-3.0.47/lib/portage/gpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/localization.py` & `portage-3.0.47/lib/portage/localization.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/locks.py` & `portage-3.0.47/lib/portage/locks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/mail.py` & `portage-3.0.47/lib/portage/mail.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/manifest.py` & `portage-3.0.47/lib/portage/manifest.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/metadata.py` & `portage-3.0.47/lib/portage/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/module.py` & `portage-3.0.47/lib/portage/module.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/news.py` & `portage-3.0.47/lib/portage/news.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/output.py` & `portage-3.0.47/lib/portage/output.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/KeywordsManager.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/KeywordsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/LicenseManager.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/LicenseManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/LocationsManager.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/LocationsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/MaskManager.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/MaskManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/UseManager.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/UseManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/VirtualsManager.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/VirtualsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/env_var_validation.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/env_var_validation.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/features_set.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/features_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/helper.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_config/special_env_vars.py` & `portage-3.0.47/lib/portage/package/ebuild/_config/special_env_vars.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_ipc/ExitCommand.py` & `portage-3.0.47/lib/portage/package/ebuild/_ipc/ExitCommand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_ipc/QueryCommand.py` & `portage-3.0.47/lib/portage/package/ebuild/_ipc/QueryCommand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_metadata_invalid.py` & `portage-3.0.47/lib/portage/package/ebuild/_metadata_invalid.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py` & `portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py` & `portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py` & `portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/_spawn_nofetch.py` & `portage-3.0.47/lib/portage/package/ebuild/_spawn_nofetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/config.py` & `portage-3.0.47/lib/portage/package/ebuild/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/deprecated_profile_check.py` & `portage-3.0.47/lib/portage/package/ebuild/deprecated_profile_check.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/digestcheck.py` & `portage-3.0.47/lib/portage/package/ebuild/digestcheck.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/digestgen.py` & `portage-3.0.47/lib/portage/package/ebuild/digestgen.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/doebuild.py` & `portage-3.0.47/lib/portage/package/ebuild/doebuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2010-2021 Gentoo Authors
+# Copyright 2010-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 __all__ = ["doebuild", "doebuild_environment", "spawn", "spawnebuild"]
 
 import grp
 import gzip
 import errno
@@ -439,23 +439,19 @@
 
     mysettings["PORTAGE_BASHRC_FILES"] = "\n".join(mysettings._pbashrc)
 
     mysettings["P"] = mysplit[0] + "-" + mysplit[1]
     mysettings["PN"] = mysplit[0]
     mysettings["PV"] = mysplit[1]
     mysettings["PR"] = mysplit[2]
+    mysettings["PVR"] = mypv[len(mysplit[0]) + 1 :]
 
     if noiselimit < 0:
         mysettings["PORTAGE_QUIET"] = "1"
 
-    if mysplit[2] == "r0":
-        mysettings["PVR"] = mysplit[1]
-    else:
-        mysettings["PVR"] = mysplit[1] + "-" + mysplit[2]
-
     # All temporary directories should be subdirectories of
     # $PORTAGE_TMPDIR/portage, since it's common for /tmp and /var/tmp
     # to be mounted with the "noexec" option (see bug #346899).
     mysettings["BUILD_PREFIX"] = mysettings["PORTAGE_TMPDIR"] + "/portage"
     mysettings["PKG_TMPDIR"] = mysettings["BUILD_PREFIX"] + "/._unmerge_"
 
     # Package {pre,post}inst and {pre,post}rm may overlap, so they must have separate
```

### Comparing `portage-3.0.46/lib/portage/package/ebuild/fetch.py` & `portage-3.0.47/lib/portage/package/ebuild/fetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/getmaskingreason.py` & `portage-3.0.47/lib/portage/package/ebuild/getmaskingreason.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/getmaskingstatus.py` & `portage-3.0.47/lib/portage/package/ebuild/getmaskingstatus.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/prepare_build_dirs.py` & `portage-3.0.47/lib/portage/package/ebuild/prepare_build_dirs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/package/ebuild/profile_iuse.py` & `portage-3.0.47/lib/portage/package/ebuild/profile_iuse.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/process.py` & `portage-3.0.47/lib/portage/process.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/progress.py` & `portage-3.0.47/lib/portage/progress.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/proxy/lazyimport.py` & `portage-3.0.47/lib/portage/proxy/lazyimport.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/proxy/objectproxy.py` & `portage-3.0.47/lib/portage/proxy/objectproxy.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/repository/config.py` & `portage-3.0.47/lib/portage/repository/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/repository/storage/hardlink_quarantine.py` & `portage-3.0.47/lib/portage/repository/storage/hardlink_quarantine.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/repository/storage/hardlink_rcu.py` & `portage-3.0.47/lib/portage/repository/storage/hardlink_rcu.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/repository/storage/inplace.py` & `portage-3.0.47/lib/portage/repository/storage/inplace.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/repository/storage/interface.py` & `portage-3.0.47/lib/portage/repository/storage/interface.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/__init__.py` & `portage-3.0.47/lib/portage/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/config_checks.py` & `portage-3.0.47/lib/portage/sync/config_checks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/controller.py` & `portage-3.0.47/lib/portage/sync/controller.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/getaddrinfo_validate.py` & `portage-3.0.47/lib/portage/sync/getaddrinfo_validate.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/cvs/__init__.py` & `portage-3.0.47/lib/portage/sync/modules/cvs/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/cvs/cvs.py` & `portage-3.0.47/lib/portage/sync/modules/cvs/cvs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/git/__init__.py` & `portage-3.0.47/lib/portage/sync/modules/git/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/git/git.py` & `portage-3.0.47/lib/portage/sync/modules/git/git.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/mercurial/__init__.py` & `portage-3.0.47/lib/portage/sync/modules/mercurial/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/mercurial/mercurial.py` & `portage-3.0.47/lib/portage/sync/modules/mercurial/mercurial.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/rsync/__init__.py` & `portage-3.0.47/lib/portage/sync/modules/rsync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/rsync/rsync.py` & `portage-3.0.47/lib/portage/sync/modules/rsync/rsync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/svn/__init__.py` & `portage-3.0.47/lib/portage/sync/modules/svn/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/svn/svn.py` & `portage-3.0.47/lib/portage/sync/modules/svn/svn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/modules/webrsync/__init__.py` & `portage-3.0.47/lib/portage/sync/modules/webrsync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 import os
 
 from portage.sync.config_checks import CheckSyncConfig
 
 
 DEFAULT_CLASS = "WebRsync"
-AVAILABLE_CLASSES = ["WebRsync", "PyWebsync"]
-options = {"1": "WebRsync", "2": "PyWebsync"}
+AVAILABLE_CLASSES = ["WebRsync", "PyWebRsync"]
+options = {"1": "WebRsync", "2": "PyWebRsync"}
 
 
 config_class = DEFAULT_CLASS
 try:
     test_param = os.environ["TESTIT"]
     if test_param in options:
         config_class = options[test_param]
```

### Comparing `portage-3.0.46/lib/portage/sync/modules/webrsync/webrsync.py` & `portage-3.0.47/lib/portage/sync/modules/webrsync/webrsync.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,29 +3,37 @@
 import logging
 
 import portage
 from portage import os
 from portage.util import writemsg_level
 from portage.util.futures import asyncio
 from portage.output import create_color_func
+from portage.sync.syncbase import SyncBase
 
 good = create_color_func("GOOD")
 bad = create_color_func("BAD")
 warn = create_color_func("WARN")
-from portage.sync.syncbase import SyncBase
 
 try:
     from gemato.exceptions import GematoException
     import gemato.openpgp
 except ImportError:
     gemato = None
 
 
 class WebRsync(SyncBase):
-    """WebRSync sync class"""
+    """WebRSync sync class
+
+    This class implements syncing via calls to an external binary, either:
+    - emerge-delta-webrsync (if sync-webrsync-delta is set), or
+    - emerge-webrsync
+
+    It wraps them and performs PGP verification if sync-webrsync-verify-signature
+    is set via gemato.
+    """
 
     short_desc = "Perform sync operations on webrsync based repositories"
 
     @staticmethod
     def name():
         return "WebRSync"
 
@@ -129,21 +137,28 @@
             return (exitcode, True)
         finally:
             if openpgp_env is not None:
                 openpgp_env.close()
 
 
 class PyWebRsync(SyncBase):
-    """WebRSync sync class"""
+    """PyWebRsync sync class
+
+    TODO: Implement the sync parts from the emerge-webrsync external
+          binary to avoid split logic for various components, which
+          is how we ended up with bug #597800.
+    """
 
     short_desc = "Perform sync operations on webrsync based repositories"
 
     @staticmethod
     def name():
         return "WebRSync"
 
     def __init__(self):
         SyncBase.__init__(self, None, ">=sys-apps/portage-2.3")
 
     def sync(self, **kwargs):
         """Sync the repository"""
-        pass
+        raise NotImplementedError(
+            "Python impl. of webrsync backend is not yet implemented"
+        )
```

### Comparing `portage-3.0.46/lib/portage/sync/old_tree_timestamp.py` & `portage-3.0.47/lib/portage/sync/old_tree_timestamp.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/sync/syncbase.py` & `portage-3.0.47/lib/portage/sync/syncbase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev` & `portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev` & `portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key` & `portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key` & `portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/.gnupg/pubring.kbx` & `portage-3.0.47/lib/portage/tests/.gnupg/pubring.kbx`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/.gnupg/trustdb.gpg` & `portage-3.0.47/lib/portage/tests/.gnupg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/__init__.py` & `portage-3.0.47/lib/portage/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/bin/setup_env.py` & `portage-3.0.47/lib/portage/tests/bin/setup_env.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/bin/test_dobin.py` & `portage-3.0.47/lib/portage/tests/bin/test_dobin.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/bin/test_dodir.py` & `portage-3.0.47/lib/portage/tests/bin/test_dodir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/bin/test_doins.py` & `portage-3.0.47/lib/portage/tests/bin/test_doins.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/bin/test_eapi7_ver_funcs.py` & `portage-3.0.47/lib/portage/tests/bin/test_eapi7_ver_funcs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/bin/test_filter_bash_env.py` & `portage-3.0.47/lib/portage/tests/bin/test_filter_bash_env.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dbapi/test_auxdb.py` & `portage-3.0.47/lib/portage/tests/dbapi/test_auxdb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dbapi/test_bintree.py` & `portage-3.0.47/lib/portage/tests/dbapi/test_bintree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dbapi/test_fakedbapi.py` & `portage-3.0.47/lib/portage/tests/dbapi/test_fakedbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dbapi/test_portdb_cache.py` & `portage-3.0.47/lib/portage/tests/dbapi/test_portdb_cache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/testAtom.py` & `portage-3.0.47/lib/portage/tests/dep/testAtom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/testCheckRequiredUse.py` & `portage-3.0.47/lib/portage/tests/dep/testCheckRequiredUse.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/testExtendedAtomDict.py` & `portage-3.0.47/lib/portage/tests/dep/testExtendedAtomDict.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/testExtractAffectingUSE.py` & `portage-3.0.47/lib/portage/tests/dep/testExtractAffectingUSE.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/testStandalone.py` & `portage-3.0.47/lib/portage/tests/dep/testStandalone.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_best_match_to_list.py` & `portage-3.0.47/lib/portage/tests/dep/test_best_match_to_list.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_dep_getcpv.py` & `portage-3.0.47/lib/portage/tests/dep/test_dep_getcpv.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_dep_getrepo.py` & `portage-3.0.47/lib/portage/tests/dep/test_dep_getrepo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_dep_getslot.py` & `portage-3.0.47/lib/portage/tests/dep/test_dep_getslot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_dep_getusedeps.py` & `portage-3.0.47/lib/portage/tests/dep/test_dep_getusedeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_dnf_convert.py` & `portage-3.0.47/lib/portage/tests/dep/test_dnf_convert.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_get_operator.py` & `portage-3.0.47/lib/portage/tests/dep/test_get_operator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_get_required_use_flags.py` & `portage-3.0.47/lib/portage/tests/dep/test_get_required_use_flags.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_isjustname.py` & `portage-3.0.47/lib/portage/tests/dep/test_isjustname.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_isvalidatom.py` & `portage-3.0.47/lib/portage/tests/dep/test_isvalidatom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_match_from_list.py` & `portage-3.0.47/lib/portage/tests/dep/test_match_from_list.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_overlap_dnf.py` & `portage-3.0.47/lib/portage/tests/dep/test_overlap_dnf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_paren_reduce.py` & `portage-3.0.47/lib/portage/tests/dep/test_paren_reduce.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_soname_atom_pickle.py` & `portage-3.0.47/lib/portage/tests/dep/test_soname_atom_pickle.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/dep/test_use_reduce.py` & `portage-3.0.47/lib/portage/tests/dep/test_use_reduce.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_array_fromfile_eof.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_array_fromfile_eof.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_config.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_doebuild_spawn.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_doebuild_spawn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_fetch.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_fetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_ipc_daemon.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_ipc_daemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_shell_quote.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_shell_quote.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_spawn.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_spawn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/ebuild/test_use_expand_incremental.py` & `portage-3.0.47/lib/portage/tests/ebuild/test_use_expand_incremental.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/emerge/test_actions.py` & `portage-3.0.47/lib/portage/tests/emerge/test_actions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/emerge/test_config_protect.py` & `portage-3.0.47/lib/portage/tests/emerge/test_config_protect.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py` & `portage-3.0.47/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/emerge/test_emerge_slot_abi.py` & `portage-3.0.47/lib/portage/tests/emerge/test_emerge_slot_abi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/emerge/test_global_updates.py` & `portage-3.0.47/lib/portage/tests/emerge/test_global_updates.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/emerge/test_simple.py` & `portage-3.0.47/lib/portage/tests/emerge/test_simple.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/env/config/test_PackageKeywordsFile.py` & `portage-3.0.47/lib/portage/tests/env/config/test_PackageKeywordsFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/env/config/test_PackageMaskFile.py` & `portage-3.0.47/lib/portage/tests/env/config/test_PackageMaskFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/env/config/test_PackageUseFile.py` & `portage-3.0.47/lib/portage/tests/env/config/test_PackageUseFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/env/config/test_PortageModulesFile.py` & `portage-3.0.47/lib/portage/tests/env/config/test_PortageModulesFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/glsa/test_security_set.py` & `portage-3.0.47/lib/portage/tests/glsa/test_security_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_checksum.py` & `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_gpg.py` & `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_gpg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_metadata_update.py` & `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_metadata_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_metadata_url.py` & `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_metadata_url.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_path.py` & `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_size.py` & `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_size.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/gpkg/test_gpkg_stream.py` & `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_stream.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/lafilefixer/test_lafilefixer.py` & `portage-3.0.47/lib/portage/tests/lafilefixer/test_lafilefixer.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py` & `portage-3.0.47/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/lazyimport/test_preload_portage_submodules.py` & `portage-3.0.47/lib/portage/tests/lazyimport/test_preload_portage_submodules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/lint/test_bash_syntax.py` & `portage-3.0.47/lib/portage/tests/lint/test_bash_syntax.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/lint/test_compile_modules.py` & `portage-3.0.47/lib/portage/tests/lint/test_compile_modules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/lint/test_import_modules.py` & `portage-3.0.47/lib/portage/tests/lint/test_import_modules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/locks/test_asynchronous_lock.py` & `portage-3.0.47/lib/portage/tests/locks/test_asynchronous_lock.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/locks/test_lock_nonblock.py` & `portage-3.0.47/lib/portage/tests/locks/test_lock_nonblock.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/news/test_NewsItem.py` & `portage-3.0.47/lib/portage/tests/news/test_NewsItem.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/process/test_AsyncFunction.py` & `portage-3.0.47/lib/portage/tests/process/test_AsyncFunction.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/process/test_PipeLogger.py` & `portage-3.0.47/lib/portage/tests/process/test_PipeLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/process/test_PopenProcess.py` & `portage-3.0.47/lib/portage/tests/process/test_PopenProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/process/test_PopenProcessBlockingIO.py` & `portage-3.0.47/lib/portage/tests/process/test_PopenProcessBlockingIO.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/process/test_poll.py` & `portage-3.0.47/lib/portage/tests/process/test_poll.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/process/test_spawn_fail_e2big.py` & `portage-3.0.47/lib/portage/tests/process/test_spawn_fail_e2big.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/process/test_spawn_warn_large_env.py` & `portage-3.0.47/lib/portage/tests/process/test_spawn_warn_large_env.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/process/test_unshare_net.py` & `portage-3.0.47/lib/portage/tests/process/test_unshare_net.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/ResolverPlayground.py` & `portage-3.0.47/lib/portage/tests/resolver/ResolverPlayground.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py` & `portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py` & `portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_autounmask.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_depclean.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_depclean.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_downgrade.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_or_choices.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_or_choices.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_reinstall.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_reinstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_skip_update.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_skip_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_slot_conflict_update.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_slot_conflict_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_soname_provided.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_soname_provided.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_unsatisfiable.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_unsatisfiable.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/soname/test_unsatisfied.py` & `portage-3.0.47/lib/portage/tests/resolver/soname/test_unsatisfied.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py` & `portage-3.0.47/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_autounmask.py` & `portage-3.0.47/lib/portage/tests/resolver/test_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_autounmask_binpkg_use.py` & `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_binpkg_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_autounmask_keep_keywords.py` & `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_keep_keywords.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_autounmask_multilib_use.py` & `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_multilib_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_autounmask_parent.py` & `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_parent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_autounmask_use_backtrack.py` & `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_backtrack.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_autounmask_use_breakage.py` & `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_breakage.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py` & `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_backtracking.py` & `portage-3.0.47/lib/portage/tests/resolver/test_backtracking.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_bdeps.py` & `portage-3.0.47/lib/portage/tests/resolver/test_bdeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py` & `portage-3.0.47/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_blocker.py` & `portage-3.0.47/lib/portage/tests/resolver/test_blocker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_changed_deps.py` & `portage-3.0.47/lib/portage/tests/resolver/test_changed_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_circular_choices.py` & `portage-3.0.47/lib/portage/tests/resolver/test_circular_choices.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_circular_choices_rust.py` & `portage-3.0.47/lib/portage/tests/resolver/test_circular_choices_rust.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_circular_dependencies.py` & `portage-3.0.47/lib/portage/tests/resolver/test_circular_dependencies.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_complete_graph.py` & `portage-3.0.47/lib/portage/tests/resolver/test_complete_graph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py` & `portage-3.0.47/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_depclean.py` & `portage-3.0.47/lib/portage/tests/resolver/test_depclean.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_depclean_order.py` & `portage-3.0.47/lib/portage/tests/resolver/test_depclean_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_depclean_slot_unavailable.py` & `portage-3.0.47/lib/portage/tests/resolver/test_depclean_slot_unavailable.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_depth.py` & `portage-3.0.47/lib/portage/tests/resolver/test_depth.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_disjunctive_depend_order.py` & `portage-3.0.47/lib/portage/tests/resolver/test_disjunctive_depend_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_eapi.py` & `portage-3.0.47/lib/portage/tests/resolver/test_eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_features_test_use.py` & `portage-3.0.47/lib/portage/tests/resolver/test_features_test_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py` & `portage-3.0.47/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_installkernel.py` & `portage-3.0.47/lib/portage/tests/resolver/test_installkernel.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_keywords.py` & `portage-3.0.47/lib/portage/tests/resolver/test_keywords.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_merge_order.py` & `portage-3.0.47/lib/portage/tests/resolver/test_merge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py` & `portage-3.0.47/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_multirepo.py` & `portage-3.0.47/lib/portage/tests/resolver/test_multirepo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_multislot.py` & `portage-3.0.47/lib/portage/tests/resolver/test_multislot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_old_dep_chain_display.py` & `portage-3.0.47/lib/portage/tests/resolver/test_old_dep_chain_display.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_onlydeps.py` & `portage-3.0.47/lib/portage/tests/resolver/test_onlydeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_onlydeps_circular.py` & `portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_circular.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_onlydeps_ideps.py` & `portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_ideps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_onlydeps_minimal.py` & `portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_minimal.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_or_choices.py` & `portage-3.0.47/lib/portage/tests/resolver/test_or_choices.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_or_downgrade_installed.py` & `portage-3.0.47/lib/portage/tests/resolver/test_or_downgrade_installed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_or_upgrade_installed.py` & `portage-3.0.47/lib/portage/tests/resolver/test_or_upgrade_installed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_output.py` & `portage-3.0.47/lib/portage/tests/resolver/test_output.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_package_tracker.py` & `portage-3.0.47/lib/portage/tests/resolver/test_package_tracker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_profile_default_eapi.py` & `portage-3.0.47/lib/portage/tests/resolver/test_profile_default_eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_profile_package_set.py` & `portage-3.0.47/lib/portage/tests/resolver/test_profile_package_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_rebuild.py` & `portage-3.0.47/lib/portage/tests/resolver/test_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py` & `portage-3.0.47/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_required_use.py` & `portage-3.0.47/lib/portage/tests/resolver/test_required_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py` & `portage-3.0.47/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_simple.py` & `portage-3.0.47/lib/portage/tests/resolver/test_simple.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_abi.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_abi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_abi_downgrade.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_abi_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_change_without_revbump.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_change_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_collisions.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_collisions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_mask_update.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_mask_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_rebuild.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_update.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_conflict_update_virt.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_update_virt.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_autounmask.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_bdeps.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_bdeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_complete_graph.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_complete_graph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_missed_update.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_missed_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_rebuild.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_required_use.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_required_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_unsolved.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_unsolved.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py` & `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py` & `portage-3.0.47/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_targetroot.py` & `portage-3.0.47/lib/portage/tests/resolver/test_targetroot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_unecessary_slot_upgrade.py` & `portage-3.0.47/lib/portage/tests/resolver/test_unecessary_slot_upgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_unmerge_order.py` & `portage-3.0.47/lib/portage/tests/resolver/test_unmerge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_update.py` & `portage-3.0.47/lib/portage/tests/resolver/test_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_use_dep_defaults.py` & `portage-3.0.47/lib/portage/tests/resolver/test_use_dep_defaults.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_useflags.py` & `portage-3.0.47/lib/portage/tests/resolver/test_useflags.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_virtual_minimize_children.py` & `portage-3.0.47/lib/portage/tests/resolver/test_virtual_minimize_children.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_virtual_slot.py` & `portage-3.0.47/lib/portage/tests/resolver/test_virtual_slot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/resolver/test_with_test_deps.py` & `portage-3.0.47/lib/portage/tests/resolver/test_with_test_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/runTests.py` & `portage-3.0.47/lib/portage/tests/runTests.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/sets/base/testInternalPackageSet.py` & `portage-3.0.47/lib/portage/tests/sets/base/testInternalPackageSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/sets/base/testVariableSet.py` & `portage-3.0.47/lib/portage/tests/sets/base/testVariableSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/sets/files/testConfigFileSet.py` & `portage-3.0.47/lib/portage/tests/sets/files/testConfigFileSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/sets/files/testStaticFileSet.py` & `portage-3.0.47/lib/portage/tests/sets/files/testStaticFileSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/sets/shell/testShell.py` & `portage-3.0.47/lib/portage/tests/sets/shell/testShell.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/sync/test_sync_local.py` & `portage-3.0.47/lib/portage/tests/sync/test_sync_local.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/unicode/test_string_format.py` & `portage-3.0.47/lib/portage/tests/unicode/test_string_format.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/update/test_move_ent.py` & `portage-3.0.47/lib/portage/tests/update/test_move_ent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/update/test_move_slot_ent.py` & `portage-3.0.47/lib/portage/tests/update/test_move_slot_ent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/update/test_update_dbentry.py` & `portage-3.0.47/lib/portage/tests/update/test_update_dbentry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/dyn_libs/test_soname_deps.py` & `portage-3.0.47/lib/portage/tests/util/dyn_libs/test_soname_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/eventloop/test_call_soon_fifo.py` & `portage-3.0.47/lib/portage/tests/util/eventloop/test_call_soon_fifo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/file_copy/test_copyfile.py` & `portage-3.0.47/lib/portage/tests/util/file_copy/test_copyfile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_child_watcher.py` & `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_child_watcher.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py` & `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py` & `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py` & `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py` & `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py` & `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py` & `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/test_compat_coroutine.py` & `portage-3.0.47/lib/portage/tests/util/futures/test_compat_coroutine.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/test_done_callback.py` & `portage-3.0.47/lib/portage/tests/util/futures/test_done_callback.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/test_done_callback_after_exit.py` & `portage-3.0.47/lib/portage/tests/util/futures/test_done_callback_after_exit.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/test_iter_completed.py` & `portage-3.0.47/lib/portage/tests/util/futures/test_iter_completed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/futures/test_retry.py` & `portage-3.0.47/lib/portage/tests/util/futures/test_retry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_checksum.py` & `portage-3.0.47/lib/portage/tests/util/test_checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_digraph.py` & `portage-3.0.47/lib/portage/tests/util/test_digraph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_file_copier.py` & `portage-3.0.47/lib/portage/tests/util/test_file_copier.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_getconfig.py` & `portage-3.0.47/lib/portage/tests/util/test_getconfig.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_install_mask.py` & `portage-3.0.47/lib/portage/tests/util/test_install_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_manifest.py` & `portage-3.0.47/lib/portage/tests/util/test_manifest.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_mtimedb.py` & `portage-3.0.47/lib/portage/tests/util/test_mtimedb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_shelve.py` & `portage-3.0.47/lib/portage/tests/util/test_shelve.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_socks5.py` & `portage-3.0.47/lib/portage/tests/util/test_socks5.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_stackDictList.py` & `portage-3.0.47/lib/portage/tests/util/test_stackDictList.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_stackDicts.py` & `portage-3.0.47/lib/portage/tests/util/test_stackDicts.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_stackLists.py` & `portage-3.0.47/lib/portage/tests/util/test_stackLists.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_uniqueArray.py` & `portage-3.0.47/lib/portage/tests/util/test_uniqueArray.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_varExpand.py` & `portage-3.0.47/lib/portage/tests/util/test_varExpand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_whirlpool.py` & `portage-3.0.47/lib/portage/tests/util/test_whirlpool.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/util/test_xattr.py` & `portage-3.0.47/lib/portage/tests/util/test_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/versions/test_cpv_sort_key.py` & `portage-3.0.47/lib/portage/tests/versions/test_cpv_sort_key.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/tests/versions/test_vercmp.py` & `portage-3.0.47/lib/portage/tests/versions/test_vercmp.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/update.py` & `portage-3.0.47/lib/portage/update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/ExtractKernelVersion.py` & `portage-3.0.47/lib/portage/util/ExtractKernelVersion.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/SlotObject.py` & `portage-3.0.47/lib/portage/util/SlotObject.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/__init__.py` & `portage-3.0.47/lib/portage/util/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/AsyncFunction.py` & `portage-3.0.47/lib/portage/util/_async/AsyncFunction.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/AsyncScheduler.py` & `portage-3.0.47/lib/portage/util/_async/AsyncScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/AsyncTaskFuture.py` & `portage-3.0.47/lib/portage/util/_async/AsyncTaskFuture.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/BuildLogger.py` & `portage-3.0.47/lib/portage/util/_async/BuildLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/FileCopier.py` & `portage-3.0.47/lib/portage/util/_async/FileCopier.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/FileDigester.py` & `portage-3.0.47/lib/portage/util/_async/FileDigester.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/ForkProcess.py` & `portage-3.0.47/lib/portage/util/_async/ForkProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/PipeLogger.py` & `portage-3.0.47/lib/portage/util/_async/PipeLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/PipeReaderBlockingIO.py` & `portage-3.0.47/lib/portage/util/_async/PipeReaderBlockingIO.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/PopenProcess.py` & `portage-3.0.47/lib/portage/util/_async/PopenProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/SchedulerInterface.py` & `portage-3.0.47/lib/portage/util/_async/SchedulerInterface.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/TaskScheduler.py` & `portage-3.0.47/lib/portage/util/_async/TaskScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_async/run_main_scheduler.py` & `portage-3.0.47/lib/portage/util/_async/run_main_scheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_compare_files.py` & `portage-3.0.47/lib/portage/util/_compare_files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_ctypes.py` & `portage-3.0.47/lib/portage/util/_ctypes.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_desktop_entry.py` & `portage-3.0.47/lib/portage/util/_desktop_entry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_dyn_libs/LinkageMapELF.py` & `portage-3.0.47/lib/portage/util/_dyn_libs/LinkageMapELF.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_dyn_libs/NeededEntry.py` & `portage-3.0.47/lib/portage/util/_dyn_libs/NeededEntry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py` & `portage-3.0.47/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_dyn_libs/display_preserved_libs.py` & `portage-3.0.47/lib/portage/util/_dyn_libs/display_preserved_libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_dyn_libs/dyn_libs.py` & `portage-3.0.47/lib/portage/util/_dyn_libs/dyn_libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_dyn_libs/soname_deps.py` & `portage-3.0.47/lib/portage/util/_dyn_libs/soname_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_dyn_libs/soname_deps_qa.py` & `portage-3.0.47/lib/portage/util/_dyn_libs/soname_deps_qa.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_eventloop/asyncio_event_loop.py` & `portage-3.0.47/lib/portage/util/_eventloop/asyncio_event_loop.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_get_vm_info.py` & `portage-3.0.47/lib/portage/util/_get_vm_info.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_info_files.py` & `portage-3.0.47/lib/portage/util/_info_files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_path.py` & `portage-3.0.47/lib/portage/util/_path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_pty.py` & `portage-3.0.47/lib/portage/util/_pty.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_urlopen.py` & `portage-3.0.47/lib/portage/util/_urlopen.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/_xattr.py` & `portage-3.0.47/lib/portage/util/_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/backoff.py` & `portage-3.0.47/lib/portage/util/backoff.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/bin_entry_point.py` & `portage-3.0.47/lib/portage/util/bin_entry_point.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/changelog.py` & `portage-3.0.47/lib/portage/util/changelog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/compression_probe.py` & `portage-3.0.47/lib/portage/util/compression_probe.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/configparser.py` & `portage-3.0.47/lib/portage/util/configparser.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/cpuinfo.py` & `portage-3.0.47/lib/portage/util/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/digraph.py` & `portage-3.0.47/lib/portage/util/digraph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/elf/constants.py` & `portage-3.0.47/lib/portage/util/elf/constants.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/elf/header.py` & `portage-3.0.47/lib/portage/util/elf/header.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/endian/decode.py` & `portage-3.0.47/lib/portage/util/endian/decode.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/env_update.py` & `portage-3.0.47/lib/portage/util/env_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/file_copy/__init__.py` & `portage-3.0.47/lib/portage/util/file_copy/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/formatter.py` & `portage-3.0.47/lib/portage/util/formatter.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/_asyncio/__init__.py` & `portage-3.0.47/lib/portage/util/futures/_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/_asyncio/streams.py` & `portage-3.0.47/lib/portage/util/futures/_asyncio/streams.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/_sync_decorator.py` & `portage-3.0.47/lib/portage/util/futures/_sync_decorator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/compat_coroutine.py` & `portage-3.0.47/lib/portage/util/futures/compat_coroutine.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/executor/fork.py` & `portage-3.0.47/lib/portage/util/futures/executor/fork.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/extendedfutures.py` & `portage-3.0.47/lib/portage/util/futures/extendedfutures.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/futures.py` & `portage-3.0.47/lib/portage/util/futures/futures.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/iter_completed.py` & `portage-3.0.47/lib/portage/util/futures/iter_completed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/retry.py` & `portage-3.0.47/lib/portage/util/futures/retry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/futures/unix_events.py` & `portage-3.0.47/lib/portage/util/futures/unix_events.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/hooks.py` & `portage-3.0.47/lib/portage/util/hooks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/install_mask.py` & `portage-3.0.47/lib/portage/util/install_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/iterators/MultiIterGroupBy.py` & `portage-3.0.47/lib/portage/util/iterators/MultiIterGroupBy.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/lafilefixer.py` & `portage-3.0.47/lib/portage/util/lafilefixer.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/listdir.py` & `portage-3.0.47/lib/portage/util/listdir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/locale.py` & `portage-3.0.47/lib/portage/util/locale.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/movefile.py` & `portage-3.0.47/lib/portage/util/movefile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/mtimedb.py` & `portage-3.0.47/lib/portage/util/mtimedb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/netlink.py` & `portage-3.0.47/lib/portage/util/netlink.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/path.py` & `portage-3.0.47/lib/portage/util/path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/shelve.py` & `portage-3.0.47/lib/portage/util/shelve.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/socks5.py` & `portage-3.0.47/lib/portage/util/socks5.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/whirlpool.py` & `portage-3.0.47/lib/portage/util/whirlpool.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/util/writeable_check.py` & `portage-3.0.47/lib/portage/util/writeable_check.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/versions.py` & `portage-3.0.47/lib/portage/versions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/xml/metadata.py` & `portage-3.0.47/lib/portage/xml/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/lib/portage/xpak.py` & `portage-3.0.47/lib/portage/xpak.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/misc/emerge-delta-webrsync` & `portage-3.0.47/misc/emerge-delta-webrsync`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/setup.py` & `portage-3.0.47/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,15 +813,15 @@
         return list(venv_data_files(venv_files))
 
     return regular_files
 
 
 setup(
     name="portage",
-    version="3.0.46",
+    version="3.0.47",
     url="https://wiki.gentoo.org/wiki/Project:Portage",
     project_urls={
         "Release Notes": "https://gitweb.gentoo.org/proj/portage.git/plain/NEWS",
         "Documentation": "https://wiki.gentoo.org/wiki/Handbook:AMD64/Working/Portage",
     },
     author="Gentoo Portage Development Team",
     author_email="dev-portage@gentoo.org",
```

### Comparing `portage-3.0.46/src/portage_util__whirlpool.c` & `portage-3.0.47/src/portage_util__whirlpool.c`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/src/portage_util_file_copy_reflink_linux.c` & `portage-3.0.47/src/portage_util_file_copy_reflink_linux.c`

 * *Files identical despite different names*

### Comparing `portage-3.0.46/src/portage_util_libc.c` & `portage-3.0.47/src/portage_util_libc.c`

 * *Files identical despite different names*

