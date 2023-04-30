# Comparing `tmp/pymultiastar-0.0.4.tar.gz` & `tmp/pymultiastar-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultiastar-0.0.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pymultiastar-0.0.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pymultiastar-0.0.4.tar` & `pymultiastar-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,49 @@
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/.github/dependabot.yml
--rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/.github/workflows/pip.yml
--rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/.gitignore
--rw-r--r--   0        0        0     1417 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/LICENSE
--rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/README.md
--rw-r--r--   0        0        0     7688 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/docs/Makefile
--rw-r--r--   0        0        0     9488 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/docs/conf.py
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/docs/index.rst
--rw-r--r--   0        0        0     7265 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/docs/make.bat
--rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/docs/python_example.rst
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/examples/__init__.py
--rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/examples/log.py
--rw-r--r--   0        0        0     1806 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/examples/run_maze_2d.py
--rw-r--r--   0        0        0     2523 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/examples/run_scenarios.py
--rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/examples/run_simple_demo.py
--rw-r--r--   0        0        0     1252 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/examples/run_simple_world_3d.py
--rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/noxfile.py
--rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/scripts/upload.sh
--rw-r--r--   0        0        0     8764 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/include/pymultiastar.hpp
--rw-r--r--   0        0        0     1426 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/main.cpp
--rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/__init__.py
--rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/_core.pyi
--rw-r--r--   0        0        0      395 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/geoplanner/__init__.py
--rw-r--r--   0        0        0     8261 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/geoplanner/geoplanner.py
--rw-r--r--   0        0        0     4253 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/geoplanner/helper.py
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/geoplanner/log.py
--rw-r--r--   0        0        0     2416 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/geoplanner/types.py
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/types.py
--rw-r--r--   0        0        0     1689 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/visualization/img2d_helpers.py
--rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/visualization/log.py
--rw-r--r--   0        0        0     5375 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar/visualization/vis3d_helpers.py
--rw-r--r--   0        0        0    18133 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/src/pymultiastar.cpp
--rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/tests/fixtures/.gitignore
--rw-r--r--   0        0        0  1869483 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/tests/fixtures/maze_large.png
--rw-r--r--   0        0        0    38313 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/tests/fixtures/maze_small.png
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/tests/fixtures/world/.gitignore
--rw-r--r--   0        0        0     2582 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/tests/fixtures/world/annarbor/plan.json
--rw-r--r--   0        0        0 38263232 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/tests/fixtures/world/annarbor/voxel_map.npy
--rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/tests/test_basic.py
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/tests/test_geo_helper.py
--rw-r--r--   0        0        0     1247 2022-11-09 12:37:21.000000 pymultiastar-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1417 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/CMakeLists.txt
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3429 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/README.md
+-rw-r--r--   0        0        0    99021 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/assets/imgs/tradeoff.png
+-rw-r--r--   0        0        0     7688 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0     9488 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/conf.py
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/index.rst
+-rw-r--r--   0        0        0     7265 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/docs/python_example.rst
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/__init__.py
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/log.py
+-rw-r--r--   0        0        0     1806 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/run_maze_2d.py
+-rw-r--r--   0        0        0     3313 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/run_scenarios.py
+-rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/run_simple_demo.py
+-rw-r--r--   0        0        0     1252 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/examples/run_simple_world_3d.py
+-rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/noxfile.py
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/output/.gitignore
+-rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/scripts/upload.sh
+-rw-r--r--   0        0        0     8764 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/include/pymultiastar.hpp
+-rw-r--r--   0        0        0     1426 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/main.cpp
+-rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/__init__.py
+-rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/_core.pyi
+-rw-r--r--   0        0        0      395 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/__init__.py
+-rw-r--r--   0        0        0     8307 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/geoplanner.py
+-rw-r--r--   0        0        0     4844 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/helper.py
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/log.py
+-rw-r--r--   0        0        0     2626 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/geoplanner/types.py
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/types.py
+-rw-r--r--   0        0        0     1689 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/visualization/img2d_helpers.py
+-rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/visualization/log.py
+-rw-r--r--   0        0        0     5375 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar/visualization/vis3d_helpers.py
+-rw-r--r--   0        0        0    18133 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/src/pymultiastar.cpp
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/.gitignore
+-rw-r--r--   0        0        0  1869483 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/maze_large.png
+-rw-r--r--   0        0        0    38313 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/maze_small.png
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/.gitignore
+-rw-r--r--   0        0        0     2582 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/annarbor/plan.json
+-rw-r--r--   0        0        0 38263232 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/annarbor/voxel_map.npy
+-rw-r--r--   0        0        0     4540 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/newyork/plan.json
+-rw-r--r--   0        0        0 68625128 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/fixtures/world/newyork/voxel_map.npy
+-rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/test_basic.py
+-rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/tests/test_geo_helper.py
+-rw-r--r--   0        0        0     4488 2022-11-09 12:37:21.000000 pymultiastar-0.0.5/PKG-INFO
```

### Comparing `pymultiastar-0.0.4/.github/workflows/pip.yml` & `pymultiastar-0.0.5/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/.github/workflows/wheels.yml` & `pymultiastar-0.0.5/.github/workflows/wheels.yml`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         os: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
     - uses: actions/checkout@v3
       with:
         submodules: true
 
-    - uses: pypa/cibuildwheel@v2.12.1
+    - uses: pypa/cibuildwheel@v2.12.3
       env:
         CIBW_TEST_REQUIRES: pytest pyproj>=3.0
         CIBW_ARCHS_MACOS: universal2
         CIBW_ARCHS_WINDOWS: auto ARM64
         CIBW_ARCHS_LINUX: auto64
         CIBW_SKIP: "cp27-* cp35-* cp36-* cp37-* cp38-* pp* *musllinux*"
```

