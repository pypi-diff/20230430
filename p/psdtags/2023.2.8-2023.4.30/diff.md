# Comparing `tmp/psdtags-2023.2.8.tar.gz` & `tmp/psdtags-2023.4.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdtags-2023.2.8.tar", last modified: Wed Feb  8 20:13:05 2023, max compression
+gzip compressed data, was "psdtags-2023.4.30.tar", last modified: Sun Apr 30 05:33:29 2023, max compression
```

## Comparing `psdtags-2023.2.8.tar` & `psdtags-2023.4.30.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 20:13:05.101364 psdtags-2023.2.8/
--rw-rw-rw-   0        0        0     1559 2023-02-08 20:13:02.000000 psdtags-2023.2.8/LICENSE
--rw-rw-rw-   0        0        0      412 2023-02-08 00:12:46.000000 psdtags-2023.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5397 2023-02-08 20:13:05.101364 psdtags-2023.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     4482 2023-02-08 20:13:02.000000 psdtags-2023.2.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-08 20:13:05.085708 psdtags-2023.2.8/examples/
--rw-rw-rw-   0        0        0     9931 2023-02-08 20:01:33.000000 psdtags-2023.2.8/examples/layered_tiff.py
--rw-rw-rw-   0        0        0     1685 2023-02-08 17:59:20.000000 psdtags-2023.2.8/examples/product.png
--rw-rw-rw-   0        0        0     2368 2023-02-08 18:00:10.000000 psdtags-2023.2.8/examples/reflection.png
--rw-rw-rw-   0        0        0      875 2023-02-08 17:59:29.000000 psdtags-2023.2.8/examples/shadow.png
-drwxrwxrwx   0        0        0        0 2023-02-08 20:13:05.085708 psdtags-2023.2.8/psdtags/
--rw-rw-rw-   0        0        0      101 2022-01-14 16:45:21.000000 psdtags-2023.2.8/psdtags/__init__.py
--rw-rw-rw-   0        0        0      132 2022-01-14 16:45:31.000000 psdtags-2023.2.8/psdtags/__main__.py
--rw-rw-rw-   0        0        0   116790 2023-02-08 20:09:40.000000 psdtags-2023.2.8/psdtags/psdtags.py
-drwxrwxrwx   0        0        0        0 2023-02-08 20:13:05.101364 psdtags-2023.2.8/psdtags.egg-info/
--rw-rw-rw-   0        0        0     5397 2023-02-08 20:13:03.000000 psdtags-2023.2.8/psdtags.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-02-08 20:13:04.000000 psdtags-2023.2.8/psdtags.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 20:13:03.000000 psdtags-2023.2.8/psdtags.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-02-08 20:13:03.000000 psdtags-2023.2.8/psdtags.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-02-08 20:13:03.000000 psdtags-2023.2.8/psdtags.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-08 20:13:03.000000 psdtags-2023.2.8/psdtags.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-08 20:13:05.101364 psdtags-2023.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2426 2023-02-08 20:12:09.000000 psdtags-2023.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:33:29.781501 psdtags-2023.4.30/
+-rw-rw-rw-   0        0        0     1559 2023-04-30 05:33:23.000000 psdtags-2023.4.30/LICENSE
+-rw-rw-rw-   0        0        0      412 2023-02-08 00:12:46.000000 psdtags-2023.4.30/MANIFEST.in
+-rw-rw-rw-   0        0        0     5854 2023-04-30 05:33:29.779523 psdtags-2023.4.30/PKG-INFO
+-rw-rw-rw-   0        0        0     4989 2023-04-30 05:33:23.000000 psdtags-2023.4.30/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 05:33:29.768753 psdtags-2023.4.30/examples/
+-rw-rw-rw-   0        0        0     9931 2023-02-08 20:01:33.000000 psdtags-2023.4.30/examples/layered_tiff.py
+-rw-rw-rw-   0        0        0     1685 2023-02-08 17:59:20.000000 psdtags-2023.4.30/examples/product.png
+-rw-rw-rw-   0        0        0     2368 2023-02-08 18:00:10.000000 psdtags-2023.4.30/examples/reflection.png
+-rw-rw-rw-   0        0        0      875 2023-02-08 17:59:29.000000 psdtags-2023.4.30/examples/shadow.png
+drwxrwxrwx   0        0        0        0 2023-04-30 05:33:29.771754 psdtags-2023.4.30/psdtags/
+-rw-rw-rw-   0        0        0      101 2022-01-14 16:45:21.000000 psdtags-2023.4.30/psdtags/__init__.py
+-rw-rw-rw-   0        0        0      132 2022-01-14 16:45:31.000000 psdtags-2023.4.30/psdtags/__main__.py
+-rw-rw-rw-   0        0        0   124090 2023-04-30 04:37:07.000000 psdtags-2023.4.30/psdtags/psdtags.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:33:29.778522 psdtags-2023.4.30/psdtags.egg-info/
+-rw-rw-rw-   0        0        0     5854 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-04-30 05:33:29.000000 psdtags-2023.4.30/psdtags.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 05:33:28.000000 psdtags-2023.4.30/psdtags.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 05:33:29.782522 psdtags-2023.4.30/setup.cfg
+-rw-rw-rw-   0        0        0     2273 2023-04-30 04:56:40.000000 psdtags-2023.4.30/setup.py
```

### Comparing `psdtags-2023.2.8/LICENSE` & `psdtags-2023.4.30/LICENSE`

 * *Files identical despite different names*

### Comparing `psdtags-2023.2.8/PKG-INFO` & `psdtags-2023.4.30/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: psdtags
-Version: 2023.2.8
+Version: 2023.4.30
 Summary: Read and write layered TIFF ImageSourceData and ImageResources tags
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psdtags/issues
 Project-URL: Source Code, https://github.com/cgohlke/psdtags
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
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
 
