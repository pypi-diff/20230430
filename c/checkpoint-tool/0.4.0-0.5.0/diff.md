# Comparing `tmp/checkpoint_tool-0.4.0.tar.gz` & `tmp/checkpoint_tool-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.4.0.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.5.0.tar", max compression
```

## Comparing `checkpoint_tool-0.4.0.tar` & `checkpoint_tool-0.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3984 2023-04-29 05:40:29.471642 checkpoint_tool-0.4.0/README.md
--rw-r--r--   0        0        0    18099 2023-04-29 05:40:29.472370 checkpoint_tool-0.4.0/checkpoint.py
--rw-r--r--   0        0        0      662 2023-04-29 05:40:51.270381 checkpoint_tool-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 checkpoint_tool-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4391 2023-04-29 13:31:23.891521 checkpoint_tool-0.5.0/README.md
+-rw-r--r--   0        0        0    21944 2023-04-30 12:26:06.634930 checkpoint_tool-0.5.0/checkpoint.py
+-rw-r--r--   0        0        0      679 2023-04-30 12:28:21.280430 checkpoint_tool-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 checkpoint_tool-0.5.0/PKG-INFO
```

### Comparing `checkpoint_tool-0.4.0/README.md` & `checkpoint_tool-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 @task
 def choose(n: int, k: int):
     if 0 < k < n:
         # Mark dependencies on other tasks;
         # The return values of these tasks are passed as the arguments.
         @requires(choose(n - 1, k - 1))
         @requires(choose(n - 1, k)) 
-        def run_task(prev1: int, prev2: int) -> int:
+        def __(prev1: int, prev2: int) -> int:
             # Main computation
             return prev1 + prev2
     elif k == 0 or k == n:
         # Dependency can change according to the task parameters (`n` and `k`).
         # Here, we need no dependency to compute `choose(n, 1)` or `choose(n, n)`.
-        def run_task() -> int:
+        def __() -> int:
             return 1
     else:
         raise ValueError(f'{(n, k)}')
 
     # Return function that produces a value instead of the value itself.
-    return run_task
+    return __
 
 # Build the task graph to compute `choose(6, 3)`
 # and greedily consume it with `concurrent.futures.ProcessPoolExecutor`
 # (i.e., as parallel as possible).
 # The cache is stored at `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/...`
 # and reused whenever available.
 ans = choose(6, 3).run()
@@ -77,30 +77,30 @@
 def task2(**param2):
     ...
 
 @task
 def task3(json_params):
     @requires(task1(**json_params['param1']))
     @requires(task2(**json_params['param2']))
-    def run_task(result1, result2):
+    def __(result1, result2):
         ...
-    return run_task
+    return __
 
 result = task3({'param1': { ... }, 'param2': { ... }}).run()
 ```
 
 Task dependencies can be specified with lists and dicts:
 ```python
 @task
 def task3(json_params):
     @requires([task1(p) for p in json_params['my_param_list']])
     @requires({k: task2(p) for k, p in json_params['my_param_dict'].items()})
-    def run_task(result_list, result_dict):
+    def __(result_list, result_dict):
         ...
-    return run_task
+    return __
 
 result = task3({'my_param_list': [ ... ], 'my_param_dict': { ... }}).run()
 ```
 
 Large outputs can be stored with compression via `zlib`:
 ```python
 @task(compress_level=-1)
@@ -109,27 +109,29 @@
 ```
 
 ### Data directories
 
 Use `@requires_directory` decorator to create a fresh directory dedicated to each task. The contents of the directory are cleared at each task call and persist until `clear`ed.
 ```python
 from pathlib import Path
+from checkpoint import requires_directory
 
 @task
 def train_model(...):
 
-    # Passing a new directory at `$CHECKPOINT_PATH/checkpoint/{module_name}.{function_name}/data/{cryptic_task_id}`
+    # Passing a new directory at
+    # `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/data/{cryptic_task_id}`
     @requires_directory
-    def run_task(path: Path):
+    def __(path: Path) -> str:
         ...
         model_path = str(path / 'model.bin')
         model.save(model_path)
         return model_path
 