### Comparing `pymultiastar-0.0.4/.gitignore` & `pymultiastar-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/.pre-commit-config.yaml` & `pymultiastar-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/docs/Makefile` & `pymultiastar-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/docs/conf.py` & `pymultiastar-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/docs/make.bat` & `pymultiastar-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/examples/run_maze_2d.py` & `pymultiastar-0.0.5/examples/run_maze_2d.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/examples/run_scenarios.py` & `pymultiastar-0.0.5/examples/run_scenarios.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from pathlib import Path
 import typer
+import json
+import uuid
 import logging
 from pymultiastar.visualization.vis3d_helpers import visualize_plan
+from pymultiastar.geoplanner.helper import EnhancedJSONEncoder
 from rich.prompt import Prompt
 
 from pymultiastar.geoplanner import (
     GeoPlanner,
     Scenario,
     GPS,
     LandingSite,
     create_planner_from_configuration,
 )
 from pymultiastar.types import LogLevel
 from log import logger
 
 
 app = typer.Typer()
+THIS_DIR = Path(__file__).parent
 WORLD_DIR = Path(__file__).parent.parent / "tests" / "fixtures" / "world"
 ANNARBOR_PLAN = WORLD_DIR / "annarbor/plan.json"
+OUTPUT_DIR = THIS_DIR.parent / "output"
 
 def plan_scenario(scenario: Scenario, geo_planner: GeoPlanner):
     start_pos = GPS(*scenario["position"])
     if scenario.get("landing_sites") is None:
         raise NotImplementedError(
             "This module relies upon the user providing landing sites"
         )
@@ -55,31 +60,49 @@
 @app.command()
 def run_city_plan(
     plan: Path = ANNARBOR_PLAN,
     log_level: LogLevel = typer.Option(
         LogLevel.INFO.value,
         help="Specify log level",
     ),
+    run_all_scenarios:bool = False,
+    visualize:bool = False,
+    output_dir:Path = OUTPUT_DIR
 ):
     # set log level
     logger.setLevel(getattr(logging, log_level.value))
     logging.getLogger().setLevel(getattr(logging, log_level.value))
 
     # read planner data
     geo_planner, planner_data = create_planner_from_configuration(plan)
     voxel_meta = planner_data["voxel_meta"]
     scenarios = planner_data["scenarios"]
 
