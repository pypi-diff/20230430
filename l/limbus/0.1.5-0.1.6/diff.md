# Comparing `tmp/limbus-0.1.5.tar.gz` & `tmp/limbus-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limbus-0.1.5.tar", last modified: Wed Mar 15 22:27:50 2023, max compression
+gzip compressed data, was "limbus-0.1.6.tar", last modified: Sun Apr 30 16:07:02 2023, max compression
```

## Comparing `limbus-0.1.5.tar` & `limbus-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:27:50.314666 limbus-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-15 22:27:45.000000 limbus-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-03-15 22:27:50.314666 limbus-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-03-15 22:27:45.000000 limbus-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:27:50.310665 limbus-0.1.5/limbus/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:27:50.314666 limbus-0.1.5/limbus/core/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/core/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/core/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    24956 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/core/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/core/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/core/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:27:50.314666 limbus-0.1.5/limbus/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/widgets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/widgets/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus/widgets/widget_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:27:50.314666 limbus-0.1.5/limbus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-03-15 22:27:50.000000 limbus-0.1.5/limbus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-15 22:27:50.000000 limbus-0.1.5/limbus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:27:50.000000 limbus-0.1.5/limbus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-15 22:27:50.000000 limbus-0.1.5/limbus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-15 22:27:50.000000 limbus-0.1.5/limbus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:27:50.314666 limbus-0.1.5/limbus_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-15 22:27:45.000000 limbus-0.1.5/limbus_config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-15 22:27:50.314666 limbus-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-15 22:27:45.000000 limbus-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:07:02.099849 limbus-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 16:06:53.000000 limbus-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-30 16:07:02.099849 limbus-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-30 16:06:53.000000 limbus-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:07:02.099849 limbus-0.1.6/limbus/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:07:02.099849 limbus-0.1.6/limbus/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/core/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28683 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/core/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/core/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21089 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/core/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:07:02.099849 limbus-0.1.6/limbus/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/widgets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/widgets/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus/widgets/widget_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:07:02.099849 limbus-0.1.6/limbus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-30 16:07:02.000000 limbus-0.1.6/limbus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-30 16:07:02.000000 limbus-0.1.6/limbus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:07:02.000000 limbus-0.1.6/limbus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-30 16:07:02.000000 limbus-0.1.6/limbus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 16:07:02.000000 limbus-0.1.6/limbus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:07:02.099849 limbus-0.1.6/limbus_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-30 16:06:53.000000 limbus-0.1.6/limbus_config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-30 16:07:02.099849 limbus-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-30 16:06:53.000000 limbus-0.1.6/setup.py
```

### Comparing `limbus-0.1.5/LICENSE` & `limbus-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `limbus-0.1.5/PKG-INFO` & `limbus-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limbus
-Version: 0.1.5
+Version: 0.1.6
 Summary: High level interface to create Pytorch Graphs.
 Home-page: https://github.com/kornia/limbus
 Author: Luis Ferraz
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: components
 Provides-Extra: widgets
```

### Comparing `limbus-0.1.5/README.md` & `limbus-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `limbus-0.1.5/limbus/core/__init__.py` & `limbus-0.1.6/limbus/core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from limbus.core.component import Component, iterations_manager
+from limbus.core.component import Component, executions_manager
 from limbus.core.states import ComponentState, PipelineState, VerboseMode
-from limbus.core.param import NoValue, Param, Reference, InputParam, OutputParam
-from limbus.core.params import Params, InputParams, OutputParams
+from limbus.core.param import NoValue, Reference, InputParam, OutputParam, PropertyParam
+from limbus.core.params import PropertyParams, InputParams, OutputParams
 from limbus.core.pipeline import Pipeline
 from limbus.core.app import App
 
 
 __all__ = [
     "App",
     "Pipeline",
     "PipelineState",
     "VerboseMode",
     "Component",
-    "iterations_manager",
+    "executions_manager",
     "ComponentState",
-    "Params",
     "Reference",
+    "PropertyParams",
     "InputParams",
     "OutputParams",
+    "PropertyParam",
     "InputParam",
     "OutputParam",
-    "Param",
     "NoValue"]
```

### Comparing `limbus-0.1.5/limbus/core/app.py` & `limbus-0.1.6/limbus/core/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """High level template to create apps."""
-from typing import List
+from __future__ import annotations
 from abc import abstractmethod
 
 from limbus.core import Pipeline, VerboseMode, Component
 
 
 class App:
     """High level template to create an app."""
@@ -11,15 +11,15 @@
         self.create_components()
         self.connect_components()
         # Create the pipeline
         self._pipeline = Pipeline()
         self._pipeline.add_nodes(self._get_component_attrs())
         self._pipeline.set_verbose_mode(VerboseMode.DISABLED)
 
-    def _get_component_attrs(self) -> List[Component]:
+    def _get_component_attrs(self) -> list[Component]:
         """Get the component attribute by name."""
         return [getattr(self, attr) for attr in dir(self) if isinstance(getattr(self, attr), Component)]
 
     @abstractmethod
     def create_components(self):
         """Create the components of the app."""
         pass
```

### Comparing `limbus-0.1.5/limbus/core/component.py` & `limbus-0.1.6/limbus/core/component.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Component definition."""
 from __future__ import annotations
 from abc import abstractmethod
-from typing import List, Optional, TYPE_CHECKING, Callable, Type, Union, Any, Coroutine
+from functools import partial
+from typing import TYPE_CHECKING, Callable, Type, Any, Coroutine
 import logging
 import asyncio
 import traceback
 import functools
 
 try:
     import torch.nn as nn
 except ImportError:
     pass
 
 from limbus_config import config
-from limbus.core.params import Params, InputParams, OutputParams
+from limbus.core.params import InputParams, OutputParams, PropertyParams
 from limbus.core.states import ComponentState, ComponentStoppedError
 # Note that Pipeline class cannot be imported to avoid circular dependencies.
 if TYPE_CHECKING:
     from limbus.core.pipeline import Pipeline
 
 log = logging.getLogger(__name__)
 
@@ -31,68 +32,94 @@
     except NameError:
         log.error("Torch not installed. Using generic base class.")
 else:
     log.error("Invalid component type. Using generic base class.")
 
 
 # this is a decorator that will determine how many iterations must be run
-def iterations_manager(func: Callable) -> Callable:
-    """Update the last iteration to be run by the component."""
+def executions_manager(func: Callable) -> Callable:
+    """Update the last execution to be run by the component."""
     @functools.wraps(func)
     async def wrapper_set_iteration(self, *args, **kwargs):
-        if self._pipeline is not None:
-            self._stopping_iteration = self._pipeline.get_component_stopping_iteration(self)
+        if self.pipeline is not None:
+            self.stopping_execution = self.pipeline.get_component_stopping_iteration(self)
         return await func(self, *args, **kwargs)
     return wrapper_set_iteration
 
 
 class _ComponentState():
     """Manage the state of the component.
 
+    Note that the state can be multiple.
+    The user interactions are the ones allowing simultaneous states, concretelly:
+        - ComponentState.STOPPED_AT_ITER
+        - ComponentState.STOPPED_BY_COMPONENT (it is generated by the STOPPED_AT_ITER state in other components)
+        - ComponentState.FORCED_STOP
+    E.g., a component can be properly executed and at the same time stopped by the user.
+
     Args:
         component (Component): component to manage.
         state (ComponentState): initial state.
         verbose (bool, optional): verbose state. Default: False.
 
     """
     def __init__(self, component: Component, state: ComponentState, verbose: bool = False):
-        self._state: ComponentState = state
+        self._states: list[ComponentState] = [state]
+        self._messages: dict[ComponentState, None | str] = {state: None}
         self._component: Component = component
         self._verbose: bool = verbose
 
-    def __call__(self, state: Optional[ComponentState] = None, msg: Optional[str] = None) -> ComponentState:
-        """Set the state of the component.
+    def __call__(self, state: None | ComponentState = None, msg: None | str = None, add: bool = False
+                 ) -> list[ComponentState]:
+        """Set or add a new state for the component.
 
         If no args are passed, it returns the current state.
 
         Args:
             state (optional): state to set. Default: None.
             msg (optional): message to log. Default: None.
+            add (optional): if True, the state is added to the list of states. Default: False.
 
         Returns:
-            The state of the component.
+            The state or states of the component.
 
         """
         if state is not None:
