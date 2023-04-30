# Comparing `tmp/dnacurve-2022.10.4.tar.gz` & `tmp/dnacurve-2023.4.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnacurve-2022.10.4.tar", last modified: Tue Oct  4 19:19:31 2022, max compression
+gzip compressed data, was "dnacurve-2023.4.30.tar", last modified: Sun Apr 30 06:19:05 2023, max compression
```

## Comparing `dnacurve-2022.10.4.tar` & `dnacurve-2023.4.30.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-10-04 19:19:31.728738 dnacurve-2022.10.4/
--rw-rw-rw-   0        0        0     1559 2022-10-04 19:19:29.000000 dnacurve-2022.10.4/LICENSE
--rw-rw-rw-   0        0        0      130 2018-08-15 23:01:21.000000 dnacurve-2022.10.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5145 2022-10-04 19:19:31.727743 dnacurve-2022.10.4/PKG-INFO
--rw-rw-rw-   0        0        0     4221 2022-10-04 19:19:29.000000 dnacurve-2022.10.4/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-04 19:19:31.720739 dnacurve-2022.10.4/dnacurve/
--rw-rw-rw-   0        0        0      104 2022-10-03 02:34:01.000000 dnacurve-2022.10.4/dnacurve/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:14:51.000000 dnacurve-2022.10.4/dnacurve/__main__.py
--rw-rw-rw-   0        0        0    54734 2022-10-04 19:07:26.000000 dnacurve-2022.10.4/dnacurve/dnacurve.py
--rw-rw-rw-   0        0        0    15980 2022-10-04 16:38:21.000000 dnacurve-2022.10.4/dnacurve/web.py
-drwxrwxrwx   0        0        0        0 2022-10-04 19:19:31.726739 dnacurve-2022.10.4/dnacurve.egg-info/
--rw-rw-rw-   0        0        0     5145 2022-10-04 19:19:30.000000 dnacurve-2022.10.4/dnacurve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2022-10-04 19:19:31.000000 dnacurve-2022.10.4/dnacurve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-04 19:19:30.000000 dnacurve-2022.10.4/dnacurve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2022-10-04 19:19:30.000000 dnacurve-2022.10.4/dnacurve.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2022-10-04 19:19:30.000000 dnacurve-2022.10.4/dnacurve.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-04 19:19:30.000000 dnacurve-2022.10.4/dnacurve.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-04 19:19:31.728738 dnacurve-2022.10.4/setup.cfg
--rw-rw-rw-   0        0        0     2463 2022-10-04 17:11:15.000000 dnacurve-2022.10.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:19:05.978207 dnacurve-2023.4.30/
+-rw-rw-rw-   0        0        0     1559 2023-04-30 06:19:00.000000 dnacurve-2023.4.30/LICENSE
+-rw-rw-rw-   0        0        0      251 2022-12-09 00:09:42.000000 dnacurve-2023.4.30/MANIFEST.in
+-rw-rw-rw-   0        0        0     5259 2023-04-30 06:19:05.977207 dnacurve-2023.4.30/PKG-INFO
+-rw-rw-rw-   0        0        0     4386 2023-04-30 06:19:00.000000 dnacurve-2023.4.30/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 06:19:05.963725 dnacurve-2023.4.30/dnacurve/
+-rw-rw-rw-   0        0        0      104 2022-10-03 02:34:01.000000 dnacurve-2023.4.30/dnacurve/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:14:51.000000 dnacurve-2023.4.30/dnacurve/__main__.py
+-rw-rw-rw-   0        0        0    55284 2023-04-30 06:16:18.000000 dnacurve-2023.4.30/dnacurve/dnacurve.py
+-rw-rw-rw-   0        0        0    15953 2023-01-04 16:38:55.000000 dnacurve-2023.4.30/dnacurve/web.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:19:05.975009 dnacurve-2023.4.30/dnacurve.egg-info/
+-rw-rw-rw-   0        0        0     5259 2023-04-30 06:19:04.000000 dnacurve-2023.4.30/dnacurve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-30 06:19:05.000000 dnacurve-2023.4.30/dnacurve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 06:19:04.000000 dnacurve-2023.4.30/dnacurve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-04-30 06:19:04.000000 dnacurve-2023.4.30/dnacurve.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-04-30 06:19:04.000000 dnacurve-2023.4.30/dnacurve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 06:19:04.000000 dnacurve-2023.4.30/dnacurve.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 06:19:05.978207 dnacurve-2023.4.30/setup.cfg
+-rw-rw-rw-   0        0        0     2405 2023-04-30 06:00:08.000000 dnacurve-2023.4.30/setup.py
```

### Comparing `dnacurve-2022.10.4/LICENSE` & `dnacurve-2023.4.30/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 1993-2022, Christoph Gohlke
+Copyright (c) 1993-2023, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `dnacurve-2022.10.4/PKG-INFO` & `dnacurve-2023.4.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 Metadata-Version: 2.1
 Name: dnacurve
-Version: 2022.10.4
-Summary: DNA Curvature Analysis
+Version: 2023.4.30
+Summary: DNA curvature analysis
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/dnacurve/issues
 Project-URL: Source Code, https://github.com/cgohlke/dnacurve
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Provides-Extra: all
 License-File: LICENSE
 
-DNA Curvature Analysis
+DNA curvature analysis
 ======================
 
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.10.4
-:DOI: 10.5281/zenodo.7135499
+:Version: 2023.4.30
+:DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
-Python Package Index::
+`Python Package Index <https://pypi.org/project/dnacurve/>`_::
 
     python -m pip install -U dnacurve[all]
 
 Print the console script usage::
 
     python -m dnacurve --help
 
