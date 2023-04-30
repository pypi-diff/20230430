# Comparing `tmp/salt_nornir-0.8.0.tar.gz` & `tmp/salt_nornir-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\salt_nornir-0.8.0.tar", last modified: Tue Dec 21 01:48:57 2021, max compression
+gzip compressed data, was "dist\salt_nornir-0.9.0.tar", last modified: Sun Feb 13 05:03:44 2022, max compression
```

## Comparing `salt_nornir-0.8.0.tar` & `salt_nornir-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/
--rw-rw-rw-   0        0        0     1071 2021-12-15 10:38:12.000000 salt_nornir-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     3185 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2143 2021-12-21 00:04:44.000000 salt_nornir-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir/
--rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.8.0/salt_nornir/__init__.py
--rw-rw-rw-   0        0        0      820 2021-12-15 11:51:45.000000 salt_nornir-0.8.0/salt_nornir/loader.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir/modules/
--rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.8.0/salt_nornir/modules/__init__.py
--rw-rw-rw-   0        0        0    97943 2021-12-21 00:04:51.000000 salt_nornir-0.8.0/salt_nornir/modules/nornir_proxy_execution_module.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir/proxy/
--rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.8.0/salt_nornir/proxy/__init__.py
--rw-rw-rw-   0        0        0    57659 2021-12-21 00:10:02.000000 salt_nornir-0.8.0/salt_nornir/proxy/nornir_proxy_module.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir/runners/
--rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.8.0/salt_nornir/runners/__init__.py
--rw-rw-rw-   0        0        0    19300 2021-12-21 00:04:50.000000 salt_nornir-0.8.0/salt_nornir/runners/nornir_proxy_runner_module.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir/states/
--rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.8.0/salt_nornir/states/__init__.py
--rw-rw-rw-   0        0        0    32229 2021-12-21 00:04:50.000000 salt_nornir-0.8.0/salt_nornir/states/nornir_proxy_state_module.py
-drwxrwxrwx   0        0        0        0 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir.egg-info/
--rw-rw-rw-   0        0        0     3185 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      109 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/salt_nornir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      143 2021-12-21 01:48:57.000000 salt_nornir-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1334 2021-12-21 01:23:21.000000 salt_nornir-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/
+-rw-rw-rw-   0        0        0     1071 2022-02-13 04:39:08.000000 salt_nornir-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     3230 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2188 2022-02-13 04:56:12.000000 salt_nornir-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/salt_nornir/
+-rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.9.0/salt_nornir/__init__.py
+-rw-rw-rw-   0        0        0      820 2021-12-15 11:51:45.000000 salt_nornir-0.9.0/salt_nornir/loader.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/salt_nornir/modules/
+-rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.9.0/salt_nornir/modules/__init__.py
+-rw-rw-rw-   0        0        0   102878 2022-02-13 04:56:18.000000 salt_nornir-0.9.0/salt_nornir/modules/nornir_proxy_execution_module.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/salt_nornir/proxy/
+-rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.9.0/salt_nornir/proxy/__init__.py
+-rw-rw-rw-   0        0        0    70790 2022-02-13 04:56:19.000000 salt_nornir-0.9.0/salt_nornir/proxy/nornir_proxy_module.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/salt_nornir/runners/
+-rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.9.0/salt_nornir/runners/__init__.py
+-rw-rw-rw-   0        0        0    19339 2022-02-13 04:50:46.000000 salt_nornir-0.9.0/salt_nornir/runners/nornir_proxy_runner_module.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/salt_nornir/states/
+-rw-rw-rw-   0        0        0        0 2021-12-15 11:51:45.000000 salt_nornir-0.9.0/salt_nornir/states/__init__.py
+-rw-rw-rw-   0        0        0    32229 2022-02-13 05:01:50.000000 salt_nornir-0.9.0/salt_nornir/states/nornir_proxy_state_module.py
+drwxrwxrwx   0        0        0        0 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/salt_nornir.egg-info/
+-rw-rw-rw-   0        0        0     3230 2022-02-13 05:03:43.000000 salt_nornir-0.9.0/salt_nornir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2022-02-13 05:03:43.000000 salt_nornir-0.9.0/salt_nornir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-13 05:03:43.000000 salt_nornir-0.9.0/salt_nornir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2022-02-13 05:03:43.000000 salt_nornir-0.9.0/salt_nornir.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      107 2022-02-13 05:03:43.000000 salt_nornir-0.9.0/salt_nornir.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-02-13 05:03:43.000000 salt_nornir-0.9.0/salt_nornir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2022-02-13 05:03:44.000000 salt_nornir-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1332 2022-02-13 04:38:10.000000 salt_nornir-0.9.0/setup.py
```

### Comparing `salt_nornir-0.8.0/LICENSE` & `salt_nornir-0.9.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Denis Mulyalin
+Copyright (c) 2022 Denis Mulyalin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `salt_nornir-0.8.0/PKG-INFO` & `salt_nornir-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt_nornir
-Version: 0.8.0
+Version: 0.9.0
 Summary: SALTSTACK Nornir Modules
 Home-page: https://github.com/dmulyalin/salt-nornir
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 License: UNKNOWN
 Description: [![Downloads](https://pepy.tech/badge/salt-nornir)](https://pepy.tech/project/salt-nornir)
         [![PyPI versions](https://img.shields.io/pypi/pyversions/salt-nornir.svg)](https://pypi.python.org/pypi/salt-nornir/)
@@ -33,15 +33,15 @@
         
         Nornir Proxy acts as a bridge between SaltStack and a wide set of network automation libraries.
         
         # Advantages
         
         Some notable benefits:
         
-        - Well tested - overall 382 tests combined as of release 0.8.0
+        - Well tested - overall 426 tests for `salt-nornir` and `nornir-salt` packages combined as of release 0.9.0
         - Brings together SaltStack and a wealth of open-source libraries - Nornir, Netmiko, NAPALM, Scrapli, Scrapli-Netconf, Ncclient, Genie&PyATS (free, not open-source), PyGNMI, NTC-Templates, TTP, Jmespath, lxml, xmltodict, requests
         - Capable of addressing overwhelming set of use cases from simple data retrieval and parsing to infrastructure provisioning, testing, orchestration and self-healing
         - Python is a first class citizen, need something special - write your own plugins, modules, scripts, codify your work flows
         - Integrate anything with anything, all you can do via CLI you can do via SaltStack and Nornir Python API or SaltStack REST API
         
         # Communication and discussion
```

### Comparing `salt_nornir-0.8.0/README.md` & `salt_nornir-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 Nornir Proxy acts as a bridge between SaltStack and a wide set of network automation libraries.
 
 # Advantages
 
 Some notable benefits:
 
-- Well tested - overall 382 tests combined as of release 0.8.0
+- Well tested - overall 426 tests for `salt-nornir` and `nornir-salt` packages combined as of release 0.9.0
 - Brings together SaltStack and a wealth of open-source libraries - Nornir, Netmiko, NAPALM, Scrapli, Scrapli-Netconf, Ncclient, Genie&PyATS (free, not open-source), PyGNMI, NTC-Templates, TTP, Jmespath, lxml, xmltodict, requests
 - Capable of addressing overwhelming set of use cases from simple data retrieval and parsing to infrastructure provisioning, testing, orchestration and self-healing
 - Python is a first class citizen, need something special - write your own plugins, modules, scripts, codify your work flows
 - Integrate anything with anything, all you can do via CLI you can do via SaltStack and Nornir Python API or SaltStack REST API
 
 # Communication and discussion
```

### Comparing `salt_nornir-0.8.0/salt_nornir/loader.py` & `salt_nornir-0.9.0/salt_nornir/loader.py`

 * *Files identical despite different names*

### Comparing `salt_nornir-0.8.0/salt_nornir/modules/nornir_proxy_execution_module.py` & `salt_nornir-0.9.0/salt_nornir/modules/nornir_proxy_execution_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,16 @@
      - Saves results to local file system using Nornir-Salt ToFileProcessor
    * - `to_dict`_
      - Transforms results to structured data using Nornir-Salt ResultSerializer
    * - `xml_flake`_
      - Uses Nornir-Salt DataProcessor ``xml_flake`` function to filter XML output
    * - `xpath`_
      - Uses Nornir-Salt DataProcessor ``xpath`` function to filter XML output
+   * - `worker`_
+     - Worker to use for task, supported values ``all`` or number from ``1`` to ``nornir_workers`` Proxy Minion parameter of default value 3
 
 Fx
 ++
 
 Uses Nornir-Salt ``FFun`` function to form a subset of hosts to run this task for.
 
 Supported functions: ``nr.task, nr.cli, nr.cfg, nr.cfg_gen, nr.test, nr.nc, nr.do, nr.http, nr.tping, nr.inventory``
@@ -357,14 +359,35 @@
 is True or ``success`` is False task considered as failed.
 
 Combining ``event_failed`` with ``nr.test`` function allows to implement event driven
 automation in response to certain tests failure. Each test translated to a separate
 task result and ``event_failed`` emit events on a per-test basis enabling to construct
 very granular react actions on Salt Master.
 
