# Comparing `tmp/gym_csle_stopping_game-0.1.9.tar.gz` & `tmp/gym_csle_stopping_game-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_stopping_game-0.1.9.tar", last modified: Tue Mar 21 08:09:55 2023, max compression
+gzip compressed data, was "gym_csle_stopping_game-0.2.0.tar", last modified: Sun Apr 30 12:37:10 2023, max compression
```

## Comparing `gym_csle_stopping_game-0.1.9.tar` & `gym_csle_stopping_game-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      695 2023-02-11 20:28:41.000000 gym_csle_stopping_game-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1370 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/
--rw-rw-r--   0 kim       (1000) kim       (1000)      651 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3002 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4948 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3249 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1375 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)       74 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    24342 2022-12-02 09:20:45.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8926 2023-03-03 06:17:38.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7639 2023-03-03 06:17:38.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18598 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/util/stopping_game_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-03-21 08:09:54.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1130 2023-03-21 08:09:55.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:54.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-03-21 08:09:55.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       23 2023-03-21 08:09:55.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      703 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1378 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      657 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3002 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4961 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/stopping_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3249 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1375 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/stopping_game_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       74 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    24656 2023-04-30 06:59:23.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/envs/stopping_game_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9022 2023-04-18 14:59:42.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7749 2023-04-30 06:59:23.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18598 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/util/stopping_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:10.968697 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-04-30 12:37:10.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1130 2023-04-30 12:37:10.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:37:10.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      259 2023-04-30 12:37:10.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       23 2023-04-30 12:37:10.000000 gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/top_level.txt
```

### Comparing `gym_csle_stopping_game-0.1.9/PKG-INFO` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gym_csle_stopping_game
-Version: 0.1.9
+Name: gym-csle-stopping-game
+Version: 0.2.0
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.1.9/pyproject.toml` & `gym_csle_stopping_game-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools==62.0.0", "gym>=0.21"]
+requires = ["setuptools==62.0.0", "gymnasium>=0.27.1"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--cov=gym_csle_stopping_game -p no:warnings"
 testpaths = [
     "tests",
 ]
```

### Comparing `gym_csle_stopping_game-0.1.9/setup.cfg` & `gym_csle_stopping_game-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	gym>=0.21
-	csle-common>=0.1.9
-	csle-attacker>=0.1.9
-	csle-defender>=0.1.9
-	csle-collector>=0.1.9
+	gymnasium>=0.27.1
+	csle-common>=0.2.0
+	csle-attacker>=0.2.0
+	csle-defender>=0.2.0
+	csle-collector>=0.2.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/__init__.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Register OpenAI Envs
 """
 from . __version__ import __version__
-from gym.envs.registration import register
+from gymnasium.envs.registration import register
 
 register(
     id='csle-stopping-game-v1',
     entry_point='gym_csle_stopping_game.envs.stopping_game_env:StoppingGameEnv',
     kwargs={'config': None}
 )
```

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/constants/constants.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_config.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/stopping_game_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, Any
-import gym
+import gymnasium as gym
 import numpy as np
 from csle_common.dao.simulation_config.simulation_env_input_config import SimulationEnvInputConfig
 
 
 class StoppingGameConfig(SimulationEnvInputConfig):
     """
     DTO class containing the configuration of the stopping game
