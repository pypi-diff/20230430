# Comparing `tmp/hitchstory-0.9.0.tar.gz` & `tmp/hitchstory-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hitchstory-0.9.0.tar", last modified: Sun Jan  7 17:44:13 2018, max compression
+gzip compressed data, was "dist/hitchstory-0.9.1.tar", last modified: Wed Jan 31 19:29:43 2018, max compression
```

## Comparing `hitchstory-0.9.0.tar` & `hitchstory-0.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 colm      (1000) colm      (1000)        0 2018-01-07 17:44:13.000000 hitchstory-0.9.0/
--rw-rw-r--   0 colm      (1000) colm      (1000)     1851 2018-01-04 19:13:36.000000 hitchstory-0.9.0/setup.py
-drwxrwxr-x   0 colm      (1000) colm      (1000)        0 2018-01-07 17:44:13.000000 hitchstory-0.9.0/hitchstory.egg-info/
--rw-rw-r--   0 colm      (1000) colm      (1000)        1 2018-01-07 17:44:12.000000 hitchstory-0.9.0/hitchstory.egg-info/dependency_links.txt
--rw-rw-r--   0 colm      (1000) colm      (1000)      101 2018-01-07 17:44:12.000000 hitchstory-0.9.0/hitchstory.egg-info/requires.txt
--rw-rw-r--   0 colm      (1000) colm      (1000)        1 2017-12-15 08:13:14.000000 hitchstory-0.9.0/hitchstory.egg-info/not-zip-safe
--rw-rw-r--   0 colm      (1000) colm      (1000)     4858 2018-01-07 17:44:12.000000 hitchstory-0.9.0/hitchstory.egg-info/PKG-INFO
--rw-rw-r--   0 colm      (1000) colm      (1000)       11 2018-01-07 17:44:12.000000 hitchstory-0.9.0/hitchstory.egg-info/top_level.txt
--rw-rw-r--   0 colm      (1000) colm      (1000)      683 2018-01-07 17:44:13.000000 hitchstory-0.9.0/hitchstory.egg-info/SOURCES.txt
--rw-rw-r--   0 colm      (1000) colm      (1000)     4858 2018-01-07 17:44:13.000000 hitchstory-0.9.0/PKG-INFO
--rw-rw-r--   0 colm      (1000) colm      (1000)        5 2018-01-07 17:44:06.000000 hitchstory-0.9.0/VERSION
--rw-rw-r--   0 colm      (1000) colm      (1000)       59 2017-12-14 08:17:21.000000 hitchstory-0.9.0/MANIFEST.in
--rw-rw-r--   0 colm      (1000) colm      (1000)     3007 2017-12-14 12:52:21.000000 hitchstory-0.9.0/README.rst
--rw-rw-r--   0 colm      (1000) colm      (1000)       38 2018-01-07 17:44:13.000000 hitchstory-0.9.0/setup.cfg
-drwxrwxr-x   0 colm      (1000) colm      (1000)        0 2018-01-07 17:44:13.000000 hitchstory-0.9.0/hitchstory/
--rw-rw-r--   0 colm      (1000) colm      (1000)     3228 2018-01-06 21:24:32.000000 hitchstory-0.9.0/hitchstory/story_step.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     1026 2017-12-14 08:17:21.000000 hitchstory-0.9.0/hitchstory/story_list.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     3138 2018-01-06 21:27:12.000000 hitchstory-0.9.0/hitchstory/step_method.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     4717 2018-01-07 15:15:28.000000 hitchstory-0.9.0/hitchstory/story_file.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     2207 2018-01-07 14:45:56.000000 hitchstory-0.9.0/hitchstory/arguments.py
-drwxrwxr-x   0 colm      (1000) colm      (1000)        0 2018-01-07 17:44:13.000000 hitchstory-0.9.0/hitchstory/templates/
--rw-rw-r--   0 colm      (1000) colm      (1000)     1310 2017-12-14 08:17:21.000000 hitchstory-0.9.0/hitchstory/templates/multiple.jinja2
--rw-rw-r--   0 colm      (1000) colm      (1000)     2702 2017-12-14 08:17:21.000000 hitchstory-0.9.0/hitchstory/templates/stacktrace_default.jinja2
--rw-rw-r--   0 colm      (1000) colm      (1000)      250 2017-12-14 08:17:21.000000 hitchstory-0.9.0/hitchstory/templates/failure.jinja2
--rw-rw-r--   0 colm      (1000) colm      (1000)      127 2017-12-19 16:19:52.000000 hitchstory-0.9.0/hitchstory/templates/success.jinja2
--rw-rw-r--   0 colm      (1000) colm      (1000)     4226 2017-12-14 08:17:21.000000 hitchstory-0.9.0/hitchstory/exceptions.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     3488 2018-01-07 14:08:03.000000 hitchstory-0.9.0/hitchstory/result.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     1802 2018-01-07 14:45:16.000000 hitchstory-0.9.0/hitchstory/utils.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     8293 2018-01-07 15:34:31.000000 hitchstory-0.9.0/hitchstory/story.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     3307 2018-01-07 15:37:28.000000 hitchstory-0.9.0/hitchstory/engine.py
--rw-rw-r--   0 colm      (1000) colm      (1000)      482 2018-01-07 17:44:12.000000 hitchstory-0.9.0/hitchstory/__init__.py
--rw-rw-r--   0 colm      (1000) colm      (1000)     8754 2018-01-04 21:51:03.000000 hitchstory-0.9.0/hitchstory/story_collection.py
+drwxrwxr-x   0 colm      (1000) colm      (1000)        0 2018-01-31 19:29:43.000000 hitchstory-0.9.1/
+-rw-rw-r--   0 colm      (1000) colm      (1000)     1851 2018-01-04 19:13:36.000000 hitchstory-0.9.1/setup.py
+drwxrwxr-x   0 colm      (1000) colm      (1000)        0 2018-01-31 19:29:43.000000 hitchstory-0.9.1/hitchstory.egg-info/
+-rw-rw-r--   0 colm      (1000) colm      (1000)        1 2018-01-31 19:29:43.000000 hitchstory-0.9.1/hitchstory.egg-info/dependency_links.txt
+-rw-rw-r--   0 colm      (1000) colm      (1000)      101 2018-01-31 19:29:43.000000 hitchstory-0.9.1/hitchstory.egg-info/requires.txt
+-rw-rw-r--   0 colm      (1000) colm      (1000)        1 2017-12-15 08:13:14.000000 hitchstory-0.9.1/hitchstory.egg-info/not-zip-safe
+-rw-rw-r--   0 colm      (1000) colm      (1000)     4858 2018-01-31 19:29:43.000000 hitchstory-0.9.1/hitchstory.egg-info/PKG-INFO
+-rw-rw-r--   0 colm      (1000) colm      (1000)       11 2018-01-31 19:29:43.000000 hitchstory-0.9.1/hitchstory.egg-info/top_level.txt
+-rw-rw-r--   0 colm      (1000) colm      (1000)      683 2018-01-31 19:29:43.000000 hitchstory-0.9.1/hitchstory.egg-info/SOURCES.txt
+-rw-rw-r--   0 colm      (1000) colm      (1000)     4858 2018-01-31 19:29:43.000000 hitchstory-0.9.1/PKG-INFO
+-rw-rw-r--   0 colm      (1000) colm      (1000)        5 2018-01-31 19:29:35.000000 hitchstory-0.9.1/VERSION
+-rw-rw-r--   0 colm      (1000) colm      (1000)       59 2017-12-14 08:17:21.000000 hitchstory-0.9.1/MANIFEST.in
+-rw-rw-r--   0 colm      (1000) colm      (1000)     3007 2017-12-14 12:52:21.000000 hitchstory-0.9.1/README.rst
+-rw-rw-r--   0 colm      (1000) colm      (1000)       38 2018-01-31 19:29:43.000000 hitchstory-0.9.1/setup.cfg
+drwxrwxr-x   0 colm      (1000) colm      (1000)        0 2018-01-31 19:29:43.000000 hitchstory-0.9.1/hitchstory/
+-rw-rw-r--   0 colm      (1000) colm      (1000)     3228 2018-01-06 21:24:32.000000 hitchstory-0.9.1/hitchstory/story_step.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     1026 2017-12-14 08:17:21.000000 hitchstory-0.9.1/hitchstory/story_list.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     3138 2018-01-06 21:27:12.000000 hitchstory-0.9.1/hitchstory/step_method.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     4717 2018-01-07 15:15:28.000000 hitchstory-0.9.1/hitchstory/story_file.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     2207 2018-01-07 14:45:56.000000 hitchstory-0.9.1/hitchstory/arguments.py
+drwxrwxr-x   0 colm      (1000) colm      (1000)        0 2018-01-31 19:29:43.000000 hitchstory-0.9.1/hitchstory/templates/
+-rw-rw-r--   0 colm      (1000) colm      (1000)     1310 2017-12-14 08:17:21.000000 hitchstory-0.9.1/hitchstory/templates/multiple.jinja2
+-rw-rw-r--   0 colm      (1000) colm      (1000)     2702 2017-12-14 08:17:21.000000 hitchstory-0.9.1/hitchstory/templates/stacktrace_default.jinja2
+-rw-rw-r--   0 colm      (1000) colm      (1000)      250 2017-12-14 08:17:21.000000 hitchstory-0.9.1/hitchstory/templates/failure.jinja2
+-rw-rw-r--   0 colm      (1000) colm      (1000)      127 2017-12-19 16:19:52.000000 hitchstory-0.9.1/hitchstory/templates/success.jinja2
+-rw-rw-r--   0 colm      (1000) colm      (1000)     4226 2017-12-14 08:17:21.000000 hitchstory-0.9.1/hitchstory/exceptions.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     3488 2018-01-07 14:08:03.000000 hitchstory-0.9.1/hitchstory/result.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     1802 2018-01-07 14:45:16.000000 hitchstory-0.9.1/hitchstory/utils.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     8854 2018-01-31 18:59:07.000000 hitchstory-0.9.1/hitchstory/story.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     3356 2018-01-29 13:35:18.000000 hitchstory-0.9.1/hitchstory/engine.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)      482 2018-01-31 19:29:42.000000 hitchstory-0.9.1/hitchstory/__init__.py
+-rw-rw-r--   0 colm      (1000) colm      (1000)     8754 2018-01-04 21:51:03.000000 hitchstory-0.9.1/hitchstory/story_collection.py
```

### Comparing `hitchstory-0.9.0/setup.py` & `hitchstory-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory.egg-info/PKG-INFO` & `hitchstory-0.9.1/hitchstory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hitchstory
-Version: 0.9.0
+Version: 0.9.1
 Summary: Type-safe, YAML-based BDD, TDD & specification by example framework for python.
 Home-page: https://hitchtest.readthedocs.org/
 Author: Colm O'Connor
 Author-email: colm.oconnor.github@gmail.com
 License: AGPL
 Description-Content-Type: UNKNOWN
 Description: HitchStory
