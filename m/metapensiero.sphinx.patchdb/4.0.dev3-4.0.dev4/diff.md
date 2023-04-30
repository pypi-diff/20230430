# Comparing `tmp/metapensiero.sphinx.patchdb-4.0.dev3.tar.gz` & `tmp/metapensiero.sphinx.patchdb-4.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev3.tar", last modified: Wed Feb 15 21:25:25 2023, max compression
+gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev4.tar", last modified: Sun Apr 30 15:01:29 2023, max compression
```

## Comparing `metapensiero.sphinx.patchdb-4.0.dev3.tar` & `metapensiero.sphinx.patchdb-4.0.dev4.tar`

### file list

```diff
@@ -1,44 +1,42 @@
--rw-r--r--   0        0        0     3111 2023-02-15 21:19:53.803277 metapensiero.sphinx.patchdb-4.0.dev3/CHANGES.rst
--rw-r--r--   0        0        0      514 2022-06-26 14:58:56.058722 metapensiero.sphinx.patchdb-4.0.dev3/Makefile
--rw-r--r--   0        0        0     1535 2017-09-27 22:05:34.323507 metapensiero.sphinx.patchdb-4.0.dev3/Makefile.i18n
--rw-r--r--   0        0        0     1982 2022-07-22 08:59:56.221874 metapensiero.sphinx.patchdb-4.0.dev3/Makefile.release
--rw-r--r--   0        0        0    10656 2017-11-02 16:23:19.429652 metapensiero.sphinx.patchdb-4.0.dev3/OLDERCHANGES.rst
--rw-r--r--   0        0        0    29250 2023-02-15 18:17:58.449422 metapensiero.sphinx.patchdb-4.0.dev3/README.rst
--rw-r--r--   0        0        0      992 2023-02-15 18:40:10.613110 metapensiero.sphinx.patchdb-4.0.dev3/flake.lock
--rw-r--r--   0        0        0     2616 2023-02-15 18:56:48.785996 metapensiero.sphinx.patchdb-4.0.dev3/flake.nix
--rw-r--r--   0        0        0     1749 2023-02-15 21:17:21.012926 metapensiero.sphinx.patchdb-4.0.dev3/pyproject.toml
--rw-r--r--   0        0        0      697 2021-10-03 08:45:32.130393 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/__init__.py
--rw-r--r--   0        0        0     7174 2021-10-13 11:20:11.798784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/__init__.py
--rw-r--r--   0        0        0     3545 2021-10-13 11:20:11.798784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/firebird.py
--rw-r--r--   0        0        0     4692 2021-10-13 11:20:11.798784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/mysql.py
--rw-r--r--   0        0        0     4289 2021-10-13 11:20:11.798784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/postgres.py
--rw-r--r--   0        0        0     1505 2021-10-03 08:49:54.268009 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/python.py
--rw-r--r--   0        0        0    16929 2021-10-13 11:20:11.798784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/sql.py
--rw-r--r--   0        0        0     3858 2021-10-13 11:20:11.798784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
--rw-r--r--   0        0        0     1546 2021-10-13 11:20:11.798784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/locale/__init__.py
--rw-r--r--   0        0        0     8569 2023-02-15 21:25:20.675738 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.mo
--rw-r--r--   0        0        0    12679 2023-02-15 21:17:22.212913 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
--rw-r--r--   0        0        0      285 2016-11-17 16:37:17.501177 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
--rw-r--r--   0        0        0     8755 2023-02-15 21:17:21.720919 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
--rw-r--r--   0        0        0    13628 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/manager.py
--rw-r--r--   0        0        0    14392 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/patch.py
--rw-r--r--   0        0        0     8827 2022-06-26 16:43:17.100329 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/pup.py
--rw-r--r--   0        0        0    24175 2023-02-15 20:34:52.928540 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/script.py
--rw-r--r--   0        0        0     7257 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/states.py
--rw-r--r--   0        0        0     7644 2023-02-15 20:08:32.746466 metapensiero.sphinx.patchdb-4.0.dev3/tests/fixtures.py
--rw-r--r--   0        0        0     7111 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_bad.py
--rw-r--r--   0        0        0     4424 2023-02-15 20:08:34.746442 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_drops.py
--rw-r--r--   0        0        0     1182 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_external_file.py
--rw-r--r--   0        0        0     4182 2021-10-03 08:50:51.055486 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_helpers.py
--rw-r--r--   0        0        0     4577 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_manager.py
--rw-r--r--   0        0        0     2284 2021-10-03 08:50:55.431445 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_modular.py
--rw-r--r--   0        0        0     2927 2021-10-03 08:50:57.083430 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_patch.py
--rw-r--r--   0        0        0     2766 2021-10-03 08:50:58.307419 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_python.py
--rw-r--r--   0        0        0     7007 2021-10-03 08:50:59.627407 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_revisions.py
--rw-r--r--   0        0        0     4632 2022-03-21 07:48:01.248519 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_sql.py
--rw-r--r--   0        0        0     2291 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_sql_fb.py
--rw-r--r--   0        0        0     4328 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_sql_ms.py
--rw-r--r--   0        0        0     2501 2021-10-13 11:20:11.802784 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_sql_pg.py
--rw-r--r--   0        0        0     2822 2021-10-03 08:51:11.223301 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_states.py
--rw-r--r--   0        0        0     2094 2021-10-03 08:51:13.179283 metapensiero.sphinx.patchdb-4.0.dev3/tests/test_variables.py
--rw-r--r--   0        0        0    30343 1970-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     3506 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/CHANGES.rst
+-rw-r--r--   0        0        0      609 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/Makefile
+-rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/OLDERCHANGES.rst
+-rw-r--r--   0        0        0    30372 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/README.rst
+-rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/flake.lock
+-rw-r--r--   0        0        0     4144 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/flake.nix
+-rw-r--r--   0        0        0     1751 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/__init__.py
+-rw-r--r--   0        0        0     7174 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/__init__.py
+-rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/firebird.py
+-rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/mysql.py
+-rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/postgres.py
+-rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/python.py
+-rw-r--r--   0        0        0    17886 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/sql.py
+-rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
+-rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/__init__.py
+-rw-r--r--   0        0        0    12981 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
+-rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
+-rw-r--r--   0        0        0     8864 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
+-rw-r--r--   0        0        0    13600 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/manager.py
+-rw-r--r--   0        0        0    14938 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/patch.py
+-rw-r--r--   0        0        0     8782 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/pup.py
+-rw-r--r--   0        0        0    24367 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/script.py
+-rw-r--r--   0        0        0     7257 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/states.py
+-rw-r--r--   0        0        0     8030 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/fixtures.py
+-rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/postgresql
+-rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_bad.py
+-rw-r--r--   0        0        0     4424 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_drops.py
+-rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_external_file.py
+-rw-r--r--   0        0        0     4182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_helpers.py
+-rw-r--r--   0        0        0     4577 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_manager.py
+-rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_modular.py
+-rw-r--r--   0        0        0     3537 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_patch.py
+-rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_python.py
+-rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_revisions.py
+-rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql.py
+-rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_fb.py
+-rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_ms.py
+-rw-r--r--   0        0        0     7631 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_pg.py
+-rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_states.py
+-rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_variables.py
+-rw-r--r--   0        0        0    31467 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/PKG-INFO
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/CHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev4/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changes\ [#]_
 -------------
 
+4.0.dev4 (2023-04-30)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Make ``--backups-dir`` an *opt-in* option, perform a pre-backup only when a directory is
+  specified (and different from ``None``, for backward compatibility).
+
+* Introduce a variant of pinned dependency, ``patchid@*``, to denote the *currently applied*
+  revision of the patch or the highest available, if not already applied
+
+* Drop Python 3.9
+
+
 4.0.dev3 (2023-02-15)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Silence warning about a missing dependency in patch that drops it
 
 
 4.0.dev2 (2022-07-22)
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/OLDERCHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev4/OLDERCHANGES.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/README.rst` & `metapensiero.sphinx.patchdb-4.0.dev4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ========================================================
 
 :version: 4
 :author: Lele Gaifax <lele@metapensiero.it>
 :license: GPLv3
 
 Building and maintaining the schema of a database is always a challenge. It may quickly become
-a nightmare when dealing with even moderately complex databases, in a distribuited development
+a nightmare when dealing with even moderately complex databases, in a distributed development
 environment. You have new features going in, and fixes here and there, that keeps accumulating
 in the development `branch`. You also have several already deployed instances of the database
 you wanna upgrade now and then.
 
 In my experience, it's very difficult to impossible to come up with a completely automated
 solution, for several reasons:
 
@@ -49,14 +49,19 @@
 
 .. [*] Just to mention a few alternatives:
 
        `Alembic <https://pypi.python.org/pypi/alembic>`_
          Written on top of SQLAlchemy_ by the same author: it does not help when you need to
          manage something outside SA knowledge (stored procedures, permissions, …)
 
+       `Pyrseas <https://pyrseas.readthedocs.io/en/latest/>`_
+         ``PostgreSQL`` specific tool, able to distill an ``SQL`` script comparing between a ``YAML``
+         description of the schema and the actual one: interesting project, but does not handle
+         *data* migration
+
        `Sqlibrist <https://pypi.python.org/pypi/sqlibrist>`_
          Some similarities with PatchDB, very young, Django integration.
 
        `Sqitch <http://sqitch.org/>`_
          Quite good, *although* Perl based…
 
        See the `schema migration <https://en.wikipedia.org/wiki/Schema_migration>`_ page on
@@ -416,14 +421,28 @@
 
 When ``patchdb`` examines the database status, it will execute one *or* the other. If the
 script `Create master table` isn't executed yet (for example when operating on a new database),
 it will take the former script (the one that creates the table from scratch).  Otherwise, if
 the database "contains" revision 1 (and not higher than 1) of the script, it will execute the
 latter, bumping up the revision number.
 
+.. note:: Any single dependency may be either `generic` or `pinned` to a particular `revision`
+          number.
+
+          A generic dependency is one that does not contain a ``@`` character followed by an
+          integer number: in this case ``patchdb`` will consider it pointing to the *highest*
+          known revision of that script.
+
+          A pinned dependency contains the ``@``: what follows may be either a revision number
+          or, **only** for the `depends` ones, the character ``*``, to indicate that any
+          revision is good enough, provided it has been applied. In other words, the asterisk
+          will be replaced by the current revision of the script if it has been already
+          applied, otherwise by its highest known revision, i.e. handled in the same way as an
+          unpinned dependency.
+
 __ master-table_
 
 
 Obsoleted patches
 +++++++++++++++++
 
 Another peculiarity of this kind of scripts is that they may references `non existing scripts`
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/flake.lock` & `metapensiero.sphinx.patchdb-4.0.dev4/flake.lock`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9522569444444443%*

 * *Differences: {"'nodes'": "{'flake-utils': {'locked': {'lastModified': 1680946745, 'narHash': "*

 * *            "'sha256-KqGlwg9UTDsFBZZB8wzXgMnc8XQm95LtSbFvBsnqkPI=', 'rev': "*

 * *            "'946da791763db1c306b86a8bd3828bf5814a1247'}}, 'nixpkgs': {'locked': {'lastModified': "*

 * *            "1680975136, 'narHash': 'sha256-mVXWfWWFV/8aD+Wdsa+UPNXPjrrkfVyg4/FItBcQhPY=', 'rev': "*

 * *            "'7f3f7ec38154b9f4eb551a67bfe4214db43d4200'}}, 'root': {'inputs': {'gitignore': "*

 * *            "'gitignore'}}, 'gitignore': OrderedDict([('inp […]*

```diff
@@ -1,42 +1,63 @@
 {
     "nodes": {
         "flake-utils": {
             "locked": {
-                "lastModified": 1676283394,
-                "narHash": "sha256-XX2f9c3iySLCw54rJ/CZs+ZK6IQy7GXNY4nSOyu2QG4=",
+                "lastModified": 1680946745,
+                "narHash": "sha256-KqGlwg9UTDsFBZZB8wzXgMnc8XQm95LtSbFvBsnqkPI=",
                 "owner": "numtide",
                 "repo": "flake-utils",
-                "rev": "3db36a8b464d0c4532ba1c7dda728f4576d6d073",
+                "rev": "946da791763db1c306b86a8bd3828bf5814a1247",
                 "type": "github"
             },
             "original": {
                 "owner": "numtide",
                 "repo": "flake-utils",
                 "type": "github"
             }
         },
+        "gitignore": {
+            "inputs": {
+                "nixpkgs": [
+                    "nixpkgs"
+                ]
+            },
+            "locked": {
+                "lastModified": 1660459072,
+                "narHash": "sha256-8DFJjXG8zqoONA1vXtgeKXy68KdJL5UaXR8NtVMUbx8=",
+                "owner": "hercules-ci",
+                "repo": "gitignore.nix",
+                "rev": "a20de23b925fd8264fd7fad6454652e142fd7f73",
+                "type": "github"
+            },
+            "original": {
+                "owner": "hercules-ci",
+                "repo": "gitignore.nix",
+                "type": "github"
+            }
+        },
         "nixpkgs": {
             "locked": {
-                "lastModified": 1676483037,
-                "narHash": "sha256-JUz3a7LWymvx1Umvbpc4odF5aCyesmHdwYnck79Uvu0=",
+                "lastModified": 1680975136,
+                "narHash": "sha256-mVXWfWWFV/8aD+Wdsa+UPNXPjrrkfVyg4/FItBcQhPY=",
                 "owner": "NixOS",
                 "repo": "nixpkgs",
-                "rev": "4f1b2d513327b121cbf82b4086b3b854a48347a3",
+                "rev": "7f3f7ec38154b9f4eb551a67bfe4214db43d4200",
                 "type": "github"
             },
             "original": {
                 "owner": "NixOS",
                 "repo": "nixpkgs",
                 "type": "github"
             }
         },
         "root": {
             "inputs": {
                 "flake-utils": "flake-utils",
+                "gitignore": "gitignore",
                 "nixpkgs": "nixpkgs"
             }
         }
     },
     "root": "root",
     "version": 7
 }
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/pyproject.toml` & `metapensiero.sphinx.patchdb-4.0.dev4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [project]
 name = "metapensiero.sphinx.patchdb"
 description = "Extract scripts from a reST document and apply them in order."
-version = "4.0.dev3"
+version = "4.0.dev4"
 authors = [
     { name = "Lele Gaifax", email = "lele@metapensiero.it" },
 ]
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Database",
     "Topic :: Utilities",
     "Framework :: Sphinx :: Extension",
     "Environment :: Console",
     "Natural Language :: English",
     "Natural Language :: Italian",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 dependencies = [
     "enlighten",
     "sqlparse",
 ]
 
 [project.license]
 text = "GPL-3.0-or-later"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/firebird.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/firebird.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/mysql.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/mysql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/postgres.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/postgres.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/python.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/sql.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- Generic SQL script execution context
 # :Created:   sab 31 mag 2014 13:00:48 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2014, 2016, 2017, 2019, 2021 Lele Gaifax
+# :Copyright: © 2014, 2016, 2017, 2019, 2021, 2023 Lele Gaifax
 #
 
 from collections import deque, namedtuple
 from datetime import datetime
 from hashlib import md5 as hash_factory
+from io import TextIOBase
+
+from sqlparse import tokens, lexer
 
 from sqlparse.tokens import Comment, Keyword, Literal, Name, Punctuation, Whitespace
 from sqlparse import tokens
-from sqlparse.keywords import SQL_REGEX
+from sqlparse.keywords import PROCESS_AS_KEYWORD
 from sqlparse.utils import consume
 
 from ..states import State
 from . import logger
 from . import ExecutionContext, ExecutionError
 
 
 def split_script(script):
     """Split the `script` into the single SQL statements.
 
-    The script may be composed zero or more SQL statements, separated by two consecutive
+    The script may be composed by zero or more SQL statements, separated by two consecutive
     semicomma ``;;`` on a line by their own::
 
       CREATE DOMAIN integer_t INTEGER
       ;;
       CREATE DOMAIN string_t VARCHAR(20)
 
     Empty statements are discarded.
@@ -50,50 +53,75 @@
 
     return statements
 
 
 ValuableToken = namedtuple('ValuableToken', 'pos, type, value')
 
 
-def valuable_tokens(statement):
-    "Iterate over `statement`'s tokens, ignoring whitespace and comments."
-
-    # This is basically the sqlparse<0.2 Lexer().get_tokens_unprocessed()
-    # Version 0.2+ does not return the position
-
-    iterable = enumerate(statement)
-    for pos, char in iterable:
-        for rexmatch, action in SQL_REGEX:
-            m = rexmatch(statement, pos)
-
-            if not m:
-                continue
-            elif isinstance(action, tokens._TokenType):
-                consume_pos = m.end() - pos - 1
-                if not (action in Whitespace or action in Comment):
-                    yield ValuableToken(pos, action, m.group())
-            elif callable(action):
-                ttype, value = action(m.group())
-                consume_pos = len(value) - 1
-                if not (ttype in Whitespace or ttype in Comment):
-                    yield ValuableToken(pos, ttype, value)
-
-            consume(iterable, consume_pos)
-            break
+class Lexer(lexer.Lexer):
+    def get_valuable_tokens(self, text, encoding=None):
+        """Iterate over `text`'s tokens, ignoring whitespace and comments.
+
+        It yields ``ValuableToken`` instances.
+        """
+
+        # This is basically the same as get_tokens(), but reports also the position of each
+        # token
+
+        if isinstance(text, TextIOBase):
+            text = text.read()
+
+        if isinstance(text, str):
+            pass
+        elif isinstance(text, bytes):
+            if encoding:
+                text = text.decode(encoding)
+            else:
+                try:
+                    text = text.decode('utf-8')
+                except UnicodeDecodeError:
+                    text = text.decode('unicode-escape')
         else:
-            yield ValuableToken(pos, tokens.Error, char)
+            raise TypeError("Expected text or file-like object, got {!r}".
+                            format(type(text)))
+
+        iterable = enumerate(text)
+        for pos, char in iterable:
+            for rexmatch, action in self._SQL_REGEX:
+                m = rexmatch(text, pos)
+
+                if not m:
+                    continue
+                elif isinstance(action, tokens._TokenType):
+                    consume_pos = m.end() - pos - 1
+                    if not (action in Whitespace or action in Comment):
+                        yield ValuableToken(pos, action, m.group())
+                elif action is PROCESS_AS_KEYWORD:
+                    ttype, value = self.is_keyword(m.group())
+                    consume_pos = len(value) - 1
+                    if not (ttype in Whitespace or ttype in Comment):
+                        yield ValuableToken(pos, ttype, value)
+                else:
+                    breakpoint()
+                    pass
+
+                consume(iterable, consume_pos)
+                break
+            else:
+                yield ValuableToken(pos, tokens.Error, char)
 
 
 def statement_starts_with(statement, expected_tokens):
     """Determine whether `statement` starts with the given set of `expected_tokens`.
 
     Return ``None`` if not, otherwise the remaining tokens.
     """
 
-    tokens = valuable_tokens(statement)
+    lexer = Lexer.get_default_instance()
+    tokens = lexer.get_valuable_tokens(statement)
 
     for etoken in expected_tokens:
         this = next(tokens, None)
         if this is None:
             return None
         ttype = this.type
         tvalue = this.value.upper()
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/contexts/sqlite.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/sqlite.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/locale/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,210 +1,216 @@
 # Italian translations for metapensiero.sphinx.patchdb.
-# Copyright (C) 2016, 2017, 2019, 2021, 2022 Lele Gaifax
+# Copyright (C) 2016, 2017, 2019, 2021, 2022, 2023 Lele Gaifax
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # Lele Gaifax <lele@metapensiero.it>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev1\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev4\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
-"POT-Creation-Date: 2023-02-15 22:17+0100\n"
-"PO-Revision-Date: 2022-06-28 17:49+0200\n"
+"POT-Creation-Date: 2023-04-30 16:25+0200\n"
+"PO-Revision-Date: 2023-04-30 16:28+0200\n"
 "Last-Translator: Lele Gaifax <lele@metapensiero.it>\n"
 "Language: it\n"
 "Language-Team: it <lele@metapensiero.it>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:67
-#: src/metapensiero/sphinx/patchdb/pup.py:90
+#: src/metapensiero/sphinx/patchdb/pup.py:65
+#: src/metapensiero/sphinx/patchdb/pup.py:88
 #, python-format
 msgid ""
 "\n"
 "Error: %s"
 msgstr ""
 "\n"
 "Errore: %s"
 
-#: src/metapensiero/sphinx/patchdb/script.py:294
 #: src/metapensiero/sphinx/patchdb/script.py:422
-#: src/metapensiero/sphinx/patchdb/script.py:442
+#: src/metapensiero/sphinx/patchdb/script.py:444
+msgid " (any revision)"
+msgstr " (qualsiasi revisione)"
+
+#: src/metapensiero/sphinx/patchdb/script.py:294
+#: src/metapensiero/sphinx/patchdb/script.py:424
+#: src/metapensiero/sphinx/patchdb/script.py:446
 #, python-format
 msgid " (revision %(revno)d)"
 msgstr " (revisione %(revno)d)"
 
-#: src/metapensiero/sphinx/patchdb/script.py:492
+#: src/metapensiero/sphinx/patchdb/script.py:496
 msgid "After any other script"
 msgstr "Dopo tutti gli altri script"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:164
+#: src/metapensiero/sphinx/patchdb/pup.py:162
 msgid "Assume missing patches are already applied, do not re-execute them."
 msgstr "Assumi che gli script mancanti siano già stati applicati, non rieseguirli."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:177
+#: src/metapensiero/sphinx/patchdb/pup.py:175
 msgid "Be quiet, emit only error messages."
 msgstr "Emetti solo messaggi di errore."
 
-#: src/metapensiero/sphinx/patchdb/script.py:490
+#: src/metapensiero/sphinx/patchdb/script.py:494
 msgid "Before any other script"
 msgstr "Prima di qualsiasi altro script"
 
-#: src/metapensiero/sphinx/patchdb/script.py:460
+#: src/metapensiero/sphinx/patchdb/script.py:464
 msgid "Brings"
 msgstr "Implementa"
 
-#: src/metapensiero/sphinx/patchdb/script.py:482
+#: src/metapensiero/sphinx/patchdb/script.py:486
 msgid "Condition"
 msgstr "Condizione"
 
-#: src/metapensiero/sphinx/patchdb/script.py:474
+#: src/metapensiero/sphinx/patchdb/script.py:478
 msgid "Conditions"
 msgstr "Condizioni"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:132
+#: src/metapensiero/sphinx/patchdb/pup.py:130
 msgid "Database script applier"
 msgstr "Database script applier"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:171
+#: src/metapensiero/sphinx/patchdb/pup.py:169
 msgid ""
 "Define an arbitrary variable usable as “{{VARNAME}}” within a script. VAR"
 " must be something like “varname=value”. This option may be given "
 "multiple times."
 msgstr ""
 "Definisce una variabile arbitraria usabile come “{{VARNAME}}” in uno "
 "script. VAR deve essere qualche cosa nella forma “nomevariabile=valore”. "
 "Questa opzione può essere specificata più di una volta."
 
-#: src/metapensiero/sphinx/patchdb/script.py:458
+#: src/metapensiero/sphinx/patchdb/script.py:462
 msgid "Depends on"
 msgstr "Dipende da"
 
-#: src/metapensiero/sphinx/patchdb/script.py:464
+#: src/metapensiero/sphinx/patchdb/script.py:468
 msgid "Direct dependants"
 msgstr "Dipendenze dirette"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:175
+#: src/metapensiero/sphinx/patchdb/pup.py:173
 msgid "Don't apply patches, just list them."
 msgstr "Non applicare gli script, elencali solamente."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:84
+#: src/metapensiero/sphinx/patchdb/pup.py:82
 #, python-format
 msgid "Done, applied %d script"
 msgid_plural "Done, applied %d scripts"
 msgstr[0] "Fatto, applicato %d script"
 msgstr[1] "Fatto, applicati %d script"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:159
+#: src/metapensiero/sphinx/patchdb/pup.py:157
 msgid "Driver to access MySQL, defaults to “pymysql”."
 msgstr "Driver per accedere a MySQL, di default “pymysql”."
 
-#: src/metapensiero/sphinx/patchdb/script.py:461
+#: src/metapensiero/sphinx/patchdb/script.py:465
 msgid "Drops"
 msgstr "Elimina"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:179
+#: src/metapensiero/sphinx/patchdb/pup.py:177
 msgid "Emit debug messages."
 msgstr "Emetti i messaggi di debug."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:157
+#: src/metapensiero/sphinx/patchdb/pup.py:155
 msgid "Encoding used by the MySQL driver, defaults to “utf8mb4”."
 msgstr "Codifica usata dal driver MySQL, di default “utf8mb4”."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:47
+#: src/metapensiero/sphinx/patchdb/pup.py:45
 #, python-format
 msgid "Error: %s"
 msgstr "Errore: %s"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:96
+#: src/metapensiero/sphinx/patchdb/pup.py:94
 msgid "Error: circular dependencies among scripts"
 msgstr "Errore: dipendenze cicliche tra gli script"
 
-#: src/metapensiero/sphinx/patchdb/script.py:488
+#: src/metapensiero/sphinx/patchdb/script.py:492
 msgid "Execute always"
 msgstr "Applicato ogni volta"
 
 #: src/metapensiero/sphinx/patchdb/script.py:233
 msgid "File insertion disabled"
 msgstr "Inclusione disabilitata"
 
-#: src/metapensiero/sphinx/patchdb/script.py:502
+#: src/metapensiero/sphinx/patchdb/script.py:506
 msgid ""
 "Go on with the next script, skipping any succeding statements of the "
 "failing script"
 msgstr ""
 "Continua con il prossimo script, saltando le istruzioni successive a "
 "quella che ha generato l'errore"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:153
+#: src/metapensiero/sphinx/patchdb/pup.py:151
 msgid "Host name where MySQL server runs, defaults to “localhost”."
 msgstr "Nome dell'host del server MySQL, di default “localhost”."
 
-#: src/metapensiero/sphinx/patchdb/script.py:506
+#: src/metapensiero/sphinx/patchdb/script.py:510
 msgid ""
 "Ignore the error and keeps going with the remaining statements in the "
 "script"
 msgstr "Ignora gli errore e prosegui con le istruzioni successive dello script"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:167
+#: src/metapensiero/sphinx/patchdb/pup.py:165
 msgid ""
 "Introduce an arbitrary assertion usable as a pre-condition by the "
 "scripts. NAME may be a simple string or something like “production=true”."
 " This option may be given multiple times."
 msgstr ""
 "Introduce una affermazione arbitraria usabile come precondizione in uno "
 "script. NAME può essere una semplice stringa oppure nella forma "
 "“produzione=true”. Questa opzione può essere specificata più di una "
 "volta."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:61
+#: src/metapensiero/sphinx/patchdb/pup.py:59
 #, python-format
 msgid "Invalid variable: %s"
 msgstr "Variabile non valida: %s"
 
 #: src/metapensiero/sphinx/patchdb/script.py:202
 #, python-format
 msgid "Missing mandatory ID for the directive \"%s\"."
 msgstr "La direttiva \"%s\" richiede un ID."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:135
+#: src/metapensiero/sphinx/patchdb/pup.py:133
 msgid ""
 "One or more archives containing collected scripts. May be either plain "
 "file names or package relative paths like “package.name:some/file”."
 msgstr ""
 "Uno o più archivi contenenti degli script. Si possono specificare sia "
 "nomi di file piuttosto che percorsi relativi tipo "
 "“nome.pacchetto:qualche/file”."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:151
+#: src/metapensiero/sphinx/patchdb/pup.py:149
 msgid "Password"
 msgstr "Password"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:181
-#, python-format
+# | msgid "" "Perform a backup of the database in directory DIR (by default "
+# | "“%(default)s”) before doing anything. Specify “None” to disable backups."
+#: src/metapensiero/sphinx/patchdb/pup.py:179
 msgid ""
-"Perform a backup of the database in directory DIR (by default "
-"“%(default)s”) before doing anything. Specify “None” to disable backups."
+"Perform a backup of the database in directory DIR before doing anything, "
+"that by default (or by specifying “None”) does not happen."
 msgstr ""
-"Esegui un backup del database nella directory DIR (di default "
-"“%(default)s”) prima di fare qualsiasi cosa. Specifica “None” per "
-"disabilitare il backup."
+"Esegui un backup del database nella directory DIR prima di fare qualsiasi "
+"cosa, che di norma (oppure quando viene specificato “None”) non viene "
+"effettuato."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:155
+#: src/metapensiero/sphinx/patchdb/pup.py:153
 msgid "Port number used by the MySQL server, defaults to “3306”."
 msgstr "Porta usata dal server MySQL, di default “3306”. "
 
-#: src/metapensiero/sphinx/patchdb/script.py:459
+#: src/metapensiero/sphinx/patchdb/script.py:463
 msgid "Preceeds"
 msgstr "Precede"
 
-#: src/metapensiero/sphinx/patchdb/script.py:650
+#: src/metapensiero/sphinx/patchdb/script.py:654
 #, python-format
 msgid "Reference to an unknown script: %(scriptid)r"
 msgstr "Riferimento a uno script sconosciuto: %(scriptid)r"
 
 #: src/metapensiero/sphinx/patchdb/script.py:219
 #, python-format
 msgid ""
@@ -287,90 +293,90 @@
 msgid "Script index"
 msgstr "Indice degli script"
 
 #: src/metapensiero/sphinx/patchdb/script.py:366
 msgid "Scripts"
 msgstr "Script"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:143
+#: src/metapensiero/sphinx/patchdb/pup.py:141
 msgid "Select the Firebird context."
 msgstr "Seleziona il contesto Firebird."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:147
+#: src/metapensiero/sphinx/patchdb/pup.py:145
 msgid "Select the MySQL context."
 msgstr "Seleziona il contesto MySQL."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:140
+#: src/metapensiero/sphinx/patchdb/pup.py:138
 msgid ""
 "Select the PostgreSQL context. DSN is a string of the kind "
 "“host=localhost dbname=mydb user=myself password=ouch”."
 msgstr ""
 "Seleziona il contesto PostgreSQL. DSN è una stringa nel formato "
 "“host=localhost dbname=miodb user=iostesso password=blabla”."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:145
+#: src/metapensiero/sphinx/patchdb/pup.py:143
 msgid "Select the SQLite context."
 msgstr "Seleziona il contesto SQLite."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:162
+#: src/metapensiero/sphinx/patchdb/pup.py:160
 msgid "Specify where to write the execution log."
 msgstr "Specifica dove scrivere il log dell'esecuzione."
 
-#: src/metapensiero/sphinx/patchdb/script.py:573
+#: src/metapensiero/sphinx/patchdb/script.py:577
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings an "
 "unknown script \"%(other)s\""
 msgstr ""
 "La %(scriptid)s (definita in %(docname)s alla riga %(lineno)s) implementa"
 " uno script sconosciuto \"%(other)s\""
 
-#: src/metapensiero/sphinx/patchdb/script.py:581
+#: src/metapensiero/sphinx/patchdb/script.py:585
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings "
 "script \"%(other)s\" to revision %(newrev)s, but it's still at revision "
 "%(currev)s"
 msgstr ""
 "La %(scriptid)s (definita in %(docname)s alla riga %(lineno)s) implementa"
 " lo script \"%(other)s\" alla revisione %(newrev)s, ma è ancora alla "
 "revisione %(currev)s"
 
-#: src/metapensiero/sphinx/patchdb/script.py:565
+#: src/metapensiero/sphinx/patchdb/script.py:569
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) depends on "
 "an unknown script \"%(other)s\""
 msgstr ""
 "Lo %(scriptid)s (definito in %(docname)s alla riga %(lineno)s) dipende da"
 " uno script sconosciuto \"%(other)s\""
 
-#: src/metapensiero/sphinx/patchdb/script.py:467
+#: src/metapensiero/sphinx/patchdb/script.py:471
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) references "
 "an unknown script \"%(other)s\""
 msgstr ""
 "Lo %(scriptid)s (definito in %(docname)s alla riga %(lineno)s) referenzia"
 " uno script sconosciuto \"%(other)s\""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:76
+#: src/metapensiero/sphinx/patchdb/pup.py:74
 msgid "Upgrading:"
 msgstr "Aggiornamento:"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:149
+#: src/metapensiero/sphinx/patchdb/pup.py:147
 msgid "Username to log into the database."
 msgstr "Nome utente per accedere al database."
 
 #: src/metapensiero/sphinx/patchdb/contexts/__init__.py:192
 #, python-format
 msgid "Would apply %s"
 msgstr "Applicherei %s"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:37
+#: src/metapensiero/sphinx/patchdb/pup.py:35
 msgid ""
 "You must select exactly one database with either “--postgresql”, "
 "“--firebird”, “--mysql” or “--sqlite”!"
 msgstr ""
 "Devi selezionare un database con “--postgresql”, “--firebird”, “--mysql” "
 "o “--sqlite”!"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot`

 * *Files 5% similar despite different names*

```diff
@@ -3,190 +3,194 @@
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev3\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev4\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
-"POT-Creation-Date: 2023-02-15 22:17+0100\n"
+"POT-Creation-Date: 2023-04-30 16:25+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:67
-#: src/metapensiero/sphinx/patchdb/pup.py:90
+#: src/metapensiero/sphinx/patchdb/pup.py:65
+#: src/metapensiero/sphinx/patchdb/pup.py:88
 #, python-format
 msgid ""
 "\n"
 "Error: %s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:294
 #: src/metapensiero/sphinx/patchdb/script.py:422
-#: src/metapensiero/sphinx/patchdb/script.py:442
+#: src/metapensiero/sphinx/patchdb/script.py:444
+msgid " (any revision)"
+msgstr ""
+
+#: src/metapensiero/sphinx/patchdb/script.py:294
+#: src/metapensiero/sphinx/patchdb/script.py:424
+#: src/metapensiero/sphinx/patchdb/script.py:446
 #, python-format
 msgid " (revision %(revno)d)"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:492
+#: src/metapensiero/sphinx/patchdb/script.py:496
 msgid "After any other script"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:164
+#: src/metapensiero/sphinx/patchdb/pup.py:162
 msgid "Assume missing patches are already applied, do not re-execute them."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:177
+#: src/metapensiero/sphinx/patchdb/pup.py:175
 msgid "Be quiet, emit only error messages."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:490
+#: src/metapensiero/sphinx/patchdb/script.py:494
 msgid "Before any other script"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:460
+#: src/metapensiero/sphinx/patchdb/script.py:464
 msgid "Brings"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:482
+#: src/metapensiero/sphinx/patchdb/script.py:486
 msgid "Condition"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:474
+#: src/metapensiero/sphinx/patchdb/script.py:478
 msgid "Conditions"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:132
+#: src/metapensiero/sphinx/patchdb/pup.py:130
 msgid "Database script applier"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:171
+#: src/metapensiero/sphinx/patchdb/pup.py:169
 msgid ""
 "Define an arbitrary variable usable as “{{VARNAME}}” within a script. VAR"
 " must be something like “varname=value”. This option may be given "
 "multiple times."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:458
+#: src/metapensiero/sphinx/patchdb/script.py:462
 msgid "Depends on"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:464
+#: src/metapensiero/sphinx/patchdb/script.py:468
 msgid "Direct dependants"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:175
+#: src/metapensiero/sphinx/patchdb/pup.py:173
 msgid "Don't apply patches, just list them."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:84
+#: src/metapensiero/sphinx/patchdb/pup.py:82
 #, python-format
 msgid "Done, applied %d script"
 msgid_plural "Done, applied %d scripts"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:159
+#: src/metapensiero/sphinx/patchdb/pup.py:157
 msgid "Driver to access MySQL, defaults to “pymysql”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:461
+#: src/metapensiero/sphinx/patchdb/script.py:465
 msgid "Drops"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:179
+#: src/metapensiero/sphinx/patchdb/pup.py:177
 msgid "Emit debug messages."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:157
+#: src/metapensiero/sphinx/patchdb/pup.py:155
 msgid "Encoding used by the MySQL driver, defaults to “utf8mb4”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:47
+#: src/metapensiero/sphinx/patchdb/pup.py:45
 #, python-format
 msgid "Error: %s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:96
+#: src/metapensiero/sphinx/patchdb/pup.py:94
 msgid "Error: circular dependencies among scripts"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:488
+#: src/metapensiero/sphinx/patchdb/script.py:492
 msgid "Execute always"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:233
 msgid "File insertion disabled"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:502
+#: src/metapensiero/sphinx/patchdb/script.py:506
 msgid ""
 "Go on with the next script, skipping any succeding statements of the "
 "failing script"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:153
+#: src/metapensiero/sphinx/patchdb/pup.py:151
 msgid "Host name where MySQL server runs, defaults to “localhost”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:506
+#: src/metapensiero/sphinx/patchdb/script.py:510
 msgid ""
 "Ignore the error and keeps going with the remaining statements in the "
 "script"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:167
+#: src/metapensiero/sphinx/patchdb/pup.py:165
 msgid ""
 "Introduce an arbitrary assertion usable as a pre-condition by the "
 "scripts. NAME may be a simple string or something like “production=true”."
 " This option may be given multiple times."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:61
+#: src/metapensiero/sphinx/patchdb/pup.py:59
 #, python-format
 msgid "Invalid variable: %s"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:202
 #, python-format
 msgid "Missing mandatory ID for the directive \"%s\"."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:135
+#: src/metapensiero/sphinx/patchdb/pup.py:133
 msgid ""
 "One or more archives containing collected scripts. May be either plain "
 "file names or package relative paths like “package.name:some/file”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:151
+#: src/metapensiero/sphinx/patchdb/pup.py:149
 msgid "Password"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:181
-#, python-format
+#: src/metapensiero/sphinx/patchdb/pup.py:179
 msgid ""
-"Perform a backup of the database in directory DIR (by default "
-"“%(default)s”) before doing anything. Specify “None” to disable backups."
+"Perform a backup of the database in directory DIR before doing anything, "
+"that by default (or by specifying “None”) does not happen."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:155
+#: src/metapensiero/sphinx/patchdb/pup.py:153
 msgid "Port number used by the MySQL server, defaults to “3306”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:459
+#: src/metapensiero/sphinx/patchdb/script.py:463
 msgid "Preceeds"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:650
+#: src/metapensiero/sphinx/patchdb/script.py:654
 #, python-format
 msgid "Reference to an unknown script: %(scriptid)r"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:219
 #, python-format
 msgid ""
@@ -252,77 +256,77 @@
 msgid "Script index"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:366
 msgid "Scripts"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:143
+#: src/metapensiero/sphinx/patchdb/pup.py:141
 msgid "Select the Firebird context."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:147
+#: src/metapensiero/sphinx/patchdb/pup.py:145
 msgid "Select the MySQL context."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:140
+#: src/metapensiero/sphinx/patchdb/pup.py:138
 msgid ""
 "Select the PostgreSQL context. DSN is a string of the kind "
 "“host=localhost dbname=mydb user=myself password=ouch”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:145
+#: src/metapensiero/sphinx/patchdb/pup.py:143
 msgid "Select the SQLite context."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:162
+#: src/metapensiero/sphinx/patchdb/pup.py:160
 msgid "Specify where to write the execution log."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:573
+#: src/metapensiero/sphinx/patchdb/script.py:577
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings an "
 "unknown script \"%(other)s\""
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:581
+#: src/metapensiero/sphinx/patchdb/script.py:585
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings "
 "script \"%(other)s\" to revision %(newrev)s, but it's still at revision "
 "%(currev)s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:565
+#: src/metapensiero/sphinx/patchdb/script.py:569
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) depends on "
 "an unknown script \"%(other)s\""
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:467
+#: src/metapensiero/sphinx/patchdb/script.py:471
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) references "
 "an unknown script \"%(other)s\""
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:76
+#: src/metapensiero/sphinx/patchdb/pup.py:74
 msgid "Upgrading:"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:149
+#: src/metapensiero/sphinx/patchdb/pup.py:147
 msgid "Username to log into the database."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/contexts/__init__.py:192
 #, python-format
 msgid "Would apply %s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:37
+#: src/metapensiero/sphinx/patchdb/pup.py:35
 msgid ""
 "You must select exactly one database with either “--postgresql”, "
 "“--firebird”, “--mysql” or “--sqlite”!"
 msgstr ""
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/manager.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- Script&Patch Manager
 # :Created:   ven 14 ago 2009 13:09:28 CEST
 # :Author:    Lele Gaifax <lele@nautilus.homeip.net>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2009, 2010, 2012-2018, 2021 Lele Gaifax
+# :Copyright: © 2009, 2010, 2012-2018, 2021, 2023 Lele Gaifax
 #
 
 from collections import defaultdict
 import json
 import logging
 import pickle
 from os.path import dirname, exists, relpath
@@ -235,15 +235,15 @@
         missing = set()
         always_first = set()
         always_last = set()
         precedences = self.precedences
 
         logger.debug("Collecting and ordering patches...")
         for pid, patch in self.db.items():
-            patch.adjustUnspecifiedRevisions(self)
+            patch.adjustUnspecifiedRevisions(self, context)
 
             applicable, reason = patch.isApplicable(context)
             if applicable:
                 for preceed in patch.preceeds:
                     precedences[preceed].add(patch)
 
                 if patch.always:
@@ -286,15 +286,14 @@
         self._checkMissingRevisionsBump()
 
         storage_path = self.storages[0]
         if storage_path is None:
             return
 
         logger.debug("Writing patches to %s", storage_path)
-        spendswith = storage_path.endswith
         if storage_path.endswith('.json'):
             storage = open(storage_path, 'w', encoding='utf-8')
 
             # Order patches by id, both for easier lookup and to
             # avoid VCs stress
 
             asdicts = [self.db[sid].as_dict for sid in sorted(self.db)]
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/patch.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- Patch object
 # :Created:   Fri Oct  3 01:13:20 2003
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2003, 2009, 2010, 2012-2017, 2019, 2021 Lele Gaifax
+# :Copyright: © 2003, 2009, 2010, 2012-2017, 2019, 2021, 2023 Lele Gaifax
 #
 
 from collections import defaultdict
 from graphlib import TopologicalSorter
 import logging
 
 
@@ -142,15 +142,15 @@
             line=self.line,
         )
         if self.patchid != self.description:
             res['description'] = self.description
 
         def rr(d):
             if d[1]:
-                return '%s@%d' % d
+                return '%s@%s' % d
             else:
                 return d[0]
 
         if self.always:
             res['always'] = self.always
         if self.depends:
             res['depends'] = [rr(d) for d in self.depends]
@@ -173,15 +173,15 @@
     def is_migration(self):
         return bool(self.brings or self.drops)
 
     @property
     def is_placeholder(self):
         return not self.script
 
-    def adjustUnspecifiedRevisions(self, pm):
+    def adjustUnspecifiedRevisions(self, pm, context):
         """
         Replace the non-specified revision numbers with the current known version of the patch.
 
         Perform also some sanity checks: all `depends`, `brings` and `preceeds` must exist at
         this point.
         """
 
@@ -196,14 +196,20 @@
                     continue
                 raise DependencyError('%s (defined in %s at line %s)'
                                       ' depends on "%s@%s",'
                                       ' which does not exist.'
                                       % (self, self.source, self.line, pid, rev))
             if rev is None:
                 self.depends[i] = (pid, p.revision)
+            elif rev == '*':
+                current_rev = context[pid]
+                if current_rev is None:
+                    self.depends[i] = (pid, p.revision)
+                else:
+                    self.depends[i] = (pid, current_rev)
 
         for i, (pid, rev) in enumerate(self.brings):
             p = pm[pid]
             if p is None:
                 logger.debug('%s (defined in %s at line %s)'
                              ' brings to "%s@%s",'
                              ' which does not exist: applying anyway'
@@ -273,41 +279,47 @@
 
         if not self.verifyConditions(lang_context):
             return False, "does not satisfy the conditions"
 
         return lang_context.isApplicable(self)
 
 
-def parse_deps(deps):
+def parse_deps(deps, allow_star=False):
     """Parse textual dependencies.
 
     `deps` is the textual representation of the dependencies specified in the ``depends``,
-    ``brings``, ``drops`` and ``preceeds`` fields.
+    ``brings``, ``drops`` and ``preceeds`` fields. `allow_star` indicates whether the form
+    ``patchid@*`` is allowed.
 
     `deps` may contain something like ``patchid@10``, to specify the revision 10 of the given
     patch. When the revision is not specified it's set to None, and later adjusted to be the
     current revision of the patch.
 
     Multiple dependencies may be separated by a comma.
+
     """
 
     result = []
 
     if deps:
         if isinstance(deps, str):
             deps = deps.split(',')
         for dep in deps:
             dep = dep.strip()
             if not dep:
                 raise ValueError("empty patch ID, spurious comma?")
             if '@' in dep:
                 depid, deprev = dep.split('@')
-                deprev = int(deprev)
-                if deprev < 1:
-                    raise ValueError("invalid revision: %r" % dep)
+                if deprev == '*':
+                    if not allow_star:
+                        raise ValueError("invalid revision: %r" % dep)
+                else:
+                    deprev = int(deprev)
+                    if deprev < 1:
+                        raise ValueError("invalid revision: %r" % dep)
             else:
                 depid = dep
                 deprev = None
 
             result.append((depid.lower(), deprev))
 
     # For purely aesthetic reasons, order dependencies alphabetically
@@ -329,15 +341,15 @@
     description = options.get('description', description or patchid)
     language = options.get('language', 'sql')
     revision = int(options.get('revision', 1))
     if revision < 1:
         raise ValueError("Invalid revision, must be greater than 0")
 
     try:
-        depends = parse_deps(options.get('depends', ''))
+        depends = parse_deps(options.get('depends', ''), allow_star=True)
     except ValueError as e:
         raise ValueError("Error in script's depends option: %s" % str(e))
 
     try:
         preceeds = parse_deps(options.get('preceeds', ''))
     except ValueError as e:
         raise ValueError("Error in script's preceeds option: %s" % str(e))
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/pup.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/pup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- Apply collected patches to a database
 # :Created:   Wed Nov 12 23:10:22 2003
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2003, 2009, 2010, 2012-2017, 2019, 2021, 2022 Lele Gaifax
+# :Copyright: © 2003, 2009, 2010, 2012-2017, 2019, 2021, 2022, 2023 Lele Gaifax
 #
 
-from collections import Counter
 from graphlib import CycleError
 from os.path import isabs
 import sys
-import tempfile
 
 import enlighten
 
 from .contexts import ExecutionContext, ExecutionError, get_context_from_args
 from .locale import gettext as _, ngettext, setup as setup_i18n
 from .patch import DependencyError
 from .manager import DuplicatedScriptError, Missing3rdPartyModule, patch_manager
@@ -34,15 +32,15 @@
 def workhorse(args, progress):
     sqlctx = get_context_from_args(args)
     if sqlctx is None:
         print(_("You must select exactly one database with either “--postgresql”,"
                 " “--firebird”, “--mysql” or “--sqlite”!"))
         return USAGE
 
-    if args.backups_dir != 'None' and not args.dry_run:
+    if args.backups_dir and args.backups_dir != 'None' and not args.dry_run:
         sqlctx.backup(args.backups_dir)
 
     try:
         pm = patch_manager(args.storage)
     except (DuplicatedScriptError, Missing3rdPartyModule) as e:
         print(_("Error: %s") % e)
         return DATAERR
@@ -124,15 +122,15 @@
     import logging
     from argparse import ArgumentParser
     from importlib import metadata
 
     locale.setlocale(locale.LC_ALL, '')
     setup_i18n()
 
-    version = metadata.version('metapensiero_sphinx_patchdb')
+    version = metadata.version('metapensiero.sphinx.patchdb')
     parser = ArgumentParser(description=_("Database script applier"))
 
     parser.add_argument("storage", type=path_spec, nargs='+',
                         help=_("One or more archives containing collected scripts."
                                " May be either plain file names or package relative paths"
                                " like “package.name:some/file”."))
     parser.add_argument('--version', action='version', version='%(prog)s ' + version)
@@ -173,18 +171,18 @@
                                " This option may be given multiple times."))
     parser.add_argument("-n", "--dry-run", default=False, action="store_true",
                         help=_("Don't apply patches, just list them."))
     parser.add_argument("-q", "--quiet", default=False, action="store_true",
                         help=_("Be quiet, emit only error messages."))
     parser.add_argument("-d", "--debug", default=False, action="store_true",
                         help=_("Emit debug messages."))
-    parser.add_argument("-b", "--backups-dir", metavar="DIR", default=tempfile.gettempdir(),
+    parser.add_argument("-b", "--backups-dir", metavar="DIR", default=None,
                         help=_("Perform a backup of the database in directory DIR"
-                               " (by default “%(default)s”) before doing anything."
-                               " Specify “None” to disable backups."))
+                               " before doing anything, that by default (or by specifying"
+                               " “None”) does not happen."))
 
     args = parser.parse_args()
 
     level = logging.DEBUG if args.debug else logging.WARNING if args.quiet else logging.INFO
     if args.log_path:
         logging.basicConfig(filename=args.log_path, level=level,
                             format="%(asctime)s [%(levelname).1s] %(message)s",
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/script.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,17 @@
                         else:
                             raise DependencyError(sid)
                     else:
                         refid = nodes.make_id("script " + sid)
                         refuri = get_relative_uri(fromdocname, docname) + '#' + refid
                         ref = nodes.paragraph('', '')
                         reftxt = sid
-                        if rev is not None:
+                        if rev == '*':
+                            reftxt += _(' (any revision)')
+                        elif rev is not None:
                             reftxt += _(' (revision %(revno)d)') % dict(revno=rev)
                         ref += nodes.reference('', reftxt, refid=refid, refuri=refuri)
                         li += ref
                         value += li
             else:
                 sid, rev = detvalue[0]
                 try:
@@ -434,15 +436,17 @@
                     else:
                         raise DependencyError(sid)
                 else:
                     refid = nodes.make_id("script " + sid)
                     refuri = get_relative_uri(fromdocname, docname) + '#' + refid
                     value = nodes.paragraph('', '')
                     reftxt = sid
-                    if rev is not None:
+                    if rev == '*':
+                        reftxt += _(' (any revision)')
+                    elif rev is not None:
                         reftxt += _(' (revision %(revno)d)') % dict(revno=rev)
                     value += nodes.reference('', reftxt, refid=refid, refuri=refuri)
             defn = nodes.definition('', value)
             item += term
             item += defn
 
             dlist += item
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/src/metapensiero/sphinx/patchdb/states.py` & `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/states.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/fixtures.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,17 @@
     SPHINX_BUILD_OPTS = ('-b', 'html', '-q', '-d', '_build/doctrees', '.', '_build/html')
 
     PATCHDB = 'patchdb'
     PATCHDB_SHELVE = 'patchdb-test.json'
 
     PDBSTATES = 'patchdb-states'
 
-    def __init__(self, db_opts, sphinx_build_opts):
+    def __init__(self, db_opts, backups_dir, sphinx_build_opts):
         self.db_opts = db_opts
+        self.backups_dir = backups_dir
         self.sphinx_build_opts = sphinx_build_opts
         self.directory = tempfile.mkdtemp()
 
     def remove(self):
         if not getenv('PATCHDB_TEST_DRD'):
             shutil.rmtree(self.directory)
 
@@ -82,14 +83,17 @@
             self.build_warning = '\n'.join(warnings) if warnings else None
             self.build_error = '\n'.join(errors) if errors else None
         return self.build_error
 
     def patchdb(self, *more_args, **kwargs):
         cmd = [self.PATCHDB]
         cmd.extend(self.db_opts)
+        if self.backups_dir:
+            cmd.append('--backups-dir')
+            cmd.append(self.backups_dir)
         cmd.extend(more_args)
         cmd.append(self.PATCHDB_SHELVE)
         stderr_fileno, stderr_filename = tempfile.mkstemp()
         try:
             try:
                 output = subprocess.check_output(cmd, cwd=self.directory, stderr=stderr_fileno)
                 output = output.decode(USER_ENCODING)
@@ -113,14 +117,16 @@
         return output
 
     def pdbstates(self, subcmd, *more_args):
         cmd = [self.PDBSTATES, subcmd]
         if subcmd == 'restore':
             cmd.extend(self.db_opts)
         cmd.extend(more_args)
+        if self.backups_dir:
+            cmd.append(self.backups_dir)
         stderr_fileno, stderr_filename = tempfile.mkstemp()
         try:
             try:
                 output = subprocess.check_output(cmd, cwd=self.directory, stderr=stderr_fileno)
                 output = output.decode(USER_ENCODING)
             except subprocess.CalledProcessError:
                 close(stderr_fileno)
@@ -140,14 +146,18 @@
     DB_OPTION = '--sqlite'
     "The option passed to ``patchdb`` to select the database engine"
 
     DB_NAME = 'patchdb-test.sqlite'
     "The name of the database to operate on"
 
     DB_OTHER_OPTIONS = ()
+    "Other options needed to conntect to the database."
+
+    BACKUPS_DIR = None
+    "The directory where to put backups and state file."
 
     SPHINX_CONF = DEFAULT_SPHINX_CONF
     "The configuration for the Sphinx environment"
 
     SPHINX_BUILD_OTHER_OPTIONS = ()
 
     INDEX_TXT = DEFAULT_INDEX_TXT
@@ -169,15 +179,15 @@
         yield from cls.OTHER_FILES
 
     @classmethod
     def setUpClass(cls):
         cls.drop_database_if_exists()
         cls.create_database()
         cls.sphinx = PatchDBSphinx((cls.DB_OPTION, cls.DB_NAME) + cls.DB_OTHER_OPTIONS,
-                                   cls.SPHINX_BUILD_OTHER_OPTIONS)
+                                   cls.BACKUPS_DIR, cls.SPHINX_BUILD_OTHER_OPTIONS)
         cls.sphinx.build({filename: content for filename, content in cls.contents()})
 
     @classmethod
     def tearDownClass(cls):
         cls.sphinx.remove()
 
     @classmethod
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_bad.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_bad.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_drops.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_drops.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_external_file.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_external_file.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_helpers.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_manager.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_modular.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_modular.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_patch.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- Patch tests
 # :Created:   mer 24 feb 2016 16:44:43 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017, 2019 Lele Gaifax
+# :Copyright: © 2016, 2017, 2019, 2023 Lele Gaifax
 #
 
+import pytest
 import fixtures
 
 
 def test_patch():
     from metapensiero.sphinx.patchdb.manager import patch_manager
     from metapensiero.sphinx.patchdb.patch import make_patch, parse_deps, DependencyError
 
@@ -35,37 +36,55 @@
     assert str(third) == 'patch "third@1"'
 
     fourth = make_patch('fourth', 'script',
                         dict(depends='unknown@1'))
     pm['fourth'] = fourth
 
     # adjustUnspecifiedRevisions
+    context = {}
     first = pm['first']
     assert first.depends == [('second', None)]
     assert first.preceeds == [('third', None)]
-    first.adjustUnspecifiedRevisions(pm)
+    first.adjustUnspecifiedRevisions(pm, context)
     assert first.depends == [('second', 2)]
     assert first.preceeds == [('third', 1)]
     third = pm['third']
     assert third.preceeds == [('fourth', 2)]
-    third.adjustUnspecifiedRevisions(pm)
+    third.adjustUnspecifiedRevisions(pm, context)
 
     try:
-        fourth.adjustUnspecifiedRevisions(pm)
+        fourth.adjustUnspecifiedRevisions(pm, context)
     except DependencyError as e:
         assert 'script "fourth@1"' in str(e) and 'depends on "unknown@1"' in str(e)
     else:
         assert False, "should raise a DependencyError"
 
+    fifth = make_patch('fifth', 'script',
+                       dict(depends="second@*"))
+    pm['fifth'] = fifth
+
+    context = {'second': 1}
+    fifth.adjustUnspecifiedRevisions(pm, context)
+    assert fifth.depends == [('second', 1)]
+
     # parse_deps
     assert parse_deps('patchid@10') == [('patchid', 10)]
     assert parse_deps('patchid@10, other') == [('other', None), ('patchid', 10)]
     assert (parse_deps(' z, x , y@10 , a,c') ==
             [('a', None), ('c', None), ('x', None), ('y', 10), ('z', None)])
 
+    with pytest.raises(ValueError):
+        make_patch('invalid', 'script', dict(brings="second@*"))
+
+    with pytest.raises(ValueError):
+        make_patch('invalid', 'script', dict(drops="second@*"))
+
+    with pytest.raises(ValueError):
+        make_patch('invalid', 'script', dict(preceeds="second@*"))
+
 
 class TestPatchNonExistingDepends(fixtures.BaseTestCase):
     TEST_TXT = """
     New table, replacing old table
     ==============================
 
     .. patchdb:script:: Create new_table
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_python.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_revisions.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_revisions.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_sql.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_sql_fb.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_fb.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_sql_ms.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_ms.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_states.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_states.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- States related tests
 # :Created:   ven 15 apr 2016 12:08:46 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017 Lele Gaifax
+# :Copyright: © 2016, 2017, 2023 Lele Gaifax
 #
 
 import hashlib
-import os
+import tempfile
 
 import test_revisions
 import test_sql
 
 
 THIRD_REV = """
 Multiple revisions
@@ -45,29 +45,32 @@
 
 
 REV1_HASH = hashlib.md5(b'create first table@1').hexdigest()
 REV2_HASH = hashlib.md5(b'create first table@2update first table@1').hexdigest()
 
 
 class TestStates(test_sql.TestSingleSQLScript):
+    BACKUPS_DIR = f'{tempfile.gettempdir()}/bcks'
+
     def test(self):
-        bckdir = os.path.join(self.sphinx.directory, 'bcks')
-        output = self.patchdb('-b', bckdir)
+        output = self.patchdb()
         self.assertIn('Done, applied 1 script', output)
-        output = self.patchdb('-b', bckdir)
+        output = self.patchdb()
         self.assertIn('Done, applied 0 scripts', output)
-        output = self.pdbstates('list', bckdir)
+        output = self.pdbstates('list')
         self.assertIn(REV1_HASH + ' <create first table@1>\n', output)
-        output = self.pdbstates('list', '--tsv', bckdir)
+        output = self.pdbstates('list', '--tsv')
         self.assertIn(REV1_HASH, (line.split('\t')[1]
                                   for line in output.splitlines()
                                   if line))
 
 
 class TestRestoreState(test_revisions.TestMultipleRevIncremental):
+    BACKUPS_DIR = f'{tempfile.gettempdir()}/bcks'
+
     def test_3(self):
         output = self.pdbstates('list')
         self.assertIn(REV1_HASH + ' <create first table@1>\n', output)
         output = self.pdbstates('restore', REV1_HASH)
         self.assertIn('Restored ', output)
         self.assertIn(' from ', output)
         self.assertIn(REV1_HASH, output)
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/tests/test_variables.py` & `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev3/PKG-INFO` & `metapensiero.sphinx.patchdb-4.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: metapensiero.sphinx.patchdb
-Version: 4.0.dev3
+Version: 4.0.dev4
 Summary: Extract scripts from a reST document and apply them in order.
 License: GPL-3.0-or-later
 Author-email: Lele Gaifax <lele@metapensiero.it>
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Italian
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Provides-Extra: dev
 Project-URL: Changelog, https://gitlab.com/metapensiero/metapensiero.sphinx.patchdb/-/blob/master/CHANGES.rst
 Project-URL: Source, https://gitlab.com/metapensiero/metapensiero.sphinx.patchdb
 Description-Content-Type: text/x-rst
 
@@ -39,15 +39,15 @@
 ========================================================
 
 :version: 4
 :author: Lele Gaifax <lele@metapensiero.it>
 :license: GPLv3
 
 Building and maintaining the schema of a database is always a challenge. It may quickly become
-a nightmare when dealing with even moderately complex databases, in a distribuited development
+a nightmare when dealing with even moderately complex databases, in a distributed development
 environment. You have new features going in, and fixes here and there, that keeps accumulating
 in the development `branch`. You also have several already deployed instances of the database
 you wanna upgrade now and then.
 
 In my experience, it's very difficult to impossible to come up with a completely automated
 solution, for several reasons:
 
@@ -74,14 +74,19 @@
 
 .. [*] Just to mention a few alternatives:
 
        `Alembic <https://pypi.python.org/pypi/alembic>`_
          Written on top of SQLAlchemy_ by the same author: it does not help when you need to
          manage something outside SA knowledge (stored procedures, permissions, …)
 
+       `Pyrseas <https://pyrseas.readthedocs.io/en/latest/>`_
+         ``PostgreSQL`` specific tool, able to distill an ``SQL`` script comparing between a ``YAML``
+         description of the schema and the actual one: interesting project, but does not handle
+         *data* migration
+
        `Sqlibrist <https://pypi.python.org/pypi/sqlibrist>`_
          Some similarities with PatchDB, very young, Django integration.
 
        `Sqitch <http://sqitch.org/>`_
          Quite good, *although* Perl based…
 
        See the `schema migration <https://en.wikipedia.org/wiki/Schema_migration>`_ page on
@@ -441,14 +446,28 @@
 
 When ``patchdb`` examines the database status, it will execute one *or* the other. If the
 script `Create master table` isn't executed yet (for example when operating on a new database),
 it will take the former script (the one that creates the table from scratch).  Otherwise, if
 the database "contains" revision 1 (and not higher than 1) of the script, it will execute the
 latter, bumping up the revision number.
 
+.. note:: Any single dependency may be either `generic` or `pinned` to a particular `revision`
+          number.
+
+          A generic dependency is one that does not contain a ``@`` character followed by an
+          integer number: in this case ``patchdb`` will consider it pointing to the *highest*
+          known revision of that script.
+
+          A pinned dependency contains the ``@``: what follows may be either a revision number
+          or, **only** for the `depends` ones, the character ``*``, to indicate that any
+          revision is good enough, provided it has been applied. In other words, the asterisk
+          will be replaced by the current revision of the script if it has been already
+          applied, otherwise by its highest known revision, i.e. handled in the same way as an
+          unpinned dependency.
+
 __ master-table_
 
 
 Obsoleted patches
 +++++++++++++++++
 
 Another peculiarity of this kind of scripts is that they may references `non existing scripts`
```

