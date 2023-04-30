# Comparing `tmp/csle_system_identification-0.1.9.tar.gz` & `tmp/csle_system_identification-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_system_identification-0.1.9.tar", last modified: Tue Mar 21 08:09:42 2023, max compression
+gzip compressed data, was "csle_system_identification-0.2.0.tar", last modified: Sun Apr 30 12:36:48 2023, max compression
```

## Comparing `csle_system_identification-0.1.9.tar` & `csle_system_identification-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4235 2023-01-03 16:53:42.000000 csle_system_identification-0.1.9/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      686 2023-02-11 20:28:41.000000 csle_system_identification-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1340 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.377235 csle_system_identification-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.377235 csle_system_identification-0.1.9/src/csle_system_identification/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_system_identification-0.1.9/src/csle_system_identification/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.377235 csle_system_identification-0.1.9/src/csle_system_identification/base/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/base/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2074 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/base/base_system_identification_algorithm.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      688 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/empirical/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/empirical/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7135 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/empirical/empirical_algorithm.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12807 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/emulator.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/expectation_maximization/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/expectation_maximization/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7380 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/gp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/gp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     9700 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/gp/gp_regression_algorithm.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      555 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.381235 csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2159 2022-12-03 16:48:17.000000 csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/data_collection_job_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2212 2022-11-28 13:03:16.000000 csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/system_identification_job_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:42.377235 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1412 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:14.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      257 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       27 2023-03-21 08:09:42.000000 csle_system_identification-0.1.9/src/csle_system_identification.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4235 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      686 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1340 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.780593 csle_system_identification-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.780593 csle_system_identification-0.2.0/src/csle_system_identification/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_system_identification-0.2.0/src/csle_system_identification/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/src/csle_system_identification/base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2074 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/base/base_system_identification_algorithm.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/src/csle_system_identification/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      688 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/src/csle_system_identification/empirical/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/empirical/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7249 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/empirical/empirical_algorithm.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17108 2023-04-18 12:43:31.000000 csle_system_identification-0.2.0/src/csle_system_identification/emulator.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/src/csle_system_identification/expectation_maximization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/expectation_maximization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7494 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/src/csle_system_identification/gp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/gp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9801 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/gp/gp_regression_algorithm.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      555 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/src/csle_system_identification/job_controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/job_controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2159 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/job_controllers/data_collection_job_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2212 2023-03-28 14:03:22.000000 csle_system_identification-0.2.0/src/csle_system_identification/job_controllers/system_identification_job_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:48.784593 csle_system_identification-0.2.0/src/csle_system_identification.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-04-30 12:36:48.000000 csle_system_identification-0.2.0/src/csle_system_identification.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1412 2023-04-30 12:36:48.000000 csle_system_identification-0.2.0/src/csle_system_identification.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:36:48.000000 csle_system_identification-0.2.0/src/csle_system_identification.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:14.000000 csle_system_identification-0.2.0/src/csle_system_identification.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      257 2023-04-30 12:36:48.000000 csle_system_identification-0.2.0/src/csle_system_identification.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       27 2023-04-30 12:36:48.000000 csle_system_identification-0.2.0/src/csle_system_identification.egg-info/top_level.txt
```

### Comparing `csle_system_identification-0.1.9/PKG-INFO` & `csle_system_identification-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_system_identification
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.1.9/README.md` & `csle_system_identification-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.9/pyproject.toml` & `csle_system_identification-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.9/setup.cfg` & `csle_system_identification-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.1.9
-	csle-collector>=0.1.9
-	csle-attacker>=0.1.9
-	csle-defender>=0.1.9
+	csle-common>=0.2.0
+	csle-collector>=0.2.0
+	csle-attacker>=0.2.0
+	csle-defender>=0.2.0
 	gpytorch>=1.9.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