@@ -28,24 +27,25 @@
 Psdtags is a Python library to read and write the Adobe Photoshop(r) specific
 ImageResources (#34377) and ImageSourceData (#37724) TIFF tags, which contain
 image resource blocks, layer and mask information found in a typical layered
 TIFF file created by Photoshop.
 
 The format is specified in the
 `Adobe Photoshop TIFF Technical Notes (March 22, 2002)
-<https://www.adobe.io/open/standards/TIFF.html>`_
+<https://www.awaresystems.be/imaging/tiff/specification/TIFFphotoshop.pdf>`_
 and
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.2.8
+:Version: 2023.4.30
+:DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
 
@@ -62,23 +62,36 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.10, 3.11.2 <https://www.python.org>`_
-- `NumPy 1.23.5 <https://pypi.org/project/numpy/>`_
-- `Imagecodecs 2023.1.23 <https://pypi.org/project/imagecodecs/>`_ (optional)
-- `Tifffile 2023.2.3 <https://pypi.org/project/tifffile/>`_  (optional)
-- `Matplotlib 3.6.3 <https://pypi.org/project/matplotlib/>`_  (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
+  (required for compressing/decompressing image data)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12
+  (required for reading/writing tags from/to TIFF files)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+  (required for plotting)
 
 Revisions
 ---------
 
+2023.4.30
+
+- Few API changes (breaking).
+- Improve object repr.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
+2023.2.18
+
+- Allow unknown PsdKeys (#5).
+
 2023.2.8
 
 - Change PsdPoint and PsdReferencePoint signatures (breaking).
 - Add helper function to create composite from layers.
 
 2022.8.25
 
@@ -111,15 +124,15 @@
 - Initial release.
 
 Notes
 -----
 
 The API is not stable yet and might change between revisions.
 
-This module has been tested with a limited number of files only.
+This library has been tested with a limited number of files only.
 
 Additional layer information is not yet supported.
 
 Consider `psd-tools <https://github.com/psd-tools/psd-tools>`_ and
 `pytoshop <https://github.com/mdboom/pytoshop>`_  for working with
 Adobe Photoshop PSD files.
 
@@ -171,7 +184,10 @@
 >>> assert isd == TiffImageSourceData.fromtiff('_layered.tif')
 >>> assert res == TiffImageResources.fromtiff('_layered.tif')
 
 View the layer and mask information as well as the image resource blocks in
 a layered TIFF file from a command line::
 
     python -m psdtags layered.tif
+
+Refer to the `layered_tiff.py` example in the source distribution for
+creating a layered TIFF file from individual layer images.
```

### Comparing `psdtags-2023.2.8/README.rst` & `psdtags-2023.4.30/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 Psdtags is a Python library to read and write the Adobe Photoshop(r) specific
 ImageResources (#34377) and ImageSourceData (#37724) TIFF tags, which contain
 image resource blocks, layer and mask information found in a typical layered
 TIFF file created by Photoshop.
 
 The format is specified in the
 `Adobe Photoshop TIFF Technical Notes (March 22, 2002)
-<https://www.adobe.io/open/standards/TIFF.html>`_
+<https://www.awaresystems.be/imaging/tiff/specification/TIFFphotoshop.pdf>`_
 and
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.2.8
+:Version: 2023.4.30
+:DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
 
@@ -38,23 +39,36 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.10, 3.11.2 <https://www.python.org>`_
-- `NumPy 1.23.5 <https://pypi.org/project/numpy/>`_
-- `Imagecodecs 2023.1.23 <https://pypi.org/project/imagecodecs/>`_ (optional)
-- `Tifffile 2023.2.3 <https://pypi.org/project/tifffile/>`_  (optional)
-- `Matplotlib 3.6.3 <https://pypi.org/project/matplotlib/>`_  (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
+  (required for compressing/decompressing image data)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12
+  (required for reading/writing tags from/to TIFF files)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+  (required for plotting)
 
 Revisions
 ---------
 
+2023.4.30
+
+- Few API changes (breaking).
+- Improve object repr.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
+2023.2.18
+
+- Allow unknown PsdKeys (#5).
+
 2023.2.8
 
 - Change PsdPoint and PsdReferencePoint signatures (breaking).
 - Add helper function to create composite from layers.
 
 2022.8.25
 
@@ -87,15 +101,15 @@
 - Initial release.
 
 Notes
 -----
 
 The API is not stable yet and might change between revisions.
 
-This module has been tested with a limited number of files only.
+This library has been tested with a limited number of files only.
 
 Additional layer information is not yet supported.
 
 Consider `psd-tools <https://github.com/psd-tools/psd-tools>`_ and
 `pytoshop <https://github.com/mdboom/pytoshop>`_  for working with
 Adobe Photoshop PSD files.
 
@@ -147,7 +161,10 @@
 >>> assert isd == TiffImageSourceData.fromtiff('_layered.tif')
 >>> assert res == TiffImageResources.fromtiff('_layered.tif')
 
 View the layer and mask information as well as the image resource blocks in
 a layered TIFF file from a command line::
 
     python -m psdtags layered.tif
+
+Refer to the `layered_tiff.py` example in the source distribution for
+creating a layered TIFF file from individual layer images.
```

### Comparing `psdtags-2023.2.8/examples/layered_tiff.py` & `psdtags-2023.4.30/examples/layered_tiff.py`

 * *Files identical despite different names*

### Comparing `psdtags-2023.2.8/examples/product.png` & `psdtags-2023.4.30/examples/product.png`

 * *Files identical despite different names*

### Comparing `psdtags-2023.2.8/examples/reflection.png` & `psdtags-2023.4.30/examples/reflection.png`

 * *Files identical despite different names*

### Comparing `psdtags-2023.2.8/examples/shadow.png` & `psdtags-2023.4.30/examples/shadow.png`

 * *Files identical despite different names*

### Comparing `psdtags-2023.2.8/psdtags/psdtags.py` & `psdtags-2023.4.30/psdtags/psdtags.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,24 +34,25 @@
 Psdtags is a Python library to read and write the Adobe Photoshop(r) specific
 ImageResources (#34377) and ImageSourceData (#37724) TIFF tags, which contain
 image resource blocks, layer and mask information found in a typical layered
 TIFF file created by Photoshop.
 
 The format is specified in the
 `Adobe Photoshop TIFF Technical Notes (March 22, 2002)
-<https://www.adobe.io/open/standards/TIFF.html>`_
+<https://www.awaresystems.be/imaging/tiff/specification/TIFFphotoshop.pdf>`_
 and
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.2.8
+:Version: 2023.4.30
+:DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
 
@@ -68,23 +69,36 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.10, 3.11.2 <https://www.python.org>`_
-- `NumPy 1.23.5 <https://pypi.org/project/numpy/>`_
-- `Imagecodecs 2023.1.23 <https://pypi.org/project/imagecodecs/>`_ (optional)
-- `Tifffile 2023.2.3 <https://pypi.org/project/tifffile/>`_  (optional)
-- `Matplotlib 3.6.3 <https://pypi.org/project/matplotlib/>`_  (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
+  (required for compressing/decompressing image data)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12
+  (required for reading/writing tags from/to TIFF files)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+  (required for plotting)
 
 Revisions
 ---------
 
+2023.4.30
+
+- Few API changes (breaking).
+- Improve object repr.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
+2023.2.18
+
+- Allow unknown PsdKeys (#5).
+
 2023.2.8
 
 - Change PsdPoint and PsdReferencePoint signatures (breaking).
 - Add helper function to create composite from layers.
 
 2022.8.25
 
@@ -117,15 +131,15 @@
 - Initial release.
 
 Notes
 -----
 
 The API is not stable yet and might change between revisions.
 
-This module has been tested with a limited number of files only.
+This library has been tested with a limited number of files only.
 
 Additional layer information is not yet supported.
 
 Consider `psd-tools <https://github.com/psd-tools/psd-tools>`_ and
 `pytoshop <https://github.com/mdboom/pytoshop>`_  for working with
 Adobe Photoshop PSD files.
 
@@ -178,19 +192,22 @@
 >>> assert res == TiffImageResources.fromtiff('_layered.tif')
 
 View the layer and mask information as well as the image resource blocks in
 a layered TIFF file from a command line::
 
     python -m psdtags layered.tif
 
+Refer to the `layered_tiff.py` example in the source distribution for
+creating a layered TIFF file from individual layer images.
+
 """
 
 from __future__ import annotations
 
-__version__ = '2023.2.8'
+__version__ = '2023.4.30'
 
 __all__ = [
     'PsdBlendMode',
     'PsdBoolean',
     'PsdBytesBlock',
     'PsdChannel',
     'PsdChannelId',
@@ -210,14 +227,15 @@
     'PsdLayer',
     'PsdLayerFlag',
     'PsdLayerMask',
     'PsdLayerMaskFlag',
     'PsdLayerMaskParameterFlag',
     'PsdLayers',
     'PsdMetadataSetting',
+    'PsdMetadataSettings',
     'PsdPascalString',
     'PsdPascalStringBlock',
     'PsdPascalStringsBlock',
     'PsdPatterns',
     'PsdPoint',
     'PsdRectangle',
     'PsdReferencePoint',
@@ -242,72 +260,97 @@
     'TiffImageSourceData',
     'read_tifftag',
     'read_psdblocks',
     'read_psdtags',
     'write_psdblocks',
     'write_psdtags',
     'overlay',
+    'compress',
+    'decompress',
+    'REPR_MAXLEN',
 ]
 
 
 import sys
 import os
 import io
 import enum
 import struct
 import zlib
 import dataclasses
 import abc
+from functools import cached_property
 
 import numpy
 
-from typing import cast, Any, BinaryIO, Iterable, Literal, NamedTuple
+from typing import TYPE_CHECKING, cast, NamedTuple
+
+if TYPE_CHECKING:
+    from typing import Any, BinaryIO, Literal
+    from collections.abc import Generator, Iterable
+
+    from numpy.typing import NDArray, DTypeLike
+
+
+REPR_MAXLEN = 24
+"""Maximum length of bytes to show in repr()."""
 
 
 class BytesEnumMeta(enum.EnumMeta):
     """Metaclass for bytes enums."""
 
     def __contains__(cls, value: object) -> bool:
         try:
             cls(value)
         except ValueError:
             return False
         else:
             return True
 
-    def __call__(cls, *args, **kwds) -> Any:
+    def __call__(cls, *args, **kwds) -> Any:  # type: ignore
         try:
             # big endian
             c = enum.EnumMeta.__call__(cls, *args, **kwds)
         except ValueError as exc:
             try:
                 # little endian
                 if args:
                     args = (args[0][::-1],) + args[1:]
                 c = enum.EnumMeta.__call__(cls, *args, **kwds)
             except Exception:
-                raise exc
+                if args and len(args[0]) == 4 and args[0].strip().isalnum():
+                    log_warning(
+                        f'psdtags.{cls.__name__}({args[0]!r}) not defined'
+                    )
+                    newargs = (b'?unk',) + args[1:]
+                    c = enum.EnumMeta.__call__(cls, *newargs, **kwds)
+                    c._value_ = args[0]
+                else:
+                    raise exc
         return c
 
 
 class BytesEnum(bytes, enum.Enum, metaclass=BytesEnumMeta):
     """Base class for bytes enums."""
 
+    value: bytes
+
     def tobytes(self, byteorder: str = '>') -> bytes:
         """Return enum value as bytes."""
         return self.value if byteorder == '>' else self.value[::-1]
 
     def write(self, fh: BinaryIO, byteorder: str = '>', /) -> int:
         """Write enum value to open file."""
         return fh.write(self.value if byteorder == '>' else self.value[::-1])
 
 
 class PsdKey(BytesEnum):
     """Keys of tagged structures."""
 
+    UNKNOWN = b'?unk'
     ALPHA = b'Alph'
     ANIMATION_EFFECTS = b'anFX'
     ANNOTATIONS = b'Anno'
     ARTBOARD_DATA = b'artb'
     ARTBOARD_DATA_2 = b'artd'
     ARTBOARD_DATA_3 = b'abdd'
     BLACK_AND_WHITE = b'blwh'
@@ -319,18 +362,20 @@
     COLOR_BALANCE = b'blnc'
     COLOR_LOOKUP = b'clrL'
     COMPOSITOR_USED = b'cinf'
     CONTENT_GENERATOR_EXTRA_DATA = b'CgEd'
     CURVES = b'curv'
     EFFECTS_LAYER = b'lrFX'
     EXPOSURE = b'expA'
+    FILL_OPACITY = b'iOpa'
     FILTER_EFFECTS = b'FXid'
     FILTER_EFFECTS_2 = b'FEid'
     FILTER_MASK = b'FMsk'
     FOREIGN_EFFECT_ID = b'ffxi'
+    FRAMED_GROUP = b'frgb'
     GRADIENT_FILL_SETTING = b'GdFl'
     GRADIENT_MAP = b'grdm'
     HUE_SATURATION = b'hue2'
     HUE_SATURATION_PS4 = b'hue '
     INVERT = b'nvrt'
     KNOCKOUT_SETTING = b'knko'
     LAYER = b'Layr'
@@ -500,14 +545,15 @@
         obj._value_ = value
         return obj
 
 
 class PsdBlendMode(BytesEnum):
     """Blend modes."""
 
+    UNKNOWN = b'?unk'
     PASS_THROUGH = b'pass'
     NORMAL = b'norm'
     DISSOLVE = b'diss'
     DARKEN = b'dark'
     MULTIPLY = b'mul '
     COLOR_BURN = b'idiv'
     LINEAR_BURN = b'lbrn'
@@ -533,15 +579,15 @@
     COLOR = b'colr'
     LUMINOSITY = b'lum '
 
 
 class PsdColorSpaceType(enum.IntEnum):
     """Color space types."""
 
-    DUMMY = -1
+    UNKNOWN = -1
     RGB = 0
     HSB = 1
     CMYK = 2
     Pantone = 3
     Focoltone = 4
     Trumatch = 5
     Toyo = 6
@@ -566,15 +612,15 @@
         obj._value_ = value
         return obj
 
 
 class PsdImageMode(enum.IntEnum):
     """Image modes."""
 
-    DUMMY = -1
+    UNKNOWN = -1
     Bitmap = 0
     Grayscale = 1
     Indexed = 2
     RGB = 3
     CMYK = 4
     Multichannel = 7
     Duotone = 8
@@ -634,36 +680,43 @@
     """Layer record flags."""
 
     TRANSPARENCY_PROTECTED = 1
     VISIBLE = 2
     OBSOLETE = 4
     PHOTOSHOP5 = 8  # 1 for Photoshop 5.0 and later, tells if bit 4 has info
     IRRELEVANT = 16  # pixel data irrelevant to appearance of document
+    _32 = 32
+    _64 = 64
 
 
 class PsdLayerMaskFlag(enum.IntFlag):
     """Layer mask flags."""
 
     RELATIVE = 1  # position relative to layer
     DISABLED = 2  # layer mask disabled
     INVERT = 4  # invert layer mask when blending (obsolete)
     RENDERED = 8  # user mask actually came from rendering other data
     APPLIED = 16  # user and/or vector masks have parameters applied to them
+    _32 = 32
+    _64 = 64
 
 
 class PsdLayerMaskParameterFlag(enum.IntFlag):
     """Layer mask parameters."""
 
     USER_DENSITY = 1  # user mask density, 1 byte
     USER_FEATHER = 2  # user mask feather, 8 byte, double
     VECTOR_DENSITY = 4  # vector mask density, 1 byte
     VECTOR_FEATHER = 8  # vector mask feather, 8 bytes, double
+    _16 = 16
+    _32 = 32
+    _64 = 64
 
 
-class PsdColorType(enum.IntFlag):
+class PsdColorType(enum.IntEnum):
     """Color IDs used by sheet color setting structure."""
 
     UNKNOWN = -1
     NONE = 0
     RED = 1
     ORANGE = 2
     YELLOW = 3
@@ -679,34 +732,35 @@
         obj._value_ = value
         return obj
 
 
 class PsdSectionDividerType(enum.IntEnum):
     """Section divider setting types."""
 
+    UNKNOWN = -1
     OTHER = 0
     OPEN_FOLDER = 1
     CLOSED_FOLDER = 2
     BOUNDING_SECTION_DIVIDER = 3
 
     @classmethod
     def _missing_(cls, value: object) -> object:
         assert isinstance(value, int)
-        obj = cls(0)
+        obj = cls(-1)
         obj._value_ = value
         return obj
 
 
 class PsdPoint(NamedTuple):
     """Point."""
 
     y: int
     x: int
 
-    def __str__(self) -> str:
+    def __repr__(self) -> str:
         return str(tuple(self))
 
 
 class PsdRectangle(NamedTuple):
     """Rectangle."""
 
     top: int
@@ -721,16 +775,19 @@
     @property
     def offset(self) -> tuple[int, int]:
         return self.top, self.left
 
     def __bool__(self) -> bool:
         return self.bottom - self.top > 0 and self.right - self.left > 0
 
-    def __str__(self) -> str:
-        return str(tuple(self))
+    def __repr__(self) -> str:
+        return (
+            f'{self.__class__.__name__}('
+            f'{self.top}, {self.left}, {self.bottom}, {self.right})'
+        )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdPascalString:
     """Pascal string."""
 
     value: str
@@ -754,20 +811,20 @@
         data = value.encode('macroman')
         size = len(data)
         fh.write(struct.pack('B', size))
         fh.write(data)
         pad = fh.write(b'\0' * ((pad - (size + 1) % pad) % pad))
         return 1 + size + pad
 
+    def __str__(self) -> str:
+        return self.value
+
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self.value!r})'
 
-    def __str__(self):
-        return self.value
-
 
 @dataclasses.dataclass(repr=False)
 class PsdUnicodeString:
     """Unicode string."""
 
     value: str
 
@@ -781,28 +838,28 @@
             raise OSError(f'could not read enough data, {len(data)} != {size}')
         value = data.decode(psdformat.utf16)
         if value and value[-1] == '\0':
             value = value[:-1]
         return cls(value=value)
 
     def write(
-        self, fh: BinaryIO, psdformat: PsdFormat, /, terminate=True
+        self, fh: BinaryIO, psdformat: PsdFormat, /, terminate: bool = True
     ) -> int:
         """Write unicode string to open file."""
         value = self.value + '\0' if terminate else self.value
         written = psdformat.write(fh, 'I', len(value))
         written += fh.write(value.encode(psdformat.utf16))
         return written
 
+    def __str__(self) -> str:
+        return self.value
+
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self.value!r})'
 
-    def __str__(self):
-        return self.value
-
 
 class PsdFormat(bytes, enum.Enum):
     """PSD format."""
 
     BE32BIT = b'8BIM'
     LE32BIT = b'MIB8'
     BE64BIT = b'8B64'
@@ -821,48 +878,48 @@
         if self.value == PsdFormat.LE32BIT:
             return '<I'
         if self.value == PsdFormat.BE64BIT:
             return '>Q'
         return '<Q'
 
     @property
-    def utf16(self):
+    def utf16(self) -> str:
         if self.value == PsdFormat.BE32BIT or self.value == PsdFormat.BE64BIT:
             return 'UTF-16-BE'
         return 'UTF-16-LE'
 
     @property
-    def isb64(self):
+    def isb64(self) -> bool:
         return (
             self.value == PsdFormat.BE64BIT or self.value == PsdFormat.LE64BIT
         )
 
     def read(self, fh: BinaryIO, fmt: str) -> Any:
         """Return unpacked values."""
         fmt = self.byteorder + fmt
         value = struct.unpack(fmt, fh.read(struct.calcsize(fmt)))
         return value[0] if len(value) == 1 else value
 
-    def write(self, fh: BinaryIO, fmt: str, *values) -> int:
+    def write(self, fh: BinaryIO, fmt: str, *values: Any) -> int:
         """Write values to open file."""
         return fh.write(struct.pack(self.byteorder + fmt, *values))
 
-    def pack(self, fmt: str, *values) -> bytes:
+    def pack(self, fmt: str, *values: Any) -> bytes:
         """Return packed values."""
         return struct.pack(self.byteorder + fmt, *values)
 
     def read_size(self, fh: BinaryIO, key: PsdKey | None = None) -> int:
         """Return integer whose size depends on signature or key from file."""
         if key is None:
             fmt = self.sizeformat
         elif self.isb64 and key in PSD_KEY_64BIT:
             fmt = self.sizeformat  # TODO: test this
         else:
             fmt = self.byteorder + 'I'
-        return struct.unpack(fmt, fh.read(struct.calcsize(fmt)))[0]
+        return int(struct.unpack(fmt, fh.read(struct.calcsize(fmt)))[0])
 
     def write_size(
         self, fh: BinaryIO, value: int, key: PsdKey | None = None
     ) -> int:
         """Write integer whose size depends on signature or key to file."""
         return fh.write(self.pack_size(value, key))
 
@@ -917,23 +974,23 @@
         return self
 
     @abc.abstractmethod
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write instance values to open file."""
         pass
 
-    def tobytes(self, psdformat: PsdFormat, /):
+    def tobytes(self, psdformat: PsdFormat, /) -> bytes:
         """Return instance values as bytes."""
         with io.BytesIO() as fh:
             self.write(fh, psdformat)
             data = fh.getvalue()
         return data
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {self.key.name}>'
+        return f'{self.__class__.__name__}{enumstr(self.key)})>'
 
 
 @dataclasses.dataclass(repr=False)
 class PsdLayers(PsdKeyABC):
     """Sequence of PsdLayer."""
 
     key: PsdKey
@@ -958,15 +1015,15 @@
     ) -> PsdLayers:
         """Return instance from open file."""
         count = psdformat.read(fh, 'h')
         has_transparency = count < 0
         count = abs(count)
 
         # layer records
-        layers = []
+        layers: list[PsdLayer] = []
         for _ in range(count):
             layers.append(PsdLayer.read(fh, psdformat, unknown=unknown))
 
         # channel image data
         dtype = PsdLayers.TYPES[key]
         shape: tuple[int, ...] = ()
         for layer in layers:
@@ -1000,15 +1057,15 @@
         return self
 
     def write(
         self,
         fh: BinaryIO,
         psdformat: PsdFormat,
         /,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
         unknown: bool = True,
     ) -> int:
         """Write layer records and channel info data to open file."""
         pos = fh.tell()
         # channel count
         psdformat.write(
             fh, 'h', (-1 if self.has_transparency else 1) * len(self.layers)
@@ -1030,25 +1087,25 @@
             size += 1
         return size
 
     def tobytes(
         self,
         psdformat: PsdFormat,
         /,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
         unknown: bool = True,
-    ):
+    ) -> bytes:
         """Return layer records and channel info data as bytes."""
         with io.BytesIO() as fh:
             self.write(fh, psdformat, compression=compression, unknown=unknown)
             data = fh.getvalue()
         return data
 
     @property
-    def dtype(self) -> numpy.dtype:
+    def dtype(self) -> numpy.dtype[Any]:
         return numpy.dtype(PsdLayers.TYPES[self.key])
 
     @property
     def shape(self) -> tuple[int, int]:
         shape = [0, 0]
         for layer in self.layers:
             if layer.rectangle[2] > shape[0]:
@@ -1067,28 +1124,29 @@
 
     def __len__(self) -> int:
         return len(self.layers)
 
     def __getitem__(self, key: int) -> PsdLayer:
         return self.layers[key]
 
-    def __setitem__(self, key: int, value: PsdLayer):
+    def __setitem__(self, key: int, value: PsdLayer) -> None:
         self.layers[key] = value
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[PsdLayer, None, None]:
         yield from self.layers
 
-    def __str__(self) -> str:
+    def __repr__(self) -> str:
+        sz = len(self.layers)
         return indent(
-            repr(self),
-            # f'length: {len(self)}',
-            f'shape: {self.shape!r}',
-            f'dtype: {numpy.dtype(self.dtype)}',
-            f'has_transparency: {self.has_transparency!r}',
-            *self.layers,
+            f'{self.__class__.__name__}(',
+            f'# {self.shape!r} {self.dtype}',
+            f'key={enumstr(self.key)},',
+            f'has_transparency={self.has_transparency},',
+            f'layers=[  # {sz}\n    {indent(*self.layers, sep=",")},\n],',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdLayer:
     """PSD layer record."""
 
@@ -1167,15 +1225,15 @@
         return self
 
     def write(
         self,
         fh: BinaryIO,
         psdformat: PsdFormat,
         /,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
         unknown: bool = True,
     ) -> bytes:
         """Write layer record to open file and return channel data records."""
         psdformat.write(fh, 'iiii', *self.rectangle)
         psdformat.write(fh, 'H', len(self.channels))
 
         channel_image_data = []
@@ -1222,29 +1280,29 @@
 
         return b''.join(channel_image_data)
 
     def tobytes(
         self,
         psdformat: PsdFormat,
         /,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
         unknown: bool = True,
     ) -> tuple[bytes, bytes]:
         """Return layer and channel data records."""
         with io.BytesIO() as fh:
             channel_image_data = self.write(
                 fh, psdformat, compression=compression, unknown=unknown
             )
             layer_record = fh.getvalue()
         return layer_record, channel_image_data
 
     def asarray(
-        self, channelid: bytes | None = None, planar: bool = False
-    ) -> numpy.ndarray:
-        """Return channel image data as numpy array."""
+        self, channelid: PsdChannelId | None = None, planar: bool = False
+    ) -> NDArray[Any]:
+        """Return channel image data."""
         if channelid is not None:
             datalist = [
                 channel.data
                 for channel in self.channels
                 if channel.channelid == channelid and channel.data is not None
             ]
         else:
@@ -1272,15 +1330,19 @@
         return self.rectangle.shape if self.rectangle else (0, 0)
 
     @property
     def offset(self) -> tuple[int, int]:
         return self.rectangle.offset
 
     @property
-    def has_unknowns(self):
+    def title(self) -> str:
+        return f'{self.__class__.__name__} {self.name!r}'
+
+    @property
+    def has_unknowns(self) -> bool:
         return any(isinstance(tag, PsdUnknown) for tag in self.info)
 
     def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, self.__class__)
             # and self.name == other.name
             and self.rectangle == other.rectangle
@@ -1291,44 +1353,47 @@
             and self.flags == other.flags
             and self.mask == other.mask
             and self.info == other.info
             and self.channels == other.channels
         )
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {str(self.name)!r}>'
-
-    def __str__(self) -> str:
+        szc = len(self.channels)
+        szi = len(self.info)
         return indent(
-            repr(self),
-            f'rectangle: {self.rectangle}',
-            f'opacity: {self.opacity}',
-            f'blendmode: {self.blendmode.name}',
-            f'clipping: {self.clipping.name}',
-            f'flags: {str(self.flags)}',
-            self.mask,
-            indent(f'channels[{len(self.channels)}]', *self.channels),
-            indent(f'info[{len(self.info)}]', *self.info),
+            f'{self.__class__.__name__}(',
+            f'name={self.name!r},',
+            f'channels=[  # {szc}\n    {indent(*self.channels, sep=",")},\n],',
+            f'rectangle={self.rectangle},',
+            f'mask={self.mask},',
+            f'opacity={self.opacity},',
+            f'blendmode={enumstr(self.blendmode)},',
+            f'blending_ranges={self.blending_ranges},',
+            f'clipping={enumstr(self.clipping)},',
+            f'flags={enumstr(self.flags)},',
+            f'info=[  # {szi}\n    {indent(*self.info, sep=",")},\n],',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdChannel:
     """ChannelInfo and ChannelImageData."""
 
     channelid: PsdChannelId
     compression: PsdCompressionType = PsdCompressionType.RAW
-    data: numpy.ndarray | None = None
+    data: NDArray[Any] | None = None
     _data_length: int = 0
 
     @classmethod
     def read(cls, fh: BinaryIO, psdformat: PsdFormat, /) -> PsdChannel:
         """Return instance from open file.
 
-        Channel image data must be read separately using read_image.
+        Channel image data must be read separately using
+        :py:meth:`PsdChannel.read_image`.
 
         """
         channelid = PsdChannelId(psdformat.read(fh, 'h'))
         data_length = psdformat.read_size(fh)
         return cls(channelid=channelid, _data_length=data_length)
 
     @classmethod
@@ -1340,15 +1405,15 @@
 
     def read_image(
         self,
         fh: BinaryIO,
         psdformat: PsdFormat,
         /,
         shape: tuple[int, ...],
-        dtype: numpy.dtype | str,
+        dtype: DTypeLike | str,
     ) -> None:
         """Read channel image data from open file."""
         if self.data is not None:
             raise RuntimeError
 
         self.compression = PsdCompressionType(psdformat.read(fh, 'H'))
 
@@ -1360,15 +1425,15 @@
             data, self.compression, shape, dtype, rlecountfmt
         )
 
     def tobytes(
         self,
         psdformat: PsdFormat,
         /,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
     ) -> tuple[bytes, bytes]:
         """Return channel info and image data records."""
         if self.data is None:
             raise ValueError('data is None')
         if compression is None:
             compression = self.compression
         else:
@@ -1389,15 +1454,15 @@
         return channel_info, channel_image_data
 
     def write(
         self,
         fh: BinaryIO,
         psdformat: PsdFormat,
         /,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
     ) -> bytes:
         """Write channel info record to file and return image data record."""
         channel_info, channel_image_data = self.tobytes(
             psdformat, compression=compression
         )
         fh.write(channel_info)
         return channel_image_data
@@ -1407,17 +1472,27 @@
             isinstance(other, self.__class__)
             and self.channelid == other.channelid
             and numpy.array_equal(self.data, other.data)  # type: ignore
             # and self.compression == other.compression
         )
 
     def __repr__(self) -> str:
-        return (
-            f'<{self.__class__.__name__}'
-            f' {self.channelid.name} {self.compression.name}>'
+        if self.data is None:
+            data = 'data=None,'
+        else:
+            data = (
+                'data=...,  # numpy.array('
+                f"{self.data.shape}, '{self.data.dtype}')"
+            )
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'channelid={enumstr(self.channelid)},',
+            f'compression={enumstr(self.compression)},',
+            data,
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdLayerMask:
     """Layer mask / adjustment layer data."""
 
@@ -1551,41 +1626,39 @@
     def offset(self) -> tuple[int, int]:
         return self.rectangle.offset if self.rectangle is not None else (0, 0)
 
     def __bool__(self) -> bool:
         return self.rectangle is not None
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {self.rectangle}>'
-
-    def __str__(self) -> str:
         if self.rectangle is None:
-            return repr(self)
+            return f'{self.__class__.__name__}()'
         info = [
-            repr(self),
-            # f'rectangle: {self.rectangle}',
-            f'default_color: {self.default_color!r}',
+            f'{self.__class__.__name__}(',
+            f'flags={enumstr(self.flags)},',
+            f'rectangle={self.rectangle},',
         ]
-        if self.flags:
-            info += [f'flags: {str(self.flags)}']
+        if self.default_color:
+            info += [f'default_color={self.default_color},']
         if self.user_mask_density is not None:
-            info += [f'user_mask_density: {self.user_mask_density}']
+            info += [f'user_mask_density={self.user_mask_density},']
         if self.user_mask_feather is not None:
-            info += [f'user_mask_feather: {self.user_mask_feather}']
+            info += [f'user_mask_feather={self.user_mask_feather},']
         if self.vector_mask_density is not None:
-            info += [f'vector_mask_density: {self.vector_mask_density}']
+            info += [f'vector_mask_density={self.vector_mask_density},']
         if self.vector_mask_feather is not None:
-            info += [f'vector_mask_feather: {self.vector_mask_feather}']
+            info += [f'vector_mask_feather={self.vector_mask_feather},']
         if self.real_flags is not None and self.real_background is not None:
             info += [
-                f'real_background: {self.real_background!r}',
-                repr(self.real_rectangle),
+                f'real_flags={enumstr(self.real_flags)},',
+                f'real_background={self.real_background},',
+                f'real_rectangle={self.real_rectangle},',
                 repr(self.real_flags),
             ]
-        return indent(*info)
+        return indent(*info, end='\n)')
 
 
 @dataclasses.dataclass(repr=False)
 class PsdUserMask(PsdKeyABC):
     """User mask. Same as global layer mask info table."""
 
     colorspace: PsdColorSpaceType = PsdColorSpaceType(-1)
@@ -1626,21 +1699,21 @@
         data += b'\0'
         return data
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write user mask record to open file."""
         return fh.write(self.tobytes(psdformat))
 
-    def __str__(self) -> str:
+    def __repr__(self) -> str:
         return indent(
-            repr(self),
-            f'colorspace: {self.colorspace.name}',
-            f'components: {self.components}',
-            f'opacity: {self.opacity}',
-            # f'flag: {self.flag}',  # always 128
+            f'{self.__class__.__name__}(',
+            f'colorspace={enumstr(self.colorspace)},',
+            f'components={self.components},',
+            f'opacity={self.opacity},',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdFilterMask(PsdKeyABC):
     """Filter Mask (Photoshop CS3)."""
 
@@ -1679,35 +1752,33 @@
         return data
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write filter mask record to open file."""
         return fh.write(self.tobytes(psdformat))
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {self.colorspace.name}>'
-
-    def __str__(self) -> str:
         return indent(
-            repr(self),
-            f'components: {self.colorspace.name}',
-            f'components: {self.components}',
-            f'opacity: {self.opacity}',
+            f'{self.__class__.__name__}(',
+            f'colorspace={enumstr(self.colorspace)},',
+            f'components={self.components},',
+            f'opacity={self.opacity},',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdPatterns(PsdKeyABC):
     """Patterns (Photoshop 6.0 and CS 8.0)."""
 
     key: PsdKey
     imagemode: PsdImageMode
     name: str
     guid: str
     data: PsdVirtualMemoryArrayList
-    colortable: numpy.ndarray | None = None
+    colortable: NDArray[numpy.uint8] | None = None
     point: PsdPoint = PsdPoint(0, 0)
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
@@ -1757,36 +1828,48 @@
         self.data.write(fh, psdformat)
         length = fh.tell() - pos
         fh.seek(length_pos)
         psdformat.write(fh, 'I', length)
         fh.seek(length, 1)
         return length + 4
 
-    def asarray(self, planar: bool = False) -> numpy.ndarray:
-        """Return channel image data as numpy array."""
-        datalist = [channel.data for channel in self.data if channel]
+    def asarray(self, planar: bool = False) -> NDArray[Any]:
+        """Return channel image data."""
+        datalist: list[NDArray[Any]] = [
+            channel.data
+            for channel in self.data
+            if channel and channel.data is not None
+        ]
         if len(datalist) == 0:
             raise ValueError('no channel data found')
         if len(datalist) == 1:
             return datalist[0]
-        data = numpy.stack(datalist)
+        data: NDArray[Any] = numpy.stack(datalist)
         if not planar:
             data = numpy.moveaxis(data, 0, -1)
         return data
 
-    def __str__(self) -> str:
-        colortable = None if self.colortable is None else self.colortable.shape
+    def __repr__(self) -> str:
+        if self.colortable is None:
+            colortable = None
+        else:
+            colortable = (
+                '...,  # numpy.zeros('
+                f'{self.colortable.shape}, {self.colortable.dtype})'
+            )
         return indent(
-            repr(self),
-            f'imagemode: {self.imagemode.name}',
-            f'name: {str(self.name)!r}',
-            f'guid: {str(self.guid)!r}',
-            f'colortable: {colortable}',
-            f'point: {self.point}',
-            self.data,
+            f'{self.__class__.__name__}(',
+            f'key={enumstr(self.key)},',
+            f'imagemode={enumstr(self.imagemode)},',
+            f'name={self.name!r},',
+            f'guid={self.guid!r},',
+            f'colortable={colortable},',
+            f'point={self.point},',
+            f'data={self.data},',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdMetadataSettings(PsdKeyABC):
     """Metadata setting (Photoshop 6.0)."""
 
@@ -1814,26 +1897,30 @@
         """Write metadata settings to open file."""
         written = psdformat.write(fh, 'I', len(self.items))
         for item in self.items:
             written = item.write(fh, psdformat)
         return written
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} [{len(self.items)}]>'
-
-    def __str__(self) -> str:
-        return indent(repr(self), *self.items)
+        sz = len(self.items)
+        if not self.items:
+            return f'{self.__class__.__name__}()'
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'items=[  # {sz}\n    {indent(*self.items, sep=",")},\n],',
+            end='\n)',
+        )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdMetadataSetting:
     """Metadata setting item."""
 
     signature: PsdFormat
-    key: bytes
+    key: bytes  # b'cust', b'cmls', b'extn', b'mlst', b'tmln', b'sgrp'
     data: bytes = b''
     copyonsheet: bool = False
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
@@ -1867,16 +1954,25 @@
             # and self.signature == other.signature
             and self.key == other.key
             and self.copyonsheet == other.copyonsheet
             and self.data == other.data
         )
 
     def __repr__(self) -> str:
-        return (
-            f'<{self.__class__.__name__} {self.key!r} {len(self.data)} bytes>'
+        if len(self.data) > REPR_MAXLEN:
+            data = f'data=...,  # bytes({len(self.data)})'
+        else:
+            data = f'data={self.data!r},'
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'signature={enumstr(self.signature)},',
+            f'key={self.key!r},',
+            f'copyonsheet={self.copyonsheet},',
+            data if self.data else '',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdVirtualMemoryArrayList:
     """Virtual memory array list."""
 
@@ -1920,44 +2016,40 @@
 
     def __len__(self) -> int:
         return len(self.channels)
 
     def __getitem__(self, key: int) -> PsdVirtualMemoryArray:
         return self.channels[key]
 
-    def __setitem__(self, key: int, value: PsdVirtualMemoryArray):
+    def __setitem__(self, key: int, value: PsdVirtualMemoryArray) -> None:
         self.channels[key] = value
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[PsdVirtualMemoryArray, None, None]:
         yield from self.channels
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} [{len(self.channels)}]>'
-
-    def __str__(self) -> str:
-        channels = [
-            repr(channel) for channel in self.channels if channel.iswritten
-        ]
+        sz = len(self.channels)
         return indent(
-            repr(self),
-            f'rectangle: {str(self.rectangle)}',
-            *channels,
+            f'{self.__class__.__name__}(',
+            f'rectangle={self.rectangle},',
+            f'channels=[  # {sz}\n    {indent(*self.channels, sep=",")},\n],',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdVirtualMemoryArray:
     """Virtual memory array."""
 
     iswritten: bool = False
     depth: int | None = None
     rectangle: PsdRectangle | None = None
     pixeldepth: int | None = None
     compression: PsdCompressionType = PsdCompressionType.RAW
-    data: numpy.ndarray | None = None
+    data: NDArray[Any] | None = None
 
     @classmethod
     def read(
         cls, fh: BinaryIO, psdformat: PsdFormat, /
     ) -> PsdVirtualMemoryArray:
         """Return instance from open file."""
         iswritten = bool(psdformat.read(fh, 'I'))
@@ -2030,15 +2122,15 @@
         fh.seek(length_pos)
         psdformat.write(fh, 'I', length)
         fh.seek(length, 1)
 
         return fh.tell() - start
 
     @property
-    def dtype(self) -> numpy.dtype:
+    def dtype(self) -> numpy.dtype[Any]:
         if self.pixeldepth is None:
             return numpy.dtype('B')
         return numpy.dtype({8: 'B', 16: 'H', 32: 'f'}[self.pixeldepth])
 
     @property
     def shape(self) -> tuple[int, int]:
         return self.rectangle.shape if self.rectangle else (0, 0)
@@ -2058,32 +2150,25 @@
             and self.pixeldepth == other.pixeldepth
             and self.rectangle == other.rectangle
             and numpy.array_equal(self.data, other.data)  # type: ignore
             # and self.compression == other.compression
         )
 
     def __repr__(self) -> str:
-        if not self.iswritten:
-            return f'<{self.__class__.__name__} notwritten>'
-        if self.rectangle is None:
-            return f'<{self.__class__.__name__} empty>'
-        return (
-            f'<{self.__class__.__name__} {str(self.rectangle.shape)} '
-            f'{self.dtype} {self.compression.name}>'
-        )
-
-    def __str__(self) -> str:
         if not self.iswritten or self.rectangle is None:
-            return repr(self)
+            return f'{self.__class__.__name__}()'
         return indent(
-            repr(self),
-            f'rectangle: {str(self.rectangle)}',
-            f'depth: {self.depth}',
-            f'pixeldepth: {self.pixeldepth}',
-            f'compression: {self.compression.name}',
+            f'{self.__class__.__name__}(',
+            f'iswritten={self.iswritten},',
+            f'depth={self.depth},',
+            f'rectangle={self.rectangle},',
+            f'pixeldepth={self.pixeldepth},',
+            f'compression={enumstr(self.compression)},',
+            f'data=...,  # numpy.empty({self.shape}, {self.dtype})',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdSectionDividerSetting(PsdKeyABC):
     """Section divider setting (Photoshop 6.0)."""
 
@@ -2123,15 +2208,21 @@
         psdformat.write_signature(fh, self.blendmode.value)
         if self.subtype is None:
             return 12
         psdformat.write(fh, 'I', self.subtype)
         return 16
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {self.kind.name}>'
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'kind={enumstr(self.kind)},',
+            f'blendmode={enumstr(self.blendmode)},',
+            f'subtype={self.subtype},',
+            end='\n)',
+        )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdSheetColorSetting(PsdKeyABC):
     """Sheet color setting (Photoshop 6.0)."""
 
     color: PsdColorType
@@ -2152,15 +2243,15 @@
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write color setting to open file."""
         psdformat.write(fh, 'H6x', self.color.value)
         return 8
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {self.color.name}>'
+        return f'{self.__class__.__name__}({enumstr(self.color)})'
 
 
 @dataclasses.dataclass(repr=False)
 class PsdReferencePoint(PsdKeyABC):
     """Reference point."""
 
     y: float
@@ -2180,15 +2271,15 @@
         return cls(*psdformat.read(fh, 'dd'))
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write reference point to open file."""
         return psdformat.write(fh, 'dd', self.y, self.x)
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} ({self.y}, {self.x})>'
+        return f'{self.__class__.__name__}({self.y}, {self.x})'
 
 
 @dataclasses.dataclass(repr=False)
 class PsdExposure(PsdKeyABC):
     """Exposure."""
 
     exposure: float
@@ -2214,17 +2305,20 @@
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write exposure to open file."""
         return psdformat.write(
             fh, 'Hfff', 1, self.exposure, self.offset, self.gamma
         )
 
     def __repr__(self) -> str:
-        return (
-            f'<{self.__class__.__name__} '
-            f'{self.exposure}, {self.offset}, {self.gamma}>'
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'exposure={self.exposure},',
+            f'offset={self.offset},',
+            f'gamma={self.gamma},',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdTextEngineData(PsdKeyABC):
     """Text Engine Data (Photoshop CS3)."""
 
@@ -2247,15 +2341,21 @@
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write unicode string to open file."""
         written = psdformat.write(fh, 'I', len(self.data))
         written += fh.write(self.data)
         return written
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {len(self.data)} bytes>'
+        if len(self.data) <= REPR_MAXLEN:
+            return f'{self.__class__.__name__}({self.data!r})'
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'...,  # bytes({len(self.data)})',
+            end='\n)',
+        )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdString(PsdKeyABC):
     """Unicode string."""
 
     key: PsdKey
@@ -2276,17 +2376,20 @@
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write unicode string to open file."""
         return PsdUnicodeString(self.value).write(
             fh, psdformat, terminate=False
         )
 
+    def __str__(self) -> str:
+        return self.value
+
     def __repr__(self) -> str:
         return (
-            f'<{self.__class__.__name__} {self.key.name} ' f'{self.value!r}>'
+            f'{self.__class__.__name__}({enumstr(self.key)}, {self.value!r})'
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdBoolean(PsdKeyABC):
     """Boolean."""
 
@@ -2311,17 +2414,15 @@
         """Write boolean to open file."""
         return fh.write(b'\1\0\0\0' if self.value else b'\0\0\0\0')
 
     def __bool__(self) -> bool:
         return self.value
 
     def __repr__(self) -> str:
-        return (
-            f'<{self.__class__.__name__} {self.key.name} ' f'{self.value!r}>'
-        )
+        return f'{self.__class__.__name__}({enumstr(self.key)}, {self.value})'
 
 
 @dataclasses.dataclass(repr=False)
 class PsdInteger(PsdKeyABC):
     """4 Byte Integer."""
 
     key: PsdKey
@@ -2341,17 +2442,15 @@
         return cls(key=key, value=value)
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write integer to open file."""
         return psdformat.write(fh, 'i', self.value)
 
     def __repr__(self) -> str:
-        return (
-            f'<{self.__class__.__name__} {self.key.name} ' f'{self.value!r}>'
-        )
+        return f'{self.__class__.__name__}({enumstr(self.key)}, {self.value})'
 
 
 @dataclasses.dataclass(repr=False)
 class PsdWord(PsdKeyABC):
     """Four bytes."""
 
     key: PsdKey
@@ -2371,15 +2470,15 @@
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write four bytes value to open file."""
         return fh.write(self.value)
 
     def __repr__(self) -> str:
         return (
-            f'<{self.__class__.__name__} {self.key.name} ' f'{self.value!r}>'
+            f'{self.__class__.__name__}({enumstr(self.key)}, {self.value!r})'
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdUnknown(PsdKeyABC):
     """Unknown keys stored as opaque bytes."""
 
@@ -2423,17 +2522,24 @@
             isinstance(other, self.__class__)
             and self.key == other.key
             and (len(self.value) <= 1 or self.psdformat == other.psdformat)
             and self.value == other.value
         )
 
     def __repr__(self) -> str:
-        return (
-            f'<{self.__class__.__name__} {self.key.name} '
-            f'{len(self.value)!r} bytes>'
+        if len(self.value) > REPR_MAXLEN:
+            value = f'value=...,  # bytes({len(self.value)})'
+        else:
+            value = f'value={self.value!r},'
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'key={enumstr(self.key)},',
+            f'psdformat={enumstr(self.psdformat)},',
+            value,
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdEmpty(PsdKeyABC):
     """Empty structure, no data associated with key."""
 
@@ -2464,14 +2570,17 @@
         """Return empty byte string."""
         return b''
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write nothing to open file."""
         return 0
 
+    def __repr__(self) -> str:
+        return f'{self.__class__.__name__}({enumstr(self.key)})'
+
 
 class PsdResourceBlockABC(metaclass=abc.ABCMeta):
     """Abstract base class for image resource block data."""
 
     resourceid: PsdResourceId
     name: str
 
@@ -2506,35 +2615,35 @@
         return self
 
     @abc.abstractmethod
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write instance values to open file."""
         pass
 
-    def tobytes(self, psdformat: PsdFormat, /):
+    def tobytes(self, psdformat: PsdFormat, /) -> bytes:
         """Return instance values as bytes."""
         with io.BytesIO() as fh:
             self.write(fh, psdformat)
             data = fh.getvalue()
         return data
 
     def __repr__(self) -> str:
         return (
-            f'<{self.__class__.__name__} {self.resourceid.name} '
-            f'{self.resourceid.value}>'
+            f'{self.__class__.__name__}('
+            f'{enumstr(self.resourceid)}, {self.name!r})'
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdBytesBlock(PsdResourceBlockABC):
     """Image resource blocks stored as opaque bytes."""
 
     resourceid: PsdResourceId
-    name: str
     value: bytes
+    name: str = ''
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
         resourceid: PsdResourceId,
@@ -2546,26 +2655,39 @@
         value = fh.read(length)
         return cls(resourceid=resourceid, name=name, value=value)
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write instance values to open file."""
         return fh.write(self.value)
 
+    def __repr__(self) -> str:
+        if len(self.value) > REPR_MAXLEN:
+            value = f'value=...,  # bytes({len(self.value)})'
+        else:
+            value = f'value={self.value!r},'
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'resourceid={enumstr(self.resourceid)},',
+            f'name={self.name!r},' if self.name else '',
+            value,
+            end='\n)',
+        )
+
 
 @dataclasses.dataclass(repr=False)
 class PsdVersionBlock(PsdResourceBlockABC):
     """Image resource blocks stored as opaque bytes."""
 
     resourceid: PsdResourceId
-    name: str
     version: int
     file_version: int
     writer_name: str
     reader_name: str
     has_real_merged_data: bool
+    name: str = ''
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
         resourceid: PsdResourceId,
@@ -2595,32 +2717,35 @@
         written += psdformat.write(fh, 'I', self.version)
         written += fh.write(b'\1' if self.has_real_merged_data else b'\0')
         written += PsdUnicodeString(self.writer_name).write(fh, psdformat)
         written += PsdUnicodeString(self.reader_name).write(fh, psdformat)
         written += psdformat.write(fh, 'I', self.file_version)
         return written
 
-    def __str__(self) -> str:
+    def __repr__(self) -> str:
         return indent(
-            repr(self),
-            f'version: {self.version}',
-            f'file_version: {self.file_version}',
-            f'writer_name: {self.writer_name}',
-            f'reader_name: {self.reader_name}',
-            f'has_real_merged_data: {self.has_real_merged_data}',
+            f'{self.__class__.__name__}(',
+            f'resourceid={enumstr(self.resourceid)},',
+            f'name={self.name!r},' if self.name else '',
+            f'version={self.version},',
+            f'file_version={self.file_version},',
+            f'writer_name={self.writer_name!r},',
+            f'reader_name={self.reader_name!r},',
+            f'has_real_merged_data={self.has_real_merged_data},',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdStringBlock(PsdResourceBlockABC):
     """Unicode string."""
 
     resourceid: PsdResourceId
-    name: str
     value: str
+    name: str = ''
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
         resourceid: PsdResourceId,
@@ -2632,25 +2757,31 @@
         value = str(PsdUnicodeString.read(fh, psdformat))
         return cls(resourceid=resourceid, name=name, value=value)
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write Pascal string to open file."""
         return PsdUnicodeString(self.value).write(fh, psdformat)
 
-    def __str__(self) -> str:
-        return indent(repr(self), self.value)
+    def __repr__(self) -> str:
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'resourceid={enumstr(self.resourceid)},',
+            f'name={self.name!r},' if self.name else '',
+            f'value={self.value!r},',
+            end='\n)',
+        )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdStringsBlock(PsdResourceBlockABC):
     """Series of Unicode strings."""
 
     resourceid: PsdResourceId
-    name: str
     values: list[str]
+    name: str = ''
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
         resourceid: PsdResourceId,
@@ -2668,25 +2799,33 @@
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write sequence of Unicode strings to open file."""
         written = 0
         for value in self.values:
             written += PsdUnicodeString(value).write(fh, psdformat)
         return written
 
-    def __str__(self) -> str:
-        return indent(repr(self), *self.values)
+    def __repr__(self) -> str:
+        values = tuple(f"'{v}'" for v in self.values)
+        sz = len(values)
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'resourceid={enumstr(self.resourceid)},',
+            f'name={self.name!r},' if self.name else '',
+            f'values=[  # {sz}\n    {indent(*values, sep=",")},\n],',
+            end='\n)',
+        )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdPascalStringBlock(PsdResourceBlockABC):
     """Pascal string."""
 
     resourceid: PsdResourceId
-    name: str
     value: str
+    name: str = ''
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
         resourceid: PsdResourceId,
@@ -2698,25 +2837,31 @@
         value = str(PsdPascalString.read(fh, pad=2))
         return cls(resourceid=resourceid, name=name, value=value)
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write Pascal string to open file."""
         return PsdPascalString(self.value).write(fh, pad=2)
 
-    def __str__(self) -> str:
-        return indent(repr(self), self.value)
+    def __repr__(self) -> str:
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'resourceid={enumstr(self.resourceid)},',
+            f'name={self.name!r},' if self.name else '',
+            f'value={self.value!r},',
+            end='\n)',
+        )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdPascalStringsBlock(PsdResourceBlockABC):
     """Series of Pascal strings."""
 
     resourceid: PsdResourceId
-    name: str
     values: list[str]
+    name: str = ''
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
         resourceid: PsdResourceId,
@@ -2734,26 +2879,34 @@
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write sequence of Pascal strings to open file."""
         written = 0
         for value in self.values:
             written += PsdPascalString(value).write(fh, pad=1)
         return written
 
-    def __str__(self) -> str:
-        return indent(repr(self), *self.values)
+    def __repr__(self) -> str:
+        values = tuple(f"'{v}'" for v in self.values)
+        sz = len(values)
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'resourceid={enumstr(self.resourceid)},',
+            f'name={self.name!r},' if self.name else '',
+            f'values=[  # {sz}\n    {indent(*values, sep=",")},\n],',
+            end='\n)',
+        )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdColorBlock(PsdResourceBlockABC):
     """Color structure."""
 
     resourceid: PsdResourceId
-    name: str
     colorspace: PsdColorSpaceType
     components: tuple[int, int, int, int] = (0, 0, 0, 0)
+    name: str = ''
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
         resourceid: PsdResourceId,
@@ -2773,32 +2926,35 @@
         )
 
     def write(self, fh: BinaryIO, psdformat: PsdFormat, /) -> int:
         """Write instance values to open file."""
         fmt = 'h4h' if self.colorspace == PsdColorSpaceType.Lab else 'h4H'
         return psdformat.write(fh, fmt, self.colorspace, *self.components)
 