-            self._state = state
-            self._logger(self._component.name, self._component.counter, self._state, msg)
-        return self._state
+            if add:
+                self._states.append(state)
+                self._messages[state] = msg
+            else:
+                self._states = [state]
+                self._messages = {state: msg}
+            self._logger()
+        return self._states
 
-    def _logger(self, comp_name: str, iters: int, state: ComponentState, msg: Optional[str]) -> None:
+    def _logger(self) -> None:
         """Log the message with the component name, iteration number and state."""
         if self._verbose:
-            if msg is None:
-                log.info(f" {comp_name}({iters}): {state.name}")
-            else:
-                log.info(f" {comp_name}({iters}): {state.name} ({msg})")
+            num_states = len(self._states)
+            for idx, state in enumerate(self._states):
+                msg = self._messages.get(state, None)
+                msg_str: str = f""
+                if num_states > 1:
+                    msg_str = f" {idx + 1}/{num_states}"
+                msg_str = f"{msg_str} {self._component.name}({self._component.executions_counter}): {state.name}"
+                if msg is not None:
+                    # concat the message
+                    msg_str = f"{msg_str} ({msg})"
+                log.info(msg_str)
+
+    def message(self, state: ComponentState) -> None | str:
+        """Get the message associated to the state. If state is not found, returns None."""
+        return self._messages.get(state, None)
 
     @property
-    def state(self) -> ComponentState:
+    def state(self) -> list[ComponentState]:
         """Get the state of the component."""
-        return self._state
+        return self._states
 
     @property
     def verbose(self) -> bool:
         """Get the verbose state."""
         return self._verbose
 
     @verbose.setter
@@ -112,75 +139,103 @@
     def __init__(self, name: str):
         super().__init__()
         self._name = name
         self._inputs = InputParams(self)
         self.__class__.register_inputs(self._inputs)
         self._outputs = OutputParams(self)
         self.__class__.register_outputs(self._outputs)
-        self._properties = Params(self)
+        self._properties = PropertyParams(self)
         self.__class__.register_properties(self._properties)
-        self._resume_event: Optional[asyncio.Event] = None
-        self._state: _ComponentState = _ComponentState(self, ComponentState.INITIALIZED)
-        self._pipeline: Optional[Pipeline] = None
-        self._exec_counter: int = 0  # Counter of executions.
+        self.__state: _ComponentState = _ComponentState(self, ComponentState.INITIALIZED)
+        self.__pipeline: None | Pipeline = None
+        self.__exec_counter: int = 0  # Counter of executions.
         # Last execution to be run in the __call__ loop.
-        self._stopping_iteration: int = 0  # 0 means run forever
+        self.__stopping_execution: int = 0  # 0 means run forever
+        self.__num_params_waiting_to_receive: int = 0  # updated from InputParam
+
+        # method called in __run_with_hooks to execute the component forward method
+        self.__run_forward: Callable[..., Coroutine[Any, Any, ComponentState]] = self.forward
+        try:
+            if nn.Module in Component.__mro__:
+                # If the component inherits from nn.Module, the forward method is called by the __call__ method
+                self.__run_forward = partial(nn.Module.__call__, self)
+        except NameError:
+            pass
 
-        # method called in _run_with_hooks to execute the component forward method
-        self._run_forward: Callable[..., Coroutine[Any, Any, ComponentState]] = self.forward
-        if nn.Module in Component.__mro__:
-            # If the component inherits from nn.Module, the forward method is called by the __call__ method
-            self._run_forward = nn.Module.__call__
+    def __del__(self):
+        self.release()
+
+    def release(self) -> None:
+        """Event executed when the component ends its execution."""
+        pass
 
     def init_from_component(self, ref_component: Component) -> None:
         """Init basic execution params from another component.
 
         Args:
             ref_component: reference component.
 
         """
-        self._pipeline = ref_component._pipeline
-        if self._pipeline is not None:
-            self._pipeline.add_nodes(self)
+        self.__pipeline = ref_component.__pipeline
+        if self.__pipeline is not None:
+            self.__pipeline.add_nodes(self)
         self.verbose = ref_component.verbose
 
     @property
-    def counter(self) -> int:
+    def executions_counter(self) -> int:
         """Get the executions counter."""
-        return self._exec_counter
+        return self.__exec_counter
 
     @property
-    def stopping_iteration(self) -> int:
-        """Get the last iteration to be run by the component in the __call__ loop."""
-        return self._stopping_iteration
+    def stopping_execution(self) -> int:
+        """Get the last execution to be run by the component in the __call__ loop.
+
+        Note that extra executions can be forced by other components to be able to run their executions.
+
+        """
+        return self.__stopping_execution
+
+    @stopping_execution.setter
+    def stopping_execution(self, value: int) -> None:
+        """Set the last execution to be run by the component in the __call__ loop.
+
+        Note that extra executions can be forced by other components to be able to run their executions.
+
+        """
+        self.__stopping_execution = value
 
     @property
-    def state(self) -> ComponentState:
-        """Get the current state of the component."""
-        return self._state.state
+    def state(self) -> list[ComponentState]:
+        """Get the current state/s of the component."""
+        return self.__state.state
 
-    def set_state(self, state: ComponentState, msg: Optional[str] = None) -> None:
+    def state_message(self, state: ComponentState) -> None | str:
+        """Get the message associated a given current state of the component."""
+        return self.__state.message(state)
+
+    def set_state(self, state: ComponentState, msg: None | str = None, add: bool = False) -> None:
         """Set the state of the component.
 
         Args:
             state: state to set.
-            msg (optional): message to log.
+            msg (optional): message to log. Default: None.
+            add (optional): if True, the state is added to the list of states. Default: False.
 
         """
-        self._state(state, msg)
+        self.__state(state, msg, add)
 
     @property
     def verbose(self) -> bool:
         """Get the verbose state."""
-        return self._state.verbose
+        return self.__state.verbose
 
     @verbose.setter
     def verbose(self, value: bool) -> None:
         """Set the verbose state."""
-        self._state.verbose = value
+        self.__state.verbose = value
 
     @property
     def name(self) -> str:
         """Name of the component."""
         return self._name
 
     @property
@@ -190,88 +245,60 @@
 
     @property
     def outputs(self) -> OutputParams:
         """Get the set of component outputs."""
         return self._outputs
 
     @property
-    def properties(self) -> Params:
+    def properties(self) -> PropertyParams:
         """Get the set of properties for this component."""
         return self._properties
 
     @staticmethod
     def register_inputs(inputs: InputParams) -> None:
         """Register the input params.
 
         Args:
-            inputs: Params object to register the inputs.
+            inputs: object to register the inputs.
 
         """
         pass
 
     @staticmethod
     def register_outputs(outputs: OutputParams) -> None:
         """Register the output params.
 
         Args:
-            outputs: Params object to register the outputs.
+            outputs: object to register the outputs.
 
         """
         pass
 
     @staticmethod
-    def register_properties(properties: Params) -> None:
+    def register_properties(properties: PropertyParams) -> None:
         """Register the properties.
 
         These params are optional.
 
         Args:
-            properties: Params object to register the properties.
+            properties: object to register the properties.
 
         """
         pass
 
-    def set_properties(self, **kwargs) -> bool:
-        """Simplify the way to set the viz params.
-
-        You can pass all the viz params you want to set as keyword arguments.
-
-        These 2 codes are equivalent:
-        >> component.set_properties(param_name_0=value_0, param_name_1=value_1, ...)
-
-        and
-        >> component.properties.set_param('param_name_0', value_0)
-        >> component.properties.set_param('param_name_1', value_1)
-        >> .
-        >> .
-
-        Returns:
-            bool: True if all the passed viz params were setted, False otherwise.
-
-        """
-        all_ok = True
-        properties: List[str] = self._properties.get_params()
-        for key, value in kwargs.items():
-            if key in properties:
-                self._properties.set_param(key, value)
-            else:
-                log.warning(f"In component {self._name} the param {key} is not a valid viz param.")
-                all_ok = False
-        return all_ok
-
     @property
