# Comparing `tmp/reticuler-0.4.tar.gz` & `tmp/reticuler-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reticuler-0.4.tar", last modified: Tue Dec 20 11:31:03 2022, max compression
+gzip compressed data, was "reticuler-1.0.tar", last modified: Sun Apr 30 21:33:50 2023, max compression
```

## Comparing `reticuler-0.4.tar` & `reticuler-1.0.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 11:31:03.236000 reticuler-0.4/
--rw-rw-rw-   0        0        0     1097 2022-11-09 13:08:57.000000 reticuler-0.4/LICENSE
--rw-rw-rw-   0        0        0     2396 2022-12-20 11:31:03.212000 reticuler-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2022-11-28 08:05:01.000000 reticuler-0.4/README.md
--rw-rw-rw-   0        0        0      962 2022-12-20 11:30:21.000000 reticuler-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-20 11:31:03.227000 reticuler-0.4/setup.cfg
--rw-rw-rw-   0        0        0       91 2022-11-02 22:21:50.000000 reticuler-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-20 11:31:02.545000 reticuler-0.4/src/
-drwxrwxrwx   0        0        0        0 2022-12-20 11:31:02.795000 reticuler-0.4/src/reticuler/
--rw-rw-rw-   0        0        0       65 2022-11-23 12:02:56.000000 reticuler-0.4/src/reticuler/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 11:31:03.137000 reticuler-0.4/src/reticuler/extending_kernels/
--rw-rw-rw-   0        0        0       93 2022-11-23 12:02:56.000000 reticuler-0.4/src/reticuler/extending_kernels/__init__.py
--rw-rw-rw-   0        0        0     7968 2022-12-20 11:26:55.000000 reticuler-0.4/src/reticuler/extending_kernels/extenders.py
--rw-rw-rw-   0        0        0    16677 2022-12-20 11:26:55.000000 reticuler-0.4/src/reticuler/extending_kernels/pde_solvers.py
--rw-rw-rw-   0        0        0     5125 2022-12-20 11:26:55.000000 reticuler-0.4/src/reticuler/extending_kernels/trajectory_integrators.py
--rw-rw-rw-   0        0        0     3572 2022-11-23 12:02:56.000000 reticuler-0.4/src/reticuler/plot_ret.py
--rw-rw-rw-   0        0        0     7606 2022-12-20 11:26:55.000000 reticuler-0.4/src/reticuler/reticulate.py
--rw-rw-rw-   0        0        0    26835 2022-12-20 11:26:55.000000 reticuler-0.4/src/reticuler/system.py
-drwxrwxrwx   0        0        0        0 2022-12-20 11:31:03.200000 reticuler-0.4/src/reticuler/user_interface/
--rw-rw-rw-   0        0        0       24 2022-11-23 12:02:56.000000 reticuler-0.4/src/reticuler/user_interface/__init__.py
--rw-rw-rw-   0        0        0     2328 2022-12-19 09:44:50.000000 reticuler-0.4/src/reticuler/user_interface/graphics.py
-drwxrwxrwx   0        0        0        0 2022-12-20 11:31:02.955000 reticuler-0.4/src/reticuler.egg-info/
--rw-rw-rw-   0        0        0     2396 2022-12-20 11:31:02.000000 reticuler-0.4/src/reticuler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2022-12-20 11:31:02.000000 reticuler-0.4/src/reticuler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 11:31:02.000000 reticuler-0.4/src/reticuler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2022-12-20 11:31:02.000000 reticuler-0.4/src/reticuler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2022-12-20 11:31:02.000000 reticuler-0.4/src/reticuler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-20 11:31:02.000000 reticuler-0.4/src/reticuler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 21:33:50.827000 reticuler-1.0/
+-rw-rw-rw-   0        0        0     1097 2022-11-09 13:08:57.000000 reticuler-1.0/LICENSE
+-rw-rw-rw-   0        0        0     2396 2023-04-30 21:33:50.763000 reticuler-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2022-11-28 08:05:01.000000 reticuler-1.0/README.md
+-rw-rw-rw-   0        0        0     1112 2023-04-28 10:05:25.000000 reticuler-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 21:33:50.802000 reticuler-1.0/setup.cfg
+-rw-rw-rw-   0        0        0       91 2022-11-02 22:21:50.000000 reticuler-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:33:48.399000 reticuler-1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 21:33:49.036000 reticuler-1.0/src/reticuler/
+-rw-rw-rw-   0        0        0      100 2023-04-28 10:12:46.000000 reticuler-1.0/src/reticuler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:33:49.723000 reticuler-1.0/src/reticuler/backward_evolution/
+-rw-rw-rw-   0        0        0       53 2023-04-28 10:06:15.000000 reticuler-1.0/src/reticuler/backward_evolution/__init__.py
+-rw-rw-rw-   0        0        0    15255 2023-04-30 20:39:35.000000 reticuler-1.0/src/reticuler/backward_evolution/system_back.py
+-rw-rw-rw-   0        0        0    13312 2023-04-30 20:39:49.000000 reticuler-1.0/src/reticuler/backward_evolution/trimmers.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:33:50.040000 reticuler-1.0/src/reticuler/extending_kernels/
+-rw-rw-rw-   0        0        0       93 2022-11-23 12:02:56.000000 reticuler-1.0/src/reticuler/extending_kernels/__init__.py
+-rw-rw-rw-   0        0        0     8831 2023-04-27 13:36:32.000000 reticuler-1.0/src/reticuler/extending_kernels/extenders.py
+-rw-rw-rw-   0        0        0    16736 2023-04-27 13:33:53.000000 reticuler-1.0/src/reticuler/extending_kernels/pde_solvers.py
+-rw-rw-rw-   0        0        0     4906 2023-04-27 14:20:25.000000 reticuler-1.0/src/reticuler/extending_kernels/trajectory_integrators.py
+-rw-rw-rw-   0        0        0    26823 2023-04-28 16:01:04.000000 reticuler-1.0/src/reticuler/system.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:33:50.714000 reticuler-1.0/src/reticuler/user_interface/
+-rw-rw-rw-   0        0        0       48 2023-04-28 09:54:46.000000 reticuler-1.0/src/reticuler/user_interface/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-28 12:37:49.000000 reticuler-1.0/src/reticuler/user_interface/clip_ret.py
+-rw-rw-rw-   0        0        0     2815 2023-04-28 09:44:01.000000 reticuler-1.0/src/reticuler/user_interface/clippers.py
+-rw-rw-rw-   0        0        0     2313 2023-04-28 12:40:36.000000 reticuler-1.0/src/reticuler/user_interface/graphics.py
+-rw-rw-rw-   0        0        0     3574 2023-04-28 13:16:15.000000 reticuler-1.0/src/reticuler/user_interface/plot_ret.py
+-rw-rw-rw-   0        0        0     7618 2022-12-20 11:49:09.000000 reticuler-1.0/src/reticuler/user_interface/reticulate.py
+-rw-rw-rw-   0        0        0     3755 2023-04-30 20:39:06.000000 reticuler-1.0/src/reticuler/user_interface/reticulate_back.py
+drwxrwxrwx   0        0        0        0 2023-04-30 21:33:49.479000 reticuler-1.0/src/reticuler.egg-info/
+-rw-rw-rw-   0        0        0     2396 2023-04-30 21:33:47.000000 reticuler-1.0/src/reticuler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2023-04-30 21:33:48.000000 reticuler-1.0/src/reticuler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 21:33:47.000000 reticuler-1.0/src/reticuler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-30 21:33:48.000000 reticuler-1.0/src/reticuler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-04-30 21:33:48.000000 reticuler-1.0/src/reticuler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-30 21:33:48.000000 reticuler-1.0/src/reticuler.egg-info/top_level.txt
```

### Comparing `reticuler-0.4/LICENSE` & `reticuler-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reticuler-0.4/PKG-INFO` & `reticuler-1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reticuler
-Version: 0.4
+Version: 1.0
 Summary: Simulations of spatial networks growth
 Author: Stanisław Żukowski
 Author-email: zukowski.st@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/stzukowski/reticuler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reticuler Version: 0.4 Summary: Simulations of