-    def __str__(self) -> str:
+    def __repr__(self) -> str:
         return indent(
-            repr(self),
-            f'colorspace: {self.colorspace.name}',
-            f'components: {self.components}',
+            f'{self.__class__.__name__}(',
+            f'resourceid={enumstr(self.resourceid)},',
+            f'name={self.name!r},' if self.name else '',
+            f'colorspace={enumstr(self.colorspace)},',
+            f'components={self.components},',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class PsdThumbnailBlock(PsdResourceBlockABC):
     """Thumbnail resource format."""
 
     resourceid: PsdResourceId
-    name: str
     format: int
     width: int
     height: int
     rawdata: bytes
+    name: str = ''
 
     @classmethod
     def read(
         cls,
         fh: BinaryIO,
         psdformat: PsdFormat,
         resourceid: PsdResourceId,
@@ -2856,15 +3012,15 @@
         return 28 + fh.write(self.rawdata)
 
     @property
     def is_bgr(self) -> bool:
         return self.resourceid.value == 1033
 
     @property
-    def data(self) -> numpy.ndarray:
+    def data(self) -> NDArray[Any]:
         if self.format == 0:
             # kRawRGB
             data = numpy.frombuffer(self.rawdata, dtype=numpy.uint8)
             data.shape = (self.height, (self.width * 24 + 31) // 32 * 4)
             data = data[:, : self.width * 3]
             data = data.reshape(self.height, self.width, 3)
         elif self.format == 1:
@@ -2873,19 +3029,29 @@
 
             data = jpeg8_decode(self.rawdata)
             assert data.shape == (self.height, self.width, 3)
         else:
             raise ValueError(f'unknown PsdThumbnailBlock format {format!r}')
         return data
 
-    def __str__(self) -> str:
+    @property
+    def title(self) -> str:
+        """Short representation of instance."""
+        return f'{self.__class__.__name__} {self.name!r}'
+
+    def __repr__(self) -> str:
         return indent(
-            repr(self),
-            f'format: {self.format}',
-            f'shape: ({self.height}, {self.width}, 3)',
+            f'{self.__class__.__name__}(',
+            f'resourceid={enumstr(self.resourceid)},',
+            f'name={self.name!r},' if self.name else '',
+            f'format={self.format},',
+            f'width={self.width},',
+            f'height={self.height},',
+            f'rawdata=...,  # bytes({len(self.rawdata)})',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class TiffImageSourceData:
     """TIFF ImageSourceData tag #37724."""
 
@@ -2973,15 +3139,15 @@
         with io.BytesIO(data) as fh:
             self = cls.read(fh, name=name, unknown=unknown)
         return self
 
     @classmethod
     def fromtiff(
         cls,
-        filename: os.PathLike | str,
+        filename: os.PathLike[Any] | str,
         /,
         pageindex: int = 0,
         unknown: bool = True,
     ) -> TiffImageSourceData:
         """Return instance from TIFF file."""
         data = read_tifftag(filename, 37724, pageindex=pageindex)
         if data is None:
@@ -2991,15 +3157,15 @@
         )
 
     def write(
         self,
         fh: BinaryIO,
         /,
         psdformat: PsdFormat | bytes | None = None,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
         unknown: bool = True,
     ) -> int:
         """Write ImageResourceData tag value to open file."""
         psdformat = (
             self.psdformat if psdformat is None else PsdFormat(psdformat)
         )
         written = fh.write(TiffImageSourceData.SIGNATURE)
@@ -3011,22 +3177,18 @@
             4,
             self.layers,
             self.usermask,
             *self.info,
         )
         return written
 
-    @property
-    def byteorder(self):
-        return self.psdformat.byteorder
-
     def tobytes(
         self,
         psdformat: PsdFormat | bytes | None = None,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
         unknown: bool = True,
     ) -> bytes:
         """Return ImageResourceData tag value as bytes."""
         with io.BytesIO() as fh:
             self.write(
                 fh,
                 psdformat,
@@ -3035,26 +3197,30 @@
             )
             value = fh.getvalue()
         return value
 
     def tifftag(
         self,
         psdformat: PsdFormat | bytes | None = None,
-        compression: PsdCompressionType | int | None = None,
+        compression: PsdCompressionType | None = None,
         unknown: bool = True,
     ) -> tuple[int, int, int, bytes, bool]:
         """Return tifffile.TiffWriter.write extratags item."""
         value = self.tobytes(
             psdformat, compression=compression, unknown=unknown
         )
         return 37724, 7, len(value), value, True
 
-    def has_unknowns(self):
+    @property
+    def byteorder(self) -> Literal['>', '<']:
+        return self.psdformat.byteorder
+
+    def has_unknowns(self) -> bool:
         return any(isinstance(tag, PsdUnknown) for tag in self.info) or any(
-            layer.has_unknowns() for layer in self.layers
+            layer.has_unknowns for layer in self.layers
         )
 
     def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, self.__class__)
             and self.layers == other.layers
             and self.info == other.info
@@ -3062,67 +3228,60 @@
             # and self.psdformat == other.psdformat
         )
 
     def __bool__(self) -> bool:
         return bool(self.layers) or len(self.info) > 1
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {self.name!r}>'
-
-    def __str__(self) -> str:
-        if not self.psdformat:
-            return repr(self)
+        sz = len(self.info)
         return indent(
-            repr(self),
-            repr(self.psdformat),
-            self.layers,
-            self.usermask,
-            *self.info,
+            f'{self.__class__.__name__}(',
+            f'name={self.name!r},' if self.name else '',
+            f'psdformat={enumstr(self.psdformat)},',
+            f'layers={self.layers},',
+            f'usermask={self.usermask},',
+            f'info=[  # {sz}\n    {indent(*self.info, sep=",")},\n],',
+            end='\n)',
         )
 
 
 @dataclasses.dataclass(repr=False)
 class TiffImageResources:
     """TIFF ImageResources tag #34377."""
 
     psdformat: PsdFormat
     blocks: list[PsdResourceBlockABC]