-    def pipeline(self) -> Optional[Pipeline]:
+    def pipeline(self) -> None | Pipeline:
         """Get the pipeline object."""
-        return self._pipeline
+        return self.__pipeline
 
-    def set_pipeline(self, pipeline: Optional[Pipeline]) -> None:
+    def set_pipeline(self, pipeline: None | Pipeline) -> None:
         """Set the pipeline running the component."""
-        self._pipeline = pipeline
+        self.__pipeline = pipeline
 
-    def _stop_component(self) -> None:
+    def __stop_component(self) -> None:
         """Prepare the component to be stopped."""
         for input in self._inputs.get_params():
             for ref in self._inputs[input].references:
                 assert ref.sent is not None
                 assert ref.consumed is not None
                 # unblock the events
                 ref.sent.set()
@@ -280,108 +307,82 @@
             for ref in self._outputs[output].references:
                 assert ref.sent is not None
                 assert ref.consumed is not None
                 # unblock the events
                 ref.sent.set()
                 ref.consumed.set()
 
-    @iterations_manager
+    @executions_manager
     async def __call__(self) -> None:
         """Execute the forward method.
 
         If the component is executed in a pipeline, the component runs forever. However,
         if the component is run alone it will run only once.
 
-        NOTE: If you want to use `async for...` instead of `while True` this method must be overridden.
+        NOTE 1: If you want to use `async for...` instead of `while True` this method must be overridden.
         E.g.:
             async for x in xyz:
-                if await self._run_with_hooks(x):
+                if await self.__run_with_hooks(x):
                     break
 
             Note that in this example the forward method will require 1 parameter.
 
+        NOTE 2: if you override this method you must add the `executions_manager` decorator.
+
         """
         while True:
-            if await self._run_with_hooks():
+            if await self.__run_with_hooks():
                 break
 
     def is_stopped(self) -> bool:
         """Check if the component is stopped or is going to be stopped."""
-        if self.state in [ComponentState.STOPPED, ComponentState.STOPPED_AT_ITER,
-                          ComponentState.ERROR, ComponentState.FORCED_STOP]:
+        if len(set(self.state).intersection(set([ComponentState.STOPPED, ComponentState.STOPPED_AT_ITER,
+                                                 ComponentState.ERROR, ComponentState.FORCED_STOP,
+                                                 ComponentState.STOPPED_BY_COMPONENT]))) > 0:
             return True
         return False
 
-    def _stop_if_needed(self) -> bool:
+    def __stop_if_needed(self) -> bool:
         """Stop the component if it is required."""
         if self.is_stopped():
-            if self.state is not ComponentState.STOPPED_AT_ITER:
+            if ComponentState.STOPPED_AT_ITER not in self.state:
                 # in this case we need to force the stop of the component. When it is stopped at a given iter
                 # the pipeline ends without forcing anything.
-                self._stop_component()
+                self.__stop_component()
             return True
         return False
 
-    async def _run_with_hooks(self, *args, **kwargs) -> bool:
-        self._exec_counter += 1
-        if self._pipeline is not None:
-            await self._pipeline.before_component_hook(self)
-            if self._stop_if_needed():
+    async def __run_with_hooks(self, *args, **kwargs) -> bool:
+        self.__exec_counter += 1
+        if self.__pipeline is not None:
+            await self.__pipeline.before_component_hook(self)
+            if self.__pipeline.before_component_user_hook:
+                await self.__pipeline.before_component_user_hook(self)
+            if self.__stop_if_needed():  # just in case the component state is changed in the before_component_hook
                 return True
         # run the component
         try:
             if len(self._inputs) == 0:
                 # RUNNING state is set once the input params are received, if there are not inputs the state is set here
                 self.set_state(ComponentState.RUNNING)
-            self.set_state(await self._run_forward(*args, **kwargs))
+            self.set_state(await self.__run_forward(*args, **kwargs))
         except ComponentStoppedError as e:
-            self.set_state(e.state)
+            self.set_state(e.state, e.message, add=True)
         except Exception as e:
             self.set_state(ComponentState.ERROR, f"{type(e).__name__} - {str(e)}")
             log.error(f"Error in component {self.name}.\n"
                       f"{''.join(traceback.format_exception(None, e, e.__traceback__))}")
-        if self._pipeline is not None:
+        if self.__pipeline is not None:
             # after component hook
-            await self._pipeline.after_component_hook(self)
-            if self._stop_if_needed():
+            await self.__pipeline.after_component_hook(self)
+            if self.__pipeline.after_component_user_hook:
+                await self.__pipeline.after_component_user_hook(self)
+            if self.__stop_if_needed():
                 return True
             return False
         # if there is not a pipeline, the component is executed only once
         return True
 
     @abstractmethod
     async def forward(self, *args, **kwargs) -> ComponentState:
         """Run the component, this method shouldn't be called, instead call __call__."""
         raise NotImplementedError
-
-    def finish_iter(self) -> None:
-        """Event executed when each pipeline iter finishes.
-
-        Note that this method can be defined as async if needed.
-
-        """
-        pass
-
-    def finish_pipeline(self) -> None:
-        """Event executed when the pipeline finishes.
-
-        Note that this method can be defined as async if needed.
-
-        """
-        pass
-
-    def init_iter(self) -> None:
-        """Event executed when each pipeline iter starts.
-
-        Note that this method can be defined as async if needed.
-
-        """
-        pass
-
-    def init_pipeline(self) -> None:
-        """Event executed when the pipeline starts.
-
-        Note that this method can be defined as async if needed.
-        For example this method is useful to init some await variables that cannot be initialized in the constructor.
-
-        """
-        pass
```

### Comparing `limbus-0.1.5/limbus/core/param.py` & `limbus-0.1.6/limbus/core/param.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Classes to define parameters."""
 from __future__ import annotations
 from dataclasses import dataclass
 from collections import defaultdict
 import typing
-from typing import Dict, Any, Set, Optional, List, Union, Tuple, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING, Callable
 import inspect
 import collections
 import asyncio
 import contextlib
+from abc import ABC
 
 import typeguard
 
 from limbus.core.states import ComponentState, ComponentStoppedError
 from limbus.core import async_utils
 # Note that Component class cannot be imported to avoid circular dependencies.
 if TYPE_CHECKING:
     from limbus.core.component import Component
 
-SUBSCRIPTABLE_TYPES: List[type] = []
+SUBSCRIPTABLE_TYPES: list[type] = []
 try:
     import torch
     SUBSCRIPTABLE_TYPES.append(torch.Tensor)
 except ImportError:
     pass
 
 try:
@@ -46,15 +47,15 @@
 class IterableContainer:
     """Denote that a param has an indexed value.
 
     Note: In our use case the maximum number of nested IterableContainers is 2.
     This number is not explicitly controlled. It is implicitly controlled in the Param class.
 
     """
-    container: Union[Container, "IterableContainer"]
+    container: Container | "IterableContainer"
     index: int
 
     @property
     def value(self) -> Any:
         """Get the value of the container."""
         if isinstance(self.container, Container):
             # return the value of the container at the index
@@ -64,19 +65,19 @@
             # If it is an IterableContainer means that the final value is nested.
             assert isinstance(self.container, IterableContainer)
             return self.container.value
 
 
 class IterableInputContainers:
     """Denote that an input param is a sequence of Containers."""
-    def __init__(self, container: Optional[IterableContainer] = None):
+    def __init__(self, container: None | IterableContainer = None):
         containers = []
         if container is not None:
             containers = [container]
-        self._containers: List[IterableContainer] = containers
+        self._containers: list[IterableContainer] = containers
 
     def __len__(self) -> int:
         return len(self._containers)
 
     def add(self, container: IterableContainer) -> None:
         """Add an IterableValue to the list of values."""
         self._containers.append(container)
@@ -84,24 +85,24 @@
     def remove(self, index: int) -> None:
         """Remove an IterableValue from the list of values."""
         for container in self._containers:
             if container.index == index:
                 self._containers.remove(container)
                 return
 
-    def get_ordered(self) -> List[Any]:
+    def get_ordered(self) -> list[Any]:
         """Return a list with the values in the order denoted by the index in the IterableValue."""
-        indices: List[int] = []
+        indices: list[int] = []
         for container in self._containers:
             assert isinstance(container, IterableContainer)
             indices.append(container.index)
 
-        containers: List[Any] = []
+        containers: list[Any] = []
         for pos_idx in sorted(range(len(indices)), key=indices.__getitem__):  # argsort
-            obj: Union[Container, IterableContainer] = self._containers[pos_idx].container
+            obj: Container | IterableContainer = self._containers[pos_idx].container
             if isinstance(obj, IterableContainer):
                 obj = obj.container.value[obj.index]  # type: ignore  # Iterable[Any] is not indexable [index]
             else:
                 assert isinstance(obj, Container)
                 obj = obj.value
             containers.append(obj)
         return containers
@@ -113,23 +114,21 @@
     Args:
         datatype (type): type to be analised.
 
     Returns:
         bool: True if datatype is a subscriptable with tensors, False otherwise.
 
     """
