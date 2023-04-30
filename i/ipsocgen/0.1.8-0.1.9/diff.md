# Comparing `tmp/ipsocgen-0.1.8.tar.gz` & `tmp/ipsocgen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipsocgen-0.1.8.tar", last modified: Sun Mar 19 15:43:55 2023, max compression
+gzip compressed data, was "ipsocgen-0.1.9.tar", last modified: Sat Apr  8 11:17:38 2023, max compression
```

## Comparing `ipsocgen-0.1.8.tar` & `ipsocgen-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:43:55.607819 ipsocgen-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-19 15:43:55.607819 ipsocgen-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:43:55.603819 ipsocgen-0.1.8/ipsocgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:43:55.607819 ipsocgen-0.1.8/ipsocgen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17779 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:43:55.607819 ipsocgen-0.1.8/ipsocgen/common/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/schemas/schema_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/schemas/schema_master.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/schemas/schema_slave.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:43:55.607819 ipsocgen-0.1.8/ipsocgen/common/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_crossbar.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_custom_master.txt
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_custom_slave.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_dma.txt
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_irq_ctrl.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_mem_ram.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_mem_rom.txt
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_rst_ctrl.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_timer.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/axi4_uart.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/clk_basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/clk_pll_xilinx.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/clk_simple.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/module_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/module_instance.txt
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/nox_wrapper.txt
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/ravenoc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/templates/rst_simple.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/common/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/ipsocgen/ipsocgen_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:43:55.603819 ipsocgen-0.1.8/ipsocgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-19 15:43:55.000000 ipsocgen-0.1.8/ipsocgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-19 15:43:55.000000 ipsocgen-0.1.8/ipsocgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 15:43:55.000000 ipsocgen-0.1.8/ipsocgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-19 15:43:55.000000 ipsocgen-0.1.8/ipsocgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-19 15:43:55.000000 ipsocgen-0.1.8/ipsocgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-19 15:43:55.000000 ipsocgen-0.1.8/ipsocgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 15:43:55.607819 ipsocgen-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-19 15:43:46.000000 ipsocgen-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:17:38.262438 ipsocgen-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-08 11:17:38.262438 ipsocgen-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:17:38.258438 ipsocgen-0.1.9/ipsocgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:17:38.258438 ipsocgen-0.1.9/ipsocgen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:17:38.258438 ipsocgen-0.1.9/ipsocgen/common/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/schemas/schema_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/schemas/schema_master.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/schemas/schema_slave.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:17:38.262438 ipsocgen-0.1.9/ipsocgen/common/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_crossbar.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_custom_master.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_custom_slave.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_dma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_irq_ctrl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_mem_ram.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_mem_rom.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_rst_ctrl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_timer.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/axi4_uart.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/clk_basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/clk_pll_xilinx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/clk_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/module_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/module_instance.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/nox_wrapper.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/ravenoc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/templates/rst_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/common/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/ipsocgen/ipsocgen_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:17:38.258438 ipsocgen-0.1.9/ipsocgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-08 11:17:38.000000 ipsocgen-0.1.9/ipsocgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-08 11:17:38.000000 ipsocgen-0.1.9/ipsocgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 11:17:38.000000 ipsocgen-0.1.9/ipsocgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-08 11:17:38.000000 ipsocgen-0.1.9/ipsocgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-08 11:17:38.000000 ipsocgen-0.1.9/ipsocgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 11:17:38.000000 ipsocgen-0.1.9/ipsocgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 11:17:38.262438 ipsocgen-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-08 11:17:28.000000 ipsocgen-0.1.9/setup.py
```

### Comparing `ipsocgen-0.1.8/LICENSE` & `ipsocgen-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/PKG-INFO` & `ipsocgen-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipsocgen
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generic SoC builder in HDL
 Home-page: https://github.com/aignacio/ipsocgen
 Author: aignacio (Anderson Ignacio)
 Author-email: <anderson@aignacio.com>
 Keywords: soc,mpsoc,hdl,verilog,systemverilog,builder
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ipsocgen-0.1.8/ipsocgen/common/constants.py` & `ipsocgen-0.1.9/ipsocgen/common/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # File              : constants.py
 # License           : MIT license <Check LICENSE>
 # Author            : Anderson Ignacio da Silva (aignacio) <anderson@aignacio.com>
 # Date              : 06.02.2023