+Metadata-Version: 2.1 Name: reticuler Version: 1.0 Summary: Simulations of
 spatial networks growth Author: StanisÅaw Å»ukowski Author-email:
 zukowski.st@gmail.com License: MIT Project-URL: Source, https://github.com/
 stzukowski/reticuler Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # Reticuler
                [PyPI] [Documentation_Status] [Code_style:_black]
```

### Comparing `reticuler-0.4/README.md` & `reticuler-1.0/README.md`

 * *Files identical despite different names*

### Comparing `reticuler-0.4/pyproject.toml` & `reticuler-1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 include = ["reticuler*"]  # package names should match these glob patterns (["*"] by default)
 
 [project]
 name = "reticuler"
-version = "0.4"
+version = "1.0"
 authors = [
 	{name="Stanisław Żukowski"},
 	{email="zukowski.st@gmail.com"}
 ]
 description = "Simulations of spatial networks growth"
 readme = "README.md"
 license = { text = "MIT" }
@@ -27,9 +27,11 @@
     "matplotlib >= 3.6",
 	]
 
 [project.urls]
 "Source" = "https://github.com/stzukowski/reticuler"
 
 [project.scripts]
-reticulate = "reticuler.reticulate:main"
-plot_ret = "reticuler.plot_ret:main"
+reticulate = "reticuler.user_interface.reticulate:main"
+reticulate_back = "reticuler.user_interface.reticulate_back:main"
+plot_ret = "reticuler.user_interface.plot_ret:main"
+clip_ret = "reticuler.user_interface.clip_ret:main"
```

### Comparing `reticuler-0.4/src/reticuler/extending_kernels/extenders.py` & `reticuler-1.0/src/reticuler/extending_kernels/extenders.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Streamline:
     """Extender based on the streamline algorithm [Ref1]_.
 
     Attributes
     ----------
-    pde_solver : object of one of the classes from pde_solvers
+    pde_solver : PDESolver
     eta : float, default 1.0
         The growth exponent (v=a1**eta).
         High values increase competition between the branches.
         Low values stabilize the growth.
     ds : float, default 0.01
         A distance over which the fastest branch in the network
         will move in each timestep.
@@ -37,27 +37,29 @@
         of max flux/velocity.
     distance_from_bif_thresh : float, default 2.1*``ds``
         A minimal distance the tip has to move from the previous bifurcations
         to split again.
 
     References
     ----------
-    .. [Ref1] "Through history to growth dynamics -- backward evolution of spatial networks",
-            S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak (2022)
+    .. [Ref1] "Through history to growth dynamics: backward evolution of spatial networks",
+            S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci Rep 12, 20407 (2022). 
+            https://doi.org/10.1038/s41598-022-24656-x
 
     """
 
     def __init__(
         self,
         pde_solver,
         eta=1.0,
         ds=0.01,
         bifurcation_type=0,
         bifurcation_thresh=0,
         bifurcation_angle=2 * np.pi / 5,
+        inflow_thresh=0.05
     ):
         """Initialize Streamline.
 
         Parameters
         ----------
         pde_solver : object of class pde_solvers
         eta : float, default 1.0
@@ -84,17 +86,16 @@
             if self.bifurcation_type == 2:
                 self.bifurcation_thresh = -0.1  # a3/a1 bifurcations
             if self.bifurcation_type == 3:
                 self.bifurcation_thresh = 3 * ds
                 # random bifurcations: bif_probability
         self.bifurcation_angle = bifurcation_angle  # 2*np.pi/5
 
-        self.inflow_thresh = (
-            0.05  # less than 5% of max flux/velocity puts branches asleep
-        )
+        # less than `inflow_thresh` of max flux/velocity puts branches asleep
+        self.inflow_thresh = inflow_thresh
         self.distance_from_bif_thresh = 2.1 * ds
 
     def __rotation_matrix(self, angle):
         """Construct a matrix to rotate a vector by an ``angle``.
 
         Parameters
         ----------
