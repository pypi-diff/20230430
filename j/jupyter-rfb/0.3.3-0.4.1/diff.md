# Comparing `tmp/jupyter_rfb-0.3.3.tar.gz` & `tmp/jupyter_rfb-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_rfb-0.3.3.tar", last modified: Fri Feb 24 11:06:33 2023, max compression
+gzip compressed data, was "jupyter_rfb-0.4.1.tar", last modified: Sun Apr 30 21:36:11 2023, max compression
```

## Comparing `jupyter_rfb-0.3.3.tar` & `jupyter_rfb-0.4.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:33.194437 jupyter_rfb-0.3.3/
--rw-r--r--   0 almar      (501) staff       (20)     1062 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/LICENSE
--rw-r--r--   0 almar      (501) staff       (20)      386 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/MANIFEST.in
--rw-r--r--   0 almar      (501) staff       (20)      824 2023-02-24 11:06:33.194681 jupyter_rfb-0.3.3/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     1880 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/README.md
--rw-r--r--   0 almar      (501) staff       (20)      182 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/install.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:32.488379 jupyter_rfb-0.3.3/js/
--rw-r--r--   0 almar      (501) staff       (20)      455 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/js/.eslintrc.json
--rw-r--r--   0 almar      (501) staff       (20)      157 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/js/README.md
--rw-r--r--   0 almar      (501) staff       (20)      647 2023-02-20 11:47:49.000000 jupyter_rfb-0.3.3/js/amd-public-path.js
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:32.493555 jupyter_rfb-0.3.3/js/dist/
--rw-r--r--   0 almar      (501) staff       (20)     7857 2023-02-24 11:06:24.000000 jupyter_rfb-0.3.3/js/dist/index.js
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:32.544172 jupyter_rfb-0.3.3/js/lib/
--rw-r--r--   0 almar      (501) staff       (20)      459 2023-02-20 11:47:49.000000 jupyter_rfb-0.3.3/js/lib/extension.js
--rw-r--r--   0 almar      (501) staff       (20)      185 2023-02-20 11:47:49.000000 jupyter_rfb-0.3.3/js/lib/index.js
--rw-r--r--   0 almar      (501) staff       (20)      522 2023-02-20 11:47:49.000000 jupyter_rfb-0.3.3/js/lib/labplugin.js
--rw-r--r--   0 almar      (501) staff       (20)    17261 2023-02-24 11:04:02.000000 jupyter_rfb-0.3.3/js/lib/widget.js
--rw-r--r--   0 almar      (501) staff       (20)     1456 2023-02-20 11:47:49.000000 jupyter_rfb-0.3.3/js/package.json
--rw-r--r--   0 almar      (501) staff       (20)     2828 2023-02-20 11:47:49.000000 jupyter_rfb-0.3.3/js/webpack.config.js
--rw-r--r--   0 almar      (501) staff       (20)   182106 2023-02-24 11:06:22.000000 jupyter_rfb-0.3.3/js/yarn.lock
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:32.687360 jupyter_rfb-0.3.3/jupyter_rfb/
--rw-r--r--   0 almar      (501) staff       (20)     1842 2023-02-24 11:04:02.000000 jupyter_rfb-0.3.3/jupyter_rfb/__init__.py
--rw-r--r--   0 almar      (501) staff       (20)     3552 2023-02-17 06:37:49.000000 jupyter_rfb-0.3.3/jupyter_rfb/_jpg.py
--rw-r--r--   0 almar      (501) staff       (20)     2416 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/jupyter_rfb/_png.py
--rw-r--r--   0 almar      (501) staff       (20)     4961 2023-02-24 11:04:02.000000 jupyter_rfb-0.3.3/jupyter_rfb/_utils.py
--rw-r--r--   0 almar      (501) staff       (20)      421 2023-02-24 11:06:05.000000 jupyter_rfb-0.3.3/jupyter_rfb/_version.py
--rw-r--r--   0 almar      (501) staff       (20)     4652 2022-09-29 21:52:25.000000 jupyter_rfb-0.3.3/jupyter_rfb/events.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:32.845179 jupyter_rfb-0.3.3/jupyter_rfb/labextension/
--rw-r--r--   0 almar      (501) staff       (20)     1572 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb/labextension/package.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:32.987990 jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/
--rw-r--r--   0 almar      (501) staff       (20)     7489 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/261.b63982d0d8bbb580738f.js
--rw-r--r--   0 almar      (501) staff       (20)     7120 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/920.1ac74c193418012f2d62.js
--rw-r--r--   0 almar      (501) staff       (20)     6441 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/remoteEntry.e973b45de9178a27e295.js
--rw-r--r--   0 almar      (501) staff       (20)      118 2023-02-24 11:06:30.000000 jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/style.js
--rw-r--r--   0 almar      (501) staff       (20)       20 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:33.097902 jupyter_rfb-0.3.3/jupyter_rfb/nbextension/
--rw-r--r--   0 almar      (501) staff       (20)      531 2023-02-24 11:06:24.000000 jupyter_rfb-0.3.3/jupyter_rfb/nbextension/extension.js
--rw-r--r--   0 almar      (501) staff       (20)     7857 2023-02-24 11:06:24.000000 jupyter_rfb-0.3.3/jupyter_rfb/nbextension/index.js
--rw-r--r--   0 almar      (501) staff       (20)    16613 2023-02-24 11:04:02.000000 jupyter_rfb-0.3.3/jupyter_rfb/widget.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:32.743682 jupyter_rfb-0.3.3/jupyter_rfb.egg-info/
--rw-r--r--   0 almar      (501) staff       (20)      824 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb.egg-info/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     1120 2023-02-24 11:06:32.000000 jupyter_rfb-0.3.3/jupyter_rfb.egg-info/SOURCES.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb.egg-info/dependency_links.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2022-02-04 09:25:53.000000 jupyter_rfb-0.3.3/jupyter_rfb.egg-info/not-zip-safe
--rw-r--r--   0 almar      (501) staff       (20)       46 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb.egg-info/requires.txt
--rw-r--r--   0 almar      (501) staff       (20)       12 2023-02-24 11:06:31.000000 jupyter_rfb-0.3.3/jupyter_rfb.egg-info/top_level.txt
--rw-r--r--   0 almar      (501) staff       (20)       65 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/jupyter_rfb.json
--rw-r--r--   0 almar      (501) staff       (20)      153 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/pyproject.toml
--rw-r--r--   0 almar      (501) staff       (20)      460 2023-02-24 11:06:33.198589 jupyter_rfb-0.3.3/setup.cfg
--rw-r--r--   0 almar      (501) staff       (20)     2525 2023-02-20 11:47:49.000000 jupyter_rfb-0.3.3/setup.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-02-24 11:06:33.193700 jupyter_rfb-0.3.3/tests/
--rw-r--r--   0 almar      (501) staff       (20)     3443 2023-02-17 06:37:49.000000 jupyter_rfb-0.3.3/tests/test_jpg.py
--rw-r--r--   0 almar      (501) staff       (20)     2614 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/tests/test_png.py
--rw-r--r--   0 almar      (501) staff       (20)     3670 2023-02-17 06:37:49.000000 jupyter_rfb-0.3.3/tests/test_utils.py
--rw-r--r--   0 almar      (501) staff       (20)     7929 2022-02-04 09:25:28.000000 jupyter_rfb-0.3.3/tests/test_widget.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.780971 jupyter_rfb-0.4.1/
+-rw-r--r--   0 almar      (501) staff       (20)     1062 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)      386 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/MANIFEST.in
+-rw-r--r--   0 almar      (501) staff       (20)      824 2023-04-30 21:36:11.781156 jupyter_rfb-0.4.1/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     1880 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/README.md
+-rw-r--r--   0 almar      (501) staff       (20)      182 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/install.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.567256 jupyter_rfb-0.4.1/js/
+-rw-r--r--   0 almar      (501) staff       (20)      455 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/js/.eslintrc.json
+-rw-r--r--   0 almar      (501) staff       (20)      157 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/js/README.md
+-rw-r--r--   0 almar      (501) staff       (20)      647 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.1/js/amd-public-path.js
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.582595 jupyter_rfb-0.4.1/js/dist/
+-rw-r--r--   0 almar      (501) staff       (20)     7981 2023-04-30 21:36:03.000000 jupyter_rfb-0.4.1/js/dist/index.js
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.622914 jupyter_rfb-0.4.1/js/lib/
+-rw-r--r--   0 almar      (501) staff       (20)      459 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.1/js/lib/extension.js
+-rw-r--r--   0 almar      (501) staff       (20)      185 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.1/js/lib/index.js
+-rw-r--r--   0 almar      (501) staff       (20)      522 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.1/js/lib/labplugin.js
+-rw-r--r--   0 almar      (501) staff       (20)    17488 2023-04-30 21:35:07.000000 jupyter_rfb-0.4.1/js/lib/widget.js
+-rw-r--r--   0 almar      (501) staff       (20)     1456 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.1/js/package.json
+-rw-r--r--   0 almar      (501) staff       (20)     2828 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.1/js/webpack.config.js
+-rw-r--r--   0 almar      (501) staff       (20)   182106 2023-02-24 11:06:22.000000 jupyter_rfb-0.4.1/js/yarn.lock
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.661293 jupyter_rfb-0.4.1/jupyter_rfb/
+-rw-r--r--   0 almar      (501) staff       (20)     1842 2023-02-24 11:04:02.000000 jupyter_rfb-0.4.1/jupyter_rfb/__init__.py
+-rw-r--r--   0 almar      (501) staff       (20)     3552 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.1/jupyter_rfb/_jpg.py
+-rw-r--r--   0 almar      (501) staff       (20)     2416 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/jupyter_rfb/_png.py
+-rw-r--r--   0 almar      (501) staff       (20)     4961 2023-02-24 11:04:02.000000 jupyter_rfb-0.4.1/jupyter_rfb/_utils.py
+-rw-r--r--   0 almar      (501) staff       (20)      421 2023-04-30 21:35:44.000000 jupyter_rfb-0.4.1/jupyter_rfb/_version.py
+-rw-r--r--   0 almar      (501) staff       (20)     4652 2022-09-29 21:52:25.000000 jupyter_rfb-0.4.1/jupyter_rfb/events.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.711572 jupyter_rfb-0.4.1/jupyter_rfb/labextension/
+-rw-r--r--   0 almar      (501) staff       (20)     1572 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb/labextension/package.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.758894 jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/
+-rw-r--r--   0 almar      (501) staff       (20)     7613 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/261.9672f89ed6262263983a.js
+-rw-r--r--   0 almar      (501) staff       (20)     7244 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/920.a581c03b63703f9841ad.js
+-rw-r--r--   0 almar      (501) staff       (20)     6441 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/remoteEntry.51511a582c8e65cc4305.js
+-rw-r--r--   0 almar      (501) staff       (20)      118 2023-04-30 21:36:09.000000 jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/style.js
+-rw-r--r--   0 almar      (501) staff       (20)       20 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.760693 jupyter_rfb-0.4.1/jupyter_rfb/nbextension/
+-rw-r--r--   0 almar      (501) staff       (20)      531 2023-04-30 21:36:03.000000 jupyter_rfb-0.4.1/jupyter_rfb/nbextension/extension.js
+-rw-r--r--   0 almar      (501) staff       (20)     7981 2023-04-30 21:36:03.000000 jupyter_rfb-0.4.1/jupyter_rfb/nbextension/index.js
+-rw-r--r--   0 almar      (501) staff       (20)    16613 2023-02-24 11:04:02.000000 jupyter_rfb-0.4.1/jupyter_rfb/widget.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.710989 jupyter_rfb-0.4.1/jupyter_rfb.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)      824 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     1120 2023-04-30 21:36:11.000000 jupyter_rfb-0.4.1/jupyter_rfb.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2022-02-04 09:25:53.000000 jupyter_rfb-0.4.1/jupyter_rfb.egg-info/not-zip-safe
+-rw-r--r--   0 almar      (501) staff       (20)       46 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb.egg-info/requires.txt
+-rw-r--r--   0 almar      (501) staff       (20)       12 2023-04-30 21:36:10.000000 jupyter_rfb-0.4.1/jupyter_rfb.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)       65 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/jupyter_rfb.json
+-rw-r--r--   0 almar      (501) staff       (20)      153 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/pyproject.toml
+-rw-r--r--   0 almar      (501) staff       (20)      460 2023-04-30 21:36:11.784195 jupyter_rfb-0.4.1/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2525 2023-04-30 21:11:03.000000 jupyter_rfb-0.4.1/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-30 21:36:11.779333 jupyter_rfb-0.4.1/tests/
+-rw-r--r--   0 almar      (501) staff       (20)     3443 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.1/tests/test_jpg.py
+-rw-r--r--   0 almar      (501) staff       (20)     2614 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/tests/test_png.py
+-rw-r--r--   0 almar      (501) staff       (20)     3670 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.1/tests/test_utils.py
+-rw-r--r--   0 almar      (501) staff       (20)     7929 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.1/tests/test_widget.py
```

### Comparing `jupyter_rfb-0.3.3/LICENSE` & `jupyter_rfb-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/PKG-INFO` & `jupyter_rfb-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_rfb
-Version: 0.3.3
+Version: 0.4.1
 Summary: Remote Frame Buffer for Jupyter
 Home-page: https://github.com/vispy/jupyter_rfb
 Author: Almar Klein
 Author-email: almar@almarklein.org
 License: MIT
 Keywords: ipython,jupyter,widgets,visualization,remote frame buffer
 Classifier: Development Status :: 4 - Beta
