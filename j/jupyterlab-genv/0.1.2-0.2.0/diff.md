# Comparing `tmp/jupyterlab_genv-0.1.2.tar.gz` & `tmp/jupyterlab_genv-0.2.0.tar.gz`

## Comparing `jupyterlab_genv-0.1.2.tar` & `jupyterlab_genv-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/.eslintrc.js
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/.stylelintrc
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/MANIFEST.in
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/Test.ipynb
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/install.json
--rw-r--r--   0        0        0   328793 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/package-lock.json
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/tsconfig.json
--rw-r--r--   0        0        0   259047 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/yarn.lock
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyter-config/nb-config/jupyterlab_genv.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyter-config/server-config/jupyterlab_genv.json
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/__init__.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/__main__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/_version.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/genv_provisioner.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/handlers.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/genv/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/genv/control.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/genv/devices.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/genv/envs.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/genv/installation.py
--rw-r--r--   0        0        0    20586 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/build_log.json
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/package.json
--rw-r--r--   0        0        0    18782 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js
--rw-r--r--   0        0        0    16241 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js.map
--rw-r--r--   0        0        0    28617 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/remoteEntry.3f30df1d6370ec409a58.js
--rw-r--r--   0        0        0    27387 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/remoteEntry.3f30df1d6370ec409a58.js.map
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/style.js
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js.map
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js.map
--rw-r--r--   0        0        0   844987 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/resources/readme/activate.gif
--rw-r--r--   0        0        0  1589295 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/resources/readme/attach.gif
--rw-r--r--   0        0        0    40559 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/resources/readme/commands.gif
--rw-r--r--   0        0        0  1278811 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/resources/readme/overview.gif
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/src/dialogs.tsx
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/src/handler.ts
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/src/index.tsx
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/style/index.js
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/LICENSE
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/README.md
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 jupyterlab_genv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.eslintrc.js
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.stylelintrc
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/TODO.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/Test.ipynb
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/install.json
+-rw-r--r--   0        0        0   328793 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/package-lock.json
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0   258893 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/yarn.lock
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyter-config/nb-config/jupyterlab_genv.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyter-config/server-config/jupyterlab_genv.json
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/__init__.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/__main__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/_version.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv_provisioner.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/handlers.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/control.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/devices.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/envs.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/installation.py
+-rw-r--r--   0        0        0    20565 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/build_log.json
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/package.json
+-rw-r--r--   0        0        0    18782 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js
+-rw-r--r--   0        0        0    16241 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js.map
+-rw-r--r--   0        0        0    28617 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js
+-rw-r--r--   0        0        0    27387 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js.map
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style.js
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js.map
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js
+-rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js.map
+-rw-r--r--   0        0        0   844987 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/resources/readme/activate.gif
+-rw-r--r--   0        0        0  1589295 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/resources/readme/attach.gif
+-rw-r--r--   0        0        0    40559 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/resources/readme/commands.gif
+-rw-r--r--   0        0        0  1278811 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/resources/readme/overview.gif
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/src/dialogs.tsx
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/src/handler.ts
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/src/index.tsx
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/style/index.js
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/README.md
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/PKG-INFO
```

### Comparing `jupyterlab_genv-0.1.2/.eslintrc.js` & `jupyterlab_genv-0.2.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/CHANGELOG.md` & `jupyterlab_genv-0.2.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.2.0] - 2023-04-30
+
+### Changed
+
+- Using updated command `genv-devices find`.
+
 ## [0.1.2] - 2022-12-11
 
 ### Changed
 
 - Initializing spawned terminals using `eval "$(genv init -)"`.
 
 ## [0.1.1] - 2022-09-24