@@ -113,16 +114,25 @@
         """
         return np.array(
             [[np.cos(angle), np.sin(angle)], [-np.sin(angle), np.cos(angle)]]
         )
 
     def check_bifurcation_and_moving_conditions(self, network):
         """Check bifurcation and moving conditions."""
-        max_a1 = np.max(self.pde_solver.a1a2a3_coefficients[..., 0])
-        for i, branch in enumerate(network.active_branches):
+
+        a1 = self.pde_solver.a1a2a3_coefficients[..., 0]
+        max_a1 = np.max(a1)
+        # checking which branches are_moving
+        # (first condition for low eta, second for high)
+        are_moving = np.logical_and(a1/max_a1 > self.inflow_thresh,
+                                    (a1/max_a1)**self.eta > self.inflow_thresh)
+
+        # shallow copy of active_branches (creates new list instance, but the elements are still the same)
+        branches_to_iterate = network.active_branches.copy()
+        for i, branch in enumerate(branches_to_iterate):
             a1 = self.pde_solver.a1a2a3_coefficients[i, 0]
             a3 = self.pde_solver.a1a2a3_coefficients[i, 2]
             if (
                 self.bifurcation_type
                 and branch.length() > self.distance_from_bif_thresh
             ):
                 # the second condition above is used to avoid many bifurcations
@@ -132,22 +142,21 @@
                 ):
                     branch.is_bifurcating = True
                 elif self.bifurcation_type == 3:
                     p = self.bifurcation_thresh * (a1 / max_a1) ** self.eta
                     r = np.random.uniform(0, 1)  # uniform distribution [0,1)
                     if p > r:
                         branch.is_bifurcating = True
+                        
+            if not are_moving[i]:
+                network.sleeping_branches.append(branch)
+                network.active_branches.remove(branch)
+                print("! Branch {ID} is sleeping !".format(ID=branch.ID))
 
-            # checking if branch is_moving
-            # (first condition for low eta, second for high)
-            if (
-                a1 < self.inflow_thresh * max_a1
-                or a1**self.eta < self.inflow_thresh * max_a1**self.eta
-            ):
-                branch.is_moving = False
+        return are_moving
 
     def __streamline_extension(self, beta, dr):
         """Calculate a vector over which the tip is shifted.
 
         Derived from the fact that the finger proceeds along a unique
         streamling going through the tip.
 
@@ -162,22 +171,23 @@
         -------
         dR : array
             An 1-2 array.
 
         """
         if np.abs(beta) < 1000:
             y = ((beta**2) / 9) * ((27 * dr / (2 * beta**2) + 1) ** (2 / 3) - 1)
-        else: 
-            y = dr - (9*dr**2)/(4*beta**2) + (27*dr**3)/(2*beta**4) - (1701*dr**4)/(16*beta**6)
-        x = np.around( \
-                      np.sign(beta) * 2 * ((y**3 / beta**2) + \
-                                           (y / beta) ** 4) ** (1 / 2), 7)
+        else:
+            y = dr - (9*dr**2)/(4*beta**2) + (27*dr**3) / \
+                (2*beta**4) - (1701*dr**4)/(16*beta**6)
+        x = np.around(
+            np.sign(beta) * 2 * ((y**3 / beta**2) +
+                                 (y / beta) ** 4) ** (1 / 2), 9)                                                      
         return np.array([x, y])
 
-    def find_test_dRs(self, network):
+    def find_test_dRs(self, network, is_BEA_off):
         """Find a single test shift over which the tip is moving.
 
         Parameters
         ----------
         network : object of class Network
 
         Returns
@@ -186,37 +196,45 @@
             An n-2 array with dx and dy shifts for each tip.
 
         """
         # running PDE solver
         # self.pde_solver.a1a2a3_coefficients are updated in FreeFEM solver
         self.pde_solver.solve_PDE(network)
 
+        # dr_norm = 1, ds <=> dt
+        dr_norm = 1
+        if is_BEA_off:
+            # normalize dr, so that the fastest tip moves over ds
+            dr_norm = np.max(self.pde_solver.a1a2a3_coefficients[..., 0] ** self.eta)
         dRs_test = np.empty((len(network.active_branches), 2))
         for i, branch in enumerate(network.active_branches):
             a1 = self.pde_solver.a1a2a3_coefficients[i, 0]
             a2 = self.pde_solver.a1a2a3_coefficients[i, 1]
             beta = a1 / a2
 
             # __streamline_extension formula is derived in the coordinate
             # system where the tip segment lies on a negative Y axis;
             # hence, we rotate obtained dR vector to that system
             tip_angle = branch.tip_angle()
-            dr = self.ds * a1**self.eta
+            dr = self.ds * a1**self.eta / dr_norm
             dRs_test[i] = np.dot(
-                self.__rotation_matrix(tip_angle), self.__streamline_extension(beta, dr)
+                self.__rotation_matrix(
+                    tip_angle), self.__streamline_extension(beta, dr)
             )
         return dRs_test
 
-    def assign_dRs(self, dRs, network):
+    def assign_dRs(self, network, dRs):
         """Assign ``dRs`` to each branch in ``network``."""
         for i, branch in enumerate(network.active_branches):
             if branch.is_bifurcating:
                 branch.dR = [
-                    np.dot(self.__rotation_matrix(-self.bifurcation_angle / 2), dRs[i]),
-                    np.dot(self.__rotation_matrix(self.bifurcation_angle / 2), dRs[i]),
+                    np.dot(
+                        self.__rotation_matrix(-self.bifurcation_angle / 2), dRs[i]),
+                    np.dot(self.__rotation_matrix(
+                        self.bifurcation_angle / 2), dRs[i]),
                 ]
             else:
                 branch.dR = dRs[i]
 
 
 # class Royal:
 #     def __init__(self, solver)
```

### Comparing `reticuler-0.4/src/reticuler/extending_kernels/pde_solvers.py` & `reticuler-1.0/src/reticuler/extending_kernels/pde_solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os.path
 import os
 from tempfile import NamedTemporaryFile
 import textwrap
 
 
 class FreeFEM:
-    """PDE solver based on finite element method implemented in FreeFEM [Ref2]_.
+    """PDE solver based on the finite element method implemented in FreeFEM [Ref2]_.
 
     Attributes
     ----------
     equation : int, default 0
         - 0: Laplace
         - 1: Poisson
     a1a2a3_coefficients : array
@@ -405,15 +405,15 @@
         print("stdout:", result.stdout.decode())
         print("stderr:", result.stderr.decode())
         if result.returncode:
             print("\nFreeFem++ failed.\n")
 
         ai_coeffs_flat = np.fromstring(result.stdout, sep=",")
         self.a1a2a3_coefficients = ai_coeffs_flat.reshape(len(ai_coeffs_flat) // 3, 3)
-        print(self.a1a2a3_coefficients)
+        # print(self.a1a2a3_coefficients)
 
     def solve_PDE(self, network):
         """Solve the PDE for the field around the network.
 
         Prepare a FreeFEM script, export it to a temporary file and run.
         Then, import the a1a2a3 coefficients to ``self.a1a2a3_coefficients``.
 
