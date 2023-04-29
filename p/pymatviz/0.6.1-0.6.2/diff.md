# Comparing `tmp/pymatviz-0.6.1.tar.gz` & `tmp/pymatviz-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatviz-0.6.1.tar", last modified: Tue Mar 21 21:42:29 2023, max compression
+gzip compressed data, was "pymatviz-0.6.2.tar", last modified: Sat Apr 29 23:06:37 2023, max compression
```

## Comparing `pymatviz-0.6.1.tar` & `pymatviz-0.6.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-03-21 21:42:29.758097 pymatviz-0.6.1/
--rw-r--r--   0 janosh     (501) wheel        (0)    17362 2023-03-21 21:42:29.757907 pymatviz-0.6.1/PKG-INFO
--rw-r--r--   0 janosh     (501) wheel        (0)     1073 2021-08-04 10:50:41.000000 pymatviz-0.6.1/license
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-03-21 21:42:29.753013 pymatviz-0.6.1/pymatviz/
--rw-r--r--   0 janosh     (501) wheel        (0)     2236 2023-02-20 20:13:42.000000 pymatviz-0.6.1/pymatviz/__init__.py
--rw-r--r--   0 janosh     (501) wheel        (0)     3675 2023-02-18 02:11:20.000000 pymatviz-0.6.1/pymatviz/correlation.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2995 2023-02-20 20:13:42.000000 pymatviz-0.6.1/pymatviz/cumulative.py
--rw-r--r--   0 janosh     (501) wheel        (0)    19361 2022-12-30 20:51:55.000000 pymatviz-0.6.1/pymatviz/elements.csv
--rw-r--r--   0 janosh     (501) wheel        (0)    12350 2023-03-12 00:39:26.000000 pymatviz-0.6.1/pymatviz/histograms.py
--rw-r--r--   0 janosh     (501) wheel        (0)     9790 2023-02-18 02:11:20.000000 pymatviz-0.6.1/pymatviz/parity.py
--rw-r--r--   0 janosh     (501) wheel        (0)     1277 2023-02-20 19:27:21.000000 pymatviz-0.6.1/pymatviz/plot_defaults.py
--rw-r--r--   0 janosh     (501) wheel        (0)    27881 2023-03-21 18:36:14.000000 pymatviz-0.6.1/pymatviz/ptable.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2795 2023-02-18 02:11:20.000000 pymatviz-0.6.1/pymatviz/relevance.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2119 2023-02-18 02:11:20.000000 pymatviz-0.6.1/pymatviz/sankey.py
--rw-r--r--   0 janosh     (501) wheel        (0)    16624 2023-03-21 18:36:59.000000 pymatviz-0.6.1/pymatviz/structure_viz.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2400 2023-02-18 02:11:20.000000 pymatviz-0.6.1/pymatviz/sunburst.py
--rw-r--r--   0 janosh     (501) wheel        (0)     9695 2023-02-18 02:11:20.000000 pymatviz-0.6.1/pymatviz/uncertainty.py
--rw-r--r--   0 janosh     (501) wheel        (0)    14467 2023-03-10 03:53:13.000000 pymatviz-0.6.1/pymatviz/utils.py
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-03-21 21:42:29.754190 pymatviz-0.6.1/pymatviz.egg-info/
--rw-r--r--   0 janosh     (501) wheel        (0)    17362 2023-03-21 21:42:29.000000 pymatviz-0.6.1/pymatviz.egg-info/PKG-INFO
--rw-r--r--   0 janosh     (501) wheel        (0)      779 2023-03-21 21:42:29.000000 pymatviz-0.6.1/pymatviz.egg-info/SOURCES.txt
--rw-r--r--   0 janosh     (501) wheel        (0)        1 2023-03-21 21:42:29.000000 pymatviz-0.6.1/pymatviz.egg-info/dependency_links.txt
--rw-r--r--   0 janosh     (501) wheel        (0)      191 2023-03-21 21:42:29.000000 pymatviz-0.6.1/pymatviz.egg-info/requires.txt
--rw-r--r--   0 janosh     (501) wheel        (0)        9 2023-03-21 21:42:29.000000 pymatviz-0.6.1/pymatviz.egg-info/top_level.txt
--rw-r--r--   0 janosh     (501) wheel        (0)     2758 2023-03-21 21:26:55.000000 pymatviz-0.6.1/pyproject.toml
--rw-r--r--   0 janosh     (501) wheel        (0)    15353 2023-03-12 22:42:32.000000 pymatviz-0.6.1/readme.md
--rw-r--r--   0 janosh     (501) wheel        (0)       38 2023-03-21 21:42:29.758133 pymatviz-0.6.1/setup.cfg
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-03-21 21:42:29.757512 pymatviz-0.6.1/tests/
--rw-r--r--   0 janosh     (501) wheel        (0)      464 2022-10-15 03:29:31.000000 pymatviz-0.6.1/tests/test_correlation.py
--rw-r--r--   0 janosh     (501) wheel        (0)      705 2022-12-24 23:29:33.000000 pymatviz-0.6.1/tests/test_cumulative.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2370 2023-02-20 19:25:40.000000 pymatviz-0.6.1/tests/test_histograms.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2575 2023-02-20 20:13:42.000000 pymatviz-0.6.1/tests/test_parity.py
--rw-r--r--   0 janosh     (501) wheel        (0)     9425 2023-03-20 20:58:57.000000 pymatviz-0.6.1/tests/test_ptable.py
--rw-r--r--   0 janosh     (501) wheel        (0)      496 2023-02-21 20:10:51.000000 pymatviz-0.6.1/tests/test_readme.py
--rw-r--r--   0 janosh     (501) wheel        (0)     1272 2022-10-14 17:22:38.000000 pymatviz-0.6.1/tests/test_relevance.py
--rw-r--r--   0 janosh     (501) wheel        (0)      589 2022-10-08 23:23:21.000000 pymatviz-0.6.1/tests/test_sankey.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2124 2023-03-20 20:58:57.000000 pymatviz-0.6.1/tests/test_structure_viz.py
--rw-r--r--   0 janosh     (501) wheel        (0)      960 2022-10-08 23:23:21.000000 pymatviz-0.6.1/tests/test_sunburst.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2006 2023-02-20 19:27:21.000000 pymatviz-0.6.1/tests/test_uncertainty.py
--rw-r--r--   0 janosh     (501) wheel        (0)     4063 2023-03-12 02:47:41.000000 pymatviz-0.6.1/tests/test_utils.py
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-04-29 23:06:37.016901 pymatviz-0.6.2/
+-rw-r--r--   0 janosh     (501) wheel        (0)    17362 2023-04-29 23:06:37.016698 pymatviz-0.6.2/PKG-INFO
+-rw-r--r--   0 janosh     (501) wheel        (0)     1073 2021-08-04 10:50:41.000000 pymatviz-0.6.2/license
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-04-29 23:06:37.012068 pymatviz-0.6.2/pymatviz/
+-rw-r--r--   0 janosh     (501) wheel        (0)     2238 2023-03-27 18:51:03.000000 pymatviz-0.6.2/pymatviz/__init__.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3675 2023-02-18 02:11:20.000000 pymatviz-0.6.2/pymatviz/correlation.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2995 2023-02-20 20:13:42.000000 pymatviz-0.6.2/pymatviz/cumulative.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    19361 2022-12-30 20:51:55.000000 pymatviz-0.6.2/pymatviz/elements.csv
+-rw-r--r--   0 janosh     (501) wheel        (0)    12350 2023-03-12 00:39:26.000000 pymatviz-0.6.2/pymatviz/histograms.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     9804 2023-03-27 18:51:03.000000 pymatviz-0.6.2/pymatviz/parity.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     1277 2023-02-20 19:27:21.000000 pymatviz-0.6.2/pymatviz/plot_defaults.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    28565 2023-04-16 23:28:04.000000 pymatviz-0.6.2/pymatviz/ptable.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2795 2023-02-18 02:11:20.000000 pymatviz-0.6.2/pymatviz/relevance.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2115 2023-03-27 18:51:03.000000 pymatviz-0.6.2/pymatviz/sankey.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    16624 2023-03-21 18:36:59.000000 pymatviz-0.6.2/pymatviz/structure_viz.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2584 2023-04-16 23:28:04.000000 pymatviz-0.6.2/pymatviz/sunburst.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     9695 2023-02-18 02:11:20.000000 pymatviz-0.6.2/pymatviz/uncertainty.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    17038 2023-04-02 04:05:42.000000 pymatviz-0.6.2/pymatviz/utils.py
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-04-29 23:06:37.013430 pymatviz-0.6.2/pymatviz.egg-info/
+-rw-r--r--   0 janosh     (501) wheel        (0)    17362 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/PKG-INFO
+-rw-r--r--   0 janosh     (501) wheel        (0)      779 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/SOURCES.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)        1 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/dependency_links.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)      191 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/requires.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)        9 2023-04-29 23:06:37.000000 pymatviz-0.6.2/pymatviz.egg-info/top_level.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)     2751 2023-04-29 23:04:24.000000 pymatviz-0.6.2/pyproject.toml
+-rw-r--r--   0 janosh     (501) wheel        (0)    15353 2023-03-12 22:42:32.000000 pymatviz-0.6.2/readme.md
+-rw-r--r--   0 janosh     (501) wheel        (0)       38 2023-04-29 23:06:37.016949 pymatviz-0.6.2/setup.cfg
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2023-04-29 23:06:37.016436 pymatviz-0.6.2/tests/
+-rw-r--r--   0 janosh     (501) wheel        (0)      464 2022-10-15 03:29:31.000000 pymatviz-0.6.2/tests/test_correlation.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      705 2022-12-24 23:29:33.000000 pymatviz-0.6.2/tests/test_cumulative.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2370 2023-02-20 19:25:40.000000 pymatviz-0.6.2/tests/test_histograms.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2575 2023-02-20 20:13:42.000000 pymatviz-0.6.2/tests/test_parity.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    10014 2023-04-16 23:28:04.000000 pymatviz-0.6.2/tests/test_ptable.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      496 2023-02-21 20:10:51.000000 pymatviz-0.6.2/tests/test_readme.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     1272 2022-10-14 17:22:38.000000 pymatviz-0.6.2/tests/test_relevance.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      589 2022-10-08 23:23:21.000000 pymatviz-0.6.2/tests/test_sankey.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2124 2023-03-20 20:58:57.000000 pymatviz-0.6.2/tests/test_structure_viz.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      960 2022-10-08 23:23:21.000000 pymatviz-0.6.2/tests/test_sunburst.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2006 2023-02-20 19:27:21.000000 pymatviz-0.6.2/tests/test_uncertainty.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     6038 2023-04-02 04:05:42.000000 pymatviz-0.6.2/tests/test_utils.py
```

### Comparing `pymatviz-0.6.1/PKG-INFO` & `pymatviz-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatviz
-Version: 0.6.1
+Version: 0.6.2
 Summary: A toolkit for visualizations in materials informatics
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pymatviz-0.6.1/license` & `pymatviz-0.6.2/license`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/__init__.py` & `pymatviz-0.6.2/pymatviz/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 from pymatviz.sankey import sankey_from_2_df_cols as sankey_from_2_df_cols
 from pymatviz.structure_viz import plot_structure_2d as plot_structure_2d
 from pymatviz.sunburst import spacegroup_sunburst as spacegroup_sunburst
 from pymatviz.uncertainty import error_decay_with_uncert as error_decay_with_uncert
 from pymatviz.uncertainty import qq_gaussian as qq_gaussian
 from pymatviz.utils import ROOT as ROOT
 from pymatviz.utils import annotate_bars as annotate_bars
-from pymatviz.utils import annotate_mae_r2 as annotate_mae_r2
+from pymatviz.utils import annotate_metrics as annotate_metrics
```