```

### Comparing `jupyterlab_genv-0.1.2/Test.ipynb` & `jupyterlab_genv-0.2.0/Test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/package-lock.json` & `jupyterlab_genv-0.2.0/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999442246835443%*

 * *Differences: {"'dependencies'": "{'http-cache-semantics': {'version': '4.1.1', 'resolved': "*

 * *                   "'https://registry.npmjs.org/http-cache-semantics/-/http-cache-semantics-4.1.1.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-er295DKPVsV82j5kw1Gjt+ADA/XYHsajl82cGNQG2eyoPkvgUhX+nDIyelzhIWbbsXP39EHcI6l5tYs2FYqYXQ=='}, "*

 * *                   "'json5': {'version': '2.2.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/json5/-/json5-2.2.3.tgz', 'integrity': "*

 * *                 […]*

```diff
@@ -3875,17 +3875,17 @@
                 "entities": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/htmlparser2/-/htmlparser2-6.1.0.tgz",
             "version": "6.1.0"
         },
         "http-cache-semantics": {
             "dev": true,
-            "integrity": "sha512-carPklcUh7ROWRK7Cv27RPtdhYhUsela/ue5/jKzjegVvXDqM2ILE9Q2BGn9JZJh1g87cp56su/FgQSzcWS8cQ==",
-            "resolved": "https://registry.npmjs.org/http-cache-semantics/-/http-cache-semantics-4.1.0.tgz",
-            "version": "4.1.0"
+            "integrity": "sha512-er295DKPVsV82j5kw1Gjt+ADA/XYHsajl82cGNQG2eyoPkvgUhX+nDIyelzhIWbbsXP39EHcI6l5tYs2FYqYXQ==",
+            "resolved": "https://registry.npmjs.org/http-cache-semantics/-/http-cache-semantics-4.1.1.tgz",
+            "version": "4.1.1"
         },
         "http-errors": {
             "dev": true,
             "integrity": "sha512-FtwrG/euBzaEjYeRqOgly7G0qviiXoJWnvEH2Z1plBdXgbyjv34pHTSb9zoeHMyDy33+DWy5Wt9Wo+TURtOYSQ==",
             "requires": {
                 "depd": "2.0.0",
                 "inherits": "2.0.4",
@@ -4470,17 +4470,17 @@
         "json-stringify-safe": {
             "dev": true,
             "integrity": "sha512-ZClg6AaYvamvYEE82d3Iyd3vSSIjQ+odgjaTzRuO3s7toCdFKczob2i0zCh7JE8kWn17yvAWhUVxvqGwUalsRA==",
             "resolved": "https://registry.npmjs.org/json-stringify-safe/-/json-stringify-safe-5.0.1.tgz",
             "version": "5.0.1"
         },
         "json5": {
-            "integrity": "sha512-1hqLFMSrGHRHxav9q9gNjJ5EXznIxGVO09xQRrwplcS8qs28pZ8s8hupZAmqDwZUmVZ2Qb2jnyPOWcDH8m8dlA==",
-            "resolved": "https://registry.npmjs.org/json5/-/json5-2.2.1.tgz",
-            "version": "2.2.1"
+            "integrity": "sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==",
+            "resolved": "https://registry.npmjs.org/json5/-/json5-2.2.3.tgz",
+            "version": "2.2.3"
         },
         "jsonfile": {
             "dev": true,
             "integrity": "sha512-5dgndWOriYSm5cnYaJNhalLNDKOqFwyDB/rr1E9ZsGciGvKPs8R2xYGCacuf3z6K1YKDz182fd+fY3cn3pMqXQ==",
             "requires": {
                 "graceful-fs": "^4.1.6",
                 "universalify": "^2.0.0"
@@ -7186,20 +7186,20 @@
             "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz",
             "version": "5.0.1"
         },
         "to-string-loader": {
             "dependencies": {
                 "json5": {
                     "dev": true,
-                    "integrity": "sha512-aKS4WQjPenRxiQsC93MNfjx+nbF4PAdYzmd/1JIj8HYzqfbu86beTuNgXDzPknWk0n0uARlyewZo4s++ES36Ow==",
+                    "integrity": "sha512-g1MWMLBiz8FKi1e4w0UyVL3w+iJceWAFBAaBnnGKOpNa5f8TLktkbre1+s6oICydWAm+HRUGTmI+//xv2hvXYA==",
                     "requires": {
                         "minimist": "^1.2.0"
                     },
-                    "resolved": "https://registry.npmjs.org/json5/-/json5-1.0.1.tgz",
-                    "version": "1.0.1"
+                    "resolved": "https://registry.npmjs.org/json5/-/json5-1.0.2.tgz",
+                    "version": "1.0.2"
                 },
                 "loader-utils": {
                     "dev": true,
                     "integrity": "sha512-I5d00Pd/jwMD2QCduo657+YM/6L3KZu++pmX9VFncxaxvHcru9jx1lBaFft+r4Mt2jK0Yhp41XlRAihzPxHNCg==",
                     "requires": {
                         "big.js": "^5.2.2",
                         "emojis-list": "^3.0.0",
@@ -8077,9 +8077,9 @@
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "lockfileVersion": 1,
     "name": "jupyterlab_genv",
     "requires": true,
-    "version": "0.1.2"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_genv-0.1.2/package.json` & `jupyterlab_genv-0.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_genv-0.1.2/tsconfig.json` & `jupyterlab_genv-0.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/yarn.lock` & `jupyterlab_genv-0.2.0/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3186,17 +3186,17 @@
   dependencies:
     domelementtype "^2.0.1"
     domhandler "^4.0.0"
     domutils "^2.5.2"
     entities "^2.0.0"
 
 http-cache-semantics@^4.0.0:
-  version "4.1.0"
-  resolved "https://registry.npmjs.org/http-cache-semantics/-/http-cache-semantics-4.1.0.tgz"
-  integrity sha512-carPklcUh7ROWRK7Cv27RPtdhYhUsela/ue5/jKzjegVvXDqM2ILE9Q2BGn9JZJh1g87cp56su/FgQSzcWS8cQ==
+  version "4.1.1"
+  resolved "https://registry.yarnpkg.com/http-cache-semantics/-/http-cache-semantics-4.1.1.tgz#abe02fcb2985460bf0323be664436ec3476a6d5a"
+  integrity sha512-er295DKPVsV82j5kw1Gjt+ADA/XYHsajl82cGNQG2eyoPkvgUhX+nDIyelzhIWbbsXP39EHcI6l5tYs2FYqYXQ==
 
 http-errors@2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/http-errors/-/http-errors-2.0.0.tgz"
   integrity sha512-FtwrG/euBzaEjYeRqOgly7G0qviiXoJWnvEH2Z1plBdXgbyjv34pHTSb9zoeHMyDy33+DWy5Wt9Wo+TURtOYSQ==
   dependencies:
     depd "2.0.0"
@@ -3663,17 +3663,17 @@
 
 json-stringify-safe@~5.0.1:
   version "5.0.1"
   resolved "https://registry.npmjs.org/json-stringify-safe/-/json-stringify-safe-5.0.1.tgz"
   integrity sha512-ZClg6AaYvamvYEE82d3Iyd3vSSIjQ+odgjaTzRuO3s7toCdFKczob2i0zCh7JE8kWn17yvAWhUVxvqGwUalsRA==
 
 json5@^1.0.1:
-  version "1.0.1"
-  resolved "https://registry.yarnpkg.com/json5/-/json5-1.0.1.tgz#779fb0018604fa854eacbf6252180d83543e3dbe"
-  integrity sha512-aKS4WQjPenRxiQsC93MNfjx+nbF4PAdYzmd/1JIj8HYzqfbu86beTuNgXDzPknWk0n0uARlyewZo4s++ES36Ow==
+  version "1.0.2"
+  resolved "https://registry.yarnpkg.com/json5/-/json5-1.0.2.tgz#63d98d60f21b313b77c4d6da18bfa69d80e1d593"
+  integrity sha512-g1MWMLBiz8FKi1e4w0UyVL3w+iJceWAFBAaBnnGKOpNa5f8TLktkbre1+s6oICydWAm+HRUGTmI+//xv2hvXYA==
   dependencies:
     minimist "^1.2.0"
 
 json5@^2.1.1, json5@^2.1.2:
   version "2.2.1"
   resolved "https://registry.npmjs.org/json5/-/json5-2.2.1.tgz"
   integrity sha512-1hqLFMSrGHRHxav9q9gNjJ5EXznIxGVO09xQRrwplcS8qs28pZ8s8hupZAmqDwZUmVZ2Qb2jnyPOWcDH8m8dlA==
@@ -4232,24 +4232,19 @@
   resolved "https://registry.npmjs.org/minimist-options/-/minimist-options-4.1.0.tgz"
   integrity sha512-Q4r8ghd80yhO/0j1O3B2BjweX3fiHg9cdOwjJd2J76Q135c+NDxGCqdYKQ1SKBuFfgWbAUzBfvYjPUEeNgqN1A==
   dependencies:
     arrify "^1.0.1"
     is-plain-obj "^1.1.0"
     kind-of "^6.0.3"
 
-minimist@^1.2.0:
+minimist@^1.2.0, minimist@^1.2.5, minimist@^1.2.6, minimist@~1.2.0:
   version "1.2.7"
   resolved "https://registry.yarnpkg.com/minimist/-/minimist-1.2.7.tgz#daa1c4d91f507390437c6a8bc01078e7000c4d18"
   integrity sha512-bzfL1YUZsP41gmu/qjrEk0Q6i2ix/cVeAhbCbqH9u3zYutS1cLg00qhrD0M2MVdCcx4Sc0UpP2eBWo9rotpq6g==
 
-minimist@^1.2.5, minimist@^1.2.6, minimist@~1.2.0:
-  version "1.2.6"
-  resolved "https://registry.npmjs.org/minimist/-/minimist-1.2.6.tgz"
-  integrity sha512-Jsjnk4bw3YJqYzbdyBiNsPWHPfO++UGG749Cxs6peCu5Xg4nrena6OVxOYxrQTqww0Jmwt+Ref8rggumkTLz9Q==
-
 minipass-collect@^1.0.2:
   version "1.0.2"
   resolved "https://registry.npmjs.org/minipass-collect/-/minipass-collect-1.0.2.tgz"
   integrity sha512-6T6lH0H8OG9kITm/Jm6tdooIbogG9e0tLgpY6mphXSm/A9u8Nq1ryBG+Qspiub9LjWlBPsPS3tWQ/Botq4FdxA==
   dependencies:
     minipass "^3.0.0"
```

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/__init__.py` & `jupyterlab_genv-0.2.0/jupyterlab_genv/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/__main__.py` & `jupyterlab_genv-0.2.0/jupyterlab_genv/__main__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/genv_provisioner.py` & `jupyterlab_genv-0.2.0/jupyterlab_genv/genv_provisioner.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Dict
 
 from . import genv
 
 class GenvProvisioner(jupyter_client.LocalProvisioner):
     async def pre_launch(self, **kwargs: Any) -> Dict[str, Any]:
         eid = await genv.envs.find(self.kernel_id) or self.kernel_id
-        indices = await genv.devices.query(eid)
+        indices = await genv.devices.find(eid)
 
         env = kwargs.pop('env', os.environ).copy()
         env.update({ 'CUDA_VISIBLE_DEVICES': ','.join(str(index) for index in indices) })
+        # TODO(raz): add 'shims' to PATH so that nvidia-smi shim would run
         kwargs['env'] = env
 
         return await super().pre_launch(**kwargs)
```

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/handlers.py` & `jupyterlab_genv-0.2.0/jupyterlab_genv/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/genv/devices.py` & `jupyterlab_genv-0.2.0/jupyterlab_genv/genv/envs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+import os
 from typing import Dict, List
 
 from . import control
 
 async def _exec(command: str) -> str:
-    return await control.exec(f'exec devices {command}')
+    return await control.exec(f'exec envs {command}')
 
-async def ps() -> Dict:
+async def activate(eid: str, kernel_id: str) -> None:
+    await _exec(f'activate --eid {eid} --uid {os.getuid()} --kernel-id {kernel_id}')
+
+async def find(kernel_id: str) -> str:
+    return await _exec(f'find --kernel-id {kernel_id}')
+
+async def ps() -> List[Dict]:
     stdout = await _exec("ps --format csv --no-header --timestamp")
     lines = [line for line in stdout.splitlines() if len(line)]
 
     infos = []
 
     for line in lines:
-        id, eid, env, attached = line.split(',')
-        id = int(id)
+        eid, user, name, created, pids = line.split(',')
 
         infos.append({
             "eid": eid,
-            "env": env,
+            "user": user,
+            "name": name,
+            "pids": [int(pid) for pid in pids.split(' ') if len(pid)],
         })
 
     return infos
-
-async def query(eid: str) -> List[int]:
-    return [int(index) for index in (await _exec(f'query --eid {eid}')).split(',') if len(index) > 0]
```

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/build_log.json` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/build_log.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827825914599614%*

 * *Differences: {'0': "{'resolve': {'alias': {'@phosphor/algorithm$': "*

 * *      "'/home/raz/work/jupyterlab_genv/node_modules/@lumino/algorithm/dist/index.js', "*

 * *      "'@phosphor/application$': "*

 * *      "'/home/raz/work/jupyterlab_genv/node_modules/@lumino/application/dist/index.js', "*

 * *      "'@phosphor/commands$': "*

 * *      "'/home/raz/work/jupyterlab_genv/node_modules/@lumino/commands/dist/index.js', "*

 * *      "'@phosphor/coreutils$': "*

 * *      "'/home/raz/work/jupyterlab_genv/node_modules/@lumino/coreutils/dist/index.node.js',  […]*

```diff
@@ -84,446 +84,446 @@
                     "use": "file-loader"
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/Users/raz/Work/jupyterlab_genv/jupyterlab_genv/labextension/static",
+            "path": "/home/raz/work/jupyterlab_genv/jupyterlab_genv/labextension/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/Users/raz/Work/jupyterlab_genv/lib/index.js",
-                        "./index": "/Users/raz/Work/jupyterlab_genv/lib/index.js",
-                        "./style": "/Users/raz/Work/jupyterlab_genv/style/index.js"
+                        "./extension": "/home/raz/work/jupyterlab_genv/lib/index.js",
+                        "./index": "/home/raz/work/jupyterlab_genv/lib/index.js",
+                        "./style": "/home/raz/work/jupyterlab_genv/style/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
                             "jupyterlab_genv"
                         ],
                         "type": "var"
                     },
                     "name": "jupyterlab_genv",
                     "shared": {
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.5.1",
+                            "requiredVersion": "^5.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/docprovider": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/docprovider-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.5.1"
+                            "requiredVersion": "^4.5.2"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.5.1",
+                            "requiredVersion": "^6.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/shared-models": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.5.1",
+                            "requiredVersion": "^5.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.5.1"
+                            "requiredVersion": "^5.5.2"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.5.1",
+                            "requiredVersion": "^3.5.2",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.1"
+                            "requiredVersion": "^3.5.2"
                         },
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
@@ -578,17 +578,17 @@
                         },
                         "@lumino/widgets": {
                             "import": false,
                             "requiredVersion": "^1.33.0",
                             "singleton": true
                         },
                         "jupyterlab_genv": {
-                            "import": "/Users/raz/Work/jupyterlab_genv/lib/index.js",
+                            "import": "/home/raz/work/jupyterlab_genv/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.1"
+                            "version": "0.1.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
@@ -604,34 +604,34 @@
                     }
                 }
             },
             {}
         ],
         "resolve": {
             "alias": {
-                "@phosphor/algorithm$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/algorithm/dist/index.js",
-                "@phosphor/application$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/application/dist/index.js",
-                "@phosphor/commands$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/commands/dist/index.js",
-                "@phosphor/coreutils$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/coreutils/dist/index.node.js",
-                "@phosphor/disposable$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/disposable/dist/index.js",
-                "@phosphor/domutils$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/domutils/dist/index.js",
-                "@phosphor/dragdrop$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/dragdrop/dist/index.js",
-                "@phosphor/dragdrop/style": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/widgets/style",
-                "@phosphor/messaging$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/messaging/dist/index.js",
-                "@phosphor/properties$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/properties/dist/index.js",
-                "@phosphor/signaling": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/signaling/dist/index.js",
-                "@phosphor/virtualdom$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/virtualdom/dist/index.js",
-                "@phosphor/widgets$": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/widgets/dist/index.js",
-                "@phosphor/widgets/style": "/Users/raz/Work/jupyterlab_genv/node_modules/@lumino/widgets/style"
+                "@phosphor/algorithm$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/algorithm/dist/index.js",
+                "@phosphor/application$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/application/dist/index.js",
+                "@phosphor/commands$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/commands/dist/index.js",
+                "@phosphor/coreutils$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/coreutils/dist/index.node.js",
+                "@phosphor/disposable$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/disposable/dist/index.js",
+                "@phosphor/domutils$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/domutils/dist/index.js",
+                "@phosphor/dragdrop$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/dragdrop/dist/index.js",
+                "@phosphor/dragdrop/style": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/widgets/style",
+                "@phosphor/messaging$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/messaging/dist/index.js",
+                "@phosphor/properties$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/properties/dist/index.js",
+                "@phosphor/signaling": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/signaling/dist/index.js",
+                "@phosphor/virtualdom$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/virtualdom/dist/index.js",
+                "@phosphor/widgets$": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/widgets/dist/index.js",
+                "@phosphor/widgets/style": "/home/raz/work/jupyterlab_genv/node_modules/@lumino/widgets/style"
             },
             "fallback": {
                 "buffer": false,
                 "crypto": false,
-                "path": "/Users/raz/Work/jupyterlab_genv/node_modules/path-browserify/index.js",
-                "process": "/Users/raz/Work/jupyterlab_genv/node_modules/process/browser.js",
+                "path": "/home/raz/work/jupyterlab_genv/node_modules/path-browserify/index.js",
+                "process": "/home/raz/work/jupyterlab_genv/node_modules/process/browser.js",
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
```

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/package.json` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.620874b13a1cfcb8a98e.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -50,15 +50,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3f30df1d6370ec409a58.js",
+            "load": "static/remoteEntry.620874b13a1cfcb8a98e.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_genv"
                 },
@@ -113,9 +113,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js.map` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/remoteEntry.3f30df1d6370ec409a58.js` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -425,15 +425,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab_genv", "0.1.1", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab_genv", "0.1.2", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -814,23 +814,23 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 5, 1])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 5, 2])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 5, 1])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 5, 2])),
             /******/
             "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 33, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 5, 1])),
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 5, 2])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 6, 5, 1])),
+            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 6, 5, 2])),
             /******/
             "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 17, 0, 1]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
