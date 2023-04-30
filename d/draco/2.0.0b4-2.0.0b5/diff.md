# Comparing `tmp/draco-2.0.0b4.tar.gz` & `tmp/draco-2.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draco-2.0.0b4.tar", max compression
+gzip compressed data, was "draco-2.0.0b5.tar", max compression
```

## Comparing `draco-2.0.0b4.tar` & `draco-2.0.0b5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1083 2022-04-19 20:57:42.753033 draco-2.0.0b4/LICENSE
--rw-r--r--   0        0        0     3549 2023-04-25 09:07:22.107407 draco-2.0.0b4/README.md
--rw-r--r--   0        0        0      707 2023-04-25 09:07:22.130663 draco-2.0.0b4/draco/__init__.py
--rw-r--r--   0        0        0      937 2023-03-14 21:04:07.214822 draco-2.0.0b4/draco/asp/constraints.lp
--rw-r--r--   0        0        0     2665 2023-02-21 20:03:46.615187 draco-2.0.0b4/draco/asp/define.lp
--rw-r--r--   0        0        0      732 2023-02-22 00:53:57.429000 draco-2.0.0b4/draco/asp/examples/binned_histogram.lp
--rw-r--r--   0        0        0      378 2023-02-22 00:53:57.429114 draco-2.0.0b4/draco/asp/examples/histogram.lp
--rw-r--r--   0        0        0      442 2023-02-22 00:53:57.429223 draco-2.0.0b4/draco/asp/examples/scatter.lp
--rw-r--r--   0        0        0     2350 2023-03-14 21:04:07.215023 draco-2.0.0b4/draco/asp/generate.lp
--rw-r--r--   0        0        0    13784 2023-04-25 09:07:22.130837 draco-2.0.0b4/draco/asp/hard.lp
--rw-r--r--   0        0        0     8080 2023-02-21 20:03:46.616073 draco-2.0.0b4/draco/asp/helpers.lp
--rw-r--r--   0        0        0       93 2022-08-01 22:17:04.349097 draco-2.0.0b4/draco/asp/optimize.lp
--rw-r--r--   0        0        0    29338 2023-03-14 21:04:07.217532 draco-2.0.0b4/draco/asp/soft.lp
--rw-r--r--   0        0        0     5131 2022-09-21 02:36:09.549479 draco-2.0.0b4/draco/asp/weights.lp
--rw-r--r--   0        0        0     2793 2022-10-20 16:32:52.848814 draco-2.0.0b4/draco/asp_utils.py
--rw-r--r--   0        0        0     4644 2023-02-22 00:53:57.429357 draco-2.0.0b4/draco/data_utils.py
--rw-r--r--   0        0        0    11482 2023-04-25 09:07:22.132754 draco-2.0.0b4/draco/debug.py
--rw-r--r--   0        0        0     6569 2023-03-14 21:04:07.219601 draco-2.0.0b4/draco/draco.py
--rw-r--r--   0        0        0     4700 2022-10-20 16:32:52.849656 draco-2.0.0b4/draco/fact_utils.py
--rw-r--r--   0        0        0     1014 2022-10-20 16:32:52.849759 draco-2.0.0b4/draco/learn.py
--rw-r--r--   0        0        0      894 2022-07-20 22:03:10.295971 draco-2.0.0b4/draco/programs.py
--rw-r--r--   0        0        0      152 2022-12-14 14:56:46.108312 draco-2.0.0b4/draco/renderer/__init__.py
--rw-r--r--   0        0        0        0 2022-12-14 14:56:46.108392 draco-2.0.0b4/draco/renderer/altair/__init__.py
--rw-r--r--   0        0        0    21230 2023-02-22 00:53:57.429553 draco-2.0.0b4/draco/renderer/altair/altair_renderer.py
--rw-r--r--   0        0        0     9115 2023-02-22 00:53:57.429707 draco-2.0.0b4/draco/renderer/altair/types.py
--rw-r--r--   0        0        0      690 2022-12-14 14:56:46.108996 draco-2.0.0b4/draco/renderer/base_renderer.py
--rw-r--r--   0        0        0     4245 2022-10-20 16:32:52.850407 draco-2.0.0b4/draco/run.py
--rw-r--r--   0        0        0     3824 2022-10-20 16:32:52.850557 draco-2.0.0b4/draco/schema.py
--rw-r--r--   0        0        0      123 2022-10-20 16:53:07.528276 draco-2.0.0b4/draco/server/__init__.py
--rw-r--r--   0        0        0      581 2022-10-20 16:53:07.528361 draco-2.0.0b4/draco/server/__main__.py
--rw-r--r--   0        0        0     4245 2023-04-25 09:07:22.132928 draco-2.0.0b4/draco/server/draco_api.py
--rw-r--r--   0        0        0     2333 2023-04-25 09:07:22.133360 draco-2.0.0b4/draco/server/main.py
--rw-r--r--   0        0        0        0 2022-10-20 16:53:07.528571 draco-2.0.0b4/draco/server/models/__init__.py
--rw-r--r--   0        0        0      382 2022-10-20 16:53:07.528705 draco-2.0.0b4/draco/server/models/clingo.py
--rw-r--r--   0        0        0     1042 2022-10-20 16:53:07.528771 draco-2.0.0b4/draco/server/models/draco.py
--rw-r--r--   0        0        0      231 2023-04-25 09:07:22.133555 draco-2.0.0b4/draco/server/models/renderer.py
--rw-r--r--   0        0        0      279 2022-10-20 16:53:07.528834 draco-2.0.0b4/draco/server/models/shared.py
--rw-r--r--   0        0        0      555 2022-10-20 16:53:07.528909 draco-2.0.0b4/draco/server/models/utility.py
--rw-r--r--   0        0        0      290 2023-04-25 09:07:22.133756 draco-2.0.0b4/draco/server/routers/__init__.py
--rw-r--r--   0        0        0     1503 2022-11-03 14:35:21.548943 draco-2.0.0b4/draco/server/routers/base.py
--rw-r--r--   0        0        0      945 2022-11-03 14:35:21.549065 draco-2.0.0b4/draco/server/routers/clingo.py
--rw-r--r--   0        0        0     1671 2022-11-03 14:35:21.549178 draco-2.0.0b4/draco/server/routers/draco.py
--rw-r--r--   0        0        0     1157 2023-04-25 09:07:22.133856 draco-2.0.0b4/draco/server/routers/renderer.py
--rw-r--r--   0        0        0     1156 2022-11-03 14:35:21.549282 draco-2.0.0b4/draco/server/routers/utility.py
--rw-r--r--   0        0        0        0 2022-10-20 16:53:07.529314 draco-2.0.0b4/draco/server/services/__init__.py
--rw-r--r--   0        0        0      456 2022-10-20 16:53:07.529403 draco-2.0.0b4/draco/server/services/clingo.py
--rw-r--r--   0        0        0     1139 2022-10-20 16:53:07.529475 draco-2.0.0b4/draco/server/services/draco.py
--rw-r--r--   0        0        0      417 2023-04-25 09:07:22.133951 draco-2.0.0b4/draco/server/services/renderer.py
--rw-r--r--   0        0        0     1036 2022-10-20 16:53:07.529542 draco-2.0.0b4/draco/server/services/utility.py
--rw-r--r--   0        0        0     1177 2023-04-25 09:07:22.134096 draco-2.0.0b4/draco/server/utils.py
--rw-r--r--   0        0        0       87 2022-10-20 16:32:52.852528 draco-2.0.0b4/draco/types.py
--rw-r--r--   0        0        0      121 2022-07-20 22:03:10.273941 draco-2.0.0b4/draco/utils.py
--rw-r--r--   0        0        0     1344 2022-10-20 16:32:52.853238 draco-2.0.0b4/draco/weights.py
--rw-r--r--   0        0        0     2233 2023-04-25 09:35:43.821264 draco-2.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 draco-2.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-04-19 20:57:42.753033 draco-2.0.0b5/LICENSE
+-rw-r--r--   0        0        0     3549 2023-04-25 09:07:22.107407 draco-2.0.0b5/README.md
+-rw-r--r--   0        0        0      707 2023-04-25 09:07:22.130663 draco-2.0.0b5/draco/__init__.py
+-rw-r--r--   0        0        0      937 2023-03-14 21:04:07.214822 draco-2.0.0b5/draco/asp/constraints.lp
+-rw-r--r--   0        0        0     2665 2023-02-21 20:03:46.615187 draco-2.0.0b5/draco/asp/define.lp
+-rw-r--r--   0        0        0      732 2023-02-22 00:53:57.429000 draco-2.0.0b5/draco/asp/examples/binned_histogram.lp
+-rw-r--r--   0        0        0      378 2023-02-22 00:53:57.429114 draco-2.0.0b5/draco/asp/examples/histogram.lp
+-rw-r--r--   0        0        0      442 2023-02-22 00:53:57.429223 draco-2.0.0b5/draco/asp/examples/scatter.lp
+-rw-r--r--   0        0        0     2350 2023-04-30 19:36:29.389186 draco-2.0.0b5/draco/asp/generate.lp
+-rw-r--r--   0        0        0    13784 2023-04-30 19:36:29.389411 draco-2.0.0b5/draco/asp/hard.lp
+-rw-r--r--   0        0        0     8081 2023-04-30 19:36:29.389605 draco-2.0.0b5/draco/asp/helpers.lp
+-rw-r--r--   0        0        0       93 2022-08-01 22:17:04.349097 draco-2.0.0b5/draco/asp/optimize.lp
+-rw-r--r--   0        0        0    29339 2023-04-30 19:36:29.393384 draco-2.0.0b5/draco/asp/soft.lp
+-rw-r--r--   0        0        0     5131 2022-09-21 02:36:09.549479 draco-2.0.0b5/draco/asp/weights.lp
+-rw-r--r--   0        0        0     2793 2022-10-20 16:32:52.848814 draco-2.0.0b5/draco/asp_utils.py
+-rw-r--r--   0        0        0     4644 2023-02-22 00:53:57.429357 draco-2.0.0b5/draco/data_utils.py
+-rw-r--r--   0        0        0    11704 2023-04-27 13:37:30.584822 draco-2.0.0b5/draco/debug.py
+-rw-r--r--   0        0        0     6569 2023-03-14 21:04:07.219601 draco-2.0.0b5/draco/draco.py
+-rw-r--r--   0        0        0     4700 2022-10-20 16:32:52.849656 draco-2.0.0b5/draco/fact_utils.py
+-rw-r--r--   0        0        0     1014 2022-10-20 16:32:52.849759 draco-2.0.0b5/draco/learn.py
+-rw-r--r--   0        0        0      894 2022-07-20 22:03:10.295971 draco-2.0.0b5/draco/programs.py
+-rw-r--r--   0        0        0      152 2022-12-14 14:56:46.108312 draco-2.0.0b5/draco/renderer/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-14 14:56:46.108392 draco-2.0.0b5/draco/renderer/altair/__init__.py
+-rw-r--r--   0        0        0    21230 2023-02-22 00:53:57.429553 draco-2.0.0b5/draco/renderer/altair/altair_renderer.py
+-rw-r--r--   0        0        0     9115 2023-02-22 00:53:57.429707 draco-2.0.0b5/draco/renderer/altair/types.py
+-rw-r--r--   0        0        0      690 2022-12-14 14:56:46.108996 draco-2.0.0b5/draco/renderer/base_renderer.py
+-rw-r--r--   0        0        0     4245 2022-10-20 16:32:52.850407 draco-2.0.0b5/draco/run.py
+-rw-r--r--   0        0        0     3824 2022-10-20 16:32:52.850557 draco-2.0.0b5/draco/schema.py
+-rw-r--r--   0        0        0      123 2022-10-20 16:53:07.528276 draco-2.0.0b5/draco/server/__init__.py
+-rw-r--r--   0        0        0      581 2022-10-20 16:53:07.528361 draco-2.0.0b5/draco/server/__main__.py
+-rw-r--r--   0        0        0     4245 2023-04-25 09:07:22.132928 draco-2.0.0b5/draco/server/draco_api.py
+-rw-r--r--   0        0        0     2333 2023-04-25 09:07:22.133360 draco-2.0.0b5/draco/server/main.py
+-rw-r--r--   0        0        0        0 2022-10-20 16:53:07.528571 draco-2.0.0b5/draco/server/models/__init__.py
+-rw-r--r--   0        0        0      382 2022-10-20 16:53:07.528705 draco-2.0.0b5/draco/server/models/clingo.py
+-rw-r--r--   0        0        0     1042 2022-10-20 16:53:07.528771 draco-2.0.0b5/draco/server/models/draco.py
+-rw-r--r--   0        0        0      231 2023-04-25 09:07:22.133555 draco-2.0.0b5/draco/server/models/renderer.py
+-rw-r--r--   0        0        0      279 2022-10-20 16:53:07.528834 draco-2.0.0b5/draco/server/models/shared.py
+-rw-r--r--   0        0        0      555 2022-10-20 16:53:07.528909 draco-2.0.0b5/draco/server/models/utility.py
+-rw-r--r--   0        0        0      290 2023-04-25 09:07:22.133756 draco-2.0.0b5/draco/server/routers/__init__.py
+-rw-r--r--   0        0        0     1503 2022-11-03 14:35:21.548943 draco-2.0.0b5/draco/server/routers/base.py
+-rw-r--r--   0        0        0      945 2022-11-03 14:35:21.549065 draco-2.0.0b5/draco/server/routers/clingo.py
+-rw-r--r--   0        0        0     1671 2022-11-03 14:35:21.549178 draco-2.0.0b5/draco/server/routers/draco.py
+-rw-r--r--   0        0        0     1157 2023-04-25 09:07:22.133856 draco-2.0.0b5/draco/server/routers/renderer.py
+-rw-r--r--   0        0        0     1156 2022-11-03 14:35:21.549282 draco-2.0.0b5/draco/server/routers/utility.py
+-rw-r--r--   0        0        0        0 2022-10-20 16:53:07.529314 draco-2.0.0b5/draco/server/services/__init__.py
+-rw-r--r--   0        0        0      456 2022-10-20 16:53:07.529403 draco-2.0.0b5/draco/server/services/clingo.py
+-rw-r--r--   0        0        0     1139 2022-10-20 16:53:07.529475 draco-2.0.0b5/draco/server/services/draco.py
+-rw-r--r--   0        0        0      417 2023-04-25 09:07:22.133951 draco-2.0.0b5/draco/server/services/renderer.py
+-rw-r--r--   0        0        0     1036 2022-10-20 16:53:07.529542 draco-2.0.0b5/draco/server/services/utility.py
+-rw-r--r--   0        0        0     1177 2023-04-25 09:07:22.134096 draco-2.0.0b5/draco/server/utils.py
+-rw-r--r--   0        0        0       87 2022-10-20 16:32:52.852528 draco-2.0.0b5/draco/types.py
+-rw-r--r--   0        0        0      121 2022-07-20 22:03:10.273941 draco-2.0.0b5/draco/utils.py
+-rw-r--r--   0        0        0     1344 2022-10-20 16:32:52.853238 draco-2.0.0b5/draco/weights.py
+-rw-r--r--   0        0        0     2379 2023-04-30 19:37:11.451472 draco-2.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     4952 1970-01-01 00:00:00.000000 draco-2.0.0b5/PKG-INFO
```

### Comparing `draco-2.0.0b4/LICENSE` & `draco-2.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/README.md` & `draco-2.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/__init__.py` & `draco-2.0.0b5/draco/__init__.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/asp/constraints.lp` & `draco-2.0.0b5/draco/asp/constraints.lp`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/asp/define.lp` & `draco-2.0.0b5/draco/asp/define.lp`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/asp/examples/binned_histogram.lp` & `draco-2.0.0b5/draco/asp/examples/binned_histogram.lp`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/asp/generate.lp` & `draco-2.0.0b5/draco/asp/generate.lp`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 % @generator(encoding_attribute) Encoding with binning, aggregate, field or stack.
 not_required((encoding,binning)).
 not_required((encoding,aggregate)).
 not_required((encoding,stack)).
 0 { attribute((encoding,field),E,N): domain((field,name),N) } 1 :- entity(encoding,_,E).
 
