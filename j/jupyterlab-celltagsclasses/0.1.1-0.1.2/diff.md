# Comparing `tmp/jupyterlab_celltagsclasses-0.1.1.tar.gz` & `tmp/jupyterlab_celltagsclasses-0.1.2.tar.gz`

## Comparing `jupyterlab_celltagsclasses-0.1.1.tar` & `jupyterlab_celltagsclasses-0.1.2.tar`

### file list

```diff
@@ -1,65 +1,117 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.editorconfig
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.eslintrc.js
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.gitattributes
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/RELEASE.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/install.json
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/package.json
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/tsconfig.json
--rw-r--r--   0        0        0   208796 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/yarn.lock
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/examples/test.ipynb
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/_version.py
--rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/build_log.json
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/package.json
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js.map
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js.map
--rw-r--r--   0        0        0    27528 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.170c8a935f39cb9518d6.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.666f3bf51bf09fc5bf7f.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.6cbab8277822394dfb29.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.933bc9f561b8ebc92287.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b24f4403982fe69ad690.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b3482340b7d50da9319c.js.map
--rw-r--r--   0        0        0    26446 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c33d2bfa2fdbc5139570.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.db28ad9a76e4c9f2ecb5.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.fb379948d6ce49efaa3b.js.map
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style.js
--rw-r--r--   0        0        0    20292 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js
--rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js.map
--rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js.map
--rw-r--r--   0        0        0    14877 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js
--rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js.map
--rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js
--rw-r--r--   0        0        0    16224 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js.map
--rw-r--r--   0        0        0    20418 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js
--rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js.map
--rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js
--rw-r--r--   0        0        0    16042 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js.map
--rw-r--r--   0        0        0    20440 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js
--rw-r--r--   0        0        0    16176 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js.map
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js
--rw-r--r--   0        0        0    16288 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js.map
--rw-r--r--   0        0        0    20474 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js
--rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js.map
--rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/media/screenshot.png
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/src/index.ts
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/style/index.js
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/LICENSE
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/README.md
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.editorconfig
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.eslintignore
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.eslintrc.js
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.gitattributes
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.prettierignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/install.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/package.json
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/release.sh
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0   208796 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/yarn.lock
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/examples/test.ipynb
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/_version.py
+-rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/build_log.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/install.json
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/package.json
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js.map
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js.map
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js.map
+-rw-r--r--   0        0        0    27528 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.0a4c39b501971c60ffd2.js.map
+-rw-r--r--   0        0        0    27528 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.121544801bc433e00240.js
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.121544801bc433e00240.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.170c8a935f39cb9518d6.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.17f7467f156319c755c0.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.1849839b62edee24aec8.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.22ac66fc46652f220c02.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.4fc7106cb22143a5fce6.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.586ed0a7209176557f21.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.666f3bf51bf09fc5bf7f.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.6cbab8277822394dfb29.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.933bc9f561b8ebc92287.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.9728aad82475f1fe62ea.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.a58905825d751323be61.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b24f4403982fe69ad690.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b3482340b7d50da9319c.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.bdfe1655a685cae2eb10.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c07b230f1f57c9e89481.js.map
+-rw-r--r--   0        0        0    26446 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c33d2bfa2fdbc5139570.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c848fd19f30b6f3af7d6.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.d1d5567cd1ed4013c60b.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.d347944507729fb1c1d2.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.db28ad9a76e4c9f2ecb5.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.dc9b6438cba1062a18bd.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e631040c6c782fc048c3.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e6d891cc83354cb06c15.js.map
+-rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.fb379948d6ce49efaa3b.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style.js
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.012e4d3162293b291168.js
+-rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.012e4d3162293b291168.js.map
+-rw-r--r--   0        0        0    20499 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.0e23ae348872f42dfa7e.js
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.0e23ae348872f42dfa7e.js.map
+-rw-r--r--   0        0        0    20292 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js
+-rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js.map
+-rw-r--r--   0        0        0    20495 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.2d159db83d8284e0cf12.js
+-rw-r--r--   0        0        0    16239 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.2d159db83d8284e0cf12.js.map
+-rw-r--r--   0        0        0    20485 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.33fc960cbf5aa7e756d6.js
+-rw-r--r--   0        0        0    16233 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.33fc960cbf5aa7e756d6.js.map
+-rw-r--r--   0        0        0    20542 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.447299cd6bd7a4db7267.js
+-rw-r--r--   0        0        0    16284 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.447299cd6bd7a4db7267.js.map
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
+-rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
+-rw-r--r--   0        0        0    20485 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.50300ed39417ed24f985.js
+-rw-r--r--   0        0        0    16229 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.50300ed39417ed24f985.js.map
+-rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js.map
+-rw-r--r--   0        0        0    14877 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js.map
+-rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js
+-rw-r--r--   0        0        0    16224 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js.map
+-rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.8484ad0db61e328da5f5.js
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.8484ad0db61e328da5f5.js.map
+-rw-r--r--   0        0        0    20484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.951d4f88d7f9cc18fa51.js
+-rw-r--r--   0        0        0    16227 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.951d4f88d7f9cc18fa51.js.map
+-rw-r--r--   0        0        0    20418 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js
+-rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js.map
+-rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js
+-rw-r--r--   0        0        0    16042 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js.map
+-rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.b48473261159e6e27fea.js
+-rw-r--r--   0        0        0    16281 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.b48473261159e6e27fea.js.map
+-rw-r--r--   0        0        0    20378 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c13f242cce861218e3cf.js
+-rw-r--r--   0        0        0    16115 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c13f242cce861218e3cf.js.map
+-rw-r--r--   0        0        0    20440 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js
+-rw-r--r--   0        0        0    16176 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js.map
+-rw-r--r--   0        0        0    20491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c804bc222706d3cf7bec.js
+-rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c804bc222706d3cf7bec.js.map
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.d3e9571212d458ccc458.js
+-rw-r--r--   0        0        0    16240 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.d3e9571212d458ccc458.js.map
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js
+-rw-r--r--   0        0        0    16288 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js.map
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.df6561a0531b63f9a29b.js
+-rw-r--r--   0        0        0    16238 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.df6561a0531b63f9a29b.js.map
+-rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.ee239d110f5f639974dc.js
+-rw-r--r--   0        0        0    16232 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.ee239d110f5f639974dc.js.map
+-rw-r--r--   0        0        0    20474 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js
+-rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js.map
+-rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/media/screenshot.png
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/src/index.ts
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/style/index.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/style/index.js
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/README.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/PKG-INFO
```