+Sample event content::
+
+    nornir-proxy/nrp1/ceos1/task/failed/nornir_salt.plugins.tasks.nr_test   {
+        "_stamp": "2022-02-11T11:14:16.081755",
+        "cmd": "_minion_event",
+        "data": {
+            "changed": false,
+            "connection_retry": 3,
+            "diff": "",
+            "exception": "",
+            "failed": true,
+            "host": "ceos1",
+            "name": "nornir_salt.plugins.tasks.nr_test",
+            "result": "Traceback (most recent call last):\\n  File \"/usr/local/lib/python3.6/site-packages/nornir/core/task.py\", line 99, in start\\n    r = self.task(self, **self.params)\\n  File \"/usr/local/lib/python3.6/site-packages/nornir_salt/plugins/tasks/nr_test.py\", line 65, in nr_test\\n    raise RuntimeError(excpt_msg)\\nRuntimeError\\n",
+            "task_retry": 3
+        },
+        "id": "nrp1",
+        "pretag": null,
+        "tag": "nornir-proxy/nrp1/ceos1/task/failed/nornir_salt.plugins.tasks.nr_test"
+    }
+
 Supported functions: ``nr.task, nr.cli, nr.cfg, nr.cfg_gen, nr.test, nr.nc, nr.do, nr.http, nr.gnmi, nr.file, nr.diff, nr.find, nr.learn``
 
 CLI Arguments:
 
 * ``event_failed`` - boolean, default is False, if True will emit events for failed tasks.
 
 Sample usage::
@@ -657,18 +680,25 @@
 ``/var/salt-nornir/{proxy_id}/files/``
 
 Supported functions: ``nr.task, nr.cli, nr.cfg, nr.cfg_gen, nr.nc, nr.do, nr.http, nr.gnmi``
 
 CLI Arguments:
 
 * ``tf`` - ``ToFileProcessor`` file group name where to save results
+* ``tf_skip_failed`` - boolean, default is False, if True, wil not save results for failed tasks
 
 Sample usage::
 
     salt nrp1 nr.cfg "logging host 1.1.1.1" tf="logging_config"
+    salt nrp1 nr.cfg "logging host 1.1.1.1" tf="logging_config" tf_skip_failed=True
+
+``tf_skip_failed`` can be useful when only want to save results to file for non failed tasks.
+For example, if ``RetryRunner`` runs task and it fails on first attempt but succeed on second,
+it might not make sense to store failed task results, which is the case by default, ``tf_skip_failed``
+help to alter that behavior.
 
 to_dict
 +++++++
 
 Uses Nornir Salt
 `ResultSerializer function <https://nornir-salt.readthedocs.io/en/latest/Functions/ResultSerializer.html#resultserializer>`_
 to transform task results in a structured data - dictionary or list.
@@ -729,14 +759,33 @@
 ``xpath`` function processes results received from device and executed locally on the minion
 machine, if you need to filter results returned from device, for ``nr.nc`` function consider
 using filter arguments. The complication is that if, for example, you running
 ``get_config`` NETCONF operation, full device config retrieved from device and passed via ``xpath``
 function on proxy minion, this could be processing intensive especially for big confiurations
 combined with significant number of devices simelteniously returning results.
 
+worker
+++++++
+
+Starting with Nornir 0.9.0 support added for several Nornir Insances with dedicated worker threads,
+allowing to greatly increase Proxy Minion task execution throughput. If no ``worker`` argument provided
+task can be executed by any of the workers.
+
+Supported functions: ``nr.task, nr.cli, nr.cfg, nr.cfg_gen, nr.test, nr.nc, nr.do, nr.http, nr.gnmi, nr.file, nr.diff, nr.find, nr.learn, nr.nornir``
+
+CLI Arguments:
+
+* ``worker`` - Worker to use for task, supported values ``all`` or number from ``1`` to ``nornir_workers`` Proxy Minion parameter of default value 3
+
+Sample usage::
+
+    salt nrp1 nr.cli "show clock" worker=3
+    salt nrp1 nr.nornir connections worker=2
+    salt nrp1 nr.nornir disconect worker=all
+
 Execution Module Functions
 --------------------------
 
 Table to summarize functions available in Nornir Proxy Execution Module and their purpose.
 
 +-----------------+---------------------------------------------------+--------------------+
 | nr.function     | description                                       | supported plugins  |
@@ -1060,24 +1109,25 @@
 
 def cfg(*commands, **kwargs):
     """
     Function to push configuration to devices using ``napalm_configure`` or
     ``netmiko_send_config`` or Scrapli ``send_config`` task plugin.
 
     :param commands: (list) list of commands or multiline string to send to device
-    :param filename: (str) path to file with configuration
+    :param filename: (str) path to file with configuration or template
     :param template_engine: (str) template engine to render configuration, default is jinja
     :param saltenv: (str) name of SALT environment
     :param context: Overrides default context variables passed to the template.
     :param defaults: Default context passed to the template.
     :param plugin: (str) name of configuration task plugin to use - ``napalm`` (default) or ``netmiko``
         or ``scrapli`` or ``pyats``
     :param dry_run: (bool) default False, controls whether to apply changes to device or simulate them
     :param commit: (bool or dict) by default commit is ``True``. With ``netmiko`` plugin
         dictionary ``commit`` argument supplied to commit call using ``**commit``
+    :param config: (str) configuration string or template to send to device
 
     .. warning:: ``dry_run`` not supported by ``netmiko`` and ``pyats`` plugins
 
     .. warning:: ``commit`` not supported by ``scrapli`` and ``pyats`` plugins. To commit need to send commit
         command as part of configuration, moreover, scrapli will not exit configuration mode,
         need to send exit command as part of configuration commands as well.
 
@@ -1089,14 +1139,16 @@
     Sample usage::
 
         salt nrp1 nr.cfg "logging host 1.1.1.1" "ntp server 1.1.1.2" FB="R[12]" dry_run=True
         salt nrp1 nr.cfg commands='["logging host 1.1.1.1", "ntp server 1.1.1.2"]' FB="R[12]"
         salt nrp1 nr.cfg "logging host 1.1.1.1" "ntp server 1.1.1.2" plugin="netmiko"
         salt nrp1 nr.cfg filename=salt://template/template_cfg.j2 FB="R[12]"
         salt nrp1 nr.cfg filename=salt://template/cfg.j2 FB="XR-1" commit='{"confirm": True}'
+        salt nrp1 nr.cfg config="snmp-server location {{ host.location }}"
+        salt nrp1 nr.cfg "snmp-server location {{ host.location }}"
 
     Filename argument can be a template string, for instance::
 
         salt nrp1 nr.cfg filename=salt://templates/{{ host.name }}_cfg.txt
 
     In that case filename rendered to form path string, after that, path string used to download file
     from master, downloaded file further rendered using specified template engine (Jinja2 by default).
@@ -1116,15 +1168,15 @@
         )
     """
     # get arguments
     default_kwargs = __proxy__["nornir.nr_data"]("nr_cfg")
     kwargs = {**default_kwargs, **kwargs}
     plugin = kwargs.pop("plugin", "napalm")
     kwargs.setdefault("add_details", True)
-    kwargs.setdefault("render", ["commands", "filename"])
+    kwargs.setdefault("render", ["commands", "filename", "config"])
     # get configuration commands
     commands = [commands] if isinstance(commands, str) else commands
     if any(commands):
         kwargs.setdefault("commands", commands)
     # decide on task plugin to run
     if plugin.lower() == "napalm":
         task_fun = "nornir_salt.plugins.tasks.napalm_configure"
@@ -1155,23 +1207,26 @@
     without pushing it to devices.
 
     :param filename: (str) path to template
     :param template_engine: (str) template engine to render configuration, default is jinja
     :param saltenv: (str) name of SALT environment
     :param context: Overrides default context variables passed to the template.
     :param defaults: Default context passed to the template.
+    :param config: (str) configuration string or template to send to device
 
     For configuration rendering purposes, in addition to normal `context variables
     <https://docs.saltstack.com/en/latest/ref/states/vars.html>`_
     template engine loaded with additional context variable `host`, to access Nornir host
     inventory data.
 
     Sample usage::
 
         salt nrp1 nr.cfg_gen filename=salt://templates/template.j2 FB="R[12]"
+        salt nrp1 nr.cfg_gen config="snmp-server location {{ host.location }}"
+        salt nrp1 nr.cfg_gen "snmp-server location {{ host.location }}"
 
     Sample template.j2 content::
 
         proxy data: {{ pillar.proxy }}
         jumphost_data: {{ host["jumphost"] }}
         hostname: {{ host.name }}
         platform: {{ host.platform }}
@@ -1195,15 +1250,15 @@
             fun="nr.cfg_gen",
             kwarg={"filename": "salt://template/{{ host.name }}_cfg.txt"},
         )
     """
     # get arguments
     default_kwargs = __proxy__["nornir.nr_data"]("nr_cfg")
     kwargs = {**default_kwargs, **kwargs}
-    kwargs.setdefault("render", ["commands", "filename"])
+    kwargs.setdefault("render", ["commands", "filename", "config"])
     # get configuration commands
     commands = [commands] if isinstance(commands, str) else commands
     if any(commands):
         kwargs.setdefault("commands", commands)
     # work and return results
     return __proxy__["nornir.execute_job"](
         task_fun="nornir_salt.plugins.tasks.salt_cfg_gen",
@@ -1419,15 +1474,15 @@
     reverse = kwargs.pop("reverse", False)  # table
     dump = kwargs.pop("dump", False)  # dump final test results
     test_results = []
     filtered_suite = []
     cli_not_command_tasks = ["run_ttp"]
 
     # check if need to download pattern file from salt master
-    if pattern.startswith("salt://"):
+    if str(pattern).startswith("salt://"):
         pattern = __salt__["cp.get_file_str"](pattern, saltenv=saltenv)
 
     # if test suite provided, download it from master and render it
     if isinstance(suite, str) and suite.startswith("salt://"):
         suite_name = suite
         suite = __salt__["slsutil.renderer"](suite)
         if not suite:
@@ -2038,14 +2093,15 @@
 def learn(*args, **kwargs):
     """
     Store task execution results to local filesystem on the minion using
     ``tf`` (to filename) attribute to form filenames.
 
     :param fun: (str) name of execution module function to call
     :param tf: (str) ``ToFileProcessor`` filegroup name