-# Last Modified Date: 17.03.2023
+# Last Modified Date: 08.04.2023
 import logging
 import os
 import abc
 from tabulate import tabulate
 from jinja2 import Environment, FileSystemLoader
-import ipsocgen
+
+__IPSOCGEN_VERSION__ = '0.1.9'
 
 class options:
     TYPES               = ['soc', 'mpsoc']
-    sch_cfg             = os.path.join(os.path.dirname(ipsocgen.__file__),'common/schemas/schema_config.yaml')
-    sch_master          = os.path.join(os.path.dirname(ipsocgen.__file__),'common/schemas/schema_master.yaml')
-    sch_slave           = os.path.join(os.path.dirname(ipsocgen.__file__),'common/schemas/schema_slave.yaml')
-    tmpl_folder         = os.path.join(os.path.dirname(ipsocgen.__file__),'common/templates')
+    sch_cfg             = os.path.join(os.path.dirname(__file__),'schemas/schema_config.yaml')
+    sch_master          = os.path.join(os.path.dirname(__file__),'schemas/schema_master.yaml')
+    sch_slave           = os.path.join(os.path.dirname(__file__),'schemas/schema_slave.yaml')
+    tmpl_folder         = os.path.join(os.path.dirname(__file__),'templates')
     tmpl_axi4_cross_bar = 'axi4_crossbar.txt'
     tmpl_nox            = 'nox_wrapper.txt'
     tmpl_axi4_mem_ram   = 'axi4_mem_ram.txt'
     tmpl_axi4_mem_rom   = 'axi4_mem_rom.txt'
     tmpl_axi4_dma       = 'axi4_dma.txt'
     tmpl_axi4_uart      = 'axi4_uart.txt'
     tmpl_axi4_irq       = 'axi4_irq_ctrl.txt'
```

### Comparing `ipsocgen-0.1.8/ipsocgen/common/generate.py` & `ipsocgen-0.1.9/ipsocgen/common/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # File              : generate.py
 # License           : MIT license <Check LICENSE>
 # Author            : Anderson Ignacio da Silva (aignacio) <anderson@aignacio.com>
 # Date              : 20.02.2023
-# Last Modified Date: 17.03.2023
+# Last Modified Date: 08.04.2023
 import logging
 import os
 import sys
 import shutil
-from ipsocgen.common.constants import options,base_module
-from ipsocgen.common.modules import *
+from common.constants import options,base_module
+from common.modules import *
 from tabulate import tabulate
 from jinja2 import Environment, FileSystemLoader
 
 def mpsoc_gen(mpsoc, mpsoc_name, desc, output, mmap):
     mpsoc_hdl_obj = []
 
     # Get all SoC IOs
@@ -129,49 +129,87 @@
     # Get the RTL modules
     for obj in hdl_obj:
         global_rtl += obj.get_hdl()
 
     global_rtl += '\nendmodule'
 
     _gen_design_files(soc_name, global_rtl, hdl_obj, output)
+    _gen_header_files(soc_name, bus, hdl_obj, output)
 
     soc_data = {}
     soc_data['name'] = soc_name
     soc_data['input'] = in_s
     soc_data['output'] = out_s
     return soc_data
 
 def _gen_design_files(soc_name, global_rtl, hdl_obj, out_dir):
     types = set()
     # Creates a set without repeated acc types
     for obj in hdl_obj:
         types.add(obj.get_acc_type())
 
     out_rtl = os.path.join(out_dir,'rtl')
-    out_ips = os.path.join(out_dir,'ips')
 
     if not os.path.exists(out_dir):
         os.mkdir(out_dir)
         logging.debug('Creating output directory: '+str(out_dir))
     if not os.path.exists(out_rtl):
         os.mkdir(out_rtl)
         logging.debug('Creating RTL directory: '+str(out_rtl))
