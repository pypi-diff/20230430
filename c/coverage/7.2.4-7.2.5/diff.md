# Comparing `tmp/coverage-7.2.4.tar.gz` & `tmp/coverage-7.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-7.2.4.tar", last modified: Fri Apr 28 09:58:42 2023, max compression
+gzip compressed data, was "coverage-7.2.5.tar", last modified: Sun Apr 30 10:54:22 2023, max compression
```

## Comparing `coverage-7.2.4.tar` & `coverage-7.2.5.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-28 09:58:29.000000 coverage-7.2.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-28 09:58:29.000000 coverage-7.2.4/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.756931 coverage-7.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.756931 coverage-7.2.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.756931 coverage-7.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/workflows/kit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/workflows/python-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/workflows/quality.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-28 09:58:29.000000 coverage-7.2.4/.github/workflows/testsuite.yml
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 09:58:29.000000 coverage-7.2.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    46496 2023-04-28 09:58:29.000000 coverage-7.2.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-28 09:58:29.000000 coverage-7.2.4/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-28 09:58:29.000000 coverage-7.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-28 09:58:29.000000 coverage-7.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-04-28 09:58:29.000000 coverage-7.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-28 09:58:29.000000 coverage-7.2.4/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-04-28 09:58:42.804935 coverage-7.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-04-28 09:58:29.000000 coverage-7.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 09:58:29.000000 coverage-7.2.4/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.760931 coverage-7.2.4/ci/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 09:58:29.000000 coverage-7.2.4/ci/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-28 09:58:29.000000 coverage-7.2.4/ci/comment_on_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-28 09:58:29.000000 coverage-7.2.4/ci/download_gha_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 09:58:29.000000 coverage-7.2.4/ci/ghrel_template.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-28 09:58:29.000000 coverage-7.2.4/ci/parse_relnotes.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-28 09:58:29.000000 coverage-7.2.4/ci/trigger_build_kits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.764932 coverage-7.2.4/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/bytecode.py
--rw-r--r--   0 runner    (1001) docker     (123)    34436 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    51867 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.768932 coverage-7.2.4/coverage/ctracer/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/datastack.c
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/datastack.h
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/filedisp.c
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/filedisp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/module.c
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/stats.h
--rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/tracer.c
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/tracer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/ctracer/util.h
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/disposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/execfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.768932 coverage-7.2.4/coverage/fullcoverage/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/fullcoverage/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.768932 coverage-7.2.4/coverage/htmlfiles/
--rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/htmlfiles/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/htmlfiles/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/htmlfiles/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/htmlfiles/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/htmlfiles/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/htmlfiles/pyfile.html
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/htmlfiles/style.css
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/htmlfiles/style.scss
--rw-r--r--   0 runner    (1001) docker     (123)    23900 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/inorout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/jsonreport.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/lcovreport.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/numbits.py
--rw-r--r--   0 runner    (1001) docker     (123)    56643 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/phystokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/plugin_support.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/python.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/pytracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    51295 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/sqldata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/templite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/tomlconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/tracer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-28 09:58:29.000000 coverage-7.2.4/coverage/xmlreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.764932 coverage-7.2.4/coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-04-28 09:58:42.000000 coverage-7.2.4/coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-28 09:58:42.000000 coverage-7.2.4/coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:58:42.000000 coverage-7.2.4/coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 09:58:42.000000 coverage-7.2.4/coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:58:42.000000 coverage-7.2.4/coverage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 09:58:42.000000 coverage-7.2.4/coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 09:58:42.000000 coverage-7.2.4/coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.772932 coverage-7.2.4/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.772932 coverage-7.2.4/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/_static/coverage.css
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/api_coverage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/api_coveragedata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/api_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/api_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/branch.rst
--rw-r--r--   0 runner    (1001) docker     (123)   112598 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    44128 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/cmd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/dbschema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/dict.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/excluding.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/howitworks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.772932 coverage-7.2.4/doc/media/
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png
--rw-r--r--   0 runner    (1001) docker     (123)   165210 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/media/sleepy-snake-600.png
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/media/sleepy-snake-circle-150.png
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/migrating.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/python-coverage.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/requirements.pip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.776933 coverage-7.2.4/doc/sample_html/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/sample_html/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/sample_html/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/sample_html/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/sleepy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/source.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/subprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/trouble.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-28 09:58:29.000000 coverage-7.2.4/doc/whatsnew5x.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-28 09:58:29.000000 coverage-7.2.4/howto.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-04-28 09:58:29.000000 coverage-7.2.4/igor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.776933 coverage-7.2.4/lab/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.776933 coverage-7.2.4/lab/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/benchmark/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/benchmark/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/bpo_prelude.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/branch_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/branches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/compare_times.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/coverage-03.dtd
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/coverage-04.dtd
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/find_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/genpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/hack_pyc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/new-data.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.780933 coverage-7.2.4/lab/notes/
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/notes/bug1303.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/notes/pypy-738-decorated-functions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/parse_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/platform_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/run_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/select_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/show_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/show_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/show_pyc.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 09:58:29.000000 coverage-7.2.4/lab/treetopy.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-28 09:58:29.000000 coverage-7.2.4/metacov.ini
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-28 09:58:29.000000 coverage-7.2.4/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-28 09:58:29.000000 coverage-7.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.780933 coverage-7.2.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/dev.pip
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/kit.in
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/kit.pip
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/light-threads.in
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/light-threads.pip
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/lint.pip
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/mypy.pip
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/pins.pip
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/pip-tools.pip
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/pip.pip
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/pytest.in
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/pytest.pip
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-28 09:58:29.000000 coverage-7.2.4/requirements/tox.pip
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 09:58:42.804935 coverage-7.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-28 09:58:29.000000 coverage-7.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.788934 coverage-7.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/balance_xdist_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/coveragetest.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/covmodzip1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.788934 coverage-7.2.4/tests/gold/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.748930 coverage-7.2.4/tests/gold/annotate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.788934 coverage-7.2.4/tests/gold/annotate/anno_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/anno_dir/d_80084bf2fba02475___init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/anno_dir/d_80084bf2fba02475_a.py,cover
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/anno_dir/d_b039179a8a4ce2c2___init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/anno_dir/d_b039179a8a4ce2c2_b.py,cover
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/anno_dir/multi.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.788934 coverage-7.2.4/tests/gold/annotate/encodings/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/encodings/utf8.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.788934 coverage-7.2.4/tests/gold/annotate/mae/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/mae/mae.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/annotate/multi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/annotate/multi/a/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/multi/a/__init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/multi/a/a.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/annotate/multi/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/multi/b/__init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/multi/b/b.py,cover
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/multi/multi.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/annotate/white/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/annotate/white/white.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/html/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/html/a/
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/a/a_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/a/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/html/b_branch/
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/b_branch/b_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/b_branch/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/html/bom/
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/bom/bom_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/bom/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/html/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/contexts/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/contexts/two_tests_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/html/isolatin1/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/isolatin1/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/isolatin1/isolatin1_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/html/omit_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_1/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_1/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_1/m2_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_1/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_1/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.792934 coverage-7.2.4/tests/gold/html/omit_2/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_2/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_2/m2_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_2/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_2/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/omit_3/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_3/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_3/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_3/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/omit_4/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_4/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_4/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_4/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_4/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/omit_5/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_5/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_5/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/omit_5/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/other/
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/other/blah_blah_other_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/other/here_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/other/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/partial/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/partial/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/partial/partial_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/partial_626/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/partial_626/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/partial_626/partial_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/styled/
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/styled/a_py.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/styled/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/styled/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/styled/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/support/
--rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/support/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/support/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/support/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/support/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/support/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.796934 coverage-7.2.4/tests/gold/html/unicode/
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/unicode/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/html/unicode/unicode_py.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.752930 coverage-7.2.4/tests/gold/testing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/gold/testing/getty/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/testing/getty/gettysburg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/gold/testing/xml/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/testing/xml/output.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.752930 coverage-7.2.4/tests/gold/xml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/gold/xml/x_xml/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/xml/x_xml/coverage.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/gold/xml/y_xml_branch/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/gold/xml/y_xml_branch/coverage.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/goldtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/js/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/aa/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/afile.odd.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/afile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/aa/bb/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/bb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/bb/bfile.odd.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/bb/bfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/aa/bb/cc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/bb/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/bb/cc/cfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/aa/bb.odd/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/bb.odd/bfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/aa/zfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/ambiguous/pkg1/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/ambiguous/pkg1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/ambiguous/pkg1/ambiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/covmod1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.752930 coverage-7.2.4/tests/modules/namespace_420/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/namespace_420/sub1/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/namespace_420/sub1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.800935 coverage-7.2.4/tests/modules/pkg1/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/p1a.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/p1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/p1c.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/runmod2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/modules/pkg1/sub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/sub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/sub/ps1a.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg1/sub/runmod3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/modules/pkg2/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg2/p2a.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/pkg2/p2b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/modules/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/plugins/a_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/plugins/another.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/modules/process_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/process_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/process_test/try_execfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/runmod1.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/modules/usepkgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.752930 coverage-7.2.4/tests/moremodules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.752930 coverage-7.2.4/tests/moremodules/namespace_420/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/moremodules/namespace_420/sub2/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/moremodules/namespace_420/sub2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/moremodules/othermods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/moremodules/othermods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/moremodules/othermods/othera.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/moremodules/othermods/otherb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/moremodules/othermods/sub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/moremodules/othermods/sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/moremodules/othermods/sub/osa.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/moremodules/othermods/sub/osb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/plugin1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/plugin2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/plugin_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/qunit/
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/qunit/jquery.tmpl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/stress_phystoken.tok
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/stress_phystoken_dos.tok
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    61833 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    63100 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_arcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44163 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    27122 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)    31526 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    50465 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)    37653 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_execfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_filereporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27463 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_goldtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    48809 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_lcov.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_numbits.py
--rw-r--r--   0 runner    (1001) docker     (123)    22363 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_oddball.py
--rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_phystokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    43888 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    47552 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_templite.py
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/test_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.752930 coverage-7.2.4/tests/zipsrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:42.804935 coverage-7.2.4/tests/zipsrc/zip1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/zipsrc/zip1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-28 09:58:29.000000 coverage-7.2.4/tests/zipsrc/zip1/zip1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-28 09:58:29.000000 coverage-7.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.305687 coverage-7.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-30 10:54:11.000000 coverage-7.2.5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-30 10:54:11.000000 coverage-7.2.5/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.261686 coverage-7.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.261686 coverage-7.2.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.265686 coverage-7.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/workflows/kit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/workflows/python-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/workflows/quality.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-30 10:54:11.000000 coverage-7.2.5/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-30 10:54:11.000000 coverage-7.2.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    46741 2023-04-30 10:54:11.000000 coverage-7.2.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-30 10:54:11.000000 coverage-7.2.5/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-30 10:54:11.000000 coverage-7.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-30 10:54:11.000000 coverage-7.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-04-30 10:54:11.000000 coverage-7.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-30 10:54:11.000000 coverage-7.2.5/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-04-30 10:54:22.305687 coverage-7.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-04-30 10:54:11.000000 coverage-7.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-30 10:54:11.000000 coverage-7.2.5/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.265686 coverage-7.2.5/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-30 10:54:11.000000 coverage-7.2.5/ci/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-30 10:54:11.000000 coverage-7.2.5/ci/comment_on_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-30 10:54:11.000000 coverage-7.2.5/ci/download_gha_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-30 10:54:11.000000 coverage-7.2.5/ci/ghrel_template.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-30 10:54:11.000000 coverage-7.2.5/ci/parse_relnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-30 10:54:11.000000 coverage-7.2.5/ci/trigger_build_kits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.269686 coverage-7.2.5/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34436 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51867 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.273686 coverage-7.2.5/coverage/ctracer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/datastack.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/datastack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/filedisp.c
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/filedisp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/tracer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/tracer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/ctracer/util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/disposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/execfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.273686 coverage-7.2.5/coverage/fullcoverage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/fullcoverage/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.273686 coverage-7.2.5/coverage/htmlfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/htmlfiles/coverage_html.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/htmlfiles/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/htmlfiles/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/htmlfiles/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/htmlfiles/keybd_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/htmlfiles/pyfile.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/htmlfiles/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/htmlfiles/style.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    23900 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/inorout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/jsonreport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/lcovreport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/numbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56643 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/phystokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/plugin_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/pytracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51295 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/sqldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/templite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/tomlconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/tracer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-30 10:54:11.000000 coverage-7.2.5/coverage/xmlreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.269686 coverage-7.2.5/coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-04-30 10:54:22.000000 coverage-7.2.5/coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-30 10:54:22.000000 coverage-7.2.5/coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:54:22.000000 coverage-7.2.5/coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-30 10:54:22.000000 coverage-7.2.5/coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:54:22.000000 coverage-7.2.5/coverage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 10:54:22.000000 coverage-7.2.5/coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 10:54:22.000000 coverage-7.2.5/coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.277686 coverage-7.2.5/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.277686 coverage-7.2.5/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/_static/coverage.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/api_coverage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/api_coveragedata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/api_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/api_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/branch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   112598 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    44128 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/cmd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/dbschema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/dict.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/excluding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/howitworks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.277686 coverage-7.2.5/doc/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)   165210 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/media/sleepy-snake-600.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/media/sleepy-snake-circle-150.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/migrating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/python-coverage.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.277686 coverage-7.2.5/doc/sample_html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/sample_html/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/sample_html/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/sample_html/keybd_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/sleepy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/source.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/subprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/trouble.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-30 10:54:11.000000 coverage-7.2.5/doc/whatsnew5x.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-30 10:54:11.000000 coverage-7.2.5/howto.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-04-30 10:54:11.000000 coverage-7.2.5/igor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.281686 coverage-7.2.5/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.281686 coverage-7.2.5/lab/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/benchmark/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/benchmark/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/bpo_prelude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/branch_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/compare_times.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/coverage-03.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/coverage-04.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/find_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/genpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/hack_pyc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/new-data.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.281686 coverage-7.2.5/lab/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/notes/bug1303.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/notes/pypy-738-decorated-functions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/parse_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/platform_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/run_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/select_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/show_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/show_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/show_pyc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-30 10:54:11.000000 coverage-7.2.5/lab/treetopy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-30 10:54:11.000000 coverage-7.2.5/metacov.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-30 10:54:11.000000 coverage-7.2.5/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-30 10:54:11.000000 coverage-7.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.281686 coverage-7.2.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/dev.pip
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/kit.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/kit.pip
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/light-threads.in
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/light-threads.pip
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/lint.pip
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/mypy.pip
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/pins.pip
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/pip-tools.pip
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/pip.pip
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/pytest.in
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/pytest.pip
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-30 10:54:11.000000 coverage-7.2.5/requirements/tox.pip
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-30 10:54:22.305687 coverage-7.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-30 10:54:11.000000 coverage-7.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.289686 coverage-7.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/balance_xdist_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/coveragetest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/covmodzip1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.289686 coverage-7.2.5/tests/gold/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.257686 coverage-7.2.5/tests/gold/annotate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.289686 coverage-7.2.5/tests/gold/annotate/anno_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/anno_dir/d_80084bf2fba02475___init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/anno_dir/d_80084bf2fba02475_a.py,cover
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/anno_dir/d_b039179a8a4ce2c2___init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/anno_dir/d_b039179a8a4ce2c2_b.py,cover
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/anno_dir/multi.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.289686 coverage-7.2.5/tests/gold/annotate/encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/encodings/utf8.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.289686 coverage-7.2.5/tests/gold/annotate/mae/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/mae/mae.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/annotate/multi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/annotate/multi/a/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/multi/a/__init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/multi/a/a.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/annotate/multi/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/multi/b/__init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/multi/b/b.py,cover
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/multi/multi.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/annotate/white/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/annotate/white/white.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/a/
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/a/a_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/a/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/b_branch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/b_branch/b_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/b_branch/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/bom/
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/bom/bom_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/bom/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/contexts/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/contexts/two_tests_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/isolatin1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/isolatin1/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/isolatin1/isolatin1_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/omit_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_1/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_1/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_1/m2_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_1/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_1/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/omit_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_2/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_2/m2_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_2/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_2/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.293686 coverage-7.2.5/tests/gold/html/omit_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_3/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_3/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_3/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/html/omit_4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_4/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_4/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_4/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_4/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/html/omit_5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_5/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_5/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/omit_5/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/html/other/
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/other/blah_blah_other_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/other/here_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/other/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/html/partial/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/partial/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/partial/partial_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/html/partial_626/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/partial_626/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/partial_626/partial_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/html/styled/
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/styled/a_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/styled/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/styled/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/styled/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/html/support/
+-rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/support/coverage_html.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/support/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/support/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/support/keybd_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/support/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/html/unicode/
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/unicode/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/html/unicode/unicode_py.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.257686 coverage-7.2.5/tests/gold/testing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/testing/getty/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/testing/getty/gettysburg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/testing/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/testing/xml/output.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.257686 coverage-7.2.5/tests/gold/xml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/xml/x_xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/xml/x_xml/coverage.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/gold/xml/y_xml_branch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/gold/xml/y_xml_branch/coverage.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/goldtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.297687 coverage-7.2.5/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/js/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/aa/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/afile.odd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/afile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/aa/bb/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/bb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/bb/bfile.odd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/bb/bfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/aa/bb/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/bb/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/bb/cc/cfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/aa/bb.odd/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/bb.odd/bfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/aa/zfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/ambiguous/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/ambiguous/pkg1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/ambiguous/pkg1/ambiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/covmod1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.257686 coverage-7.2.5/tests/modules/namespace_420/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/namespace_420/sub1/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/namespace_420/sub1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/p1a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/p1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/p1c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/runmod2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/pkg1/sub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/sub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/sub/ps1a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg1/sub/runmod3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/pkg2/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg2/p2a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/pkg2/p2b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/plugins/a_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/plugins/another.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.301687 coverage-7.2.5/tests/modules/process_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/process_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/process_test/try_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/runmod1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/modules/usepkgs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.257686 coverage-7.2.5/tests/moremodules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.257686 coverage-7.2.5/tests/moremodules/namespace_420/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.305687 coverage-7.2.5/tests/moremodules/namespace_420/sub2/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/moremodules/namespace_420/sub2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.305687 coverage-7.2.5/tests/moremodules/othermods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/moremodules/othermods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/moremodules/othermods/othera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/moremodules/othermods/otherb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.305687 coverage-7.2.5/tests/moremodules/othermods/sub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/moremodules/othermods/sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/moremodules/othermods/sub/osa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/moremodules/othermods/sub/osb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/plugin1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/plugin2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/plugin_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.305687 coverage-7.2.5/tests/qunit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/qunit/jquery.tmpl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/stress_phystoken.tok
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/stress_phystoken_dos.tok
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61833 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63100 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_arcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44163 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27122 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31526 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50465 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37653 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_filereporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27463 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_goldtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48809 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_lcov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_numbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22363 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_oddball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_phystokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43888 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47552 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_templite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.257686 coverage-7.2.5/tests/zipsrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:22.305687 coverage-7.2.5/tests/zipsrc/zip1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/zipsrc/zip1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-30 10:54:11.000000 coverage-7.2.5/tests/zipsrc/zip1/zip1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-30 10:54:11.000000 coverage-7.2.5/tox.ini
```

### Comparing `coverage-7.2.4/.editorconfig` & `coverage-7.2.5/.editorconfig`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/ISSUE_TEMPLATE/bug_report.md` & `coverage-7.2.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/ISSUE_TEMPLATE/config.yml` & `coverage-7.2.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/ISSUE_TEMPLATE/feature_request.md` & `coverage-7.2.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/workflows/codeql-analysis.yml` & `coverage-7.2.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/workflows/coverage.yml` & `coverage-7.2.5/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/workflows/dependency-review.yml` & `coverage-7.2.5/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/workflows/kit.yml` & `coverage-7.2.5/.github/workflows/kit.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/workflows/python-nightly.yml` & `coverage-7.2.5/.github/workflows/python-nightly.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/workflows/quality.yml` & `coverage-7.2.5/.github/workflows/quality.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.github/workflows/testsuite.yml` & `coverage-7.2.5/.github/workflows/testsuite.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/.readthedocs.yml` & `coverage-7.2.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/CHANGES.rst` & `coverage-7.2.5/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,24 @@
     ..  .. _changes_9-8-1:
     ..
     ..  Version 9.8.1 — 2027-07-27
     ..  --------------------------
 
 .. scriv-start-here
 
+.. _changes_7-2-5:
+
+Version 7.2.5 — 2023-04-30
+--------------------------
+
+- Fix: ``html_report()`` could fail with an AttributeError on ``isatty`` if run
+  in an unusual environment where sys.stdout had been replaced.  This is now
+  fixed.
+
+
 .. _changes_7-2-4:
 
 Version 7.2.4 — 2023-04-28
 --------------------------
 
 PyCon 2023 sprint fixes!
```