```

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_state.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/dao/stopping_game_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_env.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/envs/stopping_game_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Dict, Union, List
+from typing import Tuple, Dict, Union, List, Any
 import numpy as np
 import time
 import math
 import csle_common.constants.constants as constants
 from csle_common.dao.simulation_config.base_env import BaseEnv
 from csle_common.dao.simulation_config.simulation_trace import SimulationTrace
 from csle_common.dao.training.policy import Policy
@@ -39,14 +39,17 @@
 
         # Setup spaces
         self.attacker_observation_space = self.config.attacker_observation_space()
         self.defender_observation_space = self.config.defender_observation_space()
         self.attacker_action_space = self.config.attacker_action_space()
         self.defender_action_space = self.config.defender_action_space()
 
+        self.action_space = self.defender_action_space
+        self.observation_space = self.defender_observation_space
+
         # Setup Config
         self.viewer = None
         self.metadata = {
             'render.modes': ['human', 'rgb_array'],
             'video.frames_per_second': 50  # Video rendering speed
         }
 
@@ -55,20 +58,20 @@
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
 
         # Reset
         self.reset()
         super().__init__()
 
     def step(self, action_profile: Tuple[int, Tuple[np.ndarray, int]]) \
-            -> Tuple[Tuple[np.ndarray, np.ndarray], Tuple[int, int], bool, dict]:
+            -> Tuple[Tuple[np.ndarray, np.ndarray], Tuple[int, int], bool, bool, dict]:
         """
         Takes a step in the environment by executing the given action
 
         :param action_profile: the actions to take (both players actions
-        :return: (obs, reward, done, info)
+        :return: (obs, reward, terminated, truncated, info)
         """
 
         # Setup initial values
         a1, a2_profile = action_profile
         pi2, a2 = a2_profile
         assert pi2.shape[0] == len(self.config.S)
         assert pi2.shape[1] == len(self.config.A1)
@@ -120,15 +123,15 @@
         if not done:
             self.trace.attacker_observations.append(attacker_obs)
             self.trace.defender_observations.append(defender_obs)
 
         # Populate info
         info = self._info(info)
 
-        return (defender_obs, attacker_obs), (r, -r), done, info
+        return (defender_obs, attacker_obs), (r, -r), done, done, info
 
     def step_test(self, action_profile: Tuple[int, Tuple[np.ndarray, int]], sample_Z) \
             -> Tuple[Tuple[np.ndarray, np.ndarray], Tuple[int, int], bool, dict]:
         """
         Takes a step in the environment by executing the given action
 
         :param action_profile: the actions to take (both players actions
@@ -316,50 +319,54 @@
         upper_bound_return = 0
         defender_baseline_stop_on_first_alert_return = 0
         upper_bound_stops_remaining = self.config.L
         defender_baseline_stop_on_first_alert_stops_remaining = self.config.L
         for i in range(len(self.trace.states)):
             if defender_baseline_stop_on_first_alert_stops_remaining > 0:
                 if self.trace.infrastructure_metrics[i] > 0:
-                    defender_baseline_stop_on_first_alert_return += self.config.R[
-                        int(defender_baseline_stop_on_first_alert_stops_remaining) - 1][1][
-                        self.trace.attacker_actions[i]][self.trace.states[i]] * math.pow(self.config.gamma, i)
+                    defender_baseline_stop_on_first_alert_return += \
+                        self.config.R[int(defender_baseline_stop_on_first_alert_stops_remaining) - 1][1][
+                            self.trace.attacker_actions[i]][self.trace.states[i]] * math.pow(self.config.gamma, i)
                     defender_baseline_stop_on_first_alert_stops_remaining -= 1
                 else:
-                    defender_baseline_stop_on_first_alert_return += self.config.R[
-                        int(defender_baseline_stop_on_first_alert_stops_remaining) - 1][0][
-                        self.trace.attacker_actions[i]][self.trace.states[i]] * math.pow(self.config.gamma, i)
+                    defender_baseline_stop_on_first_alert_return += \
+                        self.config.R[int(defender_baseline_stop_on_first_alert_stops_remaining) - 1][0][
+                            self.trace.attacker_actions[i]][self.trace.states[i]] * math.pow(self.config.gamma, i)
             if upper_bound_stops_remaining > 0:
                 if self.trace.states[i] == 0:
-                    upper_bound_return += self.config.R[int(upper_bound_stops_remaining) - 1][0][
-                        self.trace.attacker_actions[i]][self.trace.states[i]] * math.pow(self.config.gamma, i)
+                    r = self.config.R[int(upper_bound_stops_remaining) - 1][0][self.trace.attacker_actions[i]][
+                        self.trace.states[i]]
+                    upper_bound_return += r * math.pow(self.config.gamma, i)
                 else:
-                    upper_bound_return += self.config.R[int(upper_bound_stops_remaining) - 1][1][
-                        self.trace.attacker_actions[i]][self.trace.states[i]] * math.pow(self.config.gamma, i)
+                    r = self.config.R[int(upper_bound_stops_remaining) - 1][1][self.trace.attacker_actions[i]][
+                        self.trace.states[i]]
+                    upper_bound_return += r * math.pow(self.config.gamma, i)
                     upper_bound_stops_remaining -= 1
         info[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = upper_bound_return
         info[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN] = \
             defender_baseline_stop_on_first_alert_return
         return info
 
-    def reset(self, soft: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+    def reset(self, seed: int = 0, soft: bool = False) -> Tuple[Tuple[np.ndarray, np.ndarray], Dict[str, Any]]:
         """
         Resets the environment state, this should be called whenever step() returns <done>
 
         :return: initial observation
         """
+        super().reset(seed=seed)
         self.state.reset()
         if len(self.trace.attacker_rewards) > 0:
             self.traces.append(self.trace)
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         attacker_obs = self.state.attacker_observation()
         defender_obs = self.state.defender_observation()
         self.trace.attacker_observations.append(attacker_obs)
         self.trace.defender_observations.append(defender_obs)
-        return defender_obs, attacker_obs
+        info = {}
+        return (defender_obs, attacker_obs), info
 
     @staticmethod
     def emulation_evaluation(env: "StoppingGameEnv", n_episodes: int, intrusion_seq: List[EmulationAttackerAction],
                              defender_policy: Policy,
                              attacker_policy: Policy,
                              emulation_env_config: EmulationEnvConfig,
                              simulation_env_config: SimulationEnvConfig
```

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Tuple, List, Union
-import gym
+from typing import Tuple, List, Union, Dict, Any
+import gymnasium as gym
 import numpy as np
 import torch
 import math
 from csle_common.dao.simulation_config.base_env import BaseEnv
 from csle_common.dao.training.mixed_multi_threshold_stopping_policy import MixedMultiThresholdStoppingPolicy
 from gym_csle_stopping_game.dao.stopping_game_attacker_mdp_config import StoppingGameAttackerMdpConfig
 from csle_common.dao.simulation_config.simulation_trace import SimulationTrace
