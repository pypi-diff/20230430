# Comparing `tmp/simulated_bifurcation-1.0.0.tar.gz` & `tmp/simulated_bifurcation-1.0.1.tar.gz`

## Comparing `simulated_bifurcation-1.0.0.tar` & `simulated_bifurcation-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.0/CITATION.cff
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.0/requirements.txt
--rw-r--r--   0        0        0    31537 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.0/src/simulated_bifurcation/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.0/.gitignore
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.0/LICENSE
--rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.0/README.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/CITATION.cff
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/requirements.txt
+-rw-r--r--   0        0        0    24832 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/__init__.py
+-rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/interface.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/markowitz.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/partitioning.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/src/simulated_bifurcation/qubo.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/LICENSE
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/README.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9425 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.1/PKG-INFO
```

### Comparing `simulated_bifurcation-1.0.0/src/simulated_bifurcation/__init__.py` & `simulated_bifurcation-1.0.1/src/simulated_bifurcation/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from abc import ABC, abstractmethod
-from typing import List, Tuple, Union, final
-
+from typing import List, Tuple, Union
 import torch
 from tqdm import tqdm
 from numpy import minimum, argmin
 
 
 class Ising:
 
@@ -300,178 +298,14 @@
 
         spins = optimizer.symplectic_update(self, use_window)
         
         if self.linear_term: self.computed_spins = spins[-1] * spins[:-1, :]
         else: self.computed_spins = spins
 
 