### Comparing `coverage-7.2.4/CONTRIBUTORS.txt` & `coverage-7.2.5/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/LICENSE.txt` & `coverage-7.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/MANIFEST.in` & `coverage-7.2.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/Makefile` & `coverage-7.2.5/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -85,25 +85,27 @@
 # and extra requirements that have been needed, but might be obsolete.
 
 .PHONY: upgrade
 
 PIP_COMPILE = pip-compile --upgrade --allow-unsafe --resolver=backtracking
 upgrade: export CUSTOM_COMPILE_COMMAND=make upgrade
 upgrade: 				## Update the *.pip files with the latest packages satisfying *.in files.
+	git switch -c nedbat/upgrade-$$(date +%Y%m%d)
 	pip install -q -r requirements/pip-tools.pip
 	$(PIP_COMPILE) -o requirements/pip-tools.pip requirements/pip-tools.in
 	$(PIP_COMPILE) -o requirements/pip.pip requirements/pip.in
 	$(PIP_COMPILE) -o requirements/pytest.pip requirements/pytest.in
 	$(PIP_COMPILE) -o requirements/kit.pip requirements/kit.in
 	$(PIP_COMPILE) -o requirements/tox.pip requirements/tox.in
 	$(PIP_COMPILE) -o requirements/dev.pip requirements/dev.in
 	$(PIP_COMPILE) -o requirements/light-threads.pip requirements/light-threads.in
 	$(PIP_COMPILE) -o doc/requirements.pip doc/requirements.in
 	$(PIP_COMPILE) -o requirements/lint.pip doc/requirements.in requirements/dev.in
 	$(PIP_COMPILE) -o requirements/mypy.pip requirements/mypy.in