-    if not os.path.exists(out_ips):
-        os.mkdir(out_ips)
-        logging.debug('Creating IPs directory: '+str(out_ips))
-
-        # logging.warning('Overwriting previous '+str(out_dir)+' directory')
-        # shutil.rmtree(out_dir)
-        # os.mkdir(out_dir)
 
     rtl_out = os.path.join(out_rtl,soc_name+'.sv')
     soc_rtl = open(rtl_out, "w")
     soc_rtl.write(global_rtl)
     soc_rtl.close()
 
+def _gen_header_files(soc_name, bus, hdl_obj, out_dir):
+    types = set()
+    # Creates a set without repeated acc types
+    for obj in hdl_obj:
+        types.add(obj.get_acc_type())
+
+    out_sw = os.path.join(out_dir,'sw')
+
+    if not os.path.exists(out_dir):
+        os.mkdir(out_dir)
+        logging.debug('Creating output directory: '+str(out_dir))
+    if not os.path.exists(out_sw):
+        os.mkdir(out_sw)
+        logging.debug('Creating SW directory: '+str(out_sw))
+
+    header_out = os.path.join(out_sw, soc_name+'.h')
+    header_file = open(header_out, "w")
+    header_file.write('#ifndef '+soc_name.upper()+'_H')
+    header_file.write('\n#define '+soc_name.upper()+'_H')
+    header_file.write('\n\n')
+    header_file.write('// AUTO-GENERATED header file through IPSoCGen')
+    header_file.write('\n// '+datetime.now().strftime('%d/%m/%Y %H:%M:%S'))
+    header_file.write('\n\n')
+    header_file.write(tabulate(bus.table_masters_c, tablefmt="plain"))
+    header_file.write('\n\n')
+    header_file.write(tabulate(bus.table_slaves_c, tablefmt="plain"))
+    header_file.write('\n\n')
+
+    table = []
+    for slave in range(len(bus.description)):
+        slave_info = _fmt_base_addr(bus.description[slave], bus.base_addr_h[slave])
+        table.append(['#define', slave_info['desc'], '0x'+slave_info['baddr']])
+    header_file.write(tabulate(table, ['//', 'SLAVE', 'BASE ADDRESS'], tablefmt='plain'))
+    header_file.write('\n')
+
+    header_file.write('\n#endif')
+    header_file.close()
+
+def _fmt_base_addr(description, base_address):
+    info  = {}
+    desc  = str(description).replace(' ','_')+'_BASE_ADDR'
+    info['desc']  = desc.upper()
+    info['baddr'] = str(base_address)
+    return info
+
 def _soc_slaves(bus, soc, soc_cfg, dma_info):
     hdl_obj = []
     mmap = bus.get_mmap()
     for slave, slave_desc in soc['slaves'].items():
         if slave_desc['type'] == 'ram_mem':
             iram = Axi4MemRAM(slave_desc, soc_cfg, slave)
             hdl_obj.append(iram)
```

### Comparing `ipsocgen-0.1.8/ipsocgen/common/modules.py` & `ipsocgen-0.1.9/ipsocgen/common/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # File              : modules.py
 # License           : MIT license <Check LICENSE>
 # Author            : Anderson Ignacio da Silva (aignacio) <anderson@aignacio.com>
 # Date              : 06.02.2023
-# Last Modified Date: 17.03.2023
+# Last Modified Date: 08.04.2023
 import logging
 import os
 import sys
-from ipsocgen.common.constants import options,base_module
+from common.constants import options,base_module
 from tabulate import tabulate
 from jinja2 import Environment, FileSystemLoader
 from datetime import datetime
 
 class Axi4Bus(base_module):
     def __init__(self, cfg, mmap):
         super().__init__(cfg['bus_name'], 0, 0, options.tmpl_axi4_cross_bar)
@@ -135,15 +135,16 @@
     def print_axi4_cfg(self):
         print(tabulate(self.table_slaves, self.headers_slaves, tablefmt="double_outline"))
 
     def get_hdl(self):
         file_loader = FileSystemLoader(options.tmpl_folder)
         env = Environment(loader=file_loader)
         template = env.get_template(options.tmpl_axi4_cross_bar)