-class SBModel(ABC):
-    """
-    An abstract class to adapt optimization problems as Ising problems.
-    """
-
-    @abstractmethod
-    def __to_Ising__(self) -> Ising:
-        """
-        Generate an equivalent Ising model of the problem.
-        The notion of equivalence means that finding the ground
-        state of this new model is strictly equivalent to find
-        the ground state of the original problem.
-        Thus, there may be no scientific signification of this
-        equivalent model.
-
-        Returns
-        -------
-        Ising
-        """
-        raise NotImplementedError
-
-    @abstractmethod
-    def __from_Ising__(self, ising: Ising) -> None:
-        """
-        Retrieves information from the optimized equivalent Ising model.
-        Modifies the object's attributes in place.
-
-        Parameters
-        ----------
-        ising : Ising
-            equivalent Ising model of the problem
-        """
-        raise NotImplementedError
-
-    @final
-    def optimize(
-        self,
-        time_step: float = .1,
-        convergence_threshold: int = 50,
-        sampling_period: int = 50,
-        max_steps: int = 10000,
-        agents: int = 128,
-        pressure_slope: float = .01,
-        gerschgorin: bool = False,
-        use_window: bool = True,
-        ballistic: bool = False,
-        heat_parameter: float = None,
-        verbose: bool = True
-    ) -> None:
-        """
-        Computes an approximated solution of the Ising problem using the
-        Simulated Bifurcation algorithm. The ground state in modified in place.
-        It should correspond to a local minimum for the Ising energy function.
-
-        The Simulated Bifurcation (SB) algorithm mimics Hamiltonian dynamics to
-        make spins evolve throughout time. It uses a symplectic Euler scheme
-        for this purpose.
-
-        There are different version of the SB algorithm:
-        - the ballistic Simulated Bifurcation (bSB) which uses the particles'
-        position for the matrix computations (usually slower but more accurate)
-        - the discrete Simulated Bifurcation (dSB) which uses the particles'
-        spin for the matrix computations (usually faster but less accurate)
-        - the Heated ballistic Simulated Bifurcation (HbSB) which uses the bSB
-        algorithm with a supplementary non-symplectic term to refine the model
-        - the Heated ballistic Simulated Bifurcation (HdSB) which uses the dSB
-        algorithm with a supplementary non-symplectic term to refine the model
-
-        To stop the iterations of the Euler scheme, a number of maximum steps
-        needs to be specified. However a refined way to stop is also possible
-        using a window that checks that the spins have not changed among a set
-        number of previous steps. In practice, a every fixed number of steps
-        (called a sampling period) the current spins will be compared to the
-        previous ones. If they remain constant throughout a certain number of
-        consecutive samplings (called the convergence threshold), the spins are
-        considered to have bifurcated and the algorithm stops.
-
-        Finally, it is possible to make several particle vectors at the same
-        time (each one being called an agent). As the vectors are randomly
-        initialized, using several agents helps exploring the solution space
-        and increases the probability of finding a better solution, though it
-        also slightly increases the computation time. In the end, only the best
-        spin vector (energy-wise) is kept and used as the new Ising model'
-        ground state.
-
-        Parameters
-        ----------
-
-        - Euler scheme parameters
-
-        time_step : float, optional
-            step size for the time discretization (default is 0.01)
-        symplectic_parameter : int | 'inf', optional
-            symplectic parameter for the Euler's scheme (default is 2)
-        convergence_threshold : int, optional
-            number of consecutive identical spin sampling considered as a proof
-            of convergence (default is 35)
-        sampling_period : int, optional
-            number of time steps between two spin sampling (default is 50)
-        max_steps : int, optional
-            number of time steps after which the algorithm will stop inevitably
-            (default is 60000)
-        agents : int, optional
-            number of vectors to make evolve at the same time (default is 20)
-        use_window : bool, optional
-            indicates whether to use the window as a stopping criterion or not
-            (default is True)
-        ballistic : bool, optional
-            if True, the ballistic SB will be used, else it will be the
-            discrete SB (default is True)
-        heated : bool, optional
-            if True, the heated SB will be used, else it will be the non-heated
-            SB (default is True)
-
-        - Quantum parameters
-
-        detuning_frequency : float, optional
-            detuning frequency of the Hamiltonian (default is 1.0)
-        pressure_slope : float, optional
-            pumping pressure's linear slope allowing adiabatic evolution
-            (default is 0.01)
-        final_pressure : float | None, optional
-            pumping pressure's maximum value; if None, no maximum value is set
-            (default is None)
-        xi0 : float | 'gerschgorin' | None, optional
-            weighting coefficient in the Hamiltonian; if None it will be
-            computed based on the J matrix (default is None)
-        heat_parameter : float, optional
-            heat parameter for the heated SB algorithm (default is 0.06)
-
-        - Others
-
-        verbose : bool, optional
-            whether to display evolution information or not (default is True)
-
-        See Also
-        --------
-
-        For more information on the Hamiltonian parameters, check
-        `SymplecticEulerScheme`.
-
-        Notes
-        -----
-
-        For low dimensions, see the `comprehensive_search` method function
-        instead that will always find the true optimal ground state.
-        """
-        ising_equivalent = self.__to_Ising__()
-        ising_equivalent.optimize(
-            time_step,
-            convergence_threshold,
-            sampling_period,
-            max_steps,
-            agents,
-            pressure_slope,
-            gerschgorin,
-            use_window,
-            ballistic,
-            heat_parameter,
-            verbose
-        )
-        self.__from_Ising__(ising_equivalent)
-
-
 class Optimizer():
     """
     An abstract class to implement a Symplectic Euler Scheme to perform the
     Simulated Bifurcation (SB) algorithm.
 
     Attributes
     ---------
```

### Comparing `simulated_bifurcation-1.0.0/.gitignore` & `simulated_bifurcation-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.0/LICENSE` & `simulated_bifurcation-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.0/README.md` & `simulated_bifurcation-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,44 +4,22 @@
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1xtse4sLIDAh8nsQ6HcIr7BzM7sft88WA?usp=sharing)
 ![GitHub stars](https://img.shields.io/github/stars/bqth29/simulated-bifurcation-algorithm.svg?style=social&label=Star)
 
 Python implementation of the _Simulated Bifurcation_ algorithm in order to approximize the optimal solution of **Ising problems**. The last accuracy tests showed a median optimality gap of less than 1% on high-dimensional instances.
 
 ## ⚙️ Install
 
-### With `pip`
-
-```
-pip install simulated_bifurcation
 ```
-
-### From GitHub
-
-1. Clone the repository
-
-```
-git clone https://github.com/bqth29/simulated-bifurcation-algorithm.git
-```
-
-1. Change directory
-
-```bash
-cd simulated-bifurcation-algorithm
-```
-
-1. Intall dependencies
-
-```powershell
-python -m pip install -r requirements.txt
+pip install simulated-bifurcation
 ```
 
 ## 🧪 Scientific background
 
 _Simulated bifurcation_ is a state-of-the-art algorithm based on quantum physics theory and used to approximize very accurately and quickly the optimal solution of Ising problems. 
->You can read about the scientific theories at stake and the engineering of the algorithm here: https://arxiv.org/abs/2108.03092
+>You can read about the scientific theories at stake and the engineering of the algorithm by Goto *et al.* here: https://www.nature.com/articles/s42005-022-00929-9
 
 Ising problems can be used in many sectors such as finance, transportation or chemistry or derived as other well-know optimization problems (QUBO, Knapsack problem, ...).
 
 ## 🚀 Optimization of an Ising model
 
 ### Definition
 
@@ -69,34 +47,31 @@
 
 ### Retrieve the ground state / Ising energy
 
 Once the model is optimized, you can get the best found Ising features using model's attributes
 
 ```python
 ising.energy # Ising energy -> float
-ising.ground_state # Ground state (best spin vector) -> numpy.ndarray
+ising.ground_state # Ground state (best spin vector) -> torch.Tensor
 ```
 
 ## 📊 Optimization parameters
 
 The `optimize` methods uses a lot of parameters but only some of them may be changes since the biggest part has been set after reserach and fine-tuning work.
 
 ### Quantum parameters
 
 These parameters stem from the quantum theory Their purpose is described in the paper cited above.
 
 > The parameters marked with ⚠️ should not be changed to ensure a good accuracy of the algorithm.
 
-- `detuning_frequency` ⚠️
 - `pressure_slope` ⚠️
-- `final_pressure` ⚠️
-- `xi0`: if `None` then uses the value defined by Goto *et al.*; if `'gerschgorin'` then uses the Gerschgorin's theorem to set the value; else uses the provided value (`float`)
+- `gerschgorin`: if `True` then uses the Gerschgorin's theorem to set the scale value; else uses the uses the value defined by Goto *et al.*
 - `heat_parameter` ⚠️
 - `time_step` ⚠️
-- `symplectic_parameter`: either an `int` or `'inf'` for the asymptotic symplectic update
 
 ### Simulated Bifurcation modes
 
 There are four modes of the algorithm (ballistic v. discrete + heated v. non-heated) that result in small variations in the algorithm general operation. These mode can be selected setting the parameters `ballistic` and `heated` to `True` or `False`.
 
 > The ballistic mode is supposed to give a slighter less satisfying accuracy but to converge faster in comparison to the discrete mode which is generally more accurate but also a bit slower.
 
@@ -116,67 +91,79 @@
 
 ### Displaying the state of evolution
 
 Finally, you can choose to show or hide the evolution of the algorithm setting the `verbose` parameter to either `True` or `False`.
 
 > If you choose to set `verbose = True`, the evolution will be displayed as `tqdm` progress bar(s) in your terminal.
 
-## 🔀 Derive the algorithm for other problems using the SBModel API
+## 🔀 Derive the algorithm for other problems using the IsingInterface API
 
 A lot of mathematical problems ([QUBO](https://en.wikipedia.org/wiki/Quadratic_unconstrained_binary_optimization), [TSP](https://en.wikipedia.org/wiki/Travelling_salesman_problem), ...) can be written as Ising problems, and thus can be solved using the Simulated Bifurcation algorithm. Some of them are already implemented in the `models` folder but you are free to create your own models using our API.
 
-To do so, you need to create a subclass of the abstract class `SBModel`.
+To do so, you need to create a subclass of the abstract class `IsingInterface` present in the `interface` submodule. The `IsingInterface` has only two attributes `dtype` and `device` which allow you to set the type of the data and the device with which you wish to work.
 
 ```python
-class YourModel(sb.SBModel):
+from simulated_bifurcation.interface import IsingInterface
+
 
-    ...
+class YourModel(IsingInterface):
+
+    def __init__(self, dtype, device, *args, **kwargs):
+        super().__init__(dtype, device) # Mandatory
+        # YOUR CODE HERE
+        ...
 ```
 
 Once created, such an object can be optimized using the same principle as an `Ising` object, using the `optimize` methods which uses the same parameters as the `Ising`'s one:
 
 ```python
 your_model = YourModel(...)
 your_model.optimize()
 ```
 
-Yet, to make it work, you will first have to overwrite two abstract methods of the `SBModel` class (`__to_Ising__` and `__from_Ising__`) that are called by the `optimize` method. Otherwise you will get a `NotImplementedError` error message.
+Yet, to make it work, you will first have to overwrite two abstract methods of the `IsingInterface` class (`__to_Ising__` and `__from_Ising__`) that are called by the `optimize` method. Otherwise you will get a `NotImplementedError` error message.
 
-When the `optimize` method is called, an equivalent Ising model will first be created using `__to_Ising__` and then optimized using the exact same parameters you provided as input for the `SBModel.optimize` method. Once it is optimized, information for your own model will be derived from the optimal features of this equivalent Ising model using `__from_Ising__`.
+When the `optimize` method is called, an equivalent Ising model will first be created using `__to_Ising__` and then optimized using the exact same parameters you provided as input for the `IsingInterface.optimize` method. Once it is optimized, information for your own model will be derived from the optimal features of this equivalent Ising model using `__from_Ising__`.
 
 ### `__to_Ising__` method
 
 The `__to_Ising__` is meant to create an instance of an Ising model based on the data of your problem. It takes no argument and must only return an `Ising` object. The idea is to rely on the parameters of your problems to derive an Ising representation of it. At some point in the definition of the method, you will have to create the `J` matrix and the `h` vector and eventually return `Ising(J, h)`.
 
 ```python
 def __to_Ising__(self) -> sb.Ising:
     # YOUR CODE HERE
     J = ...
     h = ...
-    return sb.Ising(J, h)
+    return sb.Ising(J, h, dtype=self.dtype, device=self.device)
 ```
 
+> Do not forget to set the `device` attribute when you instantiate the class if you are working on a GPU because all the tensors must be set on the same device.
+
 ### `__from_Ising__` method
 
 The `__from_Ising__` is the reciprocal method. Once the equivalent Ising model of your problem has been optimized, you can retrieve information from its ground state and/or energy and adapt them to your own problem. It must only take an `Ising` object for input and return `None`.
 
 ```python
 def __from_Ising__(self, ising: sb.Ising) -> None:
     # YOUR CODE HERE
     return 
 ```
 
+### Binary and integer formulations
+
+Note that many problems that can be represented as Ising models are not based on spin vectors but rather on binary or integer vectors. The `interface` submodule thus has two additional classes, `Binary` and `Integer`, both of which inherit from `IsingInterface` in order to generalize these cases more easily.
+
 > 🔎 You can check [Andrew Lucas' paper](https://arxiv.org/pdf/1302.5843.pdf) on Ising formulations of NP-complete and NP-hard problems, including all of Karp's 21 NP-complete problems.
 
-## 🔗 Cite this repository
+## 🔗 Cite this work
 
 If you are using this code for your own projects please cite our work:
 
 ```bibtex
 @software{Ageron_Simulated_Bifurcation_SB_2022,
     author = {Ageron, Romain and Bouquet, Thomas and Pugliese, Lorenzo},
-    month = {9},
+    month = {4},
     title = {{Simulated Bifurcation (SB) algorithm for Python}},
-    version = {2.0.1},
-    year = {2022}
+    version = {1.0.0},
+    year = {2023}
 }
 ```
```

### Comparing `simulated_bifurcation-1.0.0/pyproject.toml` & `simulated_bifurcation-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simulated_bifurcation"
-version = "1.0.0"
+version = "1.0.1"
 description = "An efficient implementation of the quantum physics-inspired Simulated Bifurcation (SB) algorithm to solve Ising-like problems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `simulated_bifurcation-1.0.0/PKG-INFO` & `simulated_bifurcation-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulated_bifurcation
-Version: 1.0.0
+Version: 1.0.1
 Summary: An efficient implementation of the quantum physics-inspired Simulated Bifurcation (SB) algorithm to solve Ising-like problems.
 Project-URL: Homepage, https://github.com/bqth29/simulated-bifurcation-algorithm
 Project-URL: Bug Tracker, https://github.com/bqth29/simulated-bifurcation-algorithm/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -17,44 +17,22 @@
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1xtse4sLIDAh8nsQ6HcIr7BzM7sft88WA?usp=sharing)
 ![GitHub stars](https://img.shields.io/github/stars/bqth29/simulated-bifurcation-algorithm.svg?style=social&label=Star)
 
 Python implementation of the _Simulated Bifurcation_ algorithm in order to approximize the optimal solution of **Ising problems**. The last accuracy tests showed a median optimality gap of less than 1% on high-dimensional instances.
 
 ## ⚙️ Install
 
-### With `pip`
-
-```
-pip install simulated_bifurcation
 ```
-
-### From GitHub
-
-1. Clone the repository
-
-```
-git clone https://github.com/bqth29/simulated-bifurcation-algorithm.git
-```
-
-1. Change directory
-
-```bash
-cd simulated-bifurcation-algorithm
-```
-
-1. Intall dependencies
-
-```powershell
-python -m pip install -r requirements.txt
+pip install simulated-bifurcation
 ```
 
 ## 🧪 Scientific background
 
 _Simulated bifurcation_ is a state-of-the-art algorithm based on quantum physics theory and used to approximize very accurately and quickly the optimal solution of Ising problems. 
->You can read about the scientific theories at stake and the engineering of the algorithm here: https://arxiv.org/abs/2108.03092
+>You can read about the scientific theories at stake and the engineering of the algorithm by Goto *et al.* here: https://www.nature.com/articles/s42005-022-00929-9
 
 Ising problems can be used in many sectors such as finance, transportation or chemistry or derived as other well-know optimization problems (QUBO, Knapsack problem, ...).
 
 ## 🚀 Optimization of an Ising model
 
 ### Definition
 
@@ -82,34 +60,31 @@
 
 ### Retrieve the ground state / Ising energy
 
 Once the model is optimized, you can get the best found Ising features using model's attributes
 
 ```python
 ising.energy # Ising energy -> float
-ising.ground_state # Ground state (best spin vector) -> numpy.ndarray
+ising.ground_state # Ground state (best spin vector) -> torch.Tensor
 ```
 
 ## 📊 Optimization parameters
 
 The `optimize` methods uses a lot of parameters but only some of them may be changes since the biggest part has been set after reserach and fine-tuning work.
 
 ### Quantum parameters
 
 These parameters stem from the quantum theory Their purpose is described in the paper cited above.
 
 > The parameters marked with ⚠️ should not be changed to ensure a good accuracy of the algorithm.
 
-- `detuning_frequency` ⚠️
 - `pressure_slope` ⚠️
-- `final_pressure` ⚠️
-- `xi0`: if `None` then uses the value defined by Goto *et al.*; if `'gerschgorin'` then uses the Gerschgorin's theorem to set the value; else uses the provided value (`float`)
+- `gerschgorin`: if `True` then uses the Gerschgorin's theorem to set the scale value; else uses the uses the value defined by Goto *et al.*
 - `heat_parameter` ⚠️
 - `time_step` ⚠️
-- `symplectic_parameter`: either an `int` or `'inf'` for the asymptotic symplectic update
 
 ### Simulated Bifurcation modes
 
 There are four modes of the algorithm (ballistic v. discrete + heated v. non-heated) that result in small variations in the algorithm general operation. These mode can be selected setting the parameters `ballistic` and `heated` to `True` or `False`.
 
 > The ballistic mode is supposed to give a slighter less satisfying accuracy but to converge faster in comparison to the discrete mode which is generally more accurate but also a bit slower.
 
@@ -129,67 +104,79 @@
 
 ### Displaying the state of evolution
 
 Finally, you can choose to show or hide the evolution of the algorithm setting the `verbose` parameter to either `True` or `False`.
 
 > If you choose to set `verbose = True`, the evolution will be displayed as `tqdm` progress bar(s) in your terminal.
 
-## 🔀 Derive the algorithm for other problems using the SBModel API
+## 🔀 Derive the algorithm for other problems using the IsingInterface API
 
 A lot of mathematical problems ([QUBO](https://en.wikipedia.org/wiki/Quadratic_unconstrained_binary_optimization), [TSP](https://en.wikipedia.org/wiki/Travelling_salesman_problem), ...) can be written as Ising problems, and thus can be solved using the Simulated Bifurcation algorithm. Some of them are already implemented in the `models` folder but you are free to create your own models using our API.
 
-To do so, you need to create a subclass of the abstract class `SBModel`.
+To do so, you need to create a subclass of the abstract class `IsingInterface` present in the `interface` submodule. The `IsingInterface` has only two attributes `dtype` and `device` which allow you to set the type of the data and the device with which you wish to work.
 
 ```python
-class YourModel(sb.SBModel):
+from simulated_bifurcation.interface import IsingInterface
+
 
-    ...
+class YourModel(IsingInterface):
+
+    def __init__(self, dtype, device, *args, **kwargs):
+        super().__init__(dtype, device) # Mandatory
+        # YOUR CODE HERE
+        ...
 ```
 
 Once created, such an object can be optimized using the same principle as an `Ising` object, using the `optimize` methods which uses the same parameters as the `Ising`'s one:
 
 ```python
 your_model = YourModel(...)
 your_model.optimize()
 ```
 
-Yet, to make it work, you will first have to overwrite two abstract methods of the `SBModel` class (`__to_Ising__` and `__from_Ising__`) that are called by the `optimize` method. Otherwise you will get a `NotImplementedError` error message.
+Yet, to make it work, you will first have to overwrite two abstract methods of the `IsingInterface` class (`__to_Ising__` and `__from_Ising__`) that are called by the `optimize` method. Otherwise you will get a `NotImplementedError` error message.
 
-When the `optimize` method is called, an equivalent Ising model will first be created using `__to_Ising__` and then optimized using the exact same parameters you provided as input for the `SBModel.optimize` method. Once it is optimized, information for your own model will be derived from the optimal features of this equivalent Ising model using `__from_Ising__`.
+When the `optimize` method is called, an equivalent Ising model will first be created using `__to_Ising__` and then optimized using the exact same parameters you provided as input for the `IsingInterface.optimize` method. Once it is optimized, information for your own model will be derived from the optimal features of this equivalent Ising model using `__from_Ising__`.
 
 ### `__to_Ising__` method
 
 The `__to_Ising__` is meant to create an instance of an Ising model based on the data of your problem. It takes no argument and must only return an `Ising` object. The idea is to rely on the parameters of your problems to derive an Ising representation of it. At some point in the definition of the method, you will have to create the `J` matrix and the `h` vector and eventually return `Ising(J, h)`.
 
 ```python
 def __to_Ising__(self) -> sb.Ising:
     # YOUR CODE HERE
     J = ...
     h = ...
-    return sb.Ising(J, h)
+    return sb.Ising(J, h, dtype=self.dtype, device=self.device)
 ```
 
+> Do not forget to set the `device` attribute when you instantiate the class if you are working on a GPU because all the tensors must be set on the same device.
+
 ### `__from_Ising__` method
 
 The `__from_Ising__` is the reciprocal method. Once the equivalent Ising model of your problem has been optimized, you can retrieve information from its ground state and/or energy and adapt them to your own problem. It must only take an `Ising` object for input and return `None`.
 
 ```python
 def __from_Ising__(self, ising: sb.Ising) -> None:
     # YOUR CODE HERE
     return 
 ```
 
+### Binary and integer formulations
+
+Note that many problems that can be represented as Ising models are not based on spin vectors but rather on binary or integer vectors. The `interface` submodule thus has two additional classes, `Binary` and `Integer`, both of which inherit from `IsingInterface` in order to generalize these cases more easily.
+
 > 🔎 You can check [Andrew Lucas' paper](https://arxiv.org/pdf/1302.5843.pdf) on Ising formulations of NP-complete and NP-hard problems, including all of Karp's 21 NP-complete problems.
 
-## 🔗 Cite this repository
+## 🔗 Cite this work
 
 If you are using this code for your own projects please cite our work:
 
 ```bibtex
 @software{Ageron_Simulated_Bifurcation_SB_2022,
     author = {Ageron, Romain and Bouquet, Thomas and Pugliese, Lorenzo},
-    month = {9},
+    month = {4},
     title = {{Simulated Bifurcation (SB) algorithm for Python}},
-    version = {2.0.1},
-    year = {2022}
+    version = {1.0.0},
+    year = {2023}
 }
 ```
```