```

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/base/base_system_identification_algorithm.py` & `csle_system_identification-0.2.0/src/csle_system_identification/base/base_system_identification_algorithm.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/constants/constants.py` & `csle_system_identification-0.2.0/src/csle_system_identification/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/empirical/empirical_algorithm.py` & `csle_system_identification-0.2.0/src/csle_system_identification/empirical/empirical_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from csle_system_identification.base.base_system_identification_algorithm import BaseSystemIdentificationAlgorithm
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.system_identification.emulation_statistics import EmulationStatistics
 from csle_common.dao.system_identification.system_identification_config import SystemIdentificationConfig
 from csle_common.dao.system_identification.empirical_system_model import EmpiricalSystemModel
 from csle_common.dao.system_identification.empirical_conditional import EmpiricalConditional
 from csle_common.dao.jobs.system_identification_job_config import SystemIdentificationJobConfig
-import csle_system_identification.constants.constants as system_identification_constants
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.logging.log import Logger
+from csle_common.util.general_util import GeneralUtil
+import csle_system_identification.constants.constants as system_identification_constants
 
 
 class EmpiricalAlgorithm(BaseSystemIdentificationAlgorithm):
     """
     Class that implements the system identification procedure using empirical distributions
     """
 
@@ -46,15 +47,16 @@
         descr = f"System identification through empirical distributions, " \
                 f"emulation:{self.emulation_env_config.name}, statistic id: {self.emulation_statistics.id}"
         if self.system_identification_job is None:
             self.system_identification_job = SystemIdentificationJobConfig(
                 emulation_env_name=self.emulation_env_config.name,
                 emulation_statistics_id=self.emulation_statistics.id, pid=pid, progress_percentage=0,
                 log_file_path=Logger.__call__().get_log_file_path(), descr=descr, system_model=None,
-                system_identification_config=self.system_identification_config
+                system_identification_config=self.system_identification_config,
+                physical_host_ip=GeneralUtil.get_host_ip()
             )
             system_identification_job_id = MetastoreFacade.save_system_identification_job(
                 system_identification_job=self.system_identification_job)
             self.system_identification_job.id = system_identification_job_id
         else:
             self.system_identification_job.pid = pid
             self.system_identification_job.progress_percentage = 0
```

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/emulator.py` & `csle_system_identification-0.2.0/src/csle_system_identification/emulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Tuple, Optional
 import time
 import os
 import sys
 import numpy as np
+import csle_common.constants.constants as constants
 from csle_common.dao.emulation_config.emulation_env_state import EmulationEnvState
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.emulation_config.emulation_trace import EmulationTrace
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.util.env_dynamics_util import EnvDynamicsUtil
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.logging.log import Logger
@@ -16,14 +17,16 @@
 from csle_common.dao.jobs.data_collection_job_config import DataCollectionJobConfig
 from csle_common.dao.emulation_action.attacker.emulation_attacker_action import EmulationAttackerAction
 from csle_common.dao.emulation_action.defender.emulation_defender_action import EmulationDefenderAction
 from csle_common.dao.emulation_action.attacker.emulation_attacker_stopping_actions \
     import EmulationAttackerStoppingActions
 from csle_common.dao.emulation_action.defender.emulation_defender_stopping_actions \
     import EmulationDefenderStoppingActions
+from csle_common.util.general_util import GeneralUtil
+from csle_cluster.cluster_manager.cluster_controller import ClusterController
 
 
 class Emulator:
     """
     Class for running episodes in the emulation system
     """
 
@@ -32,34 +35,37 @@
             emulation_env_config: EmulationEnvConfig, attacker_sequence: List[EmulationAttackerAction],
             defender_sequence: List[EmulationDefenderAction],
             repeat_times: int = 1, sleep_time: int = 1, save_dir: str = None,
             emulation_statistics: EmulationStatistics = None, descr: str = "", save: bool = True,
             data_collection_job: Optional[DataCollectionJobConfig] = None,
             save_emulation_traces_every: int = 10,
             emulation_traces_to_save_with_data_collection_job: int = 3,