@@ -13,11 +13,11 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 License-File: LICENSE
 
 Remote Frame Buffer for Jupyter
```

### Comparing `jupyter_rfb-0.3.3/README.md` & `jupyter_rfb-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/js/amd-public-path.js` & `jupyter_rfb-0.4.1/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/js/dist/index.js` & `jupyter_rfb-0.4.1/js/dist/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
                 const n = new URL(s.uri, document.location);
                 n.pathname = n.pathname.slice(0, n.pathname.lastIndexOf("/") + 1), i.p = `${n.origin}${n.pathname}`
             },
             681: (e, t, i) => {
                 i.r(t), i.d(t, {
                     RemoteFrameBufferModel: () => n,
                     RemoteFrameBufferView: () => l,
-                    version: () => _.i8
+                    version: () => a.i8
                 });
                 var s = i(146);
                 class n extends s.DOMWidgetModel {
                     defaults() {
                         return {
                             ...super.defaults(),
                             _model_name: "RemoteFrameBufferModel",
@@ -145,15 +145,15 @@
                             e._wheel_state.dx += i.deltaX * s, e._wheel_state.dy += i.deltaY * s, e._wheel_state.pending || (e._wheel_state.pending = !0, e._wheel_state.e = i, window.setTimeout(t, 20)), i.altKey || i.preventDefault()
                         })), this.focus_el.addEventListener("keydown", i, !0), this.focus_el.addEventListener("keyup", i, !0)
                     }
                     remove() {
                         super.remove.apply(this, arguments), window.setTimeout(this.model.collect_view_img_elements.bind(this.model), 10)
                     }
                     _check_resize() {
-                        if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), void(this.el.style.height = this.model.get("css_height"));
+                        if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.maxWidth = Math.max(1024, window.innerWidth) + "px", void(this.el.style.maxHeight = Math.max(1024, window.innerHeight) + "px");
                         let e = this.img.clientWidth,
                             t = this.img.clientHeight,
                             i = window.devicePixelRatio;
                         0 === e && 0 === t || this._current_size[0] === e && this._current_size[1] === t && this._current_size[2] === i || (this._current_size = [e, t, i], this.send_throttled({
                             event_type: "resize",
                             width: e,
                             height: t,
@@ -167,16 +167,16 @@
                             var i, s, n, l = null,
                                 o = 0,
                                 r = function() {
                                     o = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
                                 };
                             return function() {
                                 var h = Date.now(),
-                                    _ = t - (h - o);
-                                return i = this, s = arguments, _ <= 0 || _ > t ? (l && (clearTimeout(l), l = null), o = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(r, _)), n
+                                    a = t - (h - o);
+                                return i = this, s = arguments, a <= 0 || a > t ? (l && (clearTimeout(l), l = null), o = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(r, a)), n
                             }
                         }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
                     }
                 }
                 var o = {
                     Ctrl: "Control",
                     Del: "Delete",
@@ -188,24 +188,24 @@
                 }
 
                 function h(e, t, i, s) {
                     let n = e.getBoundingClientRect(),
                         l = [n.left, n.top],
                         o = Number(t.clientX - l[0]),
                         h = Number(t.clientY - l[1]),
-                        _ = {},
-                        a = 0;
+                        a = {},
+                        _ = 0;
                     for (let e in i) {
                         let t = i[e],
                             s = {
                                 x: Number(t.clientX - l[0]),
                                 y: Number(t.clientY - l[1]),
                                 pressure: t.pressure
                             };
-                        _[t.pointerId] = s, a += 1
+                        a[t.pointerId] = s, _ += 1
                     }
                     var d = {
                             0: 1,
                             1: 3,
                             2: 2,
                             3: 4,
                             4: 5,
@@ -216,19 +216,19 @@
                     return {
                         event_type: s,
                         x: o,
                         y: h,
                         button: d,
                         buttons: m,
                         modifiers: r(t),
-                        ntouches: a,
-                        touches: _
+                        ntouches: _,
+                        touches: a
                     }
                 }
-                const _ = {
+                const a = {
                     i8: "0.1.0"
                 }
             },
             146: e => {
                 e.exports = t
             },
             325: t => {
```

### Comparing `jupyter_rfb-0.3.3/js/lib/labplugin.js` & `jupyter_rfb-0.4.1/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/js/lib/widget.js` & `jupyter_rfb-0.4.1/js/lib/widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -355,14 +355,17 @@
         // Called when the widget resizes.
         // During initialization Jupyter sets .el.style.width and .height to the empty string.
         // It looks like VS Code tries harder to do this than the notebook,
         // so we need to check for this pretty aggressively.
         if (!this.el.style.width && this.model.get('css_width')) {
             this.el.style.width = this.model.get('css_width');
             this.el.style.height = this.model.get('css_height');
+            // prevent massive size due to auto-scroll (issue #62)
+            this.el.style.maxWidth = Math.max(1024, window.innerWidth) + 'px';
+            this.el.style.maxHeight = Math.max(1024, window.innerHeight) + 'px';
             return; // Don't send a resize event now
         }
         // Width and height are in logical pixels.
         let w = this.img.clientWidth;
         let h = this.img.clientHeight;
         let r = window.devicePixelRatio;
         if (w === 0 && h === 0) {
```

### Comparing `jupyter_rfb-0.3.3/js/package.json` & `jupyter_rfb-0.4.1/js/package.json`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/js/webpack.config.js` & `jupyter_rfb-0.4.1/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/js/yarn.lock` & `jupyter_rfb-0.4.1/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/__init__.py` & `jupyter_rfb-0.4.1/jupyter_rfb/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/_jpg.py` & `jupyter_rfb-0.4.1/jupyter_rfb/_jpg.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/_png.py` & `jupyter_rfb-0.4.1/jupyter_rfb/_png.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/_utils.py` & `jupyter_rfb-0.4.1/jupyter_rfb/_utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/events.py` & `jupyter_rfb-0.4.1/jupyter_rfb/events.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/labextension/package.json` & `jupyter_rfb-0.4.1/jupyter_rfb/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.51511a582c8e65cc4305.js'}}"}*

```diff
@@ -13,15 +13,15 @@
     "files": [
         "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e973b45de9178a27e295.js"
+            "load": "static/remoteEntry.51511a582c8e65cc4305.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../jupyter_rfb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/261.b63982d0d8bbb580738f.js` & `jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/261.9672f89ed6262263983a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 "use strict";
 (self.webpackChunkjupyter_rfb = self.webpackChunkjupyter_rfb || []).push([
     [261, 920], {
         920: (e, t, i) => {
             i.r(t), i.d(t, {
                 RemoteFrameBufferModel: () => n,
-                RemoteFrameBufferView: () => r,
+                RemoteFrameBufferView: () => l,
                 version: () => _.i8
             });
             var s = i(382);
             class n extends s.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
@@ -76,15 +76,15 @@
                 }
                 close() {
                     this.send({
                         event_type: "close"
                     }), super.close.apply(this, arguments)
                 }
             }
-            class r extends s.DOMWidgetView {
+            class l extends s.DOMWidgetView {
                 render() {
                     var e = this;
 
                     function t() {
                         let t = e._wheel_state.e,
                             i = e.img.getBoundingClientRect(),
                             s = {
@@ -98,15 +98,15 @@
                         e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
                     }
 
                     function i(t) {
                         if (null === e.el.offsetParent) return;
                         let i = {
                             event_type: "key_" + t.type.slice(3),
-                            key: l[t.key] || t.key,
+                            key: r[t.key] || t.key,
                             modifiers: o(t)
                         };
                         t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
                     }
                     this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
                         if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
                     }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
@@ -140,64 +140,64 @@
                         e._wheel_state.dx += i.deltaX * s, e._wheel_state.dy += i.deltaY * s, e._wheel_state.pending || (e._wheel_state.pending = !0, e._wheel_state.e = i, window.setTimeout(t, 20)), i.altKey || i.preventDefault()
                     })), this.focus_el.addEventListener("keydown", i, !0), this.focus_el.addEventListener("keyup", i, !0)
                 }
                 remove() {
                     super.remove.apply(this, arguments), window.setTimeout(this.model.collect_view_img_elements.bind(this.model), 10)
                 }
                 _check_resize() {
-                    if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), void(this.el.style.height = this.model.get("css_height"));
+                    if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.maxWidth = Math.max(1024, window.innerWidth) + "px", void(this.el.style.maxHeight = Math.max(1024, window.innerHeight) + "px");
                     let e = this.img.clientWidth,
                         t = this.img.clientHeight,
                         i = window.devicePixelRatio;
                     0 === e && 0 === t || this._current_size[0] === e && this._current_size[1] === t && this._current_size[2] === i || (this._current_size = [e, t, i], this.send_throttled({
                         event_type: "resize",
                         width: e,
                         height: t,
                         pixel_ratio: i
                     }, 200))
                 }
                 send_throttled(e, t) {
                     let i = e.event_type || "",
                         s = this._throttlers[i];
                     void 0 === s && (s = function(e, t) {
-                        var i, s, n, r = null,
-                            l = 0,
+                        var i, s, n, l = null,
+                            r = 0,
                             o = function() {
-                                l = Date.now(), r = null, n = e.apply(i, s), r || (i = s = null)
+                                r = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
                             };
                         return function() {
                             var h = Date.now(),
-                                _ = t - (h - l);
-                            return i = this, s = arguments, _ <= 0 || _ > t ? (r && (clearTimeout(r), r = null), l = h, n = e.apply(i, s), r || (i = s = null)) : r || (r = setTimeout(o, _)), n
+                                _ = t - (h - r);
+                            return i = this, s = arguments, _ <= 0 || _ > t ? (l && (clearTimeout(l), l = null), r = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(o, _)), n
                         }
                     }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
                 }
             }
-            var l = {
+            var r = {
                 Ctrl: "Control",
                 Del: "Delete",
                 Esc: "Escape"
             };
 
             function o(e) {
-                return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => l[e] || e))
+                return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => r[e] || e))
             }
 
             function h(e, t, i, s) {
                 let n = e.getBoundingClientRect(),
-                    r = [n.left, n.top],
-                    l = Number(t.clientX - r[0]),
-                    h = Number(t.clientY - r[1]),
+                    l = [n.left, n.top],
+                    r = Number(t.clientX - l[0]),
+                    h = Number(t.clientY - l[1]),
                     _ = {},
                     a = 0;
                 for (let e in i) {
                     let t = i[e],
                         s = {
-                            x: Number(t.clientX - r[0]),
-                            y: Number(t.clientY - r[1]),
+                            x: Number(t.clientX - l[0]),
+                            y: Number(t.clientY - l[1]),
                             pressure: t.pressure
                         };
                     _[t.pointerId] = s, a += 1
                 }
                 var d = {
                         0: 1,
                         1: 3,
@@ -206,15 +206,15 @@
                         4: 5,
                         5: 6
                     } [t.button] || 0,
                     m = [];
                 for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && m.push(e + 1);
                 return {
                     event_type: s,
-                    x: l,
+                    x: r,
                     y: h,
                     button: d,
                     buttons: m,
                     modifiers: o(t),
                     ntouches: a,
                     touches: _
                 }
@@ -222,15 +222,15 @@
             const _ = {
                 i8: "0.1.0"
             }
         },
         261: (e, t, i) => {
             i.r(t), i.d(t, {
                 remoteFrameBufferPlugin: () => n,
-                default: () => r
+                default: () => l
             });
             var s = i(920);
             const n = {
                     id: "jupyter_rfb:plugin",
                     requires: [i(382).IJupyterWidgetRegistry],
                     activate: function(e, t) {
                         t.registerWidget({
@@ -240,11 +240,11 @@
                                 RemoteFrameBufferModel: s.RemoteFrameBufferModel,
                                 RemoteFrameBufferView: s.RemoteFrameBufferView
                             }
                         })
                     },
                     autoStart: !0
                 },
-                r = n
+                l = n
         }
     }
 ]);
