# Comparing `tmp/fatpack-0.7.3.tar.gz` & `tmp/fatpack-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gunnstein/documents/fatpack/dist/tmp5q6zq4lv/fatpack-0.7.3.tar", last modified: Tue Mar  8 20:29:47 2022, max compression
+gzip compressed data, was "fatpack-0.7.5.tar", last modified: Sat Apr 29 22:05:49 2023, max compression
```

## Comparing `fatpack-0.7.3.tar` & `fatpack-0.7.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gunnstein  (1000) gunnstein  (1000)        0 2022-03-08 20:29:47.000000 fatpack-0.7.3/
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)      780 2022-03-08 20:01:35.000000 fatpack-0.7.3/LICENSE
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)     2618 2022-03-08 20:29:47.000000 fatpack-0.7.3/PKG-INFO
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)     2132 2022-03-08 20:01:35.000000 fatpack-0.7.3/README.rst
-drwxrwxr-x   0 gunnstein  (1000) gunnstein  (1000)        0 2022-03-08 20:29:47.000000 fatpack-0.7.3/fatpack/
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)      262 2022-03-08 20:24:46.000000 fatpack-0.7.3/fatpack/__init__.py
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)    11888 2022-03-08 20:01:35.000000 fatpack-0.7.3/fatpack/endurance.py
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)     4011 2022-03-08 20:24:46.000000 fatpack-0.7.3/fatpack/racetrack.py
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)    20788 2022-03-08 20:24:46.000000 fatpack-0.7.3/fatpack/rainflow.py
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)     8826 2022-03-08 20:01:35.000000 fatpack-0.7.3/fatpack/stresscorrection.py
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)    15580 2022-03-08 20:24:46.000000 fatpack-0.7.3/fatpack/test.py
-drwxrwxr-x   0 gunnstein  (1000) gunnstein  (1000)        0 2022-03-08 20:29:47.000000 fatpack-0.7.3/fatpack.egg-info/
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)     2618 2022-03-08 20:29:46.000000 fatpack-0.7.3/fatpack.egg-info/PKG-INFO
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)      317 2022-03-08 20:29:47.000000 fatpack-0.7.3/fatpack.egg-info/SOURCES.txt
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)        1 2022-03-08 20:29:46.000000 fatpack-0.7.3/fatpack.egg-info/dependency_links.txt
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)        6 2022-03-08 20:29:47.000000 fatpack-0.7.3/fatpack.egg-info/requires.txt
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)        8 2022-03-08 20:29:47.000000 fatpack-0.7.3/fatpack.egg-info/top_level.txt
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)      102 2022-03-08 20:29:47.000000 fatpack-0.7.3/setup.cfg
--rw-rw-r--   0 gunnstein  (1000) gunnstein  (1000)     1050 2022-03-08 20:12:03.000000 fatpack-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:05:49.997643 fatpack-0.7.5/
+-rw-rw-rw-   0        0        0      780 2018-11-11 21:14:52.000000 fatpack-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0     3816 2023-04-29 22:05:49.997643 fatpack-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2421 2023-04-29 21:50:25.000000 fatpack-0.7.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 22:05:49.990661 fatpack-0.7.5/fatpack/
+-rw-rw-rw-   0        0        0      271 2023-04-29 21:50:25.000000 fatpack-0.7.5/fatpack/__init__.py
+-rw-rw-rw-   0        0        0    12301 2022-12-15 13:43:38.000000 fatpack-0.7.5/fatpack/endurance.py
+-rw-rw-rw-   0        0        0     4145 2023-04-25 20:48:52.000000 fatpack-0.7.5/fatpack/racetrack.py
+-rw-rw-rw-   0        0        0    20956 2023-04-25 22:52:28.000000 fatpack-0.7.5/fatpack/rainflow.py
+-rw-rw-rw-   0        0        0     9144 2021-02-24 12:13:18.000000 fatpack-0.7.5/fatpack/stresscorrection.py
+-rw-rw-rw-   0        0        0    15983 2023-04-25 22:31:50.000000 fatpack-0.7.5/fatpack/test.py
+drwxrwxrwx   0        0        0        0 2023-04-29 22:05:49.996645 fatpack-0.7.5/fatpack.egg-info/
+-rw-rw-rw-   0        0        0     3816 2023-04-29 22:05:49.000000 fatpack-0.7.5/fatpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-04-29 22:05:49.000000 fatpack-0.7.5/fatpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 22:05:49.000000 fatpack-0.7.5/fatpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 22:05:49.000000 fatpack-0.7.5/fatpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 22:05:49.000000 fatpack-0.7.5/fatpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      739 2023-04-29 21:50:25.000000 fatpack-0.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 22:05:49.997643 fatpack-0.7.5/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fatpack-0.7.3/LICENSE` & `fatpack-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fatpack-0.7.3/README.rst` & `fatpack-0.7.5/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,94 @@
-|logo_img|
-
-=======
-fatpack
-=======
-
-Python package for fatigue analysis of data series. The package
-requires `numpy`.
-
-
-Installation
-------------
-
-Either download the repository to your computer and install, e.g. by **pip**
-
-::
-
-   pip install .
-
-
-or install directly from the python package index.
-
-::
-
-   pip install fatpack
-
-
-Usage
------
-
-The package provides classes and functions for rainflow cycle counting,
-defining endurance curves, mean and compressive stress range correction 
-and racetrack filtering. The code example below shows how fatigue damage 
-can be calculated:
-
-.. code:: python
-
-    import numpy as np
-    import fatpack
-
-
-    # Assume that `y` is the data series, we generate one here
-    y = np.random.normal(0., 30., size=10000)
-
-    # Extract the stress ranges by rainflow counting
-    S = fatpack.find_rainflow_ranges(y)
-
-    # Determine the fatigue damage, using a trilinear fatigue curve
-    # with detail category Sc, Miner's linear damage summation rule.
-    Sc = 90.0
-    curve = fatpack.TriLinearEnduranceCurve(Sc)
-    fatigue_damage = curve.find_miner_sum(S)
-
-An example is included (`example.py <https://github.com/Gunnstein/fatpack/blob/master/example.py>`_) which extracts rainflow cycles,
-generates the rainflow matrix and rainflow stress spectrum, see the
-figure presented below. The example is a good place to start to get
-into the use of the package. 
-
-|example_img|
-
-
-Additional examples are found in the `examples folder <https://github.com/Gunnstein/fatpack/tree/master/examples>`_.
-
-
-Support
--------
-
-Please `open an issue <https://github.com/Gunnstein/fatpack/issues/new>`_
-for support.
-
-
-Contributing
-------------
-
-Please contribute using `Github Flow
-<https://guides.github.com/introduction/flow/>`_.
-Create a branch, add commits, and
-`open a pull request <https://github.com/Gunnstein/fatpack/compare/>`_.
-
-.. |logo_img| image:: https://github.com/Gunnstein/fatpack/blob/master/fatpack-logo.png
-    :target: https://github.com/gunnstein/fatpack/
-
-.. |example_img| image:: https://github.com/Gunnstein/fatpack/blob/master/example.png
-    :target: https://github.com/gunnstein/fatpack/
+|logo_img|
+
+=======
+fatpack
+=======
+ 
+.. image:: https://zenodo.org/badge/113768119.svg
+   :target: https://zenodo.org/badge/latestdoi/113768119
+   
+Python package for fatigue analysis of data series. The package
+requires `numpy`.
+
+
+Installation
+------------
+
+Either install from the github repository (latest version),
+
+::
+
+   pip install git+https://github.com/gunnstein/fatpack.git
+
+
+install from the python package index
+
+::
+
+   pip install fatpack
+
+
+or from the conda-forge:
+
+::
+
+   conda install --channel=conda-forge fatpack
+
+
+Usage
+-----
+
+The package provides functionality for rainflow cycle counting, defining 
+endurance curves, mean and compressive stress range correction 
+and racetrack filtering. The code example below shows how fatigue damage 
+can be calculated:
+
+.. code:: python
+
+    import numpy as np
+    import fatpack
+
+
+    # Assume that `y` is the data series, we generate one here
+    y = np.random.normal(0., 30., size=10000)
+
+    # Extract the stress ranges by rainflow counting
+    S = fatpack.find_rainflow_ranges(y)
+
+    # Determine the fatigue damage, using a trilinear fatigue curve
+    # with detail category Sc, Miner's linear damage summation rule.
+    Sc = 90.0
+    curve = fatpack.TriLinearEnduranceCurve(Sc)
+    fatigue_damage = curve.find_miner_sum(S)
+
+An example is included (`example.py <https://github.com/Gunnstein/fatpack/blob/master/example.py>`_) which extracts rainflow cycles,
+generates the rainflow matrix and rainflow stress spectrum, see the
+figure presented below. The example is a good place to start to get
+into the use of the package. 
+
+|example_img|
+
+
+Additional examples are found in the `examples folder <https://github.com/Gunnstein/fatpack/tree/master/examples>`_.
+
+
+Support
+-------
+
+Please `open an issue <https://github.com/Gunnstein/fatpack/issues/new>`_
+for support.
+
+
+Contributing
+------------
+
+Please contribute using `Github Flow
+<https://guides.github.com/introduction/flow/>`_.
+Create a branch, add commits, and
+`open a pull request <https://github.com/Gunnstein/fatpack/compare/>`_.
+
+.. |logo_img| image:: https://github.com/Gunnstein/fatpack/blob/master/fatpack-logo.png
+    :target: https://github.com/gunnstein/fatpack/
+
+.. |example_img| image:: https://github.com/Gunnstein/fatpack/blob/master/example.png
+    :target: https://github.com/gunnstein/fatpack/
```

### Comparing `fatpack-0.7.3/fatpack/endurance.py` & `fatpack-0.7.5/fatpack/endurance.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,413 +1,413 @@
-# -*- coding: utf-8 -*-
-from __future__ import (division, print_function, absolute_import,
-                        unicode_literals)
-import abc
-from functools import wraps
-import numpy as np
-
-
-__all__ = ["LinearEnduranceCurve", "BiLinearEnduranceCurve",
-           "TriLinearEnduranceCurve"]
-
-
-def ensure_array(method):
-    @wraps(method)
-    def wrapped_method(self, x):
-        x_is_float_or_int = isinstance(x, float) or isinstance(x, int)
-        if x_is_float_or_int:
-            xm = np.array([x])
-        else:
-            xm = np.asfarray(x)
-        ym = method(self, xm)
-        if x_is_float_or_int:
-            ym = ym[0]
-        return ym
-    return wrapped_method
-
-
-class AbstractEnduranceCurve(object):
-    """Abstract endurance curve.
-
-    Concrete subclasses should define methods:
-        `get_endurance`
-        `get_stress`
-
-    """
-    __metaclass__ = abc.ABCMeta
-
-    Ninf = np.inf
-
-    def __init__(self, Sc):
-        """Define endurance curve.
-
-        See class docstring for more information.
-
-        Arguments
-        ---------
-        Sc : float
-            Characteristic stress
-        """
-        self.Sc = Sc
-
-    @abc.abstractmethod
-    def get_endurance(self, S):
-        """Return endurance value(s) for stress range(s) S.
-
-        Arguments
-        ---------
-        S : float or 1darray
-            Stress range(s) to find the corresponding endurance(s) for.
-
-        Returns
-        -------
-        float or 1darray
-            Endurance for the stress range(s) S.
-        """
-
-    @abc.abstractmethod
-    def get_stress(self, N):
-        """Return stress range(s) for the endurance(s) N.
-
-        Arguments
-        ---------
-        N : float or 1darray
-            Endurance(s) to find the corresponding stress for.
-
-        Returns
-        -------
-        float or 1darray
-            Stress range(s) for endurance(s) N.
-        """
-
-    def find_miner_sum(self, S):
-        """Calculate Miner sum of stress ranges S with the endurance curve.
-
-        The method calculates the Miner sum from the stress ranges.
-
-        Arguments
-        ---------
-        S : 1darray or 2darray
-            If `S` is a 1darray (N) it is assumed that each
-            stress range corresponds to one full cycle. If `S` is
-            given in a 2darray (N, 2), it is assumed that the first
-            column is stress range and the second column contains the
-            count of that stress range.
-
-        Returns
-        -------
-        float
-            Miner sum
-
-        Raises
-        ------
-        ValueError
-            If `S` is not a 1darray (N, ) or 2darray (N, 2).
-
-        Example
-        -------
-        >>> import fatpack
-        >>> import numpy as np
-        >>> np.random.seed(10)
-
-        First we create an endurance curve with detail category 90.
-        >>> curve = fatpack.LinearEnduranceCurve(90.)
-
-        The miner sum is then found from a signal y after extracting 
-        rainflow ranges in the following way
-
-        >>> y = np.random.normal(size=100000) * 10.
-        >>> S = fatpack.find_rainflow_ranges(y)
-        >>> D = curve.find_miner_sum(S)
-        >>> print("The damage in signal y is D={0:3.2e}".format(D))
-        The damage in signal y is D=6.56e-05
-
-        """
-
-        Sr = np.asfarray(S)
-        shape = Sr.shape
-        if len(shape) == 1:
-            miner_sum = np.sum(1. / self.get_endurance(Sr))
-        elif len(shape) == 2 and shape[1] == 2:
-            miner_sum = np.sum(Sr[:, 1] / self.get_endurance(Sr[:, 0]))
-        else:
-            raise ValueError("S must be 1darray (N) or 2darray (N, 2)")
-        return miner_sum
-
-
-class LinearEnduranceCurve(AbstractEnduranceCurve):
-    """Define a linear endurance curve.
-
-            ^                log N - log S
-            |
-            | *
-            |    *
-            |       *         m
-            |          * - - - - - +
-      S     |             *        .
-      t  Sc + - - - - - - - -*     . 1
-      r     |                .  *  .
-      e     |                .     *
-      s     |                .        *
-      s     |                .           *
-            |                .              *
-            |                .                 *
-            |                .                    *
-            |----------------|-------------------------->
-                             Nc
-                          Endurance
-
-    In fatpack the slope parameter (m) and the `detail category` or
-    `characteristic` stress and endurance (Sc, Nc) is used to define
-    the linear curve. The default values for the characteristic
-    endurance `Nc` (2.0e6) and the slope `m` (5.0) properties can be
-    adjusted on the instance and class.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    First we create an endurance curve with detail category 90.
-    >>> curve = fatpack.LinearEnduranceCurve(90.)
-
-    Let us find the damage according to Miner's linear damage rule from
-    a rainflow counted signal y
-
-    >>> y = np.random.normal(size=100000) * 10.
-    >>> S = fatpack.find_rainflow_ranges(y)
-    >>> D = curve.find_miner_sum(S)
-    >>> print("The damage in signal y is D={0:3.2e}".format(D))
-    The damage in signal y is D=6.56e-05
-
-    Finally, we can create a figure of the endurance curve with matplotlib
-    
-    >>> import matplotlib.pyplot as plt
-    >>> N = np.logspace(4, 9, 1000)
-    >>> S = curve.get_stress(N)
-    >>> line = plt.loglog(N, S)
-    >>> grd = plt.grid(which='both')
-    >>> title = plt.title("Linear endurance curve")
-    >>> xlab = plt.xlabel("Cycles to failure (1)")
-    >>> ylab = plt.ylabel("Stress range (MPa)")
-    >>> plt.show(block=True)
-
-    """
-
-    m = 5.0
-    Nc = 2.0e6
-
-    @property
-    def C(self):
-        """Characteristic intercept constant."""
-        return self.Nc * self.Sc ** self.m
-
-    @ensure_array
-    def get_endurance(self, S):
-        return self.Nc * (self.Sc / S) ** self.m
-
-    @ensure_array
-    def get_stress(self, N):
-        return self.Sc * (self.Nc / N) ** (1. / self.m)
-
-
-class BiLinearEnduranceCurve(AbstractEnduranceCurve):
-    """Define a bilinear endurance curve.
-
-            ^                log N - log S
-            |
-            |*
-            | *  m1
-            |  *- -+
-            |   *  .
-     S   Sc +- - * . 1
-     t      |    .*.
-     r      |    . *
-     e      |    .  *
-     s   Sd +- - - - *
-     s      |    .    . *      m2
-            |    .    .    * - - - -+
-            |    .    .       *     . 1
-            |    .    .          *  .
-            |    .    .             *
-            |    .    .                *
-            |    .    .                   *
-            |----|----|---------------------------------->
-                 Nc   Nd
-                             Endurance
-
-
-    The slope parameters (m1, m2), endurance value at the knee point
-    of the bilinear curve (Nd) and the `detail category` or
-    `characteristic` stress and endurance (Sc, Nc) is used to define
-    the bilinear curve. The default values for the characteristic
-    endurance `Nc` (2.0e6) and the slope `m` (5.0) properties can be
-    adjusted on the instance and class.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    First we create an endurance curve with detail category 90.
-    >>> curve = fatpack.BiLinearEnduranceCurve(90.)
-
-    Let us find the damage according to Miner's linear damage rule from
-    a rainflow counted signal y
-
-    >>> y = np.random.normal(size=100000) * 10.
-    >>> S = fatpack.find_rainflow_ranges(y)
-    >>> D = curve.find_miner_sum(S)
-    >>> print("The damage in signal y is D={0:3.2e}".format(D))
-    The damage in signal y is D=1.19e-04
-
-    Finally, we can create a figure of the endurance curve with matplotlib
-    
-    >>> import matplotlib.pyplot as plt
-    >>> N = np.logspace(4, 9, 1000)
-    >>> S = curve.get_stress(N)
-    >>> line = plt.loglog(N, S)
-    >>> grd = plt.grid(which='both')
-    >>> title = plt.title("Bi linear endurance curve")
-    >>> xlab = plt.xlabel("Cycles to failure (1)")
-    >>> ylab = plt.ylabel("Stress range (MPa)")
-    >>> plt.show(block=True)
-
-    """
-
-    Nc = 2.0e6
-    Nd = 5.0e6
-    m1 = 3.0
-    m2 = 5.0
-
-    @property
-    def Sd(self):
-        return self.Sc * (self.Nc / self.Nd) ** (1. / self.m1)
-
-    @property
-    def curve1(self):
-        curve = LinearEnduranceCurve(self.Sc)
-        curve.Nc = self.Nc
-        curve.m = self.m1
-        return curve
-
-    @property
-    def curve2(self):
-        curve = LinearEnduranceCurve(self.Sd)
-        curve.Nc = self.Nd
-        curve.m = self.m2
-        return curve
-
-    @ensure_array
-    def get_endurance(self, S):
-        Sd = self.Sd
-        N = np.ones_like(S) * self.Ninf
-        N[S > Sd] = self.curve1.get_endurance(S[S > Sd])
-        N[S <= Sd] = self.curve2.get_endurance(S[S <= Sd])
-        return N
-
-    @ensure_array
-    def get_stress(self, N):
-        S = np.zeros_like(N)
-        S[N <= self.Nd] = self.curve1.get_stress(N[N <= self.Nd])
-        S[N > self.Nd] = self.curve2.get_stress(N[N > self.Nd])
-        return S
-
-    @property
-    def C1(self):
-        """Intercept constant for the first slope."""
-        return self.curve1.C
-
-    @property
-    def C2(self):
-        """Intercept constant for the second slope."""
-        return self.curve2.C
-
-
-class TriLinearEnduranceCurve(BiLinearEnduranceCurve):
-    """Define a trilinear endurance curve.
-            ^                log N - log S
-            |              
-            |*
-            | *  m1
-            |  *---+
-            |   *  |
-     S   Sc +    * | 1
-     t      |     *|
-     r   Sd +      *       m2
-     e      |         *--------+
-     s      |            *     | 1
-     s      |               *  |
-            |                  *
-         Sl +                     *  *  *  *  *  *  *  *
-            |
-            |
-            |---|----|-------------|-------------------->
-               Nc   Nd             Nl
-                             Endurance
-
-    The slope parameters (m1, m2), endurance values at the knee points
-    of the trilinear curve (Nd, Nl) and the `detail category` or
-    `characteristic` stress and endurance (Sc, Nc) is used to define
-    the trilinear curve.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    First we create an endurance curve with detail category 90.
-    >>> curve = fatpack.TriLinearEnduranceCurve(90.)
-
-    Let us find the damage according to Miner's linear damage rule from
-    a rainflow counted signal y
-
-    >>> y = np.random.normal(size=100000) * 10.
-    >>> S = fatpack.find_rainflow_ranges(y)
-    >>> D = curve.find_miner_sum(S)
-    >>> print("The damage in signal y is D={0:3.2e}".format(D))
-    The damage in signal y is D=9.23e-05
-
-    Finally, we can create a figure of the endurance curve with matplotlib
-    
-    >>> import matplotlib.pyplot as plt
-    >>> N = np.logspace(4, 9, 1000)
-    >>> S = curve.get_stress(N)
-    >>> line = plt.loglog(N, S)
-    >>> grd = plt.grid(which='both')
-    >>> title = plt.title("Tri linear endurance curve")
-    >>> xlab = plt.xlabel("Cycles to failure (1)")
-    >>> ylab = plt.ylabel("Stress range (MPa)")
-    >>> plt.show(block=True)
-
-    """
-    
-    Nc = 2.0e6
-    Nd = 5.0e6
-    Nl = 1.0e8
-    m1 = 3.0
-    m2 = 5.0
-
-    @property
-    def Sl(self):
-        """Variable amplitude fatigue limit."""
-        return self.Sd * (self.Nd / self.Nl) ** (1. / self.m2)
-
-    @ensure_array
-    def get_endurance(self, S):
-        N = super(TriLinearEnduranceCurve, self).get_endurance(S)
-        N[S<self.Sl] = self.Ninf
-        return N
-
-    @ensure_array
-    def get_stress(self, N):
-        S = super(TriLinearEnduranceCurve, self).get_stress(N)
-        S[N > self.Nl] = self.curve2.get_stress(self.Nl)
-        return S
-
-
-if __name__ == "__main__":
-    import doctest
-    doctest.testmod()
+# -*- coding: utf-8 -*-
+from __future__ import (division, print_function, absolute_import,
+                        unicode_literals)
+import abc
+from functools import wraps
+import numpy as np
+
+
+__all__ = ["LinearEnduranceCurve", "BiLinearEnduranceCurve",
+           "TriLinearEnduranceCurve"]
+
+
+def ensure_array(method):
+    @wraps(method)
+    def wrapped_method(self, x):
+        x_is_float_or_int = isinstance(x, float) or isinstance(x, int)
+        if x_is_float_or_int:
+            xm = np.array([x])
+        else:
+            xm = np.asfarray(x)
+        ym = method(self, xm)
+        if x_is_float_or_int:
+            ym = ym[0]
+        return ym
+    return wrapped_method
+
+
+class AbstractEnduranceCurve(object):
+    """Abstract endurance curve.
+
+    Concrete subclasses should define methods:
+        `get_endurance`
+        `get_stress`
+
+    """
+    __metaclass__ = abc.ABCMeta
+
+    Ninf = np.inf
+
+    def __init__(self, Sc):
+        """Define endurance curve.
+
+        See class docstring for more information.
+
+        Arguments
+        ---------
+        Sc : float
+            Characteristic stress
+        """
+        self.Sc = Sc
+
+    @abc.abstractmethod
+    def get_endurance(self, S):
+        """Return endurance value(s) for stress range(s) S.
+
+        Arguments
+        ---------
+        S : float or 1darray
+            Stress range(s) to find the corresponding endurance(s) for.
+
+        Returns
+        -------
+        float or 1darray
+            Endurance for the stress range(s) S.
+        """
+
+    @abc.abstractmethod
+    def get_stress(self, N):
+        """Return stress range(s) for the endurance(s) N.
+
+        Arguments
+        ---------
+        N : float or 1darray
+            Endurance(s) to find the corresponding stress for.
+
+        Returns
+        -------
+        float or 1darray
+            Stress range(s) for endurance(s) N.
+        """
+
+    def find_miner_sum(self, S):
+        """Calculate Miner sum of stress ranges S with the endurance curve.
+
+        The method calculates the Miner sum from the stress ranges.
+
+        Arguments
+        ---------
+        S : 1darray or 2darray
+            If `S` is a 1darray (N) it is assumed that each
+            stress range corresponds to one full cycle. If `S` is
+            given in a 2darray (N, 2), it is assumed that the first
+            column is stress range and the second column contains the
+            count of that stress range.
+
+        Returns
+        -------
+        float
+            Miner sum
+
+        Raises
+        ------
+        ValueError
+            If `S` is not a 1darray (N, ) or 2darray (N, 2).
+
+        Example
+        -------
+        >>> import fatpack
+        >>> import numpy as np
+        >>> np.random.seed(10)
+
+        First we create an endurance curve with detail category 90.
+        >>> curve = fatpack.LinearEnduranceCurve(90.)
+
+        The miner sum is then found from a signal y after extracting 
+        rainflow ranges in the following way
+
+        >>> y = np.random.normal(size=100000) * 10.
+        >>> S = fatpack.find_rainflow_ranges(y)
+        >>> D = curve.find_miner_sum(S)
+        >>> print("The damage in signal y is D={0:3.2e}".format(D))
+        The damage in signal y is D=6.56e-05
+
+        """
+
+        Sr = np.asfarray(S)
+        shape = Sr.shape
+        if len(shape) == 1:
+            miner_sum = np.sum(1. / self.get_endurance(Sr))
+        elif len(shape) == 2 and shape[1] == 2:
+            miner_sum = np.sum(Sr[:, 1] / self.get_endurance(Sr[:, 0]))
+        else:
+            raise ValueError("S must be 1darray (N) or 2darray (N, 2)")
+        return miner_sum
+
+
+class LinearEnduranceCurve(AbstractEnduranceCurve):
+    """Define a linear endurance curve.
+
+            ^                log N - log S
+            |
+            | *
+            |    *
+            |       *         m
+            |          * - - - - - +
+      S     |             *        .
+      t  Sc + - - - - - - - -*     . 1
+      r     |                .  *  .
+      e     |                .     *
+      s     |                .        *
+      s     |                .           *
+            |                .              *
+            |                .                 *
+            |                .                    *
+            |----------------|-------------------------->
+                             Nc
+                          Endurance
+
+    In fatpack the slope parameter (m) and the `detail category` or
+    `characteristic` stress and endurance (Sc, Nc) is used to define
+    the linear curve. The default values for the characteristic
+    endurance `Nc` (2.0e6) and the slope `m` (5.0) properties can be
+    adjusted on the instance and class.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    First we create an endurance curve with detail category 90.
+    >>> curve = fatpack.LinearEnduranceCurve(90.)
+
+    Let us find the damage according to Miner's linear damage rule from
+    a rainflow counted signal y
+
+    >>> y = np.random.normal(size=100000) * 10.
+    >>> S = fatpack.find_rainflow_ranges(y)
+    >>> D = curve.find_miner_sum(S)
+    >>> print("The damage in signal y is D={0:3.2e}".format(D))
+    The damage in signal y is D=6.56e-05
+
+    Finally, we can create a figure of the endurance curve with matplotlib
+    
+    >>> import matplotlib.pyplot as plt
+    >>> N = np.logspace(4, 9, 1000)
+    >>> S = curve.get_stress(N)
+    >>> line = plt.loglog(N, S)
+    >>> grd = plt.grid(which='both')
+    >>> title = plt.title("Linear endurance curve")
+    >>> xlab = plt.xlabel("Cycles to failure (1)")
+    >>> ylab = plt.ylabel("Stress range (MPa)")
+    >>> plt.show(block=True)
+
+    """
+
+    m = 5.0
+    Nc = 2.0e6
+
+    @property
+    def C(self):
+        """Characteristic intercept constant."""
+        return self.Nc * self.Sc ** self.m
+
+    @ensure_array
+    def get_endurance(self, S):
+        return self.Nc * (self.Sc / S) ** self.m
+
+    @ensure_array
+    def get_stress(self, N):
+        return self.Sc * (self.Nc / N) ** (1. / self.m)
+
+
+class BiLinearEnduranceCurve(AbstractEnduranceCurve):
+    """Define a bilinear endurance curve.
+
+            ^                log N - log S
+            |
+            |*
+            | *  m1
+            |  *- -+
+            |   *  .
+     S   Sc +- - * . 1
+     t      |    .*.
+     r      |    . *
+     e      |    .  *
+     s   Sd +- - - - *
+     s      |    .    . *      m2
+            |    .    .    * - - - -+
+            |    .    .       *     . 1
+            |    .    .          *  .
+            |    .    .             *
+            |    .    .                *
+            |    .    .                   *
+            |----|----|---------------------------------->
+                 Nc   Nd
+                             Endurance
+
+
+    The slope parameters (m1, m2), endurance value at the knee point
+    of the bilinear curve (Nd) and the `detail category` or
+    `characteristic` stress and endurance (Sc, Nc) is used to define
+    the bilinear curve. The default values for the characteristic
+    endurance `Nc` (2.0e6) and the slope `m` (5.0) properties can be
+    adjusted on the instance and class.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    First we create an endurance curve with detail category 90.
+    >>> curve = fatpack.BiLinearEnduranceCurve(90.)
+
+    Let us find the damage according to Miner's linear damage rule from
+    a rainflow counted signal y
+
+    >>> y = np.random.normal(size=100000) * 10.
+    >>> S = fatpack.find_rainflow_ranges(y)
+    >>> D = curve.find_miner_sum(S)
+    >>> print("The damage in signal y is D={0:3.2e}".format(D))
+    The damage in signal y is D=1.19e-04
+
+    Finally, we can create a figure of the endurance curve with matplotlib
+    
+    >>> import matplotlib.pyplot as plt
+    >>> N = np.logspace(4, 9, 1000)
+    >>> S = curve.get_stress(N)
+    >>> line = plt.loglog(N, S)
+    >>> grd = plt.grid(which='both')
+    >>> title = plt.title("Bi linear endurance curve")
+    >>> xlab = plt.xlabel("Cycles to failure (1)")
+    >>> ylab = plt.ylabel("Stress range (MPa)")
+    >>> plt.show(block=True)
+
+    """
+
+    Nc = 2.0e6
+    Nd = 5.0e6
+    m1 = 3.0
+    m2 = 5.0
+
+    @property
+    def Sd(self):
+        return self.Sc * (self.Nc / self.Nd) ** (1. / self.m1)
+
+    @property
+    def curve1(self):
+        curve = LinearEnduranceCurve(self.Sc)
+        curve.Nc = self.Nc
+        curve.m = self.m1
+        return curve
+
+    @property
+    def curve2(self):
+        curve = LinearEnduranceCurve(self.Sd)
+        curve.Nc = self.Nd
+        curve.m = self.m2
+        return curve
+
+    @ensure_array
+    def get_endurance(self, S):
+        Sd = self.Sd
+        N = np.ones_like(S) * self.Ninf
+        N[S > Sd] = self.curve1.get_endurance(S[S > Sd])
+        N[S <= Sd] = self.curve2.get_endurance(S[S <= Sd])
+        return N
+
+    @ensure_array
+    def get_stress(self, N):
+        S = np.zeros_like(N)
+        S[N <= self.Nd] = self.curve1.get_stress(N[N <= self.Nd])
+        S[N > self.Nd] = self.curve2.get_stress(N[N > self.Nd])
+        return S
+
+    @property
+    def C1(self):
+        """Intercept constant for the first slope."""
+        return self.curve1.C
+
+    @property
+    def C2(self):
+        """Intercept constant for the second slope."""
+        return self.curve2.C
+
+
+class TriLinearEnduranceCurve(BiLinearEnduranceCurve):
+    """Define a trilinear endurance curve.
+            ^                log N - log S
+            |              
+            |*
+            | *  m1
+            |  *---+
+            |   *  |
+     S   Sc +    * | 1
+     t      |     *|
+     r   Sd +      *       m2
+     e      |         *--------+
+     s      |            *     | 1
+     s      |               *  |
+            |                  *
+         Sl +                     *  *  *  *  *  *  *  *
+            |
+            |
+            |---|----|-------------|-------------------->
+               Nc   Nd             Nl
+                             Endurance
+
+    The slope parameters (m1, m2), endurance values at the knee points
+    of the trilinear curve (Nd, Nl) and the `detail category` or
+    `characteristic` stress and endurance (Sc, Nc) is used to define
+    the trilinear curve.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    First we create an endurance curve with detail category 90.
+    >>> curve = fatpack.TriLinearEnduranceCurve(90.)
+
+    Let us find the damage according to Miner's linear damage rule from
+    a rainflow counted signal y
+
+    >>> y = np.random.normal(size=100000) * 10.
+    >>> S = fatpack.find_rainflow_ranges(y)
+    >>> D = curve.find_miner_sum(S)
+    >>> print("The damage in signal y is D={0:3.2e}".format(D))
+    The damage in signal y is D=9.23e-05
+
+    Finally, we can create a figure of the endurance curve with matplotlib
+    
+    >>> import matplotlib.pyplot as plt
+    >>> N = np.logspace(4, 9, 1000)
+    >>> S = curve.get_stress(N)
+    >>> line = plt.loglog(N, S)
+    >>> grd = plt.grid(which='both')
+    >>> title = plt.title("Tri linear endurance curve")
+    >>> xlab = plt.xlabel("Cycles to failure (1)")
+    >>> ylab = plt.ylabel("Stress range (MPa)")
+    >>> plt.show(block=True)
+
+    """
+    
+    Nc = 2.0e6
+    Nd = 5.0e6
+    Nl = 1.0e8
+    m1 = 3.0
+    m2 = 5.0
+
+    @property
+    def Sl(self):
+        """Variable amplitude fatigue limit."""
+        return self.Sd * (self.Nd / self.Nl) ** (1. / self.m2)
+
+    @ensure_array
+    def get_endurance(self, S):
+        N = super(TriLinearEnduranceCurve, self).get_endurance(S)
+        N[S<self.Sl] = self.Ninf
+        return N
+
+    @ensure_array
+    def get_stress(self, N):
+        S = super(TriLinearEnduranceCurve, self).get_stress(N)
+        S[N > self.Nl] = self.curve2.get_stress(self.Nl)
+        return S
+
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `fatpack-0.7.3/fatpack/racetrack.py` & `fatpack-0.7.5/fatpack/racetrack.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-# -*- coding: utf-8 -*-
-"""
-Implementation of the racetrack amplitude filter. The implementation is
-based on the following resources:
-
-    `H. O. Fuchs et al. Shortcuts in cumulative damage analysis.
-    SAE Automobile engineering meeting paper 730565. (1973)`
-
-    `H. Wu et. al. Validation of the multiaxial racetrack amplitude filter.
-    International Journal of Fatigue, 87 (2016) 167–179`
-
-"""
-from __future__ import (division, print_function, absolute_import,
-                        unicode_literals)
-import numpy as np
-from math import fabs
-from .rainflow import find_reversals
-
-__all__ = ["racetrack_filter", "find_reversals_racetrack_filtered"]
-
-
-def racetrack_filter(reversals, h):
-    """Racetrack filter for accelerated fatigue testing.
-
-    The racetrack amplitude filter removes low amplitude cycles from
-    the reversals without altering the sequence of the remaining
-    cycles. The racetrack filter therefore allows to accelerate
-    variable amplitude fatigue testing by removing low amplitude
-    cycles which does not significantly affect the overall fatigue
-    damage and at the same time preserves sequence effects inherent in
-    the original sequence.
-
-    Arguments
-    ---------
-    reversals : 1darray
-        An 1D-array of reversals.
-    h : float
-        Racetrack width, cycles with range lower than width are
-        filtered out.
-
-    Returns
-    -------
-    signal : 1darray
-        Signal after applying racetrack filter.
-    indices : 1darray
-        Indices of racetrack filtered signal.
-
-    """
-
-    y = reversals
-    yprev = None
-    ix = []
-    for n, yn in enumerate(y):
-        if (n == 0) or (n == y.size-1):
-            yprev = yn
-            ix.append(n)
-            continue
-        dy = yn - yprev
-        if fabs(dy) > h / 2.:
-            yprev = yn - dy/fabs(dy) * h/2.
-            ix.append(n)
-    ix = np.array(ix, dtype=int)
-    return y[ix], ix
-
-
-def find_reversals_racetrack_filtered(y, h, k=64):
-    """Return racetrack filtered reversals and indices in `y`.
-
-    The data points in the dataseries `y` are classified into `k`
-    constant sized intervals and then peak-valley filtered to yield
-    the successive extremas of the dataseries `y`. The reversals are
-    then filtered with the racetrack amplitude filter and then
-    peak-valley filtered again to find the racetrack filtered
-    reversals.
-
-    Arguments
-    ---------
-    y : 1darray
-        Dataseries containing the signal to find the reversals for.
-    h : float
-        Racetrack width, cycles with range lower than width are
-        filtered out.
-    k : int
-        The number of intervals to divide the min-max range of the
-        dataseries into.
-
-    Returns
-    -------
-    reversals : 1darray
-        Reversals of the initial data series `y` after racetrack
-        filtering.
-    indices : 1darray
-        The indices of the initial data series `y` which corresponds
-        to the reversals.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-
-    >>> y = np.random.normal(size=100000) * 10.
-
-    Extract reversals with all rainflow ranges lower than 15 removed
-
-    >>> rev_rtf, ix_rtf = fatpack.find_reversals_racetrack_filtered(y, h=15.)
-
-    Below a figure is created which shows reversals of the dataseris with and without the racetrack
-    filter
-
-    >>> import matplotlib.pyplot as plt
-    >>> rev, ix = fatpack.find_reversals(y)
-    >>> l1 = plt.plot(ix, rev, label='reversals')
-    >>> l2 = plt.plot(ix_rtf, rev_rtf, label='racetrack filtered reversals')
-    >>> xlim = plt.xlim(0, 100)
-    >>> leg = plt.legend(loc='best')
-    >>> xlab = plt.xlabel("Indices")
-    >>> ylab = plt.ylabel("Signal")
-    >>> plt.show(block=True)
-
-    """
-
-    _, ix = find_reversals(y, k=k)
-    z, ixz = racetrack_filter(y[ix], h)
-    ix = ix[ixz]
-    rev, ixr = find_reversals(z, k=k)
-    return y[ix[ixr]], ix[ixr]
-
-
-if __name__ == "__main__":
-    import doctest
-    doctest.testmod()
+# -*- coding: utf-8 -*-
+"""
+Implementation of the racetrack amplitude filter. The implementation is
+based on the following resources:
+
+    `H. O. Fuchs et al. Shortcuts in cumulative damage analysis.
+    SAE Automobile engineering meeting paper 730565. (1973)`
+
+    `H. Wu et. al. Validation of the multiaxial racetrack amplitude filter.
+    International Journal of Fatigue, 87 (2016) 167–179`
+
+"""
+from __future__ import (division, print_function, absolute_import,
+                        unicode_literals)
+import numpy as np
+from math import fabs
+from .rainflow import find_reversals
+
+__all__ = ["racetrack_filter", "find_reversals_racetrack_filtered"]
+
+
+def racetrack_filter(reversals, h):
+    """Racetrack filter for accelerated fatigue testing.
+
+    The racetrack amplitude filter removes low amplitude cycles from
+    the reversals without altering the sequence of the remaining
+    cycles. The racetrack filter therefore allows to accelerate
+    variable amplitude fatigue testing by removing low amplitude
+    cycles which does not significantly affect the overall fatigue
+    damage and at the same time preserves sequence effects inherent in
+    the original sequence.
+
+    Arguments
+    ---------
+    reversals : 1darray
+        An 1D-array of reversals.
+    h : float
+        Racetrack width, cycles with range lower than width are
+        filtered out.
+
+    Returns
+    -------
+    signal : 1darray
+        Signal after applying racetrack filter.
+    indices : 1darray
+        Indices of racetrack filtered signal.
+
+    """
+
+    y = reversals
+    yprev = None
+    ix = []
+    for n, yn in enumerate(y):
+        if (n == 0) or (n == y.size-1):
+            yprev = yn
+            ix.append(n)
+            continue
+        dy = yn - yprev
+        if fabs(dy) > h / 2.:
+            yprev = yn - dy/fabs(dy) * h/2.
+            ix.append(n)
+    ix = np.array(ix, dtype=int)
+    return y[ix], ix
+
+
+def find_reversals_racetrack_filtered(y, h, k=64):
+    """Return racetrack filtered reversals and indices in `y`.
+
+    The data points in the dataseries `y` are classified into `k`
+    constant sized intervals and then peak-valley filtered to yield
+    the successive extremas of the dataseries `y`. The reversals are
+    then filtered with the racetrack amplitude filter and then
+    peak-valley filtered again to find the racetrack filtered
+    reversals.
+
+    Arguments
+    ---------
+    y : 1darray
+        Dataseries containing the signal to find the reversals for.
+    h : float
+        Racetrack width, cycles with range lower than width are
+        filtered out.
+    k : int
+        The number of intervals to divide the min-max range of the
+        dataseries into.
+
+    Returns
+    -------
+    reversals : 1darray
+        Reversals of the initial data series `y` after racetrack
+        filtering.
+    indices : 1darray
+        The indices of the initial data series `y` which corresponds
+        to the reversals.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+
+    >>> y = np.random.normal(size=100000) * 10.
+
+    Extract reversals with all rainflow ranges lower than 15 removed
+
+    >>> rev_rtf, ix_rtf = fatpack.find_reversals_racetrack_filtered(y, h=15.)
+
+    Below a figure is created which shows reversals of the dataseris with and without the racetrack
+    filter
+
+    >>> import matplotlib.pyplot as plt
+    >>> rev, ix = fatpack.find_reversals(y)
+    >>> l1 = plt.plot(ix, rev, label='reversals')
+    >>> l2 = plt.plot(ix_rtf, rev_rtf, label='racetrack filtered reversals')
+    >>> xlim = plt.xlim(0, 100)
+    >>> leg = plt.legend(loc='best')
+    >>> xlab = plt.xlabel("Indices")
+    >>> ylab = plt.ylabel("Signal")
+    >>> plt.show(block=True)
+
+    """
+
+    _, ix = find_reversals(y, k=k)
+    z, ixz = racetrack_filter(y[ix], h)
+    ix = ix[ixz]
+    rev, ixr = find_reversals(z, k=k)
+    return y[ix[ixr]], ix[ixr]
+
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `fatpack-0.7.3/fatpack/rainflow.py` & `fatpack-0.7.5/fatpack/rainflow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,656 +1,642 @@
-# -*- coding: utf-8 -*-
-"""
-Implementation of 4-point rainflow counting algorithm in numpy. The
-implementation and terminology is based on the following resources:
-
-    `C. Amzallag et. al. Standardization of the rainflow counting method for
-    fatigue analysis. International Journal of Fatigue, 16 (1994) 287-293`
-
-    `ISO 12110-2, Metallic materials - Fatigue testing - Variable amplitude
-     fatigue testing.`
-
-    `G. Marsh et. al. Review and application of Rainflow residue processing
-    techniques for accurate fatigue damage estimation. International Journal
-    of Fatigue, 82 (2016) 757-765`
-
-Note that there are two functions for finding the reversals.
-
-    * `find_reversals_strict` passes the example provided in ISO12110-2 by
-    ensuring that data points which fall on a load class boundary are rounded
-    upwards if the reversal is a peak and downwards if it is a valley.
-
-    * `find_reversals` classifies the data points by rounding the datapoints
-    which lies on the boundary to the lower load class. This function is more
-    efficient than the strict version, and yields practically identical results
-    if the number of load classes is set sufficiently high.
-"""
-from __future__ import (division, print_function, absolute_import,
-                        unicode_literals)
-import numpy as np
-from math import fabs
-
-__all__ = ["find_reversals", "find_rainflow_cycles", "find_rainflow_matrix",
-           "find_rainflow_ranges", "find_range_count", "concatenate_reversals"]
-
-
-def get_load_classes(y, k=64):
-    ymax, ymin = y.max(), y.min()
-    return np.linspace(ymin, ymax, k+1)
-
-
-def get_load_class_boundaries(y, k=64):
-    ymin, ymax = y.min(), y.max()
-    dy = (ymax-ymin) / (2.0*k)
-    y0 = ymin - dy
-    y1 = ymax + dy
-    return np.linspace(y0, y1, k+2)
-
-
-def find_reversals_strict(y, k=64):
-    """Return reversals (peaks and valleys) and indices of reversals in `y`.
-
-    The data points in the dataseries `y` are classified into `k` constant
-    sized intervals and then peak-valley filtered to yield the successive
-    extremas of the dataseries `y`.
-
-    The function is strict in the sense that data points which fall on a load
-    class boundary are rounded upwards if the reversal is a peak and downwards
-    to the closest load class if it is a valley.
-
-    Arguments
-    ---------
-    y : 1darray
-        Dataseries containing the signal to find the reversals for.
-    k : int
-        The number of intervals to divide the min-max range of the dataseries
-        into.
-
-    Returns
-    -------
-    reversals : 1darray
-        The reversals of the initial data series `y`.
-    indices : 1darray
-        The indices of the initial data series `y` which corresponds to the
-        reversals.
-
-    See Also
-    --------
-    find_reversals: Faster version of this function
-
-    """
-
-    y = y.copy()  # Make sure we do not change the original sequence
-    sgn = np.sign
-    Y = get_load_class_boundaries(y, k)
-    dY = Y[1] - Y[0]
-
-    # Classifying points into levels
-    for yl, yu in zip(Y[:-1], Y[1:]):
-        y[(yl < y) & (y < yu)] = (yl+yu)/2.
-
-    # Classifying points on the level boundary
-    for n, yi in enumerate(y):
-        if not np.any(yi == Y):
-            continue
-        if n > 0:
-            dy = y[n]-y[n-1]
-        else:
-            dy = y[n+1] - y[n]
-        if dy < 0.:
-            y[n] = yi - dY / 2.
-        else:
-            y[n] = yi + dY / 2.
-
-    # Remove successive datapoints in each class
-    ix = [0]
-    for n, yi in enumerate(y):
-        if n == 0:
-            continue
-        if yi != y[ix[-1]]:
-            ix.append(n)
-
-    # Peak-valley filtering
-    revix = [0]
-    for n in range(len(ix)-1):
-        if n == 0:
-            continue
-        dy1, dy2 = y[ix[n]]-y[ix[n-1]], y[ix[n+1]]-y[ix[n]]
-        if (sgn(dy1) != sgn(dy2)):
-            revix.append(ix[n])
-
-    # Peak-valley filtering of last point
-    dy1, dy2 = y[revix[-1]]-y[revix[-2]], y[ix[-1]] - y[revix[-1]]
-    if sgn(dy1) == sgn(dy2):
-        revix[-1] = ix[-1]
-    else:
-        revix.append(ix[-1])
-
-    return y[revix], np.array(revix)
-
-
-def find_reversals(y, k=64):
-    """Return reversals (peaks and valleys) and indices of reversals in `y`.
-
-    The data points in the dataseries `y` are classified into `k` constant
-    sized intervals and then peak-valley filtered to yield the successive
-    extremas of the dataseries `y`.
-
-    Arguments
-    ---------
-    y : 1darray
-        Dataseries containing the signal to find the reversals for.
-    k : int
-        The number of intervals to divide the min-max range of the dataseries
-        into.
-
-    Returns
-    -------
-    reversals : 1darray
-        The reversals of the initial data series `y`.
-    indices : 1darray
-        The indices of the initial data series `y` which corresponds to the
-        reversals.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-
-    >>> y = np.random.normal(size=100000) * 10.
-
-    The reversals (peaks and valleys) and corresponding indices are then obtained by
-
-    >>> reversals, indices = fatpack.find_reversals(y)
-
-    """
-
-    Y = get_load_class_boundaries(y, k)
-    dY = Y[1] - Y[0]
-
-    # Classifying points into levels
-    i = np.digitize(y, Y)
-    z = Y[0] + dY/2. + (i-1) * dY
-
-    # Find successive datapoints in each class
-    dz = z[1:]-z[:-1]
-    ix = np.argwhere(dz != 0.).ravel()
-    ix = np.append(ix, (ix[-1]+1))
-    dz1, dz2 = np.diff(z[ix][:-1]), np.diff(z[ix][1:])
-    dz = dz1 * dz2
-    revix = ix[np.argwhere(dz < 0.).ravel()+1]
-    revix = np.insert(revix, (0), ix[0])
-    if (z[revix[-1]] - z[revix[-2]])*(z[ix[-1]] - z[revix[-1]]) < 0.:
-        revix = np.append(revix, ix[-1])
-    return z[revix], np.array(revix)
-
-
-def concatenate_reversals(reversals1, reversals2):
-    """Concatenate two reversal series.
-
-    The two reversal series are concatenated in the order given in args, i.e
-    'reversal1' is  placed before 'reversal2'. The concatenation preserves
-    the peak-valley condition at the border by deleting none, one or two
-    points.
-
-    Arguments
-    ---------
-    reversals1, reversals2 : 1darray
-    The sequence reversal1 is put first, i.e before reversal2
-
-    Returns
-    -------
-    1darray
-        Sequence of reversals of the concatenated sequences.
-
-    Raises
-    ------
-    ValueError
-        If the end/beginning of inputs 'reversals1'/'reversals2' are not
-        reversals.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate two dataseries for the example
-
-    >>> y1 = np.random.normal(size=50000) * 10.
-    >>> y2 = np.random.normal(size=50000) * 10.
-
-    Find the reversals in the dataseries
-
-    >>> rev_1, ix1 = fatpack.find_reversals(y1)
-    >>> rev_2, ix2 = fatpack.find_reversals(y2)
-
-    The reversals may then be concatenated (joined) into a new
-    sequence of reversals by
-
-    >>> rev = fatpack.concatenate_reversals(rev_1, rev_2)
-
-    """
-
-    R1, R2 = reversals1, reversals2
-    dRstart, dRend, dRjoin = R2[1] - R2[0], R1[-1] - R1[-2], R2[0] - R1[-1]
-    t1, t2 = dRend*dRstart, dRend*dRjoin
-    if (t1 > 0) and (t2 < 0):
-        result = (R1, R2)
-    elif (t1 > 0) and (t2 >= 0):
-        result = (R1[:-1], R2[1:])
-    elif (t1 < 0) and (t2 >= 0):
-        result = (R1, R2[1:])
-    elif (t1 < 0) and (t2 < 0):
-        result = (R1[:-1], R2)
-    else:
-        raise ValueError(
-            "Input must be reversals, end/start value of reversals1/reversals2 repeated.")
-    return np.concatenate(result)
-
-
-def find_rainflow_cycles(reversals):
-    """Return the rainflow cycles and residue from a sequence of reversals.
-
-    Arguments
-    ---------
-    reversals : 1darray
-        An 1D-array of reversals.
-
-    Returns
-    -------
-    rainflow_cycles : 2darray
-        A (Nx2)-array where the first / second column contains the
-        starting / destination point of a rainflow cycle.
-    residue : 1darray
-        The residue of the reversal series after one pass of the rainflow
-        algorithm.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-
-    >>> y = np.random.normal(size=100000) * 10.
-
-    First we must find the reversals in the dataseries
-
-    >>> rev_1, ix1 = fatpack.find_reversals(y)
-
-    then the (closed) rainflow cycles and residual reversals are extracted
-
-    >>> cyc_1, res = fatpack.find_rainflow_cycles(rev_1)
-
-    The residual after the first pass of the rainflow algorithm contains open
-    rainflow cycles. If the dataseries y represents a repeating process, these cycles
-    are closed on the next repetition and should be included in the cycle count by
-    concatenating the reversals in the residual with itself and rainflow cycle counting
-    is applied once more. The process of extracting the rainflow cycles from the residue
-    is shown below
-
-    >>> rev_res = fatpack.concatenate_reversals(res, res)
-    >>> cyc_res, _ = fatpack.find_rainflow_cycles(rev_res)
-
-    Finally, all rainflow cycles in the original sequence is joined together in a single
-    array
-
-    >>> rainflow_cycles = np.concatenate((cyc_1, cyc_res))
-
-    """
-
-    result = []
-    residue = []
-    len_residue = 0
-    for reversal in reversals:
-        residue += [reversal]
-        len_residue += 1
-        while len_residue >= 4:
-            S0, S1, S2, S3 = residue[-4], residue[-3], residue[-2], residue[-1]
-            dS1, dS2, dS3 = fabs(S1-S0), fabs(S2-S1), fabs(S3-S2)
-            if (dS2 <= dS1) and (dS2 <= dS3):
-                result += [[S1, S2]]
-                del residue[-3]
-                del residue[-2]
-                len_residue -= 2
-            else:
-                break
-    return np.array(result), np.array(residue)
-
-
-def find_rainflow_matrix(data_array, rowbins, colbins, return_bins=False):
-    """Return the rainflowmatrix for the data in data_array
-
-    The data in the first and second column of data_array are binned into
-    the row and column of the rainflow matrix, respectively.
-
-    The classification includes the smallest bin edge, i.e if the bins are
-    strictly increasing, bin_i < bin_i+1, and the classification of value x is
-    `bin_i <= x < bin_i+1` for all bins except the rightmost bin. Data lying
-    **on** the rightmost bin edge are included in the last bin.
-
-    Arguments
-    ---------
-    data_array : 2darray
-        (N x 2) array where the first column determines the row index and the
-        second column the column index according to `rowbins` and `colbins`,
-        respectively.
-
-    rowbins, colbins : 1darray or int
-        The edges of the bins for classifying the data_array into the rainflow
-        matrix.
-        - If bins is a sequence, the values are treated as the left edges (and
-        the rightmost edge) of the bins. These arrays must increase monotonically
-        and data values outside the range of the bins are ignored.
-        - If bins is an int, a sequence is created diving the range `min`--`max`
-        of y into `bin` number of equally sized bins.
-
-    return_bins : bool, optional
-        If true, row and column bins are also returned together with the rainflow
-        matrix
-
-    Returns
-    -------
-    rfcmat : 2darray
-        Rainflow matrix corresponding to the row and colbins.
-
-    or if return_bins is True:
-
-    rowbins, colbins, rfcmat : 1darray, 1darray, 2darray
-        Rainflow matrix and the corresponding row and column bins.
-
-    Raises
-    ------
-    ValueError
-        If rowbins or colbins are not monotonic.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-
-    >>> y = np.random.normal(size=100000) * 10.
-
-    Let us create a mean-stress vs stress-range rainflow matrix,
-    start by extracting the stress-range and means from the dataseries.
-
-    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
-
-    Next create the bins to divide the stress ranges and means into
-
-    >>> bins_S = np.arange(0., 76., 1)
-    >>> bins_Sm = np.arange(-25., 26., 1.)
-
-    and establish the data array. Note that other datavectors vectors, e.g.
-    Smin and Smax, may also be used to create other data arrays and
-    resulting rainflow matrices.
-
-    >>> data_array = np.array([Sm, S]).T
-
-    Finally, establish the rainflow matrix from the data array and the
-    specified row and column bins.
-
-    >>> rfcmat = fatpack.find_rainflow_matrix(data_array, bins_Sm, bins_S)
-
-    A figure of the rainflow matrix is useful, first find the coordinates of
-    each element in the rainflow matrix
-
-    >>> X, Y = np.meshgrid(bins_Sm, bins_S, indexing='ij')
-
-    and plot the rainflow matrix with matplotlib
-
-    >>> import matplotlib.pyplot as plt
-    >>> C = plt.pcolormesh(X, Y, rfcmat)
-    >>> cbar = plt.colorbar(C)
-    >>> title = plt.title("Rainflow matrix")
-    >>> xlab = plt.xlabel("Mean stress range (MPa)")
-    >>> ylab = plt.ylabel("Stress range (MPa)")
-    >>> plt.show(block=True)
-
-    """
-
-    cc = data_array
-
-    if isinstance(rowbins, int):
-        rowbins = np.linspace(cc[:, 0].min(), cc[:, 0].max(), rowbins)
-    if isinstance(colbins, int):
-        colbins = np.linspace(cc[:, 1].min(), cc[:, 1].max(), colbins)
-    N = rowbins.size-1
-    M = colbins.size-1
-    mat = np.zeros((N, M), dtype=float)
-
-    # Find bin index of each of the cycles
-    nrows = np.digitize(cc[:, 0], rowbins)-1
-    ncols = np.digitize(cc[:, 1], colbins)-1
-
-    # Include values on the rightmost edge in the last bin
-    nrows[cc[:, 0] == rowbins[-1]] = N - 1
-    ncols[cc[:, 1] == colbins[-1]] = M - 1
-
-    # Build the rainflow matrix
-    for nr, nc in zip(nrows, ncols):
-        if (nr >= N) or (nr < 0) or (nc >= M) or (nc < 0):
-            continue
-        mat[nr, nc] += 1.
-
-    if return_bins:
-        return rowbins, colbins, mat
-    else:
-        return mat
-
-
-def find_rainflow_ranges(y, k=64, return_means=False):
-    """Returns the ranges of the complete series (incl. residue)
-
-    Returns the ranges by first determining the reversals of the dataseries
-    `y` classified into `k` loaded classes, then the cycles and residue
-    of the complete series are found by concatenating the residue after the
-    first pass of the rainflow algorithm and applying the algorithm a second
-    time.
-
-    Arguments
-    ---------
-    y : 1darray
-        Dataseries to extract rainflow ranges from.
-    k : int
-        The number of intervals to divide the min-max range of the dataseries
-        into.
-    return_means : bool
-        Return mean for each rainflow range.
-
-    Returns
-    -------
-    ranges : 1darray
-        The ranges identified by the rainflow algorithm in the dataseries.
-    means : 1darray, optional
-        The mean values for each range.
-
-    Raises
-    ------
-    ValueError
-        If no rainflow cycles are found in the sequence.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-
-    >>> y = np.random.normal(size=100000) * 10.
-
-    Rainflow ranges S and the corresponding mean values Sm found in the dataseries
-    are then obtained by
-
-    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True)
-
-    """
-
-    reversals, _ = find_reversals(y, k)
-    cycles_firstpass, residue = find_rainflow_cycles(reversals)
-    processed_residue = concatenate_reversals(residue, residue)
-    cycles_open_sequence, _ = find_rainflow_cycles(processed_residue)
-    found_cycles_firstpass = len(cycles_firstpass.shape) == 2
-    found_cycles_open_sequence = len(cycles_open_sequence.shape) == 2
-    if found_cycles_firstpass and found_cycles_open_sequence:
-        cycles = np.concatenate((cycles_firstpass, cycles_open_sequence))
-    elif found_cycles_firstpass:
-        cycles = cycles_firstpass
-    elif found_cycles_open_sequence:
-        cycles = cycles_open_sequence
-    else:
-        raise ValueError("Could not find any cycles in sequence")
-    ranges = np.abs(cycles[:, 1] - cycles[:, 0])
-    if return_means:
-        means = 0.5 * (cycles[:, 0] + cycles[:, 1])
-        return ranges, means
-    else:
-        return ranges
-
-
-def find_rainflow_ranges_strict(y, k=64, return_means=False):
-    """Returns the ranges of the complete series (incl. residue)
-
-    Returns the ranges by first determining the reversals of the dataseries
-    `y` classified into `k` load classes, then the cycles and residue
-    of the complete series are found by concatenating the residue after the
-    first pass of the rainflow algorithm and applying the algorithm a second
-    time.
-
-    Note that `find_rainflow_ranges_strict` uses
-    `find_reversals_strict`, which classify reversals that lie on the
-    load class boundary to the upper or lower load classes depending
-    on wether the reversal is a peak or valley. It is recommended to
-    use `find_rainflow_ranges` because it is faster than
-    `find_rainflow_ranges_strict` and finds virtually identical
-    results if `k` is sufficiently large.
-
-    Arguments
-    ---------
-    y : 1darray
-        Dataseries to extract rainflow ranges from.
-    k : int
-        The number of intervals to divide the min-max range of the dataseries
-        into.
-    return_means : bool
-        Return mean for each rainflow range.
-
-    Returns
-    -------
-    ranges : 1darray
-        The ranges identified by the rainflow algorithm in the dataseries.
-    means : 1darray, optional
-        The mean values for each range.
-
-    Raises
-    ------
-    ValueError
-        If no rainflow cycles are found in the sequence.
-
-    See Also
-    --------
-    find_rainflow_ranges: Faster version of this function.
-
-    """
-
-    reversals, _ = find_reversals_strict(y, k)
-    cycles_firstpass, residue = find_rainflow_cycles(reversals)
-    processed_residue = concatenate_reversals(residue, residue)
-    cycles_open_sequence, _ = find_rainflow_cycles(processed_residue)
-    found_cycles_firstpass = len(cycles_firstpass.shape) == 2
-    found_cycles_open_sequence = len(cycles_open_sequence.shape) == 2
-    if found_cycles_firstpass and found_cycles_open_sequence:
-        cycles = np.concatenate((cycles_firstpass, cycles_open_sequence))
-    elif found_cycles_firstpass:
-        cycles = cycles_firstpass
-    elif found_cycles_open_sequence:
-        cycles = cycles_open_sequence
-    else:
-        raise ValueError("Could not find any cycles in sequence")
-    ranges = np.abs(cycles[:, 1] - cycles[:, 0])
-    if return_means:
-        means = 0.5 * (cycles[:, 0] + cycles[:, 1])
-        return ranges, means
-    else:
-        return ranges
-
-
-def find_range_count(ranges, bins=10, weights=None):
-    """Return count and the values ranges (midpoint of bin).
-
-    Arguments
-    ---------
-    ranges : 1darray
-        Array with the values to be counted
-    bins : 1darray, int, optional
-        If bins is a sequence, the values are treated as the left edges (and
-        the rightmost edge) of the bins.
-        If bins is an int, a sequence is created diving the range `min`--`max`
-        of y into `bin` number of equally sized bins.
-    weights : 1darray, optional
-        Array with same size as y, can be used to account for half cycles, i.e
-        applying a weight of 0.5 to a value in yields a counting value of 0.5
-
-    Returns
-    -------
-    N, S : 1darray
-        The count and the characteristic value for the ranges.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-
-    >>> y = np.random.normal(size=100000) * 10.
-
-    Extract ranges and establish the bins.
-
-    >>> ranges = fatpack.find_rainflow_ranges(y, k=256)
-    >>> bins = np.arange(0, 76., 1)
-
-    Find range count and midpoint (average) of corresponding bin
-
-    >>> N, S = fatpack.find_range_count(ranges, bins)
-
-    A figure of the range count is useful, below a bar plot of the
-    range count is shown with matplotlib
-
-    >>> import matplotlib.pyplot as plt
-    >>> fig1 = plt.figure()
-    >>> bars = plt.bar(S, N)
-    >>> title = plt.title("Range count")
-    >>> xlab = plt.xlabel("Stress range (MPa)")
-    >>> ylab = plt.ylabel("Count (1)")
-
-    Note that the cumulative count can also be easily obtained from
-    these results
-
-    >>> fig2 = plt.figure()
-    >>> Ncum = N.sum() - np.cumsum(N)
-    >>> cumulative_plot = plt.loglog(Ncum, S)
-    >>> title = plt.title("Cumulative plot")
-    >>> xlab = plt.xlabel("Cumulative count")
-    >>> ylab = plt.ylabel("Stress range (MPa)")
-    >>> plt.show(block=True)
-
-    """
-
-    N, bns = np.histogram(ranges, bins=bins, weights=weights)
-    S = bns[:-1] + np.diff(bns) / 2.
-    return N, S
-
-
-if __name__ == "__main__":
-    import doctest
-    doctest.testmod()
+# -*- coding: utf-8 -*-
+"""
+Implementation of 4-point rainflow counting algorithm in numpy. The
+implementation and terminology is based on the following resources:
+
+    `C. Amzallag et. al. Standardization of the rainflow counting method for
+    fatigue analysis. International Journal of Fatigue, 16 (1994) 287-293`
+
+    `ISO 12110-2, Metallic materials - Fatigue testing - Variable amplitude
+     fatigue testing.`
+
+    `G. Marsh et. al. Review and application of Rainflow residue processing
+    techniques for accurate fatigue damage estimation. International Journal
+    of Fatigue, 82 (2016) 757-765`
+
+Note that there are two functions for finding the reversals.
+
+    * `find_reversals_strict` passes the example provided in ISO12110-2 by
+    ensuring that data points which fall on a load class boundary are rounded
+    upwards if the reversal is a peak and downwards if it is a valley.
+
+    * `find_reversals` classifies the data points by rounding the datapoints
+    which lies on the boundary to the lower load class. This function is more
+    efficient than the strict version, and yields practically identical results
+    if the number of load classes is set sufficiently high.
+"""
+from __future__ import (division, print_function, absolute_import,
+                        unicode_literals)
+import numpy as np
+from math import fabs
+
+__all__ = ["find_reversals", "find_rainflow_cycles", "find_rainflow_matrix",
+           "find_rainflow_ranges", "find_range_count", "concatenate_reversals"]
+
+
+def get_load_classes(y, k=64):
+    ymax, ymin = y.max(), y.min()
+    return np.linspace(ymin, ymax, k+1)
+
+
+def get_load_class_boundaries(y, k=64):
+    ymin, ymax = y.min(), y.max()
+    dy = (ymax-ymin) / (2.0*k)
+    y0 = ymin - dy
+    y1 = ymax + dy
+    return np.linspace(y0, y1, k+2)
+
+
+def find_reversals_strict(y, k=64):
+    """Return reversals (peaks and valleys) and indices of reversals in `y`.
+
+    The data points in the dataseries `y` are classified into `k` constant
+    sized intervals and then peak-valley filtered to yield the successive
+    extremas of the dataseries `y`.
+
+    The function is strict in the sense that data points which fall on a load
+    class boundary are rounded upwards if the reversal is a peak and downwards
+    to the closest load class if it is a valley.
+
+    Arguments
+    ---------
+    y : 1darray
+        Dataseries containing the signal to find the reversals for.
+    k : int
+        The number of intervals to divide the min-max range of the dataseries
+        into.
+
+    Returns
+    -------
+    reversals : 1darray
+        The reversals of the initial data series `y`.
+    indices : 1darray
+        The indices of the initial data series `y` which corresponds to the
+        reversals.
+
+    See Also
+    --------
+    find_reversals: Faster version of this function
+
+    """
+
+    y = y.copy()  # Make sure we do not change the original sequence
+    sgn = np.sign
+    Y = get_load_class_boundaries(y, k)
+    dY = Y[1] - Y[0]
+
+    # Classifying points into levels
+    for yl, yu in zip(Y[:-1], Y[1:]):
+        y[(yl < y) & (y < yu)] = (yl+yu)/2.
+
+    # Classifying points on the level boundary
+    for n, yi in enumerate(y):
+        if not np.any(yi == Y):
+            continue
+        if n > 0:
+            dy = y[n]-y[n-1]
+        else:
+            dy = y[n+1] - y[n]
+        if dy < 0.:
+            y[n] = yi - dY / 2.
+        else:
+            y[n] = yi + dY / 2.
+
+    # Remove successive datapoints in each class
+    ix = [0]
+    for n, yi in enumerate(y):
+        if n == 0:
+            continue
+        if yi != y[ix[-1]]:
+            ix.append(n)
+
+    # Peak-valley filtering
+    revix = [0]
+    for n in range(len(ix)-1):
+        if n == 0:
+            continue
+        dy1, dy2 = y[ix[n]]-y[ix[n-1]], y[ix[n+1]]-y[ix[n]]
+        if (sgn(dy1) != sgn(dy2)):
+            revix.append(ix[n])
+
+    # Peak-valley filtering of last point
+    dy1, dy2 = y[revix[-1]]-y[revix[-2]], y[ix[-1]] - y[revix[-1]]
+    if sgn(dy1) == sgn(dy2):
+        revix[-1] = ix[-1]
+    else:
+        revix.append(ix[-1])
+
+    return y[revix], np.array(revix)
+
+
+def find_reversals(y, k=64):
+    """Return reversals (peaks and valleys) and indices of reversals in `y`.
+
+    The data points in the dataseries `y` are classified into `k` constant
+    sized intervals and then peak-valley filtered to yield the successive
+    extremas of the dataseries `y`.
+
+    Arguments
+    ---------
+    y : 1darray
+        Dataseries containing the signal to find the reversals for.
+    k : int
+        The number of intervals to divide the min-max range of the dataseries
+        into.
+
+    Returns
+    -------
+    reversals : 1darray
+        The reversals of the initial data series `y`.
+    indices : 1darray
+        The indices of the initial data series `y` which corresponds to the
+        reversals.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+
+    >>> y = np.random.normal(size=100000) * 10.
+
+    The reversals (peaks and valleys) and corresponding indices are then obtained by
+
+    >>> reversals, indices = fatpack.find_reversals(y)
+
+    """
+
+    Y = get_load_class_boundaries(y, k)
+    dY = Y[1] - Y[0]
+
+    # Classifying points into levels
+    i = np.digitize(y, Y)
+    z = Y[0] + dY/2. + (i-1) * dY
+
+    # Find successive datapoints in each class
+    dz = z[1:]-z[:-1]
+    ix = np.argwhere(dz != 0.).ravel()
+    ix = np.append(ix, (ix[-1]+1))
+    dz1, dz2 = np.diff(z[ix][:-1]), np.diff(z[ix][1:])
+    dz = dz1 * dz2
+    revix = ix[np.argwhere(dz < 0.).ravel()+1]
+    revix = np.insert(revix, (0), ix[0])
+    if (z[revix[-1]] - z[revix[-2]])*(z[ix[-1]] - z[revix[-1]]) < 0.:
+        revix = np.append(revix, ix[-1])
+    return z[revix], np.array(revix)
+
+
+def concatenate_reversals(reversals1, reversals2):
+    """Concatenate two reversal series.
+
+    The two reversal series are concatenated in the order given in args, i.e
+    'reversal1' is  placed before 'reversal2'. The concatenation preserves
+    the peak-valley condition at the border by deleting none, one or two
+    points.
+
+    Arguments
+    ---------
+    reversals1, reversals2 : 1darray
+    The sequence reversal1 is put first, i.e before reversal2
+
+    Returns
+    -------
+    1darray
+        Sequence of reversals of the concatenated sequences.
+
+    Raises
+    ------
+    ValueError
+        If the end/beginning of inputs 'reversals1'/'reversals2' are not
+        reversals.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate two dataseries for the example
+
+    >>> y1 = np.random.normal(size=50000) * 10.
+    >>> y2 = np.random.normal(size=50000) * 10.
+
+    Find the reversals in the dataseries
+
+    >>> rev_1, ix1 = fatpack.find_reversals(y1)
+    >>> rev_2, ix2 = fatpack.find_reversals(y2)
+
+    The reversals may then be concatenated (joined) into a new
+    sequence of reversals by
+
+    >>> rev = fatpack.concatenate_reversals(rev_1, rev_2)
+
+    """
+
+    R1, R2 = reversals1, reversals2
+    dRstart, dRend, dRjoin = R2[1] - R2[0], R1[-1] - R1[-2], R2[0] - R1[-1]
+    t1, t2 = dRend*dRstart, dRend*dRjoin
+    if (t1 > 0) and (t2 < 0):
+        result = (R1, R2)
+    elif (t1 > 0) and (t2 >= 0):
+        result = (R1[:-1], R2[1:])
+    elif (t1 < 0) and (t2 >= 0):
+        result = (R1, R2[1:])
+    elif (t1 < 0) and (t2 < 0):
+        result = (R1[:-1], R2)
+    else:
+        raise ValueError(
+            "Input must be reversals, end/start value of reversals1/reversals2 repeated.")
+    return np.concatenate(result)
+
+
+def find_rainflow_cycles(reversals):
+    """Return the rainflow cycles and residue from a sequence of reversals.
+
+    Arguments
+    ---------
+    reversals : 1darray
+        An 1D-array of reversals.
+
+    Returns
+    -------
+    rainflow_cycles : 2darray
+        A (Nx2)-array where the first / second column contains the
+        starting / destination point of a rainflow cycle.
+    residue : 1darray
+        The residue of the reversal series after one pass of the rainflow
+        algorithm.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+
+    >>> y = np.random.normal(size=100000) * 10.
+
+    First we must find the reversals in the dataseries
+
+    >>> rev_1, ix1 = fatpack.find_reversals(y)
+
+    then the (closed) rainflow cycles and residual reversals are extracted
+
+    >>> cyc_1, res = fatpack.find_rainflow_cycles(rev_1)
+
+    The residual after the first pass of the rainflow algorithm contains open
+    rainflow cycles. If the dataseries y represents a repeating process, these cycles
+    are closed on the next repetition and should be included in the cycle count by
+    concatenating the reversals in the residual with itself and rainflow cycle counting
+    is applied once more. The process of extracting the rainflow cycles from the residue
+    is shown below
+
+    >>> rev_res = fatpack.concatenate_reversals(res, res)
+    >>> cyc_res, _ = fatpack.find_rainflow_cycles(rev_res)
+
+    Finally, all rainflow cycles in the original sequence is joined together in a single
+    array
+
+    >>> rainflow_cycles = np.concatenate((cyc_1, cyc_res))
+
+    """
+
+    result = []
+    residue = []
+    len_residue = 0
+    for reversal in reversals:
+        residue += [reversal]
+        len_residue += 1
+        while len_residue >= 4:
+            S0, S1, S2, S3 = residue[-4], residue[-3], residue[-2], residue[-1]
+            dS1, dS2, dS3 = fabs(S1-S0), fabs(S2-S1), fabs(S3-S2)
+            if (dS2 <= dS1) and (dS2 <= dS3):
+                result += [[S1, S2]]
+                del residue[-3]
+                del residue[-2]
+                len_residue -= 2
+            else:
+                break
+    return np.array(result), np.array(residue)
+
+
+def find_rainflow_matrix(data_array, rowbins, colbins, counts=None, 
+                         return_bins=False):
+    """Return the rainflow matrix for the data in data_array
+
+    The data in the first and second column of data_array are binned into
+    the row and column of the rainflow matrix, respectively.
+
+    Arguments
+    ---------
+    data_array : 2darray
+        (N x 2) array where the first column determines the row index and the
+        second column the column index according to `rowbins` and `colbins`,
+        respectively.
+
+    rowbins, colbins : 1darray or int
+        The edges of the bins for classifying the data_array into the rainflow
+        matrix.
+        - If bins is a sequence, the values are treated as the left edges (and
+          the rightmost edge) of the bins. These arrays must increase 
+          monotonically and data values outside the range of the bins are 
+          ignored.
+        - If bins is an int, a sequence is created diving the range min-max
+          into `bin` number of equally sized bins.
+    
+    counts : 1darray, optional
+        Array of size (N) with counts of occurances of each data pair in data 
+        array. If `None`, one occurance of each data pair is assumed.
+
+    return_bins : bool, optional
+        If true, row and column bins are also returned together with the 
+        rainflow matrix
+
+    Returns
+    -------
+    rfcmat : 2darray
+        Rainflow matrix corresponding to the row and colbins.
+
+    or if return_bins is True:
+
+    rowbins, colbins, rfcmat : 1darray, 1darray, 2darray
+        Rainflow matrix and the corresponding row and column bins.
+
+    Raises
+    ------
+    ValueError
+        If rowbins or colbins are not monotonic.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+
+    >>> y = np.random.normal(size=100000) * 10.
+
+    Let us create a mean-stress vs stress-range rainflow matrix,
+    start by extracting the stress-range and means from the dataseries.
+
+    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
+
+    Next create the bins to divide the stress ranges and means into
+
+    >>> bins_S = np.arange(0., 76., 1)
+    >>> bins_Sm = np.arange(-25., 26., 1.)
+
+    and establish the data array. Note that other datavectors vectors, e.g.
+    Smin and Smax, may also be used to create other data arrays and
+    resulting rainflow matrices.
+
+    >>> data_array = np.array([Sm, S]).T
+
+    Finally, establish the rainflow matrix from the data array and the
+    specified row and column bins.
+
+    >>> rfcmat = fatpack.find_rainflow_matrix(data_array, bins_Sm, bins_S)
+
+    A figure of the rainflow matrix is useful, first find the coordinates of
+    each element in the rainflow matrix
+
+    >>> X, Y = np.meshgrid(bins_Sm, bins_S, indexing='ij')
+
+    and plot the rainflow matrix with matplotlib
+
+    >>> import matplotlib.pyplot as plt
+    >>> C = plt.pcolormesh(X, Y, rfcmat)
+    >>> cbar = plt.colorbar(C)
+    >>> title = plt.title("Rainflow matrix")
+    >>> xlab = plt.xlabel("Mean stress range (MPa)")
+    >>> ylab = plt.ylabel("Stress range (MPa)")
+    >>> plt.show(block=True)
+
+    """
+    Srow = data_array[:, 0]
+    Scol = data_array[:, 1]
+
+    if isinstance(rowbins, int):
+        rowbins = np.linspace(Srow.min(), Srow.max(), rowbins)
+    if isinstance(colbins, int):
+        colbins = np.linspace(Scol.min(), Scol.max(), colbins)
+    mat, _, _ = np.histogram2d(Srow, Scol, [rowbins, colbins], 
+                               weights=counts)
+
+    if return_bins:
+        return rowbins, colbins, mat
+    else:
+        return mat
+
+
+def find_rainflow_ranges(y, k=64, return_means=False):
+    """Returns the ranges of the complete series (incl. residue)
+
+    Returns the ranges by first determining the reversals of the dataseries
+    `y` classified into `k` loaded classes, then the cycles and residue
+    of the complete series are found by concatenating the residue after the
+    first pass of the rainflow algorithm and applying the algorithm a second
+    time.
+
+    Arguments
+    ---------
+    y : 1darray
+        Dataseries to extract rainflow ranges from.
+    k : int
+        The number of intervals to divide the min-max range of the dataseries
+        into.
+    return_means : bool
+        Return mean for each rainflow range.
+
+    Returns
+    -------
+    ranges : 1darray
+        The ranges identified by the rainflow algorithm in the dataseries.
+    means : 1darray, optional
+        The mean values for each range.
+
+    Raises
+    ------
+    ValueError
+        If no rainflow cycles are found in the sequence.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+
+    >>> y = np.random.normal(size=100000) * 10.
+
+    Rainflow ranges S and the corresponding mean values Sm found in the dataseries
+    are then obtained by
+
+    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True)
+
+    """
+
+    reversals, _ = find_reversals(y, k)
+    cycles_firstpass, residue = find_rainflow_cycles(reversals)
+    processed_residue = concatenate_reversals(residue, residue)
+    cycles_open_sequence, _ = find_rainflow_cycles(processed_residue)
+    found_cycles_firstpass = len(cycles_firstpass.shape) == 2
+    found_cycles_open_sequence = len(cycles_open_sequence.shape) == 2
+    if found_cycles_firstpass and found_cycles_open_sequence:
+        cycles = np.concatenate((cycles_firstpass, cycles_open_sequence))
+    elif found_cycles_firstpass:
+        cycles = cycles_firstpass
+    elif found_cycles_open_sequence:
+        cycles = cycles_open_sequence
+    else:
+        raise ValueError("Could not find any cycles in sequence")
+    ranges = np.abs(cycles[:, 1] - cycles[:, 0])
+    if return_means:
+        means = 0.5 * (cycles[:, 0] + cycles[:, 1])
+        return ranges, means
+    else:
+        return ranges
+
+
+def find_rainflow_ranges_strict(y, k=64, return_means=False):
+    """Returns the ranges of the complete series (incl. residue)
+
+    Returns the ranges by first determining the reversals of the dataseries
+    `y` classified into `k` load classes, then the cycles and residue
+    of the complete series are found by concatenating the residue after the
+    first pass of the rainflow algorithm and applying the algorithm a second
+    time.
+
+    Note that `find_rainflow_ranges_strict` uses
+    `find_reversals_strict`, which classify reversals that lie on the
+    load class boundary to the upper or lower load classes depending
+    on wether the reversal is a peak or valley. It is recommended to
+    use `find_rainflow_ranges` because it is faster than
+    `find_rainflow_ranges_strict` and finds virtually identical
+    results if `k` is sufficiently large.
+
+    Arguments
+    ---------
+    y : 1darray
+        Dataseries to extract rainflow ranges from.
+    k : int
+        The number of intervals to divide the min-max range of the dataseries
+        into.
+    return_means : bool
+        Return mean for each rainflow range.
+
+    Returns
+    -------
+    ranges : 1darray
+        The ranges identified by the rainflow algorithm in the dataseries.
+    means : 1darray, optional
+        The mean values for each range.
+
+    Raises
+    ------
+    ValueError
+        If no rainflow cycles are found in the sequence.
+
+    See Also
+    --------
+    find_rainflow_ranges: Faster version of this function.
+
+    """
+
+    reversals, _ = find_reversals_strict(y, k)
+    cycles_firstpass, residue = find_rainflow_cycles(reversals)
+    processed_residue = concatenate_reversals(residue, residue)
+    cycles_open_sequence, _ = find_rainflow_cycles(processed_residue)
+    found_cycles_firstpass = len(cycles_firstpass.shape) == 2
+    found_cycles_open_sequence = len(cycles_open_sequence.shape) == 2
+    if found_cycles_firstpass and found_cycles_open_sequence:
+        cycles = np.concatenate((cycles_firstpass, cycles_open_sequence))
+    elif found_cycles_firstpass:
+        cycles = cycles_firstpass
+    elif found_cycles_open_sequence:
+        cycles = cycles_open_sequence
+    else:
+        raise ValueError("Could not find any cycles in sequence")
+    ranges = np.abs(cycles[:, 1] - cycles[:, 0])
+    if return_means:
+        means = 0.5 * (cycles[:, 0] + cycles[:, 1])
+        return ranges, means
+    else:
+        return ranges
+
+
+def find_range_count(ranges, bins=10, weights=None):
+    """Return count and the values ranges (midpoint of bin).
+
+    Arguments
+    ---------
+    ranges : 1darray
+        Array with the values to be counted
+    bins : 1darray, int, optional
+        If bins is a sequence, the values are treated as the left edges (and
+        the rightmost edge) of the bins.
+        If bins is an int, a sequence is created diving the range `min`--`max`
+        of y into `bin` number of equally sized bins.
+    weights : 1darray, optional
+        Array with same size as y, can be used to account for half cycles, i.e
+        applying a weight of 0.5 to a value in yields a counting value of 0.5
+
+    Returns
+    -------
+    N, S : 1darray
+        The count and the characteristic value for the ranges.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+
+    >>> y = np.random.normal(size=100000) * 10.
+
+    Extract ranges and establish the bins.
+
+    >>> ranges = fatpack.find_rainflow_ranges(y, k=256)
+    >>> bins = np.arange(0, 76., 1)
+
+    Find range count and midpoint (average) of corresponding bin
+
+    >>> N, S = fatpack.find_range_count(ranges, bins)
+
+    A figure of the range count is useful, below a bar plot of the
+    range count is shown with matplotlib
+
+    >>> import matplotlib.pyplot as plt
+    >>> fig1 = plt.figure()
+    >>> bars = plt.bar(S, N)
+    >>> title = plt.title("Range count")
+    >>> xlab = plt.xlabel("Stress range (MPa)")
+    >>> ylab = plt.ylabel("Count (1)")
+
+    Note that the cumulative count can also be easily obtained from
+    these results
+
+    >>> fig2 = plt.figure()
+    >>> Ncum = N.sum() - np.cumsum(N)
+    >>> cumulative_plot = plt.loglog(Ncum, S)
+    >>> title = plt.title("Cumulative plot")
+    >>> xlab = plt.xlabel("Cumulative count")
+    >>> ylab = plt.ylabel("Stress range (MPa)")
+    >>> plt.show(block=True)
+
+    """
+
+    N, bns = np.histogram(ranges, bins=bins, weights=weights)
+    S = bns[:-1] + np.diff(bns) / 2.
+    return N, S
+
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `fatpack-0.7.3/fatpack/stresscorrection.py` & `fatpack-0.7.5/fatpack/stresscorrection.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-# -*- coding: utf-8 -*-
-"""
-Implementation of stress correction methods for stress-life
-analysis. The implementation is based on the following resources:
-
-    `N. E. Dowling et. al. Mean Stress Effects in Stress-Life Fatigue and
-    the Walker Equation. Fatigue & Fracture of Engineering Materials &
-    Structures, 32 (2009) 163-179`
-
-    `DNV GL AS, RP-C203 Fatigue Design of Offshore Steel Structures.
-    (2016)`
-
-    `CEN/TC250, Eurocode 3: Design of Steel Structures. Part 1-9:
-    Fatigue. EN 1993-1-9. (2005)`
-"""
-from __future__ import (division, print_function, absolute_import,
-                        unicode_literals)
-import abc
-import numpy as np
-
-
-__all__ = [
-    "find_walker_equivalent_stress",
-    "find_swt_equivalent_stress",
-    "find_morrow_equivalent_stress",
-    "find_goodman_equivalent_stress",
-    "find_reduced_compressive_stress",
-    ]
-
-
-def find_walker_equivalent_stress(S, Sm, gamma):
-    """Walker mean stress corrector for fatigue life analysis.
-
-    Walker mean stress corrector introduces a material factor gamma
-    and transforms the stress range S at mean stress Sm to a equivalen
-    zero mean stress range St.
-
-    Arguments
-    ---------
-    S : 1darray
-        Stress ranges
-    Sm : 1darray
-        Mean stress of stress ranges
-    gamma : float
-        Material factor for Walker mean stress correction.
-
-    Returns
-    -------
-    1darray
-        Equivalent zero mean stress range
-
-    Raises
-    ------
-    ValueError
-        SWT and Walker stress correction not defined for Smax < 0,
-        i.e. purely compressive stress ranges.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-    
-    >>> y = np.random.normal(size=100000) * 10. + 15.
-
-    Let us create a mean-stress vs stress-range rainflow matrix,
-    start by extracting the stress-range and means from the dataseries.
-
-    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
-
-    Remove purely compressive stress ranges
-
-    >>> Smax = Sm + S / 2.
-    >>> mask = (Smax > 0.)
-    >>> S, Sm = S[mask], Sm[mask]
-
-    Now, we can determine the equivalent zero mean stress range assuming
-    gamma=0.4
-
-    >>> St = fatpack.find_walker_equivalent_stress(S, Sm, 0.4)
-
-    and then we can calculate the damage for the transformed equivalent stress 
-    with the help of an endurance curve.
-
-    >>> curve = fatpack.LinearEnduranceCurve(90.)
-    >>> Dcorr = curve.find_miner_sum(St)
-
-    """
-    Smax = Sm + S / 2.
-    if np.any(Smax<=0.):
-        raise ValueError("SWT and Walker stress correction not defined for Smax <= 0")
-    return (2*Sm + S)**(1-gamma) * S**gamma
-
-
-def find_swt_equivalent_stress(S, Sm):
-    """SWT mean stress corrector for fatigue life analysis.
-
-    Smith, Watson and Topper (SWT) mean stress corrector is a special
-    case of the Walker mean stress corrector (gamma=0.5). SWT only
-    relies on the stress state and is therefore simpler in use than
-    many of the other stress corrector methods.
-
-    Arguments
-    ---------
-    S : 1darray
-        Stress ranges
-    Sm : 1darray
-        Mean stress of stress ranges
-
-    Returns
-    -------
-    1darray
-        Equivalent zero mean stress range
-
-    Raises
-    ------
-    ValueError
-        SWT and Walker stress correction not defined for Smax < 0,
-        i.e. purely compressive stress ranges.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-    
-    >>> y = np.random.normal(size=100000) * 10. + 15.
-
-    Let us create a mean-stress vs stress-range rainflow matrix,
-    start by extracting the stress-range and means from the dataseries.
-
-    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
-
-    Remove purely compressive stress ranges
-
-    >>> Smax = Sm + S / 2.
-    >>> mask = (Smax > 0.)
-    >>> S, Sm = S[mask], Sm[mask]
-
-    Now, we can determine the equivalent zero mean stress range
-
-    >>> St = fatpack.find_swt_equivalent_stress(S, Sm, 0.4)
-
-    and then we can calculate the damage for the transformed equivalent stress 
-    with the help of an endurance curve.
-
-    >>> curve = fatpack.LinearEnduranceCurve(90.)
-    >>> Dcorr = curve.find_miner_sum(St)
-    
-    """
-    return find_walker_equivalent_stress(S, Sm, 0.5)
-
-
-def find_morrow_equivalent_stress(S, Sm, sf):
-    """Morrow mean stress corrector for fatigue life analysis.
-
-    Morrow mean stress corrector uses the true fracture strength of
-    the material and transforms the stress range S at mean stress Sm
-    to a equivalent zero mean stress range St.
-
-    Arguments
-    ---------
-    S : 1darray
-        Stress ranges
-    Sm : 1darray
-        Mean stress of stress ranges
-    sf : float
-        True fracture strength of material, also equivalent to the
-        stress amplitude at 1/2 cycle of a stress endurance curve for
-        some materials.
-
-    Returns
-    -------
-    1darray
-        Equivalent zero mean stress range
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-    
-    >>> y = np.random.normal(size=100000) * 10. + 15.
-
-    Let us create a mean-stress vs stress-range rainflow matrix,
-    start by extracting the stress-range and means from the dataseries.
-
-    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
-
-    Now, we can determine the equivalent zero mean stress range assuming
-    fracture strength of 800 MPa
-
-    >>> St = fatpack.find_morrow_equivalent_stress(S, Sm, 800.)
-
-    and then we can calculate the damage for the transformed equivalent stress 
-    with the help of an endurance curve.
-
-    >>> curve = fatpack.LinearEnduranceCurve(90.)
-    >>> Dcorr = curve.find_miner_sum(St)
-    
-    """
-    return S / (1 - Sm / sf)
-
-
-def find_goodman_equivalent_stress(S, Sm, su):
-    """Goodman mean stress corrector for fatigue life analysis.
-
-    Goodman mean stress corrector uses the ultimate strength of the
-    material and transforms the stress range S at mean stress Sm to a
-    equivalent zero mean stress range St.
-
-    Arguments
-    ---------
-    S : 1darray
-        Stress ranges
-    Sm : 1darray
-        Mean stress of stress ranges
-    su : float
-        Ultimate strength of material.
-
-    Returns
-    -------
-    1darray
-        Equivalent zero mean stress range
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-    
-    >>> y = np.random.normal(size=100000) * 10. + 15.
-
-    Let us create a mean-stress vs stress-range rainflow matrix,
-    start by extracting the stress-range and means from the dataseries.
-
-    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
-
-    Now, we can determine the equivalent zero mean stress range assuming
-    ultimate strength of 500 MPa
-
-    >>> St = fatpack.find_goodman_equivalent_stress(S, Sm, 500.)
-
-    and then we can calculate the damage for the transformed equivalent stress 
-    with the help of an endurance curve.
-
-    >>> curve = fatpack.LinearEnduranceCurve(90.)
-    >>> Dcorr = curve.find_miner_sum(St)
-    
-    """
-    return find_morrow_equivalent_stress(S, Sm, su)
-
-
-def find_reduced_compressive_stress(S, Sm, alpha):
-    """Direct compressive stress correction for fatigue life analysis.
-
-    Compressive stress correction reduces the compressive part of the
-    stress range by a factor (alpha).
-
-    Arguments
-    ---------
-    S : 1darray
-        Stress ranges
-    Sm : 1darray
-        Mean stress of stress ranges
-    alpha : float
-        Reduction factor for the compressive part of stress range.
-
-    Returns
-    -------
-    1darray
-        Transformed stress range with reduced compressive stress of
-        original stress range.
-
-    Example
-    -------
-    >>> import fatpack
-    >>> import numpy as np
-    >>> np.random.seed(10)
-
-    Generate a dataseries for the example
-    
-    >>> y = np.random.normal(size=100000) * 10. + 15.
-
-    Let us create a mean-stress vs stress-range rainflow matrix,
-    start by extracting the stress-range and means from the dataseries.
-
-    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
-
-    Now, we can determine the equivalent zero mean stress range assuming
-    reduction factor of 60 %
-
-    >>> St = fatpack.find_reduced_compressive_stress(S, Sm, 0.6)
-
-    and then we can calculate the damage for the transformed equivalent stress 
-    with the help of an endurance curve.
-
-    >>> curve = fatpack.LinearEnduranceCurve(90.)
-    >>> Dcorr = curve.find_miner_sum(St)
-    
-    """
-    St = S.copy()
-    Sa = S/2
-    mask = Sm<Sa
-    St[mask] = (1-alpha)*Sm[mask] + (1+alpha)*Sa[mask]
-    return St
-
-
-if __name__ == '__main__':
-    pass
+# -*- coding: utf-8 -*-
+"""
+Implementation of stress correction methods for stress-life
+analysis. The implementation is based on the following resources:
+
+    `N. E. Dowling et. al. Mean Stress Effects in Stress-Life Fatigue and
+    the Walker Equation. Fatigue & Fracture of Engineering Materials &
+    Structures, 32 (2009) 163-179`
+
+    `DNV GL AS, RP-C203 Fatigue Design of Offshore Steel Structures.
+    (2016)`
+
+    `CEN/TC250, Eurocode 3: Design of Steel Structures. Part 1-9:
+    Fatigue. EN 1993-1-9. (2005)`
+"""
+from __future__ import (division, print_function, absolute_import,
+                        unicode_literals)
+import abc
+import numpy as np
+
+
+__all__ = [
+    "find_walker_equivalent_stress",
+    "find_swt_equivalent_stress",
+    "find_morrow_equivalent_stress",
+    "find_goodman_equivalent_stress",
+    "find_reduced_compressive_stress",
+    ]
+
+
+def find_walker_equivalent_stress(S, Sm, gamma):
+    """Walker mean stress corrector for fatigue life analysis.
+
+    Walker mean stress corrector introduces a material factor gamma
+    and transforms the stress range S at mean stress Sm to a equivalen
+    zero mean stress range St.
+
+    Arguments
+    ---------
+    S : 1darray
+        Stress ranges
+    Sm : 1darray
+        Mean stress of stress ranges
+    gamma : float
+        Material factor for Walker mean stress correction.
+
+    Returns
+    -------
+    1darray
+        Equivalent zero mean stress range
+
+    Raises
+    ------
+    ValueError
+        SWT and Walker stress correction not defined for Smax < 0,
+        i.e. purely compressive stress ranges.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+    
+    >>> y = np.random.normal(size=100000) * 10. + 15.
+
+    Let us create a mean-stress vs stress-range rainflow matrix,
+    start by extracting the stress-range and means from the dataseries.
+
+    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
+
+    Remove purely compressive stress ranges
+
+    >>> Smax = Sm + S / 2.
+    >>> mask = (Smax > 0.)
+    >>> S, Sm = S[mask], Sm[mask]
+
+    Now, we can determine the equivalent zero mean stress range assuming
+    gamma=0.4
+
+    >>> St = fatpack.find_walker_equivalent_stress(S, Sm, 0.4)
+
+    and then we can calculate the damage for the transformed equivalent stress 
+    with the help of an endurance curve.
+
+    >>> curve = fatpack.LinearEnduranceCurve(90.)
+    >>> Dcorr = curve.find_miner_sum(St)
+
+    """
+    Smax = Sm + S / 2.
+    if np.any(Smax<=0.):
+        raise ValueError("SWT and Walker stress correction not defined for Smax <= 0")
+    return (2*Sm + S)**(1-gamma) * S**gamma
+
+
+def find_swt_equivalent_stress(S, Sm):
+    """SWT mean stress corrector for fatigue life analysis.
+
+    Smith, Watson and Topper (SWT) mean stress corrector is a special
+    case of the Walker mean stress corrector (gamma=0.5). SWT only
+    relies on the stress state and is therefore simpler in use than
+    many of the other stress corrector methods.
+
+    Arguments
+    ---------
+    S : 1darray
+        Stress ranges
+    Sm : 1darray
+        Mean stress of stress ranges
+
+    Returns
+    -------
+    1darray
+        Equivalent zero mean stress range
+
+    Raises
+    ------
+    ValueError
+        SWT and Walker stress correction not defined for Smax < 0,
+        i.e. purely compressive stress ranges.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+    
+    >>> y = np.random.normal(size=100000) * 10. + 15.
+
+    Let us create a mean-stress vs stress-range rainflow matrix,
+    start by extracting the stress-range and means from the dataseries.
+
+    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
+
+    Remove purely compressive stress ranges
+
+    >>> Smax = Sm + S / 2.
+    >>> mask = (Smax > 0.)
+    >>> S, Sm = S[mask], Sm[mask]
+
+    Now, we can determine the equivalent zero mean stress range
+
+    >>> St = fatpack.find_swt_equivalent_stress(S, Sm, 0.4)
+
+    and then we can calculate the damage for the transformed equivalent stress 
+    with the help of an endurance curve.
+
+    >>> curve = fatpack.LinearEnduranceCurve(90.)
+    >>> Dcorr = curve.find_miner_sum(St)
+    
+    """
+    return find_walker_equivalent_stress(S, Sm, 0.5)
+
+
+def find_morrow_equivalent_stress(S, Sm, sf):
+    """Morrow mean stress corrector for fatigue life analysis.
+
+    Morrow mean stress corrector uses the true fracture strength of
+    the material and transforms the stress range S at mean stress Sm
+    to a equivalent zero mean stress range St.
+
+    Arguments
+    ---------
+    S : 1darray
+        Stress ranges
+    Sm : 1darray
+        Mean stress of stress ranges
+    sf : float
+        True fracture strength of material, also equivalent to the
+        stress amplitude at 1/2 cycle of a stress endurance curve for
+        some materials.
+
+    Returns
+    -------
+    1darray
+        Equivalent zero mean stress range
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+    
+    >>> y = np.random.normal(size=100000) * 10. + 15.
+
+    Let us create a mean-stress vs stress-range rainflow matrix,
+    start by extracting the stress-range and means from the dataseries.
+
+    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
+
+    Now, we can determine the equivalent zero mean stress range assuming
+    fracture strength of 800 MPa
+
+    >>> St = fatpack.find_morrow_equivalent_stress(S, Sm, 800.)
+
+    and then we can calculate the damage for the transformed equivalent stress 
+    with the help of an endurance curve.
+
+    >>> curve = fatpack.LinearEnduranceCurve(90.)
+    >>> Dcorr = curve.find_miner_sum(St)
+    
+    """
+    return S / (1 - Sm / sf)
+
+
+def find_goodman_equivalent_stress(S, Sm, su):
+    """Goodman mean stress corrector for fatigue life analysis.
+
+    Goodman mean stress corrector uses the ultimate strength of the
+    material and transforms the stress range S at mean stress Sm to a
+    equivalent zero mean stress range St.
+
+    Arguments
+    ---------
+    S : 1darray
+        Stress ranges
+    Sm : 1darray
+        Mean stress of stress ranges
+    su : float
+        Ultimate strength of material.
+
+    Returns
+    -------
+    1darray
+        Equivalent zero mean stress range
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+    
+    >>> y = np.random.normal(size=100000) * 10. + 15.
+
+    Let us create a mean-stress vs stress-range rainflow matrix,
+    start by extracting the stress-range and means from the dataseries.
+
+    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
+
+    Now, we can determine the equivalent zero mean stress range assuming
+    ultimate strength of 500 MPa
+
+    >>> St = fatpack.find_goodman_equivalent_stress(S, Sm, 500.)
+
+    and then we can calculate the damage for the transformed equivalent stress 
+    with the help of an endurance curve.
+
+    >>> curve = fatpack.LinearEnduranceCurve(90.)
+    >>> Dcorr = curve.find_miner_sum(St)
+    
+    """
+    return find_morrow_equivalent_stress(S, Sm, su)
+
+
+def find_reduced_compressive_stress(S, Sm, alpha):
+    """Direct compressive stress correction for fatigue life analysis.
+
+    Compressive stress correction reduces the compressive part of the
+    stress range by a factor (alpha).
+
+    Arguments
+    ---------
+    S : 1darray
+        Stress ranges
+    Sm : 1darray
+        Mean stress of stress ranges
+    alpha : float
+        Reduction factor for the compressive part of stress range.
+
+    Returns
+    -------
+    1darray
+        Transformed stress range with reduced compressive stress of
+        original stress range.
+
+    Example
+    -------
+    >>> import fatpack
+    >>> import numpy as np
+    >>> np.random.seed(10)
+
+    Generate a dataseries for the example
+    
+    >>> y = np.random.normal(size=100000) * 10. + 15.
+
+    Let us create a mean-stress vs stress-range rainflow matrix,
+    start by extracting the stress-range and means from the dataseries.
+
+    >>> S, Sm = fatpack.find_rainflow_ranges(y, return_means=True, k=256)
+
+    Now, we can determine the equivalent zero mean stress range assuming
+    reduction factor of 60 %
+
+    >>> St = fatpack.find_reduced_compressive_stress(S, Sm, 0.6)
+
+    and then we can calculate the damage for the transformed equivalent stress 
+    with the help of an endurance curve.
+
+    >>> curve = fatpack.LinearEnduranceCurve(90.)
+    >>> Dcorr = curve.find_miner_sum(St)
+    
+    """
+    St = S.copy()
+    Sa = S/2
+    mask = Sm<Sa
+    St[mask] = (1-alpha)*Sm[mask] + (1+alpha)*Sa[mask]
+    return St
+
+
+if __name__ == '__main__':
+    pass
```