-% generator(scale) generate scales such that their ids and channels corresponde to the encodings in each view.
+% generator(scale) generate scales such that their ids and channels corresponds to the encodings in each view.
 { entity(scale,V,(s,E)) } :- entity(mark,V,M), entity(encoding,M,E), attribute((encoding,channel),E,C).
 attribute((scale,channel),(s,E),C) :- entity(scale,V,(s,E)), attribute((encoding,channel),E,C).
 
 required((scale,channel)).
 required((scale,type)).
 not_required((scale,zero)).
```

### Comparing `draco-2.0.0b4/draco/asp/hard.lp` & `draco-2.0.0b5/draco/asp/hard.lp`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 % @hard(count_without_q) Count has to have a continuous scale.
 violation(count_without_q) :-
     attribute((encoding,aggregate),E,count),
     helper((encoding,scale_type),E,T),
     domain(discrete_scale,T).
 
-% @hard(shape_not_ordinal) Shape requires discrete and ordinal (ordinal/categorical doesn't matter as scale types, so we use oridnal only here).
+% @hard(shape_not_ordinal) Shape requires discrete and ordinal (ordinal/categorical doesn't matter as scale types, so we use ordinal only here).
 violation(shape_not_ordinal) :-
     helper(mark_scale_channel,_,T,shape),
     T != ordinal.
 
 % @hard(categorical_not_color) Categorical only works with color channel.
 violation(categorical_not_color) :-
     attribute((scale,type),S,categorical),
```