-    return run_task
+    return __
 ```
 
 ### Execution policy configuration
 
 One can control the task execution with `concurrent.futures.Executor` class:
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
@@ -147,7 +149,19 @@
 
 One can also control the concurrency at a task level:
 ```python
 @task(max_concurrency=2)
 def resource_intensive_task(*args, **kwargs):
     ...
 ```
+
+### Commandline tool
+We can use checkpoint-tool from commandline like `python -m checkpoint path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
+```python
+# taskfile.py
+
+@task
+def main():
+    ...
+```
+The command runs the `main` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
+Please refer to `python -m checkpoint --help` for more info.
```

### Comparing `checkpoint_tool-0.4.0/checkpoint.py` & `checkpoint_tool-0.5.0/checkpoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,62 @@
 """ A lightweight workflow management tool written in pure Python.
 
 TODO:
-    - Special directives
-        - @entrypoint: set the root directory of cache next to the file containing the decorated task.
-            Usage: `python -m checkpoint main.py`
-            -> Run the entrypoint task contained in main.py with cache located at ./.cache/main/{module_name}.{function_name}/...
+    - Task change detection
+        - via variable-anonymized AST
     - Priority-based scheduling
 """
 from __future__ import annotations
-from typing import Callable, ClassVar, Generic, NewType, Protocol, TypeVar, Any, cast, overload
+from typing import Callable, ClassVar, Generic, NewType, TypeVar, Any, cast, overload
 from typing_extensions import ParamSpec, Concatenate, Self
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from concurrent.futures import ProcessPoolExecutor, Future, wait, FIRST_COMPLETED, Executor
+from concurrent.futures import ProcessPoolExecutor, Future, ThreadPoolExecutor, wait, FIRST_COMPLETED, Executor
 from functools import wraps
+import importlib.util
+import ast
 import os
+import sys
 import logging
 import inspect
 import json
 import base64
 import shutil
 
+import click
 import cloudpickle
 import zlib
 import diskcache as dc
 import networkx as nx
 
 
-CHECKPOINT_PATH = Path(os.getenv('CP_CACHE_DIR', './.cache')) / 'checkpoint'
-CHECKPOINT_PATH.mkdir(parents=True, exist_ok=True)
+class Context:
+    cache_dir = Path(os.getenv('CP_CACHE_DIR', './.cache'))
+    executor_name = os.getenv('CP_EXECUTOR', 'process')
+    max_workers = int(os.getenv('CP_MAX_WORKERS', -1))
+    detect_source_change = bool(os.getenv('CP_DETECT_SOURCE_CHANGE', 0))
+    num_cpu = os.cpu_count()
+
+    @classmethod
+    def get_executor(cls, max_workers: int | None = None) -> Executor:
+        if cls.executor_name == 'process':
+            executor_type = ProcessPoolExecutor
+        elif cls.executor_name == 'thread':
+            executor_type = ThreadPoolExecutor
+        else:
+            raise ValueError('Unrecognized executor name:', cls.executor_name)
+        if max_workers is None:
+            max_workers = cls.max_workers
+        if max_workers < 0:
+            assert isinstance(cls.num_cpu, int)
+            assert -cls.num_cpu <= cls.max_workers
+            max_workers = cls.num_cpu + 1 + cls.max_workers
+        return executor_type(max_workers=max_workers)
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 Json = NewType('Json', str)
 
@@ -50,43 +72,62 @@
 DEFAULT_SERIALIZER: Serializer = (cloudpickle.dumps, cloudpickle.loads)
 
 
 @dataclass(frozen=True)
 class Database(Generic[T, D]):
     """ Manage the cache of tasks.
     Layout:
-    CHECKPOINT_PATH / name / result     # return values
-    CHECKPOINT_PATH / name / timestamp  # timestamps
-    CHECKPOINT_PATH / name / data       # other data created by tasks
+    Context.cache_dir / 'checkpoint' / name / result     # return values
+    Context.cache_dir / 'checkpoint' / name / timestamp  # timestamps
+    Context.cache_dir / 'checkpoint' / name / data       # other data created by tasks
     """
     name: str
-    base_path: str
+    base_path: Path
     compress_level: int
     result_cache: dc.Cache
     timestamp_cache: dc.Cache
     serializer: Serializer = DEFAULT_SERIALIZER
 
     @classmethod
     def make(cls, name: str, compress_level: int) -> Self:
-        base_path = str(CHECKPOINT_PATH / name)
+        base_path = Context.cache_dir / 'checkpoint' / name
         return Database(
                 name=name,
                 base_path=base_path,
                 compress_level=compress_level,
-                result_cache=dc.Cache(base_path + '/result'),
-                timestamp_cache=dc.Cache(base_path + '/timestamp'),
+                result_cache=dc.Cache(base_path / 'result'),
+                timestamp_cache=dc.Cache(base_path / 'timestamp'),
                 )
 
     def __post_init__(self) -> None:
         self.data_directory.mkdir(exist_ok=True)