-        output =  tabulate(self.table_masters_c, tablefmt="plain")
+        output = '\n'
+        output +=  tabulate(self.table_masters_c, tablefmt="plain")
         output += '\n\n'
         output += tabulate(self.table_slaves_c, tablefmt="plain")
         output += template.render(axi4bus=self)
         # if logging.getLogger().isEnabledFor(logging.DEBUG):
             # print(output)
         return output
 
@@ -233,16 +234,16 @@
         self.txn_id_w     = soc_common['txn_id']
         self.slv_id       = slv_id
         self.desc         = cfg['desc']
         self.io_rx        = cfg['io_rx']
         self.io_tx        = cfg['io_tx']
         self.irq_uart_rx  = cfg['irq_uart_rx']
         self.signals.append('  logic '+self.irq_uart_rx+';')
-        self.signals.append('  logic '+self.io_tx+'; // IO Pin')
-        self.signals.append('  logic '+self.io_rx+'; // IO Pin')
+        # self.signals.append('  logic '+self.io_tx+'; // IO Pin')
+        # self.signals.append('  logic '+self.io_rx+'; // IO Pin')
         self.io['in'].append(['logic', cfg['io_rx']])
         self.io['out'].append(['logic', cfg['io_tx']])
         self.acc_type     = 'acc_uart'
 
 class Axi4Irq(base_module):
     def __init__(self, cfg, soc_common, slv_id, base_addr):
         super().__init__(cfg['name'], soc_common['clk'], soc_common['rst'], options.tmpl_axi4_irq)
@@ -294,15 +295,15 @@
         self.rst_def_addr    = '\'h'+hex(base_addr[cfg['rst_def_addr']])[2:]
         self.rst_pulse_width = cfg['rst_pulse_width']
         self.rst_addr_out    = cfg['rst_addr_out']
         self.bootloader_type = cfg['bootloader_type']
         self.io_bootloader   = cfg['io_bootloader']
         self.io_in_rst       = cfg['io_in_rst']
         self.rst_in_type     = cfg['rst_in_type']
-        self.signals.append('  logic '+self.io_bootloader+'; // IO Pin')
+        # self.signals.append('  logic '+self.io_bootloader+'; // IO Pin')
         self.io['in'].append(['logic', cfg['io_bootloader']])
         self.io['in'].append(['logic', cfg['io_in_rst']])
         self.acc_type        = 'acc_rst'
 
 class Clock(base_module):
     def __init__(self, cfg):
         clk_cfg = cfg['clk']
@@ -312,14 +313,15 @@
             self.io_rst_pin    = clk_cfg['pll']['io_rst_pin']
             self.divclk_divide = clk_cfg['pll']['divclk_divide']
             self.clkfbout_mult = clk_cfg['pll']['clkfbout_mult']
             self.clkout_divide = clk_cfg['pll']['clkout_divide']
             self.clkin_period  = clk_cfg['pll']['clkin_period']
             self.io_clk_MHz    = clk_cfg['io_clk_MHz']
             self.clk_int       = clk_cfg['clk_int']
+            self.signals.append('  logic '+self.clk_int+';')
             self.io['in'].append(['logic', clk_cfg['io_clk_MHz']])
             self.io['in'].append(['logic', clk_cfg['pll']['io_rst_pin']])
         else:
             super().__init__(clk_cfg['name'], 0, 0, options.tmpl_clk)
             self.io_clk_MHz    = clk_cfg['io_clk_MHz']
             self.clk_int       = clk_cfg['clk_int']
             self.io['in'].append(['logic', clk_cfg['io_clk_MHz']])
@@ -347,14 +349,15 @@
             self.rst_int = rst_cfg['rst_int']
             self.io_in_rst = rst_cfg['io_in_rst']
             self.rst_in_type = rst_cfg['rst_in_type']
             self.io['in'].append(['logic', rst_cfg['io_in_rst']])
         else:
             super().__init__(rst_cfg['name'], 0, 0, options.tmpl_rst)
             self.io['in'].append(['logic', rst_cfg['io_in_rst']])
