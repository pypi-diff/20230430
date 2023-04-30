# Comparing `tmp/rewards_envs-0.0.1.tar.gz` & `tmp/rewards_envs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards_envs-0.0.1.tar", max compression
+gzip compressed data, was "rewards_envs-0.1.1.tar", max compression
```

## Comparing `rewards_envs-0.0.1.tar` & `rewards_envs-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0        0 2023-04-15 15:47:23.913921 rewards_envs-0.0.1/README.md
--rw-r--r--   0        0        0      511 2023-04-17 05:29:38.887892 rewards_envs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      135 2023-04-17 06:21:29.126919 rewards_envs-0.0.1/rewards_envs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 00:19:10.993914 rewards_envs-0.0.1/rewards_envs/engines/pygame/__init__.py
--rw-r--r--   0        0        0      192 2023-04-17 00:21:43.549724 rewards_envs-0.0.1/rewards_envs/engines/pygame/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-04-16 21:50:07.050409 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/__init__.py
--rw-r--r--   0        0        0      201 2023-04-17 00:21:43.549724 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    11016 2023-04-17 11:25:17.135216 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/__pycache__/car_race.cpython-310.pyc
--rw-r--r--   0        0        0    79384 2023-04-16 21:35:27.215637 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/car.png
--rw-r--r--   0        0        0    86212 2023-04-16 17:18:48.777957 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/evaluation/track-1.png
--rw-r--r--   0        0        0    60297 2023-04-16 17:19:04.354021 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/training/track-1.png
--rw-r--r--   0        0        0    42293 2023-04-16 17:19:04.362021 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/training/track-2.png
--rw-r--r--   0        0        0    49467 2023-04-16 17:19:04.374021 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/training/track-3.png
--rw-r--r--   0        0        0    13850 2023-04-17 11:25:04.903054 rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/car_race.py
--rw-r--r--   0        0        0        0 2023-04-17 00:20:23.669824 rewards_envs-0.0.1/rewards_envs/envs/__init__.py
--rw-r--r--   0        0        0      861 2023-04-17 05:26:34.551963 rewards_envs-0.0.1/rewards_envs/envs/car_race.py
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 rewards_envs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3938 2023-04-30 04:46:56.839050 rewards_envs-0.1.1/README.md
+-rw-r--r--   0        0        0      494 2023-04-30 09:48:53.439936 rewards_envs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      358 2023-04-26 15:08:12.400096 rewards_envs-0.1.1/rewards_envs/__init__.py
+-rw-r--r--   0        0        0     5739 2023-04-26 15:05:38.551575 rewards_envs-0.1.1/rewards_envs/core.py
+-rw-r--r--   0        0        0        0 2023-04-17 00:19:10.993914 rewards_envs-0.1.1/rewards_envs/engines/pygame/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-17 00:21:43.549724 rewards_envs-0.1.1/rewards_envs/engines/pygame/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-04-16 21:50:07.050409 rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/__init__.py
+-rw-r--r--   0        0        0    79384 2023-04-16 21:35:27.215637 rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/car.png
+-rw-r--r--   0        0        0    86212 2023-04-16 17:18:48.777957 rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/evaluation/track-1.png
+-rw-r--r--   0        0        0    60297 2023-04-16 17:19:04.354021 rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/training/track-1.png
+-rw-r--r--   0        0        0    42293 2023-04-16 17:19:04.362021 rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/training/track-2.png
+-rw-r--r--   0        0        0    49467 2023-04-16 17:19:04.374021 rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/training/track-3.png
+-rw-r--r--   0        0        0    15375 2023-04-26 14:41:52.489234 rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/car_race.py
+-rw-r--r--   0        0        0        0 2023-04-17 00:20:23.669824 rewards_envs-0.1.1/rewards_envs/envs/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-26 10:13:49.307527 rewards_envs-0.1.1/rewards_envs/envs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2834 2023-04-26 10:16:20.204393 rewards_envs-0.1.1/rewards_envs/envs/__pycache__/car_race.cpython-310.pyc
+-rw-r--r--   0        0        0     1538 2023-04-30 04:06:14.667259 rewards_envs-0.1.1/rewards_envs/envs/car_race.py
+-rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 rewards_envs-0.1.1/PKG-INFO
```

### Comparing `rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/car.png` & `rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/car.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/evaluation/track-1.png` & `rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/evaluation/track-1.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/training/track-1.png` & `rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/training/track-1.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/training/track-2.png` & `rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/training/track-2.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/assets/training/track-3.png` & `rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/assets/training/track-3.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.0.1/rewards_envs/engines/pygame/car_race/car_race.py` & `rewards_envs-0.1.1/rewards_envs/engines/pygame/car_race/car_race.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
 Copyright (c) rewards.ai 
 
 This program mainly serves as the pygame engine for the car environment. 
 User can either use it to play the game or use it to the rewards environment. 
 There are some sets of methods and attributes that are fixed here:
 
