# Comparing `tmp/arouteserver-1.8.0.tar.gz` & `tmp/arouteserver-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arouteserver-1.8.0.tar", last modified: Fri Jun 25 11:09:53 2021, max compression
+gzip compressed data, was "dist/arouteserver-1.9.0.tar", last modified: Sat Jul 24 14:32:10 2021, max compression
```

## Comparing `arouteserver-1.8.0.tar` & `arouteserver-1.9.0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35120 2021-06-25 11:09:42.000000 arouteserver-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    36483 2021-06-25 11:09:42.000000 arouteserver-1.8.0/CHANGES.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3182 2021-06-25 11:09:42.000000 arouteserver-1.8.0/scripts/arouteserver
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2021-06-25 11:09:42.000000 arouteserver-1.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10734 2021-06-25 11:09:42.000000 arouteserver-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-06-25 11:09:53.000000 arouteserver-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2756 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/fingerprints.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/templates/bird/
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/bird/irrdb.j2
--rw-r--r--   0 runner    (1001) docker     (121)    17786 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/bird/common.j2
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/bird/header.j2
--rw-r--r--   0 runner    (1001) docker     (121)    17098 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/bird/clients.j2
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/bird/main.j2
--rw-r--r--   0 runner    (1001) docker     (121)     4283 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/bird/macros.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/bird/rpki.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/irrdb.j2
--rw-r--r--   0 runner    (1001) docker     (121)      783 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/header.j2
--rw-r--r--   0 runner    (1001) docker     (121)    34567 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/filters.j2
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/clients.j2
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/main.j2
--rw-r--r--   0 runner    (1001) docker     (121)     5849 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/macros.j2
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/rpki.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/templates/template-context/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/template-context/main.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/templates/irr-as-set/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/irr-as-set/plain_rpsl.j2
--rw-r--r--   0 runner    (1001) docker     (121)      835 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/irr-as-set/ripe_ripeinator_yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/templates/html/
--rw-r--r--   0 runner    (1001) docker     (121)    18598 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/html/main.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/templates/html/macros.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      969 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/check_new_release.py
--rw-r--r--   0 runner    (1001) docker     (121)     9511 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/clients_from_euroix.py
--rw-r--r--   0 runner    (1001) docker     (121)    18415 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/setup_templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     7099 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6793 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/ixf_member_list_from_clients.py
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/verify_templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/clients_from_peeringdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    13899 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/tpl_rendering.py
--rw-r--r--   0 runner    (1001) docker     (121)     5516 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/init_scenario.py
--rw-r--r--   0 runner    (1001) docker     (121)     3962 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/commands/show_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13293 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/mocked_env.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/
--rw-r--r--   0 runner    (1001) docker     (121)    11821 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/instances.py
--rw-r--r--   0 runner    (1001) docker     (121)     8631 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/kvm.py
--rw-r--r--   0 runner    (1001) docker     (121)    36139 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/routinator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11760 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/bird.py
--rw-r--r--   0 runner    (1001) docker     (121)    17094 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/openbgpd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/exabgp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/
--rw-r--r--   0 runner    (1001) docker     (121)      799 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/AS2.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/irrdb.j2
--rw-r--r--   0 runner    (1001) docker     (121)    17786 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/common.j2
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/header.j2
--rw-r--r--   0 runner    (1001) docker     (121)    17098 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/clients.j2
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/main.j2
--rw-r--r--   0 runner    (1001) docker     (121)     4283 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/macros.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/rpki.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/irrdb.j2
--rw-r--r--   0 runner    (1001) docker     (121)      783 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/header.j2
--rw-r--r--   0 runner    (1001) docker     (121)    34567 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/filters.j2
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/clients.j2
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/main.j2
--rw-r--r--   0 runner    (1001) docker     (121)     5849 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/macros.j2
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/rpki.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/test_openbgpd6.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/test_bird4.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/clients.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11964 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3797 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bogons.yml
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      876 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/general.yml
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/AS1.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/test_bird6.py
--rw-r--r--   0 runner    (1001) docker     (121)     1889 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/test_openbgpd4.py
--rw-r--r--   0 runner    (1001) docker     (121)     7510 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/pdb_as_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/registrobr_db_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     4422 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/irr_db_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     5205 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/pdb_never_via_route_servers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3443 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/rtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     5246 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/pdb_max_prefix.py
--rw-r--r--   0 runner    (1001) docker     (121)    14048 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/irrdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/arin_db_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     5235 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/enrichers/rpki_roas.py
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/cached_objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5957 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/ripe_rpki_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/config.d/
--rw-r--r--   0 runner    (1001) docker     (121)     7858 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config.d/clients.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config.d/bogons.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config.d/arouteserver.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5335 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config.d/log.ini
--rwxr-xr-x   0 runner    (1001) docker     (121)      529 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config.d/rtt_getter.sh
--rw-r--r--   0 runner    (1001) docker     (121)    39676 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config.d/general.distrib.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/ipaddresses.py
--rw-r--r--   0 runner    (1001) docker     (121)     8966 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/peering_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/last_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    10286 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/irrdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    23747 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/euro_ix.py
--rw-r--r--   0 runner    (1001) docker     (121)     5057 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/registro_br_db_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6884 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/arin_db_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/ask.py
--rw-r--r--   0 runner    (1001) docker     (121)    57558 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/pierky/arouteserver/config/
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config/bogons.py
--rw-r--r--   0 runner    (1001) docker     (121)    11456 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29718 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config/general.py
--rw-r--r--   0 runner    (1001) docker     (121)    13924 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config/clients.py
--rw-r--r--   0 runner    (1001) docker     (121)    23833 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config/program.py
--rw-r--r--   0 runner    (1001) docker     (121)     2192 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config/asns.py
--rw-r--r--   0 runner    (1001) docker     (121)    21319 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2021-06-25 11:09:42.000000 arouteserver-1.8.0/pierky/arouteserver/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-06-25 11:09:42.000000 arouteserver-1.8.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 11:09:53.000000 arouteserver-1.8.0/arouteserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5578 2021-06-25 11:09:53.000000 arouteserver-1.8.0/arouteserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-25 11:09:53.000000 arouteserver-1.8.0/arouteserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-25 11:09:53.000000 arouteserver-1.8.0/arouteserver.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-25 11:09:53.000000 arouteserver-1.8.0/arouteserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)    56171 2021-06-25 11:09:53.000000 arouteserver-1.8.0/arouteserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-06-25 11:09:53.000000 arouteserver-1.8.0/arouteserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)    56171 2021-06-25 11:09:53.000000 arouteserver-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-06-25 11:09:42.000000 arouteserver-1.8.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2021-07-24 14:32:02.000000 arouteserver-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3907 2021-07-24 14:32:02.000000 arouteserver-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35120 2021-07-24 14:32:02.000000 arouteserver-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10794 2021-07-24 14:32:02.000000 arouteserver-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    39069 2021-07-24 14:32:02.000000 arouteserver-1.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2021-07-24 14:32:02.000000 arouteserver-1.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/arouteserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-07-24 14:32:10.000000 arouteserver-1.9.0/arouteserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-24 14:32:10.000000 arouteserver-1.9.0/arouteserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-24 14:32:10.000000 arouteserver-1.9.0/arouteserver.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-24 14:32:10.000000 arouteserver-1.9.0/arouteserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5578 2021-07-24 14:32:10.000000 arouteserver-1.9.0/arouteserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    59081 2021-07-24 14:32:10.000000 arouteserver-1.9.0/arouteserver.egg-info/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3182 2021-07-24 14:32:02.000000 arouteserver-1.9.0/scripts/arouteserver
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     2563 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/verify_templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1783 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7099 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/check_new_release.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3962 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/show_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5516 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/init_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6793 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/ixf_member_list_from_clients.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18415 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9511 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/clients_from_euroix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13899 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/tpl_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/setup_templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4048 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/commands/clients_from_peeringdb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/templates/irr-as-set/
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/irr-as-set/ripe_ripeinator_yml.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/irr-as-set/plain_rpsl.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     2756 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/fingerprints.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/templates/template-context/
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/template-context/main.j2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/
+-rw-r--r--   0 runner    (1001) docker     (121)      783 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/header.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     4476 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/rpki.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/main.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/clients.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/irrdb.j2
+-rw-r--r--   0 runner    (1001) docker     (121)    34567 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/filters.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     5849 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/macros.j2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/templates/html/
+-rw-r--r--   0 runner    (1001) docker     (121)    18598 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/html/main.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     1406 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/html/macros.j2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/templates/bird/
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/bird/header.j2
+-rw-r--r--   0 runner    (1001) docker     (121)    17786 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/bird/common.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/bird/rpki.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/bird/main.j2
+-rw-r--r--   0 runner    (1001) docker     (121)    17098 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/bird/clients.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/bird/irrdb.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     4283 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/templates/bird/macros.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     1263 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10286 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/irrdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1672 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/ipaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5057 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/registro_br_db_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9461 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/ripe_rpki_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    13293 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/mocked_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2754 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    11820 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/bird.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/exabgp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/routinator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12806 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/instances.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7510 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36139 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/AS1.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/general.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/AS2.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11964 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/test_bird6.py
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/clients.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1889 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/test_openbgpd4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/test_openbgpd6.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/
+-rw-r--r--   0 runner    (1001) docker     (121)      783 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/header.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     4476 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/rpki.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/main.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/clients.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/irrdb.j2
+-rw-r--r--   0 runner    (1001) docker     (121)    34567 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/filters.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     5849 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/macros.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     2138 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/test_bird4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3797 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bogons.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/header.j2
+-rw-r--r--   0 runner    (1001) docker     (121)    17786 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/common.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/rpki.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/main.j2
+-rw-r--r--   0 runner    (1001) docker     (121)    17098 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/clients.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/irrdb.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     4283 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/macros.j2
+-rw-r--r--   0 runner    (1001) docker     (121)    16660 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/openbgpd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8631 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/kvm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23747 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/euro_ix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    57565 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/ask.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/config/
+-rw-r--r--   0 runner    (1001) docker     (121)    21319 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config/bogons.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11456 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13924 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config/clients.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29869 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config/general.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23833 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config/program.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config/asns.py
+-rw-r--r--   0 runner    (1001) docker     (121)      763 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/config.d/
+-rw-r--r--   0 runner    (1001) docker     (121)    40516 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config.d/general.distrib.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5335 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config.d/log.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     3911 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config.d/arouteserver.yml
+-rwxr-xr-x   0 runner    (1001) docker     (121)      529 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config.d/rtt_getter.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     7858 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config.d/clients.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3632 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/config.d/bogons.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6151 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/cached_objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/last_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5096 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-24 14:32:10.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (121)    14048 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/irrdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3443 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/rtt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6381 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/rpki_roas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3690 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/pdb_as_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5205 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/pdb_never_via_route_servers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5246 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/pdb_max_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5021 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/irr_db_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/registrobr_db_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/enrichers/arin_db_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8966 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/peering_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6884 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/arouteserver/arin_db_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-07-24 14:32:02.000000 arouteserver-1.9.0/pierky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-07-24 14:32:10.000000 arouteserver-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    59081 2021-07-24 14:32:10.000000 arouteserver-1.9.0/PKG-INFO
```

### Comparing `arouteserver-1.8.0/LICENSE` & `arouteserver-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/CHANGES.rst` & `arouteserver-1.9.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,42 @@
 Change log
 ==========
 
 .. note:: **Upgrade notes**: after upgrading, run the ``arouteserver setup-templates`` command to sync the local templates with those distributed with the new version. More details on the `Upgrading <https://arouteserver.readthedocs.io/en/latest/INSTALLATION.html#upgrading>`__ section of the documentation.
 