```

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/920.1ac74c193418012f2d62.js` & `jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/920.a581c03b63703f9841ad.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -89,49 +89,49 @@
                             i = e.img.getBoundingClientRect(),
                             s = {
                                 event_type: "wheel",
                                 x: Number(t.clientX - i.left),
                                 y: Number(t.clientY - i.top),
                                 dx: e._wheel_state.dx,
                                 dy: e._wheel_state.dy,
-                                modifiers: r(t)
+                                modifiers: o(t)
                             };
                         e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
                     }
 
                     function i(t) {
                         if (null === e.el.offsetParent) return;
                         let i = {
                             event_type: "key_" + t.type.slice(3),
-                            key: o[t.key] || t.key,
-                            modifiers: r(t)
+                            key: h[t.key] || t.key,
+                            modifiers: o(t)
                         };
                         t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
                     }
                     this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
                         if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
                     }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
                         this.el.style.width = this.model.get("css_width")
                     }), this), this.model.on("change:css_height", (function() {
                         this.el.style.height = this.model.get("css_height")
                     }), this), this.model.on("change:resizable", (function() {
                         this.el.style.resize = this.model.get("resizable") ? "both" : "none"
                     }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this.img.addEventListener("pointerdown", (function(t) {
                         e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
-                        let i = h(e.img, t, e._pointers, "pointer_down");
+                        let i = r(e.img, t, e._pointers, "pointer_down");
                         e.send(i), t.altKey || t.preventDefault()
                     })), this.img.addEventListener("lostpointercapture", (function(t) {
-                        let i = h(e.img, t, e._pointers, "pointer_up");
+                        let i = r(e.img, t, e._pointers, "pointer_up");
                         delete e._pointers[t.pointerId], e.send(i)
                     })), this.img.addEventListener("pointermove", (function(t) {
                         if (void 0 === e._pointers[t.pointerId] && Object.keys(e._pointers).length > 0) return;
-                        let i = h(e.img, t, e._pointers, "pointer_move");
+                        let i = r(e.img, t, e._pointers, "pointer_move");
                         e.send_throttled(i, 20)
                     })), this.img.addEventListener("dblclick", (function(t) {
-                        let i = h(e.img, t, {}, "double_click");
+                        let i = r(e.img, t, {}, "double_click");
                         delete i.touches, delete i.ntouches, e.send(i), t.altKey || t.preventDefault()
                     })), this._wheel_state = {
                         dx: 0,
                         dy: 0,
                         e: null,
                         pending: !1
                     }, this.img.addEventListener("wheel", (function(i) {
@@ -140,15 +140,15 @@
                         e._wheel_state.dx += i.deltaX * s, e._wheel_state.dy += i.deltaY * s, e._wheel_state.pending || (e._wheel_state.pending = !0, e._wheel_state.e = i, window.setTimeout(t, 20)), i.altKey || i.preventDefault()
                     })), this.focus_el.addEventListener("keydown", i, !0), this.focus_el.addEventListener("keyup", i, !0)
                 }
                 remove() {
                     super.remove.apply(this, arguments), window.setTimeout(this.model.collect_view_img_elements.bind(this.model), 10)
                 }
                 _check_resize() {
-                    if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), void(this.el.style.height = this.model.get("css_height"));
+                    if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.maxWidth = Math.max(1024, window.innerWidth) + "px", void(this.el.style.maxHeight = Math.max(1024, window.innerHeight) + "px");
                     let e = this.img.clientWidth,
                         t = this.img.clientHeight,
                         i = window.devicePixelRatio;
                     0 === e && 0 === t || this._current_size[0] === e && this._current_size[1] === t && this._current_size[2] === i || (this._current_size = [e, t, i], this.send_throttled({
                         event_type: "resize",
                         width: e,
                         height: t,
@@ -156,70 +156,70 @@
                     }, 200))
                 }
                 send_throttled(e, t) {
                     let i = e.event_type || "",
                         s = this._throttlers[i];
                     void 0 === s && (s = function(e, t) {
                         var i, s, n, l = null,
-                            o = 0,
-                            r = function() {
-                                o = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
+                            h = 0,
+                            o = function() {
+                                h = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
                             };
                         return function() {
-                            var h = Date.now(),
-                                _ = t - (h - o);
-                            return i = this, s = arguments, _ <= 0 || _ > t ? (l && (clearTimeout(l), l = null), o = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(r, _)), n
+                            var r = Date.now(),
+                                _ = t - (r - h);
+                            return i = this, s = arguments, _ <= 0 || _ > t ? (l && (clearTimeout(l), l = null), h = r, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(o, _)), n
                         }
                     }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
                 }
             }
-            var o = {
+            var h = {
                 Ctrl: "Control",
                 Del: "Delete",
                 Esc: "Escape"
             };
 
-            function r(e) {
-                return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => o[e] || e))
+            function o(e) {
+                return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => h[e] || e))
             }
 
-            function h(e, t, i, s) {
+            function r(e, t, i, s) {
                 let n = e.getBoundingClientRect(),
                     l = [n.left, n.top],
-                    o = Number(t.clientX - l[0]),
-                    h = Number(t.clientY - l[1]),
+                    h = Number(t.clientX - l[0]),
+                    r = Number(t.clientY - l[1]),
                     _ = {},
-                    d = 0;
+                    a = 0;
                 for (let e in i) {
                     let t = i[e],
                         s = {
                             x: Number(t.clientX - l[0]),
                             y: Number(t.clientY - l[1]),
                             pressure: t.pressure
                         };
-                    _[t.pointerId] = s, d += 1
+                    _[t.pointerId] = s, a += 1
                 }
-                var a = {
+                var d = {
                         0: 1,
                         1: 3,
                         2: 2,
                         3: 4,
                         4: 5,
                         5: 6
                     } [t.button] || 0,
                     m = [];
                 for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && m.push(e + 1);
                 return {
                     event_type: s,
-                    x: o,
-                    y: h,
-                    button: a,
+                    x: h,
+                    y: r,
+                    button: d,
                     buttons: m,
-                    modifiers: r(t),
-                    ntouches: d,
+                    modifiers: o(t),
+                    ntouches: a,
                     touches: _
                 }
             }
             const _ = {
                 i8: "0.1.0"
             }
         }
```

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/labextension/static/remoteEntry.e973b45de9178a27e295.js` & `jupyter_rfb-0.4.1/jupyter_rfb/labextension/static/remoteEntry.51511a582c8e65cc4305.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -41,21 +41,21 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        261: "b63982d0d8bbb580738f",
+        261: "9672f89ed6262263983a",
         382: "1f3c426f14b6845534ba",