-    # choose a scenario in the planner data
-    scenario_str = Prompt.ask(
-        "Choose a scenario",
-        choices=[scenario["name"] for scenario in scenarios],
-        default=scenarios[0]["name"],
-    )
-    scenario = next(item for item in scenarios if item["name"] == scenario_str)
-    # plan the scenario and visualize
-    plan_result = plan_scenario(scenario, geo_planner)
-    visualize_plan(planner_data, plan_result, xres=voxel_meta["xres"])
+    scenario_results = []
+    chosen_scenarios = []
+    if not run_all_scenarios:
+        # choose a scenario in the planner data
+        scenario_str = Prompt.ask(
+            "Choose a scenario",
+            choices=[scenario["name"] for scenario in scenarios],
+            default=scenarios[0]["name"],
+        )
+        scenario = next(item for item in scenarios if item["name"] == scenario_str)
+        chosen_scenarios.append(scenario)
+
+    for scenario in chosen_scenarios:
+        scenario_result = plan_scenario(scenario, geo_planner)
+        scenario_results.append(scenario_result['plan_results'])
+        if visualize:
+            visualize_plan(planner_data, scenario_result, xres=voxel_meta["xres"])
+
+    file_name = planner_data.get('name', str(uuid.uuid4())) + ".json"
+    output_fp = output_dir / file_name
+    logger.info("Writing file to %s", output_fp)
+    with open(output_fp, 'w') as fh:
+        json.dump(scenario_results, fh, cls=EnhancedJSONEncoder, indent=2)
+
+
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pymultiastar-0.0.4/examples/run_simple_demo.py` & `pymultiastar-0.0.5/examples/run_simple_demo.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/examples/run_simple_world_3d.py` & `pymultiastar-0.0.5/examples/run_simple_world_3d.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/pyproject.toml` & `pymultiastar-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymultiastar"
-version = "0.0.4"
+version = "0.0.5"
 description="Multi-goal A* with cpp bindings to python"
 readme = "README.md"
 authors = [
   { name = "Jeremy Castagno", email = "jeremybyu@gmail.com" },
 ]
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pymultiastar-0.0.4/src/include/pymultiastar.hpp` & `pymultiastar-0.0.5/src/include/pymultiastar.hpp`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/src/main.cpp` & `pymultiastar-0.0.5/src/main.cpp`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/src/pymultiastar/_core.pyi` & `pymultiastar-0.0.5/src/pymultiastar/_core.pyi`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/src/pymultiastar/geoplanner/geoplanner.py` & `pymultiastar-0.0.5/src/pymultiastar/geoplanner/geoplanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
             for coord in path_projected
         ]
 
 
         path_length = get_path_dist(path_projected)
         # {'path_cost': dummy_path_risk(start_pos, goal_pos), 'path': path, 'index': index}
         result:GeoMultiPlannerResult = {
+            "start_position": start_position,
             "path_cells": path_cells,
             "path_projected": path_projected,
             "path_projected_zero_origin": path_projected_zero_origin,
             "path_length": path_length,
             "time_ms": elapsed_time,
             "valid_landing_site_indices": valid_landing_site_indices,
             **meta,
```

### Comparing `pymultiastar-0.0.4/src/pymultiastar/geoplanner/helper.py` & `pymultiastar-0.0.5/src/pymultiastar/geoplanner/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Tuple
-
+import dataclasses
+import json
 import numpy as np
 from pyproj import Transformer
 
 from ..types import Cell
 from .types import GPS, ArrayFloatMxNxK, Coord, CoordPath, LandingSite, VoxelMeta
 from .log import logger
 
@@ -78,19 +79,23 @@
     z_meters:float = float(coord[2] * voxel_meta['zres'])
 
     return (x_meters, y_meters, z_meters)
 
 
 def get_free_neighbor_cell(cell:Cell, cost_map:ArrayFloatMxNxK):
     neighbors = [
-        (cell[0], cell[1], cell[2] + 1),
-        (cell[0] + 1, cell[1], cell[2]),
-        (cell[0] - 1, cell[1], cell[2]),
-        (cell[0], cell[1] + 1, cell[2]),
-        (cell[0], cell[1] - 1, cell[2]),
+        (cell[0], cell[1], cell[2] + 1), # z-up
+        (cell[0] + 1, cell[1], cell[2]), # y-up
+        (cell[0] - 1, cell[1], cell[2]), # y-down
+        (cell[0], cell[1] + 1, cell[2]), # x-right
+        (cell[0], cell[1] - 1, cell[2]), # x-left
+        (cell[0] + 1, cell[1], cell[2] + 1), # y-up, z-up
+        (cell[0] - 1, cell[1], cell[2] + 1), # y-down, z-up
+        (cell[0], cell[1] + 1, cell[2] + 1), # x-right, z-up
+        (cell[0], cell[1] - 1, cell[2] + 1), # x-left, z-up
     ]
     for n in neighbors:
         try:
             if cost_map[n[0], n[1], n[2]] != np.inf:
                 return n
         except Exception as e:
             continue