-    blocks_dict: dict[int, PsdResourceBlockABC]  # TODO: use a multidict
     name: str | None = None
 
     @classmethod
     def read(
         cls, fh: BinaryIO, length: int, name: str | None = None
     ) -> TiffImageResources:
         """Return instance from open file."""
         fname = type(fh).__name__ if name is None else name
         blocks = read_psdblocks(fh, length=length)
-        blocks_dict: dict[int, PsdResourceBlockABC] = {}
-        for block in blocks:
-            if block.resourceid.value not in blocks_dict:
-                blocks_dict[block.resourceid.value] = block
+
         return cls(
             psdformat=PsdFormat.BE32BIT,
             name=fname,
             blocks=blocks,
-            blocks_dict=blocks_dict,
         )
 
     @classmethod
     def frombytes(
         cls, data: bytes, name: str | None = None
     ) -> TiffImageResources:
         """Return instance from ImageResources tag value."""
         with io.BytesIO(data) as fh:
             self = cls.read(fh, length=len(data), name=name)
         return self
 
     @classmethod
     def fromtiff(
-        cls, filename: os.PathLike | str, /, pageindex: int = 0
+        cls, filename: os.PathLike[Any] | str, /, pageindex: int = 0
     ) -> TiffImageResources:
         """Return instance from ImageResources tag in TIFF file."""
         data = read_tifftag(filename, 34377, pageindex=pageindex)
         if data is None:
             raise ValueError('TIFF file contains no ImageResources tag')
         return cls.frombytes(data, name=os.path.split(filename)[-1])
 