@@ -426,7 +426,8 @@
         -------
         None.
 
         """
         script = self.__prepare_script(network)
         self.__run_freefem_temp(script)
         # self.__run_freefem(script) # useful for debugging
+        # print('a1a2a3: ', self.a1a2a3_coefficients)
```

### Comparing `reticuler-0.4/src/reticuler/extending_kernels/trajectory_integrators.py` & `reticuler-1.0/src/reticuler/extending_kernels/trajectory_integrators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Functions to integrate the tips trajectory.
+"""Classes to integrate tip trajectories.
 
-Functions:
-    modified_euler(extender, network, max_approximation_step=3)
+Classes:
+    ModifiedEulerMethod
 
 """
 
 import numpy as np
 
 
 class ModifiedEulerMethod:
@@ -47,15 +47,15 @@
         """Move test tips (no bifurcations or killing).
 
         Assign ``dRs`` to each branch in ``network.active_branches`` and extend them.
 
         """
         for i, branch in enumerate(network.active_branches):
             branch.dR = dRs[i]
-            branch.extend_by_dR()
+            branch.extend()
 
     def integrate(self, extender, network, is_BEA_off=True):
         """Integrate tip trajectories with modified Euler's method.
     
         Parameters
         ----------
         extender : Extender
@@ -69,29 +69,26 @@
     
         Returns
         -------
         dt : float
             Time of growth at the current evolution step.
         a1a2a3_coefficients_0 : array
             An array of a_i coefficients for each tip in the network.
-            Not returned if is_BEA_off.
     
         """
         # x[n + 1] = x[n] + dt * v[x(n)]: finding position n+1 with explicit Euler
-        dRs_0 = extender.find_test_dRs(network)
-        if is_BEA_off:
-            # normalize, so that the fastest tip moves over ds
-            dRs_0 = dRs_0 / np.max(np.linalg.norm(dRs_0, axis=1)) * extender.ds
-        else:
-            # here we want to move over dt as in the backward step,
-            # so no normalization
-            a1a2a3_coefficients_0 = extender.pde_solver.a1a2a3_coefficients_0
+        dRs_0 = extender.find_test_dRs(network, is_BEA_off)
+        
+        # in the BEA we want to move over dt as in the backward step,
+        # so no normalization
+        a1a2a3_coefficients_0 = extender.pde_solver.a1a2a3_coefficients
             
-        # checking if each branch is_moving or is_bifurcating
-        extender.check_bifurcation_and_moving_conditions(network)
+        # checking if branches are_moving or each branch.is_bifurcating
+        are_moving = extender.check_bifurcation_and_moving_conditions(network)
+        dRs_0 = dRs_0[are_moving]
         # print('a1, a2, a3:\n',extender.pde_solver.a1a2a3_coefficients)
     
         # moving test_system by dRs_0
         test_network = network.copy()
         self.move_test_tips(test_network, dRs_0)
     
         dRs_test = 0
@@ -102,35 +99,32 @@
         epsilon = epsilon_thresh + 1
         # APPROXIMATION LOOP - we end when approximating isn't getting any
         # better (epsilon is the measure) or after 'max_approximation_step' steps
         while epsilon > epsilon_thresh and approximation_step < self.max_approximation_step:
             approximation_step = approximation_step + 1
     
             # v[ x(n+1)] ]: finding velocity at the next point
-            dRs_1 = extender.find_test_dRs(test_network)
-    
+            dRs_1 = extender.find_test_dRs(test_network, is_BEA_off)
+            
             # calculating approximation error and average dR
-            epsilon = np.sum(np.linalg.norm(dRs_test - (dRs_0 + dRs_1) / 2, axis=1)) / len(
-                dRs_0
-            )
+            epsilon = np.sum(np.linalg.norm(dRs_test - \
+                            (dRs_0 + dRs_1) / 2, axis=1)) / len(dRs_0)
             dRs_test = (dRs_0 + dRs_1) / 2
             if is_BEA_off:
-                # normalize
                 dRs_test = dRs_test * extender.ds / np.max(np.linalg.norm(dRs_test, axis=1))
-    
+                
             # moving test_system by dR
             test_network = network.copy()
             self.move_test_tips(test_network, dRs_test)
-    
+            
             # print('Forth loop, approximation step: {step}, epsilon = {eps}'.format(step=approximation_step, eps=epsilon) )
-    
-        extender.assign_dRs(dRs_test, network)
-        
         if is_BEA_off:
             # normally division dX/a1^eta would give single dt
             # due to the modified Euler's algorithm (dR = (dRs_0+dRs_1)/2 )
             # dt is not perfectly the same for different tips, so we take a mean
             dt = np.mean( np.linalg.norm(dRs_test, axis=1) / extender.pde_solver.a1a2a3_coefficients[...,0]**extender.eta)
-            return dt
         else: 
             dt = extender.ds
-            return dt, a1a2a3_coefficients_0
+        
+        extender.assign_dRs(network, dRs_test)
+        
+        return dt, a1a2a3_coefficients_0
```

### Comparing `reticuler-0.4/src/reticuler/plot_ret.py` & `reticuler-1.0/src/reticuler/user_interface/plot_ret.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from reticuler.system import System
 from reticuler.user_interface import graphics
 
 # %%
 def main():
     parser = argparse.ArgumentParser(
-        description="Grow a network.", formatter_class=argparse.RawTextHelpFormatter
+        description="Plot a network.", formatter_class=argparse.RawTextHelpFormatter
     )
 
     # defining arguments for parser object
     parser.add_argument(
         "input_file",
         type=str,
         nargs=1,
@@ -30,31 +30,31 @@
         "--output_file",
         type=str,
         nargs=1,
         metavar="file_name",
         help=textwrap.dedent(
             """\
                             File to export. If None the same as input.