+        self.source_path.parent.mkdir(exist_ok=True)
 
     @property
     def data_directory(self) -> Path:
         return Path(self.base_path) / 'data'
 
+    @property
+    def source_path(self) -> Path:
+        return Path(self.base_path) / 'code' / 'source.txt'
+
+    def update_source_if_necessary(self, source: str) -> datetime:
+        # Update source cache
+        if self.source_path.exists():
+            cached_source = open(self.source_path, 'r').read()
+        else:
+            cached_source = None
+        if cached_source != source:
+            open(self.source_path, 'w').write(source)
+        return self.load_source_timestamp()
+
+    def load_source_timestamp(self) -> datetime:
+        timestamp = self.source_path.stat().st_mtime_ns / 10 ** 9
+        return datetime.fromtimestamp(timestamp)
+
     def _dumps(self, obj: Any) -> bytes:
         dumps, _ = self.serializer
         return zlib.compress(dumps(obj), level=self.compress_level)
 
     def _loads(self, data: bytes) -> Any:
         _, loads = self.serializer
         return loads(zlib.decompress(data))
@@ -198,30 +239,38 @@
     runner: Runner[R]
 
     def set_result(self) -> None:
         db = self.task_factory.db
         out = self.runner()
         db.save(self.key, out)
 
-    def run(self, *, executor: Executor | None = None) -> R:
-        return self.run_with_info(executor=executor)[0]
+    def run(self, *, executor: Executor | None = None, max_workers: int | None = None) -> R:
+        return self.run_with_info(executor=executor, max_workers=max_workers)[0]
 
-    def run_with_info(self, *, executor: Executor | None = None, dump_generations: bool = False) -> tuple[R, dict[str, Any]]:
+    def run_with_info(
+            self, *,
+            executor: Executor | None = None,
+            max_workers: int | None = None,
+            dump_generations: bool = False
+            ) -> tuple[R, dict[str, Any]]:
         graph = TaskGraph.build_from(self)
         if executor is None:
-            executor = ProcessPoolExecutor()
+            executor = Context.get_executor(max_workers=max_workers)
+        else:
+            assert max_workers is None
         info = run_task_graph(graph=graph, executor=executor, dump_generations=dump_generations)
         return self.get_result(), info
 
 
 @dataclass
 class TaskFactory(Generic[P, R]):
     runner_factory: RunnerFactory[P, R]
     db: Database
     max_concurrency: int | None
+    source_timestamp: datetime
 
     def get_db_name(self) -> str:
         return self.db.name
 
     def clear(self) -> None:
         self.db.clear()
 
@@ -247,17 +296,23 @@
         *, compress_level: int = 0, max_concurrency: int | None = None
         ) -> Callable[[RunnerFactory[P, R]], TaskFactory[P, R]]:
     """ Convert a runner factory into a task factory. """
 
     def decorator(fn: RunnerFactory[P, R]) -> TaskFactory[P, R]:
         name = _serialize_function(fn)
         db = Database.make(name=name, compress_level=compress_level)
+
+        source = inspect.getsource(fn)
+        formatted_source = ast.unparse(ast.parse(source))
+        source_timestamp = db.update_source_if_necessary(formatted_source)
+
         return wraps(fn)(TaskFactory(
             runner_factory=fn, db=db,
-            max_concurrency=max_concurrency
+            max_concurrency=max_concurrency,
+            source_timestamp=source_timestamp
             ))
     return decorator
 
 
 def _serialize_function(fn: Callable[..., Any]) -> str:
     return f'{fn.__module__}.{fn.__qualname__}'
 
@@ -362,15 +417,15 @@
 class RequiresDirectory(Generic[P, R]):
     fn: Callable[Concatenate[Path, P], R]
     directory: Path | None = None
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
         assert self.directory is not None, 'Directory not set. Bug?'
         if self.directory.exists():
-            self.directory.rmdir()
+            shutil.rmtree(self.directory)
         self.directory.mkdir()
         return self.fn(self.directory, *args, **kwargs)
 
     def set_directory(self, path: Path) -> None:
         self.directory = path
 
 