-        920: "1ac74c193418012f2d62"
+        920: "a581c03b63703f9841ad"
     } [e] + ".js?v=" + {
-        261: "b63982d0d8bbb580738f",
+        261: "9672f89ed6262263983a",
         382: "1f3c426f14b6845534ba",
-        920: "1ac74c193418012f2d62"
+        920: "a581c03b63703f9841ad"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
```

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/nbextension/extension.js` & `jupyter_rfb-0.4.1/jupyter_rfb/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/nbextension/index.js` & `jupyter_rfb-0.4.1/jupyter_rfb/nbextension/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
                 const n = new URL(s.uri, document.location);
                 n.pathname = n.pathname.slice(0, n.pathname.lastIndexOf("/") + 1), i.p = `${n.origin}${n.pathname}`
             },
             681: (e, t, i) => {
                 i.r(t), i.d(t, {
                     RemoteFrameBufferModel: () => n,
                     RemoteFrameBufferView: () => l,
-                    version: () => _.i8
+                    version: () => a.i8
                 });
                 var s = i(146);
                 class n extends s.DOMWidgetModel {
                     defaults() {
                         return {
                             ...super.defaults(),
                             _model_name: "RemoteFrameBufferModel",
@@ -145,15 +145,15 @@
                             e._wheel_state.dx += i.deltaX * s, e._wheel_state.dy += i.deltaY * s, e._wheel_state.pending || (e._wheel_state.pending = !0, e._wheel_state.e = i, window.setTimeout(t, 20)), i.altKey || i.preventDefault()
                         })), this.focus_el.addEventListener("keydown", i, !0), this.focus_el.addEventListener("keyup", i, !0)
                     }
                     remove() {
                         super.remove.apply(this, arguments), window.setTimeout(this.model.collect_view_img_elements.bind(this.model), 10)
                     }
                     _check_resize() {
-                        if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), void(this.el.style.height = this.model.get("css_height"));
+                        if (!this.el.style.width && this.model.get("css_width")) return this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.maxWidth = Math.max(1024, window.innerWidth) + "px", void(this.el.style.maxHeight = Math.max(1024, window.innerHeight) + "px");
                         let e = this.img.clientWidth,
                             t = this.img.clientHeight,
                             i = window.devicePixelRatio;
                         0 === e && 0 === t || this._current_size[0] === e && this._current_size[1] === t && this._current_size[2] === i || (this._current_size = [e, t, i], this.send_throttled({
                             event_type: "resize",
                             width: e,
                             height: t,
@@ -167,16 +167,16 @@
                             var i, s, n, l = null,
                                 o = 0,
                                 r = function() {
                                     o = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
                                 };
                             return function() {
                                 var h = Date.now(),
-                                    _ = t - (h - o);
-                                return i = this, s = arguments, _ <= 0 || _ > t ? (l && (clearTimeout(l), l = null), o = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(r, _)), n
+                                    a = t - (h - o);
+                                return i = this, s = arguments, a <= 0 || a > t ? (l && (clearTimeout(l), l = null), o = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(r, a)), n
                             }
                         }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
                     }
                 }
                 var o = {
                     Ctrl: "Control",
                     Del: "Delete",
@@ -188,24 +188,24 @@
                 }
 
                 function h(e, t, i, s) {
                     let n = e.getBoundingClientRect(),
                         l = [n.left, n.top],
                         o = Number(t.clientX - l[0]),
                         h = Number(t.clientY - l[1]),
-                        _ = {},
-                        a = 0;
+                        a = {},
+                        _ = 0;
                     for (let e in i) {
                         let t = i[e],
                             s = {
                                 x: Number(t.clientX - l[0]),
                                 y: Number(t.clientY - l[1]),
                                 pressure: t.pressure
                             };
-                        _[t.pointerId] = s, a += 1
+                        a[t.pointerId] = s, _ += 1
                     }
                     var d = {
                             0: 1,
                             1: 3,
                             2: 2,
                             3: 4,
                             4: 5,
@@ -216,19 +216,19 @@
                     return {
                         event_type: s,
                         x: o,
                         y: h,
                         button: d,
                         buttons: m,
                         modifiers: r(t),
-                        ntouches: a,
-                        touches: _
+                        ntouches: _,
+                        touches: a
                     }
                 }
-                const _ = {
+                const a = {
                     i8: "0.1.0"
                 }
             },
             146: e => {
                 e.exports = t
             },
             325: t => {
```

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb/widget.py` & `jupyter_rfb-0.4.1/jupyter_rfb/widget.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb.egg-info/PKG-INFO` & `jupyter_rfb-0.4.1/jupyter_rfb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-rfb
-Version: 0.3.3
+Version: 0.4.1
 Summary: Remote Frame Buffer for Jupyter
 Home-page: https://github.com/vispy/jupyter_rfb
 Author: Almar Klein
 Author-email: almar@almarklein.org
 License: MIT
 Keywords: ipython,jupyter,widgets,visualization,remote frame buffer
 Classifier: Development Status :: 4 - Beta
@@ -13,11 +13,11 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 License-File: LICENSE
 
 Remote Frame Buffer for Jupyter
```

### Comparing `jupyter_rfb-0.3.3/jupyter_rfb.egg-info/SOURCES.txt` & `jupyter_rfb-0.4.1/jupyter_rfb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 jupyter_rfb.egg-info/PKG-INFO
 jupyter_rfb.egg-info/SOURCES.txt
 jupyter_rfb.egg-info/dependency_links.txt
 jupyter_rfb.egg-info/not-zip-safe
 jupyter_rfb.egg-info/requires.txt
 jupyter_rfb.egg-info/top_level.txt
 jupyter_rfb/labextension/package.json
-jupyter_rfb/labextension/static/261.b63982d0d8bbb580738f.js
-jupyter_rfb/labextension/static/920.1ac74c193418012f2d62.js
-jupyter_rfb/labextension/static/remoteEntry.e973b45de9178a27e295.js
+jupyter_rfb/labextension/static/261.9672f89ed6262263983a.js
+jupyter_rfb/labextension/static/920.a581c03b63703f9841ad.js
+jupyter_rfb/labextension/static/remoteEntry.51511a582c8e65cc4305.js
 jupyter_rfb/labextension/static/style.js
 jupyter_rfb/labextension/static/third-party-licenses.json
 jupyter_rfb/nbextension/extension.js
 jupyter_rfb/nbextension/index.js
 tests/test_jpg.py
 tests/test_png.py
 tests/test_utils.py
```

### Comparing `jupyter_rfb-0.3.3/setup.py` & `jupyter_rfb-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     long_description=LONG_DESCRIPTION,
     include_package_data=True,
     install_requires=[
         "numpy",
         "ipywidgets>=7.6.0,<9",
         "jupyterlab-widgets",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     packages=find_packages(),
     zip_safe=False,
     cmdclass=cmdclass,
     author="Almar Klein",
     author_email="almar@almarklein.org",
     license="MIT",
     url="https://github.com/vispy/jupyter_rfb",
```

### Comparing `jupyter_rfb-0.3.3/tests/test_jpg.py` & `jupyter_rfb-0.4.1/tests/test_jpg.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/tests/test_png.py` & `jupyter_rfb-0.4.1/tests/test_png.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/tests/test_utils.py` & `jupyter_rfb-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.3.3/tests/test_widget.py` & `jupyter_rfb-0.4.1/tests/test_widget.py`

 * *Files identical despite different names*