-            intrusion_start_p: float = 0.1, intrusion_continue: float = 0.3) -> None:
+            intrusion_start_p: float = 0.1, intrusion_continue: float = 0.3, trace_len: int = 30,
+            restart_client_population: bool = False) -> None:
         """
         Runs an attacker and defender sequence in the emulation <repeat_times> times
 
         :param emulation_env_config: the configuration of the emulation
         :param attacker_sequence: the sequence of attacker actions
-        :param defender_sequence: the sequenceo of defender actions
+        :param defender_sequence: the sequence of defender actions
         :param repeat_times: the number of times to repeat the sequences
         :param sleep_time: the number of seconds to sleep between time-steps
         :param save_dir: the directory to save the collected traces
         :param emulation_statistics: the emulation statistics to update
         :param descr: descr of the execution
         :param save: boolean parameter indicating whether traces and statistics should be saved or not
         :param data_collection_job: the system identification job configuration
         :param save_emulation_traces_every: how frequently to save emulation traces
         :param emulation_traces_to_save_with_data_collection_job: num traces to save with the job
         :param intrusion_start_p: the p parameter for the geometric distribution that determines
                                   when an intrusion starts
         :param intrusion_continue: the p parameter for the geometric distribution that determines
                                    when an intrusion continues
+        :param trace_len: fixed trace length
+        :param restart_client_population: whether to restart the client population after each trace.
         :return: None
         """
         logger = Logger.__call__().get_logger()
 
         # Setup save dir
         if save_dir is None:
             save_dir = ExperimentUtil.default_output_dir() + "/results"
@@ -80,15 +86,15 @@
         if data_collection_job is None:
             data_collection_job = DataCollectionJobConfig(
                 emulation_env_name=emulation_env_config.name, num_collected_steps=0, progress_percentage=0.0,
                 attacker_sequence=attacker_sequence, defender_sequence=defender_sequence,
                 pid=pid, descr=descr, repeat_times=repeat_times, emulation_statistic_id=statistics_id, traces=[],
                 num_sequences_completed=0, save_emulation_traces_every=save_emulation_traces_every,
                 num_cached_traces=emulation_traces_to_save_with_data_collection_job,
-                log_file_path=Logger.__call__().get_log_file_path())
+                log_file_path=Logger.__call__().get_log_file_path(), physical_host_ip=GeneralUtil.get_host_ip())
             job_id = MetastoreFacade.save_data_collection_job(
                 data_collection_job=data_collection_job)
             data_collection_job.id = job_id
         else:
             data_collection_job.pid = pid
             data_collection_job.num_collected_steps = 0
             data_collection_job.progress_percentage = 0.0
@@ -97,29 +103,35 @@
             data_collection_job.log_file_path = Logger.__call__().get_log_file_path()
             MetastoreFacade.update_data_collection_job(data_collection_job=data_collection_job,
                                                        id=data_collection_job.id)
 
         # Start the collection
         s = EmulationEnvState(emulation_env_config=emulation_env_config)
         s.initialize_defender_machines()
+        emulation_statistics.initialize_machines(s=s)
         emulation_traces = []
         collected_steps = 0
         for i in range(repeat_times):