@@ -403,51 +458,51 @@
         while to_expand:
             task = to_expand.pop()
             x = task.to_tuple()
             if x not in seen:
                 seen.add(x)
                 prerequisite_tasks = get_prerequisite_tasks(task)
                 to_expand.extend(prerequisite_tasks)
-                G.add_node(x, task=task, timestamp=task.peek_timestamp())
+                G.add_node(x, task=task, timestamp=task.peek_timestamp(), source_timestamp=task.task_factory.source_timestamp)
                 G.add_edges_from([(p.to_tuple(), x) for p in prerequisite_tasks])
         out = TaskGraph(G)
         out.trim()
         return out
 
     @property
     def size(self) -> int:
         return len(self.G)
 
     def get_task(self, key: TaskKey) -> AnyTask:
         return self.G.nodes[key]['task']
 
     def trim(self) -> None:
-        self._mark_fresh_nodes()
+        self._mark_nodes_to_update()
         self._remove_fresh_nodes()
         self._transitive_reduction()
 
-    def _mark_fresh_nodes(self) -> None:
+    def _mark_nodes_to_update(self) -> None:
         for x in nx.topological_sort(self.G):
-            ts0 = self.G.nodes[x]['timestamp']
-            if ts0 is None:
-                self.G.add_node(x, fresh=False)
+            ts_task = self.G.nodes[x]['timestamp']
+            ts_source = self.G.nodes[x]['source_timestamp']
+            if ts_task is None or (Context.detect_source_change and ts_task < ts_source):
+                self.G.add_node(x, to_update=True)
                 continue
-            for y in self.G.predecessors(x):
-                fresh_y = self.G.nodes[y]['fresh']
-                ts = self.G.nodes[y]['timestamp']
-                if not fresh_y or ts is None or ts > ts0:
-                    self.G.add_node(x, fresh=False)
+            for p in self.G.predecessors(x):
+                pred_to_update = self.G.nodes[p]['to_update']
+                ts_pred = self.G.nodes[p]['timestamp']
+                if pred_to_update or ts_task < ts_pred:
+                    self.G.add_node(x, to_update=True)
                     break
             else:
-                self.G.add_node(x, fresh=True)
+                self.G.add_node(x, to_update=False)
 
     def _remove_fresh_nodes(self) -> None:
-        to_remove = [x for x, attr in self.G.nodes.items() if attr['fresh']]
-        for x in to_remove:
-            self.G.remove_node(x)
+        to_remove = [x for x, attr in self.G.nodes.items() if not attr['to_update']]
+        self.G.remove_nodes_from(to_remove)
 
     def _transitive_reduction(self) -> None:
         TR = nx.transitive_reduction(self.G)
         TR.add_nodes_from(self.G.nodes(data=True))
         self.G = TR
 
     def get_task_factories(self) -> dict[str, TaskFactory[..., Any]]:
@@ -558,7 +613,45 @@
 
 
 def _run_task(task_data: bytes) -> tuple[str, Json]:
     task = cloudpickle.loads(task_data)
     assert isinstance(task, Task)
     task.set_result()
     return task.to_tuple()
+
+
+@click.command
+@click.argument('taskfile', type=Path)
+@click.option('-e', '--entrypoint', default='main', help='Task name for entrypoint.')
+@click.option('-t', '--exec-type', type=click.Choice(['process', 'thread']), default='process')
+@click.option('-w', '--max-workers', type=int, default=-1)
+@click.option('--cache-dir', type=Path, default=None)
+@click.option('-D', '--detect-source-change', is_flag=True, help='Automatically discard the cache per task once the source code (AST) is changed.')
+def main(taskfile: Path, entrypoint: str, exec_type: str, max_workers: int, cache_dir: Path | None, detect_source_change: bool):
+    # Set arguments as environment variables
+    os.environ['CP_EXECUTOR'] = exec_type
+    os.environ['CP_MAX_WORKERS'] = str(max_workers)
+    os.environ['CP_CACHE_DIR'] = str(taskfile.parent / '.cache') if cache_dir is None else str(cache_dir)
+    os.environ['CP_DETECT_SOURCE_CHANGE'] = str(int(detect_source_change))
+
+    # Run script as module
+    module_name = taskfile.with_suffix('').name
+    spec = importlib.util.spec_from_file_location(module_name, taskfile)
+    assert spec is not None
+    assert spec.loader is not None
+    module = importlib.util.module_from_spec(spec)
+    sys.modules[module_name] = module
+    spec.loader.exec_module(module)
+
+    # Run the main task
+    entrypoint_fn = getattr(module, entrypoint)
+    assert type(entrypoint_fn).__name__ == TaskFactory.__name__, \
+            f'Taskfile `{taskfile}` should contain a task(factory) `{entrypoint}`, but found `{entrypoint_fn}`.'
+    entrypoint_fn = cast(TaskFactory, entrypoint_fn)
+    task = entrypoint_fn()
+    task.run()
+    print(task.directory)
+    return 0
+
+
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `checkpoint_tool-0.4.0/pyproject.toml` & `checkpoint_tool-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.4.0"
+version = "0.5.0"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint.py"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.5.0"
 diskcache = "^5.6.1"
 cloudpickle = "^2.2.1"
 networkx = "^3.1"
+click = "^8.1.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `checkpoint_tool-0.4.0/PKG-INFO` & `checkpoint_tool-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.4.0
+Version: 0.5.0
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/koheimiya/checkpoint
 Description-Content-Type: text/markdown
 