@@ -44,20 +44,20 @@
         self.model = None
 
         # Reset
         self.reset()
         super().__init__()
 
     def step(self, pi2: Union[List[List[float]], int, float, np.int64, np.float]) \
-            -> Tuple[np.ndarray, int, bool, dict]:
+            -> Tuple[np.ndarray, int, bool, bool, dict]:
         """
         Takes a step in the environment by executing the given action
 
         :param pi2: attacker stage policy
-        :return: (obs, reward, done, info)
+        :return: (obs, reward, terminated, truncated, info)
         """
         if type(pi2) is int or type(pi2) is float or type(pi2) is np.int64 or type(pi2) is np.float:
             a2 = pi2
             pi2 = self.calculate_stage_policy(o=self.latest_attacker_obs, a2=a2)
         else:
             if self.model is not None:
                 pi2 = self.calculate_stage_policy(o=self.latest_attacker_obs)
@@ -87,27 +87,28 @@
         self.latest_attacker_obs = o[1]
         attacker_obs = o[1]
 
         info[env_constants.ENV_METRICS.RETURN] = -info[env_constants.ENV_METRICS.RETURN]
         info[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = \
             -info[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN]
 
-        return attacker_obs, r[1], d, info
+        return attacker_obs, r[1], d, d, info
 
-    def reset(self, soft: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+    def reset(self, seed: int = 0, soft: bool = False) -> Tuple[np.ndarray, Dict[str, Any]]:
         """
         Resets the environment state, this should be called whenever step() returns <done>
 
         :return: initial observation
         """
-        o = self.stopping_game_env.reset()
+        o, _ = self.stopping_game_env.reset()
         self.latest_defender_obs = o[0]
         self.latest_attacker_obs = o[1]
         attacker_obs = o[1]
-        return attacker_obs
+        info = {}
+        return attacker_obs, info
 
     def set_model(self, model) -> None:
         """
         Sets the model. Useful when using RL frameworks where the stage policy is not easy to extract
 
         :param model: the model
         :return: None
```

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Tuple, List
-import gym
+from typing import Tuple, List, Dict, Any
+import gymnasium as gym
 import numpy as np
 from csle_common.dao.simulation_config.base_env import BaseEnv
 from gym_csle_stopping_game.dao.stopping_game_defender_pomdp_config import StoppingGameDefenderPomdpConfig
 from csle_common.dao.simulation_config.simulation_trace import SimulationTrace
 from csle_common.dao.training.policy import Policy
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
@@ -44,31 +44,31 @@
         }
 
         self.latest_attacker_obs = None
         # Reset
         self.reset()
         super().__init__()
 
-    def step(self, a1: int) -> Tuple[np.ndarray, int, bool, dict]:
+    def step(self, a1: int) -> Tuple[np.ndarray, int, bool, bool, dict]:
         """
         Takes a step in the environment by executing the given action
 
         :param a1: defender action
-        :return: (obs, reward, done, info)
+        :return: (obs, reward, terminated, truncated, info)
         """
         # Get attacker action from static strategy
         pi2 = np.array(self.static_attacker_strategy.stage_policy(self.latest_attacker_obs))
-        a2 = StoppingGameUtil.sample_attacker_action(pi2=pi2, s=self.stopping_game_env.state.state_idx)
+        a2 = StoppingGameUtil.sample_attacker_action(pi2=pi2, s=self.stopping_game_env.state.s)
 
         # Step the game
-        o, r, d, info = self.stopping_game_env.step((a1, (pi2, a2)))
+        o, r, d, _, info = self.stopping_game_env.step((a1, (pi2, a2)))
         self.latest_attacker_obs = o[1]
         defender_obs = o[0]
 
-        return defender_obs, r[0], d, info
+        return defender_obs, r[0], d, d, info
 
     def step_test(self, a1: int, sample_Z) -> Tuple[np.ndarray, int, bool, dict]:
         """
         Takes a step in the environment by executing the given action
 
         :param a1: defender action
         :return: (obs, reward, done, info)
@@ -80,24 +80,25 @@
         # Step the game
         o, r, d, info = self.stopping_game_env.step_test((a1, (pi2, a2)), sample_Z=sample_Z)
         self.latest_attacker_obs = o[1]
         defender_obs = o[0]
 
         return defender_obs, r[0], d, info
 
-    def reset(self, soft: bool = False) -> np.ndarray:
+    def reset(self, seed: int = 0, soft: bool = False) -> Tuple[np.ndarray, Dict[str, Any]]:
         """
         Resets the environment state, this should be called whenever step() returns <done>
 
         :return: initial observation
         """
-        o = self.stopping_game_env.reset()
+        o, _ = self.stopping_game_env.reset()
         self.latest_attacker_obs = o[1]
         defender_obs = o[0]
-        return defender_obs
+        dict = {}
+        return defender_obs, dict
 
     def render(self, mode: str = 'human'):
         """
         Renders the environment.  Supported rendering modes: (1) human; and (2) rgb_array
 
         :param mode: the rendering mode
         :return: True (if human mode) otherwise an rgb array
```

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/util/stopping_game_util.py` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game/util/stopping_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/PKG-INFO` & `gym_csle_stopping_game-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gym-csle-stopping-game
-Version: 0.1.9
+Name: gym_csle_stopping_game
+Version: 0.2.0
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/SOURCES.txt` & `gym_csle_stopping_game-0.2.0/src/gym_csle_stopping_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