+    :param tf_skip_failed: (bool) default is True, do not save failed tasks
     :param args: (list) execution module function arguments
     :param kwargs: (dict) execution module function key-word arguments
 
     This task uses ``ToFileProcessor`` to store results and is a shortcut
     to calling individual exection module functions with ``tf`` argument.
 
     Supported exection module functions are ``cli, nc, do, http``. By default
@@ -2073,14 +2129,15 @@
             arg=["mac", "ip"],
             kwarg={"FB": "CORE-*"},
         )
     """
     supported_functions = ["cli", "do", "http", "nc"]
     fun = kwargs.pop("fun", "do")
     kwargs["tf"] = True if fun == "do" else kwargs.get("tf")
+    kwargs.setdefault("tf_skip_failed", True)  # do not learn failed tasks
     kwargs["identity"] = _form_identity(
         kwargs, "learn.{}".format(".".join(args) if fun == "do" else fun)
     )
 
     # run sanity checks
     if fun not in supported_functions:
         raise RuntimeError(
@@ -2245,60 +2302,89 @@
     Function to call various Nornir utility functions.
 
     :param fun: (str) utility function name to call
     :param kwargs: (dict) function arguments
 
     Available utility functions:
 
+    * ``dir`` - return a list of supported functions
     * ``test`` - this method tests proxy minion module worker thread without invoking any Nornir code
     * ``refresh`` - re-instantiates Nornir object after retrieving latest pillar data from Salt Master
     * ``kill`` - executes immediate shutdown of Nornir Proxy Minion process and child processes
     * ``shutdown`` - gracefully shutdowns Nornir Proxy Minion process and child processes
-    * ``inventory`` - interract with Nornir Process inventory data, using ``InventoryFun`` function
+    * ``inventory`` - interract with Nornir Process inventory data, using ``InventoryFun`` function,
+      by default, for ``read_host, read, read_inventory, list_hosts`` operations any Nornir worker
+      can respond, for other, non-read operations targets all Nornir workers
     * ``stats`` - returns statistics about Nornir proxy process, accepts ``stat`` argument of stat
       name to return
     * ``version`` - returns a report of Nornir related packages installed versions
     * ``initialized`` - returns Nornir Proxy Minion initialized status - True or False
     * ``hosts`` - returns a list of hosts managed by this Nornir Proxy Minion, accepts ``Fx``
       arguments to return only hosts matched by filter
-    * ``connections`` - list hosts' active connections, accepts ``Fx`` arguments to filter hosts to list
+    * ``connections`` - list hosts' active connections for all workers, accepts ``Fx`` arguments to filter hosts to list,
+      by default returns connections data for all Nornir workers
     * ``disconnect`` - close host connections, accepts ``Fx`` arguments to filter hosts and ``conn_name``
-      of connection to close, by default closes all connections
+      of connection to close, by default closes all connections for all Nornir workers
     * ``clear_hcache`` - clear task results cache from hosts' data, accepts ``cache_keys`` list argument
-      of key names to remove, if no ``cache_keys`` argument provided removes all cached data
+      of key names to remove, if no ``cache_keys`` argument provided removes all cached data, by default targets all Nornir workers
     * ``clear_dcache`` - clear task results cache from defaults data, accepts ``cache_keys`` list argument
-      of key names to remove, if no ``cache_keys`` argument provided removes all cached data
+      of key names to remove, if no ``cache_keys`` argument provided removes all cached data, by default targets all Nornir workers
+    * ``workers/worker`` - call nornir worker utilities e.g. ``stats``
+    * ``results_queue_dump`` - return content of results queue
 
     Sample Usage::
 
         salt nrp1 nr.nornir inventory FB="R[12]"
+        salt nrp1 nr.nornir inventory FB="R[12]" worker="all"
         salt nrp1 nr.nornir inventory create_host name="R1" hostname="1.2.3.4" platform="ios" groups='["lab"]'
         salt nrp1 nr.nornir inventory update_host name="R1" data='{"foo": bar}'
         salt nrp1 nr.nornir inventory read_host FB="R1"
         salt nrp1 nr.nornir inventory call=delete_host name="R1"
         salt nrp1 nr.nornir stats stat="proxy_minion_id"
         salt nrp1 nr.nornir version
         salt nrp1 nr.nornir shutdown
         salt nrp1 nr.nornir clear_hcache cache_keys='["key1", "key2]'
         salt nrp1 nr.nornir clear_dcache cache_keys='["key1", "key2]'
+        salt nrp1 nr.nornir workers stats
 
     Sample Python API usage from Salt-Master::
 
         import salt.client
         client = salt.client.LocalClient()
 
         task_result = client.cmd(
             tgt="nrp1",
             fun="nr.nornir",
             arg=["stats"],
         )
     """
+    supported_functions = [
+        "dir",
+        "test",
+        "inventory",
+        "stats",
+        "version",
+        "shutdown",
+        "initialized",
+        "kill",
+        "refresh",
+        "connections",
+        "disconnect",
+        "clear_hcache",
+        "clear_dcache",
+        "workers",
+        "worker",
+        "results_queue_dump",
+    ]
     kwargs = {k: v for k, v in kwargs.items() if not k.startswith("__")}
     if fun == "inventory":
         kwargs.setdefault("call", args[0] if args else "read_inventory")
+        # make sure by default targets all workers for non read operations
+        if kwargs["call"] not in ["read_host", "read", "read_inventory", "list_hosts"]:
+            kwargs.setdefault("worker", "all")
         return task(plugin="inventory", **kwargs)
     elif fun == "stats":
         return __proxy__["nornir.stats"](*args, **kwargs)
     elif fun == "version":
         return __proxy__["nornir.nr_version"]()
     elif fun == "shutdown":
         return task(plugin="shutdown")
@@ -2309,41 +2395,56 @@
     elif fun == "refresh":
         return task(plugin="refresh", identity=_form_identity(kwargs, "nornir.refresh"))
     elif fun == "test":
         return task(plugin="test", identity=_form_identity(kwargs, "nornir.test"))
     elif fun == "hosts":
         return __proxy__["nornir.list_hosts"](**kwargs)
     elif fun == "connections":
+        kwargs.setdefault("worker", "all")
         return task(
             plugin="nornir_salt.plugins.tasks.connections",
             call="ls",
             identity=_form_identity(kwargs, "nornir.connections"),
             **kwargs,
         )
     elif fun == "disconnect":
+        kwargs.setdefault("worker", "all")
         return task(
             plugin="nornir_salt.plugins.tasks.connections",
             call="close",
             identity=_form_identity(kwargs, "nornir.disconnect"),
             **kwargs,
         )
     elif fun == "clear_hcache":
+        # make sure to cleare hcache for all workers by default
+        kwargs.setdefault("worker", "all")
         return task(
             plugin="nornir_salt.plugins.tasks.salt_clear_hcache",
             identity=_form_identity(kwargs, "nornir.clear_hcache"),
             **kwargs,
         )
     elif fun == "clear_dcache":
+        # make sure to always cleare dcache for all workers
+        kwargs["worker"] = "all"
         return task(
             plugin="clear_dcache",
             identity=_form_identity(kwargs, "nornir.clear_dcache"),
             **kwargs,
         )
+    elif fun in ["workers", "worker"]:
+        kwargs["call"] = args[0] if len(args) == 1 else kwargs["call"]
+        return __proxy__["nornir.workers_utils"](**kwargs)
+    elif fun == "dir":
+        return {"Supported functions": sorted(supported_functions)}
+    elif fun == "results_queue_dump":
+        return __proxy__["nornir.queues_utils"](call="results_queue_dump")
     else:
-        return "Uncknown function '{}'.format(fun)"
+        return "Uncknown function '{}', call 'dir' to list supported functions".format(
+            fun
+        )
 
 
 def gnmi(call, *args, **kwargs):
     """
     Function to interact with devices using gNMI protocol utilising one of supported plugins.
 
     :param call: (str) (str) connection object method to call or name of one of extra methods
```

### Comparing `salt_nornir-0.8.0/salt_nornir/proxy/nornir_proxy_module.py` & `salt_nornir-0.9.0/salt_nornir/proxy/nornir_proxy_module.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,26 +52,33 @@
 - ``runner`` - dictionary, Nornir Runner plugin parameters, default is
   `RetryRunner <https://nornir-salt.readthedocs.io/en/latest/Runners/RetryRunner.html#retryrunner-plugin>`_
 - ``inventory`` - dictionary, Nornir Inventory plugin parameters, default is
   `DictInventory  <https://nornir-salt.readthedocs.io/en/latest/Inventory%20Plugins.html#dictinventory-plugin>`_
   populated with data from proxy-minion pillar, pillar data ignored by any other inventory plugins
 - ``child_process_max_age`` - int, default is 660s, seconds to wait before forcefully kill child process
 - ``watchdog_interval`` - int, default is 30s, interval in seconds between watchdog runs
-- ``proxy_always_alive`` - boolean, default is True, keep connections with devices alive or tear them down after each job
+- ``proxy_always_alive`` - boolean, default is True, keep connections with devices alive or tear them down
+  immidiately after each job
+- ``connections_idle_timeout`` - int, seconds, default is 1 equivalent to ``proxy_always_alive`` set to True, if
+  value equals 0 renders same behavior as if ``proxy_always_alive`` is False, if value above 1 - all host's
+  device connections torn down after it was not in use for longer then idle timeout value even if
+  ``proxy_always_alive`` set to True
 - ``job_wait_timeout`` - int, default is 600s, seconds to wait for job return until give up
 - ``memory_threshold_mbyte`` - int, default is 300, value in MBytes above each to trigger ``memory_threshold_action``
 - ``memory_threshold_action`` - str, default is ``log``, action to implement if ``memory_threshold_mbyte`` exceeded,
   possible actions: ``log`` - send syslog message, ``restart`` - shuts down proxy minion process.
+- ``nornir_workers`` - number of Nornir instances to create, each instance has worker thread associated with it
+  allowing to run multiple tasks against hosts, as each worker deque tasks from jobs queue, default is 3
 - ``files_base_path`` - str, default is ``/var/salt-nornir/{proxy_id}/files/``, OS path to folder where to save files
   on a per-host basis using `ToFileProcessor <https://nornir-salt.readthedocs.io/en/latest/Processors/ToFileProcessor.html>_`,
 - ``files_max_count`` - int, default is 5, maximum number of file version for ``tf`` argument used by
   `ToFileProcessor <https://nornir-salt.readthedocs.io/en/latest/Processors/ToFileProcessor.html#tofileprocessor-plugin>`_
-- ``nr_cli`` - dictionary of default kwargs to use with ``nr.cli`` execution module function, default is ``{}``
-- ``nr_cfg`` - dictionary of default kwargs to use with ``nr.cfg`` execution module function, default is ``{}``
-- ``nr_nc`` - dictionary of default kwargs to use with ``nr.nc`` execution module function, default is ``{}``
+- ``nr_cli`` - dictionary of default arguments to use with ``nr.cli`` execution module function, default is none
+- ``nr_cfg`` - dictionary of default arguments to use with ``nr.cfg`` execution module function, default is none
+- ``nr_nc`` - dictionary of default arguments to use with ``nr.nc`` execution module function, default is none
 - ``event_progress_all`` - boolean, default is False, if True emits progress events for all tasks using
   `SaltEventProcessor <https://nornir-salt.readthedocs.io/en/latest/Processors/SaltEventProcessor.html>_`,
   per-task ``event_progress`` argument overrides ``event_progress_all`` parameter.
 
 Nornir uses `inventory <https://nornir.readthedocs.io/en/latest/tutorials/intro/inventory.html>`_
 to store information about devices to interact with. Inventory can contain
 information about ``hosts``, ``groups`` and ``defaults``. Nornir inventory
@@ -83,14 +90,15 @@
 
     proxy:
       proxytype: nornir
       process_count_max: 3
       multiprocessing: True
       nornir_filter_required: True
       proxy_always_alive: True
+      connections_idle_timeout: 1
       watchdog_interval: 30
       child_process_max_age: 660
       job_wait_timeout: 600
       memory_threshold_mbyte: 300
       memory_threshold_action: log
       files_base_path: "/var/salt-nornir/{proxy_id}/files/"
       files_max_count: 5
@@ -200,20 +208,24 @@
      - Un-gracefully shutdown Nornir Proxy Minion process
    * - `list_hosts`_
      - Produces a list of hosts' names managed by this Proxy
    * - `nr_data`_
      - To retrieve values from ``nornir_data`` Nornir Proxy Minion dictionary
    * - `ping`_
      - To test Nornir Proxy Minion process
+   * - `queues_utils`_
+     - Utility function to manage Proxy Minion queues
    * - `run`_
      - Used to run Nornir Task
    * - `shutdown`_
      - Gracefully shutdown Nornir Instance
    * - `stats`_
      - Produces a dictionary of Nornir Proxy Minion statistics
+   * - `workers_utils`_
+     - Utility function to manage Proxy Minion workers
 
 refresh_nornir
 ++++++++++++++
 
 .. autofunction:: salt_nornir.proxy.nornir_proxy_module._refresh_nornir
 
 execute_job
@@ -257,40 +269,51 @@
 .. autofunction:: salt_nornir.proxy.nornir_proxy_module.nr_version
 
 ping
 ++++
 
 .. autofunction:: salt_nornir.proxy.nornir_proxy_module.ping
 
+queues_utils
+++++++++++++
+
+.. autofunction:: salt_nornir.proxy.nornir_proxy_module.queues_utils
+
 run
 +++
 
 .. autofunction:: salt_nornir.proxy.nornir_proxy_module.run
 
 shutdown
 ++++++++
 
 .. autofunction:: salt_nornir.proxy.nornir_proxy_module.shutdown
 
 stats
 +++++
 
 .. autofunction:: salt_nornir.proxy.nornir_proxy_module.stats
+
+workers_utils
++++++++++++++
+
+.. autofunction:: salt_nornir.proxy.nornir_proxy_module.workers_utils
 """
 
 # Import python std lib
 import logging
 import threading
 import multiprocessing
 import queue
 import os
 import time
 import traceback
 import signal
 import psutil
+import copy
 
 try:
     import resource
 
     HAS_RESOURCE_LIB = True
 except ImportError:
     HAS_RESOURCE_LIB = False
@@ -366,32 +389,34 @@
     "main_process_host": os.uname()[1] if hasattr(os, "uname") else "",
     "main_process_fd_count": 0,
     "jobs_started": 0,
     "jobs_completed": 0,
     "jobs_failed": 0,
     "jobs_job_queue_size": 0,
     "jobs_res_queue_size": 0,
+    "nornir_workers": 0,
     "hosts_count": 0,
     "hosts_connections_active": 0,
     "hosts_tasks_failed": 0,
     "timestamp": time.ctime(),
     "watchdog_runs": 0,
     "watchdog_child_processes_killed": 0,
     "watchdog_dead_connections_cleaned": 0,
     "child_processes_count": 0,
     # "child_processes_ram_usage": 0
 }
 nornir_data = {
-    "nr": None,
     "initialized": False,
-    "stats": stats_dict.copy(),
+    "stats": copy.deepcopy(stats_dict),
     "jobs_queue": None,
     "res_queue": None,
     "worker_thread": None,
     "watchdog_thread": None,
+    "nornir_workers": None,
+    "nrs": [],
 }
 
 # -----------------------------------------------------------------------------
 # propery functions
 # -----------------------------------------------------------------------------
 
 
@@ -443,27 +468,48 @@
             "options": {
                 "hosts": opts["pillar"]["hosts"],
                 "groups": opts["pillar"].get("groups", {}),
                 "defaults": opts["pillar"].get("defaults", {}),
             },
         },
     )
-    nornir_data["nr"] = InitNornir(
-        logging={"enabled": False}, runner=runner_config, inventory=inventory_config
-    )
+    nornir_data["nornir_workers"] = opts["proxy"].get("nornir_workers", 3)
+    for i in range(nornir_data["nornir_workers"]):
+        nornir_data["nrs"].append(
+            {
+                "nr": InitNornir(
+                    logging={"enabled": False},
+                    runner=copy.deepcopy(runner_config),
+                    inventory=copy.deepcopy(inventory_config),
+                ),
+                "connections_lock": multiprocessing.Lock(),
+                "is_busy": multiprocessing.Event(),
+                "worker_jobs_started": 0,
+                "worker_jobs_completed": 0,
+                "worker_jobs_failed": 0,
+                "worker_hosts_tasks_failed": 0,
+                "worker_connections": {},
+                "worker_id": i + 1,
+                "worker_jobs_queue": multiprocessing.Queue(),
+            }
+        )
     # add parameters from proxy configuration
     nornir_data["nornir_filter_required"] = opts["proxy"].get(
         "nornir_filter_required", False
     )
     nornir_data["child_process_max_age"] = opts["proxy"].get(
         "child_process_max_age", 660
     )
     nornir_data["watchdog_interval"] = int(opts["proxy"].get("watchdog_interval", 30))
     nornir_data["job_wait_timeout"] = int(opts["proxy"].get("job_wait_timeout", 600))
     nornir_data["proxy_always_alive"] = opts["proxy"].get("proxy_always_alive", True)
+    nornir_data["connections_idle_timeout"] = opts["proxy"].get(
+        "connections_idle_timeout",
+        1 if nornir_data["proxy_always_alive"] is True else 0,
+    )
     nornir_data["event_progress_all"] = opts["proxy"].get("event_progress_all", False)
     nornir_data["memory_threshold_mbyte"] = int(
         opts["proxy"].get("memory_threshold_mbyte", 300)
     )
     nornir_data["memory_threshold_action"] = opts["proxy"].get(
         "memory_threshold_action", "log"
     )
@@ -474,39 +520,39 @@
     nornir_data["nr_cli"] = opts["proxy"].get("nr_cli", {})
     nornir_data["nr_cfg"] = opts["proxy"].get("nr_cfg", {})
     nornir_data["nr_nc"] = opts["proxy"].get("nr_nc", {})
     nornir_data["initialized"] = True
     # add some stats
     nornir_data["stats"]["proxy_minion_id"] = opts["id"]
     nornir_data["stats"]["main_process_is_running"] = 1
-    nornir_data["stats"]["hosts_count"] = len(nornir_data["nr"].inventory.hosts.keys())
+    nornir_data["stats"]["hosts_count"] = len(
+        nornir_data["nrs"][0]["nr"].inventory.hosts.keys()
+    )
     # Initiate multiprocessing related queus, locks and threads
-    nornir_data["connections_lock"] = multiprocessing.Lock()
     nornir_data["jobs_queue"] = multiprocessing.Queue()
     nornir_data["res_queue"] = multiprocessing.Queue()
     # if loader not None, meaning init() called by _refresh_nornir function
     if loader:
-        nornir_data["worker_thread"] = threading.Thread(
-            target=_worker, name="{}_worker".format(opts["id"]), args=(loader,)
-        )
+        loader = loader
     # salt >3003 requires loader context to call __salt__ within threads
     elif HAS_LOADER_CONTEXT:
-        nornir_data["worker_thread"] = threading.Thread(
-            target=_worker,
-            name="{}_worker".format(opts["id"]),
-            args=(__salt__.loader(),),
-        )
+        loader = __salt__.loader()
     # salt <3003 does not use loader context
     else:
-        nornir_data["worker_thread"] = threading.Thread(
-            target=_worker, name="{}_worker".format(opts["id"]), args=(None,)
-        )
-    nornir_data["worker_thread"].start()
+        loader = None
+    # start worker threads
+    for i in range(nornir_data["nornir_workers"]):
+        nornir_data["nrs"][i]["worker_thread"] = threading.Thread(
+            target=_worker, args=(nornir_data["nrs"][i], loader)
+        )
+    for nr in nornir_data["nrs"]:
+        nr["worker_thread"].start()
+    # start watchdog thread
     nornir_data["watchdog_thread"] = threading.Thread(
-        target=_watchdog, name="{}_watchdog".format(opts["id"])
+        target=_watchdog, name="{}_watchdog".format(opts["id"]), args=(loader,)
     )
     nornir_data["watchdog_thread"].start()
     return True
 
 
 def ping():
     """
@@ -535,25 +581,26 @@
     Proxy Minion process keeps running afterwards, but cannot do anything.
     """
     log.info("Nornir-proxy MAIN PID {}, shutting down Nornir".format(os.getpid()))
     try:
         # trigger worker and watchdogs threads to stop
         nornir_data["initialized"] = False
         # close connections to devices
-        nornir_data["nr"].close_connections(on_good=True, on_failed=True)
+        for nr in nornir_data["nrs"]:
+            nr["nr"].close_connections(on_good=True, on_failed=True)
         # close queues
         nornir_data["jobs_queue"].close()
         nornir_data["jobs_queue"].join_thread()
         nornir_data["res_queue"].close()
         nornir_data["res_queue"].join_thread()
         # kill child processes left
         for p in multiprocessing.active_children():
             os.kill(p.pid, signal.SIGKILL)
         # delete old Nornir Object