@@ -44,27 +45,27 @@
 @task
 def choose(n: int, k: int):
     if 0 < k < n:
         # Mark dependencies on other tasks;
         # The return values of these tasks are passed as the arguments.
         @requires(choose(n - 1, k - 1))
         @requires(choose(n - 1, k)) 
-        def run_task(prev1: int, prev2: int) -> int:
+        def __(prev1: int, prev2: int) -> int:
             # Main computation
             return prev1 + prev2
     elif k == 0 or k == n:
         # Dependency can change according to the task parameters (`n` and `k`).
         # Here, we need no dependency to compute `choose(n, 1)` or `choose(n, n)`.
-        def run_task() -> int:
+        def __() -> int:
             return 1
     else:
         raise ValueError(f'{(n, k)}')
 
     # Return function that produces a value instead of the value itself.
-    return run_task
+    return __
 
 # Build the task graph to compute `choose(6, 3)`
 # and greedily consume it with `concurrent.futures.ProcessPoolExecutor`
 # (i.e., as parallel as possible).
 # The cache is stored at `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/...`
 # and reused whenever available.
 ans = choose(6, 3).run()
@@ -98,30 +99,30 @@
 def task2(**param2):
     ...
 
 @task
 def task3(json_params):
     @requires(task1(**json_params['param1']))
     @requires(task2(**json_params['param2']))
-    def run_task(result1, result2):
+    def __(result1, result2):
         ...
-    return run_task
+    return __
 
 result = task3({'param1': { ... }, 'param2': { ... }}).run()
 ```
 
 Task dependencies can be specified with lists and dicts:
 ```python
 @task
 def task3(json_params):
     @requires([task1(p) for p in json_params['my_param_list']])
     @requires({k: task2(p) for k, p in json_params['my_param_dict'].items()})
-    def run_task(result_list, result_dict):
+    def __(result_list, result_dict):
         ...
-    return run_task
+    return __
 
 result = task3({'my_param_list': [ ... ], 'my_param_dict': { ... }}).run()
 ```
 
 Large outputs can be stored with compression via `zlib`:
 ```python
 @task(compress_level=-1)
@@ -130,27 +131,29 @@
 ```
 
 ### Data directories
 
 Use `@requires_directory` decorator to create a fresh directory dedicated to each task. The contents of the directory are cleared at each task call and persist until `clear`ed.
 ```python
 from pathlib import Path
+from checkpoint import requires_directory
 
 @task
 def train_model(...):
 
-    # Passing a new directory at `$CHECKPOINT_PATH/checkpoint/{module_name}.{function_name}/data/{cryptic_task_id}`
+    # Passing a new directory at
+    # `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/data/{cryptic_task_id}`
     @requires_directory
-    def run_task(path: Path):
+    def __(path: Path) -> str:
         ...
         model_path = str(path / 'model.bin')
         model.save(model_path)
         return model_path
 
-    return run_task
+    return __
 ```
 
 ### Execution policy configuration
 
 One can control the task execution with `concurrent.futures.Executor` class:
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
@@ -169,7 +172,19 @@
 One can also control the concurrency at a task level:
 ```python
 @task(max_concurrency=2)
 def resource_intensive_task(*args, **kwargs):
     ...
 ```
 
+### Commandline tool
+We can use checkpoint-tool from commandline like `python -m checkpoint path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
+```python
+# taskfile.py
+
+@task
+def main():
+    ...
+```
+The command runs the `main` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
+Please refer to `python -m checkpoint --help` for more info.
+
```