+	git commit -am "chore: make upgrade"
 
 diff_upgrade:				## Summarize the last `make upgrade`
 	@# The sort flags sort by the package name first, then by the -/+, and
 	@# sort by version numbers, so we get a summary with lines like this:
 	@#	-bashlex==0.16
 	@#	+bashlex==0.17
 	@#	-build==0.9.0
```

### Comparing `coverage-7.2.4/NOTICE.txt` & `coverage-7.2.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/PKG-INFO` & `coverage-7.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: coverage
-Version: 7.2.4
+Version: 7.2.5
 Summary: Code coverage measurement for Python
 Home-page: https://github.com/nedbat/coveragepy
 Author: Ned Batchelder and 211 others
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
-Project-URL: Documentation, https://coverage.readthedocs.io/en/7.2.4
+Project-URL: Documentation, https://coverage.readthedocs.io/en/7.2.5
 Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-coverage?utm_source=pypi-coverage&utm_medium=referral&utm_campaign=pypi
 Project-URL: Issues, https://github.com/nedbat/coveragepy/issues
 Project-URL: Mastodon, https://hachyderm.io/@coveragepy
 Project-URL: Mastodon (nedbat), https://hachyderm.io/@nedbat
 Keywords: code coverage testing
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -66,15 +66,15 @@
 
 * CPython 3.7 through 3.12.0a7
 * PyPy3 7.3.11.
 
 Documentation is on `Read the Docs`_.  Code repository and issue tracker are on
 `GitHub`_.
 