+1.9.0
+-----
+
+- New: Add support for `OpenBGPD 7.1 <https://marc.info/?l=openbgpd-users&m=162461267419135&w=2>`__, also added to the integration testing suite (portable edition only).
+
+- Improvement: provide hint on how to change URL for external IRR DB data sources.
+
+  See also `GitHub issue 77 <https://github.com/pierky/arouteserver/issues/77>`_.
+
+- Fix (OpenBGPD only): `RFC8097 communities <https://datatracker.ietf.org/doc/html/rfc8097>`_ were not added after BGP Origin Validation.
+
+  The *BGP Prefix Origin Validation State Extended Communities* were not added when RPKI OV was performed. INVALID routes were still dropped when the route server was configured to do so (those routes are internally marked using locally-meaningful communities).
+
+- Improvement: RPKI ROAs files are checked for stale data.
+
+  The JSON files fetched from validating caches are now checked to detect stale data (rpki-client and OctoRPKI formats include this information) and they are ignored if the data they contain is no longer valid. In this case, the next URL in the ``rpki_roas.ripe_rpki_validator_url`` list is used.
+
+  By default, files whose content is older than 21600 seconds (6 hours) are ignored; it's possible to change this option via the newly introduced ``rpki_roas.ignore_cache_files_older_than`` setting.
+
+  Where available (rpki-client format only at this time), also the `VRP expiration time <https://github.com/openbsd/src/commit/a66158d7f8cdffc32bf2f8aa5d8bbed1f08a3a3d#diff-b2e9c61c4c7cfd2d5a0cde6066efe9a7c18dd1bdf06b1e473abc054261ea315c>`__ is checked.
+
+  As a consequence of this, the default ARouteServer cache expiration time for RPKI ROAs JSON files has been reduced to 60 minutes, to avoid caching ROAs that would turn out being expired at the next use of their cached copy.
+
+- Improvement: new order for the default URLs of the RPKI JSON files.
+
+  Since the RIPE NCC RPKI Validator `is now in EoL <https://labs.ripe.net/author/nathalie_nathalie/lifecycle-of-the-ripe-ncc-rpki-validator/>`__, the URL of the JSON file that points to rpki-validator.ripe.net has been moved as the last resort option for ``rpki_roas.ripe_rpki_validator_url``.
+  The one exposed in the `rpki-client dashboard <https://console.rpki-client.org/>`__ has been added.
+
+  Please note: this change only affects the default configuration file that ships with ARouteServer and is not be automatically reflected in existing configurations that route-servers operators are already using. If you wish this setup to be reflected in your configuration, please update your general.yml file accordingly.
+
 1.8.0
 -----
 
 - Improvement: add the ``logging`` option to ``--use-local-files`` argument, to allow customization of logging settings.
 
   Details on the documentation: `Logging configuration of the BGP daemon <https://arouteserver.readthedocs.io/en/latest/CONFIG.html#logging-configuration-of-the-bgp-daemon>`__.
```

### Comparing `arouteserver-1.8.0/scripts/arouteserver` & `arouteserver-1.9.0/scripts/arouteserver`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/setup.py` & `arouteserver-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/README.rst` & `arouteserver-1.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,85 +14,88 @@
 #. Two YAML files provide *general policies* and *clients configurations* options:
 
    .. code:: yaml
 
       cfg:
         rs_as: 64496
         router_id: "192.0.2.2"
-        add_path: True
         filtering:
-          next_hop:
-            policy: "same-as"
-        blackhole_filtering:
-          policy_ipv4: "rewrite-next-hop"
-          ...
+          irrdb:
+            enforce_origin_in_as_set: True
+            enforce_prefix_in_as_set: True
+          rpki_bgp_origin_validation:
+            enabled: True
+            reject_invalid: True
+            ...
 
    .. code:: yaml
 
       clients:
         - asn: 64511
           ip:
           - "192.0.2.11"
           - "2001:db8:1:1::11"
           irrdb:
             as_sets:
               - "RIPE::AS-FOO"
         ...
 
-#. ARouteServer acquires external information to enrich them: i.e. `bgpq4`_/`bgpq3`_ for IRR data, `PeeringDB`_ for max-prefix limit and AS-SETs, ...
+#. ARouteServer acquires external information to enrich them: i.e. `bgpq4`_/`bgpq3`_ for IRR data, `PeeringDB`_ for max-prefix limit and AS-SETs, RPKI ROAs, ...
 
 #. `Jinja2`_ built-in templates are used to render the final route server's configuration file.
 
-   Currently, **BIRD** (>= 1.6.3 up to 1.6.8), **BIRD v2** (starting from 2.0.7 - support for BIRD v2 is in `early stages <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html>`_) and **OpenBGPD** (OpenBSD 6.1 up to 7.0 and also OpenBGPD Portable 6.5p1 up to 7.0p0) are supported, with almost `feature parity <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html#supported-features>`_ between them.
+   Currently, **BIRD** (>= 1.6.3 up to 1.6.8), **BIRD v2** (starting from 2.0.7) and **OpenBGPD** (OpenBSD 6.1 up to 7.1 and also OpenBGPD Portable 6.5p1 up to 7.1p0) are supported, with almost `feature parity <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html#supported-features>`__ between them.
 
-**Validation** and testing of the configurations generated with this tool are performed using the built-in **live tests** framework: `Docker`_ instances are used to simulate several scenarios and to validate the behaviour of the route server after configuring it with ARouteServer. More details on the `Live tests <https://arouteserver.readthedocs.io/en/latest/LIVETESTS.html>`_ section.
+**Validation** and testing of the configurations generated with this tool are performed using the built-in **live tests** framework: `Docker`_ instances are used to simulate several scenarios and to validate the behaviour of the route server after configuring it with ARouteServer. More details on the `Live tests <https://arouteserver.readthedocs.io/en/latest/LIVETESTS.html>`__ section.
 
 A Docker-based `playground <https://github.com/pierky/arouteserver/tree/master/tools/playground>`__ is available to experiment with the tool in a virtual IXP environment.
 
 Also, a `Docker image <https://hub.docker.com/r/pierky/arouteserver>`__ is provided to start building rich and secure configurations in a couple of minutes.
 
 .. _bgpq3: https://github.com/snar/bgpq3
 .. _bgpq4: https://github.com/bgp/bgpq4
 .. _PeeringDB: https://www.peeringdb.com/
 .. _Jinja2: http://jinja.pocoo.org/
 .. _Docker: https://www.docker.com/
 
 Features
 --------
 
-- **Path hiding** mitigation techniques (`RFC7947`_ `section 2.3.1 <https://tools.ietf.org/html/rfc7947#section-2.3.1>`_).
+- **Path hiding** mitigation techniques (`RFC7947`_ `section 2.3.1 <https://tools.ietf.org/html/rfc7947#section-2.3.1>`__).
 
 - Basic filters (mostly enabled by default):
 
-  - **NEXT_HOP** enforcement (strict / same AS - `RFC7948`_ `section 4.8 <https://tools.ietf.org/html/rfc7948#section-4.8>`_);
+  - **NEXT_HOP** enforcement (strict / same AS - `RFC7948`_ `section 4.8 <https://tools.ietf.org/html/rfc7948#section-4.8>`__);
   - minimum and maximum IPv4/IPv6 **prefix length**;
   - maximum **AS_PATH length**;
   - reject **invalid AS_PATHs** (containing `private/invalid ASNs <http://mailman.nanog.org/pipermail/nanog/2016-June/086078.html>`_);
-  - reject AS_PATHs containing **transit-free** or **never via route-servers** ASNs (using `PeeringDB info_never_via_route_servers attribute <https://github.com/peeringdb/peeringdb/issues/394>`_);
+  - reject AS_PATHs containing **transit-free** or **never via route-servers** ASNs (using `PeeringDB info_never_via_route_servers attribute <https://github.com/peeringdb/peeringdb/issues/394>`__);
   - reject **bogons**;
   - **max-prefix limit** based on global or client-specific values or on **PeeringDB** data.
 
 - Prefixes and origin ASNs validation (also in *tag-only* mode):
 
-  - **IRR-based filters** (`RFC7948`_ `section 4.6.2 <https://tools.ietf.org/html/rfc7948#section-4.6.2>`_);
+  - **IRR-based filters** (`RFC7948`_ `section 4.6.2 <https://tools.ietf.org/html/rfc7948#section-4.6.2>`__);
   - AS-SETs configured manually or fetched from PeeringDB;
   - support for **IRR sources** (RIPE::AS-FOO, RADB::AS-BAR);
   - **white lists** support;
   - extended dataset for filters generation:
 
     - RPKI **ROAs used as route objects**;
-    - `Origin AS <https://mailman.nanog.org/pipermail/nanog/2017-December/093525.html>`_ from **ARIN Whois** database dump;
+    - `Origin AS <https://mailman.nanog.org/pipermail/nanog/2017-December/093525.html>`__ from **ARIN Whois** database dump;
     - `NIC.BR Whois data <https://ripe76.ripe.net/presentations/43-RIPE76_IRR101_Job_Snijders.pdf>`_ (slide n. 26) from Registro.br;
 
