# Comparing `tmp/PyScaffolder-1.5.2.tar.gz` & `tmp/PyScaffolder-1.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyScaffolder-1.5.2.tar", last modified: Sun Aug  8 21:14:00 2021, max compression
+gzip compressed data, was "PyScaffolder-1.5.2.post1.tar", last modified: Sun Apr 30 11:19:36 2023, max compression
```

## Comparing `PyScaffolder-1.5.2.tar` & `PyScaffolder-1.5.2.post1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 21:14:00.702906 PyScaffolder-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-08-08 21:13:42.000000 PyScaffolder-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-08-08 21:14:00.702906 PyScaffolder-1.5.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 21:14:00.702906 PyScaffolder-1.5.2/PyScaffolder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-08-08 21:14:00.000000 PyScaffolder-1.5.2/PyScaffolder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-08-08 21:14:00.000000 PyScaffolder-1.5.2/PyScaffolder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-08 21:14:00.000000 PyScaffolder-1.5.2/PyScaffolder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-08 21:14:00.000000 PyScaffolder-1.5.2/PyScaffolder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-08-08 21:14:00.000000 PyScaffolder-1.5.2/PyScaffolder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2021-08-08 21:13:42.000000 PyScaffolder-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-08-08 21:13:42.000000 PyScaffolder-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-08-08 21:14:00.702906 PyScaffolder-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2021-08-08 21:13:42.000000 PyScaffolder-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:19:36.917895 PyScaffolder-1.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 11:19:19.000000 PyScaffolder-1.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-30 11:19:36.917895 PyScaffolder-1.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-30 11:19:19.000000 PyScaffolder-1.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-30 11:19:19.000000 PyScaffolder-1.5.2.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-30 11:19:36.917895 PyScaffolder-1.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-30 11:19:19.000000 PyScaffolder-1.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:19:36.913895 PyScaffolder-1.5.2.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:19:36.917895 PyScaffolder-1.5.2.post1/src/PyScaffolder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-30 11:19:36.000000 PyScaffolder-1.5.2.post1/src/PyScaffolder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-30 11:19:36.000000 PyScaffolder-1.5.2.post1/src/PyScaffolder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:19:36.000000 PyScaffolder-1.5.2.post1/src/PyScaffolder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:19:36.000000 PyScaffolder-1.5.2.post1/src/PyScaffolder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 11:19:36.000000 PyScaffolder-1.5.2.post1/src/PyScaffolder.egg-info/top_level.txt
```

### Comparing `PyScaffolder-1.5.2/LICENSE` & `PyScaffolder-1.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyScaffolder-1.5.2/README.md` & `PyScaffolder-1.5.2.post1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Scaffolder 
-![Build Status](https://github.com/nodtem66/Scaffolder/workflows/Build/badge.svg) [![Build Status](https://dev.azure.com/n66/PublicCI/_apis/build/status/nodtem66.Scaffolder%20(Anaconda)?branchName=master)](https://dev.azure.com/n66/PublicCI/_build/latest?definitionId=6&branchName=master)
+![Build Status](https://github.com/nodtem66/Scaffolder/actions/workflows/binary.yml/badge.svg) [![Build Status](https://dev.azure.com/n66/PublicCI/_apis/build/status%2Fnodtem66.Scaffolder%20(Anaconda%20release)?branchName=master)](https://dev.azure.com/n66/PublicCI/_build/latest?definitionId=8&branchName=master)
 
-[![Anaconda](https://anaconda.org/nodtem66/scaffolder/badges/version.svg)](https://anaconda.org/nodtem66/scaffolder) ![Last update](https://anaconda.org/nodtem66/scaffolder/badges/latest_release_date.svg) ![Platform](https://anaconda.org/nodtem66/scaffolder/badges/platforms.svg) ![Install](https://anaconda.org/nodtem66/scaffolder/badges/installer/conda.svg)
+[![Anaconda](https://anaconda.org/nodtem66/scaffolder/badges/version.svg)](https://anaconda.org/nodtem66/scaffolder) ![Last update](https://anaconda.org/nodtem66/scaffolder/badges/latest_release_date.svg) ![Platform](https://anaconda.org/nodtem66/scaffolder/badges/platforms.svg)
 
 ![Scaffolder Logo](https://github.com/nodtem66/Scaffolder/raw/master/docs/images/scaffolder_logo.jpg)
 
-Generate scaffold from STL/PLY/OFF/OBJ file with implicit function (e.g., Schwarz P/ Gyroid).
+Transform a 3D model from STL/PLY/OFF/OBJ to a porous model with implicit function (e.g., Schwarz P/ Gyroid).
 
 [Documentation](https://nodtem66.github.io/Scaffolder) 
 
 ## Binary installation
 * Download from [Github Releases page](https://github.com/nodtem66/Scaffolder/releases) or
 * Install from Anaconda
 ```bash
@@ -37,40 +37,47 @@
 
 
 - **The examples of generated porous scaffold**
 
 ![Examples porous scaffold](https://github.com/nodtem66/Scaffolder/raw/master/docs/images/examples.jpg)
 
 ## Dependencies
-- [libigl](https://libigl.github.io/)
-- [vcglib](https://github.com/cnr-isti-vclab/vcglib)
-- [sol2](https://github.com/ThePhD/sol2)
-- [tbb](https://github.com/oneapi-src/oneTBB)
+- [libigl](https://libigl.github.io/) - The computational geometry library
+- [vcglib](https://github.com/cnr-isti-vclab/vcglib) - The mesh utility library
+- [sol2](https://github.com/ThePhD/sol2) - Lua script integration
+- [tbb](https://github.com/oneapi-src/oneTBB) - Threading library
 
 ## How it works
 - Read STL file and finding the boundary box
 - Generate the grid and calculate the winding number with STL mesh
 - Use winding number to determine the condition for [implicit isosurface function](https://wewanttolearn.wordpress.com/2019/02/03/triply-periodic-minimal-surfaces/)
 - Generate the isosurface field in the same-size grid
 - Perform [Dual marching cube](https://github.com/dominikwodniok/dualmc) to construct the manifold
 - Clean up the duplicated vertices or faces, and abandon the group of connected faces having the diameter below the setting
 - Export to the target 3D format
 
-## Coff and Thickness study
-[Angular frequency and iso-level](https://colab.research.google.com/github/nodtem66/Scaffolder/blob/master/data/data_visualization.ipynb)
+## FAQ
+
+### How can I find the dataset from a study of coffient and isolevel?
+The raw dataset is available at [Mendeley Data](https://data.mendeley.com/datasets/sbxr7xxvnd/2).
+The program that used to generate that data was released at [Github repository](https://github.com/nodtem66/Scaffolder). You can also find the interactive visualization at [Google Colab](https://colab.research.google.com/github/nodtem66/Scaffolder/blob/master/data/data_visualization.ipynb)
+
+### Where is the implicit functions were defined in the C++ sourcecode?
+https://github.com/nodtem66/Scaffolder/blob/master/include/implicit_function.h
+
+### Can you suggest alternative softwares like this program?
+- Rhino (Grasshopper)
+- nTopology
+- Hyperganic
 
 ## References
-- [libigl](https://github.com/libigl/libigl)
-- [vcglib](https://github.com/cnr-isti-vclab/vcglib)
-- [sol2](https://github.com/ThePhD/sol2)
-- [tbb](https://github.com/oneapi-src/oneTBB) 
-- [dualmc](https://github.com/dominikwodniok/dualmc)
-- [cxxopts](https://github.com/jarro2783/cxxopts)
-- [ProgressBar](https://github.com/prakhar1989/progress-cpp)
 - [Minimal surface Blog](https://minimalsurfaces.blog/)
+- Dual marching cube - [dualmc](https://github.com/dominikwodniok/dualmc)
+- Command line parser - [cxxopts](https://github.com/jarro2783/cxxopts)
+- Progress bar - [ProgressBar](https://github.com/prakhar1989/progress-cpp)
 
 ## Citation
 [Computational method and program for generating a porous scaffold based on implicit surfaces](https://doi.org/10.1016/j.cmpb.2021.106088)
 ```bibtex
 @article{IAMSAMANG2021106088,
 title = {Computational method and program for generating a porous scaffold based on implicit surfaces},
 journal = {Computer Methods and Programs in Biomedicine},
```

### Comparing `PyScaffolder-1.5.2/setup.py` & `PyScaffolder-1.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,17 +104,11 @@
             ["cmake", "--build", "."] + build_args, cwd=self.build_temp
         )
 
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
-    name="PyScaffolder",
-    version="1.5.2",
-    author="Jirawat Iamsamang",
-    author_email="nodtem66@gmail.com",
-    description="Python wrapper for scaffolder program",
-    long_description="https://github.com/nodtem66/Scaffolder",
     ext_modules=[CMakeExtension("PyScaffolder")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
 )
```