### Comparing `draco-2.0.0b4/draco/asp/helpers.lp` & `draco-2.0.0b5/draco/asp/helpers.lp`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 % @helper(mark_scale_channel) Whether a mark has a scale type for a channel.
 helper(mark_scale_channel,M,T,C) :-
     helper((mark,scale),M,S),
     attribute((scale,channel),S,C),
     attribute((scale,type),S,T).
 
-% @helper(mark_encoding_scale) Link mark, encoding, and scale togther.
+% @helper(mark_encoding_scale) Link mark, encoding, and scale together.
 helper(mark_encoding_scale,M,E,S) :-
     entity(encoding,M,E),
     attribute((encoding,channel),E,C),
     helper((mark,scale),M,S),
     attribute((scale,channel),S,C).
 
 % @helper(encoding_type) Whether an encoding has a channel for a scale type.
```

### Comparing `draco-2.0.0b4/draco/asp/soft.lp` & `draco-2.0.0b5/draco/asp/soft.lp`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     attribute((scale,zero),S,true).
 
 % @soft(only_y) Prefer to use only x instead of only y.
 preference(only_y,M) :-
     helper((mark,channel),M,y),
     not helper((mark,channel),M,x).
 
-% @soft(binned_orientation_not_x) Prefer binned quantative on x axis.
+% @soft(binned_orientation_not_x) Prefer binned quantitative on x axis.
 preference(binned_orientation_not_x,E) :-
     attribute((field,type),F,(number;datetime)),
     helper((encoding,field),E,F),
     attribute((encoding,binning),E,_),
     not attribute((encoding,channel),_,x).
 
 % @soft(high_cardinality_ordinal) Prefer not to use ordinal for fields with high cardinality.
@@ -423,15 +423,15 @@
     helper(overlap,M).
 
 % @soft(d_d_point) Discrete by discrete for point mark.
 preference(d_d_point,M) :-
     helper(is_d_d,M),
     attribute((mark,type),M,point).
 
-% @soft(d_d_text) Discrete by discretee for text mark.
+% @soft(d_d_text) Discrete by discrete for text mark.
 preference(d_d_text,M) :-
     helper(is_d_d,M),
     attribute((mark,type),M,text).
 
 % @soft(d_d_rect) Discrete by discrete for rect mark.
 preference(d_d_rect,M) :-
     helper(is_d_d,M),
```