-  - **RPKI**-based filtering (BGP Prefix Origin Validation).
+  - **RPKI**-based filtering (BGP Prefix Origin Validation);
+
+    - ROAs can be retrieved from publicly available JSON files or from a local validating cache.
 
 - **Blackhole filtering** support:
 
   - optional **NEXT_HOP rewriting**;
-  - signalling via BGP Communities (`BLACKHOLE <https://tools.ietf.org/html/rfc7999#section-5>`_ and custom communities);
+  - signalling via BGP Communities (`BLACKHOLE <https://tools.ietf.org/html/rfc7999#section-5>`__ and custom communities);
   - client-by-client control over propagation.
 
 - **Graceful shutdown** support:
 
   - honor the **GRACEFUL_SHUTDOWN** BGP community received from clients (`draft-ietf-grow-bgp-gshut-11 <https://tools.ietf.org/html/draft-ietf-grow-bgp-gshut-11>`_);
   - allow to perform a graceful shutdown of the route server itself.
 
@@ -102,15 +105,15 @@
   - do (not) announce to any / **peer** / on **RTT basis**;
   - **prepend** to any / **peer** / on **RTT basis**;
   - add **NO_EXPORT** / **NO_ADVERTISE** to any / **peer**;
   - custom informational BGP communities.
 
 - Optional session features on a client-by-client basis:
 
-  - prepend route server ASN (`RFC7947`_ `section 2.2.2.1 <https://tools.ietf.org/html/rfc7947#section-2.2.2.1>`_);
+  - prepend route server ASN (`RFC7947`_ `section 2.2.2.1 <https://tools.ietf.org/html/rfc7947#section-2.2.2.1>`__);
   - active sessions;
   - **GTSM** (Generalized TTL Security Mechanism - `RFC5082`_);
   - **ADD-PATH** capability (`RFC7911`_).
 
 - Automatic building of clients list:
 
   - `integration <https://arouteserver.readthedocs.io/en/latest/USAGE.html#ixp-manager-integration>`__ with **IXP-Manager**;
```

### Comparing `arouteserver-1.8.0/pierky/__init__.py` & `arouteserver-1.9.0/pierky/__init__.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/fingerprints.yml` & `arouteserver-1.9.0/pierky/arouteserver/templates/fingerprints.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 openbgpd:
   clients.j2: 518191e01b4b7194bd246b06977e54b83c53e66b0af2896c356bf1a81a41595b8dbb1e088c6f88e6d40042f3a3752d03a89c16c02e71204e41db8f7451fe3095
   filters.j2: 9eacf1262e058ed488ff862055ebad170dcf722389e8129f0959e5b5f4c805d0c1cda5337cbe95688e3b2b2748faf78ec328de8a88d0cb0ac5c5666e231f859e
   header.j2: 6d01b917dd01267e089c5b9bf887b918539e532d1fd99da297d3ede013c6678e737fb4f02d28da5ba9af81754795cac5516e940f1d2f6feb40549d982a7dbeac
   irrdb.j2: a41aff6077c4b7ddd8ae03f0ac33f3ff47c9812350204d929a8b02fe63d023a813e802a7c9183528058b55d7502f7aeaef77a65acc906022586510f37453b88a
   macros.j2: 2a2edfebbcc29835c91723da117052374b1d07c1d9e66a23717d248768cd628b7ea831971be28d42e57c58f59d27fa92333b3b0e66eb439029a0bbf9f69b85c4
   main.j2: c81d8a3d4052a440f3d404ebdadeeae181966447463f9733768d8d9da4304cd6ea1505a9fdb58e3df55521c44bd03174efa3d3f35b5b79b8d7dda17ee9589061
-  rpki.j2: 229426d64553f92b22237ed5e6f73ccf5366c0a5dfdf781d37ff8a57614662bb447e59ead30bd336c667b8f3164ec390f5944d1576713c5178b7398be350b683
+  rpki.j2: 88c5f73c7fc4f497c61b25f53d035ce15379f7d2b7e5d1ba6c170dd7a6a399f340019465e11d1cd21e4473772992d37d118e5517206368f2a9cffd6840776dd2
 template-context:
   main.j2: 3403633f71d29d06af2fcebde5fb38ba3dcf80357a966cbfcb41ddb86a081b0aeccd27e5951fa3017933b329cbec4a50caa62d4a65bacbbea6ecd9e1324e8b10
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/bird/irrdb.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/bird/irrdb.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/bird/common.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/bird/common.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/bird/header.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/bird/header.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/bird/clients.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/bird/clients.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/bird/main.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/bird/main.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/bird/macros.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/bird/macros.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/bird/rpki.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/bird/rpki.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/irrdb.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/irrdb.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/header.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/header.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/filters.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/filters.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/clients.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/clients.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/macros.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/macros.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/openbgpd/rpki.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/openbgpd/rpki.j2`

 * *Files 3% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 # ---------------------------------------------------------
 # RPKI-based Origin Validation
 
 {%   if "6.4"|target_version_ge %}
 
 # Add $INTCOMM_RPKI_UNKNOWN, $INTCOMM_RPKI_INVALID and $INTCOMM_RPKI_VALID
 # ext community on the basis of ovs.
-match from group clients ovs not-found set ext-community $INTCOMM_RPKI_UNKNOWN
-match from group clients ovs valid set ext-community $INTCOMM_RPKI_VALID
-match from group clients ovs invalid set ext-community $INTCOMM_RPKI_INVALID
+match from group clients ovs not-found set { ext-community $INTCOMM_RPKI_UNKNOWN ext-community ovs not-found }
+match from group clients ovs valid set { ext-community $INTCOMM_RPKI_VALID ext-community ovs valid }
+match from group clients ovs invalid set { ext-community $INTCOMM_RPKI_INVALID ext-community ovs invalid }
 
 {%   else %}
 
 # 1. Add $INTCOMM_RPKI_UNKNOWN ext community to all the routes.
 # 2. Add $INTCOMM_RPKI_INVALID ext community to all those routes
 #    whose prefix is covered by a ROA. Here, the aggregated address
 #    space made up by all the ROAs prefixes is used.
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/template-context/main.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/template-context/main.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/irr-as-set/plain_rpsl.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/irr-as-set/plain_rpsl.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/irr-as-set/ripe_ripeinator_yml.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/irr-as-set/ripe_ripeinator_yml.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/html/main.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/html/main.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/templates/html/macros.j2` & `arouteserver-1.9.0/pierky/arouteserver/templates/html/macros.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/check_new_release.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/check_new_release.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/clients_from_euroix.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/clients_from_euroix.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/configure.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/configure.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/setup.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/setup.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/setup_templates.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/setup_templates.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/base.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/base.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/__init__.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/ixf_member_list_from_clients.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/ixf_member_list_from_clients.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/verify_templates.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/verify_templates.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/clients_from_peeringdb.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/clients_from_peeringdb.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/tpl_rendering.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/tpl_rendering.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/init_scenario.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/init_scenario.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/commands/show_config.py` & `arouteserver-1.9.0/pierky/arouteserver/commands/show_config.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/base.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/base.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/__init__.py` & `arouteserver-1.9.0/pierky/arouteserver/__init__.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/mocked_env.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/mocked_env.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/instances.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,14 +213,23 @@
 
         localpref (int): local-pref.
 
         reject_reasons (list): list of integers that identify the reasons
             for which the route is considered to be rejected.
     """
 
+    # Constants used to map the BGP speaker's representations of
+    # RFC8097 extended communities into a normalised value that
+    # can be used by the test suite to match those communities.
+    # BIRD format: generic:0x43000000:0x[0, 1, 2]
+    # OpenBGPD format: ovs:[valid | not-found | invalid]
+    RFC8097_NOT_FOUND = "rfc8097-not-found"
+    RFC8097_VALID = "rfc8097-valid"
+    RFC8097_INVALID = "rfc8097-invalid"
+
     def _parse_bgp_communities(self, communities):
         if not communities:
             return []
 
         def parse_bgp_community(c):
             v = c
             if v.startswith("("):
@@ -238,14 +247,27 @@
 
     def _parse_std_bgp_communities(self, communities):
         return self._parse_bgp_communities(communities)
 
     def _parse_ext_bgp_communities(self, communities):
         return self._parse_bgp_communities(communities)
 
+    def _normalise_rfc8097(self, communities):
+        res = []
+        for comm in communities:
+            if comm in ("generic:0x43000000:0x1", "ovs:not-found"):
+                res.append(self.RFC8097_NOT_FOUND)
+            elif comm in ("generic:0x43000000:0x0", "ovs:valid"):
+                res.append(self.RFC8097_VALID)
+            elif comm in ("generic:0x43000000:0x2", "ovs:invalid"):
+                res.append(self.RFC8097_INVALID)
+            else:
+                res.append(comm)
+        return res
+
     def _parse_lrg_bgp_communities(self, communities):
         return self._parse_bgp_communities(communities)
 
     def __init__(self, prefix, **kwargs):
         self.prefix = prefix
         self.via = kwargs.get("via", None)
         self.as_path = kwargs.get("as_path", None)
@@ -254,15 +276,17 @@
         self.localpref = kwargs.get("localpref", None)
         if self.localpref:
             self.localpref = int(self.localpref)
         self.filtered = kwargs.get("filtered", False)
         self.best = kwargs.get("best", None)
         self.std_comms = self._parse_std_bgp_communities(kwargs.get("std_comms", None))
         self.lrg_comms = self._parse_lrg_bgp_communities(kwargs.get("lrg_comms", None))
-        self.ext_comms = self._parse_ext_bgp_communities(kwargs.get("ext_comms", None))
+        self.ext_comms = self._normalise_rfc8097(
+            self._parse_ext_bgp_communities(kwargs.get("ext_comms", None))
+        )
         self.reject_reasons = []
 
     def process_reject_cause(self, re_pattern, announced_by_pattern):
         # If a route is marked to be rejected using the 'reject_cause'
         # community it must be also set with LOCAL_PREF == 0.
         if self.localpref != 1:
             return
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/kvm.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/kvm.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/base.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/base.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/__init__.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/routinator.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/routinator.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/bird.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/bird.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
     MESSAGE_LOGGING_SUPPORT = True
 
     DOCKER_IMAGE = "pierky/bird:1.6.8"
 
     TAG = "bird16"
 
+    TARGET_VERSION = "1.6.8"
+
     def __init__(self, *args, **kwargs):
         DockerInstance.__init__(self, *args, **kwargs)
 
         # See the docstring of _get_protocols_status()
         self.protocols_status = {}
 
         self.routes = []
@@ -325,12 +327,14 @@
 
 class BIRD2Instance(BIRDInstance):
 
     DOCKER_IMAGE = "pierky/bird:2.0.8"
 
     TAG = "bird2"
 
+    TARGET_VERSION = "2.0.8"
+
     def _get_start_cmd(self):
         return "bird -c /etc/bird/bird.conf -d"
 
     def _birdcl(self, cmd):
         return self.run_cmd("birdcl {}".format(cmd))
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/openbgpd.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/openbgpd.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,47 +55,40 @@
         # If ', ' is not found, it's either a post 6.6 format
         # where different communities are separated just by a
         # space, or it's just one single community:
         # soo 65535:65281
         # rt 64537:10
         # rt 64537:10 rt 64538:20
 
-        next_field_should_be = "rt_soo"
-        rt_soo = ""
+        next_field_should_be_comm_type = True
+        comm_type = ""
         comm = ""
 
-        for part in communities.split(" "):
-            if next_field_should_be == "rt_soo":
-                if part not in ("rt", "soo"):
+        for part in communities.split():
+            if next_field_should_be_comm_type:
+                if part not in ("rt", "soo", "ovs"):
                     raise ValueError(
                         "Error while processing the extended communities "
-                        "string '{}': expected 'rt' or 'soo', but '{}' "
+                        "string '{}': expected 'rt', 'soo' or 'ovs', but '{}' "
                         "found.".format(communities, part)
                     )
-                rt_soo = part
-                next_field_should_be = "comm"
-            elif next_field_should_be == "comm":
-                if ":" not in part:
+                comm_type = part
+                next_field_should_be_comm_type = False
+            else:
+                if comm_type != "ovs" and ":" not in part:
                     raise ValueError(
                         "Error while processing the extended communities "
                         "string '{}': ':' not found in the community '{}' "
                         "part.".format(communities, part)
                     )
                 comm = part
 
-                res.append("{}:{}".format(rt_soo, comm))
+                res.append("{}:{}".format(comm_type, comm))
 
-                next_field_should_be = "rt_soo"
-
-        if next_field_should_be != "rt_soo":
-            raise ValueError(
-                "Error while processing the extended communities "
-                "string '{}': one part of the string remained "
-                "unprocessed.".format(communities)
-            )
+                next_field_should_be_comm_type = True
 
         return res
 
 class OpenBGPDInstance(object):
     """This class implements an interface to OpenBGPD client.
 
     Only methods needed to interact with the OpenBGPD bgpctl
@@ -522,52 +515,56 @@
 class OpenBGPD66PortableInstance(OpenBGPDPortableInstance):
 
     DOCKER_IMAGE = "pierky/openbgpd:6.6p0"
 
     TAG = "openbgpd66p"
 
     BGP_SPEAKER_VERSION = "6.6p0"
-    # TARGET_VERSION not set here because it's assumed to be
-    # the same of the OpenBGPD Latest one.
+    TARGET_VERSION = "6.6"
 
 class OpenBGPD67PortableInstance(OpenBGPDPortableInstance):
 
     DOCKER_IMAGE = "pierky/openbgpd:6.7p0"
 
     TAG = "openbgpd67p"
 
     BGP_SPEAKER_VERSION = "6.7p0"
-    # TARGET_VERSION not set here because it's assumed to be
-    # the same of the OpenBGPD Latest one.
+    TARGET_VERSION = "6.7"
 
 class OpenBGPD68PortableInstance(OpenBGPDPortableInstance):
 
     DOCKER_IMAGE = "pierky/openbgpd:6.8p1"
 
     TAG = "openbgpd68p"
 
     BGP_SPEAKER_VERSION = "6.8p1"
-    # TARGET_VERSION not set here because it's assumed to be
-    # the same of the OpenBGPD Latest one.
+    TARGET_VERSION = "6.8"
 
 class OpenBGPD69PortableInstance(OpenBGPDPortableInstance):
 
     DOCKER_IMAGE = "pierky/openbgpd:6.9p0-patches"
 
     TAG = "openbgpd69p"
 
     BGP_SPEAKER_VERSION = "6.9p0"
-    # TARGET_VERSION not set here because it's assumed to be
-    # the same of the OpenBGPD Latest one.
+    TARGET_VERSION = "6.9"
 
 class OpenBGPD70PortableInstance(OpenBGPDPortableInstance):
 
     DOCKER_IMAGE = "pierky/openbgpd:7.0p0"
 
     TAG = "openbgpd70p"
 
     BGP_SPEAKER_VERSION = "7.0p0"
-    # TARGET_VERSION not set here because it's assumed to be
-    # the same of the OpenBGPD Latest one.
+    TARGET_VERSION = "7.0"
+
+class OpenBGPD71PortableInstance(OpenBGPDPortableInstance):
+
+    DOCKER_IMAGE = "pierky/openbgpd:7.1p0"
+
+    TAG = "openbgpd71p"
+
+    BGP_SPEAKER_VERSION = "7.1p0"
+    TARGET_VERSION = "7.1"
 
 OpenBGPDPortablePreviousInstance = OpenBGPD68PortableInstance
-OpenBGPDPortableLatestInstance = OpenBGPD70PortableInstance
+OpenBGPDPortableLatestInstance = OpenBGPD71PortableInstance
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/exabgp.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/exabgp.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/AS2.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/AS2.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/irrdb.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/irrdb.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/common.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/common.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/header.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/header.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/clients.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/clients.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/main.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/main.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/macros.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/macros.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bird/rpki.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bird/rpki.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/irrdb.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/irrdb.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/header.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/header.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/filters.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/filters.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/clients.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/clients.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/macros.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/macros.j2`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/rpki.j2` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/openbgpd/rpki.j2`

 * *Files 3% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 # ---------------------------------------------------------
 # RPKI-based Origin Validation
 
 {%   if "6.4"|target_version_ge %}
 
 # Add $INTCOMM_RPKI_UNKNOWN, $INTCOMM_RPKI_INVALID and $INTCOMM_RPKI_VALID
 # ext community on the basis of ovs.