@@ -1078,8 +1078,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab_genv");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyterlab_genv = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.3f30df1d6370ec409a58.js.map
+//# sourceMappingURL=remoteEntry.620874b13a1cfcb8a98e.js.map
```

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/remoteEntry.3f30df1d6370ec409a58.js.map` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'remoteEntry.620874b13a1cfcb8a98e.js'",*

 * * "'sourcesContent'": "{insert: [(10, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.3f30df1d6370ec409a58.js",
+    "file": "remoteEntry.620874b13a1cfcb8a98e.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCjLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_genv/webpack/container-entry",
         "webpack://jupyterlab_genv/webpack/bootstrap",
         "webpack://jupyterlab_genv/webpack/runtime/compat get default export",
@@ -30,17 +30,17 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"ff60ebd71c9a48ac429f\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"f136769aaa598352c213\",\"style_index_js\":\"584bbd372a8c350b76d6\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_genv:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab_genv\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_genv\", \"0.1.1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab_genv\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_genv\", \"0.1.2\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,5,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,5,1])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,33,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,5,1])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,5,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,5,2])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,33,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,5,2])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab_genv\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_genv\"] = self[\"webpackChunkjupyterlab_genv\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab_genv\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js.map` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js.map` & `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/resources/readme/activate.gif` & `jupyterlab_genv-0.2.0/resources/readme/activate.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/resources/readme/attach.gif` & `jupyterlab_genv-0.2.0/resources/readme/attach.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/resources/readme/commands.gif` & `jupyterlab_genv-0.2.0/resources/readme/commands.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/resources/readme/overview.gif` & `jupyterlab_genv-0.2.0/resources/readme/overview.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/src/dialogs.tsx` & `jupyterlab_genv-0.2.0/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/src/handler.ts` & `jupyterlab_genv-0.2.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/src/index.tsx` & `jupyterlab_genv-0.2.0/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/.gitignore` & `jupyterlab_genv-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/LICENSE` & `jupyterlab_genv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.1.2/README.md` & `jupyterlab_genv-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,36 +20,47 @@
 
 Looking forward to seeing you as a part of the community!
 
 ## Table of Contents
 
 - [Getting Started](#getting-started)
 - [Installation](#installation)
+  - [Conda](#conda)
   - [Pip](#pip)
   - [Install _genv_ Kernels](#install-genv-kernels)
 - [Usage](#usage)
   - [Activate Your Environment](#activate-your-environment)
   - [Attach GPUs to Your Environment](#attach-gpus-to-your-environment)
   - [See Devices and Environments](#see-devices-and-environments)
 - [Development](#development)
 - [Publish](#publish)
+  - [PyPI](#pypi)
+  - [Conda](#conda-1)
 
 ## Getting Started
 
 Read the _genv_ [reference](https://github.com/run-ai/genv#usage) to get started.
 
 ## Installation
 
 ### Requirements
 
 JupyterLab >= 3.0
 
+### Conda
+
+If you are using [Conda](https://docs.conda.io/en/latest/), it is best to install the `jupyterlab_genv` [package](https://anaconda.org/conda-forge/jupyterlab_genv) from the channel [conda-forge](https://conda-forge.org/):
+
+```bash
+conda install -c conda-forge jupyterlab_genv
+```
+
 ### Pip
 
-You can install `jupyterlab_genv` from [PyPI](https://pypi.org/project/jupyterlab-genv/) using `pip`:
+Alternatively, you can install `jupyterlab_genv` from [PyPI](https://pypi.org/project/jupyterlab-genv/) using `pip`:
 
 ```bash
 pip install jupyterlab_genv
 ```
 
 ### Install _genv_ Kernels
 
@@ -203,41 +214,43 @@
 
 ```bash
 jupyter labextension list
 ```
 
 ## Publish
 
-The Python package is manually published to both [PyPI](https://pypi.org/project/jupyterlab-genv/) and [conda-forge](https://conda-forge.org/).
+The `jupyterlab_genv` package is manually published to both [PyPI](https://pypi.org/project/jupyterlab-genv/) and [conda-forge](https://anaconda.org/conda-forge/jupyterlab_genv).
 
 We do not publish the frontend part as an npm package because the Python package is a prebuilt server extension, and the frontend part alone is useless.
 
-Also make sure to update the [changelog](./CHANGELOG.md) ([here's](https://keepachangelog.com/en/1.0.0/#how) how).
-
-### PyPI
-
-#### Prerequisites
+Also make sure to update the [changelog](./CHANGELOG.md) ([here's](https://keepachangelog.com/en/1.0.0/#how) how) and lint the project by running `npm run lint`.
 
-```bash
-pip install build twine tbump
-```
-
-#### Bump Version
+### Bump Version
 
 The [cookiecutter template](https://github.com/jupyterlab/extension-cookiecutter-ts) uses `tbump` for bumping the version.
 However, for some reason this does not work at the moment, and we bump the version manually.
 
 Search for the current version in the project files and replace the relevant instances.
 Here is a list of files that you should update:
 
 - [package.json](package.json#L3)
 - [package-lock.json](package-lock.json#L3)
 - [pyproject.toml](pyproject.toml#L7) (also [here](pyproject.toml#L84) for future `tbump` support)
 - [jupyterlab_genv/\_version.py](jupyterlab_genv/_version.py#L6)
 
+After pushing these changes, create a release on [GitHub](https://github.com/run-ai/jupyterlab_genv/releases).
+
+### PyPI
+
+#### Prerequisites
+
+```bash
+pip install build twine tbump
+```
+
 #### Create a Python Package
 
 Create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory using:
 
 ```bash
 python -m build
 ```
@@ -245,7 +258,19 @@
 > `python setup.py sdist bdist_wheel` is deprecated and will not work for this package.
 
 Then, upload the package to [PyPI](https://pypi.org/project/jupyterlab-genv/) using:
 
 ```bash
 twine upload dist/*
 ```
+
+> We upload to PyPI with the organizational user [runai](https://pypi.org/user/runai/)
+
+### Conda
+
+The Conda package is managed using its [feedstock](https://github.com/conda-forge/jupyterlab_genv-feedstock).
+
+After publishing to [PyPI](#pypi), update the [version](https://github.com/conda-forge/jupyterlab_genv-feedstock/blob/main/recipe/meta.yaml#L2) and [sha256](https://github.com/conda-forge/jupyterlab_genv-feedstock/blob/main/recipe/meta.yaml#L10) fields in the recipe `meta.yaml` file.
+
+A few minutes after pushing these changes, you should be able to see that the Conda [package](https://anaconda.org/conda-forge/jupyterlab_genv) version was updated.
+
+> You can get the SHA256 hash from [PyPI](https://pypi.org/project/jupyterlab-genv/#files)
```

### Comparing `jupyterlab_genv-0.1.2/pyproject.toml` & `jupyterlab_genv-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.3.1", "jupyterlab~=3.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab_genv"
-version = "0.1.2"
+version = "0.2.0"
 description = "A JupyterLab extension for managing GPU environments using genv."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Raz Rotenberg", email = "raz.rotenberg@gmail.com" },
 ]
@@ -77,15 +77,15 @@
 file = [
     { src = "pyproject.toml", version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\"" },
     { src = "jupyterlab_genv/_version.py" },
     { src = "package.json" },
 ]
 
 [tool.tbump.version]
-current = "0.1.2"
+current = "0.2.0"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [project.entry-points."jupyter_client.kernel_provisioners"]
```

### Comparing `jupyterlab_genv-0.1.2/PKG-INFO` & `jupyterlab_genv-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_genv
-Version: 0.1.2
+Version: 0.2.0
 Summary: A JupyterLab extension for managing GPU environments using genv.
 Project-URL: Homepage, https://github.com/run-ai/jupyterlab_genv
 Author-email: Raz Rotenberg <raz.rotenberg@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Raz Rotenberg
         All rights reserved.
@@ -74,36 +74,47 @@
 
 Looking forward to seeing you as a part of the community!
 
 ## Table of Contents
 
 - [Getting Started](#getting-started)
 - [Installation](#installation)
+  - [Conda](#conda)
   - [Pip](#pip)
   - [Install _genv_ Kernels](#install-genv-kernels)
 - [Usage](#usage)
   - [Activate Your Environment](#activate-your-environment)
   - [Attach GPUs to Your Environment](#attach-gpus-to-your-environment)
   - [See Devices and Environments](#see-devices-and-environments)
 - [Development](#development)
 - [Publish](#publish)
+  - [PyPI](#pypi)
+  - [Conda](#conda-1)
 
 ## Getting Started
 
 Read the _genv_ [reference](https://github.com/run-ai/genv#usage) to get started.
 
 ## Installation
 
 ### Requirements
 
 JupyterLab >= 3.0
 
+### Conda
+
+If you are using [Conda](https://docs.conda.io/en/latest/), it is best to install the `jupyterlab_genv` [package](https://anaconda.org/conda-forge/jupyterlab_genv) from the channel [conda-forge](https://conda-forge.org/):
+
+```bash
+conda install -c conda-forge jupyterlab_genv
+```
+
 ### Pip
 
-You can install `jupyterlab_genv` from [PyPI](https://pypi.org/project/jupyterlab-genv/) using `pip`:
+Alternatively, you can install `jupyterlab_genv` from [PyPI](https://pypi.org/project/jupyterlab-genv/) using `pip`:
 
 ```bash
 pip install jupyterlab_genv
 ```
 
 ### Install _genv_ Kernels
 
@@ -257,41 +268,43 @@
 
 ```bash
 jupyter labextension list
 ```
 
 ## Publish
 
-The Python package is manually published to both [PyPI](https://pypi.org/project/jupyterlab-genv/) and [conda-forge](https://conda-forge.org/).
+The `jupyterlab_genv` package is manually published to both [PyPI](https://pypi.org/project/jupyterlab-genv/) and [conda-forge](https://anaconda.org/conda-forge/jupyterlab_genv).
 
 We do not publish the frontend part as an npm package because the Python package is a prebuilt server extension, and the frontend part alone is useless.
 
-Also make sure to update the [changelog](./CHANGELOG.md) ([here's](https://keepachangelog.com/en/1.0.0/#how) how).
-
-### PyPI
-
-#### Prerequisites
+Also make sure to update the [changelog](./CHANGELOG.md) ([here's](https://keepachangelog.com/en/1.0.0/#how) how) and lint the project by running `npm run lint`.
 
-```bash
-pip install build twine tbump
-```
-
-#### Bump Version
+### Bump Version
 
 The [cookiecutter template](https://github.com/jupyterlab/extension-cookiecutter-ts) uses `tbump` for bumping the version.
 However, for some reason this does not work at the moment, and we bump the version manually.
 
 Search for the current version in the project files and replace the relevant instances.
 Here is a list of files that you should update:
 
 - [package.json](package.json#L3)
 - [package-lock.json](package-lock.json#L3)
 - [pyproject.toml](pyproject.toml#L7) (also [here](pyproject.toml#L84) for future `tbump` support)
 - [jupyterlab_genv/\_version.py](jupyterlab_genv/_version.py#L6)
 
+After pushing these changes, create a release on [GitHub](https://github.com/run-ai/jupyterlab_genv/releases).
+
+### PyPI
+
+#### Prerequisites
+
+```bash
+pip install build twine tbump
+```
+
 #### Create a Python Package
 
 Create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory using:
 
 ```bash
 python -m build
 ```
@@ -299,7 +312,19 @@
 > `python setup.py sdist bdist_wheel` is deprecated and will not work for this package.
 
 Then, upload the package to [PyPI](https://pypi.org/project/jupyterlab-genv/) using:
 
 ```bash
 twine upload dist/*
 ```
+
+> We upload to PyPI with the organizational user [runai](https://pypi.org/user/runai/)
+
+### Conda
+
+The Conda package is managed using its [feedstock](https://github.com/conda-forge/jupyterlab_genv-feedstock).
+
+After publishing to [PyPI](#pypi), update the [version](https://github.com/conda-forge/jupyterlab_genv-feedstock/blob/main/recipe/meta.yaml#L2) and [sha256](https://github.com/conda-forge/jupyterlab_genv-feedstock/blob/main/recipe/meta.yaml#L10) fields in the recipe `meta.yaml` file.
+
+A few minutes after pushing these changes, you should be able to see that the Conda [package](https://anaconda.org/conda-forge/jupyterlab_genv) version was updated.
+
+> You can get the SHA256 hash from [PyPI](https://pypi.org/project/jupyterlab-genv/#files)
```