### Comparing `draco-2.0.0b4/draco/asp/weights.lp` & `draco-2.0.0b5/draco/asp/weights.lp`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/asp_utils.py` & `draco-2.0.0b5/draco/asp_utils.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/data_utils.py` & `draco-2.0.0b5/draco/data_utils.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/debug.py` & `draco-2.0.0b5/draco/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,23 +205,28 @@
         to create charts visualizing the Draco debug data.
 
         :param chart_preferences: the ``DataFrame``
                                   returned by ``DracoDebug.chart_preferences``
         """
         self.chart_preferences = chart_preferences
 
-    def _compute_ideal_plot_size(self) -> tuple[float, float]:
+    @staticmethod
+    def _compute_ideal_plot_size(
+        chart_preferences: pd.DataFrame,
+    ) -> tuple[float, float]:
         cell_width, cell_height = DracoDebugPlotter.__DEFAULT_CELL_SIZE__
-        num_prefs = len(set(self.chart_preferences["pref_name"]))
-        num_charts = len(set(self.chart_preferences["chart_name"]))
+        num_prefs = len(set(chart_preferences["pref_name"]))
+        num_charts = len(set(chart_preferences["chart_name"]))
 
         width = num_prefs * cell_width
-        height = 1.25 * (num_charts * cell_height)
+        # The heatmap has 3/4 the height of the full chart
+        heatmap_height = num_charts * cell_height
+        height = (4 / 3) * heatmap_height
         width_max, height_max = DracoDebugPlotter.__DEFAULT_PLOT_SIZE__
-        return min(width, width_max), min(height, height_max)
+        return (width, height) if width < width_max else (width_max, height_max)
 
     def create_chart(
         self,
         *,
         cfg: DracoDebugChartConfig | ChartConfig | None = None,
         violated_prefs_only: bool = False,
         plot_size: tuple[float, float] | None = None,
@@ -238,22 +243,25 @@
                                     by at least one spec. Defaults to ``False``.
         :param plot_size: the size of the plot described as a tuple of (width, height).
         :return: the above-described Altair chart
         """
         used_config: ChartConfig = DracoDebugChartConfig.SORT_ALPHABETICALLY.value
         if cfg is not None:
             used_config = cfg if isinstance(cfg, ChartConfig) else cfg.value