-.. _Read the Docs: https://coverage.readthedocs.io/en/7.2.4/
+.. _Read the Docs: https://coverage.readthedocs.io/en/7.2.5/
 .. _GitHub: https://github.com/nedbat/coveragepy
 
 **New in 7.x:**
 improved data combining;
 ``report --format=``;
 type annotations.
 
@@ -105,23 +105,23 @@
 
 Getting Started
 ---------------
 
 Looking to run ``coverage`` on your test suite? See the `Quick Start section`_
 of the docs.
 
-.. _Quick Start section: https://coverage.readthedocs.io/en/7.2.4/#quick-start
+.. _Quick Start section: https://coverage.readthedocs.io/en/7.2.5/#quick-start
 
 
 Change history
 --------------
 
 The complete history of changes is on the `change history page`_.
 
-.. _change history page: https://coverage.readthedocs.io/en/7.2.4/changes.html
+.. _change history page: https://coverage.readthedocs.io/en/7.2.5/changes.html
 
 
 Code of Conduct
 ---------------
 
 Everyone participating in the coverage.py project is expected to treat other
 people with respect and to follow the guidelines articulated in the `Python
@@ -132,15 +132,15 @@
 
 Contributing
 ------------
 
 Found a bug? Want to help improve the code or documentation? See the
 `Contributing section`_ of the docs.
 
-.. _Contributing section: https://coverage.readthedocs.io/en/7.2.4/contributing.html
+.. _Contributing section: https://coverage.readthedocs.io/en/7.2.5/contributing.html
 
 
 Security
 --------
 
 To report a security vulnerability, please use the `Tidelift security
 contact`_.  Tidelift will coordinate the fix and disclosure.
@@ -160,15 +160,15 @@
 .. |test-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml
     :alt: Test suite status
 .. |quality-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml
     :alt: Quality check status
 .. |docs| image:: https://readthedocs.org/projects/coverage/badge/?version=latest&style=flat
-    :target: https://coverage.readthedocs.io/en/7.2.4/
+    :target: https://coverage.readthedocs.io/en/7.2.5/
     :alt: Documentation
 .. |kit| image:: https://badge.fury.io/py/coverage.svg
     :target: https://pypi.org/project/coverage/
     :alt: PyPI status
 .. |format| image:: https://img.shields.io/pypi/format/coverage.svg
     :target: https://pypi.org/project/coverage/
     :alt: Kit format
```

### Comparing `coverage-7.2.4/README.rst` & `coverage-7.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/ci/comment_on_fixes.py` & `coverage-7.2.5/ci/comment_on_fixes.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/ci/download_gha_artifacts.py` & `coverage-7.2.5/ci/download_gha_artifacts.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/ci/parse_relnotes.py` & `coverage-7.2.5/ci/parse_relnotes.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/ci/trigger_build_kits.py` & `coverage-7.2.5/ci/trigger_build_kits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/__init__.py` & `coverage-7.2.5/coverage/__init__.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/annotate.py` & `coverage-7.2.5/coverage/annotate.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/bytecode.py` & `coverage-7.2.5/coverage/bytecode.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/cmdline.py` & `coverage-7.2.5/coverage/cmdline.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/collector.py` & `coverage-7.2.5/coverage/collector.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/config.py` & `coverage-7.2.5/coverage/config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/context.py` & `coverage-7.2.5/coverage/context.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/control.py` & `coverage-7.2.5/coverage/control.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/datastack.c` & `coverage-7.2.5/coverage/ctracer/datastack.c`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/datastack.h` & `coverage-7.2.5/coverage/ctracer/datastack.h`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/filedisp.c` & `coverage-7.2.5/coverage/ctracer/filedisp.c`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/filedisp.h` & `coverage-7.2.5/coverage/ctracer/filedisp.h`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/module.c` & `coverage-7.2.5/coverage/ctracer/module.c`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/stats.h` & `coverage-7.2.5/coverage/ctracer/stats.h`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/tracer.c` & `coverage-7.2.5/coverage/ctracer/tracer.c`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/tracer.h` & `coverage-7.2.5/coverage/ctracer/tracer.h`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/ctracer/util.h` & `coverage-7.2.5/coverage/ctracer/util.h`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/data.py` & `coverage-7.2.5/coverage/data.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/debug.py` & `coverage-7.2.5/coverage/debug.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/disposition.py` & `coverage-7.2.5/coverage/disposition.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/env.py` & `coverage-7.2.5/coverage/env.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/exceptions.py` & `coverage-7.2.5/coverage/exceptions.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/execfile.py` & `coverage-7.2.5/coverage/execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/files.py` & `coverage-7.2.5/coverage/files.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/fullcoverage/encodings.py` & `coverage-7.2.5/coverage/fullcoverage/encodings.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/html.py` & `coverage-7.2.5/coverage/html.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/htmlfiles/coverage_html.js` & `coverage-7.2.5/coverage/htmlfiles/coverage_html.js`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/htmlfiles/favicon_32.png` & `coverage-7.2.5/coverage/htmlfiles/favicon_32.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/htmlfiles/index.html` & `coverage-7.2.5/coverage/htmlfiles/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/htmlfiles/keybd_closed.png` & `coverage-7.2.5/coverage/htmlfiles/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/htmlfiles/keybd_open.png` & `coverage-7.2.5/coverage/htmlfiles/keybd_open.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/htmlfiles/pyfile.html` & `coverage-7.2.5/coverage/htmlfiles/pyfile.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/htmlfiles/style.css` & `coverage-7.2.5/coverage/htmlfiles/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/htmlfiles/style.scss` & `coverage-7.2.5/coverage/htmlfiles/style.scss`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/inorout.py` & `coverage-7.2.5/coverage/inorout.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/jsonreport.py` & `coverage-7.2.5/coverage/jsonreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/lcovreport.py` & `coverage-7.2.5/coverage/lcovreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/misc.py` & `coverage-7.2.5/coverage/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,11 +390,11 @@
 
 def stdout_link(text: str, url: str) -> str:
     """Format text+url as a clickable link for stdout.
 
     If attached to a terminal, use escape sequences. Otherwise, just return
     the text.
     """