+            self.signals.append('  logic '+rst_cfg['rst_int']+';')
 
 class ModuleHeader(base_module):
     def __init__(self, type_cfg, name, desc, io_list, defines):
         super().__init__(0, 0, 0, options.tmpl_module_header)
         if type_cfg == 'soc':
             self.defines = defines
             self.name = name
```

### Comparing `ipsocgen-0.1.8/ipsocgen/common/schemas/schema_config.yaml` & `ipsocgen-0.1.9/ipsocgen/common/schemas/schema_config.yaml`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/ipsocgen/common/schemas/schema_slave.yaml` & `ipsocgen-0.1.9/ipsocgen/common/schemas/schema_slave.yaml`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/axi4_crossbar.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/axi4_crossbar.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
                         {{- axi4bus.b_addr_width }}'h{{ axi4bus.base_addr_h[base] -}}
                         {% endif %}
                         {%- endfor -%}
                       }),
     .M_ADDR_WIDTH     ({
                         {%- for addr in axi4bus.addr_width|reverse -%}
                         {% if addr %}
-                        {{- axi4bus.b_addr_width }}'h{{ axi4bus.addr_width[addr] }},
+                        {{- axi4bus.b_addr_width }}'d{{ axi4bus.addr_width[addr] }},
                         {% else %}
-                        {{- axi4bus.b_addr_width }}'h{{ axi4bus.addr_width[addr] -}}
+                        {{- axi4bus.b_addr_width }}'d{{ axi4bus.addr_width[addr] -}}
                         {% endif %}
                         {%- endfor -%}
                       })
   ) u_{{ axi4bus.bus_name }} (
     .clk              ({{ axi4bus.clk }}),
     .rst              ({{ axi4bus.rst }}),
     .*
```

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/axi4_dma.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/axi4_dma.txt`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/axi4_irq_ctrl.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/axi4_irq_ctrl.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-  logic irq_vector_mapping [31:0];
+  logic [31:0] irq_vector_mapping;
 
   assign irq_vector_mapping = '0; // Default assignment
 
   {%- for irq in tmpl.vec_mapping %}
   assign irq_vector_mapping[{{ loop.index0 }}] = {{ irq }};
   {%- endfor %}
```

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/axi4_mem_ram.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/axi4_mem_ram.txt`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/axi4_rst_ctrl.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/axi4_rst_ctrl.txt`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/clk_basic.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/clk_basic.txt`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/clk_pll_xilinx.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/clk_pll_xilinx.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,18 @@
   logic pll_locked;
   logic rst_pll;
   {% if tmpl.rst_in_type == 'act_l' %}
   assign rst_pll = ~{{ tmpl.io_rst_pin }};
   {% else %}
   assign rst_pll = {{ tmpl.io_rst_pin }};
   {% endif %}
+
+`ifdef SIMULATION
+  assign {{ tmpl.clk_int }} = {{ tmpl.io_clk_MHz }};
+`else
   //
   // PLLE2_BASE: Base Phase Locked Loop (PLL)
   //             7 Series
   PLLE2_ADV#(
     .BANDWIDTH           ("OPTIMIZED"),
     .COMPENSATION        ("ZHOLD"),
     .STARTUP_WAIT        ("FALSE"),
@@ -57,7 +61,8 @@
     .O (clk_feedback_out)
   );
 
   BUFG clk_out_buf(
     .I (clk_buff_out),
     .O ({{ tmpl.clk_int }})
   );
+`endif
```

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/module_header.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/module_header.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 /**
  * File              : {{ tmpl.name }}.sv
  * License           : MIT license <Check LICENSE>
  * Author            : IPSoCGen
  * Date              : {{ tmpl.date }}
  * Description       : {{ tmpl.desc }}
- * --------------------------------------------
- * ---- Do not edit, design auto-generated ----
- * --------------------------------------------
+ * -------------------------------------------
+ * -- Design AUTO-GENERATED using IPSoC Gen --
+ * -------------------------------------------
  **/
 {{ tmpl.defines }}
 module {{ tmpl.name }}
   {%- if tmpl.type == 'mpsoc' %}
   import amba_axi_pkg::*;
   import ravenoc_pkg::*;