-match from group clients ovs not-found set ext-community $INTCOMM_RPKI_UNKNOWN
-match from group clients ovs valid set ext-community $INTCOMM_RPKI_VALID
-match from group clients ovs invalid set ext-community $INTCOMM_RPKI_INVALID
+match from group clients ovs not-found set { ext-community $INTCOMM_RPKI_UNKNOWN ext-community ovs not-found }
+match from group clients ovs valid set { ext-community $INTCOMM_RPKI_VALID ext-community ovs valid }
+match from group clients ovs invalid set { ext-community $INTCOMM_RPKI_INVALID ext-community ovs invalid }
 
 {%   else %}
 
 # 1. Add $INTCOMM_RPKI_UNKNOWN ext community to all the routes.
 # 2. Add $INTCOMM_RPKI_INVALID ext community to all those routes
 #    whose prefix is covered by a ROA. Here, the aggregated address
 #    space made up by all the ROAs prefixes is used.
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/test_openbgpd6.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/test_openbgpd6.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/test_bird4.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/test_bird4.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/base.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/base.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/__init__.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/bogons.yml` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/bogons.yml`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/general.yml` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/general.yml`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/test_bird6.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/test_bird6.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/skeleton/test_openbgpd4.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/test_openbgpd4.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/tests/live_tests/docker.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/docker.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/pdb_as_set.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/pdb_as_set.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/registrobr_db_dump.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/registrobr_db_dump.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/irr_db_dump.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/irr_db_dump.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,15 +86,29 @@
         irrdb_cfg = self.builder.cfg_general["filtering"]["irrdb"]
         whois_db_dump = irrdb_cfg[self.CONFIG_SECTION_NAME]
         source = whois_db_dump["source"]
 
         whois_db_dump = self.PARSER_CLASS(
             cache_dir=cache_dir, cache_expiry=self.builder.cache_expiry,
             source=source)
-        whois_db_dump.load_data()
+        try:
+            whois_db_dump.load_data()
+        except ARouteServerError as e:
+            raise e.__class__(
+                str(e) + " - "
+                "The error occurred while loading the IRR data from "
+                "{source}. If the data was moved to a different "
+                "location, it is possible to adjust the configuration "
+                "by changing the value of "
+                "'filtering.irrdb.{section}.source' inside "
+                "the general.yml file.".format(
+                    source=source,
+                    section=self.CONFIG_SECTION_NAME
+                )
+            )
         whois_records = whois_db_dump.whois_records
 
         # "ASx": ["1.2.3.0/24", ...]
         asn_prefixes = {}
 
         for record in whois_records:
             asn = record["originas"]
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/base.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/base.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/__init__.py` & `arouteserver-1.9.0/pierky/arouteserver/tests/live_tests/skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/pdb_never_via_route_servers.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/pdb_never_via_route_servers.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/rtt.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/rtt.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/pdb_max_prefix.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/pdb_max_prefix.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/irrdb.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/irrdb.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/arin_db_dump.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/arin_db_dump.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/enrichers/rpki_roas.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/rpki_roas.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,35 @@
                 return True
 
         return False
 
     def enrich(self):
         logging.info("Updating RPKI ROAs...")
 
+        roas_cache_expiry = self.builder.cache_expiry.get(
+            RIPE_RPKI_ROAs.EXPIRY_TIME_TAG,
+            self.builder.cache_expiry.get(
+                "general",
+                None
+            )
+        )
+
+        if roas_cache_expiry > 60 * 60:
+            logging.warning(
+                "The cache expiry time for the JSON files used to get RPKI ROAs "
+                "is set to {} seconds, which is more than 1 hour. "
+                "Given the stale data checks that are implemented since version "
+                "1.9.0 of ARouteServer, it is advisable to use a cache expiry "
+                "time not longer than 1 hour, in order to avoid caching ROAs "
+                "that would turn out being expired at the next usage of the "
+                "cached copy of the files. "
+                "This setting can be changed in the arouteserver.yml file, "
+                "'cache_expiry' section.".format(roas_cache_expiry)
+            )
+
         filtering = self.builder.cfg_general["filtering"]
         self._roas_as_route_object = \
             filtering["irrdb"]["use_rpki_roas_as_route_objects"]["enabled"]
         self._origin_validation = \
             filtering["rpki_bgp_origin_validation"]["enabled"]
 
         assert self._roas_as_route_object or self._origin_validation, \