### Comparing `jupyterlab_celltagsclasses-0.1.1/.eslintrc.js` & `jupyterlab_celltagsclasses-0.1.2/.eslintrc.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -35,8 +35,8 @@
                 allowTemplateLiterals: false
             }
         ],
         curly: ['error', 'all'],
         eqeqeq: 'error',
         'prefer-arrow-callback': 'error'
     }
-};
+}
```

### Comparing `jupyterlab_celltagsclasses-0.1.1/RELEASE.md` & `jupyterlab_celltagsclasses-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/package.json` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.09eb75b8b35017dd61cc.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.1.0'"}*

```diff
@@ -39,14 +39,19 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/parmentelat/jupyterlab-celltagsclasses",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.09eb75b8b35017dd61cc.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "jupyterlab_celltagsclasses/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -90,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.0"
 }
```

### Comparing `jupyterlab_celltagsclasses-0.1.1/tsconfig.json` & `jupyterlab_celltagsclasses-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/yarn.lock` & `jupyterlab_celltagsclasses-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/examples/test.ipynb` & `jupyterlab_celltagsclasses-0.1.2/examples/test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/build_log.json` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/package.json` & `jupyterlab_celltagsclasses-0.1.2/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.1.2'"}*

```diff
@@ -39,19 +39,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/parmentelat/jupyterlab-celltagsclasses",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.09eb75b8b35017dd61cc.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "jupyterlab_celltagsclasses/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -95,9 +90,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.170c8a935f39cb9518d6.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.170c8a935f39cb9518d6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.666f3bf51bf09fc5bf7f.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.666f3bf51bf09fc5bf7f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.6cbab8277822394dfb29.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.6cbab8277822394dfb29.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.933bc9f561b8ebc92287.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.933bc9f561b8ebc92287.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b24f4403982fe69ad690.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b24f4403982fe69ad690.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b3482340b7d50da9319c.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b3482340b7d50da9319c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c33d2bfa2fdbc5139570.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c33d2bfa2fdbc5139570.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.db28ad9a76e4c9f2ecb5.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.db28ad9a76e4c9f2ecb5.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.fb379948d6ce49efaa3b.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.fb379948d6ce49efaa3b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js.map` & `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/media/screenshot.png` & `jupyterlab_celltagsclasses-0.1.2/media/screenshot.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/src/index.ts` & `jupyterlab_celltagsclasses-0.1.2/src/index.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,119 +1,115 @@
 /*
  * for attaching keybindings later on, see
  * https://towardsdatascience.com/how-to-customize-jupyterlab-keyboard-shortcuts-72321f73753d
  */
 
 /* eslint-disable prettier/prettier */
 