-    if inspect.isclass(datatype):
-        return False
-
-    # in this case is a typing expresion
     # we need to know if it is a variable size datatype, we assume that all the sequences are variable size
-    # if they contain tensors. E.g. List[Tensor], Tuple[Tensor], Sequence[Tensor].
-    # Note that e.g. for the case Tuple[Tensor, Tensor] we don't assume it is variable since the size is known.
+    # if they contain tensors. E.g. list[Tensor], tuple[Tensor], Sequence[Tensor].
+    # Note that e.g. for the case tuple[Tensor, Tensor] we don't assume it is variable since the size is known.
     origin = typing.get_origin(datatype)
-    datatype_args: Tuple = typing.get_args(datatype)
+    if origin is None:  # discard datatypes that are not typing expressions
+        return False
+    datatype_args: tuple = typing.get_args(datatype)
     if inspect.isclass(origin):
         is_abstract: bool = inspect.isabstract(origin)
         is_abstract_seq: bool = origin is collections.abc.Sequence or origin is collections.abc.Iterable
         # mypy complaints in the case origin is NoneType
         if is_abstract_seq or (not is_abstract and isinstance(origin(), typing.Iterable)):  # type: ignore
             if (len(datatype_args) == 1 or (len(datatype_args) == 2 and Ellipsis in datatype_args)):
                 if datatype_args[0] in SUBSCRIPTABLE_TYPES:
@@ -138,15 +137,15 @@
 
 
 class IterableParam:
     """Temporal class to manage indexing inside a parameter."""
     def __init__(self, param: "Param", index: int) -> None:
         self._param: Param = param
         # TODO: validate that _iter_container can be an IterableInputContainers, I feel it cannot!!
-        self._iter_container: Union[IterableContainer, IterableInputContainers]
+        self._iter_container: IterableContainer | IterableInputContainers
         if isinstance(param.container, Container):
             self._iter_container = IterableContainer(param.container, index)
         elif isinstance(param.container, IterableInputContainers):
             # since it is an input, the pointer to the value is not relevant at this stage
             self._iter_container = IterableContainer(Container(None), index)
 
     @property
@@ -158,151 +157,172 @@
     def index(self) -> int:
         """Return the selected index in the sequence."""
         if isinstance(self._iter_container, IterableInputContainers):
             raise TypeError("Cannot get the index of a list of input containers.")
         return self._iter_container.index
 
     @property
-    def value(self) -> Union[Any, List[Any]]:
+    def value(self) -> Any | list[Any]:
         """Get the value of the parameter.
 
         It can be a list of values if the parameter is an IterableInputContainers.
 
         """
         if isinstance(self._iter_container, IterableContainer):
             return self._iter_container.value
         else:
             assert isinstance(self._iter_container, IterableInputContainers)
             return self._iter_container.get_ordered()
 
     @property
-    def iter_container(self) -> Union[IterableContainer, IterableInputContainers]:
+    def iter_container(self) -> IterableContainer | IterableInputContainers:
         """Get the container of the parameter."""
         return self._iter_container
 
     def ref_counter(self) -> int:
         """Return the number of references for this parameter."""
         if isinstance(self._iter_container, IterableInputContainers):
             raise TypeError("At this moment the number of references for IterableInputContainers cannot be retrieved.")
         return self._param.ref_counter(self._iter_container.index)
 
-    def connect(self, dst: Union["Param", "IterableParam"]) -> None:
+    def connect(self, dst: "Param" | "IterableParam") -> None:
         """Connect this parameter (output) with the dst (input) parameter."""
         self._param._connect(self, dst)
 
-    def __rshift__(self, rvalue: Union["Param", "IterableParam"]):
+    def __rshift__(self, rvalue: "Param" | "IterableParam"):
         """Allow to connect params using the >> operator."""
         self.connect(rvalue)
 
-    def disconnect(self, dst: Union["Param", "IterableParam"]) -> None:
+    def disconnect(self, dst: "Param" | "IterableParam") -> None:
         """Disconnect this parameter (output) with the dst (input) parameter."""
         self._param._disconnect(self, dst)
 
 
 @dataclass
 class Reference:
     """Reference to a parameter.
 
     It is used to keep track of the references to a parameter.
 
     """
     param: "Param"
-    index: Optional[int] = None
+    ori_param: "Param"  # added to avoid duplicated references, it is rare but it could happen.
+    index: None | int = None
+    ori_index: None | int = None  # added to avoid duplicated references, it is rare but it could happen.
     # allow to know if there is a new value for the parameter
-    sent: Optional[asyncio.Event] = None
+    sent: None | asyncio.Event = None
     # allow to know if the value has been consumed
-    consumed: Optional[asyncio.Event] = None
+    consumed: None | asyncio.Event = None
 
     def __hash__(self) -> int:
         # this method is required to be able to use Reference in a set.
         # Note that we don't use the consumed attribute in the hash since it is dynamic.
-        return hash((self.param, self.index))
+        return hash((self.param, self.index, self.ori_param, self.ori_index))
 
     def __eq__(self, other: Any) -> bool:
         # this method is required to be able to use Reference in a set.
         # Note that we don't use the consumed attribute in the hash since it is dynamic.
         if isinstance(other, Reference):
-            return self.param == other.param and self.index == other.index
+            return (self.param == other.param and self.index == other.index and
+                    self.ori_param == other.ori_param and self.ori_index == other.ori_index)
         return False
 
 
-class Param:
-    """Class to store data for each parameter.
+class Param(ABC):
+    """Base class to store data for each parameter.
 
     Args:
         name: name of the parameter.
         tp (optional): type of the parameter. Madnatory for subscriptable params. Default: Any.
         value (optional): value of the parameter. Default: NoValue().
         arg (optional): name of the argument in the component constructor related with this param. Default: None.
         parent (optional): parent component. Default: None.