-                            default = '' """
+                            default = None """
         ),
         default=None,
     )
 
     parser.add_argument(
         "-out_ext",
         "--output_extension",
         type=str,
         nargs=1,
         metavar="ext",
         help=textwrap.dedent(
             """\
                             Output extension ('.pdf', '.svg', '.png', etc.)
-                            default = '.pdf' """
+                            default = '.jpg' """
         ),
-        default=[".pdf"],
+        default=[".jpg"],
     )
 
     # Plotting options
     parser.add_argument(
         "--ylim",
         type=float,
         nargs=1,
```

### Comparing `reticuler-0.4/src/reticuler/reticulate.py` & `reticuler-1.0/src/reticuler/user_interface/reticulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,17 @@
         "--trajectory_integrator",
         type=str,
         nargs=1,
         metavar="name",
         help=textwrap.dedent(
             """\
             Trajectory integrator
-            default = modified_euler"""
+            default = ModifiedEulerMethod"""
         ),
-        default=["modified_euler"],
+        default=["ModifiedEulerMethod"],
     )
 
     # Solver
     parser.add_argument(
         "--pde_solver",
         type=str,
         nargs=1,
@@ -234,15 +234,15 @@
         )
 
         # Network
         network = Network(box=box, branches=branches, active_branches=branches.copy())
 
         # Trajectory integrator
         if args.trajectory_integrator[0] == "ModifiedEulerMethod":
-            trajectory_integrator = trajectory_integrators.ModifiedEulerMethod
+            trajectory_integrator = trajectory_integrators.ModifiedEulerMethod()
 
         # Solver
         if args.pde_solver[0] == "FreeFEM":
             pde_solver = pde_solvers.FreeFEM(**args.pde_solver_params[0])
 
         # Extender
         if args.extender[0] == "Streamline":
```

### Comparing `reticuler-0.4/src/reticuler/system.py` & `reticuler-1.0/src/reticuler/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import copy
 import json
 import importlib.metadata
 
 from .extending_kernels import extenders, pde_solvers, trajectory_integrators
 
 
-class _NumpyEncoder(json.JSONEncoder):
+class NumpyEncoder(json.JSONEncoder):
     """Special json encoder for numpy types.
 
     References
     ----------
     .. [1] https://stackoverflow.com/questions/26646362/numpy-array-is-not-json-serializable
     """
 
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()
+        if isinstance(obj, np.int32): 
+            return int(obj)
         return json.JSONEncoder.default(self, obj)
 
 
 class Branch:
     """A class of a single branch in a network.
 
     Attributes
@@ -45,17 +47,14 @@
     steps : array
         A 1-n array with evolution steps at which corresponding points were added.
     dR : array or 0, default 0
         A 1-2 array of tip progression ([dx, dy]).
     is_bifurcating : bool, default False
         A boolean condition if branch is bifurcating or not.
         (Based on the bifurcation_type and bifurcation_thresh from extender.)
-    is_moving : bool, default True
-        A boolean condition if branch is moving further or not
-        (Based on the inflow_thresh from extender.)
 
     """
 
     def __init__(self, ID, points, steps):
         """Initialize Branch.
 
         Parameters
@@ -72,44 +71,39 @@
         self.ID = ID
 
         self.points = points  # in order of creation
         self.steps = steps  # at which step of the evolution the point was added
 
         self.dR = 0
         self.is_bifurcating = False
-        self.is_moving = True
 
-    def extend_by_dR(self):
+    def extend(self):
         """Add a new point to ``self.points`` (progressed tip)."""
         self.points = np.vstack((self.points, self.points[-1] + self.dR))
 
     def length(self):
         """Return length of the Branch."""
-        return np.sum(
-            np.linalg.norm((np.roll(self.points, -1, axis=0) - self.points), axis=1)[
-                :-1
-            ]
-        )
+        return np.sum(np.linalg.norm(self.points[1:]-self.points[:-1], axis=1))
 
     def tip_angle(self):
-        """Return angle between the tip segment (last and penultimate point) and Y axis."""
+        """Return the angle between the tip segment (last and penultimate point) and Y axis."""
         point_penult = self.points[-2]
         point_last = self.points[-1]
         dx = point_last[0] - point_penult[0]
         dy = point_last[1] - point_penult[1]
         return np.pi / 2 - np.arctan2(dy, dx)
 
     def points_steps(self):
         """Return a 3-n array of points and evolution steps when they were added."""
         return np.column_stack((self.points, self.steps))
 
 
 class Box:
     """A class containing borders of the simulation domain.
-    
+
     Attributes
     ----------
     points : array, default []
         A 2-n array with xy coordinates of the points composing the Box.
     connections : array, default []
         A 2-n array with connections between the ``points``.
     boundary_conditions : array, default []
@@ -118,19 +112,19 @@
             - 1: absorbing BC (vanishing field)
             - 2: reflective BC (vanishing normal derivative)
             - 3: constant flux
     seeds_connectivity : array, default []
         A 2-n array of seeds connectivity.
             - 1st column: index in ``points``
             - 2nd column: outgoing branch ``ID`` 
-        
+
     """
 
     def __init__(
-        self, points=[], connections=[], boundary_conditions=[], seeds_connectivity=[]
+        self, points, connections, boundary_conditions, seeds_connectivity
     ):
         """Initialize Box.
 
         Parameters
         ----------
         points : array, default []
         connections : array, default []
@@ -138,22 +132,22 @@
         seeds_connectivity : array, default []
 
         Returns
         -------
         None.
 
         """
-        self.points = points
+        self.points = points # [] if points is None else points
         self.connections = connections
         self.boundary_conditions = boundary_conditions
 
         # 1st column: index on border
         # 2nd column: branch_id
         self.seeds_connectivity = seeds_connectivity
-
+        
     def __add_points(self, points):
         if not len(self.points):
             self.points = points
         else:
             self.points = np.vstack((self.points, points))
 
     def __add_connection(self, connections, boundary_conditions):
@@ -174,15 +168,15 @@
         (1st/2nd column - point indices, 3rd column - BC)
         """
         return np.column_stack((self.connections, self.boundary_conditions))
 
     @classmethod
     def construct(cls, initial_condition=0, **kwargs_construct):
         """Construct a Box with given initial condition.
-        
+
         Parameters
         ----------
         initial_condition : int, default 0
             IC = 0 or 1. Rectangular box of dimensions ``width`` x ``height``,
             absorbing bottom wall, reflecting left and right, and:
                 - IC = 0: constant flux on top (Laplacian case)
                 - IC = 1: reflective top (Poissonian case)
@@ -201,15 +195,15 @@
 
         Returns
         -------
         box : Box
             An object of class Box.
         branches : list
             A list of objects of class Branch.
-            
+
 
         """
         # Labels for boundary conditions
         DIRICHLET = 1
         NEUMANN = 2
         CONSTANT_FLUX = 3
 