-    if sys.stdout.isatty():
+    if hasattr(sys.stdout, "isatty") and sys.stdout.isatty():
         return f"\033]8;;{url}\a{text}\033]8;;\a"
     else:
         return text
```

### Comparing `coverage-7.2.4/coverage/multiproc.py` & `coverage-7.2.5/coverage/multiproc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/numbits.py` & `coverage-7.2.5/coverage/numbits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/parser.py` & `coverage-7.2.5/coverage/parser.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/phystokens.py` & `coverage-7.2.5/coverage/phystokens.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/plugin.py` & `coverage-7.2.5/coverage/plugin.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/plugin_support.py` & `coverage-7.2.5/coverage/plugin_support.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/python.py` & `coverage-7.2.5/coverage/python.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/pytracer.py` & `coverage-7.2.5/coverage/pytracer.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/report.py` & `coverage-7.2.5/coverage/report.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/results.py` & `coverage-7.2.5/coverage/results.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/sqldata.py` & `coverage-7.2.5/coverage/sqldata.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/summary.py` & `coverage-7.2.5/coverage/summary.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/templite.py` & `coverage-7.2.5/coverage/templite.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/tomlconfig.py` & `coverage-7.2.5/coverage/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/tracer.pyi` & `coverage-7.2.5/coverage/tracer.pyi`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/types.py` & `coverage-7.2.5/coverage/types.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage/version.py` & `coverage-7.2.5/coverage/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """The version and URL for coverage.py"""
 # This file is exec'ed in setup.py, don't import anything!
 
 from __future__ import annotations
 
 # version_info: same semantics as sys.version_info.
 # _dev: the .devN suffix if any.
-version_info = (7, 2, 4, "final", 0)
+version_info = (7, 2, 5, "final", 0)
 _dev = 0
 
 
 def _make_version(
     major: int,
     minor: int,
     micro: int,
```

### Comparing `coverage-7.2.4/coverage/xmlreport.py` & `coverage-7.2.5/coverage/xmlreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/coverage.egg-info/PKG-INFO` & `coverage-7.2.5/coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: coverage
-Version: 7.2.4
+Version: 7.2.5
 Summary: Code coverage measurement for Python
 Home-page: https://github.com/nedbat/coveragepy
 Author: Ned Batchelder and 211 others
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
-Project-URL: Documentation, https://coverage.readthedocs.io/en/7.2.4
+Project-URL: Documentation, https://coverage.readthedocs.io/en/7.2.5
 Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-coverage?utm_source=pypi-coverage&utm_medium=referral&utm_campaign=pypi
 Project-URL: Issues, https://github.com/nedbat/coveragepy/issues
 Project-URL: Mastodon, https://hachyderm.io/@coveragepy
 Project-URL: Mastodon (nedbat), https://hachyderm.io/@nedbat
 Keywords: code coverage testing
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -66,15 +66,15 @@
 
 * CPython 3.7 through 3.12.0a7
 * PyPy3 7.3.11.
 
 Documentation is on `Read the Docs`_.  Code repository and issue tracker are on
 `GitHub`_.
 
-.. _Read the Docs: https://coverage.readthedocs.io/en/7.2.4/
+.. _Read the Docs: https://coverage.readthedocs.io/en/7.2.5/
 .. _GitHub: https://github.com/nedbat/coveragepy
 
 **New in 7.x:**
 improved data combining;
 ``report --format=``;
 type annotations.
 
@@ -105,23 +105,23 @@
 
 Getting Started
 ---------------
 
 Looking to run ``coverage`` on your test suite? See the `Quick Start section`_
 of the docs.
 
-.. _Quick Start section: https://coverage.readthedocs.io/en/7.2.4/#quick-start
+.. _Quick Start section: https://coverage.readthedocs.io/en/7.2.5/#quick-start
 
 
 Change history
 --------------
 
 The complete history of changes is on the `change history page`_.
 
-.. _change history page: https://coverage.readthedocs.io/en/7.2.4/changes.html
+.. _change history page: https://coverage.readthedocs.io/en/7.2.5/changes.html
 
 
 Code of Conduct
 ---------------
 
 Everyone participating in the coverage.py project is expected to treat other
 people with respect and to follow the guidelines articulated in the `Python
@@ -132,15 +132,15 @@
 
 Contributing
 ------------
 
 Found a bug? Want to help improve the code or documentation? See the
 `Contributing section`_ of the docs.
 
-.. _Contributing section: https://coverage.readthedocs.io/en/7.2.4/contributing.html
+.. _Contributing section: https://coverage.readthedocs.io/en/7.2.5/contributing.html
 
 
 Security
 --------
 
 To report a security vulnerability, please use the `Tidelift security
 contact`_.  Tidelift will coordinate the fix and disclosure.
@@ -160,15 +160,15 @@
 .. |test-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml
     :alt: Test suite status
 .. |quality-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml
     :alt: Quality check status
 .. |docs| image:: https://readthedocs.org/projects/coverage/badge/?version=latest&style=flat
-    :target: https://coverage.readthedocs.io/en/7.2.4/
+    :target: https://coverage.readthedocs.io/en/7.2.5/
     :alt: Documentation
 .. |kit| image:: https://badge.fury.io/py/coverage.svg
     :target: https://pypi.org/project/coverage/
     :alt: PyPI status
 .. |format| image:: https://img.shields.io/pypi/format/coverage.svg
     :target: https://pypi.org/project/coverage/
     :alt: Kit format
```

### Comparing `coverage-7.2.4/coverage.egg-info/SOURCES.txt` & `coverage-7.2.5/coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/_static/coverage.css` & `coverage-7.2.5/doc/_static/coverage.css`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/api.rst` & `coverage-7.2.5/doc/api.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/api_module.rst` & `coverage-7.2.5/doc/api_module.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/api_plugin.rst` & `coverage-7.2.5/doc/api_plugin.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/branch.rst` & `coverage-7.2.5/doc/branch.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/changes.rst` & `coverage-7.2.5/doc/changes.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/cmd.rst` & `coverage-7.2.5/doc/cmd.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/conf.py` & `coverage-7.2.5/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,19 +62,19 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
 # @@@ editable
 copyright = "2009–2023, Ned Batchelder" # pylint: disable=redefined-builtin
 # The short X.Y.Z version.
-version = "7.2.4"
+version = "7.2.5"
 # The full version, including alpha/beta/rc tags.
-release = "7.2.4"
+release = "7.2.5"
 # The date of release, in "monthname day, year" format.