+        callback (optional): async callback to be called when the value of the parameter changes.
+            Prototype: `async def callback(parent: Component, value: TYPE) -> TYPE:`
+                - MUST return the value to be finally used.
+            Default: None.
 
     """
-    def __init__(self, name: str, tp: Any = Any, value: Any = NoValue(), arg: Optional[str] = None,
-                 parent: Optional[Component] = None) -> None:
+    def __init__(self, name: str, tp: Any = Any, value: Any = NoValue(), arg: None | str = None,
+                 parent: None | Component = None, callback: Callable | None = None) -> None:
         # validate that the type is coherent with the value
         if not isinstance(value, NoValue):
             typeguard.check_type(name, value, tp)
 
         self._name: str = name
         self._type: Any = tp
-        self._arg: Optional[str] = arg
+        self._arg: None | str = arg
         # We store all the references for each param.
         # The key is the slicing for the current param.
-        self._refs: Dict[Any, Set[Reference]] = defaultdict(set)
-        self._value: Union[Container, IterableContainer, IterableInputContainers] = Container(value)
+        self._refs: dict[Any, set[Reference]] = defaultdict(set)
+        self._value: Container | IterableContainer | IterableInputContainers = Container(value)
         # only sequences with tensors inside are subscriptable
         self._is_subscriptable = _check_subscriptable(tp)
-        self._parent: Optional[Component] = parent
+        self._parent: None | Component = parent
+        self._callback: None | Callable = callback
 
     @property
-    def parent(self) -> Optional[Component]:
+    def is_subscriptable(self) -> bool:
+        """Return if the parameter is subscriptable."""
+        return self._is_subscriptable
+
+    def reset_is_subscriptable(self) -> None:
+        """Reset the subscriptable flag."""
+        self._is_subscriptable = _check_subscriptable(self._type)
+
+    def set_as_non_subscriptable(self) -> None:
+        """Set the subscriptable flag to False."""
+        self._is_subscriptable = False
+
+    @property
+    def parent(self) -> None | Component:
         """Get the parent component."""
         return self._parent
 
     @property
-    def arg(self) -> Optional[str]:
-        """Get the argument related with the param."""
+    def arg(self) -> None | str:
+        """Get the argument in the Component constructor related with this param.
+
+        This is a trick to pass a value and type of an argument in the Component constructor to this parameter.
+
+        """
         return self._arg
 
     @property
     def type(self) -> Any:
         """Return the type of the parameter."""
         return self._type
 
     @property
     def name(self) -> str:
         """Get the name of the parameter."""
         return self._name
 
     @property
-    def references(self) -> Set[Reference]:
+    def references(self) -> set[Reference]:
         """Get all the references for the parameter."""
-        refs: Set[Reference] = set()
+        refs: set[Reference] = set()
         for ref_set in self._refs.values():
             refs = refs.union(ref_set)
         return refs
 
-    def __call__(self) -> Any:
-        """Get the value of the parameter."""
-        return self.value
-
     @property
     def value(self) -> Any:
         """Get the value of the parameter."""
         if isinstance(self._value, Container):
             if isinstance(self._value.value, IterableContainer):
                 # mypy error: Iterable[Any] is not indexable [index]
                 return self._value.value.container.value[self._value.value.index]  # type: ignore
             else:
                 return self._value.value
         elif isinstance(self._value, IterableInputContainers):
             assert self._is_subscriptable
             origin = typing.get_origin(self._type)
             assert origin is not None
-            res_value: List[Any] = self._value.get_ordered()
+            res_value: list[Any] = self._value.get_ordered()
             return origin(res_value)
 
     @value.setter
     def value(self, value: Any) -> None:
         """Set the value of the parameter.
 
         Args:
@@ -313,36 +333,36 @@
 
     def _set_value(self, value: Any) -> None:
         # trick to easily override the setter of the value property
         if isinstance(value, Param):
             value = value.value
         if not isinstance(self._value, Container):
             raise TypeError(f"Param '{self.name}' cannot be assigned.")
-        if isinstance(value, (Container, IterableContainer, Set)):
+        if isinstance(value, (Container, IterableContainer, set)):
             raise TypeError(
                 f"The type of the value to be assigned to param '{self.name}' cannot have a 'value' attribute.")
         typeguard.check_type(self._name, value, self._type)
         self._value.value = value
 
     @property
-    def container(self) -> Union[Container, IterableContainer, IterableInputContainers]:
+    def container(self) -> Container | IterableContainer | IterableInputContainers:
         """Get the container for this parameter."""
         return self._value
 
     @container.setter
-    def container(self, value: Union[Container, IterableContainer, IterableInputContainers]) -> None:
+    def container(self, value: Container | IterableContainer | IterableInputContainers) -> None:
         """Set the container for this parameter.
 
         Args:
             value (Container, IterableContainer or IterableInputContainers): The container to set.
 
         """
         self._value = value
 
-    def ref_counter(self, index: Optional[int] = None) -> int:
+    def ref_counter(self, index: None | int = None) -> int:
         """Return the number of references for this parameter."""
         if index is not None:
             return len(self._refs[index])
         else:
             return len(self.references)
 
     def select(self, index: int) -> IterableParam:
@@ -357,24 +377,24 @@
         """
         if not self._is_subscriptable:
             raise ValueError(f"The param '{self.name}' is not subscriptable (it must be a sequence of tensors).")
         # NOTE: we cannot check if the index is valid because it is not known at this point the len of the sequence
         # create a new param with the selected slice inside the param
         return IterableParam(self, index)
 
-    def _connect(self, ori: Union["Param", IterableParam], dst: Union["Param", IterableParam]) -> None:
+    def _connect(self, ori: "Param" | IterableParam, dst: "Param" | IterableParam) -> None:
         """Connect this parameter (output) with the dst (input) parameter."""
         # Disable this check until a better solution is found to connect 2 lists.
         # if isinstance(ori, Param) and ori._is_subscriptable:
         #    raise ValueError(f"The param '{ori.name}' must be connected using indexes.")
 
         # if isinstance(dst, Param) and dst._is_subscriptable:
         #    raise ValueError(f"The param '{dst.name}' must be connected using indexes.")
 
-        # NOTE that there are not type validation, we will trust in the user to connect params.
+        # NOTE that there is not type validation, we will trust in the user to connect params.
         # We only check when there is an explicit value in the ori param.
         if isinstance(ori, Param) and not isinstance(ori.value, NoValue):
             if isinstance(dst, Param):
                 typeguard.check_type(self._name, ori.value, dst.type)
             else:
                 typeguard.check_type(self._name, ori.value, typing.get_args(dst.param.type)[0])
 
@@ -415,23 +435,23 @@
             if isinstance(dst.param.container, IterableInputContainers):
                 dst.param.container.add(dst.iter_container)
             else:
                 dst.param.container = IterableInputContainers(dst.iter_container)
 
         self._update_references('add', ori, dst)
 
-    def connect(self, dst: Union["Param", IterableParam]) -> None:
+    def connect(self, dst: "Param" | IterableParam) -> None:
         """Connect this parameter (output) with the dst (input) parameter."""
         self._connect(self, dst)
 
-    def __rshift__(self, rvalue: Union["Param", IterableParam]):
+    def __rshift__(self, rvalue: "Param" | IterableParam):
         """Allow to connect params using the >> operator."""
         self.connect(rvalue)
 
-    def _disconnect(self, ori: Union["Param", IterableParam], dst: Union["Param", IterableParam]) -> None:
+    def _disconnect(self, ori: "Param" | IterableParam, dst: "Param" | IterableParam) -> None:
         """Disconnect this parameter from the dst parameter."""
         if isinstance(dst, Param):
             assert isinstance(dst.container, Container)
             dst.container = Container(NoValue())
         elif isinstance(dst, IterableParam):
             if isinstance(dst.param.container, IterableInputContainers):
                 assert isinstance(dst.iter_container, IterableContainer)
@@ -439,15 +459,15 @@
                 if len(dst.param.container) == 0:
                     dst.param.container = Container(NoValue())
             else:
                 dst.param.container = Container(NoValue())
 
         self._update_references('remove', ori, dst)
 
-    def _update_references(self, type: str, ori: Union["Param", IterableParam], dst: Union["Param", IterableParam]
+    def _update_references(self, type: str, ori: "Param" | IterableParam, dst: "Param" | IterableParam
                            ) -> None:
         # assign references
         ori_idx = None
         dst_idx = None
         if isinstance(ori, IterableParam):
             ori_idx = ori.index
             ori = ori.param
@@ -455,45 +475,81 @@
             dst_idx = dst.index
             dst = dst.param
         if type == 'add':
             # Set events denoting that the param is sent/consumed. Note that the same events are set in the
             # references of both params.
             consumed_event = asyncio.Event()
             sent_event = asyncio.Event()
-            ori._refs[ori_idx].add(Reference(dst, dst_idx, sent_event, consumed_event))
-            dst._refs[dst_idx].add(Reference(ori, ori_idx, sent_event, consumed_event))
+            ori._refs[ori_idx].add(Reference(dst, ori, dst_idx, ori_idx, sent_event, consumed_event))
+            dst._refs[dst_idx].add(Reference(ori, dst, ori_idx, dst_idx, sent_event, consumed_event))
         elif type == 'remove':
-            ori._refs[ori_idx].remove(Reference(dst, dst_idx))
-            dst._refs[dst_idx].remove(Reference(ori, ori_idx))
+            ori._refs[ori_idx].remove(Reference(dst, ori, dst_idx, ori_idx))
+            dst._refs[dst_idx].remove(Reference(ori, dst, ori_idx, dst_idx))
 
-    def disconnect(self, dst: Union["Param", IterableParam]) -> None:
+    def disconnect(self, dst: "Param" | IterableParam) -> None:
         """Disconnect this parameter (output) from the dst (input) parameter."""
         self._disconnect(self, dst)
 
 
+class PropertyParam(Param):
+    """Class to manage the comunication for each property parameter."""
+
+    def init_property(self, value: Any) -> None:
+        """Initialize the property with the given value.
+
+        This method should be called before running the component to init the property.
+        So, it is not running the callback function.
+
+        """
+        # ComponentState.INITIALIZED means that the component was just created
+        if self._parent is not None and ComponentState.INITIALIZED not in self._parent.state:
+            raise RuntimeError("The property can only be initialized before running the component.")
+        self.value = value
+
+    async def set_property(self, value: Any) -> None:
+        """Set the value of the property.
+
+        Note: using this method is the only way to run the callback function.
+
+        """
+        assert self._parent is not None
+        if self._callback is None:
+            self.value = value
+        else:
+            self.value = await self._callback(self._parent, value)
+
+
 class InputParam(Param):
     """Class to manage the comunication for each input parameter."""
 
     async def receive(self) -> Any:
-        """Wait until the input param receives a value from the connected output param."""
+        """Wait until the input param receives a value from the connected output param.
+
+        Note that using this metohd will run the callback function as soon as a new value is received.
+        Note tha the callback changes teh result returned by the received method, not the value inside the
+            param (Param.value). This is in this way because the param can be shared between several input params,
+            so each callback call could change its value.
+
+        """
         assert self._parent is not None
+        self._parent._Component__num_params_waiting_to_receive += 1
         if self.references:
             for ref in self.references:
                 # NOTE: each input param can be connected to 0 or 1 output param (N output params if it is iterable).
                 # ref: Reference = next(iter(self.references))
                 # ensure the component related with the output param exists
                 assert ref.param is not None
                 ori_param: Param = ref.param
                 assert isinstance(ori_param, OutputParam)  # they must be of type OutputParam
                 assert ori_param.parent is not None
                 self._parent.set_state(ComponentState.RECEIVING_PARAMS,
                                        f"{ori_param.parent.name}.{ori_param.name} -> {self._parent.name}.{self.name}")
                 async_utils.create_task_if_needed(self._parent, ori_param.parent)
 
-            if self._parent.stopping_iteration == 0:
+            if self._parent.stopping_execution == 0:
                 # fast way, in contrast with the while loop below, to wait for the input param.
                 # wait until all the output params send the values
                 await asyncio.gather(*[ref.sent.wait() for ref in self.references if ref.sent is not None])
             else:
                 sent: int = 0
                 while sent < len(self.references):
                     for ref in self.references:
@@ -509,43 +565,63 @@
                             await asyncio.wait_for(ref.sent.wait(), timeout=0.1)
                     sent = sum([ref.sent.is_set() for ref in self.references if ref.sent is not None])
 
             for ref in self.references:
                 assert ref.param is not None
                 assert ref.param.parent is not None
                 # if we want to stop at a given min iter then it is posible to require more iters
-                if ref.param.parent.state is not ComponentState.STOPPED_AT_ITER and ref.param.parent.is_stopped():
-                    raise ComponentStoppedError(ref.param.parent.state)
+                if ComponentState.STOPPED_AT_ITER not in ref.param.parent.state and ref.param.parent.is_stopped():
+                    raise ComponentStoppedError(ComponentState.STOPPED_BY_COMPONENT)
 
             for ref in self.references:
                 # NOTE: depending on how the value is consumed we should apply a copy here.
                 # - We assume components do not modify the value. (this can happen)
                 # - When the value is setted reusing the same memory, instead of creating a new var, then
                 # the changes will also be propagated to components consuming the previous value. (in theory
                 # this cannot happen)
                 # TODO: add a flag to allow to determine if we want to copy the value.
                 value = self.value  # get the value before allowing to send again
                 assert isinstance(ref.sent, asyncio.Event)
                 assert isinstance(ref.consumed, asyncio.Event)
                 ref.consumed.set()  # denote that the param is consumed
                 ref.sent.clear()  # allow to know to the sender that it can send again
-                self._parent.set_state(ComponentState.RUNNING)
-            return value
         else:
+            value = self.value
+        if self._callback is not None:
+            # specific callback for this param
+            value = await self._callback(self._parent, value)
+        await self._are_all_waiting_params_received()
+        if self._parent.pipeline and self._parent.pipeline.param_received_user_hook:
+            # hook from the pipeline, all the components and input params run the same code
+            await self._parent.pipeline.param_received_user_hook(self)
+        return value
+
+    async def _are_all_waiting_params_received(self) -> None:
+        """Check if the component is waiting for other params before changing the component state."""
+        assert self._parent is not None
+        self._parent._Component__num_params_waiting_to_receive -= 1
+        if self._parent._Component__num_params_waiting_to_receive == 0:
             self._parent.set_state(ComponentState.RUNNING)
-            return self.value
 
 
 class OutputParam(Param):
     """Class to manage the comunication for each output parameter."""
 
     async def send(self, value: Any) -> None:
-        """Send the value of this param to the connected input params."""
+        """Send the value of this param to the connected input params.
+
+        Note that using this metohd will run the callback function as soon as a new value is received.
+
+        """
         assert self._parent is not None
-        self.value = value  # set the value for the param
+        if self._callback is None:
+            self.value = value  # set the value for the param
+        else:
+            self.value = await self._callback(self._parent, value)
+
         for ref in self.references:
             assert isinstance(ref.sent, asyncio.Event)
             assert isinstance(ref.consumed, asyncio.Event)
             ref.consumed.clear()  # init the state of the event
             ref.sent.set()  # denote that the param is ready to be consumed
 
             # ensure the component related with the input param exists
@@ -553,15 +629,18 @@
             dst_param: Param = ref.param
             assert isinstance(dst_param, InputParam)  # they must be of type InputParam
             assert dst_param.parent is not None
             self._parent.set_state(ComponentState.SENDING_PARAMS,
                                    f"{self._parent.name}.{self.name} -> {dst_param.parent.name}.{dst_param.name}")
             async_utils.create_task_if_needed(self._parent, dst_param.parent)
 
+        if self._parent.pipeline and self._parent.pipeline.param_sent_user_hook:
+            await self._parent.pipeline.param_sent_user_hook(self)
+
         # wait until all the input params read the value
         await asyncio.gather(*[ref.consumed.wait() for ref in self.references if ref.consumed is not None])
         for ref in self.references:
             assert ref.param is not None
             assert ref.param.parent is not None
             # if we want to stop at a given min iter then it is posible to require more iters
-            if ref.param.parent.state is not ComponentState.STOPPED_AT_ITER and ref.param.parent.is_stopped():
-                raise ComponentStoppedError(ref.param.parent.state)
+            if ComponentState.STOPPED_AT_ITER not in ref.param.parent.state and ref.param.parent.is_stopped():
+                raise ComponentStoppedError(ComponentState.STOPPED_BY_COMPONENT)
```

### Comparing `limbus-0.1.5/limbus/core/params.py` & `limbus-0.1.6/limbus/core/params.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,103 +1,47 @@
 """Classes to define set of parameters."""
-from typing import Dict, Any, Optional, List, Iterator, Iterable
+from __future__ import annotations
+from typing import Any, Iterator, Iterable, Callable
+from abc import ABC, abstractmethod
 
 # Note that Component class cannot be imported to avoid circular dependencies.
 # Since it is only used for type hints we import the module and use "component.Component" for typing.
 from limbus.core import component
-from limbus.core.param import Param, NoValue, InputParam, OutputParam
+from limbus.core.param import Param, NoValue, InputParam, OutputParam, PropertyParam
 
 
-class Params(Iterable):
+class Params(Iterable, ABC):
     """Class to store parameters."""
 
-    def __init__(self, parent_component: Optional["component.Component"] = None):
+    def __init__(self, parent_component: None | "component.Component" = None):
         super().__init__()
         self._parent = parent_component
 
-    def declare(self, name: str, tp: Any = Any, value: Any = NoValue(), arg: Optional[str] = None) -> None:
-        """Add or modify a param.
-
-        Args:
-            name: name of the parameter.
-            tp: type (e.g. str, int, list, Union[str, int]...). Default: typing.Any
-            value (optional): value for the parameter. Default: NoValue().
-            arg (optional): Component argument directly related with the value of the parameter. Default: None.
-                            E.g. this is useful to propagate datatypes and values from a pin with a default value to
-                            an argument in a Component (GUI).
-
-        """
-        if isinstance(value, Param):
-            value = value.value
-        setattr(self, name, Param(name, tp, value, arg, self._parent))
-
-    def __getattr__(self, name: str) -> Param:  # type: ignore  # it should return a Param
-        """Trick to avoid mypy issues with dinamyc attributes."""
-        ...
-
-    def get_related_arg(self, name: str) -> Optional[str]:
-        """Return the argument in the Component constructor related with a given param.
+    @abstractmethod
+    def declare(self, *args, **kwargs) -> None:
+        """Add or modify a param."""
+        raise NotImplementedError
 
