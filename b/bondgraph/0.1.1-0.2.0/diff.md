# Comparing `tmp/bondgraph-0.1.1.tar.gz` & `tmp/bondgraph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondgraph-0.1.1.tar", last modified: Sun Apr 30 07:10:47 2023, max compression
+gzip compressed data, was "bondgraph-0.2.0.tar", last modified: Sun Apr 30 18:32:11 2023, max compression
```

## Comparing `bondgraph-0.1.1.tar` & `bondgraph-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.808578 bondgraph-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.804578 bondgraph-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.804578 bondgraph-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-30 07:10:31.000000 bondgraph-0.1.1/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-30 07:10:31.000000 bondgraph-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-30 07:10:31.000000 bondgraph-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-30 07:10:31.000000 bondgraph-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 07:10:31.000000 bondgraph-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-30 07:10:47.808578 bondgraph-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-30 07:10:31.000000 bondgraph-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.804578 bondgraph-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-30 07:10:31.000000 bondgraph-0.1.1/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-30 07:10:31.000000 bondgraph-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 07:10:47.808578 bondgraph-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.804578 bondgraph-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.808578 bondgraph-0.1.1/src/bondgraph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:31.000000 bondgraph-0.1.1/src/bondgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-30 07:10:31.000000 bondgraph-0.1.1/src/bondgraph/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-04-30 07:10:31.000000 bondgraph-0.1.1/src/bondgraph/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.808578 bondgraph-0.1.1/src/bondgraph/elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:31.000000 bondgraph-0.1.1/src/bondgraph/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-04-30 07:10:31.000000 bondgraph-0.1.1/src/bondgraph/elements/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-30 07:10:31.000000 bondgraph-0.1.1/src/bondgraph/elements/hydraulics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-30 07:10:31.000000 bondgraph-0.1.1/src/bondgraph/junctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-30 07:10:31.000000 bondgraph-0.1.1/src/bondgraph/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.808578 bondgraph-0.1.1/src/bondgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-30 07:10:47.000000 bondgraph-0.1.1/src/bondgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-30 07:10:47.000000 bondgraph-0.1.1/src/bondgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 07:10:47.000000 bondgraph-0.1.1/src/bondgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-30 07:10:47.000000 bondgraph-0.1.1/src/bondgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 07:10:47.000000 bondgraph-0.1.1/src/bondgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 07:10:47.808578 bondgraph-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-30 07:10:31.000000 bondgraph-0.1.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:32:11.444614 bondgraph-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:32:11.440614 bondgraph-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:32:11.444614 bondgraph-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-30 18:31:59.000000 bondgraph-0.2.0/.github/workflows/python-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-30 18:31:59.000000 bondgraph-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-30 18:31:59.000000 bondgraph-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-30 18:31:59.000000 bondgraph-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 18:31:59.000000 bondgraph-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-30 18:32:11.444614 bondgraph-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-30 18:31:59.000000 bondgraph-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:32:11.444614 bondgraph-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-30 18:31:59.000000 bondgraph-0.2.0/examples/custom_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-30 18:31:59.000000 bondgraph-0.2.0/examples/simple_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-30 18:31:59.000000 bondgraph-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:32:11.444614 bondgraph-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:32:11.440614 bondgraph-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:32:11.444614 bondgraph-0.2.0/src/bondgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:31:59.000000 bondgraph-0.2.0/src/bondgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-30 18:31:59.000000 bondgraph-0.2.0/src/bondgraph/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-04-30 18:31:59.000000 bondgraph-0.2.0/src/bondgraph/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-30 18:31:59.000000 bondgraph-0.2.0/src/bondgraph/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-30 18:31:59.000000 bondgraph-0.2.0/src/bondgraph/junctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-30 18:31:59.000000 bondgraph-0.2.0/src/bondgraph/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:32:11.444614 bondgraph-0.2.0/src/bondgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-30 18:32:11.000000 bondgraph-0.2.0/src/bondgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-30 18:32:11.000000 bondgraph-0.2.0/src/bondgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:32:11.000000 bondgraph-0.2.0/src/bondgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-30 18:32:11.000000 bondgraph-0.2.0/src/bondgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 18:32:11.000000 bondgraph-0.2.0/src/bondgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:32:11.444614 bondgraph-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-30 18:31:59.000000 bondgraph-0.2.0/tests/test_core.py
```

### Comparing `bondgraph-0.1.1/.github/workflows/python-package.yaml` & `bondgraph-0.2.0/.github/workflows/python-package.yaml`

 * *Files identical despite different names*

### Comparing `bondgraph-0.1.1/.github/workflows/release.yml` & `bondgraph-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `bondgraph-0.1.1/.gitignore` & `bondgraph-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bondgraph-0.1.1/LICENSE` & `bondgraph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bondgraph-0.1.1/PKG-INFO` & `bondgraph-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondgraph
-Version: 0.1.1
+Version: 0.2.0
 Summary: A library to create bond graphs for physical systems and generate their differential equations.
 Author-email: Karl Linderhed <bondgraph@karlinde.se>
 License: MIT License
         
         Copyright (c) 2022 Karl Linderhed
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,16 +32,14 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: visualization
 License-File: LICENSE
 
 # bondgraph
-[![Python package](https://github.com/Karlinde/bondgraph/actions/workflows/python-package.yaml/badge.svg)](https://github.com/Karlinde/bondgraph/actions/workflows/python-package.yaml)
-
 A python library for creating [bond graphs](https://en.wikipedia.org/wiki/Bond_graph) of 
 physical systems and generating differential equations.
 
 It heavily relies on `sympy` for manipulation and simplification of equations symbolically.
 
 ## Installation
 Install via pip:
@@ -62,15 +60,15 @@
 # Se ---> 1 ---> I
 #         |
 #         v
 #         R
 
 from bondgraph.core import Bond, BondGraph
 from bondgraph.junctions import JunctionEqualFlow
-from bondgraph.elements.basic import Element_R, Element_I, Source_effort
+from bondgraph.elements import Element_R, Element_I, Source_effort
 from sympy import Symbol
 
 force = Source_effort("force", Symbol("F"))
 friction = Element_R("friction", Symbol("k_f"))
 inertia = Element_I("inertia", Symbol("m"), Symbol("p"))
 mass_object = JunctionEqualFlow("mass_object")
```