-        nornir_data["nr"] = None
+        nornir_data["nrs"] = []
         log.info("Nornir-proxy MAIN PID {}, Nornir shutted down".format(os.getpid()))
         return True
     except:
         tb = traceback.format_exc()
         log.error(
             "Nornir-proxy MAIN PID {}, Nornir shutdown failed, error: {}".format(
                 os.getpid(), tb
@@ -666,15 +713,15 @@
         module = __import__(plugin, fromlist=[""])
         task_function = getattr(module, task_fun)
         # save loaded task function to globals
         globals()[task_fun] = task_function
     return task_function
 
 
-def _watchdog():
+def _watchdog(loader):
     """
     Thread worker to maintain nornir proxy process and it's children liveability.
     """
     child_processes = {}
     while nornir_data["initialized"]:
         nornir_data["stats"]["watchdog_runs"] += 1
         # run FD limit checks
@@ -716,18 +763,20 @@
             log.error(
                 "Nornir-proxy MAIN PID {} watchdog, memory usage check error: {}".format(
                     os.getpid(), traceback.format_exc()
                 )
             )
         # check if worker thread is alive and restart it if not
         try:
-            if not nornir_data["worker_thread"].is_alive():
-                nornir_data["worker_thread"] = threading.Thread(
-                    target=_worker, name="{}_worker".format(opts["id"])
-                ).start()
+            for nr in nornir_data["nrs"]:
+                if not nr["worker_thread"].is_alive():
+                    nr["worker_thread"] = threading.Thread(
+                        target=_worker, args=(nr, loader)
+                    )
+                    nr["worker_thread"].start()
         except:
             log.error(
                 "Nornir-proxy MAIN PID {} watchdog, worker thread is_alive check error: {}".format(
                     os.getpid(), traceback.format_exc()
                 )
             )
         # Handle child processes lifespan
@@ -760,124 +809,199 @@
                     )
         except:
             log.error(
                 "Nornir-proxy MAIN PID {} watchdog, child processes error: {}".format(
                     os.getpid(), traceback.format_exc()
                 )
             )
+        # check if need to tear down connections that are idle
+        try:
+            # iterate over Nornir worker instances
+            timeout = nornir_data["connections_idle_timeout"]
+            for nr in nornir_data["nrs"]:
+                # get a list of hosts that aged beyond idle timeout
+                hosts_to_disconnect = []
+                if timeout > 1:
+                    for host_name in list(nr["worker_connections"].keys()):
+                        conn_data = nr["worker_connections"][host_name]
+                        age = time.time() - conn_data["last_use_timestamp"]
+                        if age > timeout:
+                            hosts_to_disconnect.append(host_name)
+                # run task to disconnect connections for aged hosts
+                if hosts_to_disconnect and nr["connections_lock"].acquire(block=False):
+                    try:
+                        aged_hosts = FFun(nr["nr"], FL=hosts_to_disconnect)
+                        aged_hosts.run(
+                            task=_get_or_import_task_fun(
+                                "nornir_salt.plugins.tasks.connections"
+                            ),
+                            call="close",
+                        )
+                        log.debug(
+                            "Nornir-proxy MAIN PID {} watchdog, nornir-worker-{}, disconnected: {}".format(
+                                os.getpid(), nr["worker_id"], hosts_to_disconnect
+                            )
+                        )
+                        # remove disconnected hosts from stats
+                        for h_name in hosts_to_disconnect:
+                            nr["worker_connections"].pop(h_name)
+                    except Exception as e:
+                        raise e
+                    finally:
+                        nr["connections_lock"].release()
+        except:
+            log.error(
+                "Nornir-proxy MAIN PID {} watchdog, connections idle check error: {}".format(
+                    os.getpid(), traceback.format_exc()
+                )
+            )
         # keepalive connections and clean up dead connections if any
         try:
-            if nornir_data["proxy_always_alive"] and nornir_data[
-                "connections_lock"
-            ].acquire(block=False):
-                try:
-                    stats = HostsKeepalive(nornir_data["nr"])
-                    nornir_data["stats"]["watchdog_dead_connections_cleaned"] += stats[
-                        "dead_connections_cleaned"
-                    ]
-                except Exception as e:
-                    raise e
-                finally:
-                    nornir_data["connections_lock"].release()
+            for nr in nornir_data["nrs"]:
+                if nornir_data["proxy_always_alive"] and nr["connections_lock"].acquire(
+                    block=False
+                ):
+                    log.debug(
+                        "Nornir-proxy {} MAIN PID {} watchdog, nornir-worker-{} connections keepalive".format(
+                            nornir_data["stats"]["proxy_minion_id"],
+                            nornir_data["stats"]["main_process_pid"],
+                            nr["worker_id"],
+                        )
+                    )
+                    try:
+                        stats = HostsKeepalive(nr["nr"])
+                        nornir_data["stats"][
+                            "watchdog_dead_connections_cleaned"
+                        ] += stats["dead_connections_cleaned"]
+                    except Exception as e:
+                        raise e
+                    finally:
+                        nr["connections_lock"].release()
         except:
             log.error(
                 "Nornir-proxy MAIN PID {} watchdog, HostsKeepalive check error: {}".format(
                     os.getpid(), traceback.format_exc()
                 )
             )
 
         time.sleep(nornir_data["watchdog_interval"])
 
 
-def _worker(loader=None):
+def _worker(wkr_data, loader):
     """
     Target function for worker thread to run jobs from
     jobs_queue submitted by execution module processes
+
+    :param wkr_data: (dict) dictionaru that contain nornir instance and other parameters
+    :param loader: (obj or None) SaltStack loader context object
     """
-    ppid = os.getpid()
+    worker_id = wkr_data["worker_id"]  # get worker ID integer
+    ppid = nornir_data["stats"]["main_process_pid"]
     while nornir_data["initialized"]:
+        wkr_data["is_busy"].clear()  # no longer busy
         time.sleep(0.01)
         job, output = None, None
         try:
-            # get job from queue
-            job = nornir_data["jobs_queue"].get(block=True, timeout=0.1)
-            # run job
-            nornir_data["stats"]["jobs_started"] += 1
+            # try to get job from worker specific queue
+            try:
+                job = wkr_data["worker_jobs_queue"].get(block=True, timeout=0.1)
+            except queue.Empty:
+                # check if all higher order workers are busy
+                if all(
+                    [
+                        wkr["is_busy"].is_set()
+                        for wkr in nornir_data["nrs"][: worker_id - 1]
+                    ]
+                ):
+                    # try to get job from shared queue
+                    job = nornir_data["jobs_queue"].get(block=True, timeout=0.1)
+                else:
+                    continue
+            # got the job, I am busy now
+            wkr_data["is_busy"].set()
+            wkr_data["worker_jobs_started"] += 1
             # check if its a call for a special task
             if job["task_fun"] == "test":
-                nornir_data["stats"]["jobs_completed"] += 1
+                wkr_data["worker_jobs_completed"] += 1
                 nornir_data["res_queue"].put(
                     {"output": True, "identity": job["identity"]}
                 )
                 continue
             if job["task_fun"] == "clear_dcache":
-                output = _clear_dcache(**job["kwargs"])
-                nornir_data["stats"]["jobs_completed"] += 1
+                output = _clear_dcache(
+                    nr=wkr_data["nr"], cache_keys=job["kwargs"].get("cache_keys")
+                )
+                wkr_data["worker_jobs_completed"] += 1
                 nornir_data["res_queue"].put(
                     {"output": output, "identity": job["identity"]}
                 )
                 continue
             if job["task_fun"] == "refresh":
-                nornir_data["stats"]["jobs_completed"] += 1
+                wkr_data["worker_jobs_completed"] += 1
                 nornir_data["res_queue"].put(
                     {"output": True, "identity": job["identity"]}
                 )
                 # loader used by decorator, loader_ used by _refresh_nornir itself
                 _refresh_nornir(loader=loader, loader_=loader)
                 # stop this worker thread as another one will be started
                 break
             if job["task_fun"] == "shutdown":
-                nornir_data["stats"]["jobs_completed"] += 1
+                wkr_data["worker_jobs_completed"] += 1
                 nornir_data["res_queue"].put(
                     {"output": True, "identity": job["identity"]}
                 )
                 # stop this worker thread as another one will be started
                 shutdown()
                 break
             if job["task_fun"] == "inventory":
-                output = InventoryFun(nornir_data["nr"], **job["kwargs"])
-                nornir_data["stats"]["jobs_completed"] += 1
+                output = InventoryFun(wkr_data["nr"], **job["kwargs"])
+                wkr_data["worker_jobs_completed"] += 1
                 nornir_data["res_queue"].put(
                     {"output": output, "identity": job["identity"]}
                 )
                 continue
             # execute nornir task
             task_fun = _get_or_import_task_fun(job["task_fun"], loader=loader)
             log.info(
                 "Nornir-proxy MAIN PID {} starting task '{}'".format(ppid, job["name"])
             )
             # lock connections and run the task
-            with nornir_data["connections_lock"]:
+            with wkr_data["connections_lock"]:
                 output = run(
                     task=task_fun,
                     loader=loader,
                     identity=job["identity"],
                     name=job["name"],
+                    nr=wkr_data["nr"],
+                    wkr_data=wkr_data,
                     **job["kwargs"],
                 )
-            nornir_data["stats"]["hosts_tasks_failed"] += len(
-                nornir_data["nr"].data.failed_hosts
+            wkr_data["worker_hosts_tasks_failed"] += len(
+                wkr_data["nr"].data.failed_hosts
             )
-            nornir_data["stats"]["jobs_completed"] += 1
+            wkr_data["worker_jobs_completed"] += 1
         except queue.Empty:
             continue
         except:
             tb = traceback.format_exc()
             output = "Nornir-proxy MAIN PID {} job failed: {}, error:\n'{}'".format(
                 ppid, job, tb
             )
             log.error(output)
-            nornir_data["stats"]["jobs_failed"] += 1
+            wkr_data["worker_jobs_failed"] += 1
         # submit job results in results queue
         nornir_data["res_queue"].put({"output": output, "identity": job["identity"]})
         del job, output
         # close connections to devices if proxy_always_alive is False
-        if nornir_data["proxy_always_alive"] is False:
+        if (
+            nornir_data["proxy_always_alive"] is False
+            or nornir_data["connections_idle_timeout"] == 0
+        ):
             try:
-                nornir_data["nr"].close_connections(on_good=True, on_failed=True)
+                wkr_data["nr"].close_connections(on_good=True, on_failed=True)
             except:
                 log.error(
                     "Nornir-proxy MAIN PID {} worker thread, Nornir close_connections error: {}".format(
                         ppid, traceback.format_exc()
                     )
                 )
 
@@ -1004,30 +1128,31 @@
         log.debug(
             "Nornir-proxy MAIN PID {} worker thread, donwloaded '{}' data from Master".format(
                 os.getpid(), key
             )
         )
 
 
-def _add_processors(kwargs, loader, identity):
+def _add_processors(kwargs, loader, identity, nr):
     """
     Helper function to exctrat processors arguments and add processors
     to Nornir.
 
     :param kwargs: (dict) dictionary with kwargs
     :param loader: (obj) SaltStack loader context
     :param identity: (dict) task identity dictionary for SaltEventProcessor
     :return: (obj) Nornir object
     """
     processors = []
 
     # get parameters
     tf = kwargs.pop("tf", None)  # to file
+    tf_skip_failed = kwargs.pop("tf_skip_failed", False)  # to file
     tests = kwargs.pop("tests", None)  # tests
-    remove_tasks = kwargs.pop("remove_tasks", True)  # testsand/or run_ttp
+    remove_tasks = kwargs.pop("remove_tasks", True)  # tests and/or run_ttp
     failed_only = kwargs.pop("failed_only", False)  # tests
     diff = kwargs.pop("diff", "")  # diff processor
     last = kwargs.pop("last", 1) if diff else None  # diff processor
     dp = kwargs.pop("dp", [])  # data processor
     xml_flake = kwargs.pop("xml_flake", "")  # data processor xml_flake function
     match = kwargs.pop("match", "")  # data processor match function
     before = kwargs.pop("before", 0)  # data processor match function
@@ -1113,18 +1238,19 @@
     if tf and isinstance(tf, str):
         processors.append(
             ToFileProcessor(
                 tf=tf,
                 base_url=nornir_data["files_base_path"],
                 index=nornir_data["stats"]["proxy_minion_id"],
                 max_files=nornir_data["files_max_count"],
+                skip_failed=tf_skip_failed,
             )
         )
 
-    return nornir_data["nr"].with_processors(processors)
+    return nr.with_processors(processors)
 
 
 def _cache_task_results_to_host_data(hosts, results, cache_key):
     """
     Function to save task results to host data under cache key.
 
     :param hosts: (obj) Nornir object
@@ -1135,37 +1261,46 @@
     cache_key = cache_key if isinstance(cache_key, str) else "hcache"
     log.debug(
         "salt-nornir:hcache saving results in hosts data under '{}' key".format(
             cache_key
         )
     )
 
-    # iterate over hosts and save results to data cache
-    for host_name, host_object in hosts.inventory.hosts.items():
-        # add metadata on cache keys so that can clean them up
-        host_object.data.setdefault("_hcache_keys_", [])
-        if cache_key not in host_object.data["_hcache_keys_"]:
-            host_object.data["_hcache_keys_"].append(cache_key)
-        # cache results
-        host_object.data.setdefault(cache_key, {})
-        # dictionary results should be keyed by host name
-        if isinstance(results, dict):
-            host_object.data[cache_key].update(results.get(host_name, {}))
-        # save string results as is
-        elif isinstance(results, str):
-            host_object.data[cache_key] = results
-        # convert list results back to dictionary keyd by task name
-        elif isinstance(results, list):
-            host_object.data[cache_key].update(
-                {i["name"]: i["result"] for i in results if i["host"] == host_name}
-            )
-        else:
-            log.error(
-                "salt-nornir:hcache unsupported results type '{}'".format(type(results))
-            )
+    # form a list of hosts to add hcache to
+    hosts_to_cache = list(hosts.inventory.hosts.keys())
+
+    # iteare over Nornir instances and cache results to hosts
+    for nr in nornir_data["nrs"]:
+        # iterate over hosts and save results to data cache
+        for host_name, host_object in nr["nr"].inventory.hosts.items():
+            if host_name not in hosts_to_cache:
+                continue
+            # add metadata on cache keys so that can clean them up
+            host_object.data.setdefault("_hcache_keys_", [])
+            if cache_key not in host_object.data["_hcache_keys_"]:
+                host_object.data["_hcache_keys_"].append(cache_key)
+            # cache results
+            host_object.data.setdefault(cache_key, {})
+            # dictionary results should be keyed by host name
+            if isinstance(results, dict):
+                host_object.data[cache_key].update(results.get(host_name, {}))
+            # save string results as is
+            elif isinstance(results, str):
+                host_object.data[cache_key] = results
+            # convert list results back to dictionary keyd by task name
+            elif isinstance(results, list):
+                host_object.data[cache_key].update(
+                    {i["name"]: i["result"] for i in results if i["host"] == host_name}
+                )
+            else:
+                log.error(
+                    "salt-nornir:hcache unsupported results type '{}'".format(
+                        type(results)
+                    )
+                )
 
     log.debug(
         "salt-nornir:hcache saved results in hosts data under '{}' key".format(
             cache_key
         )
     )
 
@@ -1182,50 +1317,49 @@
     log.debug(
         "salt-nornir:dcache saving results in defaults data under '{}' key".format(
             cache_key
         )
     )
 
     # add metadata about cache keys so that can clean them up later on
-    nornir_data["nr"].inventory.defaults.data.setdefault("_dcache_keys_", [])
-    if cache_key not in nornir_data["nr"].inventory.defaults.data["_dcache_keys_"]:
-        nornir_data["nr"].inventory.defaults.data["_dcache_keys_"].append(cache_key)
+    for nr in nornir_data["nrs"]:
+        nr["nr"].inventory.defaults.data.setdefault("_dcache_keys_", [])
+        if cache_key not in nr["nr"].inventory.defaults.data["_dcache_keys_"]:
+            nr["nr"].inventory.defaults.data["_dcache_keys_"].append(cache_key)
 
-    # cache results
-    nornir_data["nr"].inventory.defaults.data[cache_key] = results
+        # cache results
+        nr["nr"].inventory.defaults.data[cache_key] = results
     log.debug(
         "salt-nornir:dcache saved results in defaults data under '{}' key".format(
             cache_key
         )
     )
 
 
-def _clear_dcache(**kwargs):
+def _clear_dcache(nr, cache_keys=None):
     """
     Function to clear task results cache from defaults data.
 
     :param cache_keys: (str) list of key names to remove
+    :param nr: (obj) Nornir Instance to clear dcache for
     """
     result = {}
 
     # get keys to clear
-    cache_keys = kwargs.get("cache_keys", None)
     if cache_keys is None:
         # need to itearete over a copy of the keys - list() makes a copy
-        cache_keys = list(
-            nornir_data["nr"].inventory.defaults.data.get("_dcache_keys_", [])
-        )
+        cache_keys = list(nr.inventory.defaults.data.get("_dcache_keys_", []))
 
     # iterate over given cache keys and clean them up from data
     for key in cache_keys:
-        if key in nornir_data["nr"].inventory.defaults.data and key in nornir_data[
-            "nr"
-        ].inventory.defaults.data.get("_dcache_keys_", []):
-            nornir_data["nr"].inventory.defaults.data.pop(key)
-            nornir_data["nr"].inventory.defaults.data["_dcache_keys_"].remove(key)
+        if key in nr.inventory.defaults.data and key in nr.inventory.defaults.data.get(
+            "_dcache_keys_", []
+        ):
+            nr.inventory.defaults.data.pop(key)
+            nr.inventory.defaults.data["_dcache_keys_"].remove(key)
             result[key] = True
         else:
             result[key] = False
 
     return result
 
 
@@ -1238,24 +1372,37 @@
     from master and calls ``init`` function to reinstantiate Nornir object,
     worker&watchod threads and queus.
 
     It takes about a minute to finish refresh process.
 
     :param loader_: (obj) ``__salt__.loader`` object instance for ``init``
     """
-    log.info("Nornir-proxy refreshing!")
+    log.info("Nornir-proxy MAIN PID {}, refreshing".format(os.getpid()))
     if shutdown():
         # refresh all modules
         __salt__["saltutil.sync_all"]()
-        # refresh im memory pillar
+        # refresh in memory pillar
         __salt__["saltutil.refresh_pillar"]()
-        # get latest pillar data
+        # get latest pillar data from master
         __opts__["pillar"] = __salt__["pillar.items"]()
+        __opts__["proxy"] = __opts__["pillar"]["proxy"]
+        log.debug(
+            "Nornir-proxy MAIN PID {}, refreshing, new proxy data: {}".format(
+                os.getpid(), __opts__["proxy"]
+            )
+        )
+        log.debug(
+            "Nornir-proxy MAIN PID {}, refreshing, new pillar data: {}".format(
+                os.getpid(), __opts__["pillar"]
+            )
+        )
         # re-init proxy module
         init(__opts__, loader_)
+        # refresh in memory pillar one more time for salt to ead updated data
+        __salt__["saltutil.refresh_pillar"]()
         log.info("Nornir-proxy MAIN PID {}, process refreshed!".format(os.getpid()))
         return True
     return False
 
 
 def _rm_tasks_data_from_hosts(hosts):
     """
@@ -1263,37 +1410,50 @@
 
     :param hosts: (obj) Nornir object
     """
     for host_name, host_object in hosts.inventory.hosts.items():
         _ = host_object.data.pop("__task__", None)
 
 
+def _update_worker_connections(hosts, wkr_data):
+    """
+    Helper function to update stats for worker's hosts connections.
+
+    :param hosts: (obj) Nornir Object filtered instance
+    :param wkr_data: (dict) worker data dictionary
+    """
+    for host_name in hosts.inventory.hosts:
+        wkr_data["worker_connections"].setdefault(host_name, {})
+        wkr_data["worker_connections"][host_name]["last_use_timestamp"] = time.time()
+
+
 # -----------------------------------------------------------------------------
 # callable functions
 # -----------------------------------------------------------------------------
 
 
 def list_hosts(**kwargs):
     """
     Return a list of hosts managed by this Nornir instance
 
     :param Fx: filters to filter hosts
     """
-    return InventoryFun(nornir_data["nr"], call="list_hosts", **kwargs)
+    return InventoryFun(nornir_data["nrs"][0]["nr"], call="list_hosts", **kwargs)
 
 
-def run(task, loader, identity, name, **kwargs):
+def run(task, loader, identity, name, nr, wkr_data, **kwargs):
     """
     Function for worker Thread to run Nornir tasks.
 
     :param task: (obj) callable task function
     :param loader: (obj) ``__salt__.loader`` object instance
     :param identity: (dict) Task results queue identity for SaltEventProcessor
     :param kwargs: (dict) passed to ``task.run`` after extracting CLI arguments
     :param name: (str) Nornir task name to run
+    :param nr: (obj) Worker instance Nornir object
     """
     # extract attributes
     add_details = kwargs.pop("add_details", False)  # ResultSerializer
     to_dict = kwargs.pop("to_dict", True)  # ResultSerializer
     table = kwargs.pop("table", {})  # tabulate
     headers = kwargs.pop("headers", "keys")  # tabulate
     headers_exclude = kwargs.pop("headers_exclude", [])  # tabulate
@@ -1305,25 +1465,27 @@
         "render", ["config", "data", "filter", "filter_", "filters", "filename"]
     )  # render data
     event_failed = kwargs.pop("event_failed", False)  # events
     hcache = kwargs.pop("hcache", False)  # cache task results
     dcache = kwargs.pop("dcache", False)  # cache task results
 
     # set dry_run argument
-    nornir_data["nr"].data.dry_run = kwargs.get("dry_run", False)
+    nr.data.dry_run = kwargs.get("dry_run", False)
 
     # reset failed hosts if any
-    nornir_data["nr"].data.reset_failed_hosts()
+    nr.data.reset_failed_hosts()
 
     # download files
     if download:
         _download_files(download, kwargs, loader=loader)
 
     # add processors
-    nr_with_processors = _add_processors(kwargs, loader=loader, identity=identity)
+    nr_with_processors = _add_processors(
+        kwargs, loader=loader, identity=identity, nr=nr
+    )
 
     # Filter hosts to run tasks for
     hosts, has_filter = FFun(
         nr_with_processors, kwargs=kwargs, check_if_has_filter=True
     )
 
     # check if nornir_filter_required is True but no filter
@@ -1334,14 +1496,17 @@
 
     # download and render files
     if render:
         _download_and_render_files(
             hosts, render, kwargs, ignore_keys=download, loader=loader
         )
 
+    # update hosts connections ages
+    _update_worker_connections(hosts, wkr_data)
+
     # run tasks
     result = hosts.run(
         task, name=name, **{k: v for k, v in kwargs.items() if not k.startswith("_")}
     )
 
     # post clean-up - remove tasks rendered data from hosts inventory
     if render:
@@ -1392,18 +1557,87 @@
     :param task_fun: (str) name of nornir task function/plugin to import and run
     :param kwargs: (dict) any arguments to submit to Nornir task ``**kwargs``
     :param identity: (dict) dictionary of uuid4, jid, funtion_name keys
 
     ``identity`` parameter used to identify job results in results queue and
     must be unique for each submitted job.
     """
-    # add new job in jobs queue
-    nornir_data["jobs_queue"].put(
-        {"task_fun": task_fun, "kwargs": kwargs, "identity": identity, "name": task_fun}
-    )
+    # broadcast job to all nornir workers
+    if kwargs.get("worker") == "all":
+        _ = kwargs.pop("worker")
+        identities = []
+        results = []
+        # add jobs to the queue for each worker
+        for nr in nornir_data["nrs"]:
+            # make sure each worker receives its own copy of identity and kwargs
+            job_identity = copy.deepcopy(identity)
+            job_kwargs = copy.deepcopy(kwargs)
+            job_identity["worker"] = nr["worker_id"]
+            identities.append(job_identity)
+            nr["worker_jobs_queue"].put(
+                {
+                    "task_fun": task_fun,
+                    "kwargs": job_kwargs,
+                    "identity": job_identity,
+                    "name": task_fun,
+                }
+            )
+        # wait for jobs to complete and return results
+        start_time = time.time()
+        while (time.time() - start_time) < nornir_data["job_wait_timeout"]:
+            time.sleep(0.1)
+            try:
+                res = nornir_data["res_queue"].get(block=True, timeout=0.1)
+                if res["identity"] in identities:
+                    results.append(res)
+                else:
+                    nornir_data["res_queue"].put(res)
+            except queue.Empty:
+                continue
+            # check if collected results from all workers
+            if len(results) == nornir_data["nornir_workers"]:
+                break
+        else:
+            raise TimeoutError(
+                "Nornir-proxy MAIN PID {}, identities '{}', {}s job_wait_timeout expired.".format(
+                    os.getpid(), identities, nornir_data["job_wait_timeout"]
+                )
+            )
+        return {
+            "nornir-worker-{}".format(r["identity"]["worker"]): r["output"]
+            for r in results
+        }
+    # submit job to certain worker's queue only
+    elif kwargs.get("worker"):
+        if kwargs["worker"] not in list(range(1, len(nornir_data["nrs"]) + 1)):
+            return "Error: Non existing worker '{}'; worker IDs 1 - {}".format(
+                kwargs["worker"], len(nornir_data["nrs"])
+            )
+        nr = nornir_data["nrs"][kwargs.pop("worker") - 1]
+        identity["worker"] = nr["worker_id"]
+        # add job to the worker queue
+        nr["worker_jobs_queue"].put(
+            {
+                "task_fun": task_fun,
+                "kwargs": kwargs,
+                "identity": identity,
+                "name": task_fun,
+            }
+        )
+    # submit job to shared queue for one of the workers to execute
+    else:
+        nornir_data["jobs_queue"].put(
+            {
+                "task_fun": task_fun,
+                "kwargs": kwargs,
+                "identity": identity,
+                "name": task_fun,
+            }
+        )
+
     # wait for job to complete and return results
     start_time = time.time()
     while (time.time() - start_time) < nornir_data["job_wait_timeout"]:
         time.sleep(0.1)
         try:
             res = nornir_data["res_queue"].get(block=True, timeout=0.1)
             if res["identity"] == identity:
@@ -1450,21 +1684,14 @@
     * ``watchdog_child_processes_killed`` - int, number of stale child processes killed by watchdog
     * ``watchdog_dead_connections_cleaned`` - int, number of stale hosts' connections cleaned by watchdog
     * ``child_processes_count`` - int, number of child processes currently running
     * ``main_process_fd_count`` - int, number of file descriptors in use by main proxy minion process
     * ``main_process_fd_limit`` - int, fd count limit imposed by Operating System for minion process
     """
     stat = args[0] if args else kwargs.get("stat", None)
-    # get approximate queue sizes
-    try:
-        jobs_job_queue_size = nornir_data["jobs_queue"].qsize()
-        jobs_res_queue_size = nornir_data["res_queue"].qsize()
-    except:
-        jobs_job_queue_size = -1
-        jobs_res_queue_size = -1
     # get File Descriptors limit and usage
     try:
         if HAS_RESOURCE_LIB:
             fd_count = len(os.listdir("/proc/{}/fd/".format(os.getpid())))
             fd_limit = resource.getrlimit(resource.RLIMIT_NOFILE)[0]
     except:
         fd_count = -1
@@ -1472,26 +1699,37 @@
     # update stats
     nornir_data["stats"].update(
         {
             "main_process_ram_usage_mbyte": minion_process.memory_info().rss / 1024000,
             "main_process_fd_count": fd_count,
             "main_process_fd_limit": fd_limit,
             "timestamp": time.ctime(),
-            "jobs_job_queue_size": jobs_job_queue_size,
-            "jobs_res_queue_size": jobs_res_queue_size,
+            "jobs_job_queue_size": nornir_data["jobs_queue"].qsize(),
+            "jobs_res_queue_size": nornir_data["res_queue"].qsize(),
             "child_processes_count": len(multiprocessing.active_children()),
             "hosts_connections_active": sum(
                 [
                     len(host.connections)
-                    for host in nornir_data["nr"].inventory.hosts.values()
+                    for nr in nornir_data["nrs"]
+                    for host in nr["nr"].inventory.hosts.values()
                 ]
             ),
+            "hosts_connections_idle_timeout": nornir_data["connections_idle_timeout"],
             "main_process_uptime_seconds": round(
                 time.time() - nornir_data["stats"]["main_process_start_time"], 3
             ),
+            "nornir_workers": len(nornir_data["nrs"]),
+            "jobs_started": sum([w["worker_jobs_started"] for w in nornir_data["nrs"]]),
+            "jobs_completed": sum(
+                [w["worker_jobs_completed"] for w in nornir_data["nrs"]]
+            ),
+            "jobs_failed": sum([w["worker_jobs_failed"] for w in nornir_data["nrs"]]),
+            "hosts_tasks_failed": sum(
+                [w["worker_hosts_tasks_failed"] for w in nornir_data["nrs"]]
+            ),
         }
     )
     # check if need to return single stat
     if isinstance(stat, str):
         try:
             return {stat: nornir_data["stats"][stat]}
         except KeyError:
@@ -1597,7 +1835,89 @@
         if p.pid == os.getpid():
             continue
         os.kill(p.pid, signal.SIGKILL)
     # kill main process
     os.kill(nornir_data["stats"]["main_process_pid"], signal.SIGKILL)
     # kill itself if still can
     os.kill(os.getpid(), signal.SIGKILL)
+
+
+def workers_utils(call):
+    """
+    Function to retrieve operational data for Nornir Worker instances
+
+    :param call: (str) utility to invoke
+
+    Supported calls:
+
+    * ``stats`` - return worker statistics keyed by worker id with these parameters:
+
+       * ``is_busy`` - boolean, indicates if worker doing the work
+       * ``worker_jobs_completed`` - counter of completed jobs
+       * ``worker_jobs_failed`` - counter of completely failed jobs
+       * ``worker_connections`` - hosts' connections info
+       * ``worker_jobs_queue`` - size of the worker specific jobs queue
+       * ``worker_hosts_tasks_failed`` - counter of overall host failed tasks
+       * ``worker_jobs_started`` - counter of started jobs
+
+    """
+    supported_calls = ["stats"]
+    if call == "stats":
+        ret = {}
+        for w in nornir_data["nrs"]:
+            # calculate connections age
+            worker_connections = {
+                host_name: {
+                    "last_use_timestamp": conn_data["last_use_timestamp"],
+                    "age": int(time.time() - conn_data["last_use_timestamp"]),
+                }
+                for host_name, conn_data in w["worker_connections"].items()
+            }
+            # form workers stats
+            ret["nornir-worker-{}".format(w["worker_id"])] = {
+                "is_busy": w["is_busy"].is_set(),
+                "worker_jobs_completed": w["worker_jobs_completed"],
+                "worker_jobs_failed": w["worker_jobs_failed"],
+                "worker_connections": worker_connections,
+                "worker_jobs_queue": w["worker_jobs_queue"].qsize(),
+                "worker_hosts_tasks_failed": w["worker_hosts_tasks_failed"],
+                "worker_jobs_started": w["worker_jobs_started"],
+            }
+        return ret
+    else:
+        raise CommandExecutionError(
+            "Nornir-proxy workers_utils unsupported call - '{}', supported - '{}'".format(
+                call, ", ".join(supported_calls)
+            )
+        )
+
+
+def queues_utils(call):
+    """
+    Function to retrieve operational data for job queues
+
+    :param call: (str) utility to invoke - ``results_queue_dump``
+
+    Suppoted calls:
+
+    * ``results_queue_dump`` - drain items from result queue and return their content,
+        put items copies back into the queue afterwards
+    """
+    supported_calls = ["results_queue_dump"]
+    if call == "results_queue_dump":
+        ret = []
+        # drain items from results queue
+        while True:
+            try:
+                ret.append(nornir_data["res_queue"].get(block=True, timeout=0.5))
+            except queue.Empty:
+                break
+        # put drained items copies back into the queue
+        for i in ret:
+            nornir_data["res_queue"].put(copy.deepcopy(i))
+        return ret
+    else:
+        raise CommandExecutionError(
+            "Nornir-proxy queues_utils unsupported call - '{}', supported - '{}'".format(
+                call, ", ".join(supported_calls)
+            )
+        )
```

### Comparing `salt_nornir-0.8.0/salt_nornir/runners/nornir_proxy_runner_module.py` & `salt_nornir-0.9.0/salt_nornir/runners/nornir_proxy_runner_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,16 @@
         )
     # stop eventloop thread
     if show_progress:
         stop_signal.set()
         events_thread.join(timeout=5)
 
     # kill local client instance