-        Args:
-            name: name of the param.
-
-        """
-        return getattr(self, name).arg
-
-    def get_params(self, only_connected: bool = False) -> List[str]:
+    def get_params(self, only_connected: bool = False) -> list[str]:
         """Return the name of all the params.
 
         Args:
             only_connected: If True, only return the params that are connected.
 
         """
         params = []
         for name in self.__dict__:
             param = getattr(self, name)
             if isinstance(param, Param) and (not only_connected or param.ref_counter()):
                 params.append(name)
         return params
 
-    def get_types(self) -> Dict[str, type]:
-        """Return the name and the type of all the params."""
-        types: Dict[str, type] = {
-            name: getattr(self, name).type for name in self.__dict__ if not name.startswith('_')}
-        return types
-
-    def get_type(self, name: str) -> type:
-        """Return the type of a given param.
-
-        Args:
-            name: name of the param.
-
-        """
-        return getattr(self, name).type
-
-    def get_param(self, name: str) -> Any:
-        """Return the param value.
-
-        Args:
-            name: name of the param.
-
-        """
-        return getattr(self, name).value
-
     def __len__(self) -> int:
         return len(self.get_params())
 
-    def set_param(self, name: str, value: Any) -> None:
-        """Set the param value.
-
-        Args:
-            name: name of the param.
-            value: value to be setted.
-
-        """
-        getattr(self, name).value = value
-
     def __getitem__(self, name: str) -> Param:
         return getattr(self, name)
 
     def __iter__(self) -> Iterator[Param]:
         for name in self.__dict__:
             attr = getattr(self, name)
             if isinstance(attr, Param):
@@ -114,50 +58,77 @@
             )
         )
 
 
 class InputParams(Params):
     """Class to manage input parameters."""
 
-    def declare(self, name: str, tp: Any = Any, value: Any = NoValue(), arg: Optional[str] = None) -> None:
+    def declare(self, name: str, tp: Any = Any, value: Any = NoValue(), callback: Callable | None = None) -> None:
         """Add or modify a param.
 
         Args:
             name: name of the parameter.
-            tp: type (e.g. str, int, list, Union[str, int]...). Default: typing.Any
+            tp: type (e.g. str, int, list, str | int,...). Default: typing.Any
             value (optional): value for the parameter. Default: NoValue().
-            arg (optional): Component argument directly related with the value of the parameter. Default: None.
-                            E.g. this is useful to propagate datatypes and values from a pin with a default value to
-                            an argument in a Component (GUI).
+            callback (optional): async callback function to be called when the parameter value changes.
+                Prototype: `async def callback(parent: Component, value: TYPE) -> TYPE:`
+                    - MUST return the value to be finally used.
+                Default: None.
 
         """
         if isinstance(value, Param):
             value = value.value
-        setattr(self, name, InputParam(name, tp, value, arg, self._parent))
+        setattr(self, name, InputParam(name, tp, value, None, self._parent, callback))
 
     def __getattr__(self, name: str) -> InputParam:  # type: ignore  # it should return an InitParam
         """Trick to avoid mypy issues with dinamyc attributes."""
         ...
 
 
-class OutputParams(Params):
-    """Class to manage output parameters."""
+class PropertyParams(Params):
+    """Class to manage property parameters."""
 
-    def declare(self, name: str, tp: Any = Any, value: Any = NoValue(), arg: Optional[str] = None) -> None:
+    def declare(self, name: str, tp: Any = Any, value: Any = NoValue(), callback: Callable | None = None) -> None:
         """Add or modify a param.
 
         Args:
             name: name of the parameter.
-            tp: type (e.g. str, int, list, Union[str, int]...). Default: typing.Any
+            tp: type (e.g. str, int, list, str | int,...). Default: typing.Any
             value (optional): value for the parameter. Default: NoValue().
-            arg (optional): Component argument directly related with the value of the parameter. Default: None.
-                            E.g. this is useful to propagate datatypes and values from a pin with a default value to
-                            an argument in a Component (GUI).
+            callback (optional): async callback function to be called when the parameter value changes.
+                Prototype: `async def callback(parent: Component, value: TYPE) -> TYPE:`
+                    - MUST return the value to be finally used.
+                Default: None.
 
         """
         if isinstance(value, Param):
             value = value.value
-        setattr(self, name, OutputParam(name, tp, value, arg, self._parent))
+        setattr(self, name, PropertyParam(name, tp, value, None, self._parent, callback))
+
+    def __getattr__(self, name: str) -> PropertyParam:  # type: ignore  # it should return an PropParam
+        """Trick to avoid mypy issues with dinamyc attributes."""
+        ...
+
+
+class OutputParams(Params):
+    """Class to manage output parameters."""
+
+    def declare(self, name: str, tp: Any = Any, arg: None | str = None, callback: Callable | None = None) -> None:
+        """Add or modify a param.
+
+        Args:
+            name: name of the parameter.
+            tp: type (e.g. str, int, list, str | int,...). Default: typing.Any
+            arg (optional): Component argument directly related with the value of the parameter. Default: None.
+                E.g. this is useful to propagate datatypes and values from a pin with a default value to an argument
+                in a Component (GUI).
+            callback (optional): async callback function to be called when the parameter value changes.
+                Prototype: `async def callback(parent: Component, value: TYPE) -> TYPE:`
+                    - MUST return the value to be finally used.
+                Default: None.
+
+        """
+        setattr(self, name, OutputParam(name, tp, NoValue(), arg, self._parent, callback))
 
     def __getattr__(self, name: str) -> OutputParam:  # type: ignore  # it should return an OutputParam
         """Trick to avoid mypy issues with dinamyc attributes."""
         ...
```

### Comparing `limbus-0.1.5/limbus/core/states.py` & `limbus-0.1.6/limbus/core/states.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Define the states for components/pipelines."""
+from __future__ import annotations
 from enum import Enum
 
 
 class ComponentStoppedError(Exception):
     """Raised when trying to interact with a stopped component.
 
     Properties:
         state: state of the component when the error was raised.
         message: explanation of the error.
 
     """
-    def __init__(self, state: "ComponentState"):
+    def __init__(self, state: "ComponentState", message: None | str = None):
         self.state: ComponentState = state
+        self.message: None | str = message
         super().__init__()
 
 
 class VerboseMode(Enum):
     """Possible states for the verbose in the pipeline objects."""
     DISABLED = 0
     PIPELINE = 1
@@ -32,20 +34,27 @@
     FORCED_STOP = 5  # when the stop is because the user requires it
     INITIALIZED = 6  # whe it is created
     RUNNING = 7
     RECEIVING_PARAMS = 8
     SENDING_PARAMS = 9
     STOPPED_AT_ITER = 10  # when the stop is because of the iteration number
     READY = 11  # when the component is ready to be executed at the beginning of each iteration
+    STOPPED_BY_COMPONENT = 12  # when the stop is because another component forces it
 
 
 class PipelineState(Enum):
     """Possible states for the pipeline."""
     STARTED = 0
     ENDED = 1
     PAUSED = 2
     ERROR = 3
     EMPTY = 4
     RUNNING = 5
     INITIALIZING = 6
     FORCED_STOP = 7