@@ -56,25 +55,30 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/dnacurve>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `Numpy 1.22.4 <https://pypi.org/project/numpy/>`_
-- `Matplotlib 3.5.3 <https://pypi.org/project/matplotlib/>`_
-- `Flask 2.2.2 <https://pypi.org/project/Flask/>`_ (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `Numpy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+- `Flask <https://pypi.org/project/Flask/>`_ 2.3.1 (optional)
 
 Revisions
 ---------
 
+2023.4.30
+
+- Improve type hints.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.10.4
 
 - Rename dnacurve_web.py to web.py (breaking).
 - Deprecate save functions (use write functions).
 - Add options to specify URL of web application and not opening web browser.
 - Run web application using Flask if installed.
 - Convert to Google style docstrings.
```

### Comparing `dnacurve-2022.10.4/README.rst` & `dnacurve-2023.4.30/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-DNA Curvature Analysis
+DNA curvature analysis
 ======================
 
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.10.4
-:DOI: 10.5281/zenodo.7135499
+:Version: 2023.4.30
+:DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
-Python Package Index::
+`Python Package Index <https://pypi.org/project/dnacurve/>`_::
 
     python -m pip install -U dnacurve[all]
 
 Print the console script usage::
 
     python -m dnacurve --help
 
@@ -31,25 +31,30 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/dnacurve>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `Numpy 1.22.4 <https://pypi.org/project/numpy/>`_
-- `Matplotlib 3.5.3 <https://pypi.org/project/matplotlib/>`_
-- `Flask 2.2.2 <https://pypi.org/project/Flask/>`_ (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `Numpy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+- `Flask <https://pypi.org/project/Flask/>`_ 2.3.1 (optional)
 
 Revisions
 ---------
 
+2023.4.30
+
+- Improve type hints.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.10.4
 
 - Rename dnacurve_web.py to web.py (breaking).
 - Deprecate save functions (use write functions).
 - Add options to specify URL of web application and not opening web browser.
 - Run web application using Flask if installed.
 - Convert to Google style docstrings.
```

### Comparing `dnacurve-2022.10.4/dnacurve/dnacurve.py` & `dnacurve-2023.4.30/dnacurve/dnacurve.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # dnacurve.py
 
-# Copyright (c) 1993-2022, Christoph Gohlke
+# Copyright (c) 1993-2023, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -25,31 +25,31 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-"""DNA Curvature Analysis.
+"""DNA curvature analysis.
 
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.10.4
-:DOI: 10.5281/zenodo.7135499
+:Version: 2023.4.30
+:DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
-Python Package Index::
+`Python Package Index <https://pypi.org/project/dnacurve/>`_::
 
     python -m pip install -U dnacurve[all]
 
 Print the console script usage::
 
     python -m dnacurve --help
 
@@ -61,25 +61,30 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/dnacurve>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `Numpy 1.22.4 <https://pypi.org/project/numpy/>`_
-- `Matplotlib 3.5.3 <https://pypi.org/project/matplotlib/>`_
-- `Flask 2.2.2 <https://pypi.org/project/Flask/>`_ (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `Numpy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+- `Flask <https://pypi.org/project/Flask/>`_ 2.3.1 (optional)
 
 Revisions
 ---------
 
+2023.4.30
+
+- Improve type hints.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.10.4
 
 - Rename dnacurve_web.py to web.py (breaking).
 - Deprecate save functions (use write functions).
 - Add options to specify URL of web application and not opening web browser.
 - Run web application using Flask if installed.
 - Convert to Google style docstrings.
@@ -183,15 +188,15 @@
 >>> result.write_pdb('_test.pdb')
 >>> result.plot('_test.png', dpi=120)
 
 """
 
 from __future__ import annotations
 
-__version__ = '2022.10.4'
+__version__ = '2023.4.30'
 
 __all__ = [
     'CurvedDNA',
     'Model',
     'Sequence',
     'MAXLEN',
     'MODELS',
@@ -214,15 +219,17 @@
 import warnings
 
 import numpy
 
 from typing import TYPE_CHECKING, overload
 
 if TYPE_CHECKING:
-    from typing import Any, BinaryIO, Iterable, Iterator
+    from typing import Any, BinaryIO
+    from collections.abc import Iterable, Iterator
+    from numpy.typing import NDArray
 
 MAXLEN: int = 510
 """Maximum length of sequences to analyze."""
 
 MODELS: list[str] = []  # updated later
 """Predefined models."""
 
@@ -282,50 +289,50 @@
     """Cylindrical coordinates of 5' phosphate:
 
     0. distance from axis
     1. angle to roll axis
     2. distance from basepair plane
     """
 
-    coordinates: numpy.ndarray
+    coordinates: NDArray[Any]
     """Homogeneous coordinates at each nucleotide of:
 
     0. helix axis
     1. phosphate of 5'-3' strand
     2. phosphate of antiparallel strand
     3. basepair normal vector
     4. smoothed basepair normal vector
     """
 
-    curvature: numpy.ndarray
+    curvature: NDArray[Any]
     """Values at each nucleotide relative to curvature in nucleosome:
 
     0. curvature
     1. local bend angle
     2. curvature angle
     """
 
-    scales: numpy.ndarray
+    scales: NDArray[Any]
     """Scaling factors used to normalize curvature array."""
 
     windows: tuple[int, int, int]
     """Window sizes for calculating curvature, local bend angle, and
     curvature angle.
     """
 
     date: datetime.datetime
     """Date and time of analysis."""
 
     _limits: tuple[float, float, float]
 
     def __init__(
         self,
-        sequence: Sequence | os.PathLike | str,
+        sequence: Sequence | os.PathLike[Any] | str,
         /,
-        model: Model | os.PathLike | str = 'trifonov',
+        model: Model | os.PathLike[Any] | str = 'trifonov',
         name: str = 'Untitled',
         curvature_window: int = 10,
         bend_window: int = 2,
         curve_window: int = 15,
         maxlen: int = MAXLEN,
     ) -> None:
         if isinstance(model, Model):
@@ -384,38 +391,38 @@
             for i in 0, 1, 2:
                 xyz[4, :, i] = numpy.convolve(kernel, xyz[3, :, i], 'same')
             for i in range(5, len(self.sequence) - 5):
                 xyz[4, i, :] /= norm(xyz[4, i, :])
 
     def _reorient(self) -> None:
         """Reorient coordinates."""
-        xyz: numpy.ndarray = self.coordinates[0, :, 0:3]  # helix axis
+        xyz: NDArray[Any] = self.coordinates[0, :, 0:3]  # helix axis
         xyz = xyz - xyz[-1]
         # assert start point is at origin
         assert numpy.allclose(xyz[-1], (0, 0, 0))
         # normalized end to end vector
-        e: numpy.ndarray = +xyz[0]
+        e: NDArray[Any] = +xyz[0]
         e_len = norm(e)
         e /= e_len
         # point i of maximum distance to end to end line
-        t: numpy.ndarray = numpy.cross(e, xyz)
+        t: NDArray[Any] = numpy.cross(e, xyz)
         t = numpy.sum(t * t, axis=1)
         i = numpy.argmax(t)
         x = math.sqrt(t[i])
         # distance of endpoint to xyz[i]
         w = norm(xyz[i])
         # distance of endpoint to point on end to end line nearest to xyz[i]
         u = math.sqrt(w * w - x * x)
         # find transformation matrix
-        v0: numpy.ndarray = xyz[[0, i, -1]]  # type: ignore
-        v1: numpy.ndarray = numpy.array(
+        v0: NDArray[Any] = xyz[[0, i, -1]]  # type: ignore
+        v1: NDArray[Any] = numpy.array(
             ((0, 0, 0), (e_len - u, 0, x), (e_len, 0, 0))
         )
         M = superimpose_matrix(v0, v1)
-        self.coordinates: numpy.ndarray = numpy.dot(self.coordinates, M.T)
+        self.coordinates: NDArray[Any] = numpy.dot(self.coordinates, M.T)
 
     def _center(self) -> None:
         """Center atomic coordinates at origin."""
         xyz = self.coordinates[0:3, :, 0:3]  # helix axis and P atoms
         low = numpy.min(numpy.min(xyz, axis=1), axis=0)
         upp = numpy.max(numpy.max(xyz, axis=1), axis=0)
         lim = (upp - low) / 2.0
@@ -474,41 +481,41 @@
         self.curvature = numpy.nan_to_num(self.curvature)
 
         # normalize relative to curvature in nucleosome
         self.scales[0] = 0.0234
         self.scales[1:] = 0.0234 * 2 * self.windows[2] * self.model.rise
         self.curvature /= self.scales
 
-    def write_csv(self, path: os.PathLike | str, /) -> None:
+    def write_csv(self, path: os.PathLike[Any] | str, /) -> None:
         """Write coordinates and curvature values to CSV file.
 
         Parameters:
             path: Name of CSV file to write.
 
         """
         with open(path, 'w', newline='\r\n') as fh:
             fh.write(self.csv())
 
-    def save_csv(self, path):
+    def save_csv(self, path: os.PathLike[Any] | str) -> None:
         # deprecated
-        return self.write_csv(path)
+        self.write_csv(path)
 
-    def write_pdb(self, path: os.PathLike | str, /) -> None:
+    def write_pdb(self, path: os.PathLike[Any] | str, /) -> None:
         """Write atomic coordinates to PDB file.
 
         Parameters:
             path: Name of PDB file to write.
 
         """
         with open(path, 'w', newline='\n') as fh:
             fh.write(self.pdb())
 
-    def save_pdb(self, path):
+    def save_pdb(self, path: os.PathLike[Any] | str) -> None:
         # deprecated
-        return self.write_pdb(path)
+        self.write_pdb(path)
 
     def csv(self) -> str:
         """Return coordinates and curvature values in CSV format."""
         seq = self.sequence
         cur = self.curvature
         xyz = self.coordinates
         csv = [
@@ -588,20 +595,20 @@
             serial += 1
         pdb_append(f'TER   {serial:5}       D{seq[i]:<1s} B{serial - 1:4}')
         pdb_append('END')
         return ''.join(pdb)
 
     def plot(
         self,
-        arg: str | os.PathLike | BinaryIO | bool = True,
+        arg: str | os.PathLike[Any] | BinaryIO | bool = True,
         /,
         dpi: int = 96,
         figsize: tuple[float, float] = (6.0, 7.5),
         imageformat: str | None = None,
-    ) -> None:
+    ) -> Any:
         """Plot results using matplotlib.
 
         Parameters:
             arg:
                 Specifies how to plot:
 
                 - **False**: do not plot.
@@ -939,22 +946,22 @@
 
     roll: dict[str, float]
     """Rotation angle in deg about the Y axis for all oligonucleotides."""
 
     tilt: dict[str, float]
     """Rotation angle in deg about the X axis for all oligonucleotides."""
 
-    matrices: dict[str | None, numpy.ndarray]
+    matrices: dict[str | None, NDArray[Any]]
     """Homogeneous transformation matrices for all oligonucleotides."""
 
     def __init__(
         self,
-        model: Model | dict[str, Any] | os.PathLike | str | None = None,
+        model: Model | dict[str, Any] | os.PathLike[Any] | str | None = None,
         /,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         modeldict: dict[str, Any]
         if model:
             # TODO: type importfunction
             for importfunction in (
                 self._fromname,
                 self._fromdict,
@@ -996,15 +1003,15 @@
                 self.rise,
                 self.twist[oligo],
                 self.roll[oligo],
                 self.tilt[oligo],
             ).T
         self.matrices[None] = dinucleotide_matrix(self.rise, 34.3, 0.0, 0.0).T
 
-    def _fromfile(self, path: os.PathLike | str, /) -> dict[str, Any]:
+    def _fromfile(self, path: os.PathLike[Any] | str, /) -> dict[str, Any]:
         """Return model parameters as dict from file."""
         d: dict[str, Any] = {}
         with open(path) as fh:
             d['name'] = fh.readline().rstrip()
             d['rise'] = float(fh.readline().split()[-1])
 
             def readtuple(
@@ -1023,34 +1030,34 @@
             d['twist'], line = readtuple(float, line)
             d['roll'], line = readtuple(float, line)
             d['tilt'], line = readtuple(float, line)
         return d
 
     def _fromname(self, name: str, /) -> dict[str, Any]:
         """Return predefined model parameters as dict."""
-        return getattr(Model, name.upper())
+        return getattr(Model, name.upper())  # type: ignore
 
     def _fromclass(self, aclass: Model, /) -> dict[str, Any]:
         """Return model parameters as dict from class."""
         return {a: getattr(aclass, a) for a in Model.STRAIGHT}
 
     def _fromdict(self, adict: dict[str, Any], /) -> dict[str, Any]:
         """Return model parameters as dict from dictionary."""
         for attr in Model.STRAIGHT:
             adict[attr]  # noqa: validation
         return adict
 
-    def write(self, path: os.PathLike | str, /) -> None:
+    def write(self, path: os.PathLike[Any] | str, /) -> None:
         """Write model to file."""
         with open(path, 'w', newline='\n') as fh:
             fh.write(str(self))
 
-    def save(self, path):
+    def save(self, path: os.PathLike[Any] | str, /) -> None:
         # deprecated
-        return self.write(path)
+        self.write(path)
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__} {self.name!r}>'
 
     def __str__(self) -> str:
         if self.order % 2:
             oligos = list(oligonucleotides(self.order))
@@ -1128,15 +1135,15 @@
     fname: str | None
     """File name."""
 
     _sequence: str
 
     def __init__(
         self,
-        arg: os.PathLike | str,
+        arg: os.PathLike[Any] | str,
         /,
         name: str = 'Untitled',
         comment: str = '',
         maxlen: int = 1024 * 1024,
     ) -> None:
         self.name = name if name else 'Untitled'
         self.comment = comment
@@ -1161,38 +1168,40 @@
         # limit length of sequence
         if maxlen and len(self._sequence) > maxlen:
             warnings.warn(f'sequence truncated to {maxlen} nucleotides')
             self._sequence = self._sequence[:maxlen]
         if not self._sequence:
             raise ValueError('not a valid sequence')
 
-    def _fromfile(self, path: os.PathLike | str, /, maxsize: int = -1) -> None:
+    def _fromfile(
+        self, path: os.PathLike[Any] | str, /, maxsize: int = -1
+    ) -> None:
         """Read name, comment and sequence from file."""
         with open(path) as fh:
             firstline = fh.readline().rstrip()
             if firstline.startswith('>'):  # FASTA format
                 self.name, self.comment = (firstline[1:] + ' ').split(' ', 1)
             elif firstline:
                 self.name = firstline
                 self.comment = fh.readline()
             self._sequence = fh.read(maxsize)
 
-    def write(self, path: os.PathLike | str, /) -> None:
+    def write(self, path: os.PathLike[Any] | str, /) -> None:
         """Write sequence to file.
 
         Parameters:
             path: Name of file to write.
 
         """
         with open(path, 'w', newline='\n') as fh:
             fh.write(f'{self.name}\n{self.comment}\n{self.format()}')
 
-    def save(self, path):
+    def save(self, path: os.PathLike[Any] | str, /) -> None:
         # deprecated
-        return self.write(path)
+        self.write(path)
 
     @property
     def string(self) -> str:
         """Sequence string containing only ATCG."""
         return self._sequence
 
     def format(self, block: int = 10, line: int = 6) -> str:
@@ -1227,15 +1236,15 @@
 
     def __repr__(self) -> str:
         return (
             f'<{self.__class__.__name__} {self.name!r} '
             f'length={len(self._sequence)!r}>'
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'{self.name}\n{self.comment}\n{self.format()}'
 
 
 def complementary(sequence: Sequence | str) -> str:
     """Return complementary DNA sequence.
 
     Parameters:
@@ -1384,15 +1393,15 @@
         yield sequence[i : i + size]
     for i in range(len(sequence) - size + border, len(sequence) - 1):
         yield None
 
 
 def dinucleotide_matrix(
     rise: float, twist: float, roll: float, tilt: float, /
-) -> numpy.ndarray:
+) -> NDArray[Any]:
     """Return transformation matrix to move from one nucleotide to next.
 
     Parameters:
         rise: Displacement along the Z axis.
         twist: Rotation angle in deg about the Z axis.
         roll: Rotation angle in deg about the Y axis.
         tilt: Rotation angle in deg about the X axis.
@@ -1424,17 +1433,15 @@
             (-sint, sinr * cost, cosr * cost, rise),
             (0.0, 0.0, 0.0, 1.0),
         ),
         dtype=numpy.float64,
     )
 
 
-def superimpose_matrix(
-    v0: numpy.ndarray, v1: numpy.ndarray, /
-) -> numpy.ndarray:
+def superimpose_matrix(v0: NDArray[Any], v1: NDArray[Any], /) -> NDArray[Any]:
     """Return matrix to transform given vector set to second vector set.
 
     Parameters:
         v0: Given vector set.
         v1: Target vector set.
 
     """
@@ -1455,15 +1462,15 @@
     T = numpy.identity(4, dtype=numpy.float64)
     M[0:3, 0:3] = R
     M[:3, 3] = t1
     T[0:3, 3] = -t0
     return numpy.dot(M, T)
 
 
-def norm(vector: numpy.ndarray, /) -> float:
+def norm(vector: NDArray[Any], /) -> float:
     """Return length of vector, i.e., its euclidean norm.
 
     Parameters:
         vector: Vector.
 
     """
     # return numpy.linalg.norm(vector)
@@ -1479,16 +1486,21 @@
     """
     if argv is None:
         argv = sys.argv
 
     # TODO: use argparse module
     import optparse
 
-    def search_doc(r, d):
-        return re.search(r, __doc__).group(1) if __doc__ else d
+    def search_doc(r: str, d: str) -> str:
+        if not __doc__:
+            return d
+        match = re.search(r, __doc__)
+        if match is None:
+            return d
+        return match.group(1)
 
     parser = optparse.OptionParser(
         usage='usage: %prog [options] sequence | file',
         description=search_doc('\n\n([^|]*?)\n\n', ''),
         version=f'%prog {__version__}',
         prog='dnacurve',
     )
@@ -1629,13 +1641,13 @@
                 results.plot(settings.png, dpi=settings.dpi)
     return 0
 
 
 MODELS.extend(
     sorted(
         (a for a in dir(Model) if not a.startswith('_') and a.isupper()),
-        key=lambda x: getattr(Model, x)['name'],
+        key=lambda x: getattr(Model, x)['name'],  # type: ignore
     )
 )
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `dnacurve-2022.10.4/dnacurve/web.py` & `dnacurve-2023.4.30/dnacurve/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # dnacurve/web.py
 
-# Copyright (c) 2005-2022, Christoph Gohlke
+# Copyright (c) 2005-2023, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -55,16 +55,14 @@
     def root():
         return response(request.form, request.base_url)
 
 """
 
 from __future__ import annotations
 
-__version__ = '2022.10.4'
-
 __all__ = ['main', 'response']
 
 import os
 import sys
 import io
 import base64
 import hashlib
```

### Comparing `dnacurve-2022.10.4/dnacurve.egg-info/PKG-INFO` & `dnacurve-2023.4.30/dnacurve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 Metadata-Version: 2.1
 Name: dnacurve
-Version: 2022.10.4
-Summary: DNA Curvature Analysis
+Version: 2023.4.30
+Summary: DNA curvature analysis
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/dnacurve/issues
 Project-URL: Source Code, https://github.com/cgohlke/dnacurve
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Provides-Extra: all
 License-File: LICENSE
 
-DNA Curvature Analysis
+DNA curvature analysis
 ======================
 
 Dnacurve is a Python library, console script, and web application to calculate
 the global 3D structure of a B-DNA molecule from its nucleotide sequence
 according to the dinucleotide wedge model. Local bending angles and macroscopic
 curvature are calculated at each nucleotide.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.10.4
-:DOI: 10.5281/zenodo.7135499
+:Version: 2023.4.30
+:DOI: `10.5281/zenodo.7135499 <https://doi.org/10.5281/zenodo.7135499>`_
 
 Quickstart
 ----------
 
 Install the dnacurve package and all dependencies from the
-Python Package Index::
+`Python Package Index <https://pypi.org/project/dnacurve/>`_::
 
     python -m pip install -U dnacurve[all]
 
 Print the console script usage::
 
     python -m dnacurve --help
 
@@ -56,25 +55,30 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/dnacurve>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `Numpy 1.22.4 <https://pypi.org/project/numpy/>`_
-- `Matplotlib 3.5.3 <https://pypi.org/project/matplotlib/>`_
-- `Flask 2.2.2 <https://pypi.org/project/Flask/>`_ (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `Numpy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+- `Flask <https://pypi.org/project/Flask/>`_ 2.3.1 (optional)
 
 Revisions
 ---------
 
+2023.4.30
+
+- Improve type hints.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.10.4
 
 - Rename dnacurve_web.py to web.py (breaking).
 - Deprecate save functions (use write functions).
 - Add options to specify URL of web application and not opening web browser.
 - Run web application using Flask if installed.
 - Convert to Google style docstrings.
```

### Comparing `dnacurve-2022.10.4/setup.py` & `dnacurve-2023.4.30/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,30 +59,29 @@
     url='https://www.cgohlke.com',
     project_urls={
         'Bug Tracker': 'https://github.com/cgohlke/dnacurve/issues',
         'Source Code': 'https://github.com/cgohlke/dnacurve',
         # 'Documentation': 'https://',
     },
     packages=['dnacurve'],
-    python_requires='>=3.8',
-    install_requires=['numpy>=1.19.2', 'matplotlib'],
+    install_requires=['numpy', 'matplotlib'],
     extras_require={'all': ['Flask']},
     entry_points={
         'console_scripts': [
             'dnacurve = dnacurve.dnacurve:main',
             'dnacurve_web = dnacurve.web:main',
         ]
     },
     platforms=['any'],
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: BSD License',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
```