### Comparing `bondgraph-0.1.1/README.md` & `bondgraph-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # bondgraph
-[![Python package](https://github.com/Karlinde/bondgraph/actions/workflows/python-package.yaml/badge.svg)](https://github.com/Karlinde/bondgraph/actions/workflows/python-package.yaml)
-
 A python library for creating [bond graphs](https://en.wikipedia.org/wiki/Bond_graph) of 
 physical systems and generating differential equations.
 
 It heavily relies on `sympy` for manipulation and simplification of equations symbolically.
 
 ## Installation
 Install via pip:
@@ -25,15 +23,15 @@
 # Se ---> 1 ---> I
 #         |
 #         v
 #         R
 
 from bondgraph.core import Bond, BondGraph
 from bondgraph.junctions import JunctionEqualFlow
-from bondgraph.elements.basic import Element_R, Element_I, Source_effort
+from bondgraph.elements import Element_R, Element_I, Source_effort
 from sympy import Symbol
 
 force = Source_effort("force", Symbol("F"))
 friction = Element_R("friction", Symbol("k_f"))
 inertia = Element_I("inertia", Symbol("m"), Symbol("p"))
 mass_object = JunctionEqualFlow("mass_object")
```

### Comparing `bondgraph-0.1.1/examples/simple.py` & `bondgraph-0.2.0/examples/simple_graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Se ---> 1 ---> I
         |
         v
         R
 """
 from bondgraph.core import Bond, BondGraph
 from bondgraph.junctions import JunctionEqualFlow
-from bondgraph.elements.basic import Element_R, Element_I, Source_effort
+from bondgraph.elements import Element_R, Element_I, Source_effort
 from sympy import Symbol
 
 force = Source_effort("force", Symbol("F"))
 friction = Element_R("friction", Symbol("k_f"))
 inertia = Element_I("inertia", Symbol("m"), Symbol("p"))
 mass_object = JunctionEqualFlow("mass_object")
```

### Comparing `bondgraph-0.1.1/pyproject.toml` & `bondgraph-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bondgraph-0.1.1/src/bondgraph/common.py` & `bondgraph-0.2.0/src/bondgraph/common.py`

 * *Files identical despite different names*

### Comparing `bondgraph-0.1.1/src/bondgraph/core.py` & `bondgraph-0.2.0/src/bondgraph/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from bondgraph.elements.basic import (
+from bondgraph.elements import (
     OnePortElement,
     TwoPortElement,
 )
 from bondgraph.junctions import Junction, JunctionEqualEffort, JunctionEqualFlow
 from bondgraph.common import (
     Causality,
     Bond,
     HasStateEquations,
     Node,
     AlgebraicLoopError,
 )
-from typing import Dict, List, Set
+from typing import Dict, List
 from sympy import Expr, Symbol, Equality
 import logging
 
 _BG_STATE_INIT = 0
 _BG_STATE_CAUSALITIES_DONE = 1
 
 
@@ -185,15 +185,14 @@
 
 class BondGraph:
     def __init__(self):
         self._bonds: List[Bond] = []
         self._elements: List[OnePortElement] = []
         self._junctions: List[Junction] = []
         self._two_port_elements: List[TwoPortElement] = []
-        self.parameters: Set[Symbol] = set()
         self._state = _BG_STATE_INIT
 
     def all_causalities_set(self):
         for bond in self._bonds:
             if not bond.has_causality_set():
                 return False
         return True
@@ -234,45 +233,41 @@
             if bond.node_from in self._elements:
                 raise Exception(
                     f"OnePortElement {bond.node_from} can only be bonded once!"
                 )
             if bond.node_from not in self._elements:
                 self._elements.append(bond.node_from)
             bond.node_from.bond = bond
-            self.parameters.update(bond.node_from.parameter_symbols())
         elif isinstance(bond.node_from, Junction):
             if bond.node_from not in self._junctions:
                 self._junctions.append(bond.node_from)
             if bond not in bond.node_from.bonds:
                 bond.node_from.bonds.append(bond)
         elif isinstance(bond.node_from, TwoPortElement):
             if bond.node_from not in self._two_port_elements:
                 self._two_port_elements.append(bond.node_from)
             bond.node_from.bond_2 = bond
-            self.parameters.update(bond.node_from.parameter_symbols())
 
         if isinstance(bond.node_to, OnePortElement):
             if bond.node_to in self._elements:
                 raise Exception(
                     f"OnePortElement {bond.node_to} can only be bonded once!"
                 )
             if bond.node_to not in self._elements:
                 self._elements.append(bond.node_to)
             bond.node_to.bond = bond
-            self.parameters.update(bond.node_to.parameter_symbols())
         elif isinstance(bond.node_to, Junction):
             if bond.node_to not in self._junctions:
                 self._junctions.append(bond.node_to)
             if bond not in bond.node_to.bonds:
                 bond.node_to.bonds.append(bond)
         elif isinstance(bond.node_to, TwoPortElement):
             if bond.node_to not in self._two_port_elements:
                 self._two_port_elements.append(bond.node_to)
             bond.node_to.bond_1 = bond
-            self.parameters.update(bond.node_to.parameter_symbols())
 
         bond.num = len(self._bonds) + 1
         bond.flow_symbol = Symbol(f"f_{bond.num}")
         bond.effort_symbol = Symbol(f"e_{bond.num}")
 
         self._bonds.append(bond)
```

### Comparing `bondgraph-0.1.1/src/bondgraph/elements/basic.py` & `bondgraph-0.2.0/src/bondgraph/elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from sympy import Symbol, Equality, Expr
-from typing import List, Set, Tuple
+from typing import List, Tuple
 from bondgraph.common import Causality, Node, Bond, HasStateEquations
 
 import logging
 
 
 class OnePortElement(Node):
     def __init__(self, name: str):
@@ -22,17 +22,14 @@
 
     def assign_arbitrary_causality(self) -> bool:
         return False
 
     def __str__(self) -> str:
         return self.name
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        raise NotImplementedError()
-
 
 class TwoPortElement(Node):
     def __init__(self, name: str):
         super().__init__(name)
         self.bond_1: Bond | None = None
         self.bond_2: Bond | None = None
 
@@ -43,17 +40,14 @@
 
     def assign_constraint_causality(self) -> bool:
         return False
 
     def __str__(self) -> str:
         return self.name
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        raise NotImplementedError()
-
 
 class Element_R(OnePortElement):
     def __init__(self, name: str, symbol: Symbol):
         super().__init__(name)
         self.symbol = symbol
 
     def equations(self, effort: Symbol, flow: Symbol) -> List[Equality]:
@@ -75,17 +69,14 @@
             self.bond.effort_in_at_to = True
             logging.debug(
                 f"Set indifferent effort-in causality at {self.bond.node_to} (vs {self.bond.node_from})"
             )
             return True
         return False
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        return {self.symbol}
-
     def visualization_label(self) -> str:
         return f"R: {self.symbol}"
 
 
 class Element_C(OnePortElement, HasStateEquations):
     def __init__(self, name: str, compliance: Symbol, displacement: Symbol):
         super().__init__(name)
@@ -118,17 +109,14 @@
                 self.bond.effort_in_at_to = False
                 logging.debug(
                     f"Set preferred effort-out causality at {self.bond.node_to} (vs {self.bond.node_from})"
                 )
                 return True
         return False
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        return {self._compliance}
-
     def visualization_label(self) -> str:
         return f"C: {self._compliance}"
 
 
 class Element_I(OnePortElement, HasStateEquations):
     def __init__(self, name: str, inertia: Symbol, momentum: Symbol):
         super().__init__(name)
@@ -161,17 +149,14 @@
                 self.bond.effort_in_at_to = True
                 logging.debug(
                     f"Set preferred effort-in causality at {self.bond.node_to} (vs {self.bond.node_from})"
                 )
                 return True
         return False
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        return {self._inertia}
-
     def visualization_label(self) -> str:
         return f"I: {self._inertia}"
 
 
 class Source_effort(OnePortElement):
     def __init__(self, name: str, symbol: Symbol):
         super().__init__(name)
@@ -198,17 +183,14 @@
                 self.bond.effort_in_at_to = False
                 logging.debug(
                     f"Set fixed effort-out causality at {self.bond.node_to} (vs {self.bond.node_from})"
                 )
                 return True
         return False
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        return {self.symbol}
-
     def visualization_label(self) -> str:
         return f"Se: {self.symbol}"
 
 
 class Source_flow(OnePortElement):
     def __init__(self, name: str, symbol: Symbol):
         super().__init__(name)
@@ -235,17 +217,14 @@
                 self.bond.effort_in_at_to = True
                 logging.debug(
                     f"Set fixed effort-in causality at {self.bond.node_to} (vs {self.bond.node_from})"
                 )
                 return True
         return False
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        return {self.symbol}
-
     def visualization_label(self) -> str:
         return f"Sf: {self.symbol}"
 
 
 class Transformer(TwoPortElement):
     def __init__(self, name: str, ratio: Symbol):
         super().__init__(name)
@@ -290,17 +269,14 @@
             logging.debug(
                 f"Set constrained {msg_dir} causality at {self.bond_1.node_to} "
                 + f"(vs {self.bond_1.node_from}) due to transformer {self}"
             )
             return True
         return False
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        return {self.ratio}
-
     def visualization_label(self) -> str:
         return f"TF\n{self.ratio}"
 
 
 class Gyrator(TwoPortElement):
     def __init__(self, name: str, ratio: Symbol):
         super().__init__(name)
@@ -344,12 +320,9 @@
             logging.debug(
                 f"Set constrained {msg_dir} causality at {self.bond_1.node_to} "
                 + f"(vs {self.bond_1.node_from}) due to gyrator {self}"
             )
             return True
         return False
 
-    def parameter_symbols(self) -> Set[Symbol]:
-        return {self.ratio}
-
     def visualization_label(self) -> str:
         return f"GY\n{self.ratio}"
```

### Comparing `bondgraph-0.1.1/src/bondgraph/junctions.py` & `bondgraph-0.2.0/src/bondgraph/junctions.py`

 * *Files identical despite different names*

### Comparing `bondgraph-0.1.1/src/bondgraph/visualization.py` & `bondgraph-0.2.0/src/bondgraph/visualization.py`

 * *Files identical despite different names*

### Comparing `bondgraph-0.1.1/src/bondgraph.egg-info/PKG-INFO` & `bondgraph-0.2.0/src/bondgraph.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondgraph
-Version: 0.1.1
+Version: 0.2.0
 Summary: A library to create bond graphs for physical systems and generate their differential equations.
 Author-email: Karl Linderhed <bondgraph@karlinde.se>
 License: MIT License
         
         Copyright (c) 2022 Karl Linderhed
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,16 +32,14 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: visualization
 License-File: LICENSE
 
 # bondgraph
-[![Python package](https://github.com/Karlinde/bondgraph/actions/workflows/python-package.yaml/badge.svg)](https://github.com/Karlinde/bondgraph/actions/workflows/python-package.yaml)
-
 A python library for creating [bond graphs](https://en.wikipedia.org/wiki/Bond_graph) of 
 physical systems and generating differential equations.
 
 It heavily relies on `sympy` for manipulation and simplification of equations symbolically.
 
 ## Installation
 Install via pip:
@@ -62,15 +60,15 @@
 # Se ---> 1 ---> I
 #         |
 #         v
 #         R
 
 from bondgraph.core import Bond, BondGraph
 from bondgraph.junctions import JunctionEqualFlow
-from bondgraph.elements.basic import Element_R, Element_I, Source_effort
+from bondgraph.elements import Element_R, Element_I, Source_effort
 from sympy import Symbol
 
 force = Source_effort("force", Symbol("F"))
 friction = Element_R("friction", Symbol("k_f"))
 inertia = Element_I("inertia", Symbol("m"), Symbol("p"))
 mass_object = JunctionEqualFlow("mass_object")
```

### Comparing `bondgraph-0.1.1/src/bondgraph.egg-info/SOURCES.txt` & `bondgraph-0.2.0/src/bondgraph.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 .gitignore
 CHANGELOG.md
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/python-package.yaml
 .github/workflows/release.yml
-examples/simple.py
+examples/custom_element.py
+examples/simple_graph.py
 src/bondgraph/__init__.py
 src/bondgraph/common.py
 src/bondgraph/core.py
+src/bondgraph/elements.py
 src/bondgraph/junctions.py
 src/bondgraph/visualization.py
 src/bondgraph.egg-info/PKG-INFO
 src/bondgraph.egg-info/SOURCES.txt
 src/bondgraph.egg-info/dependency_links.txt
 src/bondgraph.egg-info/requires.txt
 src/bondgraph.egg-info/top_level.txt
-src/bondgraph/elements/__init__.py
-src/bondgraph/elements/basic.py
-src/bondgraph/elements/hydraulics.py
 tests/test_core.py
```

### Comparing `bondgraph-0.1.1/tests/test_core.py` & `bondgraph-0.2.0/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bondgraph.common import AlgebraicLoopError
 from bondgraph.core import Bond, BondGraph
 from bondgraph.junctions import JunctionEqualEffort, JunctionEqualFlow
-from bondgraph.elements.basic import (
+from bondgraph.elements import (
     Element_R,
     Element_I,
     Element_C,
     Transformer,
     Source_effort,
     Source_flow,
 )
```