-    CREATED = 8
+
+
+class IterationState(Enum):
+    """Internal state to control the pipeline iterations."""
+    COMPONENT_EXECUTED = 0
+    COMPONENT_NOT_EXECUTED = 1
+    COMPONENT_IN_EXECUTION = 2
```

### Comparing `limbus-0.1.5/limbus/widgets/types.py` & `limbus-0.1.6/limbus/widgets/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module containing the visualization interfaces."""
+from __future__ import annotations
 from abc import abstractmethod
 import math
-from typing import Optional, Union, List, Callable, Set, Tuple, Dict, Any
+from typing import Callable, Any
 import logging
 import functools
 
 try:
     # NOTE: we import these modules here to avoid having it as a dependency
     # for the whole project.
     import cv2
@@ -41,20 +42,20 @@
         return args[1]
     elif "title" in kwargs:
         return kwargs["title"]
     else:
         raise ValueError("No title found in args or kwargs.")
 
 
-def _set_title_in_args(title: str, args: Tuple[Any, ...], kwargs: Dict[Any, Any]
-                       ) -> Tuple[Tuple[Any, ...], Dict[Any, Any]]:
+def _set_title_in_args(title: str, args: tuple[Any, ...], kwargs: dict[Any, Any]
+                       ) -> tuple[tuple[Any, ...], dict[Any, Any]]:
     # NOTE: this is a hack to update the title from the args. We know that the second argument is the title in all the
     # methods.
     if len(args) > 1:
-        new_args: List[Any] = list(args)
+        new_args: list[Any] = list(args)
         new_args[1] = title
         return (tuple(new_args), kwargs)
     elif "title" in kwargs:
         kwargs.update({"title": title})
     return (args, kwargs)
 
 
@@ -130,16 +131,16 @@
             image: Tensor with shape ([1, 3] x H x W) or (H x W). Values can be float in [0, 1] or uint8 in [0, 255].
 
         """
         raise NotImplementedError
 
     @abstractmethod
     def show_images(self, component: Component, title: str,
-                    images: Union["torch.Tensor", List["torch.Tensor"]],
-                    nrow: Optional[int] = None
+                    images: "torch.Tensor" | list["torch.Tensor"],
+                    nrow: None | int = None
                     ) -> None:
         """Show a batch of images.
 
         Args:
             component: component that calls this method.
             title: Title of the window.
             images: 4D Tensor with shape (B x [1, 3] x H x W) or a list of tensors with the same shape
@@ -170,15 +171,15 @@
     def __init__(self) -> None:
         super().__init__()
         try:
             import visdom
         except:
             raise ImportError("To use Visdom as backend install the widgets extras: "
                               "pip install limbus[widgets]")
-        self._vis: Optional[visdom.Visdom] = None
+        self._vis: None | visdom.Visdom = None
         self._try_init()
 
     def _try_init(self) -> None:
         try:
             self._vis = visdom.Visdom(port=Visdom.VISDOM_PORT, raise_exceptions=True)
             self._enabled = True
         except:
@@ -215,16 +216,16 @@
         opts = {"title": title}
         assert self._vis is not None, "Visdom is not initialized."
         self._vis.image(image, win=title, opts=opts)
 
     @is_enabled
     @set_title
     def show_images(self, component: Component, title: str,
-                    images: Union["torch.Tensor", List["torch.Tensor"]],
-                    nrow: Optional[int] = None
+                    images: "torch.Tensor" | list["torch.Tensor"],
+                    nrow: None | int = None
                     ) -> None:
         """Show a batch of images.
 
         Args:
             component: component that calls this method.
             title: Title of the window.
             images: 4D Tensor with shape (B x [1, 3] x H x W) or a list of tensors with the same shape
@@ -279,16 +280,16 @@
 
         """
         log.warning("Console visualization does not show images.")
 
     @is_enabled
     @set_title
     def show_images(self, component: Component, title: str,
-                    images: Union["torch.Tensor", List["torch.Tensor"]],
-                    nrow: Optional[int] = None
+                    images: "torch.Tensor" | list["torch.Tensor"],
+                    nrow: None | int = None
                     ) -> None:
         """Show a batch of images.
 
         Args:
             component: component that calls this method.
             title: Title of the window.
             images: 4D Tensor with shape (B x [1, 3] x H x W) or a list of tensors with the same shape
@@ -353,16 +354,16 @@
         np_img: np.ndarray = kornia.tensor_to_image(image)
         cv2.imshow(title, cv2.cvtColor(np_img, cv2.COLOR_RGB2BGR))
         cv2.waitKey(1)
 
     @is_enabled
     @set_title
     def show_images(self, component: Component, title: str,
-                    images: Union["torch.Tensor", List["torch.Tensor"]],
-                    nrow: Optional[int] = None
+                    images: "torch.Tensor" | list["torch.Tensor"],
+                    nrow: None | int = None
                     ) -> None:
         """Show a batch of images.
 
         Args:
             component: component that calls this method.
             title: Title of the window.
             images: 4D Tensor with shape (B x [1, 3] x H x W) or a list of tensors with the same shape
```

### Comparing `limbus-0.1.5/limbus/widgets/viz.py` & `limbus-0.1.6/limbus/widgets/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Module to manage the visualization tools in limbus."""
-from typing import Optional, Type, Union
+from __future__ import annotations
+from typing import Type
 import inspect
 
 from limbus.widgets import types
 
 
 # global var to store the visualization backend. We want a single instance.
-_viz: Optional[types.Viz] = None
+_viz: None | types.Viz = None
 # global var to store the type used for the visualization backend.
 _viz_cls: Type[types.Viz] = types.Console  # Default value is Console.
 
 
-def set_type(viz_cls: Union[Type[types.Viz], str]) -> None:
+def set_type(viz_cls: Type[types.Viz] | str) -> None:
     """Set the visualization class that will be used to create the visualization object.
 
     Args:
         viz_cls: The visualization class that will be used to create the visualization object.
             It can be a string with the name of the class (defined in limbus/viz/types.py) or the class itself.
 
     """
```

### Comparing `limbus-0.1.5/limbus/widgets/widget_component.py` & `limbus-0.1.6/limbus/widgets/widget_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module containing the base component for visualization components."""
 import functools
 from abc import abstractmethod
 from typing import Callable
 from enum import Enum
 
 from limbus import widgets
-from limbus.core import Component, ComponentState, Params
+from limbus.core import Component, ComponentState, PropertyParams
 
 
 class WidgetState(Enum):
     """Possible states for the viz."""
     DISABLED = 0  # viz is disabled but can be enabled.
     ENABLED = 1  # viz is enabled.
     NO = 2  # viz cannot be used.
@@ -61,32 +61,32 @@
         name (str): component name.
 
     """
     # by default Widget Components have the viz enabled, to disable it use the widget_state property.
     WIDGET_STATE: WidgetState = WidgetState.ENABLED
 
     @staticmethod
-    def register_properties(properties: Params) -> None:
+    def register_properties(properties: PropertyParams) -> None:
         """Register the properties.
 
         Args:
-             properties: Params object to register the properties.
+             properties: object to register the properties.
 
         """
         # this line is like super() but for static methods.
         Component.register_properties(properties)
         properties.declare("title", str, "")
 
     @abstractmethod
     async def _show(self, title: str) -> None:
         """Show the data.
 
         Args:
-            title: same as self._properties.get_param("title").
+            title: same as self._properties[]"title"].value.
 
         """
         raise NotImplementedError
 
     @is_disabled
     async def forward(self) -> ComponentState:  # noqa: D102
-        await self._show(self._properties.get_param("title"))
+        await self._show(self._properties["title"].value)
         return ComponentState.OK
```

### Comparing `limbus-0.1.5/limbus.egg-info/PKG-INFO` & `limbus-0.1.6/limbus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limbus
-Version: 0.1.5
+Version: 0.1.6
 Summary: High level interface to create Pytorch Graphs.
 Home-page: https://github.com/kornia/limbus
 Author: Luis Ferraz
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: components
 Provides-Extra: widgets
```

### Comparing `limbus-0.1.5/limbus.egg-info/SOURCES.txt` & `limbus-0.1.6/limbus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limbus-0.1.5/setup.cfg` & `limbus-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `limbus-0.1.5/setup.py` & `limbus-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='limbus',
-      version='0.1.5',
+      version='0.1.6',
       description='High level interface to create Pytorch Graphs.',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       author='Luis Ferraz',
       url='https://github.com/kornia/limbus',
       install_requires=[
           'typeguard<3.0.0',
```