-    client.destroy()
+    if hasattr(client, "destroy"):
+        client.destroy()
 
     return ret
 
 
 # -----------------------------------------------------------------------------
 # callable module function
 # -----------------------------------------------------------------------------
```

### Comparing `salt_nornir-0.8.0/salt_nornir/states/nornir_proxy_state_module.py` & `salt_nornir-0.9.0/salt_nornir/states/nornir_proxy_state_module.py`

 * *Files identical despite different names*

### Comparing `salt_nornir-0.8.0/salt_nornir.egg-info/PKG-INFO` & `salt_nornir-0.9.0/salt_nornir.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-nornir
-Version: 0.8.0
+Version: 0.9.0
 Summary: SALTSTACK Nornir Modules
 Home-page: https://github.com/dmulyalin/salt-nornir
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 License: UNKNOWN
 Description: [![Downloads](https://pepy.tech/badge/salt-nornir)](https://pepy.tech/project/salt-nornir)
         [![PyPI versions](https://img.shields.io/pypi/pyversions/salt-nornir.svg)](https://pypi.python.org/pypi/salt-nornir/)
@@ -33,15 +33,15 @@
         
         Nornir Proxy acts as a bridge between SaltStack and a wide set of network automation libraries.
         
         # Advantages
         
         Some notable benefits:
         
-        - Well tested - overall 382 tests combined as of release 0.8.0
+        - Well tested - overall 426 tests for `salt-nornir` and `nornir-salt` packages combined as of release 0.9.0
         - Brings together SaltStack and a wealth of open-source libraries - Nornir, Netmiko, NAPALM, Scrapli, Scrapli-Netconf, Ncclient, Genie&PyATS (free, not open-source), PyGNMI, NTC-Templates, TTP, Jmespath, lxml, xmltodict, requests
         - Capable of addressing overwhelming set of use cases from simple data retrieval and parsing to infrastructure provisioning, testing, orchestration and self-healing
         - Python is a first class citizen, need something special - write your own plugins, modules, scripts, codify your work flows
         - Integrate anything with anything, all you can do via CLI you can do via SaltStack and Nornir Python API or SaltStack REST API
         
         # Communication and discussion
```

### Comparing `salt_nornir-0.8.0/salt_nornir.egg-info/SOURCES.txt` & `salt_nornir-0.9.0/salt_nornir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salt_nornir-0.8.0/setup.py` & `salt_nornir-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 __author__ = "Denis Mulyalin <d.mulyalin@gmail.com>"
 
 setup(
     name="salt_nornir",
-    version="0.8.0",
+    version="0.9.0",
     author="Denis Mulyalin",
     author_email="d.mulyalin@gmail.com",
     description="SALTSTACK Nornir Modules",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dmulyalin/salt-nornir",
     packages=find_packages(),
@@ -28,16 +28,16 @@
     python_requires=">=3.6",
     install_requires=[
         "netmiko==3.*",
         "nornir==3.*",
         "napalm==3.*",
         "nornir_netmiko==0.*",
         "nornir_napalm==0.*",
-        "nornir_salt==0.8.*",
-        "psutil==5.8.*",
+        "nornir_salt==0.9.*",
+        "psutil==5.*",
     ],
     entry_points="""
     [salt.loader]
     module_dirs=salt_nornir.loader:module_dirs
     proxy_dirs=salt_nornir.loader:proxy_dirs
     states_dirs=salt_nornir.loader:states_dirs
     runner_dirs=salt_nornir.loader:runner_dirs
```