+  {% else %}
+  import amba_axi_pkg::*;
   {%- endif %}
 (
   {% for io in tmpl.io_list -%}
   {% if loop.last%}
   {{- io -}}
   {% else %}
   {{- io }},
```

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/nox_wrapper.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/nox_wrapper.txt`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/ipsocgen/common/templates/ravenoc.txt` & `ipsocgen-0.1.9/ipsocgen/common/templates/ravenoc.txt`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/ipsocgen/common/validate.py` & `ipsocgen-0.1.9/ipsocgen/common/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import argparse
 import pathlib
 import sys
 import yaml
-from ipsocgen.common.constants import options, CustomFormatter
+from common.constants import options, CustomFormatter
 from cerberus import Validator
 
 def validate_config(args):
     try:
         cfg = yaml.safe_load(args['config'])
     except yaml.YAMLError as exc:
         logging.error('Error while parsing YAML file:')
```

### Comparing `ipsocgen-0.1.8/ipsocgen/ipsocgen_cli.py` & `ipsocgen-0.1.9/ipsocgen/ipsocgen_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # File              : ipsocgen_cli.py
 # License           : MIT license <Check LICENSE>
 # Author            : Anderson Ignacio da Silva (aignacio) <anderson@aignacio.com>
 # Date              : 06.02.2023
-# Last Modified Date: 19.03.2023
+# Last Modified Date: 08.04.2023
 import logging
 import argparse
 import pathlib
 import sys
 import yaml
 import pkg_resources
-from ipsocgen.common.constants import options, CustomFormatter
-from ipsocgen.common.validate import validate_config
-from ipsocgen.common.modules import *
-from ipsocgen.common.generate import *
+from common.constants import options, CustomFormatter
+from common.validate import validate_config
+from common.modules import *
+from common.generate import *
+from common.constants import __IPSOCGEN_VERSION__
 
 def _gen(cfg, output, mmap):
     if cfg['type'] == 'soc':
         soc_gen(cfg['soc_desc'], cfg['proj_name'], cfg['desc'], output, mmap)
     else:
         mpsoc_gen(cfg['mpsoc_desc'], cfg['proj_name'], cfg['desc'], output, mmap)
 
     return True
 
 def main():
-    version = pkg_resources.require("ipsocgen")[0].version
+    version = __IPSOCGEN_VERSION__
     parser = argparse.ArgumentParser(description='IP SoC Generator CLI v'+version)
 
     parser.add_argument('-c','--cfg',
                         nargs='?',
                         type=argparse.FileType('r'),
                         help='YAML file with the configuration of the MP/SoC')
```

### Comparing `ipsocgen-0.1.8/ipsocgen.egg-info/PKG-INFO` & `ipsocgen-0.1.9/ipsocgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipsocgen
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generic SoC builder in HDL
 Home-page: https://github.com/aignacio/ipsocgen
 Author: aignacio (Anderson Ignacio)
 Author-email: <anderson@aignacio.com>
 Keywords: soc,mpsoc,hdl,verilog,systemverilog,builder
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ipsocgen-0.1.8/ipsocgen.egg-info/SOURCES.txt` & `ipsocgen-0.1.9/ipsocgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipsocgen-0.1.8/setup.py` & `ipsocgen-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
+#from ipsocgen.common.constants import __IPSOCGEN_VERSION__
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
+#__IPSOCGEN_VERSION__
 DESCRIPTION = 'Generic SoC builder in HDL'
 LONG_DESCRIPTION = 'Build SoCs (System-on-Chip) and MPSoCs (Multi-Processor) through yaml configuration files.'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
@@ -22,18 +24,18 @@
     url='https://github.com/aignacio/ipsocgen',
     packages=find_packages(),
     package_data={
         '':['common/schemas/*.yaml', 'common/templates/*.txt']
     },
     include_package_data=True,
     install_requires=[
+        'tabulate',
         'argparse',
         'pyyaml',
         'cerberus',
-        'tabulate',
         'jinja2'
     ],
     keywords=['soc', 'mpsoc', 'hdl',  'verilog', 'systemverilog', 'builder'],
     entry_points = {
         'console_scripts': ['ipsocgen=ipsocgen.ipsocgen_cli:main'],
     },
     classifiers=[
```