@@ -109,8 +114,17 @@
         a = np.array(path[i], dtype=np.float32)
         b = np.array(path[i + 1], dtype=np.float32)
         dist += float(np.linalg.norm(a - b))
     return dist
 
 
 
+class EnhancedJSONEncoder(json.JSONEncoder):
+        def default(self, o):
+            if dataclasses.is_dataclass(o):
+                return dataclasses.asdict(o)
+            if isinstance(o, np.ndarray):
+                return o.tolist()
+            return super().default(o)
+
+
```

### Comparing `pymultiastar-0.0.4/src/pymultiastar/geoplanner/types.py` & `pymultiastar-0.0.5/src/pymultiastar/geoplanner/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     goal_weight:float = 0.5
     path_weight: float = 0.5
     keep_nodes: bool = False
     path_w0: float = 1.0
 
 class Scenario(TypedDict):
     name:str
-    position: Coord # assumed to be in GPS!
-    active: bool
     details:Optional[str]
+    position: Coord # assumed to be in GPS!
+    active: Optional[bool]
     landing_sites: Optional[List[Dict]]
     planner_kwargs: Optional[Dict]
 
 class VoxelMeta(TypedDict):
     srid:str
     nrows:int
     ncols:int
@@ -42,14 +42,21 @@
     xres:float
     yres:float
     zres:float
     xmin:float
     ymin:float
     zmin:float
 
+class Plan(TypedDict):
+    name:str
+    cost_map_fp: str
+    voxel_meta: VoxelMeta
+    map_bbox: Optional[Dict]
+    planner_kwargs: PlannerKwargs
+    scenarios: List[Scenario]
 @dataclass
 class GPS():
     lat: float
     lon: float
     alt: float = np.nan
 
     def to_array(self, always_xy=False) -> List:
@@ -73,14 +80,15 @@
     centroid: GPS
     "The centroid of the landing site in GPS coordinates"
     landing_site_risk: float
     "The normalized risk of this landing site [0-1]"
 
 
 class GeoMultiPlannerResult(TypedDict):
+    start_position: GPS
     path_cells: CellPath
     path_projected: CoordPath
     path_projected_zero_origin: CoordPath
     path_length: float
     time_ms: float
     valid_landing_site_indices: List[int]
     goal_index: int
```

### Comparing `pymultiastar-0.0.4/src/pymultiastar/types.py` & `pymultiastar-0.0.5/src/pymultiastar/types.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/src/pymultiastar/visualization/img2d_helpers.py` & `pymultiastar-0.0.5/src/pymultiastar/visualization/img2d_helpers.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/src/pymultiastar/visualization/vis3d_helpers.py` & `pymultiastar-0.0.5/src/pymultiastar/visualization/vis3d_helpers.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/src/pymultiastar.cpp` & `pymultiastar-0.0.5/src/pymultiastar.cpp`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/tests/fixtures/maze_large.png` & `pymultiastar-0.0.5/tests/fixtures/maze_large.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/tests/fixtures/maze_small.png` & `pymultiastar-0.0.5/tests/fixtures/maze_small.png`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/tests/fixtures/world/annarbor/plan.json` & `pymultiastar-0.0.5/tests/fixtures/world/annarbor/plan.json`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/tests/fixtures/world/annarbor/voxel_map.npy` & `pymultiastar-0.0.5/tests/fixtures/world/annarbor/voxel_map.npy`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/tests/test_basic.py` & `pymultiastar-0.0.5/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pymultiastar-0.0.4/tests/test_geo_helper.py` & `pymultiastar-0.0.5/tests/test_geo_helper.py`

 * *Files identical despite different names*