@@ -233,29 +227,31 @@
                     [options_construct["width"], options_construct["height"]],
                     [0, options_construct["height"]],
                     [0, 0],
                 ]
             )
             box.seeds_connectivity = np.column_stack(
                 (
-                    len(box.points) + np.arange(len(options_construct["seeds_x"])),
+                    len(box.points) +
+                    np.arange(len(options_construct["seeds_x"])),
                     np.arange(len(options_construct["seeds_x"])),
                 )
             )
             box.__add_points(
                 np.vstack(
                     [
                         options_construct["seeds_x"],
                         np.zeros(len(options_construct["seeds_x"])),
                     ]
                 ).T
             )
 
             connections_to_add = np.vstack(
-                [np.arange(len(box.points)), np.roll(np.arange(len(box.points)), -1)]
+                [np.arange(len(box.points)), np.roll(
+                    np.arange(len(box.points)), -1)]
             ).T
             box.__add_connection(
                 connections_to_add,
                 boundary_conditions=DIRICHLET
                 * np.ones(len(connections_to_add), dtype=int),
             )
 
@@ -305,18 +301,18 @@
         (noted with branch IDs).
 
     """
 
     def __init__(
         self,
         box,
-        branches=[],
-        active_branches=[],
-        sleeping_branches=[],
-        branch_connectivity=[],
+        branches=None,
+        active_branches=None,
+        sleeping_branches=None,
+        branch_connectivity=None,
     ):
         """Initialize Network.
 
         Parameters
         ----------
         box : Box
         branches : list, default []
@@ -328,19 +324,21 @@
         -------
         None.
 
         """
 
         self.box = box
 
-        self.branches = branches  # all branches (to construct mesh): moving + sleeping + branches inside the tree
-        self.active_branches = active_branches  # moving branches (to extend)
-        self.sleeping_branches = sleeping_branches  # branches without enough flux to move (may revive in the Poisson case)
+        # all branches (to construct mesh): moving + sleeping + branches inside the tree
+        self.branches = [] if branches is None else branches
+        self.active_branches = [] if active_branches is None else active_branches  # moving branches (to extend)
+        # branches without enough flux to move (may revive in the Poisson case)
+        self.sleeping_branches = [] if sleeping_branches is None else sleeping_branches
 
-        self.branch_connectivity = branch_connectivity
+        self.branch_connectivity = [] if branch_connectivity is None else branch_connectivity
 
     def copy(self):
         """Return a deepcopy of the Network."""
         return copy.deepcopy(self)
 
     def height_and_length(self):
         """Return network height (max y coordinate) and total length of the branches."""
@@ -352,15 +350,16 @@
         return height, ruler
 
     def __add_connection(self, connection):
         """Add connection to self.branch_connectivity."""
         if not len(self.branch_connectivity):
             self.branch_connectivity = connection
         else:
-            self.branch_connectivity = np.vstack((self.branch_connectivity, connection))
+            self.branch_connectivity = np.vstack(
+                (self.branch_connectivity, connection))
 
     def move_tips(self, step):
         """Move tips (with bifurcations and killing).
 
         Parameters
         ----------
         step : int, default 0
@@ -370,50 +369,47 @@
         -------
         None.
 
         """
 
         # shallow copy of active_branches (creates new list instance, but the elements are still the same)
         branches_to_iterate = self.active_branches.copy()
-        for i, branch in enumerate(branches_to_iterate):
-            if not branch.is_moving:
-                self.sleeping_branches.append(branch)
+        for branch in branches_to_iterate:
+            if branch.is_bifurcating:
+                print("! Branch {ID} bifurcated !".format(ID=branch.ID))
+                max_branch_id = len(self.branches) - 1
+
+                for i, dR in enumerate(branch.dR):
+                    points = np.array(
+                        [branch.points[-1], branch.points[-1] + dR])
+                    branch_new = Branch(
+                        ID=max_branch_id + i + 1,
+                        points=points,
+                        steps=np.array([step - 1]),
+                    )
+                    self.branches.append(branch_new)
+                    self.active_branches.append(branch_new)
+                    self.__add_connection(
+                        np.array([branch.ID, branch_new.ID]))
                 self.active_branches.remove(branch)
-                print("! Branch {ID} is sleeping !".format(ID=branch.ID))
             else:
-                if branch.is_bifurcating:
-                    print("! Branch {ID} bifurcated !".format(ID=branch.ID))
-                    max_branch_id = len(self.branches) - 1
-
-                    for i, dR in enumerate(branch.dR):
-                        points = np.array([branch.points[-1], branch.points[-1] + dR])
-                        branch_new = Branch(
-                            ID=max_branch_id + i + 1,
-                            points=points,
-                            steps=np.array([step - 1]),
-                        )
-                        self.branches.append(branch_new)
-                        self.active_branches.append(branch_new)
-                        self.__add_connection(np.array([branch.ID, branch_new.ID]))
-                    self.active_branches.remove(branch)
-                else:
-                    branch.extend_by_dR()
+                branch.extend()
 
 
 class System:
     """A class containing all the elements to run a network simulation.
 
     Attributes
     ----------
     network : Network
         An object of class Network.
     extender : Extender
         An object of one of the classes from reticuler.extending_kernels.extenders.
-    trajectory_integrator : function
-        One of the classes from reticuler.extending_kernels.trajectory_integrator.
+    trajectory_integrator : TrajectoryIntegrator
+        One of the classes from reticuler.extending_kernels.trajectory_integrators.
     growth_thresh_type : int, default 0
         Type of growth threshold.
             - 0: number of steps
             - 1: height
             - 2: network length
     growth_thresh : float, default 5
         A value of growth threshold. The simulation is stopped, when it's reached.
@@ -427,17 +423,17 @@
     """
 
     def __init__(
         self,
         network,
         extender,
         trajectory_integrator,
-        growth_gauges=np.zeros(4),
         growth_thresh_type=0,
         growth_thresh=5,
+        growth_gauges=None,
         dump_every=1,
         exp_name="",
     ):
         """Initialize System.
 
         Parameters
         ----------