@@ -3138,22 +3297,31 @@
         return value
 
     def tifftag(self) -> tuple[int, int, int, bytes, bool]:
         """Return tifffile.TiffWriter.write extratags item."""
         value = self.tobytes()
         return 34377, 7, len(value), value, True
 
-    def thumbnail(self) -> numpy.ndarray | None:
+    def thumbnail(self) -> NDArray[Any] | None:
         """Return thumbnail image if any, else None."""
         if 1036 in self.blocks_dict:
             return cast(PsdThumbnailBlock, self.blocks_dict[1036]).data
         if 1033 in self.blocks_dict:
             return cast(PsdThumbnailBlock, self.blocks_dict[1033]).data
         return None
 
+    @cached_property
+    def blocks_dict(self) -> dict[int, PsdResourceBlockABC]:
+        # TODO: use a multidict
+        blocks_dict: dict[int, PsdResourceBlockABC] = {}
+        for block in self.blocks:
+            if block.resourceid.value not in blocks_dict:
+                blocks_dict[block.resourceid.value] = block
+        return blocks_dict
+
     def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, self.__class__)
             and self.tobytes() == other.tobytes()
         )
 
     def __contains__(self, key: int) -> bool:
@@ -3164,22 +3332,26 @@
 
     def __len__(self) -> int:
         return len(self.blocks)
 
     def __getitem__(self, key: int) -> PsdResourceBlockABC:
         return self.blocks_dict[key]
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[PsdResourceBlockABC, None, None]:
         yield from self.blocks
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} {self.name!r}>'
-
-    def __str__(self) -> str:
-        return indent(repr(self), *self.blocks)
+        sz = len(self.blocks)
+        return indent(
+            f'{self.__class__.__name__}(',
+            f'name={self.name!r},' if self.name else '',
+            f'psdformat={enumstr(self.psdformat)},',
+            f'blocks=[  # {sz}\n    {indent(*self.blocks, sep=",")},\n],',
+            end='\n)',
+        )
 
 
 PSD_KEY_64BIT = {
     # if 64 bit format, these keys use a length count of 8 bytes
     PsdKey.ALPHA,
     PsdKey.FILTER_MASK,
     PsdKey.USER_MASK,
@@ -3244,16 +3416,18 @@
     # PsdKey.CHANNEL_MIXER: PsdUnknown,
     # PsdKey.COLOR_BALANCE: PsdUnknown,
     # PsdKey.COLOR_LOOKUP: PsdUnknown,
     # PsdKey.COMPOSITOR_USED: PsdUnknown,
     # PsdKey.CONTENT_GENERATOR_EXTRA_DATA: PsdUnknown,
     # PsdKey.CURVES: PsdUnknown,
     # PsdKey.EFFECTS_LAYER: PsdUnknown,
+    # PsdKey.FILL_OPACITY: PsdUnknown,
     # PsdKey.FILTER_EFFECTS: PsdUnknown,
     # PsdKey.FILTER_EFFECTS_2: PsdUnknown,
+    # PsdKey.FRAMED_GROUP: PsdUnknown,
     # PsdKey.GRADIENT_FILL_SETTING: PsdUnknown,
     # PsdKey.GRADIENT_MAP: PsdUnknown,
     # PsdKey.HUE_SATURATION: PsdUnknown,
     # PsdKey.HUE_SATURATION_PS4: PsdUnknown,
     # PsdKey.INVERT: PsdUnknown,
     # PsdKey.LEVELS: PsdUnknown,
     # PsdKey.LINKED_LAYER: PsdUnknown,
@@ -3370,68 +3544,66 @@
     return tags
 
 
 def write_psdtags(
     fh: BinaryIO,
     psdformat: PsdFormat,
     /,
-    compression: PsdCompressionType | int | None,
+    compression: PsdCompressionType | None,
     unknown: bool,
     align: int,
     *tags: PsdKeyABC,
 ) -> int:
     """Write sequence of tags to open file."""
     start = fh.tell()
 
     for tag in tags:
         if tag is None:
             continue
         if isinstance(tag, PsdUnknown):
             if not unknown:
                 continue
-            if tag.psdformat != psdformat:  # type: ignore
+            if tag.psdformat != psdformat:
                 log_warning(
                     f'<PsdUnknown {tag.key.value.decode()!r}> not written'
                 )
                 continue
         fh.write(psdformat.value)
         psdformat.write_key(fh, tag.key)
         size_pos = fh.tell()
         psdformat.write_size(fh, 0, tag.key)
         pos = fh.tell()
         if isinstance(tag, PsdLayers):
-            tag.write(
-                fh, psdformat, compression=compression, unknown=unknown
-            )  # type: ignore
+            tag.write(fh, psdformat, compression=compression, unknown=unknown)
         else:
             tag.write(fh, psdformat)
         size = fh.tell() - pos
         fh.seek(size_pos)
         psdformat.write_size(fh, size, tag.key)
         fh.seek(size, 1)
         fh.write(b'\0' * ((align - size % align) % align))
 
     return fh.tell() - start
 
 
 def read_tifftag(
-    filename: os.PathLike | str, tag: int | str, /, pageindex: int = 0
-) -> bytes | None:
+    filename: os.PathLike[Any] | str, tag: int | str, /, pageindex: int = 0
+) -> Any:
     """Return tag value from TIFF file."""
