# Comparing `tmp/gym_csle_intrusion_response_game-0.1.9.tar.gz` & `tmp/gym_csle_intrusion_response_game-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_intrusion_response_game-0.1.9.tar", last modified: Tue Mar 21 08:10:08 2023, max compression
+gzip compressed data, was "gym_csle_intrusion_response_game-0.2.0.tar", last modified: Sun Apr 30 12:37:26 2023, max compression
```

## Comparing `gym_csle_intrusion_response_game-0.1.9.tar` & `gym_csle_intrusion_response_game-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      719 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      705 2023-02-28 13:20:12.000000 gym_csle_intrusion_response_game-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1394 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 gym_csle_intrusion_response_game-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/
--rw-rw-r--   0 kim       (1000) kim       (1000)     1183 2023-03-07 08:02:15.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1403 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3189 2023-03-06 16:53:37.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3194 2023-03-06 16:51:52.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2468 2023-03-06 13:37:53.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5513 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5154 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2890 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2890 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)      588 2023-03-07 08:02:15.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12607 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12670 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12682 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    12691 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    36796 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      719 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1837 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-02-28 13:33:21.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       33 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      719 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      713 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1402 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.780772 gym_csle_intrusion_response_game-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.780772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1479 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.780772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1841 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.784772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3189 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3258 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2468 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6078 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4599 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2890 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2890 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      749 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13921 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17161 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12925 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12783 2023-04-18 14:55:10.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16406 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.788772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    52898 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:26.780772 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      719 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1936 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 11:24:24.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      259 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       33 2023-04-30 12:37:26.000000 gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/PKG-INFO` & `gym_csle_intrusion_response_game-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_intrusion_response_game
-Version: 0.1.9
+Version: 0.2.0
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/pyproject.toml` & `gym_csle_intrusion_response_game-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools==62.0.0", "gym>=0.21"]
+requires = ["setuptools==62.0.0", "gymnasium>=0.27.1"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--cov=gym_csle_intrusion_response_game -p no:warnings"
 testpaths = [
     "tests",
 ]
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/setup.cfg` & `gym_csle_intrusion_response_game-0.2.0/setup.cfg`

 * *Files 26% similar despite different names*

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

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/__init__.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Register OpenAI Envs
 """
 from . __version__ import __version__
-from gym.envs.registration import register
+from gymnasium.envs.registration import register
 
 register(
     id='csle-intrusion-response-game-local-pomdp-defender-v1',
     entry_point='gym_csle_intrusion_response_game.envs.intrusion_response_game_local_pomdp_defender:'
                 'IntrusionResponseGameLocalPOMDPDefenderEnv', kwargs={'config': None}
 )
 
@@ -22,8 +22,14 @@
                 'IntrusionResponseGameWorkflowPOMDPDefenderEnv', kwargs={'config': None}
 )
 
 register(
     id='csle-intrusion-response-game-workflow-pomdp-attacker-v1',
     entry_point='gym_csle_intrusion_response_game.envs.intrusion_response_game_workflow_pomdp_attacker:'
                 'IntrusionResponseGameWorkflowPOMDPAttackerEnv', kwargs={'config': None}
+)
+
+register(
+    id='csle-intrusion-response-game-local-stopping-pomdp-defender-v1',
+    entry_point='gym_csle_intrusion_response_game.envs.intrusion_response_game_local_stopping_pomdp_defender:'
+                'IntrusionResponseGameLocalStoppingPOMDPDefenderEnv', kwargs={'config': None}
 )
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         :param local_intrusion_response_game_config: The underlying game config
         :param attacker_strategy: the attacker's strategy name
         """
         super().__init__()
         self.env_name = env_name
         self.local_intrusion_response_game_config = local_intrusion_response_game_config
         self.attacker_strategy = attacker_strategy
+        self.stopping_action = 3
+        self.stopping_zone = 3
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "IntrusionResponseGameLocalPOMDPDefenderConfig":
         """
         Converts a dict representation to an instance
 
         :param d: the dict to convert
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Any
 import numpy as np
-import gym
+import gymnasium as gym
 import gym_csle_intrusion_response_game.constants.constants as env_constants
 
 
 class LocalIntrusionResponseGameConfig:
     """
     DTO representing the configuration of the local intrusion response game
     """
@@ -72,30 +72,44 @@
                               high=np.array([len(self.S_A)] + [1] * len(self.S_D)),
                               dtype=np.float32, shape=(len(self.S_D) + 1,))
 
     def defender_observation_space(self) -> gym.spaces.Box:
         """
         :return: the defender's observation space
         """
-        return gym.spaces.Box(low=np.array([0] * (len(self.S_A) + 1)),
+        return gym.spaces.Box(low=np.array(([0] * (len(self.S_A) + 1))),
                               high=np.array([len(self.zones)] + [1] * len(self.S_A)),
                               dtype=np.float32, shape=(len(self.S_A) + 1,))
 
+    def defender_observation_space_stopping(self) -> gym.spaces.Box:
+        """
+        :return: the defender's observation space
+        """
+        return gym.spaces.Box(low=np.array(([0] * (len(self.S_A)))),
+                              high=np.array([1] * len(self.S_A)),
+                              dtype=np.float32, shape=(len(self.S_A),))
+
     def attacker_action_space(self) -> gym.spaces.Discrete:
         """
         :return: the attacker's action space
         """
         return gym.spaces.Discrete(len(self.A2))
 
     def defender_action_space(self) -> gym.spaces.Discrete:
         """
         :return: the defender's action space
         """
         return gym.spaces.Discrete(len(self.A1))
 
+    def defender_action_space_stopping(self) -> gym.spaces.Discrete:
+        """
+        :return: the defender's action space in the stopping POMDP
+        """
+        return gym.spaces.Discrete(2)
+
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["T"] = list(self.T.tolist())
         d["O"] = list(self.O.tolist())
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, Any
-import gym
+import gymnasium as gym
 import numpy as np
 
 
 class WorkflowIntrusionResponseGameConfig:
     """
     DTO representing the configuration of a workflow intrusion response game
     """
@@ -61,28 +61,20 @@
                               dtype=np.float32, shape=(4 * len(self.nodes),))
 
     def attacker_action_space(self) -> gym.spaces.MultiDiscrete:
         """
         :return: the attacker's action space
         """
         return gym.spaces.MultiDiscrete(nvec=np.array([4] * len(self.nodes)), dtype=np.int64)
-        # return gym.spaces.Box(low=np.array([0]*len(self.nodes)), high=np.array([3]*len(self.nodes)), dtype=np.int,
-        #                       shape=(len(self.nodes),))
-        # return gym.spaces.Discrete(4*len(self.nodes))
 
     def defender_action_space(self) -> gym.spaces.MultiDiscrete:
         """
         :return: the defender's action space
         """
-        # print(np.array(([0] + self.zones.tolist())*len(self.nodes)))
         return gym.spaces.MultiDiscrete(nvec=np.array([1 + len(self.zones)] * len(self.nodes)), dtype=np.int64)
-        # return gym.spaces.Box(low=np.array([0]*len(self.nodes)), high=np.array([len(self.zones)]*len(self.nodes)),
-        # dtype=np.int,
-        #                       shape=(len(self.nodes),))
-        # gym.spaces.Discrete((len(self.zones)+1)*len(self.nodes))
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["nodes"] = list(self.nodes.tolist())
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/__init__.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,7 +2,9 @@
     import IntrusionResponseGameLocalPOMDPDefenderEnv
 from gym_csle_intrusion_response_game.envs.intrusion_response_game_local_pomdp_attacker \
     import IntrusionResponseGameLocalPOMDPAttackerEnv
 from gym_csle_intrusion_response_game.envs.intrusion_response_game_workflow_pomdp_defender \
     import IntrusionResponseGameWorkflowPOMDPDefenderEnv
 from gym_csle_intrusion_response_game.envs.intrusion_response_game_workflow_pomdp_attacker \
     import IntrusionResponseGameWorkflowPOMDPAttackerEnv
+from gym_csle_intrusion_response_game.envs.intrusion_response_game_local_stopping_pomdp_defender \
+    import IntrusionResponseGameLocalStoppingPOMDPDefenderEnv
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,38 +58,67 @@
 
         # Reset
         self.reset()
 
         # Get upper bound and random return estimate
         self.upper_bound_return = 0
         self.random_return = 0
+        self.attack_return = 0
         self.upper_bound_return = self.get_upper_bound_return(samples=100)
         self.random_return = self.get_random_baseline_return(samples=100)
+        self.attack_return = self.get_attack_baseline_return(samples=100)
 
         # Reset
         self.reset()
         super().__init__()
 
     def get_random_baseline_return(self, samples: int = 100) -> float:
         """
-        Utiltiy function for estimating the average return of a random defender strategy
+        Utiltiy function for estimating the average return of a random attacker strategy
 
         :param samples: the number of samples to use for estimation
         :return: the estimated return
         """
         max_horizon = 1000
         returns = []
         for i in range(samples):
-            o = self.reset()
+            o, _ = self.reset()
             done = False
             t = 0
             cumulative_reward = 0
             while not done and t <= max_horizon:
                 a2 = np.random.choice(self.config.local_intrusion_response_game_config.A2)
-                o, r, done, info = self.step(a2)
+                o, r, done, _, info = self.step(a2)
+                cumulative_reward += r * math.pow(self.config.local_intrusion_response_game_config.gamma, t)
+                t += 1
+            returns.append(cumulative_reward)
+        return np.mean(np.array(returns))
+
+    def get_attack_baseline_return(self, samples: int = 100) -> float:
+        """
+        Utiltiy function for estimating the average return of the "always attacker" attacker strategy
+
+        :param samples: the number of samples to use for estimation
+        :return: the estimated return
+        """
+        max_horizon = 1000
+        returns = []
+        for i in range(samples):
+            o, _ = self.reset()
+            done = False
+            t = 0
+            cumulative_reward = 0
+            while not done and t <= max_horizon:
+                if o[0] == 0:
+                    a2 = 1
+                if o[0] == 1:
+                    a2 = np.random.choice([2, 3])
+                if o[0] == 2:
+                    a2 = 0
+                o, r, done, _, info = self.step(a2)
                 cumulative_reward += r * math.pow(self.config.local_intrusion_response_game_config.gamma, t)
                 t += 1
             returns.append(cumulative_reward)
         return np.mean(np.array(returns))
 
     def get_upper_bound_return(self, samples: int = 100) -> float:
         """
@@ -97,36 +126,36 @@
 
         :param samples: the number of sample returns to average
         :return: the estimated upper bound
         """
         max_horizon = 1000
         returns = []
         for i in range(samples):
-            o = self.reset()
+            o, _ = self.reset()
             done = False
             t = 0
             cumulative_reward = 0
             while not done and t <= max_horizon:
                 a2 = 0
                 if self.state.attacker_state() == env_constants.ATTACK_STATES.HEALTHY:
                     a2 = env_constants.ATTACKER_ACTIONS.RECON
                 elif self.state.attacker_state() == env_constants.ATTACK_STATES.RECON:
                     a2 = env_constants.ATTACKER_ACTIONS.EXPLOIT
-                o, r, done, info = self.step(a2)
+                o, r, done, _, info = self.step(a2)
                 cumulative_reward += r * math.pow(self.config.local_intrusion_response_game_config.gamma, t)
                 t += 1
             returns.append(cumulative_reward)
         return np.mean(np.array(returns))
 
-    def step(self, a2: int) -> Tuple[np.ndarray, float, bool, Dict[str, Union[float, int]]]:
+    def step(self, a2: int) -> Tuple[np.ndarray, float, bool, bool, Dict[str, Union[float, int]]]:
         """
         Takes a step in the environment by executing the given action
 
         :param a2: defender action
-        :return: (obs, reward, done, info)
+        :return: (obs, reward, terminated, truncated, info)
         """
         done, info = False, {}
 
         # Extract the attacker action
         if isinstance(a2, list):
             a2 = a2[0]
 
@@ -189,46 +218,49 @@
         self.trace.infrastructure_metrics.append(o)
         if not done:
             self.trace.attacker_observations.append(attacker_obs)
             self.trace.defender_observations.append(defender_obs)
 
         # Populate info
         info = self._info(info)
-        return attacker_obs, -r, done, info
+        return attacker_obs, -r, done, done, info
 
     def _info(self, info) -> Dict[str, Union[float, int]]:
         """
         Adds the cumulative reward and episode length to the info dict
         :param info: the info dict to update
         :return: the updated info dict
         """
         R = 0
         for i in range(len(self.trace.attacker_rewards)):
             R += self.trace.attacker_rewards[i] * math.pow(self.config.local_intrusion_response_game_config.gamma, i)
         info[env_constants.ENV_METRICS.RETURN] = R
         info[env_constants.ENV_METRICS.TIME_HORIZON] = self.state.t
         info[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = self.upper_bound_return
         info[env_constants.ENV_METRICS.AVERAGE_RANDOM_RETURN] = self.random_return
+        info[env_constants.ENV_METRICS.AVERAGE_HEURISTIC_RETURN] = self.attack_return
         return info
 
-    def reset(self, soft: bool = False) -> np.ndarray:
+    def reset(self, seed: int = 0, soft: bool = False) -> np.ndarray:
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
-        return attacker_obs
+        info = {}
+        return attacker_obs, info
 
     def render(self, mode: str = 'human'):
         """
         Renders the environment.  Supported rendering modes: (1) human; and (2) rgb_array
 
         :param mode: the rendering mode
         :return: True (if human mode) otherwise an rgb array
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,69 @@
-from typing import Tuple, List, Dict, Union
+from typing import Tuple, List, Dict, Union, Any
 import numpy as np
 import time
 import math
 import csle_common.constants.constants as constants
 from csle_common.dao.simulation_config.base_env import BaseEnv
 from csle_common.dao.simulation_config.simulation_trace import SimulationTrace
 from gym_csle_intrusion_response_game.dao.intrusion_response_game_local_pomdp_defender_config import \
     IntrusionResponseGameLocalPOMDPDefenderConfig
 from gym_csle_intrusion_response_game.util.intrusion_response_game_util import IntrusionResponseGameUtil
-from gym_csle_intrusion_response_game.dao.intrusion_response_game_state_local import IntrusionResponseGameStateLocal
 import gym_csle_intrusion_response_game.constants.constants as env_constants
 
 
-class IntrusionResponseGameLocalPOMDPDefenderEnv(BaseEnv):
+class IntrusionResponseGameLocalStoppingPOMDPDefenderEnv(BaseEnv):
     """
     OpenAI Gym Env for the POMDP of the defender when facing a static attacker.
 
-    (A PO-POSG, i.e a partially observed stochastic game with public observations) where the attacker strategy
-    is fixed)
+    (A Partially observed Dynkin game where the attacker strategy is fixed)
     """
 
     def __init__(self, config: IntrusionResponseGameLocalPOMDPDefenderConfig) -> None:
         """
         Initializes the environment
 
         :param config: the environment configuration
         """
+        a1 = config.stopping_action
+        self.zone = config.stopping_zone
+        if config is None:
+            raise ValueError("Configuration cannot be None")
         self.config = config
 
-        # Initialize environment state
-        self.state = IntrusionResponseGameStateLocal(
-            d_b1=self.config.local_intrusion_response_game_config.d_b1,
-            a_b1=self.config.local_intrusion_response_game_config.a_b1,
+        self.Z = IntrusionResponseGameUtil.local_stopping_pomdp_observation_tensor(
+            S=self.config.local_intrusion_response_game_config.S,
+            A2=self.config.local_intrusion_response_game_config.A2,
+            Z=self.config.local_intrusion_response_game_config.Z,
+            S_A=self.config.local_intrusion_response_game_config.S_A,
+            a1=a1, zone=self.zone, O=self.config.local_intrusion_response_game_config.O
+        )
+
+        self.R = IntrusionResponseGameUtil.local_stopping_pomdp_reward_tensor(
             S=self.config.local_intrusion_response_game_config.S,
+            A2=self.config.local_intrusion_response_game_config.A2,
+            R=self.config.local_intrusion_response_game_config.R[0],
             S_A=self.config.local_intrusion_response_game_config.S_A,
-            S_D=self.config.local_intrusion_response_game_config.S_D,
-            s_1_idx=self.config.local_intrusion_response_game_config.s_1_idx)
+            a1=a1, zone=self.zone)
+
+        self.T = IntrusionResponseGameUtil.local_stopping_pomdp_transition_tensor(
+            S=self.config.local_intrusion_response_game_config.S,
+            A2=self.config.local_intrusion_response_game_config.A2,
+            T=self.config.local_intrusion_response_game_config.T[0],
+            S_A=self.config.local_intrusion_response_game_config.S_A,
+            a1=a1
+        )
+
+        # Initialize environment state
+        self.s = 0
+        self.b = self.config.local_intrusion_response_game_config.d_b1
 
         # Setup spaces
-        self.observation_space = self.config.local_intrusion_response_game_config.defender_observation_space()
-        self.action_space = self.config.local_intrusion_response_game_config.defender_action_space()
+        self.observation_space = self.config.local_intrusion_response_game_config.defender_observation_space_stopping()
+        self.action_space = self.config.local_intrusion_response_game_config.defender_action_space_stopping()
 
         # Setup static attacker strategy
         self.static_attacker_strategy = self.config.attacker_strategy
 
         # Setup Config
         self.viewer = None
         self.metadata = {
@@ -51,156 +71,120 @@
             'video.frames_per_second': 50  # Video rendering speed
         }
 
         # Setup traces
         self.traces = []
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         self.latest_attacker_obs = None
+        self.latest_obs = 0
+        self.latest_a2 = 0
 
         # Reset
         self.reset()
 
         # Get upper bound and random return estimate
         self.upper_bound_return = 0
         self.random_return = 0
+        self.t = 0
+        self.intrusion_length = 0
         self.upper_bound_return = self.get_upper_bound_return(samples=100)
-        self.random_return = self.get_random_baseline_return(samples=100)
 
         # Reset
         self.reset()
         super().__init__()
 
-    def get_random_baseline_return(self, samples: int = 100) -> float:
-        """
-        Utiltiy function for estimating the average return of a random defender strategy
-
-        :param samples: the number of samples to use for estimation
-        :return: the estimated return
-        """
-        max_horizon = 1000
-        returns = []
-        for i in range(samples):
-            o = self.reset()
-            done = False
-            t = 0
-            cumulative_reward = 0
-            while not done and t <= max_horizon:
-                a1 = np.random.choice(self.config.local_intrusion_response_game_config.A1)
-                o, r, done, info = self.step(a1)
-                cumulative_reward += r * math.pow(self.config.local_intrusion_response_game_config.gamma, t)
-                t += 1
-            returns.append(cumulative_reward)
-        return np.mean(np.array(returns))
-
-    def get_upper_bound_return(self, samples: int = 100) -> float:
-        """
-        Utiltiy method for getting an upper bound on the average return
-
-        :param samples: the number of sample returns to average
-        :return: the estimated upper bound
-        """
-        max_horizon = 1000
-        returns = []
-        initial_zone = self.config.local_intrusion_response_game_config.S[
-            self.config.local_intrusion_response_game_config.s_1_idx][env_constants.STATES.D_STATE_INDEX]
-        for i in range(samples):
-            o = self.reset()
-            done = False
-            t = 0
-            cumulative_reward = 0
-            while not done and t <= max_horizon:
-                a1 = 0
-                if self.state.attacker_state() == env_constants.ATTACK_STATES.COMPROMISED:
-                    a1 = initial_zone
-                o, r, done, info = self.step(a1)
-                cumulative_reward += r * math.pow(self.config.local_intrusion_response_game_config.gamma, t)
-                t += 1
-            returns.append(cumulative_reward)
-        return np.mean(np.array(returns))
-
-    def step(self, a1: int) -> Tuple[np.ndarray, float, bool, Dict[str, Union[float, int]]]:
+    def step(self, a1: int) -> Tuple[np.ndarray, float, bool, bool, Dict[str, Union[float, int]]]:
         """
         Takes a step in the environment by executing the given action
 
         :param a1: defender action
-        :return: (obs, reward, done, info)
+        :return: (obs, reward, terminated, truncated, info)
         """
         done, info = False, {}
 
         # Extract the defender action
         if isinstance(a1, list):
             a1 = a1[0]
         a1 = int(a1)
 
         # Get attacker action from static strategy
         pi2 = np.array(self.static_attacker_strategy.stage_policy(self.latest_attacker_obs))
-        a2 = IntrusionResponseGameUtil.sample_attacker_action(pi2=pi2, s=self.state.attacker_state())
-
-        # Save current defender state (needed later for updating the belief)
-        s_d = self.state.defender_state()
+        a2 = IntrusionResponseGameUtil.sample_attacker_action(pi2=pi2, s=self.s)
+        self.latest_a2 = a2
 
         # Compute the reward
-        r = self.config.local_intrusion_response_game_config.R[0][a1][a2][self.state.s_idx]
+        r = self.R[a1][a2][self.s + 1]
 
         # Sample the next state
+        S = np.append([-1], self.config.local_intrusion_response_game_config.S_A)
         s_idx_prime = IntrusionResponseGameUtil.sample_next_state(
-            a1=a1, a2=a2, T=self.config.local_intrusion_response_game_config.T[0],
-            S=self.config.local_intrusion_response_game_config.S, s_idx=self.state.s_idx)
+            a1=a1, a2=a2, T=self.T, S=S,
+            s_idx=self.s + 1)
 
         # Sample the next observation
         o = IntrusionResponseGameUtil.sample_next_observation(
-            Z=self.config.local_intrusion_response_game_config.Z,
-            O=self.config.local_intrusion_response_game_config.O,
+            Z=self.Z, O=self.config.local_intrusion_response_game_config.O,
             s_prime_idx=s_idx_prime, a1=a1, a2=a2)
+        self.latest_obs = o
 
         # Move to the next state
-        self.state.s_idx = s_idx_prime
+        self.s = s_idx_prime - 1
 
         # Check if game is done
-        if IntrusionResponseGameUtil.is_local_state_terminal(self.state.state_vector()):
+        if self.s == -1:
+            done = True
+        if a1 == 1:
             done = True
 
         if not done:
+            # S = np.append([-1], self.config.local_intrusion_response_game_config.S_A)
+            S = self.config.local_intrusion_response_game_config.S_A
             # Update the beliefs
-            self.state.d_b = IntrusionResponseGameUtil.next_local_defender_belief(
-                o=o, a1=a1, d_b=self.state.d_b, pi2=pi2, config=self.config.local_intrusion_response_game_config,
-                a2=a2, s_a=self.state.attacker_state(),
-                s_d_prime=self.state.defender_state(), s_d=s_d)
-
-        # Update time-step
-        self.state.t += 1
+            self.b = IntrusionResponseGameUtil.next_stopping_belief(
+                o=o, a1=a1, b=self.b, pi2=pi2, S=S, Z=self.Z,
+                O=self.config.local_intrusion_response_game_config.O,
+                T=self.T,
+                A2=self.config.local_intrusion_response_game_config.A2, a2=a2, s=self.s)
+
+        # Update metrics
+        self.t += 1
+        if self.s == env_constants.ATTACK_STATES.COMPROMISED:
+            self.intrusion_length += 1
 
         # Populate info dict
-        info[env_constants.ENV_METRICS.STATE] = self.state.state_vector()
+        info[env_constants.ENV_METRICS.STATE] = self.s
         info[env_constants.ENV_METRICS.DEFENDER_ACTION] = a1
         info[env_constants.ENV_METRICS.ATTACKER_ACTION] = a2
         info[env_constants.ENV_METRICS.OBSERVATION] = o
-        info[env_constants.ENV_METRICS.TIME_STEP] = self.state.t
+        info[env_constants.ENV_METRICS.TIME_STEP] = self.t
+        info[env_constants.ENV_METRICS.INTRUSION_LENGTH] = self.intrusion_length
+        info[env_constants.ENV_METRICS.WEIGHTED_INTRUSION_PREDICTION_DISTANCE] = 0
+        info[env_constants.ENV_METRICS.START_POINT_CORRECT] = 0
+        info[env_constants.ENV_METRICS.INTRUSION_START] = 0
+        info[env_constants.ENV_METRICS.INTRUSION_END] = 0
 
         # Get observations
-        attacker_obs = self.state.attacker_observation()
-        defender_obs = self.state.defender_observation()
+        defender_obs = self.b
 
         # Log trace
         self.trace.defender_rewards.append(r)
         self.trace.attacker_rewards.append(-r)
         self.trace.attacker_actions.append(a2)
         self.trace.defender_actions.append(a1)
         self.trace.infos.append(info)
-        self.trace.states.append(self.state.s_idx)
-        self.trace.beliefs.append(self.state.d_b)
+        self.trace.states.append(self.s)
+        self.trace.beliefs.append(self.b)
         self.trace.infrastructure_metrics.append(o)
         if not done:
-            self.trace.attacker_observations.append(attacker_obs)
+            self.trace.attacker_observations.append(defender_obs)
             self.trace.defender_observations.append(defender_obs)
 
         # Populate info
         info = self._info(info)
-
-        return defender_obs, r, done, info
+        return defender_obs, r, done, done, info
 
     def _info(self, info) -> Dict[str, Union[float, int]]:
         """
         Adds the cumulative reward and episode length to the info dict
         :param info: the info dict to update
         :return: the updated info dict
         """
@@ -209,29 +193,57 @@
             R += self.trace.defender_rewards[i] * math.pow(self.config.local_intrusion_response_game_config.gamma, i)
         info[env_constants.ENV_METRICS.RETURN] = R
         info[env_constants.ENV_METRICS.TIME_HORIZON] = len(self.trace.defender_actions)
         info[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = self.upper_bound_return
         info[env_constants.ENV_METRICS.AVERAGE_RANDOM_RETURN] = self.random_return
         return info
 
-    def reset(self, soft: bool = False) -> np.ndarray:
+    def get_upper_bound_return(self, samples: int = 100) -> float:
+        """
+        Utiltiy method for getting an upper bound on the average return
+
+        :param samples: the number of sample returns to average
+        :return: the estimated upper bound
+        """
+        max_horizon = 1000
+        returns = []
+        for i in range(samples):
+            _, _ = self.reset()
+            done = False
+            t = 0
+            cumulative_reward = 0
+            while not done and t <= max_horizon:
+                a1 = 0
+                if self.s == 2:
+                    a1 = 1
+                o, r, done, _, info = self.step(a1)
+                cumulative_reward += r * math.pow(self.config.local_intrusion_response_game_config.gamma, t)
+                t += 1
+            returns.append(cumulative_reward)
+        return np.mean(np.array(returns))
+
+    def reset(self, seed: int = 0, soft: bool = False) -> Tuple[np.ndarray, Dict[str, Any]]:
         """
         Resets the environment state, this should be called whenever step() returns <done>
 
         :return: initial observation
         """
-        self.state.reset()
+        super().reset(seed=seed)
+        self.s = 0
+        self.intrusion_length = 0
+        self.b = self.config.local_intrusion_response_game_config.d_b1
         if len(self.trace.attacker_rewards) > 0:
             self.traces.append(self.trace)
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
-        attacker_obs = self.state.attacker_observation()
-        defender_obs = self.state.defender_observation()
+        attacker_obs = self.b
+        defender_obs = self.b
         self.trace.attacker_observations.append(attacker_obs)
         self.trace.defender_observations.append(defender_obs)
-        return defender_obs
+        info = {}
+        return defender_obs, info
 
     def render(self, mode: str = 'human'):
         """
         Renders the environment.  Supported rendering modes: (1) human; and (2) rgb_array
 
         :param mode: the rendering mode
         :return: True (if human mode) otherwise an rgb array
@@ -291,34 +303,35 @@
     def manual_play(self) -> None:
         """
         An interactive loop to test the environment manually
 
         :return: None
         """
         done = False
-        o = self.reset()
+        o, _ = self.reset()
         print(f"o:{list(map(lambda x: round(x, 3), list(o.tolist())))}")
         while True:
             raw_input = input("> ")
             raw_input = raw_input.strip()
             if raw_input == "help":
                 print("Enter an action id to execute the action, "
                       "press R to reset,"
                       "press S to print the state, press A to print the actions, "
                       "press D to check if done"
                       "press H to print the history of actions")
             elif raw_input == "A":
                 print(f"Action space: {self.action_space}")
             elif raw_input == "S":
-                print(self.state)
+                print(self.s)
             elif raw_input == "D":
                 print(done)
             elif raw_input == "H":
                 print(self.trace)
             elif raw_input == "R":
                 print("Resetting the state")
-                o = self.reset()
+                o, _ = self.reset()
                 print(f"o:{list(map(lambda x: round(x, 3), list(o.tolist())))}")
             else:
                 a1 = int(raw_input)
-                o, r, done, _ = self.step(a1=a1)
-                print(f"o:{list(map(lambda x: round(x, 3), list(o.tolist())))}, r:{round(r, 2)}, done: {done}")
+                o, r, done, _, _ = self.step(a1=a1)
+                print(f"o:{list(map(lambda x: round(x, 3), list(o.tolist())))}, r:{round(r, 2)}, done: {done}, "
+                      f"a1: {a1}, s:{self.s}, o:{self.latest_obs}, a2: {self.latest_a2}")
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,20 +102,20 @@
         # State metrics
         self.t = 0
 
         # Reset
         self.reset()
         super().__init__()
 
-    def step(self, a2: np.ndarray) -> Tuple[np.ndarray, float, bool, Dict[str, Union[float, int]]]:
+    def step(self, a2: np.ndarray) -> Tuple[np.ndarray, float, bool, bool, Dict[str, Union[float, int]]]:
         """
         Takes a step in the environment by executing the given action
 
         :param a1: defender action
-        :return: (obs, reward, done, info)
+        :return: (obs, reward, terminated, truncated, info)
         """
         done, info = False, {}
 
         r = 0
         attacker_obs = []
         defender_obs = []
         d_a = []
@@ -161,15 +161,15 @@
         if not done:
             self.trace.attacker_observations.append(defender_obs)
             self.trace.defender_observations.append(attacker_obs)
 
         # Populate info
         info = self._info(info)
 
-        return attacker_obs, r, done, info
+        return attacker_obs, r, done, done, info
 
     def _info(self, info) -> Dict[str, Union[float, int]]:
         """
         Adds the cumulative reward and episode length to the info dict
         :param info: the info dict to update
         :return: the updated info dict
         """
@@ -178,35 +178,37 @@
             R += self.trace.defender_rewards[i] * math.pow(self.config.game_config.gamma, i)
         info[env_constants.ENV_METRICS.RETURN] = R
         info[env_constants.ENV_METRICS.TIME_HORIZON] = len(self.trace.defender_actions)
         info[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = self.upper_bound_return
         info[env_constants.ENV_METRICS.AVERAGE_RANDOM_RETURN] = self.random_return
         return info
 
-    def reset(self, soft: bool = False) -> np.ndarray:
+    def reset(self, seed: int = 0, soft: bool = False) -> np.ndarray:
         """
         Resets the environment state, this should be called whenever step() returns <done>
 
         :return: initial observation
         """
+        super().reset(seed=seed)
         self.t = 0
         attacker_obs = []
         defender_obs = []
         for local_env in self.local_envs:
             local_o = local_env.reset()
             attacker_obs = attacker_obs + local_o.tolist()
             defender_obs = defender_obs + local_env.trace.defender_observations[-1].tolist()
         attacker_obs = np.array(attacker_obs)
         defender_obs = np.array(defender_obs)
         if len(self.trace.defender_rewards) > 0:
             self.traces.append(self.trace)
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         self.trace.attacker_observations.append(defender_obs)
         self.trace.defender_observations.append(attacker_obs)
-        return attacker_obs
+        info = {}
+        return attacker_obs, info
 
     def render(self, mode: str = 'human'):
         """
         Renders the environment.  Supported rendering modes: (1) human; and (2) rgb_array
 
         :param mode: the rendering mode
         :return: True (if human mode) otherwise an rgb array
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,33 +29,32 @@
         Initializes the environment
 
         :param config: the environment configuration
         """
         self.config = config
         self.local_envs = []
         for node in config.game_config.nodes:
-            reachable = True
+            reachable = self.reachable(node)
             S = IntrusionResponseGameUtil.local_state_space(number_of_zones=len(self.config.game_config.zones))
             states_to_idx = {}
             for i, s in enumerate(S):
                 states_to_idx[(s[env_constants.STATES.D_STATE_INDEX], s[env_constants.STATES.A_STATE_INDEX])] = i
             S_A = IntrusionResponseGameUtil.local_attacker_state_space()
             S_D = IntrusionResponseGameUtil.local_defender_state_space(
                 number_of_zones=len(self.config.game_config.zones))
             A1 = IntrusionResponseGameUtil.local_defender_actions(number_of_zones=len(self.config.game_config.zones))
             A2 = IntrusionResponseGameUtil.local_attacker_actions()
             O = IntrusionResponseGameUtil.local_observation_space(X_max=self.config.game_config.X_max)
             T = np.array([IntrusionResponseGameUtil.local_transition_tensor(
                 S=S, A1=A1, A2=A2, Z_D=self.config.game_config.Z_D_P, A_P=self.config.game_config.A_P)])
             Z = IntrusionResponseGameUtil.local_observation_tensor_betabinom(S=S, A1=A1, A2=A2, O=O)
-            Z_U = np.array([0, 1, 3, 3.5, 4])
             R = np.array(
                 [IntrusionResponseGameUtil.local_reward_tensor(
                     eta=self.config.game_config.eta, C_D=self.config.game_config.C_D, A1=A1, A2=A2,
-                    reachable=reachable, beta=self.config.game_config.beta, S=S, Z_U=Z_U,
+                    reachable=reachable, beta=self.config.game_config.beta, S=S, Z_U=self.config.game_config.Z_U,
                     initial_zone=self.config.game_config.initial_zones[node])])
             d_b1 = IntrusionResponseGameUtil.local_initial_defender_belief(S_A=S_A)
             a_b1 = IntrusionResponseGameUtil.local_initial_attacker_belief(
                 S_D=S_D, initial_zone=self.config.game_config.initial_zones[node])
             initial_state = [self.config.game_config.initial_zones[node], 0]
             initial_state_idx = states_to_idx[(initial_state[env_constants.STATES.D_STATE_INDEX],
                                                initial_state[env_constants.STATES.A_STATE_INDEX])]
@@ -89,47 +88,48 @@
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         self.latest_attacker_obs = None
 
         # Reset
         self.reset()
 
         # Get upper bound and random return estimate
-        self.upper_bound_return = 0
-        self.random_return = 0
-        for env in self.local_envs:
-            self.upper_bound_return += env.upper_bound_return
-            self.random_return += env.random_return
+        self.upper_bound_return = self.get_upper_bound_return(samples=100)
+        self.random_return = self.get_random_baseline_return(samples=100)
 
         # State metrics
         self.t = 0
 
         # Reset
         self.reset()
         super().__init__()
 
-    def step(self, a1: np.ndarray) -> Tuple[np.ndarray, float, bool, Dict[str, Union[float, int]]]:
+    def step(self, a1: np.ndarray) -> Tuple[np.ndarray, float, bool, bool, Dict[str, Union[float, int]]]:
         """
         Takes a step in the environment by executing the given action
 
         :param a1: defender action
-        :return: (obs, reward, done, info)
+        :return: (obs, reward, terminated, truncated, info)
         """
         done, info = False, {}
 
         r = 0
         defender_obs = []
         attacker_obs = []
         d_b = []
         s = []
         a2 = []
 
         # Step the envs
         for i, local_env in enumerate(self.local_envs):
+            reachable = self.reachable(i)
             local_a1 = a1[i]
-            local_o, local_r, local_done, _ = local_env.step(a1=local_a1)
+            local_o, local_r, local_done, _, _ = local_env.step(a1=local_a1)
+            if not reachable:
+                local_r = local_env.config.local_intrusion_response_game_config.C_D[local_a1]
+                local_o = np.array([local_o[0], 1, 0, 0])
             if local_done:
                 done = True
             r = r + local_r
             defender_obs = defender_obs + local_o.tolist()
             s = s + local_env.state.state_vector().tolist()
             a2.append(local_env.trace.attacker_actions[-1])
             attacker_obs = attacker_obs + local_env.trace.attacker_observations[-1].tolist()
@@ -161,15 +161,99 @@
         if not done:
             self.trace.attacker_observations.append(attacker_obs)
             self.trace.defender_observations.append(defender_obs)
 
         # Populate info
         info = self._info(info)
 
-        return defender_obs, r, done, info
+        return defender_obs, r, done, done, info
+
+    def get_upper_bound_return(self, samples: int = 100) -> float:
+        """
+        Utiltiy method for getting an upper bound on the average return
+
+        :param samples: the number of sample returns to average
+        :return: the estimated upper bound
+        """
+        max_horizon = 200
+        returns = []
+        for i in range(samples):
+            o, _ = self.reset()
+            done = False
+            t = 0
+            cumulative_reward = 0
+            while not done and t <= max_horizon:
+                r = 0
+                for i, local_env in enumerate(self.local_envs):
+                    reachable = self.reachable(i)
+                    local_a1 = 0
+                    if reachable and local_env.state.attacker_state() == env_constants.ATTACK_STATES.COMPROMISED:
+                        local_a1 = 3
+                    local_o, local_r, local_done, _, _ = local_env.step(a1=local_a1)
+                    if not reachable:
+                        local_r = 0
+                    if local_done:
+                        done = True
+                    r = r + local_r
+                cumulative_reward += r * math.pow(self.config.game_config.gamma, t)
+                t += 1
+            returns.append(cumulative_reward)
+        return np.mean(np.array(returns))
+
+    def get_random_baseline_return(self, samples: int = 100) -> float:
+        """
+        Utiltiy method for getting the average return of a random strategy
+
+        :param samples: the number of sample returns to average
+        :return: the estimated upper bound
+        """
+        max_horizon = 200
+        returns = []
+        for i in range(samples):
+            o, _ = self.reset()
+            done = False
+            t = 0
+            cumulative_reward = 0
+            while not done and t <= max_horizon:
+                r = 0
+                for i, local_env in enumerate(self.local_envs):
+                    reachable = self.reachable(i)
+                    local_a1 = np.random.choice(local_env.config.local_intrusion_response_game_config.A1)
+                    local_o, local_r, local_done, _, _ = local_env.step(a1=local_a1)
+                    if not reachable:
+                        local_r = 0
+                    if local_done:
+                        done = True
+                    r = r + local_r
+                cumulative_reward += r * math.pow(self.config.game_config.gamma, t)
+                t += 1
+            returns.append(cumulative_reward)
+        return np.mean(np.array(returns))
+
+    def reachable(self, node: int) -> bool:
+        """
+        Checks if a node is reachable from the gw
+
+        :param node: the node to check
+        :return: True if reachable otherwise False
+        """
+        num_nodes = len(self.config.game_config.nodes)
+        A = self.config.game_config.adjacency_matrix.copy()
+        for i, local_env in enumerate(self.local_envs):
+            if local_env.state.defender_state() in [env_constants.DEFENDER_STATES.SHUTDOWN,
+                                                    env_constants.DEFENDER_STATES.REDIRECT]:
+                A[i] = [0] * num_nodes
+        gw_reachable_nodes = self.config.game_config.gw_reachable
+        A = np.array(A)
+        for i in range(1, num_nodes + 1):
+            A_n = np.linalg.matrix_power(A, i)
+            for gw_reachable in gw_reachable_nodes:
+                if A_n[gw_reachable][node] != 0:
+                    return True
+        return False
 
     def _info(self, info) -> Dict[str, Union[float, int]]:
         """
         Adds the cumulative reward and episode length to the info dict
         :param info: the info dict to update
         :return: the updated info dict
         """
@@ -178,35 +262,37 @@
             R += self.trace.defender_rewards[i] * math.pow(self.config.game_config.gamma, i)
         info[env_constants.ENV_METRICS.RETURN] = R
         info[env_constants.ENV_METRICS.TIME_HORIZON] = len(self.trace.defender_actions)
         info[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = self.upper_bound_return
         info[env_constants.ENV_METRICS.AVERAGE_RANDOM_RETURN] = self.random_return
         return info
 
-    def reset(self, soft: bool = False) -> np.ndarray:
+    def reset(self, seed: int = 0, soft: bool = False) -> np.ndarray:
         """
         Resets the environment state, this should be called whenever step() returns <done>
 
         :return: initial observation
         """
+        super().reset(seed=seed)
         self.t = 0
         defender_obs = []
         attacker_obs = []
         for local_env in self.local_envs:
-            local_o = local_env.reset()
+            local_o, _ = local_env.reset()
             defender_obs = defender_obs + local_o.tolist()
             attacker_obs = attacker_obs + local_env.trace.attacker_observations[-1].tolist()
         defender_obs = np.array(defender_obs)
         attacker_obs = np.array(attacker_obs)
         if len(self.trace.defender_rewards) > 0:
             self.traces.append(self.trace)
         self.trace = SimulationTrace(simulation_env=self.config.env_name)
         self.trace.attacker_observations.append(attacker_obs)
         self.trace.defender_observations.append(defender_obs)
-        return defender_obs
+        info = {}
+        return defender_obs, info
 
     def render(self, mode: str = 'human'):
         """
         Renders the environment.  Supported rendering modes: (1) human; and (2) rgb_array
 
         :param mode: the rendering mode
         :return: True (if human mode) otherwise an rgb array
@@ -266,15 +352,15 @@
     def manual_play(self) -> None:
         """
         An interactive loop to test the environment manually
 
         :return: None
         """
         done = False
-        o = self.reset()
+        o, _ = self.reset()
         print(f"o:{list(map(lambda x: round(x, 3), list(o.tolist())))}")
         while True:
             raw_input = input("> ")
             raw_input = raw_input.strip()
             if raw_input == "help":
                 print("Enter an action id to execute the action, "
                       "press R to reset,"
@@ -287,13 +373,13 @@
                 print(self.state)
             elif raw_input == "D":
                 print(done)
             elif raw_input == "H":
                 print(self.trace)
             elif raw_input == "R":
                 print("Resetting the state")
-                o = self.reset()
+                o, _ = self.reset()
                 print(f"o:{list(map(lambda x: round(x, 3), list(o.tolist())))}")
             else:
                 a1 = np.array(list(map(lambda x: int(x), raw_input.split(","))))
-                o, r, done, _ = self.step(a1=a1)
+                o, r, done, _, _ = self.step(a1=a1)
                 print(f"o:{list(map(lambda x: round(x, 3), list(o.tolist())))}, r:{round(r, 2)}, done: {done}")
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from scipy.stats import betabinom
 from gym_csle_intrusion_response_game.dao.local_intrusion_response_game_config import LocalIntrusionResponseGameConfig
 import gym_csle_intrusion_response_game.constants.constants as env_constants
+from csle_common.dao.training.policy import Policy
 
 
 class IntrusionResponseGameUtil:
     """
     Class with utility functions for the intrusion response game environment
     """
 
@@ -27,14 +28,26 @@
         :param s: the local state to check
         :param zone: the zone to check
         :return: True if the state is in the given zone, false otherwise
         """
         return s[env_constants.STATES.D_STATE_INDEX] == zone
 
     @staticmethod
+    def is_local_state_shutdown_or_redirect(s: np.ndarray) -> bool:
+        """
+        Utility function for checking if a local node is in shutdown or redirect state
+
+        :param s: the local state to check
+        :param zone: the zone to check
+        :return: True if the node is in shutdown or redirect state, otherwise fasle
+        """
+        return (s[env_constants.STATES.D_STATE_INDEX] == env_constants.DEFENDER_STATES.SHUTDOWN
+                and s[env_constants.STATES.D_STATE_INDEX] == env_constants.DEFENDER_STATES.REDIRECT)
+
+    @staticmethod
     def is_local_state_compromised(s: np.ndarray) -> bool:
         """
         Utility function for checking if a local state has been compromised
 
         :param s: the local state to check
         :return: True if compromised, otherwise False
         """
@@ -248,15 +261,15 @@
         :return: the workflow utility
         """
         impact = 0
         if reachable and not IntrusionResponseGameUtil.is_local_state_compromised(s) and \
                 not s[env_constants.STATES.D_STATE_INDEX] in [env_constants.ZONES.SHUTDOWN_ZONE,
                                                               env_constants.ZONES.REDIRECTION_ZONE]:
             impact = 1
-        return beta * impact * int(IntrusionResponseGameUtil.is_local_state_in_zone(s=s, zone=initial_zone))
+        return beta * impact * int(not IntrusionResponseGameUtil.is_local_state_shutdown_or_redirect(s=s))
 
     @staticmethod
     def constant_defender_action_costs(A1: np.ndarray, constant_cost: float) -> np.ndarray:
         """
         Returns a vector with the local defender action costs where each action has the same constant cost
 
         :param A1: a vector with the actions of the defender in the local game
@@ -342,73 +355,160 @@
         :param s: the current state
         :param Z_U: the vector with zone utilities
         :return: the intrusion cost
         """
         if not reachable or s[env_constants.STATES.D_STATE_INDEX] == env_constants.ZONES.SHUTDOWN_ZONE:
             return D_C[a1]  # No intrusion cost if the node is not reachable
         compromised = int((s[env_constants.STATES.A_STATE_INDEX] == env_constants.ATTACK_STATES.COMPROMISED))
-        return Z_U[s[env_constants.STATES.D_STATE_INDEX] - 1] * compromised + D_C[a1]
+        if compromised:
+            return Z_U[s[env_constants.STATES.D_STATE_INDEX] - 1]
+        else:
+            return D_C[a1]
 
     @staticmethod
     def local_defender_utility_function(s: np.ndarray, a1: int, eta: float, reachable: bool, initial_zone: int,
-                                        beta: float, C_D: np.ndarray, Z_U: np.ndarray):
+                                        beta: float, C_D: np.ndarray, Z_U: np.ndarray, topology_cost: float = 0):
         """
         The local utility function of the defender
 
         :param s: the current state of the local game
         :param a1: the defender action
         :param eta: a scaling parameter to balance QoS and security
         :param reachable: a boolean flag indicating whether the node is reachable from the public gateway or not
         :param initial_zone: the initial zone of the node in the local game
         :param beta: a scaling parameter indicating the importance of the workflow of the local game
         :param C_D: the vector with the costs of the local defender actions
         :param Z_U: the utilities of the zones in the network
+        :param topology_cost: extra topology cost
         :return: the utility of the defender
         """
         if IntrusionResponseGameUtil.is_local_state_terminal(s):
             return 0
         workflow_utility = IntrusionResponseGameUtil.local_workflow_utility(beta=beta, reachable=reachable, s=s,
                                                                             initial_zone=initial_zone)
         intrusion_cost = IntrusionResponseGameUtil.local_intrusion_cost(a1=a1, D_C=C_D, reachable=reachable, s=s,
                                                                         Z_U=Z_U)
-        return eta * workflow_utility - (1 - eta) * intrusion_cost
+        if s[env_constants.STATES.D_STATE_INDEX] not in [0, 1]:
+            topology_cost = 0
+        return eta * workflow_utility - (1 - eta) * intrusion_cost - topology_cost
 
     @staticmethod
     def local_reward_tensor(eta: float, C_D: np.ndarray, reachable: bool, Z_U: np.ndarray, initial_zone: int,
-                            beta: float, S: np.ndarray, A1: np.ndarray, A2: np.ndarray) -> np.ndarray:
+                            beta: float, S: np.ndarray, A1: np.ndarray, A2: np.ndarray,
+                            topology_cost: float = 0) -> np.ndarray:
         """
         Gets the defender's utility tensor of the local version of the game
 
         :param eta: a scaling parameter for the local rewards
         :param C_D: the vector with the costs of the local defender actions
         :param reachable: a boolean flag indicating whether the node of the local game is reachable or not
         :param Z_U: the vector with utilities of the different zones in the network
         :param initial_zone: the initial zone of the node
         :param beta: a scaling parameter for the workflow utility
         :param S: the local state space of the game
         :param A1: the local action space of the defender
-        :param A2: teh local action space of the attacker
+        :param A2: the local action space of the attacker
+        :param topology_cost: extra topology costs
         :return: a (A1)(A2)(S) tensor giving the rewards of the state transitions in the local game
         """
         R = []
         for a1 in A1:
             a1_rews = []
             for a2 in A2:
                 a1_a2_rews = []
                 for s in S:
                     a1_a2_rews.append(IntrusionResponseGameUtil.local_defender_utility_function(
                         s=s, a1=a1, eta=eta, reachable=reachable, initial_zone=initial_zone,
-                        beta=beta, C_D=C_D, Z_U=Z_U
+                        beta=beta, C_D=C_D, Z_U=Z_U, topology_cost=topology_cost
                     ))
                 a1_rews.append(a1_a2_rews)
             R.append(a1_rews)
         R = np.array(R)
         return R
 
     @staticmethod
+    def local_stopping_mdp_reward_tensor(S: np.ndarray, A1: np.ndarray, A2: np.ndarray,
+                                         R: np.ndarray, S_D: np.ndarray) -> np.ndarray:
+        R_1 = []
+        S_D = np.append([-1], S_D)
+        for a1 in A1:
+            if a1 == 0:
+                continue
+            a1_rews = []
+            for a2 in A2:
+                a1_a2_rews = []
+                for s in S_D:
+                    r = 0
+                    for i, full_s in enumerate(S):
+                        if full_s[env_constants.STATES.D_STATE_INDEX] == s and \
+                                full_s[env_constants.STATES.A_STATE_INDEX] == env_constants.ATTACK_STATES.COMPROMISED:
+                            r = R[a1][a2][i]
+                    a1_a2_rews.append(r)
+                a1_rews.append(a1_a2_rews)
+            R_1.append(a1_rews)
+        R_1 = np.array(R_1)
+        return R_1
+
+    @staticmethod
+    def local_stopping_pomdp_reward_tensor(S: np.ndarray, A2: np.ndarray,
+                                           R: np.ndarray, S_A: np.ndarray,
+                                           a1: int, zone: int) -> np.ndarray:
+        R_1 = []
+        S_A = np.append([-1], S_A)
+        for stop in [0, 1]:
+            a1_rews = []
+            for a2 in A2:
+                a1_a2_rews = []
+                for s in S_A:
+                    r = 0
+                    for i, full_s in enumerate(S):
+                        if full_s[env_constants.STATES.A_STATE_INDEX] == s \
+                                and full_s[env_constants.STATES.D_STATE_INDEX] == zone:
+                            # print(f"match, s_a: {s}, i:{i}, full_s:{full_s}")
+                            if stop == 1:
+                                r = R[a1][a2][i]
+                            else:
+                                r = R[0][a2][i]
+                    a1_a2_rews.append(r)
+                a1_rews.append(a1_a2_rews)
+            R_1.append(a1_rews)
+        R_1 = np.array(R_1)
+        return R_1
+
+    @staticmethod
+    def local_stopping_pomdp_observation_tensor(S: np.ndarray, A2: np.ndarray, S_A: np.ndarray,
+                                                Z: np.ndarray, a1: int, zone: int,
+                                                O: np.ndarray) -> np.ndarray:
+        Z_1 = []
+        S_A = np.append([-1], S_A)
+        for stop in [0, 1]:
+            a1_obs_probs = []
+            for a2 in A2:
+                a1_a2_obs_probs = []
+                for s in S_A:
+                    obs_prob = []
+                    for i, full_s_prime in enumerate(S):
+                        if full_s_prime[env_constants.STATES.A_STATE_INDEX] == s \
+                                and full_s_prime[env_constants.STATES.D_STATE_INDEX] == zone:
+                            if stop == 1:
+                                obs_prob = Z[a1][a2][i]
+                            else:
+                                obs_prob = Z[0][a2][i]
+                    if len(obs_prob) == 0:
+                        obs_prob = np.zeros(len(O)).tolist()
+                        obs_prob[0] = 1
+                    else:
+                        obs_prob = obs_prob.tolist()
+                    a1_a2_obs_probs.append(obs_prob)
+                a1_obs_probs.append(a1_a2_obs_probs)
+            Z_1.append(a1_obs_probs)
+        Z_1 = np.array(Z_1)
+        return Z_1
+
+    @staticmethod
     def local_transition_probability(s: np.ndarray, s_prime: np.ndarray, a1: int, a2: int, Z_D_P: np.ndarray,
                                      A_P: np.ndarray):
         """
         Gets the probability of a local state transition
 
         :param s: the current state
         :param s_prime: the next  state
@@ -439,17 +539,16 @@
                     and IntrusionResponseGameUtil.is_local_state_healthy(s=s_prime):
                 return 1 * P_not_detected
             else:
                 return 0
         else:
             # Defender did not take defensive action
 
-            # If the node is shutdown or traffic redirect, the state remains the same
-            if s[env_constants.STATES.D_STATE_INDEX] in [env_constants.ZONES.SHUTDOWN_ZONE,
-                                                         env_constants.ZONES.REDIRECTION_ZONE]:
+            # If the node is shutdown, the state remains the same
+            if s[env_constants.STATES.D_STATE_INDEX] in [env_constants.ZONES.SHUTDOWN_ZONE]:
                 if IntrusionResponseGameUtil.are_local_states_equal(s=s, s_prime=s_prime):
                     return 1 * P_not_detected
                 else:
                     return 0
 
             # If attacker waits, then the state remains the same
             if a2 == env_constants.ATTACKER_ACTIONS.WAIT:
@@ -549,14 +648,104 @@
                     a1_a2_probs.append(a1_a2_s_probs)
                 a1_probs.append(a1_a2_probs)
             T.append(a1_probs)
         T = np.array(T)
         return T
 
     @staticmethod
+    def local_stopping_mdp_transition_tensor(S: np.ndarray, A1: np.ndarray,
+                                             A2: np.ndarray, T: np.ndarray, S_D: np.ndarray) -> np.ndarray:
+        """
+        Gets the transition tensor for the local MDP of the stopping decomposition in the temporal domain
+
+        :param S: the full state space of the local problem
+        :param A1: the defender's action space in the local problem
+        :param A2: the attacker's action space in the local problem
+        :param T: the full transition tensor of the local problem
+        :param S_D: the defender's state spce
+        :return: the transition tensor for the local MDP of the stopping formulation
+        """
+        S_D = np.append([-1], S_D)
+        T_1 = []
+        for a1 in A1:
+            if a1 == 0:
+                continue
+            a1_probs = []
+            for a2 in A2:
+                a1_a2_probs = []
+                for s in S_D:
+                    a1_a2_s_probs = []
+                    for s_prime in S_D:
+                        prob = 0
+                        total_prob = 0
+                        for i, full_s in enumerate(S):
+                            for j, full_s_prime in enumerate(S):
+                                if full_s[env_constants.STATES.D_STATE_INDEX] == s:
+                                    total_prob += T[a1][a2][i][j]
+                                if full_s[env_constants.STATES.D_STATE_INDEX] == s \
+                                        and full_s_prime[env_constants.STATES.D_STATE_INDEX] == s_prime:
+                                    prob += T[a1][a2][i][j]
+                        prob = prob / total_prob
+                        prob = min(1, prob)
+                        a1_a2_s_probs.append(prob)
+                    assert round(sum(a1_a2_s_probs), 3) == 1
+                    a1_a2_probs.append(a1_a2_s_probs)
+                a1_probs.append(a1_a2_probs)
+            T_1.append(a1_probs)
+        T_1 = np.array(T_1)
+        return T_1
+
+    @staticmethod
+    def local_stopping_pomdp_transition_tensor(S: np.ndarray, A2: np.ndarray, T: np.ndarray, S_A: np.ndarray,
+                                               a1: int) -> np.ndarray:
+        """
+        Gets the transition tensor for the local POMDP of the stopping decomposition in the temporal domain
+
+        :param S: the full state space of the local problem
+        :param A1: the defender's action space in the local problem
+        :param A2: the attacker's action space in the local problem
+        :param T: the full transition tensor of the local problem
+        :param S_D: the defender's state spce
+        :return: the transition tensor for the local MDP of the stopping formulation
+        """
+        S_A = np.append([-1], S_A)
+        T_1 = []
+        for stop in [0, 1]:
+            stop_probs = []
+            for a2 in A2:
+                a1_a2_probs = []
+                for s in S_A:
+                    a1_a2_s_probs = []
+                    for s_prime in S_A:
+                        if a1 == 1:
+                            if s_prime == -1:
+                                a1_a2_s_probs.append(1)
+                            else:
+                                a1_a2_s_probs.append(0)
+                        else:
+                            prob = 0
+                            total_prob = 0
+                            for i, full_s in enumerate(S):
+                                for j, full_s_prime in enumerate(S):
+                                    if full_s[env_constants.STATES.A_STATE_INDEX] == s:
+                                        total_prob += T[a1][a2][i][j]
+                                    if full_s[env_constants.STATES.A_STATE_INDEX] == s \
+                                            and full_s_prime[env_constants.STATES.A_STATE_INDEX] == s_prime:
+                                        prob += T[stop][a2][i][j]
+                            prob = prob / total_prob
+                            # prob=min(1, prob)
+                            a1_a2_s_probs.append(prob)
+                    assert round(sum(a1_a2_s_probs), 3) == 1
+                    a1_a2_probs.append(a1_a2_s_probs)
+                stop_probs.append(a1_a2_probs)
+            T_1.append(stop_probs)
+        T_1 = np.array(T_1)
+        return T_1
+
+    @staticmethod
     def local_observation_tensor_betabinom(S: np.ndarray, A1: np.ndarray, A2: np.ndarray, O: np.ndarray):
         """
         Gets the observation tensor of the local game where the observations follow beta-binomial distributions
 
         :param S: the local state space of the game
         :param A1: the local action space of the defender
         :param A2: the local action space of the attacker
@@ -813,7 +1002,172 @@
                     (config.Z[a1][a2][s_prime_idx][o]
                      * config.T[0][a1][a2][s_idx][s_prime_idx] * a_b[s_d] * pi1[s_d][a1])
         b_prime_s_prime = temp / norm
         if round(b_prime_s_prime, 2) > 1:
             print(f"b_prime_s_prime >= 1: {b_prime_s_prime}, a2:{a2}, s_prime:{s_a_prime}, o:{o}, pi1:{pi1}")
         assert round(b_prime_s_prime, 2) <= 1
         return b_prime_s_prime
+
+    @staticmethod
+    def get_local_defender_pomdp_solver_file(S: np.ndarray, A1: np.ndarray, A2: np.ndarray,
+                                             O: np.ndarray, R: np.ndarray, T: np.ndarray,
+                                             static_attacker_strategy: Policy,
+                                             s_1_idx: int, discount_factor: float = 0.99) -> str:
+        """
+        Gets the POMDP environment specification based on the format at http://www.pomdp.org/code/index.html,
+        for the defender's local problem against a static attacker
+
+        :param S: the state spaec
+        :param A1: the defender's local action space
+        :param A2: the attacker's local action space
+        :param O: the observation space
+        :param R: the reward tensor
+        :param T: the transition tensor
+        :param static_attacker_strategy: the static attacker opponent strategy
+        :param s_1_idx: the initial state index
+        :param discount_factor: the discount  factor
+        :return: the file content string
+        """
+        file_str = ""
+        file_str = file_str + f"discount: {discount_factor}\n\n"
+        file_str = file_str + "values: reward\n\n"
+        file_str = file_str + f"states: {len(S)}\n\n"
+        file_str = file_str + f"actions: {len(A1)}\n\n"
+        file_str = file_str + f"observations: {len(O)}\n\n"
+        initial_belief = [0] * len(S)
+        initial_belief[s_1_idx] = 1
+        initial_belief_str = " ".join(list(map(lambda x: str(x), initial_belief)))
+        file_str = file_str + f"start: {initial_belief_str}\n\n\n"
+        T = T[0]
+        num_transitions = 0
+        for s in range(len(S)):
+            for a1 in range(len(A1)):
+                probs = []
+                for s_prime in range(len(S)):
+                    num_transitions += 1
+                    prob = 0
+                    pi2 = np.array(static_attacker_strategy.stage_policy(None))[
+                        S[s][env_constants.STATES.A_STATE_INDEX]]
+                    for a2 in range(len(A2)):
+                        prob += pi2[a2] * T[a1][a2][s][s_prime]
+                    file_str = file_str + f"T: {a1} : {s} : {s_prime} {prob}\n"
+                    probs.append(prob)
+                assert round(sum(probs), 3) == 1
+        file_str = file_str + "\n\n"
+        for s_prime in range(len(S)):
+            for a1 in range(len(A1)):
+                total_transition_prob = 0
+                a2_transition_probs = np.zeros(len(A2))
+                for s in range(len(S)):
+                    pi2 = np.array(static_attacker_strategy.stage_policy(None))[
+                        S[s][env_constants.STATES.A_STATE_INDEX]]
+                    for a2 in range(len(A2)):
+                        total_transition_prob += pi2[a2] * T[a1][a2][s][s_prime]
+                        a2_transition_probs[a2] += T[a1][a2][s][s_prime] * pi2[a2]
+                probs = []
+                for o in range(len(O)):
+                    prob = 0
+                    if total_transition_prob == 0:
+                        prob = (1 / len(O))
+                    else:
+                        for a2 in range(len(A2)):
+                            a2_prob = (a2_transition_probs[a2]) / total_transition_prob
+                            prob += a2_prob * Z[a1][a2][s_prime][o]
+                    file_str = file_str + f"O : {a1} : {s_prime} : {o} {prob}\n"
+                    probs.append(prob)
+                assert round(sum(probs), 3) == 1
+        file_str = file_str + "\n\n"
+
+        for s in range(len(S)):
+            for a1 in range(len(A1)):
+                for s_prime in range(len(S)):
+                    pi2 = np.array(static_attacker_strategy.stage_policy(None))[
+                        S[s][env_constants.STATES.A_STATE_INDEX]]
+                    for o in range(len(O)):
+                        r = 0
+                        for a2 in range(len(A2)):
+                            r += pi2[a2] * R[0][a1][a2][s]
+                        file_str = file_str + f"R: {a1} : {s} : {s_prime} : {o} {r}\n"
+        return file_str
+
+    @staticmethod
+    def stopping_bayes_filter(s_prime: int, o: int, a1: int, b: np.ndarray, pi2: np.ndarray,
+                              S: np.ndarray, Z: np.ndarray, T: np.ndarray, A2: np.ndarray,
+                              O: np.ndarray) -> float:
+        """
+        A Bayesian filter to compute the belief of player 1
+        of being in s_prime when observing o after taking action a in belief b given that the opponent follows
+        strategy pi2
+
+        :param s_prime: the state to compute the belief of
+        :param o: the observation
+        :param a1: the action of player 1
+        :param b: the current belief point
+        :param pi2: the policy of player 2
+        :param l: stops remaining
+        :return: b_prime(s_prime)
+        """
+        norm = 0
+        for s in S:
+            for a2 in A2:
+                for s_prime_1 in S:
+                    prob_1 = Z[a1][a2][s_prime_1 + 1][o]
+                    norm += b[s] * prob_1 * T[a1][a2][s + 1][s_prime_1 + 1] * pi2[s][a2]
+        if norm == 0:
+            print(f"zero norm, s_prime:{s_prime}, o:{o}, a1:{a1}, b:{b}")
+            return 0
+        temp = 0
+
+        for s in S:
+            for a2 in A2:
+                temp += Z[a1][a2][s_prime + 1][o] * T[a1][a2][s + 1][s_prime + 1] * b[s] * pi2[s][a2]
+        b_prime_s_prime = temp / norm
+        if round(b_prime_s_prime, 3) > 1:
+            print(f"b_prime_s_prime >= 1: {b_prime_s_prime}, a1:{a1}, s_prime:{s_prime}, o:{o}, pi2:{pi2}")
+        assert round(b_prime_s_prime, 3) <= 1
+        return b_prime_s_prime
+
+    @staticmethod
+    def stopping_p_o_given_b_a1_a2(o: int, b: np.ndarray, a1: int, a2: int, S: np.ndarray, Z: np.ndarray,
+                                   T: np.ndarray) -> float:
+        """
+        Computes P[o|a,b]
+
+        :param o: the observation
+        :param b: the belief point
+        :param a1: the action of player 1
+        :param a2: the action of player 2
+        :param config: the game config
+        :return: the probability of observing o when taking action a in belief point b
+        """
+        prob = 0
+        for s in S:
+            for s_prime in S:
+                prob += b[s] * T[a1][a2][s][s_prime] * Z[a1][a2][s_prime][o]
+        assert prob < 1
+        return prob
+
+    @staticmethod
+    def next_stopping_belief(o: int, a1: int, b: np.ndarray, pi2: np.ndarray, S: np.ndarray,
+                             Z: np.ndarray, O: np.ndarray, T: np.ndarray, A2: np.ndarray,
+                             a2: int = 0, s: int = 0) -> np.ndarray:
+        """
+        Computes the next belief using a Bayesian filter
+
+        :param o: the latest observation
+        :param a1: the latest action of player 1
+        :param b: the current belief
+        :param pi2: the policy of player 2
+        :param config: the game config
+        :param a2: the attacker action (for debugging, should be consistent with pi2)
+        :param s: the true state (for debugging)
+        :return: the new belief
+        """
+        b_prime = np.zeros(len(S))
+        for s_prime in S:
+            b_prime[s_prime] = IntrusionResponseGameUtil.stopping_bayes_filter(s_prime=s_prime, o=o, a1=a1, b=b,
+                                                                               pi2=pi2, S=S, Z=Z, T=T, A2=A2, O=O)
+        if round(sum(b_prime), 2) != 1:
+            print(f"error, b_prime:{b_prime}, o:{o}, a1:{a1}, b:{b}, pi2:{pi2}, "
+                  f"a2: {a2}, s:{s}")
+        assert round(sum(b_prime), 2) == 1
+        return b_prime
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-intrusion-response-game
-Version: 0.1.9
+Version: 0.2.0
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt` & `gym_csle_intrusion_response_game-0.2.0/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
 src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
 src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
 src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
 src/gym_csle_intrusion_response_game/envs/__init__.py
 src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
 src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
+src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py
 src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
 src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
 src/gym_csle_intrusion_response_game/util/__init__.py
 src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
```