-            intrusion_start_time = np.random.geometric(p=intrusion_start_p, size=1)[0]
-            attacker_wait_seq = [EmulationAttackerStoppingActions.CONTINUE(index=-1)] * intrusion_start_time
-            defender_wait_seq = [EmulationDefenderStoppingActions.CONTINUE(index=-1)] * intrusion_start_time
-            full_attacker_sequence = attacker_wait_seq
-            full_defender_sequence = defender_wait_seq
-            for i in range(len(attacker_sequence)):
-                num_wait_steps = np.random.geometric(p=intrusion_continue, size=1)[0] - 1
-                wait_steps = [EmulationAttackerStoppingActions.CONTINUE(index=-1)] * num_wait_steps
-                full_attacker_sequence = full_attacker_sequence + wait_steps
-                full_attacker_sequence = full_attacker_sequence + [attacker_sequence[i]]
-                full_defender_sequence = full_defender_sequence + [
-                    EmulationDefenderStoppingActions.CONTINUE(index=-1)] * (num_wait_steps + 1)
+            intrusion_start_time = -1
+            if intrusion_start_p > 0:
+                intrusion_start_time = np.random.geometric(p=intrusion_start_p, size=1)[0]
+                attacker_wait_seq = [EmulationAttackerStoppingActions.CONTINUE(index=-1)] * intrusion_start_time
+                defender_wait_seq = [EmulationDefenderStoppingActions.CONTINUE(index=-1)] * intrusion_start_time
+                full_attacker_sequence = attacker_wait_seq
+                full_defender_sequence = defender_wait_seq
+                for j in range(len(attacker_sequence)):
+                    num_wait_steps = np.random.geometric(p=intrusion_continue, size=1)[0] - 1
+                    wait_steps = [EmulationAttackerStoppingActions.CONTINUE(index=-1)] * num_wait_steps
+                    full_attacker_sequence = full_attacker_sequence + wait_steps
+                    full_attacker_sequence = full_attacker_sequence + [attacker_sequence[j]]
+                    full_defender_sequence = full_defender_sequence + [
+                        EmulationDefenderStoppingActions.CONTINUE(index=-1)] * (num_wait_steps + 1)
+            else:
+                full_attacker_sequence = [EmulationAttackerStoppingActions.CONTINUE(index=-1)] * trace_len
+                full_defender_sequence = [EmulationDefenderStoppingActions.CONTINUE(index=-1)] * trace_len
             T = len(full_attacker_sequence)
             assert len(full_defender_sequence) == len(full_attacker_sequence)
             logger.info(f"Starting execution of static action sequences, iteration:{i}, T:{T}, "
                         f"I_t:{intrusion_start_time}")
             sys.stdout.flush()
             s.reset()
             emulation_trace = EmulationTrace(initial_attacker_observation_state=s.attacker_obs_state,
@@ -130,38 +142,92 @@
             s.defender_obs_state.average_metric_lists()
             emulation_statistics.update_initial_statistics(s=s)
             traces = emulation_traces + [emulation_trace]
             if len(traces) > data_collection_job.num_cached_traces:
                 data_collection_job.traces = traces[-data_collection_job.num_cached_traces:]
             else:
                 data_collection_job.traces = traces
+
+            if restart_client_population:
+                ClusterController.stop_kafka_client_producer(
+                    ip=emulation_env_config.traffic_config.client_population_config.physical_host_ip,
+                    port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT, ip_first_octet=emulation_env_config.execution_id,
+                    emulation=emulation_env_config.name)
+                ClusterController.stop_client_population(
+                    ip=emulation_env_config.traffic_config.client_population_config.physical_host_ip,
+                    port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT, ip_first_octet=emulation_env_config.execution_id,
+                    emulation=emulation_env_config.name)
+                time.sleep(5)
+                ClusterController.start_client_population(
+                    ip=emulation_env_config.traffic_config.client_population_config.physical_host_ip,
+                    port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT, ip_first_octet=emulation_env_config.execution_id,
+                    emulation=emulation_env_config.name
+                )
+                time.sleep(5)
+                ClusterController.start_kafka_client_producer(
+                    ip=emulation_env_config.traffic_config.client_population_config.physical_host_ip,
+                    port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT, ip_first_octet=emulation_env_config.execution_id,
+                    emulation=emulation_env_config.name
+                )
+                time.sleep(15)
+
             for t in range(T):
                 old_state = s.copy()
                 a1 = full_defender_sequence[t]
                 a2 = full_attacker_sequence[t]
                 logger.info(f"t:{t}, a1: {a1}, a2: {a2}")
                 s.defender_obs_state.reset_metric_lists()
                 emulation_trace, s = Emulator.run_actions(
                     emulation_env_config=emulation_env_config, attacker_action=a2, defender_action=a1,
                     sleep_time=sleep_time, trace=emulation_trace, s=s)
                 emulation_statistics.update_delta_statistics(s=old_state, s_prime=s, a1=a1, a2=a2)
-                total_steps = (1 / intrusion_start_p) * repeat_times
+                if intrusion_start_p > 0:
+                    total_steps = (1 / intrusion_start_p) * repeat_times
+                else:
+                    total_steps = trace_len
                 collected_steps += 1
                 data_collection_job.num_collected_steps = collected_steps
                 data_collection_job.progress_percentage = (round(collected_steps / total_steps, 2))
                 data_collection_job.num_sequences_completed = i
                 data_collection_job.traces[-1] = emulation_trace
                 logger.debug(f"job updated, steps collected: {data_collection_job.num_collected_steps}, "
                              f"progress: {data_collection_job.progress_percentage}, "
                              f"sequences completed: {i}/{repeat_times}")
                 sys.stdout.flush()
                 MetastoreFacade.update_data_collection_job(data_collection_job=data_collection_job,
                                                            id=data_collection_job.id)
                 MetastoreFacade.update_emulation_statistic(emulation_statistics=emulation_statistics, id=statistics_id)
 
+                if restart_client_population:
+                    ClusterController.stop_kafka_client_producer(
+                        ip=emulation_env_config.traffic_config.client_population_config.physical_host_ip,
+                        port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+                        ip_first_octet=emulation_env_config.execution_id,
+                        emulation=emulation_env_config.name)
+                    ClusterController.stop_client_population(
+                        ip=emulation_env_config.traffic_config.client_population_config.physical_host_ip,
+                        port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+                        ip_first_octet=emulation_env_config.execution_id,
+                        emulation=emulation_env_config.name)
+                    time.sleep(5)
+                    ClusterController.start_client_population(
+                        ip=emulation_env_config.traffic_config.client_population_config.physical_host_ip,
+                        port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+                        ip_first_octet=emulation_env_config.execution_id,
+                        emulation=emulation_env_config.name
+                    )
+                    time.sleep(5)
+                    ClusterController.start_kafka_client_producer(
+                        ip=emulation_env_config.traffic_config.client_population_config.physical_host_ip,
+                        port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+                        ip_first_octet=emulation_env_config.execution_id,
+                        emulation=emulation_env_config.name
+                    )
+                    time.sleep(15)
+
             if save and i % save_emulation_traces_every == 0:
                 MetastoreFacade.save_emulation_trace(emulation_trace)
             emulation_traces.append(emulation_trace)
 
         logger.info("All sequences completed, saving traces and emulation statistics")
         sys.stdout.flush()
         if save:
@@ -187,16 +253,17 @@
         :return: the updated trace and state
         """
         logger = Logger.__call__().get_logger()
         attacker_action.ips = s.attacker_obs_state.get_action_ips(a=attacker_action,
                                                                   emulation_env_config=emulation_env_config)
         defender_action.ips = s.defender_obs_state.get_action_ips(a=defender_action,
                                                                   emulation_env_config=emulation_env_config)
-        logger.debug(f"Executing attacker action:{attacker_action.name} on machine index: {attacker_action.index}, "
-                     f"ips:{attacker_action.ips}")
+        logger.info(f"Executing attacker action:{attacker_action.name} on machine index: {attacker_action.index}, "
+                    f"ips:{attacker_action.ips}")
+        logger.info(f"Machines: {list(map(lambda x: x.ips[0], s.attacker_obs_state.machines))}")
         s_prime = Attacker.attacker_transition(s=s, attacker_action=attacker_action)
         logger.debug(f"Attacker action complete, attacker state:{s_prime.attacker_obs_state}")
         EnvDynamicsUtil.cache_attacker_action(a=attacker_action, s=s_prime)
         logger.debug(f"Executing defender action:{defender_action.name} on machine index: {defender_action.index}")
         s_prime_prime = Defender.defender_transition(s=s_prime, defender_action=defender_action)
         logger.debug(f"Defender action complete, defender state:{s_prime.defender_obs_state}, "
                      f"ips:{defender_action.ips}")
```

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py` & `csle_system_identification-0.2.0/src/csle_system_identification/expectation_maximization/expectation_maximization_algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from csle_system_identification.base.base_system_identification_algorithm import BaseSystemIdentificationAlgorithm
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.system_identification.emulation_statistics import EmulationStatistics
 from csle_common.dao.system_identification.system_identification_config import SystemIdentificationConfig
 from csle_common.dao.system_identification.gaussian_mixture_system_model import GaussianMixtureSystemModel
 from csle_common.dao.system_identification.gaussian_mixture_conditional import GaussianMixtureConditional
 from csle_common.dao.jobs.system_identification_job_config import SystemIdentificationJobConfig
-import csle_system_identification.constants.constants as system_identification_constants
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.logging.log import Logger
+from csle_common.util.general_util import GeneralUtil
+import csle_system_identification.constants.constants as system_identification_constants
 
 
 class ExpectationMaximizationAlgorithm(BaseSystemIdentificationAlgorithm):
     """
     Class that implements the system identification procedure using EM
     """
 
@@ -46,15 +47,16 @@
         descr = f"System identification through Expectation Maximization, " \
                 f"emulation:{self.emulation_env_config.name}, statistic id: {self.emulation_statistics.id}"
         if self.system_identification_job is None:
             self.system_identification_job = SystemIdentificationJobConfig(
                 emulation_env_name=self.emulation_env_config.name,
                 emulation_statistics_id=self.emulation_statistics.id, pid=pid, progress_percentage=0,
                 log_file_path=Logger.__call__().get_log_file_path(), descr=descr, system_model=None,
-                system_identification_config=self.system_identification_config
+                system_identification_config=self.system_identification_config,
+                physical_host_ip=GeneralUtil.get_host_ip()
             )
             system_identification_job_id = MetastoreFacade.save_system_identification_job(
                 system_identification_job=self.system_identification_job)
             self.system_identification_job.id = system_identification_job_id
         else:
             self.system_identification_job.pid = pid
             self.system_identification_job.progress_percentage = 0
```

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/gp/gp_regression_algorithm.py` & `csle_system_identification-0.2.0/src/csle_system_identification/gp/gp_regression_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from csle_system_identification.base.base_system_identification_algorithm import BaseSystemIdentificationAlgorithm
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.system_identification.emulation_statistics import EmulationStatistics
 from csle_common.dao.system_identification.system_identification_config import SystemIdentificationConfig
 from csle_common.dao.system_identification.gp_system_model import GPSystemModel
 from csle_common.dao.system_identification.gp_conditional import GPConditional
 from csle_common.dao.jobs.system_identification_job_config import SystemIdentificationJobConfig
-import csle_system_identification.constants.constants as system_identification_constants
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.logging.log import Logger
+from csle_common.util.general_util import GeneralUtil
+import csle_system_identification.constants.constants as system_identification_constants
 from csle_system_identification.gp.gp_regression_model_with_gauissan_noise import GPRegressionModelWithGaussianNoise
 
 
 class GPRegressionAlgorithm(BaseSystemIdentificationAlgorithm):
     """
     Class that implements the system identification procedure using EM
     """
@@ -48,16 +49,16 @@
         descr = f"System identification through Gaussian Process Regression, " \
                 f"emulation:{self.emulation_env_config.name}, statistic id: {self.emulation_statistics.id}"
         if self.system_identification_job is None:
             self.system_identification_job = SystemIdentificationJobConfig(
                 emulation_env_name=self.emulation_env_config.name,
                 emulation_statistics_id=self.emulation_statistics.id, pid=pid, progress_percentage=0,
                 log_file_path=Logger.__call__().get_log_file_path(), descr=descr, system_model=None,
-                system_identification_config=self.system_identification_config
-            )
+                system_identification_config=self.system_identification_config,
+                physical_host_ip=GeneralUtil.get_host_ip())
             system_identification_job_id = MetastoreFacade.save_system_identification_job(
                 system_identification_job=self.system_identification_job)
             self.system_identification_job.id = system_identification_job_id
         else:
             self.system_identification_job.pid = pid
             self.system_identification_job.progress_percentage = 0
             self.system_identification_job.system_model = None
```

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py` & `csle_system_identification-0.2.0/src/csle_system_identification/gp/gp_regression_model_with_gauissan_noise.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/data_collection_job_manager.py` & `csle_system_identification-0.2.0/src/csle_system_identification/job_controllers/data_collection_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification/job_controllers/system_identification_job_manager.py` & `csle_system_identification-0.2.0/src/csle_system_identification/job_controllers/system_identification_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification.egg-info/PKG-INFO` & `csle_system_identification-0.2.0/src/csle_system_identification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-system-identification
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for system identification in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_system_identification-0.1.9/src/csle_system_identification.egg-info/SOURCES.txt` & `csle_system_identification-0.2.0/src/csle_system_identification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