-release_date = "April 28, 2023"
+release_date = "April 30, 2023"
 # @@@ end
 
 rst_epilog = """
 .. |release_date| replace:: {release_date}
 .. |coverage-equals-release| replace:: coverage=={release}
 .. |doc-url| replace:: https://coverage.readthedocs.io/en/{release}
 .. |br| raw:: html
```

### Comparing `coverage-7.2.4/doc/config.rst` & `coverage-7.2.5/doc/config.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/contexts.rst` & `coverage-7.2.5/doc/contexts.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/contributing.rst` & `coverage-7.2.5/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/dbschema.rst` & `coverage-7.2.5/doc/dbschema.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/dict.txt` & `coverage-7.2.5/doc/dict.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/excluding.rst` & `coverage-7.2.5/doc/excluding.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/faq.rst` & `coverage-7.2.5/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/howitworks.rst` & `coverage-7.2.5/doc/howitworks.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/index.rst` & `coverage-7.2.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/install.rst` & `coverage-7.2.5/doc/install.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png` & `coverage-7.2.5/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png` & `coverage-7.2.5/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/media/sleepy-snake-600.png` & `coverage-7.2.5/doc/media/sleepy-snake-600.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/media/sleepy-snake-circle-150.png` & `coverage-7.2.5/doc/media/sleepy-snake-circle-150.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/migrating.rst` & `coverage-7.2.5/doc/migrating.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/plugins.rst` & `coverage-7.2.5/doc/plugins.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/python-coverage.1.txt` & `coverage-7.2.5/doc/python-coverage.1.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/requirements.pip` & `coverage-7.2.5/doc/requirements.pip`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     # via
     #   -r doc/requirements.in
     #   sphinxcontrib-spelling
 pygments==2.15.1
     # via sphinx
 pytz==2023.3
     # via babel
-requests==2.28.2
+requests==2.29.0
     # via
     #   scriv
     #   sphinx
 scriv==1.3.1
     # via -r doc/requirements.in
 six==1.16.0
     # via livereload
```

### Comparing `coverage-7.2.4/doc/sample_html/favicon_32.png` & `coverage-7.2.5/doc/sample_html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/sample_html/keybd_closed.png` & `coverage-7.2.5/doc/sample_html/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/sample_html/keybd_open.png` & `coverage-7.2.5/doc/sample_html/keybd_open.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/sleepy.rst` & `coverage-7.2.5/doc/sleepy.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/source.rst` & `coverage-7.2.5/doc/source.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/subprocess.rst` & `coverage-7.2.5/doc/subprocess.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/trouble.rst` & `coverage-7.2.5/doc/trouble.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/doc/whatsnew5x.rst` & `coverage-7.2.5/doc/whatsnew5x.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/howto.txt` & `coverage-7.2.5/howto.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/igor.py` & `coverage-7.2.5/igor.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/benchmark/benchmark.py` & `coverage-7.2.5/lab/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/benchmark/empty.py` & `coverage-7.2.5/lab/benchmark/empty.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/benchmark/run.py` & `coverage-7.2.5/lab/benchmark/run.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/branches.py` & `coverage-7.2.5/lab/branches.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/compare_times.sh` & `coverage-7.2.5/lab/compare_times.sh`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/coverage-03.dtd` & `coverage-7.2.5/lab/coverage-03.dtd`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/coverage-04.dtd` & `coverage-7.2.5/lab/coverage-04.dtd`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/extract_code.py` & `coverage-7.2.5/lab/extract_code.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/find_class.py` & `coverage-7.2.5/lab/find_class.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/genpy.py` & `coverage-7.2.5/lab/genpy.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/goals.py` & `coverage-7.2.5/lab/goals.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/hack_pyc.py` & `coverage-7.2.5/lab/hack_pyc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/new-data.js` & `coverage-7.2.5/lab/new-data.js`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/notes/bug1303.txt` & `coverage-7.2.5/lab/notes/bug1303.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/notes/pypy-738-decorated-functions.txt` & `coverage-7.2.5/lab/notes/pypy-738-decorated-functions.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/parse_all.py` & `coverage-7.2.5/lab/parse_all.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/parser.py` & `coverage-7.2.5/lab/parser.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/platform_info.py` & `coverage-7.2.5/lab/platform_info.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/run_trace.py` & `coverage-7.2.5/lab/run_trace.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/select_contexts.py` & `coverage-7.2.5/lab/select_contexts.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/lab/show_pyc.py` & `coverage-7.2.5/lab/show_pyc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/metacov.ini` & `coverage-7.2.5/metacov.ini`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/pylintrc` & `coverage-7.2.5/pylintrc`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/pyproject.toml` & `coverage-7.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/requirements/dev.in` & `coverage-7.2.5/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/requirements/dev.pip` & `coverage-7.2.5/requirements/dev.pip`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     # via
     #   tox
     #   virtualenv
 flaky==3.7.0
     # via -r requirements/pytest.in
 greenlet==2.0.2
     # via -r requirements/dev.in
-hypothesis==6.72.2
+hypothesis==6.74.1
     # via -r requirements/pytest.in
 idna==3.4
     # via requests
 importlib-metadata==6.6.0
     # via
     #   attrs
     #   build
@@ -94,15 +94,15 @@
     #   pyproject-api
     #   pytest
     #   tox
 parso==0.8.3
     # via jedi
 pkginfo==1.9.6
     # via twine
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via
     #   pylint
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -110,15 +110,15 @@
 pudb==2022.1.3
     # via -r requirements/dev.in
 pygments==2.15.1
     # via
     #   pudb
     #   readme-renderer
     #   rich
-pylint==2.17.2
+pylint==2.17.3
     # via -r requirements/dev.in
 pyproject-api==1.5.1
     # via tox
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
     # via
@@ -126,41 +126,41 @@
     #   pytest-xdist
 pytest-xdist==3.2.1
     # via -r requirements/pytest.in
 readme-renderer==37.3
     # via
     #   -r requirements/dev.in
     #   twine
-requests==2.28.2
+requests==2.29.0
     # via
     #   -r requirements/dev.in
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.4
+rich==13.3.5
     # via twine
 six==1.16.0
     # via bleach
 sortedcontainers==2.4.0
     # via hypothesis
 tomli==2.0.1
     # via
     #   build
     #   check-manifest
     #   pylint
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via pylint
-tox==4.5.0
+tox==4.5.1
     # via
     #   -r requirements/tox.in
     #   tox-gh
 tox-gh==1.0.0
     # via -r requirements/tox.in
 twine==4.0.2
     # via -r requirements/dev.in
@@ -181,28 +181,28 @@
     #   twine
 urwid==2.1.2
     # via
     #   pudb
     #   urwid-readline
 urwid-readline==0.13
     # via pudb
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via
     #   -r requirements/pip.in
     #   tox
 webencodings==0.5.1
     # via bleach
 wrapt==1.15.0
     # via astroid
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==23.1.1
+pip==23.1.2
     # via -r requirements/pip.in
 setuptools==65.7.0
     # via
     #   -c requirements/pins.pip
     #   -r requirements/pip.in
     #   check-manifest
```

### Comparing `coverage-7.2.4/requirements/kit.pip` & `coverage-7.2.5/requirements/kit.pip`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # via
     #   auditwheel
     #   build
 packaging==23.1
     # via
     #   build
     #   cibuildwheel
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via cibuildwheel
 pyelftools==0.29
     # via auditwheel
 pyproject-hooks==1.0.0
     # via build
 tomli==2.0.1
     # via
```

### Comparing `coverage-7.2.4/requirements/light-threads.pip` & `coverage-7.2.5/requirements/light-threads.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/requirements/lint.pip` & `coverage-7.2.5/requirements/lint.pip`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # via
     #   tox
     #   virtualenv
 flaky==3.7.0
     # via -r requirements/pytest.in
 greenlet==2.0.2
     # via -r requirements/dev.in
-hypothesis==6.72.2
+hypothesis==6.74.1
     # via -r requirements/pytest.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==6.6.0
     # via
@@ -126,15 +126,15 @@
     #   pytest
     #   sphinx
     #   tox
 parso==0.8.3
     # via jedi
 pkginfo==1.9.6
     # via twine
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via
     #   pylint
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -147,15 +147,15 @@
     #   sphinxcontrib-spelling
 pygments==2.15.1
     # via
     #   pudb
     #   readme-renderer
     #   rich
     #   sphinx
-pylint==2.17.2
+pylint==2.17.3
     # via -r requirements/dev.in
 pyproject-api==1.5.1
     # via tox
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
     # via
@@ -165,26 +165,26 @@
     # via -r requirements/pytest.in
 pytz==2023.3
     # via babel
 readme-renderer==37.3
     # via
     #   -r requirements/dev.in
     #   twine
-requests==2.28.2
+requests==2.29.0
     # via
     #   -r requirements/dev.in
     #   requests-toolbelt
     #   scriv
     #   sphinx
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.4
+rich==13.3.5
     # via twine
 scriv==1.3.1
     # via -r doc/requirements.in
 six==1.16.0
     # via
     #   bleach
     #   livereload
@@ -227,19 +227,19 @@
     #   build
     #   check-manifest
     #   pylint
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via pylint
 tornado==6.2
     # via livereload
-tox==4.5.0
+tox==4.5.1
     # via
     #   -r requirements/tox.in
     #   tox-gh
 tox-gh==1.0.0
     # via -r requirements/tox.in
 twine==4.0.2
     # via -r requirements/dev.in
@@ -260,28 +260,28 @@
     #   twine
 urwid==2.1.2
     # via
     #   pudb
     #   urwid-readline
 urwid-readline==0.13
     # via pudb
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via
     #   -r requirements/pip.in
     #   tox
 webencodings==0.5.1
     # via bleach
 wrapt==1.15.0
     # via astroid
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==23.1.1
+pip==23.1.2
     # via -r requirements/pip.in
 setuptools==65.7.0
     # via
     #   -c requirements/pins.pip
     #   -r requirements/pip.in
     #   check-manifest
```

### Comparing `coverage-7.2.4/requirements/mypy.pip` & `coverage-7.2.5/requirements/mypy.pip`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via
     #   hypothesis
     #   pytest
 execnet==1.9.0
     # via pytest-xdist
 flaky==3.7.0
     # via -r requirements/pytest.in
-hypothesis==6.72.2
+hypothesis==6.74.1
     # via -r requirements/pytest.in
 importlib-metadata==6.6.0
     # via
     #   attrs
     #   pluggy
     #   pytest
 iniconfig==2.0.0
```

### Comparing `coverage-7.2.4/requirements/pins.pip` & `coverage-7.2.5/requirements/pins.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/requirements/pip-tools.pip` & `coverage-7.2.5/requirements/pip-tools.pip`

 * *Files 16% similar despite different names*

```diff
@@ -26,13 +26,13 @@
     # via importlib-metadata
 wheel==0.40.0
     # via pip-tools
 zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==23.1.1
+pip==23.1.2
     # via pip-tools
 setuptools==65.7.0
     # via
     #   -c requirements/pins.pip
     #   pip-tools
```

### Comparing `coverage-7.2.4/requirements/pip.pip` & `coverage-7.2.5/requirements/pip.pip`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 #
 distlib==0.3.6
     # via virtualenv
 filelock==3.12.0
     # via virtualenv
 importlib-metadata==6.6.0
     # via virtualenv
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via virtualenv
 typing-extensions==4.5.0
     # via
     #   importlib-metadata
     #   platformdirs
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via -r requirements/pip.in
 zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==23.1.1
+pip==23.1.2
     # via -r requirements/pip.in
 setuptools==65.7.0
     # via -r requirements/pip.in
```

### Comparing `coverage-7.2.4/requirements/pytest.pip` & `coverage-7.2.5/requirements/pytest.pip`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via
     #   hypothesis
     #   pytest
 execnet==1.9.0
     # via pytest-xdist
 flaky==3.7.0
     # via -r requirements/pytest.in
-hypothesis==6.72.2
+hypothesis==6.74.1
     # via -r requirements/pytest.in
 importlib-metadata==6.6.0
     # via
     #   attrs
     #   pluggy
     #   pytest
 iniconfig==2.0.0
```

### Comparing `coverage-7.2.4/requirements/tox.pip` & `coverage-7.2.5/requirements/tox.pip`

 * *Files 25% similar despite different names*

```diff
@@ -23,34 +23,34 @@
     #   pluggy
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.5.0
+tox==4.5.1
     # via
     #   -r requirements/tox.in
     #   tox-gh
 tox-gh==1.0.0
     # via -r requirements/tox.in
 typing-extensions==4.5.0
     # via
     #   importlib-metadata
     #   platformdirs
     #   tox
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `coverage-7.2.4/setup.py` & `coverage-7.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/balance_xdist_plugin.py` & `coverage-7.2.5/tests/balance_xdist_plugin.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/conftest.py` & `coverage-7.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/coveragetest.py` & `coverage-7.2.5/tests/coveragetest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/README.rst` & `coverage-7.2.5/tests/gold/README.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/annotate/white/white.py,cover` & `coverage-7.2.5/tests/gold/annotate/white/white.py,cover`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/Makefile` & `coverage-7.2.5/tests/gold/html/Makefile`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/a/a_py.html` & `coverage-7.2.5/tests/gold/html/a/a_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/a/index.html` & `coverage-7.2.5/tests/gold/html/a/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/b_branch/b_py.html` & `coverage-7.2.5/tests/gold/html/b_branch/b_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/b_branch/index.html` & `coverage-7.2.5/tests/gold/html/b_branch/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/bom/bom_py.html` & `coverage-7.2.5/tests/gold/html/bom/bom_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/bom/index.html` & `coverage-7.2.5/tests/gold/html/bom/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/contexts/index.html` & `coverage-7.2.5/tests/gold/html/contexts/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/contexts/two_tests_py.html` & `coverage-7.2.5/tests/gold/html/contexts/two_tests_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/isolatin1/index.html` & `coverage-7.2.5/tests/gold/html/isolatin1/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/isolatin1/isolatin1_py.html` & `coverage-7.2.5/tests/gold/html/isolatin1/isolatin1_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_1/index.html` & `coverage-7.2.5/tests/gold/html/omit_1/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_1/m1_py.html` & `coverage-7.2.5/tests/gold/html/omit_1/m1_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_1/m2_py.html` & `coverage-7.2.5/tests/gold/html/omit_1/m2_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_1/m3_py.html` & `coverage-7.2.5/tests/gold/html/omit_1/m3_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_1/main_py.html` & `coverage-7.2.5/tests/gold/html/omit_1/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_2/index.html` & `coverage-7.2.5/tests/gold/html/omit_2/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_2/m2_py.html` & `coverage-7.2.5/tests/gold/html/omit_2/m2_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_2/m3_py.html` & `coverage-7.2.5/tests/gold/html/omit_2/m3_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_2/main_py.html` & `coverage-7.2.5/tests/gold/html/omit_2/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_3/index.html` & `coverage-7.2.5/tests/gold/html/omit_3/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_3/m3_py.html` & `coverage-7.2.5/tests/gold/html/omit_3/m3_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_3/main_py.html` & `coverage-7.2.5/tests/gold/html/omit_3/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_4/index.html` & `coverage-7.2.5/tests/gold/html/omit_4/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_4/m1_py.html` & `coverage-7.2.5/tests/gold/html/omit_4/m1_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_4/m3_py.html` & `coverage-7.2.5/tests/gold/html/omit_4/m3_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_4/main_py.html` & `coverage-7.2.5/tests/gold/html/omit_4/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_5/index.html` & `coverage-7.2.5/tests/gold/html/omit_5/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_5/m1_py.html` & `coverage-7.2.5/tests/gold/html/omit_5/m1_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/omit_5/main_py.html` & `coverage-7.2.5/tests/gold/html/omit_5/main_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/other/blah_blah_other_py.html` & `coverage-7.2.5/tests/gold/html/other/blah_blah_other_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/other/here_py.html` & `coverage-7.2.5/tests/gold/html/other/here_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/other/index.html` & `coverage-7.2.5/tests/gold/html/other/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/partial/index.html` & `coverage-7.2.5/tests/gold/html/partial/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/partial/partial_py.html` & `coverage-7.2.5/tests/gold/html/partial/partial_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/partial_626/index.html` & `coverage-7.2.5/tests/gold/html/partial_626/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/partial_626/partial_py.html` & `coverage-7.2.5/tests/gold/html/partial_626/partial_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/styled/a_py.html` & `coverage-7.2.5/tests/gold/html/styled/a_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/styled/index.html` & `coverage-7.2.5/tests/gold/html/styled/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/styled/style.css` & `coverage-7.2.5/tests/gold/html/styled/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/support/coverage_html.js` & `coverage-7.2.5/tests/gold/html/support/coverage_html.js`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/support/favicon_32.png` & `coverage-7.2.5/tests/gold/html/support/favicon_32.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/support/keybd_closed.png` & `coverage-7.2.5/tests/gold/html/support/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/support/keybd_open.png` & `coverage-7.2.5/tests/gold/html/support/keybd_open.png`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/support/style.css` & `coverage-7.2.5/tests/gold/html/support/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/unicode/index.html` & `coverage-7.2.5/tests/gold/html/unicode/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/html/unicode/unicode_py.html` & `coverage-7.2.5/tests/gold/html/unicode/unicode_py.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/xml/x_xml/coverage.xml` & `coverage-7.2.5/tests/gold/xml/x_xml/coverage.xml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/gold/xml/y_xml_branch/coverage.xml` & `coverage-7.2.5/tests/gold/xml/y_xml_branch/coverage.xml`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/goldtest.py` & `coverage-7.2.5/tests/goldtest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/helpers.py` & `coverage-7.2.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/js/index.html` & `coverage-7.2.5/tests/js/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/js/tests.js` & `coverage-7.2.5/tests/js/tests.js`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/mixins.py` & `coverage-7.2.5/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/modules/plugins/another.py` & `coverage-7.2.5/tests/modules/plugins/another.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/modules/process_test/try_execfile.py` & `coverage-7.2.5/tests/modules/process_test/try_execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/osinfo.py` & `coverage-7.2.5/tests/osinfo.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/plugin1.py` & `coverage-7.2.5/tests/plugin1.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/plugin2.py` & `coverage-7.2.5/tests/plugin2.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/plugin_config.py` & `coverage-7.2.5/tests/plugin_config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/qunit/jquery.tmpl.min.js` & `coverage-7.2.5/tests/qunit/jquery.tmpl.min.js`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/stress_phystoken.tok` & `coverage-7.2.5/tests/stress_phystoken.tok`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/stress_phystoken_dos.tok` & `coverage-7.2.5/tests/stress_phystoken_dos.tok`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_annotate.py` & `coverage-7.2.5/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_api.py` & `coverage-7.2.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_arcs.py` & `coverage-7.2.5/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_cmdline.py` & `coverage-7.2.5/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_collector.py` & `coverage-7.2.5/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_concurrency.py` & `coverage-7.2.5/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_config.py` & `coverage-7.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_context.py` & `coverage-7.2.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_coverage.py` & `coverage-7.2.5/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_data.py` & `coverage-7.2.5/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_debug.py` & `coverage-7.2.5/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_execfile.py` & `coverage-7.2.5/tests/test_execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_filereporter.py` & `coverage-7.2.5/tests/test_filereporter.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_files.py` & `coverage-7.2.5/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_goldtest.py` & `coverage-7.2.5/tests/test_goldtest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_html.py` & `coverage-7.2.5/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_json.py` & `coverage-7.2.5/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_lcov.py` & `coverage-7.2.5/tests/test_lcov.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_misc.py` & `coverage-7.2.5/tests/test_misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # For details: https://github.com/nedbat/coveragepy/blob/master/NOTICE.txt
 
 """Tests of miscellaneous stuff."""
 
 from __future__ import annotations
 
 import sys
+from typing import Any
 from unittest import mock
 
 import pytest
 
 from coverage.exceptions import CoverageException
 from coverage.misc import file_be_gone
 from coverage.misc import Hasher, substitute_variables, import_third_party
@@ -161,7 +162,23 @@
         link = stdout_link("some text", "some url")
     assert link == "\033]8;;some url\asome text\033]8;;\a"
 
 
 def test_stdout_link_not_tty() -> None:
     # Without mocking isatty, it reports False in a pytest suite.
     assert stdout_link("some text", "some url") == "some text"
+
+
+def test_stdout_link_with_fake_stdout() -> None:
+    # If stdout is another object, we should still be ok.
+    class FakeStdout:
+        """New stdout, has .write(), but not .isatty()."""
+        def __init__(self, f: Any) -> None:
+            self.f = f
+
+        def write(self, data: str) -> Any:
+            """Write through to the underlying file."""
+            return self.f.write(data)
+
+    with mock.patch.object(sys, "stdout", FakeStdout(sys.stdout)):
+        link = stdout_link("some text", "some url")
+    assert link == "some text"
```

### Comparing `coverage-7.2.4/tests/test_mixins.py` & `coverage-7.2.5/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_numbits.py` & `coverage-7.2.5/tests/test_numbits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_oddball.py` & `coverage-7.2.5/tests/test_oddball.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_parser.py` & `coverage-7.2.5/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_phystokens.py` & `coverage-7.2.5/tests/test_phystokens.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_plugins.py` & `coverage-7.2.5/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_process.py` & `coverage-7.2.5/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_python.py` & `coverage-7.2.5/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_report.py` & `coverage-7.2.5/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_results.py` & `coverage-7.2.5/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_setup.py` & `coverage-7.2.5/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_summary.py` & `coverage-7.2.5/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_templite.py` & `coverage-7.2.5/tests/test_templite.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_testing.py` & `coverage-7.2.5/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_venv.py` & `coverage-7.2.5/tests/test_venv.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_version.py` & `coverage-7.2.5/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tests/test_xml.py` & `coverage-7.2.5/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `coverage-7.2.4/tox.ini` & `coverage-7.2.5/tox.ini`

 * *Files identical despite different names*