### Comparing `pymatviz-0.6.1/pymatviz/correlation.py` & `pymatviz-0.6.2/pymatviz/correlation.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/cumulative.py` & `pymatviz-0.6.2/pymatviz/cumulative.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/elements.csv` & `pymatviz-0.6.2/pymatviz/elements.csv`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/histograms.py` & `pymatviz-0.6.2/pymatviz/histograms.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/parity.py` & `pymatviz-0.6.2/pymatviz/parity.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy.interpolate
 from matplotlib.gridspec import GridSpec
 
-from pymatviz.utils import Array, annotate_mae_r2, df_to_arrays, with_hist
+from pymatviz.utils import Array, annotate_metrics, df_to_arrays, with_hist
 
 
 def hist_density(
     x: Array | str,
     y: Array | str,
     df: pd.DataFrame = None,
     sort: bool = True,
@@ -78,15 +78,15 @@
         density_bins (int, optional): How many density_bins to use for the density
             histogram, i.e. granularity of the density color scale. Defaults to 100.
         xlabel (str, optional): x-axis label. Defaults to "Actual".
         ylabel (str, optional): y-axis label. Defaults to "Predicted".
         identity (bool, optional): Whether to add an identity/parity line (y = x).
             Defaults to True.
         stats (bool | dict[str, Any], optional): Whether to display a text box with MAE
-            and R^2. Defaults to True. Can be dict to pass kwargs to `annotate_mae_r2`.
+            and R^2. Defaults to True. Can be dict to pass kwargs to annotate_metrics().
             E.g. stats=dict(loc="upper left", prefix="Title", prop=dict(fontsize=16)).
         **kwargs: Additional keyword arguments to pass to ax.scatter(). E.g. cmap to
             change the color map.
 
     Returns:
         ax: The plot's matplotlib Axes.
     """
@@ -112,15 +112,15 @@
             alpha=0.5,
             zorder=0,
             linestyle="dashed",
             color="black",
         )
 
     if stats:
-        annotate_mae_r2(x, y, ax, **(stats if isinstance(stats, dict) else {}))
+        annotate_metrics(x, y, ax=ax, **(stats if isinstance(stats, dict) else {}))
 
     ax.set(xlabel=xlabel, ylabel=ylabel)
 
     return ax
 
 
 def scatter_with_err_bar(
@@ -159,15 +159,15 @@
 
     styles = dict(markersize=6, fmt="o", ecolor="g", capthick=2, elinewidth=2)
     ax.errorbar(x, y, xerr=xerr, yerr=yerr, **kwargs, **styles)
 
     # identity line
     ax.axline((0, 0), (1, 1), alpha=0.5, zorder=0, linestyle="dashed", color="black")
 
-    annotate_mae_r2(x, y, ax)
+    annotate_metrics(x, y, ax=ax)
 
     ax.set(xlabel=xlabel, ylabel=ylabel, title=title)
 
     return ax
 
 
 def density_hexbin(
@@ -207,15 +207,15 @@
     cb_ax = ax.inset_axes([0.95, 0.03, 0.03, 0.7])  # [x, y, width, height]
     plt.colorbar(hexbin, cax=cb_ax)
     cb_ax.yaxis.set_ticks_position("left")
 
     # identity line
     ax.axline((0, 0), (1, 1), alpha=0.5, zorder=0, linestyle="dashed", color="black")
 
-    annotate_mae_r2(x, y, ax, loc="upper left")
+    annotate_metrics(x, y, ax=ax, loc="upper left")
 
     ax.set(xlabel=xlabel, ylabel=ylabel)
 
     return ax
 
 
 def density_scatter_with_hist(
```

### Comparing `pymatviz-0.6.1/pymatviz/plot_defaults.py` & `pymatviz-0.6.2/pymatviz/plot_defaults.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/ptable.py` & `pymatviz-0.6.2/pymatviz/ptable.py`

 * *Files 6% similar despite different names*

```diff
@@ -452,15 +452,16 @@
             swapped depending on the colorscale.
         gap (float): Gap in pixels between tiles of the periodic table. Defaults to 5.
         font_size (int): Element symbol and heat label text size. Any valid CSS size
             allowed. Defaults to automatic font size based on plot size. Element symbols
             will be bold and 1.5x this size.
         bg_color (str): Plot background color. Defaults to "rgba(0, 0, 0, 0)".
         color_bar (dict[str, Any]): Plotly color bar properties documented at
-            https://plotly.com/python/reference#heatmap-colorbar. Defaults to `{}`.
+            https://plotly.com/python/reference#heatmap-colorbar. Defaults to
+            dict(orientation="h").
         cscale_range (tuple[float | None, float | None]): Color bar range. Defaults to
             (None, None) meaning the range is automatically determined from the data.
         exclude_elements (list[str]): Elements to exclude from the heatmap. E.g. if
             oxygen overpowers everything, you can do exclude_elements=['O'].
             Defaults to ().
         log (bool): Whether to use a logarithmic color scale. Defaults to False.
             Piece of advice: colorscale='viridis' and log=True go well together.
@@ -474,14 +475,20 @@
     if log and heat_mode in ("fraction", "percent"):
         raise ValueError(
             "Combining log color scale and heat_mode='fraction'/'percent' unsupported"
         )
     if len(cscale_range) != 2:
         raise ValueError(f"{cscale_range=} should have length 2")
 
+    color_bar = color_bar or {}
+    color_bar.setdefault("orientation", "h")
+    # if elem_values is a series with a name, use it as the color bar title
+    if isinstance(elem_values, pd.Series) and elem_values.name:
+        color_bar.setdefault("title", elem_values.name)
+
     elem_values = count_elements(elem_values, count_mode, exclude_elements, fill_value)
 
     if log and elem_values[elem_values != 0].min() <= 1:
         raise ValueError(
             "Log color scale requires all heat map values to be > 1 since values <= 1 "
             "map to negative log values which throws off the color scale."
         )
@@ -612,11 +619,20 @@
         plot_bgcolor="rgba(0, 0, 0, 0)",
         xaxis=dict(zeroline=False, showgrid=False),
         yaxis=dict(zeroline=False, showgrid=False, scaleanchor="x"),
         font_size=font_size,
         width=1000,
         height=500,
     )
-    fig.update_traces(
-        colorbar=dict(lenmode="fraction", len=0.87, thickness=15, **(color_bar or {}))
-    )
+
+    if color_bar.get("orientation") == "h":
+        dct = dict(x=0.4, y=0.75, titleside="top", len=0.4)
+        color_bar = {**dct, **color_bar}
+    else:  # make title vertical
+        dct = dict(titleside="right", len=0.87)
+        color_bar = {**dct, **color_bar}
+        if title := color_bar.get("title"):
+            # <br><br> to increase title offset
+            color_bar["title"] = f"<br><br>{title}"
+
+    fig.update_traces(colorbar=dict(lenmode="fraction", thickness=15, **color_bar))
     return fig
```

### Comparing `pymatviz-0.6.1/pymatviz/relevance.py` & `pymatviz-0.6.2/pymatviz/relevance.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/sankey.py` & `pymatviz-0.6.2/pymatviz/sankey.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     labels_with_counts: bool | Literal["percent"] = True,
     **kwargs: Any,
 ) -> go.Figure:
     """Plot two columns of a dataframe as a Plotly Sankey diagram.
 
     Args:
         df (pd.DataFrame): Pandas dataframe.
-        cols (Sequence[str]): 2-tuple of source and target column names. Source
+        cols (list[str]): 2-tuple of source and target column names. Source
             corresponds to left, target to right side of the diagram.
         labels_with_counts (bool, optional): Whether to append value counts to node
             labels. Defaults to True.
         **kwargs: Additional keyword arguments passed to plotly.graph_objects.Sankey.
 
     Raises:
         ValueError: If len(cols) != 2.
```

### Comparing `pymatviz-0.6.1/pymatviz/structure_viz.py` & `pymatviz-0.6.2/pymatviz/structure_viz.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/sunburst.py` & `pymatviz-0.6.2/pymatviz/sunburst.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     fig.update_layout(uniformtext=dict(minsize=9, mode="hide"))
 
     Args:
         data (list[int] | pd.Series): A sequence (list, tuple, pd.Series) of
             space group strings or numbers (from 1 - 230) or pymatgen structures.
         show_counts ("value" | "percent" | False): Whether to display values below each
             labels on the sunburst.
+        color_discrete_sequence (list[str]): A list of 7 colors, one for each crystal
+            system. Defaults to plotly.express.colors.qualitative.G10.
         **kwargs: Additional keyword arguments passed to plotly.express.sunburst.
 
     Returns:
         Figure: The Plotly figure.
     """
     if isinstance(next(iter(data)), Structure):
         # if 1st sequence item is structure, assume all are
@@ -40,21 +42,20 @@
         )
     else:
         series = pd.Series(data)
 
     df = pd.DataFrame(series.value_counts().reset_index())
     df.columns = ["spacegroup", "count"]
 
-    try:
+    try:  # assume column contains integers as space group numbers
         df["crystal_sys"] = [get_crystal_sys(x) for x in df.spacegroup]
-    except ValueError:  # column must be space group strings
+    except ValueError:  # column must be strings of space group symbols
         df["crystal_sys"] = [SpaceGroup(x).crystal_system for x in df.spacegroup]
 
-    if "color_discrete_sequence" not in kwargs:
-        kwargs["color_discrete_sequence"] = px.colors.qualitative.G10
+    kwargs.setdefault("color_discrete_sequence", px.colors.qualitative.G10)
 
     fig = px.sunburst(df, path=["crystal_sys", "spacegroup"], values="count", **kwargs)
 
     if show_counts == "percent":
         fig.data[0].textinfo = "label+percent entry"
     elif show_counts == "value":
         fig.data[0].textinfo = "label+value"
```

### Comparing `pymatviz-0.6.1/pymatviz/uncertainty.py` & `pymatviz-0.6.2/pymatviz/uncertainty.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pymatviz/utils.py` & `pymatviz-0.6.2/pymatviz/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 from shutil import which
 from typing import Any, Literal, Sequence, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
+import sklearn
 from matplotlib.gridspec import GridSpec
 from matplotlib.offsetbox import AnchoredText
 from numpy.typing import NDArray
+from sklearn.metrics import mean_absolute_percentage_error as mape
 from sklearn.metrics import r2_score
 
 
 ROOT = dirname(dirname(__file__))
 
 Array = NDArray[Union[np.float64, np.int_]]
 
@@ -128,54 +130,81 @@
         # place label at end of the bar and center horizontally
         ax.annotate(txt, (x_pos, y_pos), ha="center", fontsize=fontsize, **kwargs)
 
     # ensure enough vertical space to display label above highest bar
     ax.set(ylim=(None, y_max * y_max_headroom))
 
 
-def annotate_mae_r2(
+def annotate_metrics(
     xs: NDArray[np.float64 | np.int_],
     ys: NDArray[np.float64 | np.int_],
     ax: plt.Axes = None,
+    metrics: dict[str, float] | Sequence[str] = ("MAE", "R2"),
     prefix: str = "",
     suffix: str = "",
     prec: int = 3,
     **kwargs: Any,
 ) -> AnchoredText:
     """Provide a set of x and y values of equal length and an optional Axes
     object on which to print the values' mean absolute error and R^2
     coefficient of determination.
 
     Args:
         xs (array, optional): x values.
         ys (array, optional): y values.
+        metrics (dict[str, float] | list[str], optional): Metrics to show. Can be a
+            subset of recognized keys MAE, R2, R2_adj, RMSE, MSE, MAPE or the names of
+            sklearn.metrics.regression functions or any dict of metric names and values.
+            Defaults to ("MAE", "R2").
         ax (Axes, optional): matplotlib Axes on which to add the box. Defaults to None.
         loc (str, optional): Where on the plot to place the AnchoredText object.
             Defaults to "lower right".
-        prec (int, optional): decimal places in printed metrics. Defaults to 3.
+        prec (int, optional): Precision, i.e. decimal places to show in printed metrics.
+            Defaults to 3.
         prefix (str, optional): Title or other string to prepend to metrics.
             Defaults to "".
         suffix (str, optional): Text to append after metrics. Defaults to "".
         **kwargs: Additional arguments (rotation, arrowprops, frameon, loc, etc.) are
             passed to matplotlib.offsetbox.AnchoredText. Sets default loc="lower right"
             and frameon=False.
 
     Returns:
         AnchoredText: Instance containing the metrics.
     """
-    ax = ax or plt.gca()
+    funcs = {
+        "MAE": lambda x, y: np.abs(x - y).mean(),
+        "RMSE": lambda x, y: (((x - y) ** 2).mean()) ** 0.5,
+        "MSE": lambda x, y: ((x - y) ** 2).mean(),
+        "MAPE": mape,
+        "R2": r2_score,
+        # TODO: check this for correctness
+        "R2_adj": lambda x, y: 1 - (1 - r2_score(x, y)) * (len(x) - 1) / (len(x) - 2),
+    }
+    for key in set(metrics) - set(funcs):
+        func = getattr(sklearn.metrics, key, None)
+        if func:
+            funcs[key] = func
+    if bad_keys := set(metrics) - set(funcs):
+        raise ValueError(f"Unrecognized metrics: {bad_keys}")
 
+    ax = ax or plt.gca()
     nans = np.isnan(xs) | np.isnan(ys)
     xs, ys = xs[~nans], ys[~nans]
 
-    text = f"{prefix}$\\mathrm{{MAE}} = {np.abs(xs - ys).mean():.{prec}f}$"
-    text += f"\n$R^2 = {r2_score(xs, ys):.{prec}f}${suffix}"
+    text = prefix
+    if isinstance(metrics, dict):
+        for key, val in metrics.items():
+            text += f"{key} = {val:.{prec}f}\n"
+    else:
+        for metric in metrics:
+            text += f"{metric} = {funcs[metric](xs, ys):.{prec}f}\n"
+    text += suffix
 
-    kwargs["frameon"] = kwargs.get("frameon", False)
-    kwargs["loc"] = kwargs.get("loc", "lower right")
+    kwargs["frameon"] = kwargs.get("frameon", False)  # default to no frame
+    kwargs["loc"] = kwargs.get("loc", "lower right")  # default to lower right
     text_box = AnchoredText(text, **kwargs)
     ax.add_artist(text_box)
 
     return text_box
 
 
 CrystalSystem = Literal[
@@ -405,7 +434,51 @@
         if isinstance(col_name, (str, int)):
             args[idx] = df_no_nan[col_name].values  # type: ignore[index]
         else:
             col_data = df_no_nan[[*col_name]].values.T
             args[idx] = dict(zip(col_name, col_data))  # type: ignore[index]
 
     return args  # type: ignore[return-value]
+
+
+def bin_df_cols(
+    df: pd.DataFrame,
+    bin_by_cols: Sequence[str],
+    group_by_cols: Sequence[str] = (),
+    n_bins: int | Sequence[int] = 100,
+    verbose: bool = True,
+) -> pd.DataFrame:
+    """Bin columns of a DataFrame.
+
+    Args:
+        df (pd.DataFrame): DataFrame to bin.
+        bin_by_cols (Sequence[str]): Columns to bin.
+        group_by_cols (Sequence[str]): Additional columns to group by. Defaults to ().
+        n_bins (int): Number of bins to use. Defaults to 100.
+        verbose (bool): If True, report df length reduction. Defaults to True.
+
+    Returns:
+        pd.DataFrame: Binned DataFrame.
+    """
+    if isinstance(n_bins, int):
+        n_bins = [n_bins] * len(bin_by_cols)
+
+    if len(bin_by_cols) != len(n_bins):
+        raise ValueError(f"{len(bin_by_cols)=} != {len(n_bins)=}")
+
+    index_name = df.index.name
+
+    for col, bins in zip(bin_by_cols, n_bins):
+        df[f"{col}_bins"] = pd.cut(df[col], bins=bins)
+
+    df_bin = (
+        df.reset_index()
+        .groupby([*[f"{c}_bins" for c in bin_by_cols], *group_by_cols])
+        .first()
+        .dropna()
+    )
+    if verbose:
+        print(f"{len(df_bin)=:,} / {len(df)=:,} = {len(df_bin)/len(df):.1%}")
+
+    if index_name is None:
+        return df_bin
+    return df_bin.reset_index().set_index(index_name)
```

### Comparing `pymatviz-0.6.1/pymatviz.egg-info/PKG-INFO` & `pymatviz-0.6.2/pymatviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatviz
-Version: 0.6.1
+Version: 0.6.2
 Summary: A toolkit for visualizations in materials informatics
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pymatviz-0.6.1/pymatviz.egg-info/SOURCES.txt` & `pymatviz-0.6.2/pymatviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/pyproject.toml` & `pymatviz-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymatviz"
-version = "0.6.1"
+version = "0.6.2"
 description = "A toolkit for visualizations in materials informatics"
 authors = [{ name = "Janosh Riebesell", email = "janosh.riebesell@gmail.com" }]
 readme = "readme.md"
 license = { file = "license" }
 keywords = [
     "science",
     "materials informatics",
@@ -62,17 +62,14 @@
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 show_error_codes = true
 no_implicit_optional = false
 
-[tool.codespell]
-ignore-words-list = "hist"
-
 [tool.ruff]
 target-version = "py38"
 select = [
     "B",   # flake8-bugbear
     "D",   # pydocstyle
     "E",   # pycodestyle
     "F",   # pyflakes
@@ -94,11 +91,12 @@
     "D205",    # 1 blank line required between summary line and description
     "SIM105",  # Use contextlib.suppress(FileNotFoundError) instead of try-except-pass
     "SIM115",  # Use context handler for opening files
     "PLW2901", # Outer for loop variable overwritten by inner assignment target
 ]
 pydocstyle.convention = "google"
 isort.lines-after-imports = 2
+isort.split-on-trailing-comma = false
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D103"]
 "examples/*" = ["E402"] # E402 Module level import not at top of file
```

### Comparing `pymatviz-0.6.1/readme.md` & `pymatviz-0.6.2/readme.md`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/tests/test_cumulative.py` & `pymatviz-0.6.2/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/tests/test_histograms.py` & `pymatviz-0.6.2/tests/test_histograms.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/tests/test_parity.py` & `pymatviz-0.6.2/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/tests/test_ptable.py` & `pymatviz-0.6.2/tests/test_ptable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Literal, Sequence
+from typing import TYPE_CHECKING, Any, Literal, Sequence
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import plotly.graph_objects as go
 import pytest
 from plotly.exceptions import PlotlyError
 from pymatgen.core import Composition
@@ -247,14 +247,31 @@
     glass_formulas: list[str], colorscale: str | list[tuple[float, str]] | list[str]
 ) -> None:
     fig = ptable_heatmap_plotly(glass_formulas, colorscale=colorscale)
     assert isinstance(fig, go.Figure)
 
 
 @pytest.mark.parametrize(
+    "color_bar", [{}, dict(orientation="v", len=0.8), dict(orientation="h", len=0.3)]
+)
+def test_ptable_heatmap_plotly_color_bar(
+    glass_formulas: list[str], color_bar: dict[str, Any]
+) -> None:
+    fig = ptable_heatmap_plotly(glass_formulas, color_bar=color_bar)
+    # check color bar has expected length
+    assert fig.data[0].colorbar.len == color_bar.get("len", 0.4)
+    # check color bar has expected title side
+    assert (
+        fig.data[0].colorbar.title.side == "right"
+        if color_bar.get("orientation") == "v"
+        else "top"
+    )
+
+
+@pytest.mark.parametrize(
     "cscale_range", [(None, None), (None, 10), (2, None), (2, 87123)]
 )
 def test_ptable_heatmap_plotly_cscale_range(
     cscale_range: tuple[float | None, float | None]
 ) -> None:
     fig = ptable_heatmap_plotly(df_ptable.density, cscale_range=cscale_range)
     trace = fig.data[0]
```

### Comparing `pymatviz-0.6.1/tests/test_relevance.py` & `pymatviz-0.6.2/tests/test_relevance.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/tests/test_sankey.py` & `pymatviz-0.6.2/tests/test_sankey.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/tests/test_structure_viz.py` & `pymatviz-0.6.2/tests/test_structure_viz.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/tests/test_sunburst.py` & `pymatviz-0.6.2/tests/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.6.1/tests/test_uncertainty.py` & `pymatviz-0.6.2/tests/test_uncertainty.py`

 * *Files identical despite different names*