@@ -458,24 +454,29 @@
         self.network = network
         self.extender = extender
         self.trajectory_integrator = trajectory_integrator
 
         # Growth limits:
         # 0: number of steps, 1: max height
         # 2: max tree length 3: max time
-        self.growth_gauges = growth_gauges
+        self.growth_gauges = np.zeros(4) if growth_gauges is None else growth_gauges
         self.growth_thresh_type = growth_thresh_type
         self.growth_thresh = growth_thresh
 
         self.dump_every = dump_every
         self.exp_name = exp_name
+    
+    def copy(self):
+        """Return a deepcopy of the Network."""
+        return copy.deepcopy(self)
 
     def export_json(self):
         """Export all the information to 'self.exp_name'+'.json'."""
-        growth_type_legend = ["number of steps", "max height", "max tree length", "max time"]
+        growth_type_legend = ["number of steps",
+                              "max height", "max tree length", "max time"]
         export_general = {
             "reticuler_version": importlib.metadata.version("reticuler"),
             "exp_name": self.exp_name,
             "growth": {
                 "threshold_type": growth_type_legend[self.growth_thresh_type],
                 "threshold": self.growth_thresh,
                 "growth_gauges": {
@@ -483,29 +484,30 @@
                     "height": self.growth_gauges[1],
                     "network_length": self.growth_gauges[2],
                     "time": self.growth_gauges[3],
                 },
                 "dump_every": self.dump_every,
             },
         }
-        
+
         if type(self.extender).__name__ == "Streamline":
             if type(self.trajectory_integrator).__name__ == "ModifiedEulerMethod":
                 export_trajectory_integrator = {
                     "type": type(self.trajectory_integrator).__name__,
                     "max_approximation_step": self.trajectory_integrator.max_approximation_step,
-                }            
+                }
             if type(self.extender.pde_solver).__name__ == "FreeFEM":
                 equation_legend = ["Laplace", "Poisson"]
                 export_solver = {
                     "type": type(self.extender.pde_solver).__name__,
                     "equation": equation_legend[self.extender.pde_solver.equation],
-                }            
+                }
 
-            bifurcation_type_legend = ["no bifurcations", "a1", "a3/a1", "random"]
+            bifurcation_type_legend = [
+                "no bifurcations", "a1", "a3/a1", "random"]
             export_extender = {
                 "type": type(self.extender).__name__,
                 "eta": self.extender.eta,
                 "ds": self.extender.ds,
                 "bifurcations": {
                     "type": bifurcation_type_legend[
                         self.extender.bifurcation_type
@@ -513,15 +515,15 @@
                     "threshold": self.extender.bifurcation_thresh,
                     "angle": self.extender.bifurcation_angle,
                 },
                 "inflow_thresh": self.extender.inflow_thresh,
                 "distance_from_bif_thresh": self.extender.distance_from_bif_thresh,
                 "pde_solver": {**export_solver},
             }
-            
+
             export_extending_kernel = {
                 "extending_kernel": {
                     "trajectory_integrator": {**export_trajectory_integrator},
                     "extender": {**export_extender},
                 }
             }
 
@@ -553,15 +555,16 @@
                 "branch_connectivity": self.network.branch_connectivity,
                 "branches": {**export_branches},
             }
         }
 
         to_export = export_general | export_extending_kernel | export_network
         with open(self.exp_name + ".json", "w", encoding="utf-8") as f:
-            json.dump(to_export, f, ensure_ascii=False, indent=4, cls=_NumpyEncoder)
+            json.dump(to_export, f, ensure_ascii=False,
+                      indent=4, cls=NumpyEncoder)
 
     @classmethod
     def import_json(cls, input_file):
         """Construct an instance of class System based on the imported .json file.
 
         Parameters
         ----------
@@ -582,66 +585,67 @@
         sleeping_branches = []
         for i in reversed(list(json_load["network"]["branches"].keys())):
             json_branch = json_load["network"]["branches"][i]
             points_steps = np.asarray(json_branch["points_and_steps"])
             branch = Branch(
                 ID=json_branch["ID"],
                 points=points_steps[:, :2],
-                steps=points_steps[:, 2],
+                steps=np.array(points_steps[:, 2], dtype=int),
             )
 
             branches.append(branch)
             if json_branch["state"] == "active":
                 active_branches.append(branch)
             elif json_branch["state"] == "sleeping":
                 sleeping_branches.append(branch)
-                branch.is_moving = False
-            elif json_branch["state"] == "dead":
-                branch.is_moving = False
 
         # Box
         json_box = json_load["network"]["box"]
         connections_bc = np.asarray(json_box["connections_and_bc"])
         box = Box(
             points=np.asarray(json_box["points"]),
             connections=connections_bc[:, :2],
             boundary_conditions=connections_bc[:, 2],
             seeds_connectivity=np.asarray(json_box["seeds_connectivity"]),
         )
         # Network
-        branch_connectivity = np.asarray(json_load["network"]["branch_connectivity"])
+        branch_connectivity = np.asarray(
+            json_load["network"]["branch_connectivity"])
         network = Network(
             box=box,
             branches=branches,
             active_branches=active_branches,
             sleeping_branches=sleeping_branches,
             branch_connectivity=branch_connectivity,
         )
 
         # Trajectory integrator
         json_trajectory_integrator = json_load["extending_kernel"][
             "trajectory_integrator"
         ]
         if json_trajectory_integrator["type"] == "ModifiedEulerMethod":
             max_approximation_step = json_trajectory_integrator["max_approximation_step"]
-            trajectory_integrator = trajectory_integrators.ModifiedEulerMethod(max_approximation_step=max_approximation_step)
+            trajectory_integrator = trajectory_integrators.ModifiedEulerMethod(
+                max_approximation_step=max_approximation_step)
 
         # Solver
         json_solver = json_load["extending_kernel"]["extender"]["pde_solver"]
         if json_solver["type"] == "FreeFEM":
             equation_legend = ["Laplace", "Poisson"]
             equation = equation_legend.index(json_solver["equation"])
             pde_solver = pde_solvers.FreeFEM(equation=equation)
 
         # Extender
         json_extender = json_load["extending_kernel"]["extender"]
         if json_extender["type"] == "Streamline":
             json_bifurcation = json_extender["bifurcations"]
-            bifurcation_type_legend = ["no bifurcations", "a1", "a3/a1", "random"]
-            bifurcation_type = bifurcation_type_legend.index(json_bifurcation["type"])
+            bifurcation_type_legend = [
+                "no bifurcations", "a1", "a3/a1", "random"]
+            bifurcation_type = bifurcation_type_legend.index(
+                json_bifurcation["type"])
             extender = extenders.Streamline(
                 pde_solver=pde_solver,
                 eta=json_extender["eta"],
                 ds=json_extender["ds"],
                 bifurcation_type=bifurcation_type,
                 bifurcation_thresh=json_bifurcation["threshold"],
                 bifurcation_angle=json_bifurcation["angle"],
@@ -649,16 +653,18 @@
             extender.inflow_thresh = json_extender["inflow_thresh"]
             extender.distance_from_bif_thresh = json_extender[
                 "distance_from_bif_thresh"
             ]
 
         # General
         json_growth = json_load["growth"]
-        growth_type_legend = ["number of steps", "max height", "max tree length", "max time"]
-        growth_thresh_type = growth_type_legend.index(json_growth["threshold_type"])
+        growth_type_legend = ["number of steps",
+                              "max height", "max tree length", "max time"]
+        growth_thresh_type = growth_type_legend.index(
+            json_growth["threshold_type"])
         growth_thresh = json_growth["threshold"]
         dump_every = json_growth["dump_every"]
 
         json_growth_gauges = json_growth["growth_gauges"]
         growth_gauges = np.array(
             [
                 json_growth_gauges["number_of_steps"],
@@ -679,21 +685,23 @@
             exp_name=input_file,
         )
 
         return system
 
     def __update_growth_gauges(self, dt):
         """Update growth gauges."""
-        self.growth_gauges[1], self.growth_gauges[2] = self.network.height_and_length()
+        self.growth_gauges[1], self.growth_gauges[2] = self.network.height_and_length(
+        )
         self.growth_gauges[3] = self.growth_gauges[3] + dt
 
-        print("Active branches: {n:d}".format(n=len(self.network.active_branches)))
+        print("Active branches: {n:d}".format(
+            n=len(self.network.active_branches)))
         print("Network height: {h:.3f}".format(h=self.growth_gauges[1]))
         print("Network length: {l:.3f}".format(l=self.growth_gauges[2]))
-        print("Evolution time: {l:.3f}".format(l=self.growth_gauges[3]))
+        print("Evolution time: {t:.3f}".format(t=self.growth_gauges[3]))
 
         for branch in self.network.active_branches:
             branch.steps = np.append(branch.steps, self.growth_gauges[0])
             # branch.timestamps = np.append( branch.timestamps, self.growth_gauges[3] )
 
     def evolve(self):
         """Run the simulation.
@@ -712,15 +720,16 @@
             print(
                 "\n-------------------   Growth step: {step:.0f}   -------------------\n".format(
                     step=self.growth_gauges[0]
                 )
             )
             print("Date and time: ", datetime.datetime.now())
 
-            dt = self.trajectory_integrator.integrate(extender=self.extender, network=self.network)
+            dt, _ = self.trajectory_integrator.integrate(
+                extender=self.extender, network=self.network)
             self.network.move_tips(step=self.growth_gauges[0])
             self.__update_growth_gauges(dt)
 
             if not self.growth_gauges[0] % self.dump_every:
                 self.export_json()
 
         self.export_json()
```

### Comparing `reticuler-0.4/src/reticuler/user_interface/graphics.py` & `reticuler-1.0/src/reticuler/user_interface/graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,11 +71,9 @@
     ax.axis("off")
     # colouring background
     ax.add_artist(ax.patch)
     ax.patch.set_zorder(-1)
     ax.set_facecolor("#def1ff")
     ax.set_aspect("equal")
     ax.set_xlim(0, xlim)
-    if ylim is None:
-        ax.set_ylim(0, y_max)
-    else:
-        ax.set_ylim(0, ylim)
+    ylim = 1.05*y_max if ylim is None else ylim
+    ax.set_ylim(0, ylim)
```

### Comparing `reticuler-0.4/src/reticuler.egg-info/PKG-INFO` & `reticuler-1.0/src/reticuler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reticuler
-Version: 0.4
+Version: 1.0
 Summary: Simulations of spatial networks growth
 Author: Stanisław Żukowski
 Author-email: zukowski.st@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/stzukowski/reticuler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reticuler Version: 0.4 Summary: Simulations of
+Metadata-Version: 2.1 Name: reticuler Version: 1.0 Summary: Simulations of
 spatial networks growth Author: StanisÅaw Å»ukowski Author-email:
 zukowski.st@gmail.com License: MIT Project-URL: Source, https://github.com/
 stzukowski/reticuler Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # Reticuler
                [PyPI] [Documentation_Status] [Code_style:_black]
```

### Comparing `reticuler-0.4/src/reticuler.egg-info/SOURCES.txt` & `reticuler-1.0/src/reticuler.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/reticuler/__init__.py
-src/reticuler/plot_ret.py
-src/reticuler/reticulate.py
 src/reticuler/system.py
 src/reticuler.egg-info/PKG-INFO
 src/reticuler.egg-info/SOURCES.txt
 src/reticuler.egg-info/dependency_links.txt
 src/reticuler.egg-info/entry_points.txt
 src/reticuler.egg-info/requires.txt
 src/reticuler.egg-info/top_level.txt
+src/reticuler/backward_evolution/__init__.py
+src/reticuler/backward_evolution/system_back.py
+src/reticuler/backward_evolution/trimmers.py
 src/reticuler/extending_kernels/__init__.py
 src/reticuler/extending_kernels/extenders.py
 src/reticuler/extending_kernels/pde_solvers.py
 src/reticuler/extending_kernels/trajectory_integrators.py
 src/reticuler/user_interface/__init__.py
-src/reticuler/user_interface/graphics.py
+src/reticuler/user_interface/clip_ret.py
+src/reticuler/user_interface/clippers.py
+src/reticuler/user_interface/graphics.py
+src/reticuler/user_interface/plot_ret.py
+src/reticuler/user_interface/reticulate.py
+src/reticuler/user_interface/reticulate_back.py
```