```

### Comparing `hitchstory-0.9.0/hitchstory.egg-info/SOURCES.txt` & `hitchstory-0.9.1/hitchstory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/PKG-INFO` & `hitchstory-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hitchstory
-Version: 0.9.0
+Version: 0.9.1
 Summary: Type-safe, YAML-based BDD, TDD & specification by example framework for python.
 Home-page: https://hitchtest.readthedocs.org/
 Author: Colm O'Connor
 Author-email: colm.oconnor.github@gmail.com
 License: AGPL
 Description-Content-Type: UNKNOWN
 Description: HitchStory
```

### Comparing `hitchstory-0.9.0/README.rst` & `hitchstory-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/story_step.py` & `hitchstory-0.9.1/hitchstory/story_step.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/story_list.py` & `hitchstory-0.9.1/hitchstory/story_list.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/step_method.py` & `hitchstory-0.9.1/hitchstory/step_method.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/story_file.py` & `hitchstory-0.9.1/hitchstory/story_file.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/arguments.py` & `hitchstory-0.9.1/hitchstory/arguments.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/templates/multiple.jinja2` & `hitchstory-0.9.1/hitchstory/templates/multiple.jinja2`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/templates/stacktrace_default.jinja2` & `hitchstory-0.9.1/hitchstory/templates/stacktrace_default.jinja2`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/exceptions.py` & `hitchstory-0.9.1/hitchstory/exceptions.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/result.py` & `hitchstory-0.9.1/hitchstory/result.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/utils.py` & `hitchstory-0.9.1/hitchstory/utils.py`

 * *Files identical despite different names*

### Comparing `hitchstory-0.9.0/hitchstory/story.py` & `hitchstory-0.9.1/hitchstory/story.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,26 @@
         for name, precondition in precondition_dict.items():
             if utils.is_parameter(precondition):
                 precondition_dict[name] = \
                     self.params[utils.parameter_name(precondition)]
             else:
                 precondition_dict[name] = precondition
         self._precondition_dict = precondition_dict