-import {
-  JupyterFrontEnd,
-  JupyterFrontEndPlugin,
-} from '@jupyterlab/application'
-
-import {
-  INotebookTracker,
-} from '@jupyterlab/notebook'
-
-import {
-  ICellModel,
-  Cell,
-} from '@jupyterlab/cells'
+import { JupyterFrontEnd, JupyterFrontEndPlugin } from '@jupyterlab/application'
 
+import { INotebookTracker } from '@jupyterlab/notebook'
 
+import { ICellModel, Cell } from '@jupyterlab/cells'
 
 /**
  * Initialization data for the jupyterlab-celltagsclasses extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: 'jupyterlab-celltagsclasses:plugin',
   autoStart: true,
   requires: [INotebookTracker],
   activate: (app: JupyterFrontEnd, notebookTracker: INotebookTracker) => {
     console.log('extension jupyterlab-celltagsclasses is activating')
 
     const class_for_tag = (tag: string) => `cell-tag-${tag}`
 
     notebookTracker.widgetAdded.connect((_, panel) => {
-        const notebookModel = panel.content.model
-        if (notebookModel === null) {
+      const notebookModel = panel.content.model
+      if (notebookModel === null) {
+        return
+      }
+
+      notebookModel.cells.changed.connect((cellList, change) => {
+        if (change.type !== 'add') {
           return
         }
-
-        notebookModel.cells.changed.connect((cellList, change) => {
-          if (change.type !== 'add') {
+        change.newValues.forEach(cellModel => {
+          // compute widgets attached to cellModel
+          const cellWidgets =
+            notebookTracker.currentWidget?.content.widgets.filter(
+              (cell: Cell, index: number) => cell.model.id === cellModel.id
+            )
+          if (cellWidgets === undefined || cellWidgets?.length === 0) {
+            console.warn('could not find cell widget for cell model', cellModel)
             return
           }
-          change.newValues.forEach((cellModel) => {
+          console.debug(
+            `found ${cellWidgets?.length} cell widgets`,
+            cellWidgets[0]
+          )
+
+          // add classes for pre-existing tags
+          cellModel.getMetadata('tags')?.forEach((tag: string) =>
+            cellWidgets?.forEach(cellWidget => {
+              console.debug(
+                `adding initial class for tag ${class_for_tag(tag)}`
+              )
+              cellWidget.addClass(class_for_tag(tag))
+            })
+          )
 
-            // compute widgets attached to cellModel
-            const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(
-              (cell: Cell, index: number) => (cell.model.id === cellModel.id)
-            )
-            if ((cellWidgets === undefined) || (cellWidgets?.length === 0)) {
-              console.warn('could not find cell widget for cell model', cellModel)
+          // react to changes in tags
+          cellModel.metadataChanged.connect((sender: ICellModel, change) => {
+            console.debug('metadata changed', sender, change)
+            if (change.key !== 'tags') {
+              // console.debug("ignoring non-tags metadata change")
               return
             }
-            console.debug(`found ${cellWidgets?.length} cell widgets`, cellWidgets[0])
-
-            // add classes for pre-existing tags
-            cellModel.getMetadata('tags')?.forEach(
-              (tag: string) => cellWidgets?.forEach(cellWidget => {
-                console.debug(`adding initial class for tag ${class_for_tag(tag)}`)
-                cellWidget.addClass(class_for_tag(tag))
-              }))
-
-            // react to changes in tags
-            cellModel.metadataChanged.connect((sender: ICellModel, change) => {
-              console.debug('metadata changed', sender, change)
-              if (change.key !== 'tags') {
-                // console.debug("ignoring non-tags metadata change")
-                return
-              }
-              // does not seem useful to recompute this
-              // const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(
-              //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)
-              // )
-              if (change.type === 'change') {
-                console.debug('change', change, change.newValue)
-                // compute difference between old and new tags
-                const oldTags = change.oldValue as string[]
-                const newTags = change.newValue as string[]
-                const addedTags = newTags.filter((tag) => !oldTags.includes(tag))
-                const removedTags = oldTags.filter((tag) => !newTags.includes(tag))
-                console.log('addedTags', addedTags)
-                console.log('removedTags', removedTags)
-                cellWidgets.forEach(cellWidget => {
-                  addedTags.forEach(tag => {
-                    console.debug(`adding class for tag ${class_for_tag(tag)}`)
-                    cellWidget.addClass(class_for_tag(tag))
-                  })
-                  removedTags.forEach(tag => {
-                    console.debug(`removing class for tag ${class_for_tag(tag)}`)
-                    cellWidget.removeClass(class_for_tag(tag))
-                  })
-                })
-              } else if (change.type === 'add') {
-                console.log('add', change, change.newValue)
-                cellWidgets.forEach((cellWidget) => {
-                  for (const tag of change.newValue) {
-                    console.debug(`adding class for tag ${class_for_tag(tag)}`)
-                    cellWidget.addClass(class_for_tag(tag))
-                  }
+            // does not seem useful to recompute this
+            // const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(
+            //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)
+            // )
+            if (change.type === 'change') {
+              console.debug('change', change, change.newValue)
+              // compute difference between old and new tags
+              const oldTags = change.oldValue as string[]
+              const newTags = change.newValue as string[]
+              const addedTags = newTags.filter(tag => !oldTags.includes(tag))
+              const removedTags = oldTags.filter(tag => !newTags.includes(tag))
+              // console.debug('addedTags', addedTags)
+              // console.debug('removedTags', removedTags)
+              cellWidgets.forEach(cellWidget => {
+                addedTags.forEach(tag => {
+                  console.debug(`adding class for tag ${class_for_tag(tag)}`)
+                  cellWidget.addClass(class_for_tag(tag))
                 })
-              } else if (change.type === 'remove') {
-                console.log('remove', change, change.newValue)
-                cellWidgets.forEach((cellWidget) => {
-                  for (const tag of change.newValue) {
-                    console.debug(`removing class for tag ${class_for_tag(tag)}`)
-                    cellWidget.removeClass(class_for_tag(tag))
-                  }
+                removedTags.forEach(tag => {
+                  console.debug(`removing class for tag ${class_for_tag(tag)}`)
+                  cellWidget.removeClass(class_for_tag(tag))
                 })
-              }
-            })
+              })
+            } else if (change.type === 'add') {
+              console.log('add', change, change.newValue)
+              cellWidgets.forEach(cellWidget => {
+                for (const tag of change.newValue) {
+                  console.debug(`adding class for tag ${class_for_tag(tag)}`)
+                  cellWidget.addClass(class_for_tag(tag))
+                }
+              })
+            } else if (change.type === 'remove') {
+              console.log('remove', change, change.newValue)
+              cellWidgets.forEach(cellWidget => {
+                for (const tag of change.newValue) {
+                  console.debug(`removing class for tag ${class_for_tag(tag)}`)
+                  cellWidget.removeClass(class_for_tag(tag))
+                }
+              })
+            }
           })
         })
       })
-    }
+    })
   }
+}
 
 export default plugin
```

### Comparing `jupyterlab_celltagsclasses-0.1.1/style/base.css` & `jupyterlab_celltagsclasses-0.1.2/style/base.css`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,24 @@
     See the JupyterLab Developer Guide for useful CSS Patterns:
 
     https://jupyterlab.readthedocs.io/en/stable/developer/css.html
 */
 
 /* hide only the input of cells with the tag 'hide-input' */
 .cell-tag-celltagsclasses-test1 {
-    padding: 10px;
-    border: 2.5px black solid;
-    border-radius: 10px;
-    background-color: yellow !important;    /* could be overridden if cell is active */
+  padding: 10px;
+  border: 2.5px black solid;
+  border-radius: 10px;
+
+  /* could be overridden if cell is active */
+  background-color: yellow !important;
 }
 
 .cell-tag-celltagsclasses-test2 {
-    background-color: red;                  /* see how it goes if cell is active */
+  /* see how it goes if cell is active */
+  background-color: red;
 }
 
 /* hide the 6-buttons toolbar */
 .cell-tag-celltagsclasses-test2 .jp-cell-toolbar {
-    display: none;
+  display: none;
 }
-
```

### Comparing `jupyterlab_celltagsclasses-0.1.1/.gitignore` & `jupyterlab_celltagsclasses-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/LICENSE` & `jupyterlab_celltagsclasses-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/README.md` & `jupyterlab_celltagsclasses-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.1/pyproject.toml` & `jupyterlab_celltagsclasses-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0b0,<5", "hatch-nodejs-version"]
+requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0rc0,<5", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab_celltagsclasses"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `jupyterlab_celltagsclasses-0.1.1/PKG-INFO` & `jupyterlab_celltagsclasses-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_celltagsclasses
-Version: 0.1.1
+Version: 0.1.2
 Summary: JLAB extension to add classes to cells based on their tags
 Project-URL: Homepage, https://github.com/parmentelat/jupyterlab-celltagsclasses
 Project-URL: Bug Tracker, https://github.com/parmentelat/jupyterlab-celltagsclasses/issues
 Project-URL: Repository, https://github.com/parmentelat/jupyterlab-celltagsclasses.git
 Author-email: Thierry Parmentelat <thierry.parmentelat@inria.fr>
 License: BSD 3-Clause License
```