-    from tifffile import TiffFile  # type: ignore
+    from tifffile import TiffFile
 
     with TiffFile(filename) as tif:
         data = tif.pages[pageindex].tags.valueof(tag)
         # if data is None:
         #     raise ValueError(f'TIFF file contains no tag {tag!r}')
     return data
 
 
 def compress(
-    data: numpy.ndarray, compression: PsdCompressionType, rlecountfmt: str
+    data: NDArray[Any], compression: PsdCompressionType, rlecountfmt: str
 ) -> bytes:
     """Return compressed numpy array."""
     if data.dtype.char not in 'BHf':
         raise ValueError(f'data type {data.dtype!r} not supported')
 
     if data.size == 0:
         return b''
@@ -3462,17 +3634,17 @@
     raise ValueError(f'unknown compression type {compression!r}')
 
 
 def decompress(
     data: bytes,
     compression: PsdCompressionType,
     shape: tuple[int, ...],
-    dtype: numpy.dtype,
+    dtype: numpy.dtype[Any],
     rlecountfmt: str,
-) -> numpy.ndarray:
+) -> NDArray[Any]:
     """Return decompressed numpy array."""
     if dtype.char not in 'BHf':
         raise ValueError(f'data type {dtype!r} not supported')
 
     uncompressed_size = product(shape) * dtype.itemsize
 
     if uncompressed_size == 0:
@@ -3501,18 +3673,18 @@
         data = imagecodecs.packbits_decode(data[offset:])
         return numpy.frombuffer(data, dtype=dtype).reshape(shape).copy()
 
     raise ValueError(f'unknown compression type {compression!r}')
 
 
 def overlay(
-    *layers: tuple[numpy.ndarray, tuple[int, int] | None],
+    *layers: tuple[NDArray[Any], tuple[int, int] | None],
     shape: tuple[int, ...] | None = None,
     vmax: float | None = None,
-) -> numpy.ndarray:
+) -> NDArray[Any]:
     """Return overlay of image layers with unassociated alpha channels.
 
     Parameters:
         layers:
             RGBA image array and offset of layer in canvas.
             Layers must not exceed the canvas boundaries and must all
             have the same data types. Alpha channels are unassociated.
@@ -3532,15 +3704,17 @@
         if dtype.kind == 'f':
             vmax = 1.0
         else:
             vmax = numpy.iinfo(dtype).max
     if shape is None:
         shape = layers[0][0].shape
 
-    def over(b, a, offset) -> None:
+    def over(
+        b: NDArray[Any], a: NDArray[Any], offset: tuple[int, int] | None
+    ) -> None:
         assert shape is not None
         if offset is None:
             offset = (0, 0)
         if (
             offset[0] < 0
             or offset[1] < 0
             or offset[0] + a.shape[0] > shape[0]
@@ -3560,35 +3734,60 @@
     composite = numpy.zeros((*shape, 4))
     for layer in layers:
         over(composite, layer[0] / vmax, layer[1])
     composite *= vmax
     return composite.astype(dtype)
 
 
-def log_warning(msg, *args, **kwargs):
+def log_warning(msg: Any, *args: Any, **kwargs: Any) -> None:
     """Log message with level WARNING."""
     import logging
 
     logging.getLogger(__name__).warning(msg, *args, **kwargs)
 
 
 def product(iterable: Iterable[int]) -> int:
     """Return product of sequence of numbers."""
     prod = 1
     for i in iterable:
         prod *= i
     return prod
 
 
-def indent(*args) -> str:
+def indent(*args: Any, sep='', end='') -> str:
     """Return joined string representations of objects with indented lines."""
-    text = '\n'.join(str(arg) for arg in args)
-    return '\n'.join(
-        ('  ' + line if line else line) for line in text.splitlines() if line
-    )[2:]
+    text = (sep + '\n').join(
+        arg if isinstance(arg, str) else repr(arg) for arg in args
+    )
+    return (
+        '\n'.join(
+            ('    ' + line if line else line)
+            for line in text.splitlines()
+            if line
+        )[4:]
+        + end
+    )
+
+
+def enumstr(v: enum.Enum | None, /) -> str:
+    """Return IntEnum or IntFlag as str."""
+    # repr() and str() of enums are type, value, and version dependent
+    if v is None:
+        return 'None'
+    # return f'{v.__class__.__name__}({v.value})'
+    s = repr(v)
+    s = s[1:].split(':', 1)[0]
+    if 'UNKNOWN' in s:
+        s = f'{v.__class__.__name__}({v.value})'
+    elif '|' in s:
+        # IntFlag combination
+        s = s.replace('|', ' | ' + v.__class__.__name__ + '.')
+    elif not hasattr(v, 'name') or v.name is None:
+        s = f'{v.__class__.__name__}({v.value})'
+    return s
 
 
 def test(verbose: bool = False) -> None:
     """Test TiffImageSourceData and TiffImageResources classes."""
     from glob import glob
     import tifffile
     import imagecodecs
@@ -3720,15 +3919,15 @@
                 isd = TiffImageSourceData.frombytes(imagesourcedata, name=name)
                 print(isd)
                 print()
                 if isd.layers and len(files) == 1:
                     for layer in isd.layers:
                         image = layer.asarray()
                         if image.size > 0:
-                            imshow(image, title=repr(layer))
+                            imshow(image, title=layer.title)
                             doplot = True
 
             if imageresources is not None:
                 irs = TiffImageResources.frombytes(imageresources, name=name)
                 print(irs)
                 print()
 
@@ -3737,22 +3936,22 @@
                 elif 1033 in irs:
                     thumbnailblock = cast(PsdThumbnailBlock, irs[1033])
                 else:
                     thumbnailblock = None
                 if thumbnailblock is not None:
                     thumbnail = thumbnailblock.data
                     if thumbnail.size > 0:
-                        imshow(thumbnail, title=repr(thumbnailblock))
+                        imshow(thumbnail, title=thumbnailblock.title)
                         doplot = True
 
             if doplot:
                 pyplot.show()
 
         except ValueError as exc:
-            # raise  # enable for debugging
+            raise  # enable for debugging
             print(fname, exc)
             continue
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `psdtags-2023.2.8/psdtags.egg-info/PKG-INFO` & `psdtags-2023.4.30/psdtags.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: psdtags
-Version: 2023.2.8
+Version: 2023.4.30
 Summary: Read and write layered TIFF ImageSourceData and ImageResources tags
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psdtags/issues
 Project-URL: Source Code, https://github.com/cgohlke/psdtags
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
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
 
@@ -28,24 +27,25 @@
 Psdtags is a Python library to read and write the Adobe Photoshop(r) specific
 ImageResources (#34377) and ImageSourceData (#37724) TIFF tags, which contain
 image resource blocks, layer and mask information found in a typical layered
 TIFF file created by Photoshop.
 
 The format is specified in the
 `Adobe Photoshop TIFF Technical Notes (March 22, 2002)
-<https://www.adobe.io/open/standards/TIFF.html>`_
+<https://www.awaresystems.be/imaging/tiff/specification/TIFFphotoshop.pdf>`_
 and
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.2.8
+:Version: 2023.4.30
+:DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
 
@@ -62,23 +62,36 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.10, 3.11.2 <https://www.python.org>`_
-- `NumPy 1.23.5 <https://pypi.org/project/numpy/>`_
-- `Imagecodecs 2023.1.23 <https://pypi.org/project/imagecodecs/>`_ (optional)
-- `Tifffile 2023.2.3 <https://pypi.org/project/tifffile/>`_  (optional)
-- `Matplotlib 3.6.3 <https://pypi.org/project/matplotlib/>`_  (optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
+  (required for compressing/decompressing image data)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12
+  (required for reading/writing tags from/to TIFF files)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+  (required for plotting)
 
 Revisions
 ---------
 
+2023.4.30
+
+- Few API changes (breaking).
+- Improve object repr.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
+2023.2.18
+
+- Allow unknown PsdKeys (#5).
+
 2023.2.8
 
 - Change PsdPoint and PsdReferencePoint signatures (breaking).
 - Add helper function to create composite from layers.
 
 2022.8.25
 
@@ -111,15 +124,15 @@
 - Initial release.
 
 Notes
 -----
 
 The API is not stable yet and might change between revisions.
 
-This module has been tested with a limited number of files only.
+This library has been tested with a limited number of files only.
 
 Additional layer information is not yet supported.
 
 Consider `psd-tools <https://github.com/psd-tools/psd-tools>`_ and
 `pytoshop <https://github.com/mdboom/pytoshop>`_  for working with
 Adobe Photoshop PSD files.
 
@@ -171,7 +184,10 @@
 >>> assert isd == TiffImageSourceData.fromtiff('_layered.tif')
 >>> assert res == TiffImageResources.fromtiff('_layered.tif')
 
 View the layer and mask information as well as the image resource blocks in
 a layered TIFF file from a command line::
 
     python -m psdtags layered.tif
+
+Refer to the `layered_tiff.py` example in the source distribution for
+creating a layered TIFF file from individual layer images.
```

### Comparing `psdtags-2023.2.8/setup.py` & `psdtags-2023.4.30/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,28 +61,21 @@
         'Bug Tracker': 'https://github.com/cgohlke/psdtags/issues',
         'Source Code': 'https://github.com/cgohlke/psdtags',
         # 'Documentation': 'https://',
     },
     packages=['psdtags'],
     entry_points={'console_scripts': ['psdtags = psdtags.psdtags:main']},
     python_requires='>=3.8',
-    install_requires=['numpy>=1.19.2'],
-    extras_require={
-        'all': [
-            'matplotlib>=3.3',
-            'tifffile>=2021.11.2',
-            'imagecodecs>=2021.11.20',
-        ]
-    },
+    install_requires=['numpy'],
+    extras_require={'all': ['matplotlib', 'tifffile', 'imagecodecs']},
     platforms=['any'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: BSD License',
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