+
+        from strictyaml.compound import MapValidator, SeqValidator
+
+        for name, definition in self.engine.given_definition.given_properties.items():
+            if name not in self._precondition_dict.keys():
+                if isinstance(definition.schema, MapValidator):
+                    self._precondition_dict[name] = {}
+                elif isinstance(definition.schema, SeqValidator):
+                    self._precondition_dict[name] = []
+                else:
+                    self._precondition_dict[name] = None
+
         number_of_parent_steps = len(self._parent_steps)
         self._steps = [
             StoryStep(
                 self, parsed_step, index, index - number_of_parent_steps, self.params
             ) for index, parsed_step in enumerate(self._yaml_steps)
         ]
 
@@ -105,15 +117,15 @@
     def name(self):
         return self._name if not self.variation\
             else "{0}/{1}".format(self._variation_of, self._name)
 
     @property
     def slug(self):
         if self._slug is None:
-            self._slug = slugify(self.name)
+            self._slug = slugify(self.name)  # relatively slow method
         return self._slug
 
     @property
     def parent(self):
         return self._parent
 
     @property
```

### Comparing `hitchstory-0.9.0/hitchstory/engine.py` & `hitchstory-0.9.1/hitchstory/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 class GivenProperty(object):
     def __init__(self, schema=None):
         self.schema = Any() if schema is None else schema
 
 
 class GivenDefinition(object):
     def __init__(self, **given_properties):
+        self.given_properties = given_properties
         mapping = {}
         for name, given_property in given_properties.items():
             assert isinstance(given_property, GivenProperty), \
               "{0} must be GivenProperty.".format(name)
             mapping[Optional(name)] = utils.YAML_Param | given_property.schema
         self.preconditions = Map(mapping, key_validator=utils.UnderscoredSlug())
```

### Comparing `hitchstory-0.9.0/hitchstory/story_collection.py` & `hitchstory-0.9.1/hitchstory/story_collection.py`

 * *Files identical despite different names*