@@ -76,18 +97,20 @@
 
         afis = [4, 6] if self.builder.ip_ver is None else [self.builder.ip_ver]
 
         rpki_roas_cfg = self.builder.cfg_general["rpki_roas"]
         assert rpki_roas_cfg["source"] == "ripe-rpki-validator-cache", \
             "source is not ripe-rpki-validator-cache"
         urls = rpki_roas_cfg["ripe_rpki_validator_url"]
+        ignore_cache_files_older_than = rpki_roas_cfg["ignore_cache_files_older_than"]
 
         ripe_cache = RIPE_RPKI_ROAs(cache_dir=self.builder.cache_dir,
                                     cache_expiry=self.builder.cache_expiry,
-                                    ripe_rpki_validator_url=urls)
+                                    ripe_rpki_validator_url=urls,
+                                    ignore_cache_files_older_than=ignore_cache_files_older_than)
         ripe_cache.load_data()
         roas = ripe_cache.roas
 
         allowed_tas = rpki_roas_cfg["allowed_trust_anchors"]
 
         roas_cnt = {
             "total": 0,
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/cached_objects.py` & `arouteserver-1.9.0/pierky/arouteserver/cached_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     return res
 
 class CachedObject(object):
 
     DEFAULT_EXPIRY = {
         "general": 43200,
         "pdb_info": 86400,
-        "ripe_rpki_roas": 43200,
+        "ripe_rpki_roas": 3600,
         "irr_as_sets": 43200,
         "arin_whois_db_dump": 43200,
         "registrobr_whois_db_dump": 43200
     }
 
     # Keep in sync with config.d/arouteserver.yml cache_expiry
     ALLOWED_EXPIRY_TIME_TAGS = ("general", "pdb_info", "ripe_rpki_roas",
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/__init__.py` & `arouteserver-1.9.0/pierky/arouteserver/config/__init__.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/ripe_rpki_cache.py` & `arouteserver-1.9.0/pierky/arouteserver/ripe_rpki_cache.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,46 +11,57 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import logging
+import datetime
 
 import requests
 
 from .cached_objects import CachedObject
 from .errors import RPKIValidatorCacheError
 from .ipaddresses import IPNetwork
 
 
 class RIPE_RPKI_ROAs(CachedObject):
 
     EXPIRY_TIME_TAG = "ripe_rpki_roas"
 
-    DEFAULT_URL = "https://rpki-validator.ripe.net/api/export.json"
+    DEFAULT_URL = "https://console.rpki-client.org/vrps.json"
+    DEFAULT_IGNORE_FILES_OLDER_THAN = 21600
 
     def __init__(self, *args, **kwargs):
         CachedObject.__init__(self, *args, **kwargs)
 
         self.urls = kwargs.get("ripe_rpki_validator_url",
                                [self.DEFAULT_URL])
 
+        self.ignore_cache_files_older_than = kwargs.get(
+            "ignore_cache_files_older_than",
+            self.DEFAULT_IGNORE_FILES_OLDER_THAN
+        )
+
         self.roas = {}
 
     def load_data(self):
         logging.debug("Loading RPKI ROAs...")
 
         CachedObject.load_data(self)
 
         self.roas = self.raw_data
 
     def _get_object_filename(self):
         return "ripe-rpki-cache.json"
 
+    @staticmethod
+    def _get_utc_now():
+        return datetime.datetime.utcnow()
+
     def _get_data_from_url(self, url):
         if url.lower().startswith(("http://", "https://")):
             logging.debug("Fetching RPKI ROAs from {}".format(url))
             try:
                 response = requests.get(url,
                                         headers={'Accept': 'text/json'})
                 response.raise_for_status()
@@ -93,18 +104,106 @@
             )
 
         if "roas" not in roas:
             raise RPKIValidatorCacheError("missing 'roas' root element")
         if not isinstance(roas["roas"], list):
             raise RPKIValidatorCacheError("'roas' root element is not a list")
 
+        buildtime_dt_utc = None
+
+        if "metadata" in roas and "buildtime" in roas["metadata"]:
+            # rpki-client format.
+
+            buildtime = roas["metadata"]["buildtime"]
+
+            try:
+                buildtime_dt_utc = datetime.datetime.strptime(
+                    buildtime,
+                    "%Y-%m-%dT%H:%M:%SZ"
+                )
+            except Exception as e:
+                raise RPKIValidatorCacheError(
+                    "Error while parsing metadata.buildtime from "
+                    "RPKI cache file ({}): {}".format(
+                        url, str(e)
+                    )
+                )
+
+        elif "metadata" in roas and "generated" in roas["metadata"]:
+            # OctoRPKI format.
+
+            generated = roas["metadata"]["generated"]
+
+            try:
+                buildtime_dt_utc = datetime.datetime.utcfromtimestamp(int(generated))
+            except Exception as e:
+                raise RPKIValidatorCacheError(
+                    "Error while parsing metadata.generated from "
+                    "RPKI cache file ({}): {}".format(
+                        url, str(e)
+                    )
+                )
+
+        if buildtime_dt_utc and buildtime_dt_utc < self._get_utc_now() - datetime.timedelta(
+            seconds=self.ignore_cache_files_older_than
+        ):
+            raise RPKIValidatorCacheError(
+                "The RPKI cache file from {} was built at {} UTC, "
+                "so it was generated more than {} seconds ago "
+                "(ignore_cache_files_older_than), hence "
+                "it will be ignored.".format(
+                    url,
+                    buildtime_dt_utc,
+                    self.ignore_cache_files_older_than
+                )
+            )
+
+        valid_dt_utc = None
+
+        if "metadata" in roas and "valid" in roas["metadata"]:
+            # OctoRPKI format.
+
+            valid = roas["metadata"]["valid"]
+
+            try:
+                valid_dt_utc = datetime.datetime.utcfromtimestamp(int(valid))
+            except Exception as e:
+                raise RPKIValidatorCacheError(
+                    "Error while parsing metadata.valid from "
+                    "RPKI cache file ({}): {}".format(
+                        url, str(e)
+                    )
+                )
+
+        if valid_dt_utc and valid_dt_utc < self._get_utc_now():
+            raise RPKIValidatorCacheError(
+                "The RPKI cache file from {} is valid till {} UTC, "
+                "hence it will be ignored.".format(
+                    url,
+                    valid_dt_utc
+                )
+            )
+
         max_invalid_roas = 10
         invalid = 0
+        timestamp_now_utc = int(datetime.datetime.timestamp(self._get_utc_now()))
+
+        result = {"roas": []}
         for roa in roas["roas"]:
             try:
+                if "expires" in roa:
+                    expires = roa["expires"]
+                    if not isinstance(expires, int):
+                        if not expires.isdigit():
+                            raise ValueError("invalid expires")
+                        else:
+                            expires = int(expires)
+                    if expires < timestamp_now_utc:
+                        continue
+
                 asn = roa.get("asn", None)
                 if asn is None:
                     raise ValueError("missing ASN")
                 if isinstance(asn, int):
                     roa["asn"] = "AS{}".format(asn)
                 elif asn.isdigit():
                     roa["asn"] = "AS{}".format(asn)
@@ -130,38 +229,40 @@
                     raise ValueError("missing maxLength")
                 if not isinstance(max_len, int):
                     if not max_len.isdigit():
                         raise ValueError("invalid maxLength: " + max_len)
                     else:
                         roa["maxLength"] = int(max_len)
 
+                result["roas"].append(roa)
+
             except ValueError as e:
                 logging.warning("Invalid ROA: {}, {}".format(
                     str(roa), str(e)
                 ))
 
                 invalid += 1
                 if invalid > max_invalid_roas:
                     raise RPKIValidatorCacheError(
                         "More than {} invalid ROAs have been found. "
                         "Aborting.".format(max_invalid_roas)
                     )
 
                 continue
 
-        return roas
+        return result
 
     def _get_data(self):
         # List of (url, error)
         errors = []
         for url in self.urls:
             try:
                 res = self._get_data_from_url(url)
                 logging.info(
-                        "RPKI ROAs loaded successfully from {}".format(url)
+                    "RPKI ROAs loaded successfully from {}".format(url)
                 )
                 return res
             except RPKIValidatorCacheError as e:
                 logging.warning(str(e))
                 errors.append((url, str(e)))
 
         exc_msg = "Impossible to load RPKI ROAs:\n"
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config.d/clients.yml` & `arouteserver-1.9.0/pierky/arouteserver/config.d/clients.yml`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config.d/bogons.yml` & `arouteserver-1.9.0/pierky/arouteserver/config.d/bogons.yml`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config.d/arouteserver.yml` & `arouteserver-1.9.0/pierky/arouteserver/config.d/arouteserver.yml`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 # Single value:
 #cache_expiry: 43200
 #
 # Multiple values (default):
 #cache_expiry:
 #  general: 43200
 #  pdb_info: 86400
-#  ripe_rpki_roas: 43200
+#  ripe_rpki_roas: 3600
 #  irr_as_sets: 43200
 #  arin_whois_db_dump: 43200
 
 # Enable automatic checking for new release.
 # When set to True, the program automatically checks PyPI for
 # a new release; if found, it logs a warning message.
 #check_new_release: True
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config.d/log.ini` & `arouteserver-1.9.0/pierky/arouteserver/config.d/log.ini`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config.d/rtt_getter.sh` & `arouteserver-1.9.0/pierky/arouteserver/config.d/rtt_getter.sh`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config.d/general.distrib.yml` & `arouteserver-1.9.0/pierky/arouteserver/config.d/general.distrib.yml`

 * *Files 2% similar despite different names*

```diff
@@ -310,15 +310,15 @@
         #
         # Default: False
         enabled: False
 
         # The source of the data must be set here.
         #
         # It can be an 'http://' or 'https://' URL or a local file
-        # path. The file must be in JSON format, accordingly to the
+        # path. The file must be in JSON format, according to the
         # following schema:
         #
         # {
         #   "json_schema": "0.0.2",
         #   "source": "ARIN-WHOIS",
         #   "whois_records": {
         #     "v4": [{"originas": "ASxxx", "prefix": "w.x.y.z/l"}],
@@ -532,14 +532,16 @@
     #   the RTR protocol BIRD must be compiled with --enable-libssh).
     # - 'ripe-rpki-validator-cache': ROAs are loaded from a JSON
     #   file in RIPE NCC RPKI Validator cache format.
     #
     #   Known compatible implementations at time of writing:
     #   - RIPE NCC RPKI Validator: https://www.ripe.net
     #   - Routinator: https://nlnetlabs.nl/projects/rpki/routinator/
+    #   - rpki-client: https://www.rpki-client.org/
+    #   - OctoRPKI: https://github.com/cloudflare/cfrpki
     #
     #   Please note that the second method is far from guaranteeing
     #   that a cryptographically validated dataset is retrieved
     #   from a trusted cache, unless the URL of a local, trusted
     #   instance of a RPKI validator is provided below in the
     #   'ripe_rpki_validator_url' option.
     #
@@ -549,28 +551,30 @@
     # URLs of files in RIPE NCC RPKI Validator cache format.
     # Meaningful only when 'source' is 'ripe-rpki-validator-cache'.
     # Multiple URLs can be provided here; they will be tried in
     # the same order in which they are listed below.
     # They can be 'http://' or 'https://' URLs or paths of
     # local files.
     #
-    # Default: RIPE NCC instance, NTT instance
+    # Default: rpki-client instance, NTT instance, RIPE NCC instance
     ripe_rpki_validator_url:
-      - "https://rpki-validator.ripe.net/api/export.json"
+      - "https://console.rpki-client.org/vrps.json"
       - "https://rpki.gin.ntt.net/api/export.json"
+      - "https://rpki-validator.ripe.net/api/export.json"
 
     # When using the 'ripe-rpki-validator-cache' source, only the
     # following Trust Anchors will be taken into account.
     #
     # Values must be taken among those published in the RIPE RPKI
     # Validator cache file configured above.
     #
     # Configured Trust Anchors pages:
     # - NTT instance: https://rpki.gin.ntt.net/trust-anchors
     # - RIPE NCC instance: https://rpki-validator.ripe.net/trust-anchors
+    # - rpki-client: https://console.rpki-client.org/
     #
     # Before enabling any ARIN TA, please consider the
     # following URLs:
     #
     # http://lists.arin.net/pipermail/arin-ppml/2017-January/031231.html
     #
     # https://www.arin.net/resources/rpki/rpa.pdf
@@ -584,14 +588,29 @@
       #- "ARIN"
       - "apnic"
       - "afrinic"
       - "lacnic"
       - "ripe"
       #- "arin"
 
+    # When using the 'ripe-rpki-validator-cache' source, ignore
+    # cache files that are older than this period of time (in
+    # seconds).
+    #
+    # When a file is ignored, the next source is used (from the
+    # 'ripe_rpki_validator_url' list).
+    #
+    # Depending on the format of the cache file, the build time
+    # may be unavailable. At the moment, this information is known
+    # to be included in the rpki-client and OctoRPKI JSON formats,
+    # but not in the original RIPE NCC RPKI Validator format.
+    #
+    # Default: 6 hours (21600 seconds).
+    ignore_cache_files_older_than: 21600
+
   blackhole_filtering:
     # Destination-based blackholing policy: if a policy is given,
     # accept prefixes of any length if they are tagged with the
     # 'blackholing' BGP community and if they are "covered by an
     # equal or shorter prefix that the neighboring network is
     # authorized to advertise."
     # (https://tools.ietf.org/html/rfc7999#section-3.3).
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/ipaddresses.py` & `arouteserver-1.9.0/pierky/arouteserver/ipaddresses.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/peering_db.py` & `arouteserver-1.9.0/pierky/arouteserver/peering_db.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/last_version.py` & `arouteserver-1.9.0/pierky/arouteserver/last_version.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/irrdb.py` & `arouteserver-1.9.0/pierky/arouteserver/irrdb.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/euro_ix.py` & `arouteserver-1.9.0/pierky/arouteserver/euro_ix.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/registro_br_db_dump.py` & `arouteserver-1.9.0/pierky/arouteserver/registro_br_db_dump.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/errors.py` & `arouteserver-1.9.0/pierky/arouteserver/errors.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/arin_db_dump.py` & `arouteserver-1.9.0/pierky/arouteserver/arin_db_dump.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/ask.py` & `arouteserver-1.9.0/pierky/arouteserver/ask.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/builder.py` & `arouteserver-1.9.0/pierky/arouteserver/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,15 +876,15 @@
                        "pre-irrdb", "post-irrdb",
                        "pre-clients", "post-clients", "client",
                        "pre-filters", "post-filters",
                        "footer"]
     LOCAL_FILES_BASE_DIR = "/etc/bgpd"
 
     AVAILABLE_VERSION = ["6.0", "6.1", "6.2", "6.3", "6.4", "6.5", "6.6", "6.7",
-                         "6.8", "6.9", "7.0"]
+                         "6.8", "6.9", "7.0", "7.1"]
     DEFAULT_VERSION = AVAILABLE_VERSION[-1]
 
     IGNORABLE_ISSUES = ["path_hiding", "transit_free_action",
                         "add_path", "max_prefix_action",
                         "max_prefix_count_rejected_routes",
                         "blackhole_filtering_rewrite_ipv6_nh",
                         "large_communities", "extended_communities",
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config/bogons.py` & `arouteserver-1.9.0/pierky/arouteserver/config/bogons.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config/base.py` & `arouteserver-1.9.0/pierky/arouteserver/config/base.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config/__init__.py` & `arouteserver-1.9.0/pierky/arouteserver/enrichers/__init__.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config/general.py` & `arouteserver-1.9.0/pierky/arouteserver/config/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,30 +208,32 @@
             ("ripe-rpki-validator-cache", "rtr"),
             mandatory=True,
             default="ripe-rpki-validator-cache"
         )
         r["ripe_rpki_validator_url"] = ValidatorListOf(
             ValidatorText, mandatory=True,
             default=[
-                "https://rpki-validator.ripe.net/api/export.json",
-                "https://rpki.gin.ntt.net/api/export.json"
+                "https://console.rpki-client.org/vrps.json",
+                "https://rpki.gin.ntt.net/api/export.json",
+                "https://rpki-validator.ripe.net/api/export.json"
             ]
         )
         r["allowed_trust_anchors"] = ValidatorListOf(
             ValidatorText, mandatory=True, default=[
                 "APNIC RPKI Root",
                 "AfriNIC RPKI Root",
                 "LACNIC RPKI Root",
                 "RIPE NCC RPKI Root",
                 "apnic",
                 "afrinic",
                 "lacnic",
                 "ripe"
             ]
         )
+        r["ignore_cache_files_older_than"] = ValidatorUInt(default=21600, mandatory=True)
 
         c["blackhole_filtering"] = OrderedDict()
         b = c["blackhole_filtering"]
 
         b["announce_to_client"] = ValidatorBool(mandatory=True, default=True)
         b["policy_ipv4"] = ValidatorOption(
             "policy_ipv4",
```

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config/clients.py` & `arouteserver-1.9.0/pierky/arouteserver/config/clients.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config/program.py` & `arouteserver-1.9.0/pierky/arouteserver/config/program.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config/asns.py` & `arouteserver-1.9.0/pierky/arouteserver/config/asns.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/config/validators.py` & `arouteserver-1.9.0/pierky/arouteserver/config/validators.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/resources.py` & `arouteserver-1.9.0/pierky/arouteserver/resources.py`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/pierky/arouteserver/version.py` & `arouteserver-1.9.0/pierky/arouteserver/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "1.8.0" # pragma: no cover
+__version__ = "1.9.0" # pragma: no cover
 COPYRIGHT_YEAR = 2021 # pragma: no cover
```

### Comparing `arouteserver-1.8.0/MANIFEST.in` & `arouteserver-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/arouteserver.egg-info/SOURCES.txt` & `arouteserver-1.9.0/arouteserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arouteserver-1.8.0/arouteserver.egg-info/PKG-INFO` & `arouteserver-1.9.0/arouteserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arouteserver
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Python tool to automatically build (and test) configurations for BGP route servers.
 Home-page: https://github.com/pierky/arouteserver
 Author: Pier Carlo Chiodi
 Author-email: pierky@pierky.com
 Maintainer: Pier Carlo Chiodi
 Maintainer-email: pierky@pierky.com
 License: GPLv3
@@ -25,85 +25,88 @@
         #. Two YAML files provide *general policies* and *clients configurations* options:
         
            .. code:: yaml
         
               cfg:
                 rs_as: 64496
                 router_id: "192.0.2.2"
-                add_path: True
                 filtering:
-                  next_hop:
-                    policy: "same-as"
-                blackhole_filtering:
-                  policy_ipv4: "rewrite-next-hop"
-                  ...
+                  irrdb:
+                    enforce_origin_in_as_set: True
+                    enforce_prefix_in_as_set: True
+                  rpki_bgp_origin_validation:
+                    enabled: True
+                    reject_invalid: True
+                    ...
         
            .. code:: yaml
         
               clients:
                 - asn: 64511
                   ip:
                   - "192.0.2.11"
                   - "2001:db8:1:1::11"
                   irrdb:
                     as_sets:
                       - "RIPE::AS-FOO"
                 ...
         
-        #. ARouteServer acquires external information to enrich them: i.e. `bgpq4`_/`bgpq3`_ for IRR data, `PeeringDB`_ for max-prefix limit and AS-SETs, ...
+        #. ARouteServer acquires external information to enrich them: i.e. `bgpq4`_/`bgpq3`_ for IRR data, `PeeringDB`_ for max-prefix limit and AS-SETs, RPKI ROAs, ...
         
         #. `Jinja2`_ built-in templates are used to render the final route server's configuration file.
         
-           Currently, **BIRD** (>= 1.6.3 up to 1.6.8), **BIRD v2** (starting from 2.0.7 - support for BIRD v2 is in `early stages <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html>`_) and **OpenBGPD** (OpenBSD 6.1 up to 7.0 and also OpenBGPD Portable 6.5p1 up to 7.0p0) are supported, with almost `feature parity <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html#supported-features>`_ between them.
+           Currently, **BIRD** (>= 1.6.3 up to 1.6.8), **BIRD v2** (starting from 2.0.7) and **OpenBGPD** (OpenBSD 6.1 up to 7.1 and also OpenBGPD Portable 6.5p1 up to 7.1p0) are supported, with almost `feature parity <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html#supported-features>`__ between them.
         
-        **Validation** and testing of the configurations generated with this tool are performed using the built-in **live tests** framework: `Docker`_ instances are used to simulate several scenarios and to validate the behaviour of the route server after configuring it with ARouteServer. More details on the `Live tests <https://arouteserver.readthedocs.io/en/latest/LIVETESTS.html>`_ section.
+        **Validation** and testing of the configurations generated with this tool are performed using the built-in **live tests** framework: `Docker`_ instances are used to simulate several scenarios and to validate the behaviour of the route server after configuring it with ARouteServer. More details on the `Live tests <https://arouteserver.readthedocs.io/en/latest/LIVETESTS.html>`__ section.
         
         A Docker-based `playground <https://github.com/pierky/arouteserver/tree/master/tools/playground>`__ is available to experiment with the tool in a virtual IXP environment.
         
         Also, a `Docker image <https://hub.docker.com/r/pierky/arouteserver>`__ is provided to start building rich and secure configurations in a couple of minutes.
         
         .. _bgpq3: https://github.com/snar/bgpq3
         .. _bgpq4: https://github.com/bgp/bgpq4
         .. _PeeringDB: https://www.peeringdb.com/
         .. _Jinja2: http://jinja.pocoo.org/
         .. _Docker: https://www.docker.com/
         
         Features
         --------
         
-        - **Path hiding** mitigation techniques (`RFC7947`_ `section 2.3.1 <https://tools.ietf.org/html/rfc7947#section-2.3.1>`_).
+        - **Path hiding** mitigation techniques (`RFC7947`_ `section 2.3.1 <https://tools.ietf.org/html/rfc7947#section-2.3.1>`__).
         
         - Basic filters (mostly enabled by default):
         
-          - **NEXT_HOP** enforcement (strict / same AS - `RFC7948`_ `section 4.8 <https://tools.ietf.org/html/rfc7948#section-4.8>`_);
+          - **NEXT_HOP** enforcement (strict / same AS - `RFC7948`_ `section 4.8 <https://tools.ietf.org/html/rfc7948#section-4.8>`__);
           - minimum and maximum IPv4/IPv6 **prefix length**;
           - maximum **AS_PATH length**;
           - reject **invalid AS_PATHs** (containing `private/invalid ASNs <http://mailman.nanog.org/pipermail/nanog/2016-June/086078.html>`_);
-          - reject AS_PATHs containing **transit-free** or **never via route-servers** ASNs (using `PeeringDB info_never_via_route_servers attribute <https://github.com/peeringdb/peeringdb/issues/394>`_);
+          - reject AS_PATHs containing **transit-free** or **never via route-servers** ASNs (using `PeeringDB info_never_via_route_servers attribute <https://github.com/peeringdb/peeringdb/issues/394>`__);
           - reject **bogons**;
           - **max-prefix limit** based on global or client-specific values or on **PeeringDB** data.
         
         - Prefixes and origin ASNs validation (also in *tag-only* mode):
         
-          - **IRR-based filters** (`RFC7948`_ `section 4.6.2 <https://tools.ietf.org/html/rfc7948#section-4.6.2>`_);
+          - **IRR-based filters** (`RFC7948`_ `section 4.6.2 <https://tools.ietf.org/html/rfc7948#section-4.6.2>`__);
           - AS-SETs configured manually or fetched from PeeringDB;
           - support for **IRR sources** (RIPE::AS-FOO, RADB::AS-BAR);
           - **white lists** support;
           - extended dataset for filters generation:
         
             - RPKI **ROAs used as route objects**;
-            - `Origin AS <https://mailman.nanog.org/pipermail/nanog/2017-December/093525.html>`_ from **ARIN Whois** database dump;
+            - `Origin AS <https://mailman.nanog.org/pipermail/nanog/2017-December/093525.html>`__ from **ARIN Whois** database dump;
             - `NIC.BR Whois data <https://ripe76.ripe.net/presentations/43-RIPE76_IRR101_Job_Snijders.pdf>`_ (slide n. 26) from Registro.br;
         
-          - **RPKI**-based filtering (BGP Prefix Origin Validation).
+          - **RPKI**-based filtering (BGP Prefix Origin Validation);
+        
+            - ROAs can be retrieved from publicly available JSON files or from a local validating cache.
         
         - **Blackhole filtering** support:
         
           - optional **NEXT_HOP rewriting**;
-          - signalling via BGP Communities (`BLACKHOLE <https://tools.ietf.org/html/rfc7999#section-5>`_ and custom communities);
+          - signalling via BGP Communities (`BLACKHOLE <https://tools.ietf.org/html/rfc7999#section-5>`__ and custom communities);
           - client-by-client control over propagation.
         
         - **Graceful shutdown** support:
         
           - honor the **GRACEFUL_SHUTDOWN** BGP community received from clients (`draft-ietf-grow-bgp-gshut-11 <https://tools.ietf.org/html/draft-ietf-grow-bgp-gshut-11>`_);
           - allow to perform a graceful shutdown of the route server itself.
         
@@ -113,15 +116,15 @@
           - do (not) announce to any / **peer** / on **RTT basis**;
           - **prepend** to any / **peer** / on **RTT basis**;
           - add **NO_EXPORT** / **NO_ADVERTISE** to any / **peer**;
           - custom informational BGP communities.
         
         - Optional session features on a client-by-client basis:
         
-          - prepend route server ASN (`RFC7947`_ `section 2.2.2.1 <https://tools.ietf.org/html/rfc7947#section-2.2.2.1>`_);
+          - prepend route server ASN (`RFC7947`_ `section 2.2.2.1 <https://tools.ietf.org/html/rfc7947#section-2.2.2.1>`__);
           - active sessions;
           - **GTSM** (Generalized TTL Security Mechanism - `RFC5082`_);
           - **ADD-PATH** capability (`RFC7911`_).
         
         - Automatic building of clients list:
         
           - `integration <https://arouteserver.readthedocs.io/en/latest/USAGE.html#ixp-manager-integration>`__ with **IXP-Manager**;
@@ -249,14 +252,44 @@
         
         
         Change log
         ==========
         
         .. note:: **Upgrade notes**: after upgrading, run the ``arouteserver setup-templates`` command to sync the local templates with those distributed with the new version. More details on the `Upgrading <https://arouteserver.readthedocs.io/en/latest/INSTALLATION.html#upgrading>`__ section of the documentation.
         
+        1.9.0
+        -----
+        
+        - New: Add support for `OpenBGPD 7.1 <https://marc.info/?l=openbgpd-users&m=162461267419135&w=2>`__, also added to the integration testing suite (portable edition only).
+        
+        - Improvement: provide hint on how to change URL for external IRR DB data sources.
+        
+          See also `GitHub issue 77 <https://github.com/pierky/arouteserver/issues/77>`_.
+        
+        - Fix (OpenBGPD only): `RFC8097 communities <https://datatracker.ietf.org/doc/html/rfc8097>`_ were not added after BGP Origin Validation.
+        
+          The *BGP Prefix Origin Validation State Extended Communities* were not added when RPKI OV was performed. INVALID routes were still dropped when the route server was configured to do so (those routes are internally marked using locally-meaningful communities).
+        
+        - Improvement: RPKI ROAs files are checked for stale data.
+        
+          The JSON files fetched from validating caches are now checked to detect stale data (rpki-client and OctoRPKI formats include this information) and they are ignored if the data they contain is no longer valid. In this case, the next URL in the ``rpki_roas.ripe_rpki_validator_url`` list is used.
+        
+          By default, files whose content is older than 21600 seconds (6 hours) are ignored; it's possible to change this option via the newly introduced ``rpki_roas.ignore_cache_files_older_than`` setting.
+        
+          Where available (rpki-client format only at this time), also the `VRP expiration time <https://github.com/openbsd/src/commit/a66158d7f8cdffc32bf2f8aa5d8bbed1f08a3a3d#diff-b2e9c61c4c7cfd2d5a0cde6066efe9a7c18dd1bdf06b1e473abc054261ea315c>`__ is checked.
+        
+          As a consequence of this, the default ARouteServer cache expiration time for RPKI ROAs JSON files has been reduced to 60 minutes, to avoid caching ROAs that would turn out being expired at the next use of their cached copy.
+        
+        - Improvement: new order for the default URLs of the RPKI JSON files.
+        
+          Since the RIPE NCC RPKI Validator `is now in EoL <https://labs.ripe.net/author/nathalie_nathalie/lifecycle-of-the-ripe-ncc-rpki-validator/>`__, the URL of the JSON file that points to rpki-validator.ripe.net has been moved as the last resort option for ``rpki_roas.ripe_rpki_validator_url``.
+          The one exposed in the `rpki-client dashboard <https://console.rpki-client.org/>`__ has been added.
+        
+          Please note: this change only affects the default configuration file that ships with ARouteServer and is not be automatically reflected in existing configurations that route-servers operators are already using. If you wish this setup to be reflected in your configuration, please update your general.yml file accordingly.
+        
         1.8.0
         -----
         
         - Improvement: add the ``logging`` option to ``--use-local-files`` argument, to allow customization of logging settings.
         
           Details on the documentation: `Logging configuration of the BGP daemon <https://arouteserver.readthedocs.io/en/latest/CONFIG.html#logging-configuration-of-the-bgp-daemon>`__.
```

### Comparing `arouteserver-1.8.0/PKG-INFO` & `arouteserver-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arouteserver
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Python tool to automatically build (and test) configurations for BGP route servers.
 Home-page: https://github.com/pierky/arouteserver
 Author: Pier Carlo Chiodi
 Author-email: pierky@pierky.com
 Maintainer: Pier Carlo Chiodi
 Maintainer-email: pierky@pierky.com
 License: GPLv3
@@ -25,85 +25,88 @@
         #. Two YAML files provide *general policies* and *clients configurations* options:
         
            .. code:: yaml
         
               cfg:
                 rs_as: 64496
                 router_id: "192.0.2.2"
-                add_path: True
                 filtering:
-                  next_hop:
-                    policy: "same-as"
-                blackhole_filtering:
-                  policy_ipv4: "rewrite-next-hop"
-                  ...
+                  irrdb:
+                    enforce_origin_in_as_set: True
+                    enforce_prefix_in_as_set: True
+                  rpki_bgp_origin_validation:
+                    enabled: True
+                    reject_invalid: True
+                    ...
         
            .. code:: yaml
         
               clients:
                 - asn: 64511
                   ip:
                   - "192.0.2.11"
                   - "2001:db8:1:1::11"
                   irrdb:
                     as_sets:
                       - "RIPE::AS-FOO"
                 ...
         
-        #. ARouteServer acquires external information to enrich them: i.e. `bgpq4`_/`bgpq3`_ for IRR data, `PeeringDB`_ for max-prefix limit and AS-SETs, ...
+        #. ARouteServer acquires external information to enrich them: i.e. `bgpq4`_/`bgpq3`_ for IRR data, `PeeringDB`_ for max-prefix limit and AS-SETs, RPKI ROAs, ...
         
         #. `Jinja2`_ built-in templates are used to render the final route server's configuration file.
         
-           Currently, **BIRD** (>= 1.6.3 up to 1.6.8), **BIRD v2** (starting from 2.0.7 - support for BIRD v2 is in `early stages <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html>`_) and **OpenBGPD** (OpenBSD 6.1 up to 7.0 and also OpenBGPD Portable 6.5p1 up to 7.0p0) are supported, with almost `feature parity <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html#supported-features>`_ between them.
+           Currently, **BIRD** (>= 1.6.3 up to 1.6.8), **BIRD v2** (starting from 2.0.7) and **OpenBGPD** (OpenBSD 6.1 up to 7.1 and also OpenBGPD Portable 6.5p1 up to 7.1p0) are supported, with almost `feature parity <https://arouteserver.readthedocs.io/en/latest/SUPPORTED_SPEAKERS.html#supported-features>`__ between them.
         
-        **Validation** and testing of the configurations generated with this tool are performed using the built-in **live tests** framework: `Docker`_ instances are used to simulate several scenarios and to validate the behaviour of the route server after configuring it with ARouteServer. More details on the `Live tests <https://arouteserver.readthedocs.io/en/latest/LIVETESTS.html>`_ section.
+        **Validation** and testing of the configurations generated with this tool are performed using the built-in **live tests** framework: `Docker`_ instances are used to simulate several scenarios and to validate the behaviour of the route server after configuring it with ARouteServer. More details on the `Live tests <https://arouteserver.readthedocs.io/en/latest/LIVETESTS.html>`__ section.
         
         A Docker-based `playground <https://github.com/pierky/arouteserver/tree/master/tools/playground>`__ is available to experiment with the tool in a virtual IXP environment.
         
         Also, a `Docker image <https://hub.docker.com/r/pierky/arouteserver>`__ is provided to start building rich and secure configurations in a couple of minutes.
         
         .. _bgpq3: https://github.com/snar/bgpq3
         .. _bgpq4: https://github.com/bgp/bgpq4
         .. _PeeringDB: https://www.peeringdb.com/
         .. _Jinja2: http://jinja.pocoo.org/
         .. _Docker: https://www.docker.com/
         
         Features
         --------
         
-        - **Path hiding** mitigation techniques (`RFC7947`_ `section 2.3.1 <https://tools.ietf.org/html/rfc7947#section-2.3.1>`_).
+        - **Path hiding** mitigation techniques (`RFC7947`_ `section 2.3.1 <https://tools.ietf.org/html/rfc7947#section-2.3.1>`__).
         
         - Basic filters (mostly enabled by default):
         
-          - **NEXT_HOP** enforcement (strict / same AS - `RFC7948`_ `section 4.8 <https://tools.ietf.org/html/rfc7948#section-4.8>`_);
+          - **NEXT_HOP** enforcement (strict / same AS - `RFC7948`_ `section 4.8 <https://tools.ietf.org/html/rfc7948#section-4.8>`__);
           - minimum and maximum IPv4/IPv6 **prefix length**;
           - maximum **AS_PATH length**;
           - reject **invalid AS_PATHs** (containing `private/invalid ASNs <http://mailman.nanog.org/pipermail/nanog/2016-June/086078.html>`_);
-          - reject AS_PATHs containing **transit-free** or **never via route-servers** ASNs (using `PeeringDB info_never_via_route_servers attribute <https://github.com/peeringdb/peeringdb/issues/394>`_);
+          - reject AS_PATHs containing **transit-free** or **never via route-servers** ASNs (using `PeeringDB info_never_via_route_servers attribute <https://github.com/peeringdb/peeringdb/issues/394>`__);
           - reject **bogons**;
           - **max-prefix limit** based on global or client-specific values or on **PeeringDB** data.
         
         - Prefixes and origin ASNs validation (also in *tag-only* mode):
         
-          - **IRR-based filters** (`RFC7948`_ `section 4.6.2 <https://tools.ietf.org/html/rfc7948#section-4.6.2>`_);
+          - **IRR-based filters** (`RFC7948`_ `section 4.6.2 <https://tools.ietf.org/html/rfc7948#section-4.6.2>`__);
           - AS-SETs configured manually or fetched from PeeringDB;
           - support for **IRR sources** (RIPE::AS-FOO, RADB::AS-BAR);
           - **white lists** support;
           - extended dataset for filters generation:
         
             - RPKI **ROAs used as route objects**;
-            - `Origin AS <https://mailman.nanog.org/pipermail/nanog/2017-December/093525.html>`_ from **ARIN Whois** database dump;
+            - `Origin AS <https://mailman.nanog.org/pipermail/nanog/2017-December/093525.html>`__ from **ARIN Whois** database dump;
             - `NIC.BR Whois data <https://ripe76.ripe.net/presentations/43-RIPE76_IRR101_Job_Snijders.pdf>`_ (slide n. 26) from Registro.br;
         
-          - **RPKI**-based filtering (BGP Prefix Origin Validation).
+          - **RPKI**-based filtering (BGP Prefix Origin Validation);
+        
+            - ROAs can be retrieved from publicly available JSON files or from a local validating cache.
         
         - **Blackhole filtering** support:
         
           - optional **NEXT_HOP rewriting**;
-          - signalling via BGP Communities (`BLACKHOLE <https://tools.ietf.org/html/rfc7999#section-5>`_ and custom communities);
+          - signalling via BGP Communities (`BLACKHOLE <https://tools.ietf.org/html/rfc7999#section-5>`__ and custom communities);
           - client-by-client control over propagation.
         
         - **Graceful shutdown** support:
         
           - honor the **GRACEFUL_SHUTDOWN** BGP community received from clients (`draft-ietf-grow-bgp-gshut-11 <https://tools.ietf.org/html/draft-ietf-grow-bgp-gshut-11>`_);
           - allow to perform a graceful shutdown of the route server itself.
         
@@ -113,15 +116,15 @@
           - do (not) announce to any / **peer** / on **RTT basis**;
           - **prepend** to any / **peer** / on **RTT basis**;
           - add **NO_EXPORT** / **NO_ADVERTISE** to any / **peer**;
           - custom informational BGP communities.
         
         - Optional session features on a client-by-client basis:
         
-          - prepend route server ASN (`RFC7947`_ `section 2.2.2.1 <https://tools.ietf.org/html/rfc7947#section-2.2.2.1>`_);
+          - prepend route server ASN (`RFC7947`_ `section 2.2.2.1 <https://tools.ietf.org/html/rfc7947#section-2.2.2.1>`__);
           - active sessions;
           - **GTSM** (Generalized TTL Security Mechanism - `RFC5082`_);
           - **ADD-PATH** capability (`RFC7911`_).
         
         - Automatic building of clients list:
         
           - `integration <https://arouteserver.readthedocs.io/en/latest/USAGE.html#ixp-manager-integration>`__ with **IXP-Manager**;
@@ -249,14 +252,44 @@
         
         
         Change log
         ==========
         
         .. note:: **Upgrade notes**: after upgrading, run the ``arouteserver setup-templates`` command to sync the local templates with those distributed with the new version. More details on the `Upgrading <https://arouteserver.readthedocs.io/en/latest/INSTALLATION.html#upgrading>`__ section of the documentation.
         
+        1.9.0
+        -----
+        
+        - New: Add support for `OpenBGPD 7.1 <https://marc.info/?l=openbgpd-users&m=162461267419135&w=2>`__, also added to the integration testing suite (portable edition only).
+        
+        - Improvement: provide hint on how to change URL for external IRR DB data sources.
+        
+          See also `GitHub issue 77 <https://github.com/pierky/arouteserver/issues/77>`_.
+        
+        - Fix (OpenBGPD only): `RFC8097 communities <https://datatracker.ietf.org/doc/html/rfc8097>`_ were not added after BGP Origin Validation.
+        
+          The *BGP Prefix Origin Validation State Extended Communities* were not added when RPKI OV was performed. INVALID routes were still dropped when the route server was configured to do so (those routes are internally marked using locally-meaningful communities).
+        
+        - Improvement: RPKI ROAs files are checked for stale data.
+        
+          The JSON files fetched from validating caches are now checked to detect stale data (rpki-client and OctoRPKI formats include this information) and they are ignored if the data they contain is no longer valid. In this case, the next URL in the ``rpki_roas.ripe_rpki_validator_url`` list is used.
+        
+          By default, files whose content is older than 21600 seconds (6 hours) are ignored; it's possible to change this option via the newly introduced ``rpki_roas.ignore_cache_files_older_than`` setting.
+        
+          Where available (rpki-client format only at this time), also the `VRP expiration time <https://github.com/openbsd/src/commit/a66158d7f8cdffc32bf2f8aa5d8bbed1f08a3a3d#diff-b2e9c61c4c7cfd2d5a0cde6066efe9a7c18dd1bdf06b1e473abc054261ea315c>`__ is checked.
+        
+          As a consequence of this, the default ARouteServer cache expiration time for RPKI ROAs JSON files has been reduced to 60 minutes, to avoid caching ROAs that would turn out being expired at the next use of their cached copy.
+        
+        - Improvement: new order for the default URLs of the RPKI JSON files.
+        
+          Since the RIPE NCC RPKI Validator `is now in EoL <https://labs.ripe.net/author/nathalie_nathalie/lifecycle-of-the-ripe-ncc-rpki-validator/>`__, the URL of the JSON file that points to rpki-validator.ripe.net has been moved as the last resort option for ``rpki_roas.ripe_rpki_validator_url``.
+          The one exposed in the `rpki-client dashboard <https://console.rpki-client.org/>`__ has been added.
+        
+          Please note: this change only affects the default configuration file that ships with ARouteServer and is not be automatically reflected in existing configurations that route-servers operators are already using. If you wish this setup to be reflected in your configuration, please update your general.yml file accordingly.
+        
         1.8.0
         -----
         
         - Improvement: add the ``logging`` option to ``--use-local-files`` argument, to allow customization of logging settings.
         
           Details on the documentation: `Logging configuration of the BGP daemon <https://arouteserver.readthedocs.io/en/latest/CONFIG.html#logging-configuration-of-the-bgp-daemon>`__.
```

