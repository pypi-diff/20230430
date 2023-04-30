# Comparing `tmp/sball-1.0.3.tar.gz` & `tmp/sball-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sball-1.0.3.tar", last modified: Wed Apr 19 19:13:25 2023, max compression
+gzip compressed data, was "sball-1.0.4.tar", last modified: Sun Apr 30 16:41:34 2023, max compression
```

## Comparing `sball-1.0.3.tar` & `sball-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 19:13:25.121790 sball-1.0.3/
--rw-rw-rw-   0        0        0     1090 2023-04-15 03:14:00.000000 sball-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     4267 2023-04-19 19:13:25.120787 sball-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3769 2023-04-15 03:09:19.000000 sball-1.0.3/README.md
--rw-rw-rw-   0        0        0      632 2023-04-19 19:12:20.000000 sball-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 19:13:25.122784 sball-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 19:13:25.077786 sball-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 19:13:25.105783 sball-1.0.3/src/sball/
--rw-rw-rw-   0        0        0       38 2023-04-19 19:12:13.000000 sball-1.0.3/src/sball/__init__.py
--rw-rw-rw-   0        0        0      302 2023-04-15 02:27:19.000000 sball-1.0.3/src/sball/__main__.py
--rw-rw-rw-   0        0        0     5027 2023-04-19 19:12:06.000000 sball-1.0.3/src/sball/sball.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:13:25.117784 sball-1.0.3/src/sball.egg-info/
--rw-rw-rw-   0        0        0     4267 2023-04-19 19:13:25.000000 sball-1.0.3/src/sball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-19 19:13:25.000000 sball-1.0.3/src/sball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 19:13:25.000000 sball-1.0.3/src/sball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-19 19:13:25.000000 sball-1.0.3/src/sball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 19:13:25.000000 sball-1.0.3/src/sball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 16:41:34.522629 sball-1.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 03:14:00.000000 sball-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4267 2023-04-30 16:41:34.521628 sball-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3769 2023-04-15 03:09:19.000000 sball-1.0.4/README.md
+-rw-rw-rw-   0        0        0      632 2023-04-30 16:40:27.000000 sball-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:41:34.522629 sball-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 16:41:34.482301 sball-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 16:41:34.508629 sball-1.0.4/src/sball/
+-rw-rw-rw-   0        0        0       38 2023-04-30 16:40:37.000000 sball-1.0.4/src/sball/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-04-15 02:27:19.000000 sball-1.0.4/src/sball/__main__.py
+-rw-rw-rw-   0        0        0     5072 2023-04-30 16:40:53.000000 sball-1.0.4/src/sball/sball.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:41:34.519630 sball-1.0.4/src/sball.egg-info/
+-rw-rw-rw-   0        0        0     4267 2023-04-30 16:41:34.000000 sball-1.0.4/src/sball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-30 16:41:34.000000 sball-1.0.4/src/sball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 16:41:34.000000 sball-1.0.4/src/sball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-30 16:41:34.000000 sball-1.0.4/src/sball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 16:41:34.000000 sball-1.0.4/src/sball.egg-info/top_level.txt
```

### Comparing `sball-1.0.3/LICENSE` & `sball-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sball-1.0.3/PKG-INFO` & `sball-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sball
-Version: 1.0.3
+Version: 1.0.4
 Summary: Submit scripts in job arrays using Yale's dSQ.
 Author-email: Michael Wilson <michael.a.wilson@yale.edu>
 Project-URL: Homepage, https://github.com/mawilson1234/sball
 Keywords: slurm,job array,sbatch,dSQ,dsq
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sball-1.0.3/README.md` & `sball-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sball-1.0.3/pyproject.toml` & `sball-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires=['setuptools', 'wheel']
 build-backend='setuptools.build_meta'
 
 [project]
 name='sball'
-version='1.0.3'
+version='1.0.4'
 description="Submit scripts in job arrays using Yale's dSQ."
 readme='README.md'
 authors=[{name="Michael Wilson", email='michael.a.wilson@yale.edu'}]
 classifiers=[
 	'Development Status :: 4 - Beta',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
```

### Comparing `sball-1.0.3/src/sball/sball.py` & `sball-1.0.4/src/sball/sball.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 		
 		with open(joblist_file, 'wt') as out_file:
 			out_file.write(joblist)
 			
 		k_options = ['--' + k for k, _ in options]
 		v_options = [v for _, v in options]
 		options = list(zip(k_options, v_options))
+		options = [v for t in options for v in t]
 		
 		x = subprocess.Popen([
 			'dsq', 
 			'--job-file', joblist_file, 
 			'--status-dir', log_dir + os.path.sep,
 			'--job-name', name + formatter,
 			'--output', os.path.join(log_dir, name + formatter + '-%A_%a.txt'),
```

### Comparing `sball-1.0.3/src/sball.egg-info/PKG-INFO` & `sball-1.0.4/src/sball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sball
-Version: 1.0.3
+Version: 1.0.4
 Summary: Submit scripts in job arrays using Yale's dSQ.
 Author-email: Michael Wilson <michael.a.wilson@yale.edu>
 Project-URL: Homepage, https://github.com/mawilson1234/sball
 Keywords: slurm,job array,sbatch,dSQ,dsq
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