-        width, height = plot_size or self._compute_ideal_plot_size()
 
         chart_preferences = self.chart_preferences
         if violated_prefs_only:
             chart_preferences = chart_preferences[
                 chart_preferences["count"] != 0
             ].reset_index()
 
+        width, height = plot_size or DracoDebugPlotter._compute_ideal_plot_size(
+            chart_preferences
+        )
+
         return self.__create_chart(
             chart_preferences=chart_preferences,
             cfg=used_config,
             width=width,
             height=height,
         )
```

### Comparing `draco-2.0.0b4/draco/draco.py` & `draco-2.0.0b5/draco/draco.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/fact_utils.py` & `draco-2.0.0b5/draco/fact_utils.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/learn.py` & `draco-2.0.0b5/draco/learn.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/programs.py` & `draco-2.0.0b5/draco/programs.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/renderer/altair/altair_renderer.py` & `draco-2.0.0b5/draco/renderer/altair/altair_renderer.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/renderer/altair/types.py` & `draco-2.0.0b5/draco/renderer/altair/types.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/renderer/base_renderer.py` & `draco-2.0.0b5/draco/renderer/base_renderer.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/run.py` & `draco-2.0.0b5/draco/run.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/schema.py` & `draco-2.0.0b5/draco/schema.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/__main__.py` & `draco-2.0.0b5/draco/server/__main__.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/draco_api.py` & `draco-2.0.0b5/draco/server/draco_api.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/main.py` & `draco-2.0.0b5/draco/server/main.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/models/draco.py` & `draco-2.0.0b5/draco/server/models/draco.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/models/utility.py` & `draco-2.0.0b5/draco/server/models/utility.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/routers/base.py` & `draco-2.0.0b5/draco/server/routers/base.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/routers/clingo.py` & `draco-2.0.0b5/draco/server/routers/clingo.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/routers/draco.py` & `draco-2.0.0b5/draco/server/routers/draco.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/routers/renderer.py` & `draco-2.0.0b5/draco/server/routers/renderer.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/routers/utility.py` & `draco-2.0.0b5/draco/server/routers/utility.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/services/draco.py` & `draco-2.0.0b5/draco/server/services/draco.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/services/utility.py` & `draco-2.0.0b5/draco/server/services/utility.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/server/utils.py` & `draco-2.0.0b5/draco/server/utils.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/draco/weights.py` & `draco-2.0.0b5/draco/weights.py`

 * *Files identical despite different names*

### Comparing `draco-2.0.0b4/pyproject.toml` & `draco-2.0.0b5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "draco"
-version = "2.0.0b4"
+version = "2.0.0b5"
 description = "Visualization recommendation using constraints"
 authors = [
     "Dominik Moritz <domoritz@cmu.edu>",
     "Chenglong Wang <clwang@cs.washington.edu>",
     "JunranY <junran@cs.washington.edu>",
     "Zehua Zeng <zhzeng@umd.edu>",
     "Péter Ferenc Gyarmati <peter.ferenc.gyarmati@univie.ac.at>"
@@ -16,18 +16,23 @@
 keywords = ["constraints", "visualization", "design", "charts"]
 exclude = ["draco/tests/*"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Environment :: MacOS X",
+    "Environment :: WebAssembly",
+    "Framework :: FastAPI",
+    "Framework :: Jupyter",
+    "Framework :: Pydantic",
+    "Framework :: Pytest",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
-    "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
+    "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 altair = "^4.2.2"
 clingo = "^5.5.2"
 fastapi = ">=0.85,<0.96"
```

### Comparing `draco-2.0.0b4/PKG-INFO` & `draco-2.0.0b5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: draco
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: Visualization recommendation using constraints
 Home-page: https://github.com/cmudig/draco2
 License: MIT
 Keywords: constraints,visualization,design,charts
 Author: Dominik Moritz
 Author-email: domoritz@cmu.edu
 Requires-Python: >=3.10.0,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
+Classifier: Environment :: WebAssembly
+Classifier: Framework :: FastAPI
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: draco Version: 2.0.0b4 Summary: Visualization
+Metadata-Version: 2.1 Name: draco Version: 2.0.0b5 Summary: Visualization
 recommendation using constraints Home-page: https://github.com/cmudig/draco2
 License: MIT Keywords: constraints,visualization,design,charts Author: Dominik
 Moritz Author-email: domoritz@cmu.edu Requires-Python: >=3.10.0,<3.11
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
-Classifier: Environment :: MacOS X Classifier: License :: OSI Approved :: MIT
-License Classifier: Natural Language :: English Classifier: Operating System ::
-MacOS :: MacOS X Classifier: Operating System :: POSIX :: Linux Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
-altair (>=4.2.2,<5.0.0) Requires-Dist: clingo (>=5.5.2,<6.0.0) Requires-Dist:
-fastapi (>=0.85,<0.96) Requires-Dist: pandas (>=1.4.2,<3.0.0) Requires-Dist:
-pydantic (>=1.10.5,<2.0.0) Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
-Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist: uvicorn
-(>=0.18.3,<0.22.0) Project-URL: Documentation, https://dig.cmu.edu/draco2/
-Project-URL: Repository, https://github.com/cmudig/draco2 Description-Content-
-Type: text/markdown
+Classifier: Environment :: MacOS X Classifier: Environment :: WebAssembly
+Classifier: Framework :: FastAPI Classifier: Framework :: Jupyter Classifier:
+Framework :: Pydantic Classifier: Framework :: Pytest Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
+Linux Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: altair (>=4.2.2,<5.0.0) Requires-Dist: clingo (>=5.5.2,<6.0.0)
+Requires-Dist: fastapi (>=0.85,<0.96) Requires-Dist: pandas (>=1.4.2,<3.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist: scikit-learn
+(>=1.2.1,<2.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
+uvicorn (>=0.18.3,<0.22.0) Project-URL: Documentation, https://dig.cmu.edu/
+draco2/ Project-URL: Repository, https://github.com/cmudig/draco2 Description-
+Content-Type: text/markdown
   ___[The_Draco_logo._A_set_of_circles_connected_by_lines_depicting_the_draco
                              star_constellation.]_
 # Draco v2 [![Open in GitHub Codespaces](https://img.shields.io/badge/launch-
 Codespaces-blue)](https://github.com/codespaces/
 new?hide_repo_select=true&ref=main&repo=313704611&machine=standardLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)
 [![PyPi](https://img.shields.io/pypi/v/draco.svg)](https://pypi.org/project/
 draco/) [![npm](https://img.shields.io/npm/v/draco-pyodide)](https://
```