-from rewards_envs.engine.pygame import CarGame 
-
 TODO:
 -----
 - Able to add more tracks 
-- Add the functionality to play the game in the human mode 
+- Add the functionality to play the game in the human mode. Current version has some bugs in 
+`human` mode 
 """
 
 import os
 import math
 import pygame
 from pathlib import Path
 import matplotlib.pyplot as plt
 from pydantic import BaseModel, Field
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, SupportsFloat
 
 
 class CarConfig(BaseModel):
     car_scale: int = Field(default=500)
     drive_factor: int = Field(default=12)
     car_fps: int = Field(default=15)
     car_angle: int = Field(default=0)
@@ -120,39 +119,48 @@
         # current observation space 
         self.params = {
             "is_alive": None,
             "observation": None,
             "direction": None,
             "rotational_velocity": None,
         }
+        
+        self.info =  {
+            'direction' : self.direction,
+            'rotational_velocity' : self.rotation_vel
+        }
         print("=> Game initialization finished")
         
     def _default_reward_function(self, props: Dict[str, Any]) -> Union[int, float]:
         if props["is_alive"]:
             return 1
         return 0
     
-    def initialize(self) -> None:
+    def initialize(self) -> Union[List[float], Dict[str, Any]]:
         """
         Initializes the car environment with all the default properties
         
-        TODO: 
-            Should we also initialize the observation space ?
+        Returns:
+            info : List[List[float], Dict[str, Any]]. A List that returns the current environment state and the current environment information. 
         """
         self.angle = self.config.car_angle
         self.original_image = self.car_image
         self.image = pygame.transform.rotozoom(self.original_image, self.angle, 0.1)
         self.rect = self.image.get_rect(center=self.config.car_rect_size)
         self.vel_vector = pygame.math.Vector2(self.config.car_velocity_vector)
         self.rotation_vel = self.config.car_rotational_velocity
         self.direction = self.config.car_direction
         self.drive_factor = self.config.drive_factor
         self.alive = self.config.car_is_alive
         self.radars = self.config.car_radar
         self.reward = 0
+
+        self.info['direction'] = self.direction
+        self.info['rotational_velocity'] = self.rotation_vel
+        return self.radars, self.info 
         
         
     def _did_quit(self):
         """
         Quits the game when user presses the 'quit'/'close' key.
         """
         for event in pygame.event.get():
@@ -354,15 +362,44 @@
             "direction": self.direction,
             "rotational_velocity": self.rotation_vel,
         }
 
         return self.params
 
     
-    def play_step(self, action: List[str]) -> List[Any]:
+    def step(self, action: List[int]) -> List[Any]:
+        """
+        Plays a single step of the game. This function is called by the agent during each step.
+        Current version of rewards-envs does not provides `info` of that given step. However,it 
+        will be supported in the future versions. 
+
+        Args:
+            action (List[int]): The current action of the agent
+
+        Returns:
+            List[Any]: [observation, reward, terminated, info]
+        """
+        self.iterations += 1
+        if self.config.render_mode == "human":
+            self._did_quit()
+        self.draw()
+        self.radars = [0, 0, 0, 0, 0]
+        self._drive()
+        
+        current_state_params = self.get_current_state(action=action)
+        current_reward = self.reward_function(current_state_params)
+        self.reward += current_reward
+        
+        observation = current_state_params['observation']
+        terminated = current_state_params['is_alive']
+        return observation, self.reward, terminated, self.info 
+
+    
+    # TODO: Needs to deprecated soon in the next major release
+    def play_step(self, action: List[int]) -> List[Any]:
         """
         Plays a single step of the game. This function is called by the agent during each step.
 
         Args:
             action (List[int]): The current action of the agent
 
         Returns:
@@ -382,10 +419,11 @@
         self.reward += current_reward
 
         if self.config.render_mode == "rgb_array":
             pixel_data = pygame.surfarray.array3d(self.screen)
             return current_reward, not self.alive, self.reward, pixel_data
         else:
             return current_reward, not self.alive, self.reward
+    
 
 if __name__ == '__main__':
     car_game = CarGame(mode="training", track_num=1)
```

