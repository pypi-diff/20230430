# Comparing `tmp/tkfly-0.1.0a3.tar.gz` & `tmp/tkfly-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfly-0.1.0a3.tar", max compression
+gzip compressed data, was "tkfly-0.1.0a4.tar", max compression
```

## Comparing `tkfly-0.1.0a3.tar` & `tkfly-0.1.0a4.tar`

### file list

```diff
@@ -1,499 +1,568 @@
--rw-r--r--   0        0        0      280 2023-04-30 02:01:10.901849 tkfly-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     7415 2023-04-30 02:00:57.214361 tkfly-0.1.0a3/README.md
--rw-r--r--   0        0        0      757 2023-04-30 01:01:58.479143 tkfly-0.1.0a3/tkfly/__init__.py
--rw-r--r--   0        0        0      673 2023-04-29 10:25:40.967581 tkfly-0.1.0a3/tkfly/__main__.py
--rw-r--r--   0        0        0  1739496 2023-04-15 14:33:36.000000 tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libblend2d.dylib
--rw-r--r--   0        0        0   150336 2023-04-15 14:33:36.000000 tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libtclb2d.dylib
--rw-r--r--   0        0        0   168576 2023-04-15 14:33:36.000000 tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libtkb2d.dylib
--rw-r--r--   0        0        0    51952 2018-05-12 08:44:20.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Blacksword.otf
--rw-r--r--   0        0        0      139 2020-03-05 14:21:50.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/chessboard.png
--rw-r--r--   0        0        0    10845 2020-03-08 17:01:24.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/CMYK.png
--rw-r--r--   0        0        0     4335 2020-05-14 16:48:44.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/CompositionTest.tcl
--rw-r--r--   0        0        0     7576 2020-05-14 16:47:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/PorterDuffInAction.tcl
--rw-r--r--   0        0        0     9507 2020-03-08 17:06:24.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/RGB.png
--rw-r--r--   0        0        0     5298 2020-08-12 14:00:30.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/demo-tiger.tcl
--rw-r--r--   0        0        0   175050 2019-10-09 17:27:50.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/bl-qt-tiger.h
--rw-r--r--   0        0        0    68630 2019-09-16 05:50:56.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/Ghostscript_Tiger.svg
--rw-r--r--   0        0        0     3368 2019-10-18 06:47:24.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.cpp
--rwxr-xr-x   0        0        0   174080 2019-10-15 16:30:08.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.exe
--rw-r--r--   0        0        0   220752 2019-10-15 16:31:28.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/tiger-data.tcl
--rw-r--r--   0        0        0     3873 2020-06-23 06:06:42.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/greenSlate.jpg
--rw-r--r--   0        0        0     5415 2020-09-03 09:32:10.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/EbuttonColor-1.0.1.tm
--rw-r--r--   0        0        0     4958 2020-09-03 09:38:00.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/Eseparator-1.0.tm
--rw-r--r--   0        0        0     5965 2020-08-26 14:52:44.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/hatching-1.0.tm
--rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/IKscale-1.0.1.tm
--rw-r--r--   0        0        0    33360 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/darwin-x64/perlin.dylib
--rw-r--r--   0        0        0      513 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/license.terms
--rw-r--r--   0        0        0    11404 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x32/perlin.so
--rw-r--r--   0        0        0    12456 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x64/perlin.so
--rw-r--r--   0        0        0     1149 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/pkgIndex.tcl
--rw-r--r--   0        0        0    11776 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/win-x32/perlin.dll
--rw-r--r--   0        0        0    13312 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/win-x64/perlin.dll
--rw-r--r--   0        0        0    12189 2020-08-28 04:04:42.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/sketchline-1.0.tm
--rw-r--r--   0        0        0   125189 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/main2.tcl
--rw-r--r--   0        0        0     1052 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/pkgIndex.tcl
--rw-r--r--   0        0        0      769 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/snit2.tcl
--rw-r--r--   0        0        0      510 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/teapot.txt
--rw-r--r--   0        0        0    18959 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/validate.tcl
--rw-r--r--   0        0        0    14134 2021-12-02 19:08:46.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/Spline-1.0.tm
--rw-r--r--   0        0        0    17997 2023-03-14 07:49:04.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/moby.svg
--rw-r--r--   0        0        0    22057 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_1.svg
--rw-r--r--   0        0        0    29922 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_2.svg
--rw-r--r--   0        0        0    22020 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_3.svg
--rw-r--r--   0        0        0    23936 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_4.svg
--rw-r--r--   0        0        0    16595 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_5.svg
--rw-r--r--   0        0        0      279 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_6.svg
--rw-r--r--   0        0        0      436 2016-06-18 19:26:30.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Road_Rage-License.txt
--rw-r--r--   0        0        0   341760 2016-06-18 17:26:30.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Road_Rage.otf
--rw-r--r--   0        0        0     4861 2020-08-12 16:10:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample-poly.tcl
--rw-r--r--   0        0        0     4989 2020-08-12 13:52:06.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample-rect.tcl
--rw-r--r--   0        0        0      461 2023-04-29 15:43:17.299023 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample01.tcl
--rw-r--r--   0        0        0      443 2020-04-25 17:15:52.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample02.tcl
--rw-r--r--   0        0        0      392 2020-04-25 17:15:32.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample03.tcl
--rw-r--r--   0        0        0      754 2021-08-24 13:22:40.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample04i.tcl
--rw-r--r--   0        0        0     1660 2020-04-25 17:24:14.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample04ii.tcl
--rw-r--r--   0        0        0      579 2020-07-16 15:31:02.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample05.tcl
--rw-r--r--   0        0        0      621 2020-05-07 08:13:30.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample06.tcl
--rw-r--r--   0        0        0      718 2020-05-14 15:18:06.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample07.tcl
--rw-r--r--   0        0        0     2161 2020-05-14 15:16:08.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample101.tcl
--rw-r--r--   0        0        0     6635 2022-12-23 15:25:00.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample102.tcl
--rw-r--r--   0        0        0     2946 2020-09-02 17:00:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103.tcl
--rw-r--r--   0        0        0     3074 2021-08-24 13:03:58.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103a.tcl
--rw-r--r--   0        0        0     4231 2021-08-24 13:07:52.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103b.tcl
--rw-r--r--   0        0        0     8403 2020-09-04 06:06:22.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample104-handmadelines.tcl
--rw-r--r--   0        0        0     3006 2023-04-11 10:02:10.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample105-SVGmoby.tcl
--rw-r--r--   0        0        0     3392 2022-05-15 17:34:40.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample106.tcl
--rw-r--r--   0        0        0     2375 2022-01-03 04:49:40.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample107.tcl
--rw-r--r--   0        0        0     4366 2022-01-03 04:48:10.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample108.tcl
--rw-r--r--   0        0        0     2992 2023-04-15 16:03:48.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample109.tcl
--rw-r--r--   0        0        0     4160 2023-04-15 14:44:48.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample110.tcl
--rw-r--r--   0        0        0     3662 2023-04-15 19:37:46.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample111.tcl
--rw-r--r--   0        0        0    76248 2019-08-19 07:45:32.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/texture.jpeg
--rw-r--r--   0        0        0    85398 2023-04-15 17:26:48.000000 tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.html
--rw-r--r--   0        0        0    47336 2023-04-15 17:26:36.000000 tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.man
--rw-r--r--   0        0        0    46275 2023-04-15 17:26:50.000000 tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.wiki.txt
--rw-r--r--   0        0        0     3283 2020-06-26 04:05:56.000000 tkfly-0.1.0a3/tkfly/_blend2d/HSB.tcl
--rw-r--r--   0        0        0  1947176 2023-04-15 14:12:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libblend2d.so
--rw-r--r--   0        0        0   221592 2023-04-15 14:12:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libtclb2d.so
--rw-r--r--   0        0        0   235800 2023-04-15 14:12:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libtkb2d.so
--rw-r--r--   0        0        0     6274 2020-06-21 16:12:56.000000 tkfly-0.1.0a3/tkfly/_blend2d/Mtx.tcl
--rw-r--r--   0        0        0     1044 2023-04-08 17:37:10.000000 tkfly-0.1.0a3/tkfly/_blend2d/pkgIndex.tcl
--rw-r--r--   0        0        0     6003 2023-04-11 14:15:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/SVGpath.tcl
--rw-r--r--   0        0        0     5983 2023-04-12 14:44:44.000000 tkfly-0.1.0a3/tkfly/_blend2d/t2d.tcl
--rw-r--r--   0        0        0     7462 2023-04-15 19:35:42.000000 tkfly-0.1.0a3/tkfly/_blend2d/t2d_filters.tcl
--rw-r--r--   0        0        0     6750 2023-04-08 17:29:54.000000 tkfly-0.1.0a3/tkfly/_blend2d/t2dsvg.tcl
--rw-r--r--   0        0        0      826 2020-07-09 13:31:32.000000 tkfly-0.1.0a3/tkfly/_blend2d/tclBlend2D-license.terms
--rw-r--r--   0        0        0  1350656 2023-04-15 11:18:54.000000 tkfly-0.1.0a3/tkfly/_blend2d/win-x64/blend2d.dll
--rw-r--r--   0        0        0   138240 2023-04-15 15:25:58.000000 tkfly-0.1.0a3/tkfly/_blend2d/win-x64/tclb2d.dll
--rw-r--r--   0        0        0   146944 2023-04-15 15:25:58.000000 tkfly-0.1.0a3/tkfly/_blend2d/win-x64/tkb2d.dll
--rw-r--r--   0        0        0     1005 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/CHANGES.txt
--rw-r--r--   0        0        0   124568 2021-03-11 08:11:16.000000 tkfly-0.1.0a3/tkfly/_mupdf/demo/demo.pdf
--rw-r--r--   0        0        0     4292 2021-11-07 08:03:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/demo/demo.tcl
--rw-r--r--   0        0        0     6150 2021-11-07 08:08:52.000000 tkfly-0.1.0a3/tkfly/_mupdf/demo/demo_sharedPdf.tcl
--rw-r--r--   0        0        0    26755 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/docs/MuPDFWidget.html
--rw-r--r--   0        0        0    14092 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/docs/MuPDFWidget.man
--rw-r--r--   0        0        0      314 2021-03-11 08:27:06.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/Readme.txt
--rw-r--r--   0        0        0   125189 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/main2.tcl
--rw-r--r--   0        0        0     1052 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/pkgIndex.tcl
--rw-r--r--   0        0        0      769 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/snit2.tcl
--rw-r--r--   0        0        0      510 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/teapot.txt
--rw-r--r--   0        0        0    18959 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/validate.tcl
--rw-r--r--   0        0        0    37749 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/MuPDFWidget.tcl
--rw-r--r--   0        0        0       69 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/pkgIndex.tcl
--rw-r--r--   0        0        0      224 2023-04-19 11:06:45.090485 tkfly-0.1.0a3/tkfly/_tklib/__init__.py
--rw-r--r--   0        0        0      677 2023-04-19 11:08:58.393781 tkfly-0.1.0a3/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1667 2023-04-14 12:45:42.167394 tkfly-0.1.0a3/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7112 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/autoscroll/autoscroll.tcl
--rw-r--r--   0        0        0      611 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/autoscroll/pkgIndex.tcl
--rw-r--r--   0        0        0     7344 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_drag.tcl
--rw-r--r--   0        0        0    10374 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_epoints.tcl
--rw-r--r--   0        0        0    12828 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_epolyline.tcl
--rw-r--r--   0        0        0    11211 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_equad.tcl
--rw-r--r--   0        0        0     7467 2014-08-11 05:20:11.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_gradient.tcl
--rw-r--r--   0        0        0     2947 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_highlight.tcl
--rw-r--r--   0        0        0     9922 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_mvg.tcl
--rw-r--r--   0        0        0     2964 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_snap.tcl
--rw-r--r--   0        0        0    21321 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_sqmap.tcl
--rw-r--r--   0        0        0     1545 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_tags.tcl
--rw-r--r--   0        0        0     2195 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_trlines.tcl
--rw-r--r--   0        0        0     5161 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_zoom.tcl
--rw-r--r--   0        0        0     1295 2014-08-11 05:20:11.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/pkgIndex.tcl
--rw-r--r--   0        0        0    26671 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/chatwidget/chatwidget.tcl
--rw-r--r--   0        0        0       80 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/chatwidget/pkgIndex.tcl
--rw-r--r--   0        0        0     1365 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/bindDown.tcl
--rw-r--r--   0        0        0      381 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/controlwidget.tcl
--rw-r--r--   0        0        0     3401 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/led.tcl
--rw-r--r--   0        0        0      903 2018-05-11 03:56:07.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/pkgIndex.tcl
--rw-r--r--   0        0        0     7666 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/radioMatrix.tcl
--rw-r--r--   0        0        0    16186 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/rdial.tcl
--rw-r--r--   0        0        0    12150 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/tachometer.tcl
--rw-r--r--   0        0        0    48034 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/vertical_meter.tcl
--rw-r--r--   0        0        0    11332 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/voltmeter.tcl
--rw-r--r--   0        0        0    16207 2014-08-11 05:20:11.000000 tkfly-0.1.0a3/tkfly/_tklib/crosshair/crosshair.tcl
--rw-r--r--   0        0        0      138 2013-05-10 05:18:16.000000 tkfly-0.1.0a3/tkfly/_tklib/crosshair/pkgIndex.tcl
--rw-r--r--   0        0        0    27293 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ctext/ctext.tcl
--rw-r--r--   0        0        0       68 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ctext/pkgIndex.tcl
--rw-r--r--   0        0        0     3924 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/cursor/cursor.tcl
--rw-r--r--   0        0        0       72 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/cursor/pkgIndex.tcl
--rw-r--r--   0        0        0    12481 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/datefield/datefield.tcl
--rw-r--r--   0        0        0       76 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/datefield/pkgIndex.tcl
--rw-r--r--   0        0        0    12537 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/application.tcl
--rw-r--r--   0        0        0    10383 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/attributes.tcl
--rw-r--r--   0        0        0    37096 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/basic.tcl
--rw-r--r--   0        0        0    32433 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/core.tcl
--rw-r--r--   0        0        0     1557 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/diagram.tcl
--rw-r--r--   0        0        0     7807 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/direction.tcl
--rw-r--r--   0        0        0     7931 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/element.tcl
--rw-r--r--   0        0        0     3423 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/navigation.tcl
--rw-r--r--   0        0        0      847 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/pkgIndex.tcl
--rw-r--r--   0        0        0     4837 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/point.tcl
--rw-r--r--   0        0        0      612 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/getstring/pkgIndex.tcl
--rw-r--r--   0        0        0     4224 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/getstring/tk_getString.tcl
--rw-r--r--   0        0        0     3187 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/history/history.tcl
--rw-r--r--   0        0        0      605 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/history/pkgIndex.tcl
--rw-r--r--   0        0        0    44954 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ico/ico.tcl
--rw-r--r--   0        0        0    35176 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ico/ico0.tcl
--rw-r--r--   0        0        0      292 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ico/pkgIndex.tcl
--rw-r--r--   0        0        0    29231 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ipentry/ipentry.tcl
--rw-r--r--   0        0        0      139 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ipentry/pkgIndex.tcl
--rw-r--r--   0        0        0     3795 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/cs.msg
--rw-r--r--   0        0        0     3718 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/da.msg
--rw-r--r--   0        0        0     4409 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/de.msg
--rw-r--r--   0        0        0     3918 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/en.msg
--rw-r--r--   0        0        0     3979 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/es.msg
--rw-r--r--   0        0        0    56665 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/khim.tcl
--rw-r--r--   0        0        0      534 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/pkgIndex.tcl
--rw-r--r--   0        0        0     4124 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/pl.msg
--rw-r--r--   0        0        0     2937 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/ROOT.msg
--rw-r--r--   0        0        0     6679 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/ru.msg
--rw-r--r--   0        0        0     6361 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/uk.msg
--rw-r--r--   0        0        0      444 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/mentry.tcl
--rw-r--r--   0        0        0      737 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/mentry_tile.tcl
--rw-r--r--   0        0        0     2592 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/mentryPublic.tcl
--rw-r--r--   0        0        0      860 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/pkgIndex.tcl
--rw-r--r--   0        0        0    25858 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl
--rw-r--r--   0        0        0     4298 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl
--rw-r--r--   0        0        0     5661 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl
--rw-r--r--   0        0        0     6884 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl
--rw-r--r--   0        0        0    18737 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryThemes.tcl
--rw-r--r--   0        0        0    60325 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryWidget.tcl
--rw-r--r--   0        0        0    19506 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mwutil.tcl
--rw-r--r--   0        0        0    10636 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/tclIndex
--rw-r--r--   0        0        0     5469 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/debug.tcl
--rw-r--r--   0        0        0    53951 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/menubar.tcl
--rw-r--r--   0        0        0     3859 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/node.tcl
--rw-r--r--   0        0        0      299 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/pkgIndex.tcl
--rw-r--r--   0        0        0    26016 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/tree.tcl
--rw-r--r--   0        0        0     4015 2023-04-29 05:27:10.370187 tkfly-0.1.0a3/tkfly/_tklib/notifywindow/notifywindow.tcl
--rw-r--r--   0        0        0      548 2016-07-14 05:57:54.000000 tkfly-0.1.0a3/tkfly/_tklib/notifywindow/pkgIndex.tcl
--rw-r--r--   0        0        0   120514 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/ntext/ntext.tcl
--rw-r--r--   0        0        0      132 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/ntext/pkgIndex.tcl
--rw-r--r--   0        0        0    30859 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/persistentSelection/persistentSelection.tcl
--rw-r--r--   0        0        0      160 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/persistentSelection/pkgIndex.tcl
--rw-r--r--   0        0        0     3291 2023-04-14 12:33:32.365933 tkfly-0.1.0a3/tkfly/_tklib/pkgIndex.tcl
--rw-r--r--   0        0        0      321 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/pkgIndex.tcl
--rw-r--r--   0        0        0    13471 2015-04-21 06:10:00.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plot3d.tcl
--rw-r--r--   0        0        0    15740 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotanim.tcl
--rw-r--r--   0        0        0    12916 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotannot.tcl
--rw-r--r--   0        0        0    67951 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotaxis.tcl
--rw-r--r--   0        0        0     6478 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotbind.tcl
--rw-r--r--   0        0        0    11059 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotbusiness.tcl
--rw-r--r--   0        0        0   108162 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotchart.tcl
--rw-r--r--   0        0        0     5721 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotcombined.tcl
--rw-r--r--   0        0        0    16783 2015-04-21 06:10:00.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotconfig.tcl
--rw-r--r--   0        0        0    61163 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotcontour.tcl
--rw-r--r--   0        0        0    10041 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotgantt.tcl
--rw-r--r--   0        0        0     8895 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotobject.tcl
--rw-r--r--   0        0        0     9423 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotpack.tcl
--rw-r--r--   0        0        0   139321 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotpriv.tcl
--rw-r--r--   0        0        0     8072 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotscada.tcl
--rw-r--r--   0        0        0     5697 2016-07-14 05:57:54.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotspecial.tcl
--rw-r--r--   0        0        0     7475 2014-08-11 05:20:12.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotstatustimeline.tcl
--rw-r--r--   0        0        0     9893 2015-04-21 06:10:00.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plottable.tcl
--rw-r--r--   0        0        0     5215 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/scaling.tcl
--rw-r--r--   0        0        0    16372 2014-11-24 17:34:56.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/xyplot.tcl
--rw-r--r--   0        0        0      867 2022-07-14 16:02:02.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/pkgIndex.tcl
--rw-r--r--   0        0        0     2420 2022-08-15 11:36:06.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/attrib.tcl
--rw-r--r--   0        0        0    19506 2020-01-08 04:03:39.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/mwutil.tcl
--rw-r--r--   0        0        0    16416 2022-04-25 10:54:58.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl
--rw-r--r--   0        0        0    25675 2022-08-23 17:53:48.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/pagesman.tcl
--rw-r--r--   0        0        0    53698 2022-08-23 18:08:46.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl
--rw-r--r--   0        0        0    36010 2022-08-17 10:02:40.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl
--rw-r--r--   0        0        0    36693 2022-08-17 10:03:10.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl
--rw-r--r--   0        0        0    57949 2022-09-11 08:36:20.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl
--rw-r--r--   0        0        0    18623 2022-08-17 10:05:36.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl
--rw-r--r--   0        0        0    19056 2022-08-15 19:39:16.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/tclIndex
--rw-r--r--   0        0        0        0 2022-10-29 06:04:07.908293 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/__init__.py
--rw-r--r--   0        0        0    21894 2022-05-20 15:38:54.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl
--rw-r--r--   0        0        0      537 2022-10-19 15:21:54.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl
--rw-r--r--   0        0        0    22642 2022-05-29 18:19:18.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl
--rw-r--r--   0        0        0    51787 2022-10-22 15:11:52.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl
--rw-r--r--   0        0        0    27243 2022-04-10 15:20:18.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl
--rw-r--r--   0        0        0      686 2022-07-14 16:02:24.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutil.tcl
--rw-r--r--   0        0        0     1138 2022-07-14 16:03:16.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutil_tile.tcl
--rw-r--r--   0        0        0     3214 2022-10-18 14:23:10.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutilCommon.tcl
--rw-r--r--   0        0        0    15316 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/style/as.tcl
--rw-r--r--   0        0        0     2848 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/style/lobster.tcl
--rw-r--r--   0        0        0      684 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/style/pkgIndex.tcl
--rw-r--r--   0        0        0      765 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/style/style.tcl
--rw-r--r--   0        0        0      607 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/swaplist/pkgIndex.tcl
--rw-r--r--   0        0        0    13365 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/swaplist/swaplist.tcl
--rw-r--r--   0        0        0      898 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/pkgIndex.tcl
--rw-r--r--   0        0        0    19506 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/mwutil.tcl
--rw-r--r--   0        0        0     4286 2015-04-21 06:10:00.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/pencil.cur
--rw-r--r--   0        0        0     2911 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/repair.tcl
--rw-r--r--   0        0        0   133438 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl
--rw-r--r--   0        0        0   120387 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl
--rw-r--r--   0        0        0    93461 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl
--rw-r--r--   0        0        0   125609 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl
--rw-r--r--   0        0        0    17564 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl
--rw-r--r--   0        0        0    20512 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl
--rw-r--r--   0        0        0    68715 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl
--rw-r--r--   0        0        0   202524 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl
--rw-r--r--   0        0        0   267492 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl
--rw-r--r--   0        0        0    62720 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tclIndex
--rw-r--r--   0        0        0      488 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelist.tcl
--rw-r--r--   0        0        0      763 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelist_tile.tcl
--rw-r--r--   0        0        0     3022 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelistPublic.tcl
--rw-r--r--   0        0        0     4807 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/boxlabel.tcl
--rw-r--r--   0        0        0     7705 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/canlabel.tcl
--rw-r--r--   0        0        0     3303 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/labarray.tcl
--rw-r--r--   0        0        0     1185 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/objselec.tcl
--rw-r--r--   0        0        0     8331 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/perilabel.tcl
--rw-r--r--   0        0        0    15130 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pie.tcl
--rw-r--r--   0        0        0     1231 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pielabel.tcl
--rw-r--r--   0        0        0      154 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pkgIndex.tcl
--rw-r--r--   0        0        0     4150 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/relirect.tcl
--rw-r--r--   0        0        0     4729 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/selector.tcl
--rw-r--r--   0        0        0    13055 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/slice.tcl
--rw-r--r--   0        0        0     4728 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/tkpiechart.tcl
--rw-r--r--   0        0        0      166 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/tooltip/pkgIndex.tcl
--rw-r--r--   0        0        0     4021 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tooltip/tipstack.tcl
--rw-r--r--   0        0        0    14446 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/tooltip/tooltip.tcl
--rw-r--r--   0        0        0      427 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/pkgIndex.tcl
--rw-r--r--   0        0        0     3561 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/tclIndex
--rw-r--r--   0        0        0    14936 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbCommon.tcl
--rw-r--r--   0        0        0    11684 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbEntry.tcl
--rw-r--r--   0        0        0     2174 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbListbox.tcl
--rw-r--r--   0        0        0     3247 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl
--rw-r--r--   0        0        0     6860 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbText.tcl
--rw-r--r--   0        0        0     2701 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl
--rw-r--r--   0        0        0     1839 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/wcb.tcl
--rw-r--r--   0        0        0     3866 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/arrowb.tcl
--rw-r--r--   0        0        0    20697 2013-03-26 03:28:23.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/calendar.tcl
--rw-r--r--   0        0        0    10039 2013-03-26 03:28:23.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/dateentry.tcl
--rw-r--r--   0        0        0    14200 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/dialog.tcl
--rw-r--r--   0        0        0     9158 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/mentry.tcl
--rw-r--r--   0        0        0     6617 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/panelframe.tcl
--rw-r--r--   0        0        0     1144 2013-03-26 03:28:23.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/pkgIndex.tcl
--rw-r--r--   0        0        0    18647 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/ruler.tcl
--rw-r--r--   0        0        0     7563 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/scrollw.tcl
--rw-r--r--   0        0        0     8025 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/statusbar.tcl
--rw-r--r--   0        0        0     2093 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/stext.tcl
--rw-r--r--   0        0        0     3927 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/superframe.tcl
--rw-r--r--   0        0        0     7915 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/toolbar.tcl
--rw-r--r--   0        0        0     4374 2023-04-29 05:46:59.130164 tkfly-0.1.0a3/tkfly/_tklib/widget/widget.tcl
--rw-r--r--   0        0        0    32987 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetl/listentry.tcl
--rw-r--r--   0        0        0    18733 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetl/listsimple.tcl
--rw-r--r--   0        0        0      237 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetl/pkgIndex.tcl
--rw-r--r--   0        0        0      142 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetPlus/pkgIndex.tcl
--rw-r--r--   0        0        0    57846 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetPlus/widgetPlus.tcl
--rw-r--r--   0        0        0      146 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetv/pkgIndex.tcl
--rw-r--r--   0        0        0    12031 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetv/validator.tcl
--rw-r--r--   0        0        0      224 2023-04-29 07:23:36.893330 tkfly-0.1.0a3/tkfly/_twapi/__init__.py
--rw-r--r--   0        0        0      677 2023-04-29 07:27:32.485989 tkfly-0.1.0a3/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    35822 2021-11-07 07:09:24.000000 tkfly-0.1.0a3/tkfly/_twapi/account.tcl
--rw-r--r--   0        0        0      721 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/adsi.tcl
--rw-r--r--   0        0        0     3004 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/apputil.tcl
--rw-r--r--   0        0        0    63943 2021-11-09 02:43:04.000000 tkfly-0.1.0a3/tkfly/_twapi/base.tcl
--rw-r--r--   0        0        0     7099 2022-06-04 05:48:24.000000 tkfly-0.1.0a3/tkfly/_twapi/clipboard.tcl
--rw-r--r--   0        0        0   149879 2021-11-02 05:34:50.000000 tkfly-0.1.0a3/tkfly/_twapi/com.tcl
--rw-r--r--   0        0        0    24031 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/console.tcl
--rw-r--r--   0        0        0   118653 2022-06-03 06:01:30.000000 tkfly-0.1.0a3/tkfly/_twapi/crypto.tcl
--rw-r--r--   0        0        0    22667 2022-06-04 15:03:22.000000 tkfly-0.1.0a3/tkfly/_twapi/device.tcl
--rw-r--r--   0        0        0    51643 2020-10-09 10:08:22.000000 tkfly-0.1.0a3/tkfly/_twapi/etw.tcl
--rw-r--r--   0        0        0    14722 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/eventlog.tcl
--rw-r--r--   0        0        0    23130 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/evt.tcl
--rw-r--r--   0        0        0     7268 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/handle.tcl
--rw-r--r--   0        0        0    24383 2020-06-24 02:08:54.000000 tkfly-0.1.0a3/tkfly/_twapi/input.tcl
--rw-r--r--   0        0        0     1480 2019-07-25 11:50:02.000000 tkfly-0.1.0a3/tkfly/_twapi/LICENSE
--rw-r--r--   0        0        0    23492 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/metoo.tcl
--rw-r--r--   0        0        0    37265 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/msi.tcl
--rw-r--r--   0        0        0    22693 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/mstask.tcl
--rw-r--r--   0        0        0     1793 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/multimedia.tcl
--rw-r--r--   0        0        0     3535 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/namedpipe.tcl
--rw-r--r--   0        0        0    37061 2020-10-14 07:59:02.000000 tkfly-0.1.0a3/tkfly/_twapi/network.tcl
--rw-r--r--   0        0        0    17196 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/nls.tcl
--rw-r--r--   0        0        0    43660 2022-06-04 00:12:28.000000 tkfly-0.1.0a3/tkfly/_twapi/os.tcl
--rw-r--r--   0        0        0    34543 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/pdh.tcl
--rw-r--r--   0        0        0     7293 2022-06-22 13:03:38.000000 tkfly-0.1.0a3/tkfly/_twapi/pkgIndex.tcl
--rw-r--r--   0        0        0     3758 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/power.tcl
--rw-r--r--   0        0        0     1802 2020-06-23 03:12:46.000000 tkfly-0.1.0a3/tkfly/_twapi/printer.tcl
--rw-r--r--   0        0        0    69738 2022-06-03 07:57:36.000000 tkfly-0.1.0a3/tkfly/_twapi/process.tcl
--rw-r--r--   0        0        0     6602 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/rds.tcl
--rw-r--r--   0        0        0     2037 2022-06-22 09:04:10.000000 tkfly-0.1.0a3/tkfly/_twapi/README.md
--rw-r--r--   0        0        0    13900 2022-06-03 13:37:40.000000 tkfly-0.1.0a3/tkfly/_twapi/registry.tcl
--rw-r--r--   0        0        0    18583 2022-06-04 12:13:10.000000 tkfly-0.1.0a3/tkfly/_twapi/resource.tcl
--rw-r--r--   0        0        0    76964 2021-11-06 08:18:08.000000 tkfly-0.1.0a3/tkfly/_twapi/security.tcl
--rw-r--r--   0        0        0    40542 2022-06-04 14:46:44.000000 tkfly-0.1.0a3/tkfly/_twapi/service.tcl
--rw-r--r--   0        0        0    30062 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/share.tcl
--rw-r--r--   0        0        0    19297 2020-12-15 00:37:00.000000 tkfly-0.1.0a3/tkfly/_twapi/shell.tcl
--rw-r--r--   0        0        0    28334 2022-06-04 12:24:36.000000 tkfly-0.1.0a3/tkfly/_twapi/sspi.tcl
--rw-r--r--   0        0        0    20059 2022-06-05 01:39:28.000000 tkfly-0.1.0a3/tkfly/_twapi/storage.tcl
--rw-r--r--   0        0        0     2632 2020-07-01 00:57:00.000000 tkfly-0.1.0a3/tkfly/_twapi/synch.tcl
--rw-r--r--   0        0        0    49870 2022-06-22 10:37:46.000000 tkfly-0.1.0a3/tkfly/_twapi/tls.tcl
--rw-r--r--   0        0        0    26955 2020-06-22 09:54:26.000000 tkfly-0.1.0a3/tkfly/_twapi/twapi.tcl
--rw-r--r--   0        0        0   389718 2022-06-22 13:03:36.000000 tkfly-0.1.0a3/tkfly/_twapi/twapi_base.dll
--rw-r--r--   0        0        0   516096 2022-06-22 12:59:36.000000 tkfly-0.1.0a3/tkfly/_twapi/twapi_base64.dll
--rw-r--r--   0        0        0    42512 2022-06-04 14:52:14.000000 tkfly-0.1.0a3/tkfly/_twapi/ui.tcl
--rw-r--r--   0        0        0     4286 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/win.tcl
--rw-r--r--   0        0        0    10975 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/winlog.tcl
--rw-r--r--   0        0        0     3148 2022-06-04 03:20:02.000000 tkfly-0.1.0a3/tkfly/_twapi/winsta.tcl
--rw-r--r--   0        0        0     6978 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/wmi.tcl
--rw-r--r--   0        0        0     7757 2023-04-30 01:54:11.126193 tkfly-0.1.0a3/tkfly/blend2d/__init__.py
--rw-r--r--   0        0        0    18386 2023-04-30 01:54:11.252535 tkfly-0.1.0a3/tkfly/blend2d/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      279 2023-04-29 15:49:52.339077 tkfly-0.1.0a3/tkfly/blend2d/demos/__init__.py
--rw-r--r--   0        0        0      967 2023-04-29 15:49:52.453599 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      564 2023-04-29 15:56:22.183150 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d1.cpython-311.pyc
--rw-r--r--   0        0        0     2310 2023-04-29 16:00:46.536617 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d101.cpython-311.pyc
--rw-r--r--   0        0        0     6614 2023-04-30 01:28:39.554804 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d102.cpython-311.pyc
--rw-r--r--   0        0        0      545 2023-04-29 15:56:23.597866 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d2.cpython-311.pyc
--rw-r--r--   0        0        0      614 2023-04-29 15:50:14.121768 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d3.cpython-311.pyc
--rw-r--r--   0        0        0      982 2023-04-29 15:56:25.545873 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d4_1.cpython-311.pyc
--rw-r--r--   0        0        0     1886 2023-04-29 15:56:26.850266 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d4_2.cpython-311.pyc
--rw-r--r--   0        0        0      800 2023-04-29 15:56:28.253430 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d5.cpython-311.pyc
--rw-r--r--   0        0        0      840 2023-04-29 15:56:29.505015 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d6.cpython-311.pyc
--rw-r--r--   0        0        0      939 2023-04-29 16:00:45.037364 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d7.cpython-311.pyc
--rw-r--r--   0        0        0     4459 2023-04-30 01:29:00.414309 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/dct.cpython-311.pyc
--rw-r--r--   0        0        0     7447 2023-04-30 01:34:26.070503 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/dpda.cpython-311.pyc
--rw-r--r--   0        0        0    51952 2018-05-12 08:44:20.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Blacksword.otf
--rw-r--r--   0        0        0      139 2020-03-05 14:21:50.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/chessboard.png
--rw-r--r--   0        0        0    10845 2020-03-08 17:01:24.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/CMYK.png
--rw-r--r--   0        0        0     4335 2020-05-14 16:48:44.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/CompositionTest.tcl
--rw-r--r--   0        0        0      151 2023-04-30 01:34:16.617334 tkfly-0.1.0a3/tkfly/blend2d/demos/d.py
--rw-r--r--   0        0        0      375 2023-04-29 15:45:26.183596 tkfly-0.1.0a3/tkfly/blend2d/demos/d1.py
--rw-r--r--   0        0        0     2176 2023-04-29 15:59:15.161435 tkfly-0.1.0a3/tkfly/blend2d/demos/d101.py
--rw-r--r--   0        0        0     6639 2023-04-29 16:01:28.838141 tkfly-0.1.0a3/tkfly/blend2d/demos/d102.py
--rw-r--r--   0        0        0     4035 2023-04-30 01:41:51.892376 tkfly-0.1.0a3/tkfly/blend2d/demos/d110.py
--rw-r--r--   0        0        0      350 2023-04-29 15:46:13.786327 tkfly-0.1.0a3/tkfly/blend2d/demos/d2.py
--rw-r--r--   0        0        0      422 2023-04-29 15:47:21.757569 tkfly-0.1.0a3/tkfly/blend2d/demos/d3.py
--rw-r--r--   0        0        0      806 2023-04-29 15:52:04.223698 tkfly-0.1.0a3/tkfly/blend2d/demos/d4_1.py
--rw-r--r--   0        0        0     1733 2023-04-29 15:54:13.375735 tkfly-0.1.0a3/tkfly/blend2d/demos/d4_2.py
--rw-r--r--   0        0        0      612 2023-04-29 15:54:54.800543 tkfly-0.1.0a3/tkfly/blend2d/demos/d5.py
--rw-r--r--   0        0        0      663 2023-04-29 15:55:42.846526 tkfly-0.1.0a3/tkfly/blend2d/demos/d6.py
--rw-r--r--   0        0        0      759 2023-04-29 16:00:16.838813 tkfly-0.1.0a3/tkfly/blend2d/demos/d7.py
--rw-r--r--   0        0        0     4399 2023-04-30 01:27:49.755083 tkfly-0.1.0a3/tkfly/blend2d/demos/dct.py
--rw-r--r--   0        0        0     5298 2020-08-12 14:00:30.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/demo-tiger.tcl
--rw-r--r--   0        0        0     7474 2023-04-30 01:32:16.757048 tkfly-0.1.0a3/tkfly/blend2d/demos/dpda.py
--rw-r--r--   0        0        0     4972 2023-04-29 16:03:00.011251 tkfly-0.1.0a3/tkfly/blend2d/demos/drect.py
--rw-r--r--   0        0        0     5302 2023-04-30 01:25:21.918029 tkfly-0.1.0a3/tkfly/blend2d/demos/dtiger.py
--rw-r--r--   0        0        0     3873 2020-06-23 06:06:42.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/greenSlate.jpg
--rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/IKscale-1.0.1.tm
--rw-r--r--   0        0        0     5415 2020-09-03 09:32:10.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/EbuttonColor-1.0.1.tm
--rw-r--r--   0        0        0     4958 2020-09-03 09:38:00.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/Eseparator-1.0.tm
--rw-r--r--   0        0        0     5965 2020-08-26 14:52:44.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/hatching-1.0.tm
--rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/IKscale-1.0.1.tm
--rw-r--r--   0        0        0    33360 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/darwin-x64/perlin.dylib
--rw-r--r--   0        0        0      513 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/license.terms
--rw-r--r--   0        0        0    11404 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/linux-x32/perlin.so
--rw-r--r--   0        0        0    12456 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/linux-x64/perlin.so
--rw-r--r--   0        0        0     1149 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/pkgIndex.tcl
--rw-r--r--   0        0        0    11776 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/win-x32/perlin.dll
--rw-r--r--   0        0        0    13312 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/win-x64/perlin.dll
--rw-r--r--   0        0        0    12189 2020-08-28 04:04:42.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/sketchline-1.0.tm
--rw-r--r--   0        0        0   125189 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/main2.tcl
--rw-r--r--   0        0        0     1052 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/pkgIndex.tcl
--rw-r--r--   0        0        0      769 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/snit2.tcl
--rw-r--r--   0        0        0      510 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/teapot.txt
--rw-r--r--   0        0        0    18959 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/validate.tcl
--rw-r--r--   0        0        0    14134 2021-12-02 19:08:46.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/Spline-1.0.tm
--rw-r--r--   0        0        0    17997 2023-03-14 07:49:04.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/moby.svg
--rw-r--r--   0        0        0     7576 2020-05-14 16:47:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/PorterDuffInAction.tcl
--rw-r--r--   0        0        0    22057 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_1.svg
--rw-r--r--   0        0        0    29922 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_2.svg
--rw-r--r--   0        0        0    22020 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_3.svg
--rw-r--r--   0        0        0    23936 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_4.svg
--rw-r--r--   0        0        0    16595 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_5.svg
--rw-r--r--   0        0        0      279 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_6.svg
--rw-r--r--   0        0        0     9507 2020-03-08 17:06:24.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/RGB.png
--rw-r--r--   0        0        0      436 2016-06-18 19:26:30.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Road_Rage-License.txt
--rw-r--r--   0        0        0   341760 2016-06-18 17:26:30.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Road_Rage.otf
--rw-r--r--   0        0        0    76248 2019-08-19 07:45:32.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/texture.jpeg
--rw-r--r--   0        0        0   220752 2019-10-15 16:31:28.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/tiger-data.tcl
--rw-r--r--   0        0        0   146164 2021-05-28 11:22:28.000000 tkfly-0.1.0a3/tkfly/blend2d/HarmonyOS_Sans_Medium.ttf
--rw-r--r--   0        0        0   640122 2023-04-29 13:45:10.413812 tkfly-0.1.0a3/tkfly/blend2d/surface.bmp
--rw-r--r--   0        0        0     2217 2023-04-29 15:42:02.761477 tkfly-0.1.0a3/tkfly/core.py
--rw-r--r--   0        0        0      239 2023-04-29 23:59:46.170477 tkfly-0.1.0a3/tkfly/mupdf/__init__.py
--rw-r--r--   0        0        0      222 2023-04-14 12:59:16.512351 tkfly-0.1.0a3/tkfly/tkimg/__init__.py
--rw-r--r--   0        0        0   221710 2022-11-24 07:55:52.000000 tkfly-0.1.0a3/tkfly/tkimg/jpegtcl950.dll
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libjpegtclstub950.a
--rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libpngtclstub1638.a
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libtifftclstub440.a
--rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libtkimgstub1414.a
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libzlibtclstub1213.a
--rw-r--r--   0        0        0     6851 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/pkgIndex.tcl
--rw-r--r--   0        0        0   231950 2022-11-24 07:55:52.000000 tkfly-0.1.0a3/tkfly/tkimg/pngtcl1638.dll
--rw-r--r--   0        0        0   416782 2022-11-24 07:55:52.000000 tkfly-0.1.0a3/tkfly/tkimg/tifftcl440.dll
--rw-r--r--   0        0        0    40462 2022-11-24 07:55:54.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimg1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:54.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgbmp1414.dll
--rw-r--r--   0        0        0    22030 2022-11-24 07:55:54.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgdted1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:56.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgflir1414.dll
--rw-r--r--   0        0        0    24590 2022-11-24 07:55:56.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimggif1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:56.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgico1414.dll
--rw-r--r--   0        0        0    23054 2022-11-24 07:55:56.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgjpeg1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgpcx1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:58.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgpixmap1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgpng1414.dll
--rw-r--r--   0        0        0    25102 2022-11-24 07:56:00.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgppm1414.dll
--rw-r--r--   0        0        0    21006 2022-11-24 07:56:00.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgps1414.dll
--rw-r--r--   0        0        0    31758 2022-11-24 07:56:00.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgraw1414.dll
--rw-r--r--   0        0        0    28174 2022-11-24 07:56:02.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgsgi1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:56:02.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgsun1414.dll
--rw-r--r--   0        0        0    25102 2022-11-24 07:56:02.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgtga1414.dll
--rw-r--r--   0        0        0    70158 2022-11-24 07:56:04.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgtiff1414.dll
--rw-r--r--   0        0        0    17934 2022-11-24 07:56:04.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgwindow1414.dll
--rw-r--r--   0        0        0    19470 2022-11-24 07:56:04.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgxbm1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:56:06.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgxpm1414.dll
--rw-r--r--   0        0        0    91662 2022-11-24 07:56:06.000000 tkfly-0.1.0a3/tkfly/tkimg/zlibtcl1213.dll
--rw-r--r--   0        0        0        0 2023-04-19 11:17:10.457150 tkfly-0.1.0a3/tkfly/tklib/__init__.py
--rw-r--r--   0        0        0      141 2023-04-19 12:43:56.373512 tkfly-0.1.0a3/tkfly/tklib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2594 2023-04-29 11:00:59.295786 tkfly-0.1.0a3/tkfly/tklib/__pycache__/datefield.cpython-311.pyc
--rw-r--r--   0        0        0     8914 2023-04-29 05:02:59.020777 tkfly-0.1.0a3/tkfly/tklib/__pycache__/history.cpython-311.pyc
--rw-r--r--   0        0        0     3960 2023-04-19 12:45:43.059958 tkfly-0.1.0a3/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc
--rw-r--r--   0        0        0      538 2023-04-29 05:32:30.677805 tkfly-0.1.0a3/tkfly/tklib/autoscroll.py
--rw-r--r--   0        0        0      573 2023-04-19 14:52:50.309476 tkfly-0.1.0a3/tkfly/tklib/chatwidget.py
--rw-r--r--   0        0        0     1265 2023-04-29 10:59:14.922692 tkfly-0.1.0a3/tkfly/tklib/datefield.py
--rw-r--r--   0        0        0     5389 2023-04-29 05:02:58.918925 tkfly-0.1.0a3/tkfly/tklib/history.py
--rw-r--r--   0        0        0      583 2023-04-19 12:47:17.815625 tkfly-0.1.0a3/tkfly/tklib/menubar.py
--rw-r--r--   0        0        0     1002 2023-04-29 05:26:07.066657 tkfly-0.1.0a3/tkfly/tklib/notifywindow.py
--rw-r--r--   0        0        0     1331 2023-04-29 06:07:26.214511 tkfly-0.1.0a3/tkfly/tklib/plotchart.py
--rw-r--r--   0        0        0     5389 2023-04-29 05:38:33.820659 tkfly-0.1.0a3/tkfly/tklib/shtmlview.py
--rw-r--r--   0        0        0     2066 2023-04-19 12:45:42.877555 tkfly-0.1.0a3/tkfly/tklib/tooltip.py
--rw-r--r--   0        0        0      902 2023-04-19 11:28:27.786655 tkfly-0.1.0a3/tkfly/tklib/wcb.py
--rw-r--r--   0        0        0      523 2023-04-29 05:46:46.161323 tkfly-0.1.0a3/tkfly/tklib/widget.py
--rw-r--r--   0        0        0      506 2023-04-29 11:29:28.404486 tkfly-0.1.0a3/tkfly/tkscrollutil/__init__.py
--rw-r--r--   0        0        0      804 2023-04-29 11:29:28.606524 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1165 2023-04-29 11:09:26.181908 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc
--rw-r--r--   0        0        0     1258 2023-04-29 11:29:43.706687 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc
--rw-r--r--   0        0        0     3023 2023-04-29 11:14:55.822881 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc
--rw-r--r--   0        0        0     4204 2023-04-29 11:12:49.744284 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc
--rw-r--r--   0        0        0     3011 2023-04-29 11:29:28.610040 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc
--rw-r--r--   0        0        0     2069 2023-04-29 11:34:46.885357 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc
--rw-r--r--   0        0        0     3060 2023-04-29 11:26:17.297437 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2023-04-29 11:29:28.614038 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc
--rw-r--r--   0        0        0      413 2022-10-29 06:29:19.142527 tkfly-0.1.0a3/tkfly/tkscrollutil/attrib.py
--rw-r--r--   0        0        0      458 2023-04-29 11:29:43.603589 tkfly-0.1.0a3/tkfly/tkscrollutil/load.py
--rw-r--r--   0        0        0     1793 2023-04-29 13:55:50.749585 tkfly-0.1.0a3/tkfly/tkscrollutil/scrollableframe.py
--rw-r--r--   0        0        0     1921 2023-04-29 11:14:55.722630 tkfly-0.1.0a3/tkfly/tkscrollutil/scrollarea.py
--rw-r--r--   0        0        0     2480 2023-04-29 11:10:41.419659 tkfly-0.1.0a3/tkfly/tkscrollutil/scrollsync.py
--rw-r--r--   0        0        0     1910 2023-04-29 11:29:28.409999 tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollarea.py
--rw-r--r--   0        0        0     1142 2023-04-29 11:34:46.766705 tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollednotebook.py
--rw-r--r--   0        0        0     1689 2023-04-29 11:26:17.197236 tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollsync.py
--rw-r--r--   0        0        0     1435 2023-04-29 11:28:26.430882 tkfly-0.1.0a3/tkfly/tkscrollutil/wheelevent.py
--rw-r--r--   0        0        0      544 2023-04-29 11:43:18.104764 tkfly-0.1.0a3/tkfly/twapi/__init__.py
--rw-r--r--   0        0        0     1464 2023-04-29 11:43:18.209994 tkfly-0.1.0a3/tkfly/twapi/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      359 2023-04-29 07:58:45.679468 tkfly-0.1.0a3/tkfly/twapi/base.py
--rw-r--r--   0        0        0      230 2023-04-29 07:58:45.713014 tkfly-0.1.0a3/tkfly/twapi/msi.py
--rw-r--r--   0        0        0      704 2023-04-29 10:07:46.018924 tkfly-0.1.0a3/tkfly/twapi/ui.py
--rw-r--r--   0        0        0      585 2023-04-29 08:16:43.020235 tkfly-0.1.0a3/tkfly/twapi/win.py
--rw-r--r--   0        0        0     7660 1970-01-01 00:00:00.000000 tkfly-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0      280 2023-04-30 06:20:19.032893 tkfly-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     8620 2023-04-30 06:30:48.854637 tkfly-0.1.0a4/README.md
+-rw-r--r--   0        0        0     1008 2023-04-30 06:20:09.106247 tkfly-0.1.0a4/tkfly/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-29 10:25:40.967581 tkfly-0.1.0a4/tkfly/__main__.py
+-rw-r--r--   0        0        0  1739496 2023-04-15 14:33:36.000000 tkfly-0.1.0a4/tkfly/_blend2d/darwin-x64/libblend2d.dylib
+-rw-r--r--   0        0        0   150336 2023-04-15 14:33:36.000000 tkfly-0.1.0a4/tkfly/_blend2d/darwin-x64/libtclb2d.dylib
+-rw-r--r--   0        0        0   168576 2023-04-15 14:33:36.000000 tkfly-0.1.0a4/tkfly/_blend2d/darwin-x64/libtkb2d.dylib
+-rw-r--r--   0        0        0    51952 2018-05-12 08:44:20.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Blacksword.otf
+-rw-r--r--   0        0        0      139 2020-03-05 14:21:50.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/chessboard.png
+-rw-r--r--   0        0        0    10845 2020-03-08 17:01:24.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/CMYK.png
+-rw-r--r--   0        0        0     4335 2020-05-14 16:48:44.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/CompositionTest.tcl
+-rw-r--r--   0        0        0     7576 2020-05-14 16:47:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/PorterDuffInAction.tcl
+-rw-r--r--   0        0        0     9507 2020-03-08 17:06:24.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/RGB.png
+-rw-r--r--   0        0        0     5298 2020-08-12 14:00:30.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/demo-tiger.tcl
+-rw-r--r--   0        0        0   175050 2019-10-09 17:27:50.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/develTools/bl-qt-tiger.h
+-rw-r--r--   0        0        0    68630 2019-09-16 05:50:56.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/develTools/Ghostscript_Tiger.svg
+-rw-r--r--   0        0        0     3368 2019-10-18 06:47:24.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.cpp
+-rwxr-xr-x   0        0        0   174080 2019-10-15 16:30:08.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.exe
+-rw-r--r--   0        0        0   220752 2019-10-15 16:31:28.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/tiger-data.tcl
+-rw-r--r--   0        0        0     3873 2020-06-23 06:06:42.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/greenSlate.jpg
+-rw-r--r--   0        0        0     5415 2020-09-03 09:32:10.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/EbuttonColor-1.0.1.tm
+-rw-r--r--   0        0        0     4958 2020-09-03 09:38:00.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/Eseparator-1.0.tm
+-rw-r--r--   0        0        0     5965 2020-08-26 14:52:44.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/hatching-1.0.tm
+-rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/IKscale-1.0.1.tm
+-rw-r--r--   0        0        0    33360 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/darwin-x64/perlin.dylib
+-rw-r--r--   0        0        0      513 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/license.terms
+-rw-r--r--   0        0        0    11404 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x32/perlin.so
+-rw-r--r--   0        0        0    12456 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x64/perlin.so
+-rw-r--r--   0        0        0     1149 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/pkgIndex.tcl
+-rw-r--r--   0        0        0    11776 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/win-x32/perlin.dll
+-rw-r--r--   0        0        0    13312 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/win-x64/perlin.dll
+-rw-r--r--   0        0        0    12189 2020-08-28 04:04:42.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/sketchline-1.0.tm
+-rw-r--r--   0        0        0   125189 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/main2.tcl
+-rw-r--r--   0        0        0     1052 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/pkgIndex.tcl
+-rw-r--r--   0        0        0      769 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/snit2.tcl
+-rw-r--r--   0        0        0      510 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/teapot.txt
+-rw-r--r--   0        0        0    18959 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/validate.tcl
+-rw-r--r--   0        0        0    14134 2021-12-02 19:08:46.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/Spline-1.0.tm
+-rw-r--r--   0        0        0    17997 2023-03-14 07:49:04.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/moby.svg
+-rw-r--r--   0        0        0    22057 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_1.svg
+-rw-r--r--   0        0        0    29922 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_2.svg
+-rw-r--r--   0        0        0    22020 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_3.svg
+-rw-r--r--   0        0        0    23936 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_4.svg
+-rw-r--r--   0        0        0    16595 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_5.svg
+-rw-r--r--   0        0        0      279 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_6.svg
+-rw-r--r--   0        0        0      436 2016-06-18 19:26:30.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Road_Rage-License.txt
+-rw-r--r--   0        0        0   341760 2016-06-18 17:26:30.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/Road_Rage.otf
+-rw-r--r--   0        0        0     4861 2020-08-12 16:10:38.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample-poly.tcl
+-rw-r--r--   0        0        0     4989 2020-08-12 13:52:06.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample-rect.tcl
+-rw-r--r--   0        0        0      461 2023-04-29 15:43:17.299023 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample01.tcl
+-rw-r--r--   0        0        0      443 2020-04-25 17:15:52.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample02.tcl
+-rw-r--r--   0        0        0      392 2020-04-25 17:15:32.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample03.tcl
+-rw-r--r--   0        0        0      754 2021-08-24 13:22:40.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample04i.tcl
+-rw-r--r--   0        0        0     1660 2020-04-25 17:24:14.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample04ii.tcl
+-rw-r--r--   0        0        0      579 2020-07-16 15:31:02.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample05.tcl
+-rw-r--r--   0        0        0      621 2020-05-07 08:13:30.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample06.tcl
+-rw-r--r--   0        0        0      718 2020-05-14 15:18:06.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample07.tcl
+-rw-r--r--   0        0        0     2161 2020-05-14 15:16:08.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample101.tcl
+-rw-r--r--   0        0        0     6635 2022-12-23 15:25:00.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample102.tcl
+-rw-r--r--   0        0        0     2946 2020-09-02 17:00:12.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample103.tcl
+-rw-r--r--   0        0        0     3074 2021-08-24 13:03:58.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample103a.tcl
+-rw-r--r--   0        0        0     4231 2021-08-24 13:07:52.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample103b.tcl
+-rw-r--r--   0        0        0     8403 2020-09-04 06:06:22.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample104-handmadelines.tcl
+-rw-r--r--   0        0        0     3006 2023-04-11 10:02:10.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample105-SVGmoby.tcl
+-rw-r--r--   0        0        0     3392 2022-05-15 17:34:40.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample106.tcl
+-rw-r--r--   0        0        0     2375 2022-01-03 04:49:40.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample107.tcl
+-rw-r--r--   0        0        0     4366 2022-01-03 04:48:10.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample108.tcl
+-rw-r--r--   0        0        0     2992 2023-04-15 16:03:48.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample109.tcl
+-rw-r--r--   0        0        0     4160 2023-04-15 14:44:48.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample110.tcl
+-rw-r--r--   0        0        0     3662 2023-04-15 19:37:46.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/sample111.tcl
+-rw-r--r--   0        0        0    76248 2019-08-19 07:45:32.000000 tkfly-0.1.0a4/tkfly/_blend2d/demo/texture.jpeg
+-rw-r--r--   0        0        0    85398 2023-04-15 17:26:48.000000 tkfly-0.1.0a4/tkfly/_blend2d/docs/tclBlend2d.html
+-rw-r--r--   0        0        0    47336 2023-04-15 17:26:36.000000 tkfly-0.1.0a4/tkfly/_blend2d/docs/tclBlend2d.man
+-rw-r--r--   0        0        0    46275 2023-04-15 17:26:50.000000 tkfly-0.1.0a4/tkfly/_blend2d/docs/tclBlend2d.wiki.txt
+-rw-r--r--   0        0        0     3283 2020-06-26 04:05:56.000000 tkfly-0.1.0a4/tkfly/_blend2d/HSB.tcl
+-rw-r--r--   0        0        0  1947176 2023-04-15 14:12:12.000000 tkfly-0.1.0a4/tkfly/_blend2d/linux-x64/libblend2d.so
+-rw-r--r--   0        0        0   221592 2023-04-15 14:12:12.000000 tkfly-0.1.0a4/tkfly/_blend2d/linux-x64/libtclb2d.so
+-rw-r--r--   0        0        0   235800 2023-04-15 14:12:12.000000 tkfly-0.1.0a4/tkfly/_blend2d/linux-x64/libtkb2d.so
+-rw-r--r--   0        0        0     6274 2020-06-21 16:12:56.000000 tkfly-0.1.0a4/tkfly/_blend2d/Mtx.tcl
+-rw-r--r--   0        0        0     1044 2023-04-08 17:37:10.000000 tkfly-0.1.0a4/tkfly/_blend2d/pkgIndex.tcl
+-rw-r--r--   0        0        0     6003 2023-04-11 14:15:12.000000 tkfly-0.1.0a4/tkfly/_blend2d/SVGpath.tcl
+-rw-r--r--   0        0        0     5983 2023-04-12 14:44:44.000000 tkfly-0.1.0a4/tkfly/_blend2d/t2d.tcl
+-rw-r--r--   0        0        0     7462 2023-04-15 19:35:42.000000 tkfly-0.1.0a4/tkfly/_blend2d/t2d_filters.tcl
+-rw-r--r--   0        0        0     6750 2023-04-08 17:29:54.000000 tkfly-0.1.0a4/tkfly/_blend2d/t2dsvg.tcl
+-rw-r--r--   0        0        0      826 2020-07-09 13:31:32.000000 tkfly-0.1.0a4/tkfly/_blend2d/tclBlend2D-license.terms
+-rw-r--r--   0        0        0  1350656 2023-04-15 11:18:54.000000 tkfly-0.1.0a4/tkfly/_blend2d/win-x64/blend2d.dll
+-rw-r--r--   0        0        0   138240 2023-04-15 15:25:58.000000 tkfly-0.1.0a4/tkfly/_blend2d/win-x64/tclb2d.dll
+-rw-r--r--   0        0        0   146944 2023-04-15 15:25:58.000000 tkfly-0.1.0a4/tkfly/_blend2d/win-x64/tkb2d.dll
+-rw-r--r--   0        0        0     8776 2000-10-08 11:36:14.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Aclock.tcl
+-rw-r--r--   0        0        0     7959 2000-10-08 12:25:22.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Calendar.tcl
+-rw-r--r--   0        0        0     8431 2001-07-10 13:11:34.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Combobox.tcl
+-rw-r--r--   0        0        0      899 1999-12-27 05:50:50.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Aclock.gif
+-rw-r--r--   0        0        0      899 1999-12-27 05:51:18.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Calendar.gif
+-rw-r--r--   0        0        0      895 2000-02-10 12:05:24.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Combobox.gif
+-rw-r--r--   0        0        0      920 1999-12-27 05:56:06.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Compass.gif
+-rw-r--r--   0        0        0     1107 2000-02-08 11:05:04.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Compass32.gif
+-rw-r--r--   0        0        0      876 1999-12-27 05:48:04.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Document.gif
+-rw-r--r--   0        0        0      900 2000-02-08 09:53:10.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/File.gif
+-rw-r--r--   0        0        0      997 2000-02-08 09:56:46.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/File32.gif
+-rw-r--r--   0        0        0      894 2000-02-08 09:45:34.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Folder.gif
+-rw-r--r--   0        0        0      979 2000-02-08 09:54:42.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Folder32.gif
+-rw-r--r--   0        0        0      902 2000-02-08 14:44:18.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Gridcontrol.gif
+-rw-r--r--   0        0        0      887 2000-02-09 14:31:44.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Ibutton.gif
+-rw-r--r--   0        0        0      880 2000-02-08 10:03:56.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Iconbox.gif
+-rw-r--r--   0        0        0      862 2000-02-08 09:59:14.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Large.gif
+-rw-r--r--   0        0        0      870 2000-02-08 09:58:48.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/List.gif
+-rw-r--r--   0        0        0      888 2000-02-08 14:43:28.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Listcontrol.gif
+-rw-r--r--   0        0        0     1968 1999-12-31 07:06:12.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Llama.gif
+-rw-r--r--   0        0        0      891 2000-02-08 11:48:26.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Nodes.gif
+-rw-r--r--   0        0        0      968 1999-12-27 05:55:04.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Notebook.gif
+-rw-r--r--   0        0        0     1088 2000-02-08 11:05:32.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Notebook32.gif
+-rw-r--r--   0        0        0      896 1999-12-27 11:41:02.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Pane.gif
+-rw-r--r--   0        0        0      876 1999-12-27 05:57:28.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Progressbar.gif
+-rw-r--r--   0        0        0    13612 2000-10-01 12:15:36.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/pspbrwse.jbf
+-rw-r--r--   0        0        0      890 1999-12-27 12:29:58.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Scrollbox.gif
+-rw-r--r--   0        0        0      873 2000-02-08 09:59:36.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Small.gif
+-rw-r--r--   0        0        0      886 2000-02-10 12:02:14.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Spinentry.gif
+-rw-r--r--   0        0        0      889 1999-12-27 12:30:28.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Statusbar.gif
+-rw-r--r--   0        0        0      891 1999-12-27 12:32:48.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Tabcontrol.gif
+-rw-r--r--   0        0        0      890 1999-12-27 12:31:48.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Textframe.gif
+-rw-r--r--   0        0        0      869 1999-12-27 12:25:34.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Tinyclock.gif
+-rw-r--r--   0        0        0      882 1999-12-27 05:41:24.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Toolbar.gif
+-rw-r--r--   0        0        0      872 1999-12-27 11:53:48.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Tooltip.gif
+-rw-r--r--   0        0        0      881 2000-02-08 10:17:18.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/images/Treecontrol.gif
+-rw-r--r--   0        0        0    18569 2001-07-11 12:49:08.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/demos/metademo.tcl
+-rw-r--r--   0        0        0    23297 2001-07-11 07:46:44.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Document.tcl
+-rw-r--r--   0        0        0    35855 2001-07-11 12:47:44.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Gridcontrol.tcl
+-rw-r--r--   0        0        0     2205 2000-10-17 11:08:12.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Ibutton.tcl
+-rw-r--r--   0        0        0    39251 2000-10-25 09:45:54.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Iconbox.tcl
+-rw-r--r--   0        0        0    33462 2001-07-12 09:28:42.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Listcontrol.tcl
+-rw-r--r--   0        0        0    26895 2001-07-11 07:54:00.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/metawidget.tcl
+-rw-r--r--   0        0        0    30205 2003-07-08 13:35:52.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/mkWidgets13.htm
+-rw-r--r--   0        0        0    65292 2003-07-08 13:35:54.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/mkWidgetsCol13.htm
+-rw-r--r--   0        0        0    10122 2001-07-08 05:58:14.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Pane.tcl
+-rw-r--r--   0        0        0     1018 2001-07-11 12:36:48.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/pkgIndex.tcl
+-rw-r--r--   0        0        0     3193 2000-10-25 13:42:14.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Progressbar.tcl
+-rw-r--r--   0        0        0      237 2000-03-26 13:12:28.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/ReadMe.txt
+-rw-r--r--   0        0        0     6133 2000-10-25 14:02:00.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Scrollbox.tcl
+-rw-r--r--   0        0        0     3872 2000-10-26 12:39:18.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Spinentry.tcl
+-rw-r--r--   0        0        0     6365 2000-10-26 13:09:12.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Statusbar.tcl
+-rw-r--r--   0        0        0    12759 2001-07-08 06:42:04.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Tabcontrol.tcl
+-rw-r--r--   0        0        0     3693 2000-10-26 13:54:28.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Textframe.tcl
+-rw-r--r--   0        0        0    13012 2001-07-06 16:07:24.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Toolbar.tcl
+-rw-r--r--   0        0        0     4221 2000-03-20 12:51:28.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Tooltip.tcl
+-rw-r--r--   0        0        0    35987 2001-07-06 16:09:24.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Treecontrol.tcl
+-rw-r--r--   0        0        0     3744 2001-07-11 12:36:34.000000 tkfly-0.1.0a4/tkfly/_mkwidgets/Window.tcl
+-rw-r--r--   0        0        0     1005 2021-11-07 07:32:30.000000 tkfly-0.1.0a4/tkfly/_mupdf/CHANGES.txt
+-rw-r--r--   0        0        0   124568 2021-03-11 08:11:16.000000 tkfly-0.1.0a4/tkfly/_mupdf/demo/demo.pdf
+-rw-r--r--   0        0        0     4292 2021-11-07 08:03:30.000000 tkfly-0.1.0a4/tkfly/_mupdf/demo/demo.tcl
+-rw-r--r--   0        0        0     6150 2021-11-07 08:08:52.000000 tkfly-0.1.0a4/tkfly/_mupdf/demo/demo_sharedPdf.tcl
+-rw-r--r--   0        0        0    26755 2021-11-07 07:32:30.000000 tkfly-0.1.0a4/tkfly/_mupdf/docs/MuPDFWidget.html
+-rw-r--r--   0        0        0    14092 2021-11-07 07:32:30.000000 tkfly-0.1.0a4/tkfly/_mupdf/docs/MuPDFWidget.man
+-rw-r--r--   0        0        0      314 2021-03-11 08:27:06.000000 tkfly-0.1.0a4/tkfly/_mupdf/lib/Readme.txt
+-rw-r--r--   0        0        0   125189 2012-03-30 13:55:46.000000 tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/main2.tcl
+-rw-r--r--   0        0        0     1052 2012-03-30 13:55:46.000000 tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/pkgIndex.tcl
+-rw-r--r--   0        0        0      769 2012-03-30 13:55:46.000000 tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/snit2.tcl
+-rw-r--r--   0        0        0      510 2012-03-30 13:55:46.000000 tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/teapot.txt
+-rw-r--r--   0        0        0    18959 2012-03-30 13:55:46.000000 tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/validate.tcl
+-rw-r--r--   0        0        0    37749 2021-11-07 07:32:30.000000 tkfly-0.1.0a4/tkfly/_mupdf/MuPDFWidget.tcl
+-rw-r--r--   0        0        0       69 2021-11-07 07:32:30.000000 tkfly-0.1.0a4/tkfly/_mupdf/pkgIndex.tcl
+-rw-r--r--   0        0        0      224 2023-04-19 11:06:45.090485 tkfly-0.1.0a4/tkfly/_tklib/__init__.py
+-rw-r--r--   0        0        0      677 2023-04-19 11:08:58.393781 tkfly-0.1.0a4/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1667 2023-04-14 12:45:42.167394 tkfly-0.1.0a4/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7112 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/autoscroll/autoscroll.tcl
+-rw-r--r--   0        0        0      611 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/autoscroll/pkgIndex.tcl
+-rw-r--r--   0        0        0     7344 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_drag.tcl
+-rw-r--r--   0        0        0    10374 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_epoints.tcl
+-rw-r--r--   0        0        0    12828 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_epolyline.tcl
+-rw-r--r--   0        0        0    11211 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_equad.tcl
+-rw-r--r--   0        0        0     7467 2014-08-11 05:20:11.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_gradient.tcl
+-rw-r--r--   0        0        0     2947 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_highlight.tcl
+-rw-r--r--   0        0        0     9922 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_mvg.tcl
+-rw-r--r--   0        0        0     2964 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_snap.tcl
+-rw-r--r--   0        0        0    21321 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_sqmap.tcl
+-rw-r--r--   0        0        0     1545 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_tags.tcl
+-rw-r--r--   0        0        0     2195 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_trlines.tcl
+-rw-r--r--   0        0        0     5161 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_zoom.tcl
+-rw-r--r--   0        0        0     1295 2014-08-11 05:20:11.000000 tkfly-0.1.0a4/tkfly/_tklib/canvas/pkgIndex.tcl
+-rw-r--r--   0        0        0    26671 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/chatwidget/chatwidget.tcl
+-rw-r--r--   0        0        0       80 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/chatwidget/pkgIndex.tcl
+-rw-r--r--   0        0        0     1365 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/bindDown.tcl
+-rw-r--r--   0        0        0      381 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/controlwidget.tcl
+-rw-r--r--   0        0        0     3401 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/led.tcl
+-rw-r--r--   0        0        0      903 2018-05-11 03:56:07.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/pkgIndex.tcl
+-rw-r--r--   0        0        0     7666 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/radioMatrix.tcl
+-rw-r--r--   0        0        0    16186 2018-05-11 03:56:08.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/rdial.tcl
+-rw-r--r--   0        0        0    12150 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/tachometer.tcl
+-rw-r--r--   0        0        0    48034 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/vertical_meter.tcl
+-rw-r--r--   0        0        0    11332 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/controlwidget/voltmeter.tcl
+-rw-r--r--   0        0        0    16207 2014-08-11 05:20:11.000000 tkfly-0.1.0a4/tkfly/_tklib/crosshair/crosshair.tcl
+-rw-r--r--   0        0        0      138 2013-05-10 05:18:16.000000 tkfly-0.1.0a4/tkfly/_tklib/crosshair/pkgIndex.tcl
+-rw-r--r--   0        0        0    27293 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/ctext/ctext.tcl
+-rw-r--r--   0        0        0       68 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/ctext/pkgIndex.tcl
+-rw-r--r--   0        0        0     3924 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/cursor/cursor.tcl
+-rw-r--r--   0        0        0       72 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/cursor/pkgIndex.tcl
+-rw-r--r--   0        0        0    12481 2020-01-06 23:27:53.000000 tkfly-0.1.0a4/tkfly/_tklib/datefield/datefield.tcl
+-rw-r--r--   0        0        0       76 2020-01-06 23:27:53.000000 tkfly-0.1.0a4/tkfly/_tklib/datefield/pkgIndex.tcl
+-rw-r--r--   0        0        0    12537 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/application.tcl
+-rw-r--r--   0        0        0    10383 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/attributes.tcl
+-rw-r--r--   0        0        0    37096 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/basic.tcl
+-rw-r--r--   0        0        0    32433 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/core.tcl
+-rw-r--r--   0        0        0     1557 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/diagram.tcl
+-rw-r--r--   0        0        0     7807 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/direction.tcl
+-rw-r--r--   0        0        0     7931 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/element.tcl
+-rw-r--r--   0        0        0     3423 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/navigation.tcl
+-rw-r--r--   0        0        0      847 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/pkgIndex.tcl
+-rw-r--r--   0        0        0     4837 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/diagrams/point.tcl
+-rw-r--r--   0        0        0      612 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/getstring/pkgIndex.tcl
+-rw-r--r--   0        0        0     4224 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/getstring/tk_getString.tcl
+-rw-r--r--   0        0        0     3187 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/history/history.tcl
+-rw-r--r--   0        0        0      605 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/history/pkgIndex.tcl
+-rw-r--r--   0        0        0    44954 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/ico/ico.tcl
+-rw-r--r--   0        0        0    35176 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/ico/ico0.tcl
+-rw-r--r--   0        0        0      292 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/ico/pkgIndex.tcl
+-rw-r--r--   0        0        0    29231 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/ipentry/ipentry.tcl
+-rw-r--r--   0        0        0      139 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/ipentry/pkgIndex.tcl
+-rw-r--r--   0        0        0     3795 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/cs.msg
+-rw-r--r--   0        0        0     3718 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/da.msg
+-rw-r--r--   0        0        0     4409 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/de.msg
+-rw-r--r--   0        0        0     3918 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/en.msg
+-rw-r--r--   0        0        0     3979 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/es.msg
+-rw-r--r--   0        0        0    56665 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/khim.tcl
+-rw-r--r--   0        0        0      534 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/pkgIndex.tcl
+-rw-r--r--   0        0        0     4124 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/pl.msg
+-rw-r--r--   0        0        0     2937 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/ROOT.msg
+-rw-r--r--   0        0        0     6679 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/ru.msg
+-rw-r--r--   0        0        0     6361 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/khim/uk.msg
+-rw-r--r--   0        0        0      444 2020-01-06 23:27:53.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/mentry.tcl
+-rw-r--r--   0        0        0      737 2020-01-06 23:27:53.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/mentry_tile.tcl
+-rw-r--r--   0        0        0     2592 2020-01-06 23:27:53.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/mentryPublic.tcl
+-rw-r--r--   0        0        0      860 2020-01-06 23:27:53.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/pkgIndex.tcl
+-rw-r--r--   0        0        0    25858 2019-08-21 18:42:16.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl
+-rw-r--r--   0        0        0     4298 2019-08-21 18:42:16.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl
+-rw-r--r--   0        0        0     5661 2019-08-21 18:42:16.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl
+-rw-r--r--   0        0        0     6884 2019-08-21 18:42:16.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl
+-rw-r--r--   0        0        0    18737 2019-08-21 18:42:16.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryThemes.tcl
+-rw-r--r--   0        0        0    60325 2019-08-21 18:42:16.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryWidget.tcl
+-rw-r--r--   0        0        0    19506 2020-01-06 23:27:53.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mwutil.tcl
+-rw-r--r--   0        0        0    10636 2020-01-06 23:27:53.000000 tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/tclIndex
+-rw-r--r--   0        0        0     5469 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/menubar/debug.tcl
+-rw-r--r--   0        0        0    53951 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/menubar/menubar.tcl
+-rw-r--r--   0        0        0     3859 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/menubar/node.tcl
+-rw-r--r--   0        0        0      299 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/menubar/pkgIndex.tcl
+-rw-r--r--   0        0        0    26016 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/menubar/tree.tcl
+-rw-r--r--   0        0        0     4015 2023-04-29 05:27:10.370187 tkfly-0.1.0a4/tkfly/_tklib/notifywindow/notifywindow.tcl
+-rw-r--r--   0        0        0      548 2016-07-14 05:57:54.000000 tkfly-0.1.0a4/tkfly/_tklib/notifywindow/pkgIndex.tcl
+-rw-r--r--   0        0        0   120514 2018-05-11 03:56:08.000000 tkfly-0.1.0a4/tkfly/_tklib/ntext/ntext.tcl
+-rw-r--r--   0        0        0      132 2020-02-09 20:50:00.000000 tkfly-0.1.0a4/tkfly/_tklib/ntext/pkgIndex.tcl
+-rw-r--r--   0        0        0    30859 2020-02-09 20:50:00.000000 tkfly-0.1.0a4/tkfly/_tklib/persistentSelection/persistentSelection.tcl
+-rw-r--r--   0        0        0      160 2020-02-09 20:50:00.000000 tkfly-0.1.0a4/tkfly/_tklib/persistentSelection/pkgIndex.tcl
+-rw-r--r--   0        0        0     3291 2023-04-14 12:33:32.365933 tkfly-0.1.0a4/tkfly/_tklib/pkgIndex.tcl
+-rw-r--r--   0        0        0      321 2018-05-11 03:56:08.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/pkgIndex.tcl
+-rw-r--r--   0        0        0    13471 2015-04-21 06:10:00.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plot3d.tcl
+-rw-r--r--   0        0        0    15740 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotanim.tcl
+-rw-r--r--   0        0        0    12916 2018-05-11 03:56:08.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotannot.tcl
+-rw-r--r--   0        0        0    67951 2018-05-11 03:56:08.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotaxis.tcl
+-rw-r--r--   0        0        0     6478 2019-08-21 18:42:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotbind.tcl
+-rw-r--r--   0        0        0    11059 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotbusiness.tcl
+-rw-r--r--   0        0        0   108162 2019-08-21 18:42:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotchart.tcl
+-rw-r--r--   0        0        0     5721 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotcombined.tcl
+-rw-r--r--   0        0        0    16783 2015-04-21 06:10:00.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotconfig.tcl
+-rw-r--r--   0        0        0    61163 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotcontour.tcl
+-rw-r--r--   0        0        0    10041 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotgantt.tcl
+-rw-r--r--   0        0        0     8895 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotobject.tcl
+-rw-r--r--   0        0        0     9423 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotpack.tcl
+-rw-r--r--   0        0        0   139321 2018-05-11 03:56:08.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotpriv.tcl
+-rw-r--r--   0        0        0     8072 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotscada.tcl
+-rw-r--r--   0        0        0     5697 2016-07-14 05:57:54.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotspecial.tcl
+-rw-r--r--   0        0        0     7475 2014-08-11 05:20:12.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotstatustimeline.tcl
+-rw-r--r--   0        0        0     9893 2015-04-21 06:10:00.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/plottable.tcl
+-rw-r--r--   0        0        0     5215 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/scaling.tcl
+-rw-r--r--   0        0        0    16372 2014-11-24 17:34:56.000000 tkfly-0.1.0a4/tkfly/_tklib/plotchart/xyplot.tcl
+-rw-r--r--   0        0        0      867 2022-07-14 16:02:02.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/pkgIndex.tcl
+-rw-r--r--   0        0        0     2420 2022-08-15 11:36:06.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/attrib.tcl
+-rw-r--r--   0        0        0    19506 2020-01-08 04:03:39.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/mwutil.tcl
+-rw-r--r--   0        0        0    16416 2022-04-25 10:54:58.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl
+-rw-r--r--   0        0        0    25675 2022-08-23 17:53:48.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/pagesman.tcl
+-rw-r--r--   0        0        0    53698 2022-08-23 18:08:46.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl
+-rw-r--r--   0        0        0    36010 2022-08-17 10:02:40.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl
+-rw-r--r--   0        0        0    36693 2022-08-17 10:03:10.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl
+-rw-r--r--   0        0        0    57949 2022-09-11 08:36:20.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl
+-rw-r--r--   0        0        0    18623 2022-08-17 10:05:36.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl
+-rw-r--r--   0        0        0    19056 2022-08-15 19:39:16.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/tclIndex
+-rw-r--r--   0        0        0        0 2022-10-29 06:04:07.908293 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/__init__.py
+-rw-r--r--   0        0        0    21894 2022-05-20 15:38:54.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl
+-rw-r--r--   0        0        0      537 2022-10-19 15:21:54.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl
+-rw-r--r--   0        0        0    22642 2022-05-29 18:19:18.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl
+-rw-r--r--   0        0        0    51787 2022-10-22 15:11:52.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl
+-rw-r--r--   0        0        0    27243 2022-04-10 15:20:18.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl
+-rw-r--r--   0        0        0      686 2022-07-14 16:02:24.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scrollutil.tcl
+-rw-r--r--   0        0        0     1138 2022-07-14 16:03:16.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scrollutil_tile.tcl
+-rw-r--r--   0        0        0     3214 2022-10-18 14:23:10.000000 tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scrollutilCommon.tcl
+-rw-r--r--   0        0        0    15316 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/style/as.tcl
+-rw-r--r--   0        0        0     2848 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/style/lobster.tcl
+-rw-r--r--   0        0        0      684 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/style/pkgIndex.tcl
+-rw-r--r--   0        0        0      765 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/style/style.tcl
+-rw-r--r--   0        0        0      607 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/swaplist/pkgIndex.tcl
+-rw-r--r--   0        0        0    13365 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/swaplist/swaplist.tcl
+-rw-r--r--   0        0        0      898 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/pkgIndex.tcl
+-rw-r--r--   0        0        0    19506 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/mwutil.tcl
+-rw-r--r--   0        0        0     4286 2015-04-21 06:10:00.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/pencil.cur
+-rw-r--r--   0        0        0     2911 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/repair.tcl
+-rw-r--r--   0        0        0   133438 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl
+-rw-r--r--   0        0        0   120387 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl
+-rw-r--r--   0        0        0    93461 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl
+-rw-r--r--   0        0        0   125609 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl
+-rw-r--r--   0        0        0    17564 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl
+-rw-r--r--   0        0        0    20512 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl
+-rw-r--r--   0        0        0    68715 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl
+-rw-r--r--   0        0        0   202524 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl
+-rw-r--r--   0        0        0   267492 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl
+-rw-r--r--   0        0        0    62720 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tclIndex
+-rw-r--r--   0        0        0      488 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/tablelist.tcl
+-rw-r--r--   0        0        0      763 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/tablelist_tile.tcl
+-rw-r--r--   0        0        0     3022 2020-01-06 23:27:54.000000 tkfly-0.1.0a4/tkfly/_tklib/tablelist/tablelistPublic.tcl
+-rw-r--r--   0        0        0     4807 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/boxlabel.tcl
+-rw-r--r--   0        0        0     7705 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/canlabel.tcl
+-rw-r--r--   0        0        0     3303 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/labarray.tcl
+-rw-r--r--   0        0        0     1185 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/objselec.tcl
+-rw-r--r--   0        0        0     8331 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/perilabel.tcl
+-rw-r--r--   0        0        0    15130 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/pie.tcl
+-rw-r--r--   0        0        0     1231 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/pielabel.tcl
+-rw-r--r--   0        0        0      154 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/pkgIndex.tcl
+-rw-r--r--   0        0        0     4150 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/relirect.tcl
+-rw-r--r--   0        0        0     4729 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/selector.tcl
+-rw-r--r--   0        0        0    13055 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/slice.tcl
+-rw-r--r--   0        0        0     4728 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/tkpiechart.tcl
+-rw-r--r--   0        0        0      166 2018-05-11 03:56:08.000000 tkfly-0.1.0a4/tkfly/_tklib/tooltip/pkgIndex.tcl
+-rw-r--r--   0        0        0     4021 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/tooltip/tipstack.tcl
+-rw-r--r--   0        0        0    14446 2018-05-11 03:56:08.000000 tkfly-0.1.0a4/tkfly/_tklib/tooltip/tooltip.tcl
+-rw-r--r--   0        0        0      427 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/pkgIndex.tcl
+-rw-r--r--   0        0        0     3561 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/tclIndex
+-rw-r--r--   0        0        0    14936 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbCommon.tcl
+-rw-r--r--   0        0        0    11684 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbEntry.tcl
+-rw-r--r--   0        0        0     2174 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbListbox.tcl
+-rw-r--r--   0        0        0     3247 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl
+-rw-r--r--   0        0        0     6860 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbText.tcl
+-rw-r--r--   0        0        0     2701 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl
+-rw-r--r--   0        0        0     1839 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/wcb/wcb.tcl
+-rw-r--r--   0        0        0     3866 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/arrowb.tcl
+-rw-r--r--   0        0        0    20697 2013-03-26 03:28:23.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/calendar.tcl
+-rw-r--r--   0        0        0    10039 2013-03-26 03:28:23.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/dateentry.tcl
+-rw-r--r--   0        0        0    14200 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/dialog.tcl
+-rw-r--r--   0        0        0     9158 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/mentry.tcl
+-rw-r--r--   0        0        0     6617 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/panelframe.tcl
+-rw-r--r--   0        0        0     1144 2013-03-26 03:28:23.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/pkgIndex.tcl
+-rw-r--r--   0        0        0    18647 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/ruler.tcl
+-rw-r--r--   0        0        0     7563 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/scrollw.tcl
+-rw-r--r--   0        0        0     8025 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/statusbar.tcl
+-rw-r--r--   0        0        0     2093 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/stext.tcl
+-rw-r--r--   0        0        0     3927 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/superframe.tcl
+-rw-r--r--   0        0        0     7915 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widget/toolbar.tcl
+-rw-r--r--   0        0        0     4374 2023-04-29 05:46:59.130164 tkfly-0.1.0a4/tkfly/_tklib/widget/widget.tcl
+-rw-r--r--   0        0        0    32987 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/widgetl/listentry.tcl
+-rw-r--r--   0        0        0    18733 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/widgetl/listsimple.tcl
+-rw-r--r--   0        0        0      237 2019-08-21 18:42:17.000000 tkfly-0.1.0a4/tkfly/_tklib/widgetl/pkgIndex.tcl
+-rw-r--r--   0        0        0      142 2020-02-09 20:50:00.000000 tkfly-0.1.0a4/tkfly/_tklib/widgetPlus/pkgIndex.tcl
+-rw-r--r--   0        0        0    57846 2020-02-09 20:50:00.000000 tkfly-0.1.0a4/tkfly/_tklib/widgetPlus/widgetPlus.tcl
+-rw-r--r--   0        0        0      146 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widgetv/pkgIndex.tcl
+-rw-r--r--   0        0        0    12031 2013-02-14 03:37:16.000000 tkfly-0.1.0a4/tkfly/_tklib/widgetv/validator.tcl
+-rw-r--r--   0        0        0      224 2023-04-29 07:23:36.893330 tkfly-0.1.0a4/tkfly/_twapi/__init__.py
+-rw-r--r--   0        0        0      677 2023-04-29 07:27:32.485989 tkfly-0.1.0a4/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    35822 2021-11-07 07:09:24.000000 tkfly-0.1.0a4/tkfly/_twapi/account.tcl
+-rw-r--r--   0        0        0      721 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/adsi.tcl
+-rw-r--r--   0        0        0     3004 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/apputil.tcl
+-rw-r--r--   0        0        0    63943 2021-11-09 02:43:04.000000 tkfly-0.1.0a4/tkfly/_twapi/base.tcl
+-rw-r--r--   0        0        0     7099 2022-06-04 05:48:24.000000 tkfly-0.1.0a4/tkfly/_twapi/clipboard.tcl
+-rw-r--r--   0        0        0   149879 2021-11-02 05:34:50.000000 tkfly-0.1.0a4/tkfly/_twapi/com.tcl
+-rw-r--r--   0        0        0    24031 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/console.tcl
+-rw-r--r--   0        0        0   118653 2022-06-03 06:01:30.000000 tkfly-0.1.0a4/tkfly/_twapi/crypto.tcl
+-rw-r--r--   0        0        0    22667 2022-06-04 15:03:22.000000 tkfly-0.1.0a4/tkfly/_twapi/device.tcl
+-rw-r--r--   0        0        0    51643 2020-10-09 10:08:22.000000 tkfly-0.1.0a4/tkfly/_twapi/etw.tcl
+-rw-r--r--   0        0        0    14722 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/eventlog.tcl
+-rw-r--r--   0        0        0    23130 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/evt.tcl
+-rw-r--r--   0        0        0     7268 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/handle.tcl
+-rw-r--r--   0        0        0    24383 2020-06-24 02:08:54.000000 tkfly-0.1.0a4/tkfly/_twapi/input.tcl
+-rw-r--r--   0        0        0     1480 2019-07-25 11:50:02.000000 tkfly-0.1.0a4/tkfly/_twapi/LICENSE
+-rw-r--r--   0        0        0    23492 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/metoo.tcl
+-rw-r--r--   0        0        0    37265 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/msi.tcl
+-rw-r--r--   0        0        0    22693 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/mstask.tcl
+-rw-r--r--   0        0        0     1793 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/multimedia.tcl
+-rw-r--r--   0        0        0     3535 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/namedpipe.tcl
+-rw-r--r--   0        0        0    37061 2020-10-14 07:59:02.000000 tkfly-0.1.0a4/tkfly/_twapi/network.tcl
+-rw-r--r--   0        0        0    17196 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/nls.tcl
+-rw-r--r--   0        0        0    43660 2022-06-04 00:12:28.000000 tkfly-0.1.0a4/tkfly/_twapi/os.tcl
+-rw-r--r--   0        0        0    34543 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/pdh.tcl
+-rw-r--r--   0        0        0     7293 2022-06-22 13:03:38.000000 tkfly-0.1.0a4/tkfly/_twapi/pkgIndex.tcl
+-rw-r--r--   0        0        0     3758 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/power.tcl
+-rw-r--r--   0        0        0     1802 2020-06-23 03:12:46.000000 tkfly-0.1.0a4/tkfly/_twapi/printer.tcl
+-rw-r--r--   0        0        0    69738 2022-06-03 07:57:36.000000 tkfly-0.1.0a4/tkfly/_twapi/process.tcl
+-rw-r--r--   0        0        0     6602 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/rds.tcl
+-rw-r--r--   0        0        0     2037 2022-06-22 09:04:10.000000 tkfly-0.1.0a4/tkfly/_twapi/README.md
+-rw-r--r--   0        0        0    13900 2022-06-03 13:37:40.000000 tkfly-0.1.0a4/tkfly/_twapi/registry.tcl
+-rw-r--r--   0        0        0    18583 2022-06-04 12:13:10.000000 tkfly-0.1.0a4/tkfly/_twapi/resource.tcl
+-rw-r--r--   0        0        0    76964 2021-11-06 08:18:08.000000 tkfly-0.1.0a4/tkfly/_twapi/security.tcl
+-rw-r--r--   0        0        0    40542 2022-06-04 14:46:44.000000 tkfly-0.1.0a4/tkfly/_twapi/service.tcl
+-rw-r--r--   0        0        0    30062 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/share.tcl
+-rw-r--r--   0        0        0    19297 2020-12-15 00:37:00.000000 tkfly-0.1.0a4/tkfly/_twapi/shell.tcl
+-rw-r--r--   0        0        0    28334 2022-06-04 12:24:36.000000 tkfly-0.1.0a4/tkfly/_twapi/sspi.tcl
+-rw-r--r--   0        0        0    20059 2022-06-05 01:39:28.000000 tkfly-0.1.0a4/tkfly/_twapi/storage.tcl
+-rw-r--r--   0        0        0     2632 2020-07-01 00:57:00.000000 tkfly-0.1.0a4/tkfly/_twapi/synch.tcl
+-rw-r--r--   0        0        0    49870 2022-06-22 10:37:46.000000 tkfly-0.1.0a4/tkfly/_twapi/tls.tcl
+-rw-r--r--   0        0        0    26955 2020-06-22 09:54:26.000000 tkfly-0.1.0a4/tkfly/_twapi/twapi.tcl
+-rw-r--r--   0        0        0   389718 2022-06-22 13:03:36.000000 tkfly-0.1.0a4/tkfly/_twapi/twapi_base.dll
+-rw-r--r--   0        0        0   516096 2022-06-22 12:59:36.000000 tkfly-0.1.0a4/tkfly/_twapi/twapi_base64.dll
+-rw-r--r--   0        0        0    42512 2022-06-04 14:52:14.000000 tkfly-0.1.0a4/tkfly/_twapi/ui.tcl
+-rw-r--r--   0        0        0     4286 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/win.tcl
+-rw-r--r--   0        0        0    10975 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/winlog.tcl
+-rw-r--r--   0        0        0     3148 2022-06-04 03:20:02.000000 tkfly-0.1.0a4/tkfly/_twapi/winsta.tcl
+-rw-r--r--   0        0        0     6978 2019-07-25 11:50:04.000000 tkfly-0.1.0a4/tkfly/_twapi/wmi.tcl
+-rw-r--r--   0        0        0     8486 2023-04-30 03:30:14.017782 tkfly-0.1.0a4/tkfly/blend2d/__init__.py
+-rw-r--r--   0        0        0    20274 2023-04-30 03:30:14.148768 tkfly-0.1.0a4/tkfly/blend2d/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      279 2023-04-29 15:49:52.339077 tkfly-0.1.0a4/tkfly/blend2d/demos/__init__.py
+-rw-r--r--   0        0        0      967 2023-04-29 15:49:52.453599 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      564 2023-04-29 15:56:22.183150 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d1.cpython-311.pyc
+-rw-r--r--   0        0        0     2310 2023-04-29 16:00:46.536617 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d101.cpython-311.pyc
+-rw-r--r--   0        0        0     6614 2023-04-30 01:28:39.554804 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d102.cpython-311.pyc
+-rw-r--r--   0        0        0      545 2023-04-29 15:56:23.597866 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d2.cpython-311.pyc
+-rw-r--r--   0        0        0      614 2023-04-29 15:50:14.121768 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d3.cpython-311.pyc
+-rw-r--r--   0        0        0      982 2023-04-29 15:56:25.545873 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d4_1.cpython-311.pyc
+-rw-r--r--   0        0        0     1886 2023-04-29 15:56:26.850266 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d4_2.cpython-311.pyc
+-rw-r--r--   0        0        0      800 2023-04-29 15:56:28.253430 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d5.cpython-311.pyc
+-rw-r--r--   0        0        0      840 2023-04-29 15:56:29.505015 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d6.cpython-311.pyc
+-rw-r--r--   0        0        0      939 2023-04-29 16:00:45.037364 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d7.cpython-311.pyc
+-rw-r--r--   0        0        0     4459 2023-04-30 01:29:00.414309 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/dct.cpython-311.pyc
+-rw-r--r--   0        0        0     7447 2023-04-30 01:34:26.070503 tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/dpda.cpython-311.pyc
+-rw-r--r--   0        0        0    51952 2018-05-12 08:44:20.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Blacksword.otf
+-rw-r--r--   0        0        0      139 2020-03-05 14:21:50.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/chessboard.png
+-rw-r--r--   0        0        0    10845 2020-03-08 17:01:24.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/CMYK.png
+-rw-r--r--   0        0        0     4335 2020-05-14 16:48:44.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/CompositionTest.tcl
+-rw-r--r--   0        0        0      151 2023-04-30 01:34:16.617334 tkfly-0.1.0a4/tkfly/blend2d/demos/d.py
+-rw-r--r--   0        0        0      375 2023-04-29 15:45:26.183596 tkfly-0.1.0a4/tkfly/blend2d/demos/d1.py
+-rw-r--r--   0        0        0     2176 2023-04-29 15:59:15.161435 tkfly-0.1.0a4/tkfly/blend2d/demos/d101.py
+-rw-r--r--   0        0        0     6639 2023-04-29 16:01:28.838141 tkfly-0.1.0a4/tkfly/blend2d/demos/d102.py
+-rw-r--r--   0        0        0     4035 2023-04-30 01:41:51.892376 tkfly-0.1.0a4/tkfly/blend2d/demos/d110.py
+-rw-r--r--   0        0        0      350 2023-04-29 15:46:13.786327 tkfly-0.1.0a4/tkfly/blend2d/demos/d2.py
+-rw-r--r--   0        0        0      422 2023-04-29 15:47:21.757569 tkfly-0.1.0a4/tkfly/blend2d/demos/d3.py
+-rw-r--r--   0        0        0      806 2023-04-29 15:52:04.223698 tkfly-0.1.0a4/tkfly/blend2d/demos/d4_1.py
+-rw-r--r--   0        0        0     1733 2023-04-29 15:54:13.375735 tkfly-0.1.0a4/tkfly/blend2d/demos/d4_2.py
+-rw-r--r--   0        0        0      612 2023-04-29 15:54:54.800543 tkfly-0.1.0a4/tkfly/blend2d/demos/d5.py
+-rw-r--r--   0        0        0      663 2023-04-29 15:55:42.846526 tkfly-0.1.0a4/tkfly/blend2d/demos/d6.py
+-rw-r--r--   0        0        0      759 2023-04-29 16:00:16.838813 tkfly-0.1.0a4/tkfly/blend2d/demos/d7.py
+-rw-r--r--   0        0        0     4399 2023-04-30 01:27:49.755083 tkfly-0.1.0a4/tkfly/blend2d/demos/dct.py
+-rw-r--r--   0        0        0     5298 2020-08-12 14:00:30.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/demo-tiger.tcl
+-rw-r--r--   0        0        0     7474 2023-04-30 01:32:16.757048 tkfly-0.1.0a4/tkfly/blend2d/demos/dpda.py
+-rw-r--r--   0        0        0     4972 2023-04-29 16:03:00.011251 tkfly-0.1.0a4/tkfly/blend2d/demos/drect.py
+-rw-r--r--   0        0        0     5302 2023-04-30 01:25:21.918029 tkfly-0.1.0a4/tkfly/blend2d/demos/dtiger.py
+-rw-r--r--   0        0        0     3873 2020-06-23 06:06:42.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/greenSlate.jpg
+-rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/IKscale-1.0.1.tm
+-rw-r--r--   0        0        0     5415 2020-09-03 09:32:10.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/EbuttonColor-1.0.1.tm
+-rw-r--r--   0        0        0     4958 2020-09-03 09:38:00.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/Eseparator-1.0.tm
+-rw-r--r--   0        0        0     5965 2020-08-26 14:52:44.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/hatching-1.0.tm
+-rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/IKscale-1.0.1.tm
+-rw-r--r--   0        0        0    33360 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/darwin-x64/perlin.dylib
+-rw-r--r--   0        0        0      513 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/license.terms
+-rw-r--r--   0        0        0    11404 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/linux-x32/perlin.so
+-rw-r--r--   0        0        0    12456 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/linux-x64/perlin.so
+-rw-r--r--   0        0        0     1149 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/pkgIndex.tcl
+-rw-r--r--   0        0        0    11776 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/win-x32/perlin.dll
+-rw-r--r--   0        0        0    13312 2023-04-15 16:05:38.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/win-x64/perlin.dll
+-rw-r--r--   0        0        0    12189 2020-08-28 04:04:42.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/sketchline-1.0.tm
+-rw-r--r--   0        0        0   125189 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/main2.tcl
+-rw-r--r--   0        0        0     1052 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/pkgIndex.tcl
+-rw-r--r--   0        0        0      769 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/snit2.tcl
+-rw-r--r--   0        0        0      510 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/teapot.txt
+-rw-r--r--   0        0        0    18959 2020-09-03 12:26:26.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/validate.tcl
+-rw-r--r--   0        0        0    14134 2021-12-02 19:08:46.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/lib/Spline-1.0.tm
+-rw-r--r--   0        0        0    17997 2023-03-14 07:49:04.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/moby.svg
+-rw-r--r--   0        0        0     7576 2020-05-14 16:47:38.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/PorterDuffInAction.tcl
+-rw-r--r--   0        0        0    22057 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_1.svg
+-rw-r--r--   0        0        0    29922 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_2.svg
+-rw-r--r--   0        0        0    22020 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_3.svg
+-rw-r--r--   0        0        0    23936 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_4.svg
+-rw-r--r--   0        0        0    16595 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_5.svg
+-rw-r--r--   0        0        0      279 2023-03-14 14:01:34.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_6.svg
+-rw-r--r--   0        0        0     9507 2020-03-08 17:06:24.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/RGB.png
+-rw-r--r--   0        0        0      436 2016-06-18 19:26:30.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Road_Rage-License.txt
+-rw-r--r--   0        0        0   341760 2016-06-18 17:26:30.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/Road_Rage.otf
+-rw-r--r--   0        0        0    76248 2019-08-19 07:45:32.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/texture.jpeg
+-rw-r--r--   0        0        0   220752 2019-10-15 16:31:28.000000 tkfly-0.1.0a4/tkfly/blend2d/demos/tiger-data.tcl
+-rw-r--r--   0        0        0   146164 2021-05-28 11:22:28.000000 tkfly-0.1.0a4/tkfly/blend2d/HarmonyOS_Sans_Medium.ttf
+-rw-r--r--   0        0        0   640122 2023-04-29 13:45:10.413812 tkfly-0.1.0a4/tkfly/blend2d/surface.bmp
+-rw-r--r--   0        0        0     2217 2023-04-29 15:42:02.761477 tkfly-0.1.0a4/tkfly/core.py
+-rw-r--r--   0        0        0    18967 2023-04-30 04:52:41.939045 tkfly-0.1.0a4/tkfly/mkwidgets/__init__.py
+-rw-r--r--   0        0        0    19461 2023-04-30 04:59:06.062740 tkfly-0.1.0a4/tkfly/mkwidgets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2330 2023-04-30 06:26:29.255313 tkfly-0.1.0a4/tkfly/mkwidgets/__pycache__/calendar.cpython-311.pyc
+-rw-r--r--   0        0        0     2444 2023-04-30 05:39:01.184338 tkfly-0.1.0a4/tkfly/mkwidgets/__pycache__/document.cpython-311.pyc
+-rw-r--r--   0        0        0     8650 2023-04-30 06:11:01.304774 tkfly-0.1.0a4/tkfly/mkwidgets/__pycache__/toolbar.cpython-311.pyc
+-rw-r--r--   0        0        0     1735 2023-04-30 05:39:01.181335 tkfly-0.1.0a4/tkfly/mkwidgets/__pycache__/window.cpython-311.pyc
+-rw-r--r--   0        0        0      828 2023-04-30 06:19:04.707093 tkfly-0.1.0a4/tkfly/mkwidgets/calendar.py
+-rw-r--r--   0        0        0     1141 2023-04-30 04:51:39.983269 tkfly-0.1.0a4/tkfly/mkwidgets/document.py
+-rw-r--r--   0        0        0     5643 2023-04-30 06:11:01.170574 tkfly-0.1.0a4/tkfly/mkwidgets/toolbar.py
+-rw-r--r--   0        0        0      752 2023-04-30 05:34:41.536963 tkfly-0.1.0a4/tkfly/mkwidgets/window.py
+-rw-r--r--   0        0        0      239 2023-04-29 23:59:46.170477 tkfly-0.1.0a4/tkfly/mupdf/__init__.py
+-rw-r--r--   0        0        0    82231 2023-04-30 04:17:46.277250 tkfly-0.1.0a4/tkfly/saMDI.py
+-rw-r--r--   0        0        0      222 2023-04-14 12:59:16.512351 tkfly-0.1.0a4/tkfly/tkimg/__init__.py
+-rw-r--r--   0        0        0   221710 2022-11-24 07:55:52.000000 tkfly-0.1.0a4/tkfly/tkimg/jpegtcl950.dll
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a4/tkfly/tkimg/libjpegtclstub950.a
+-rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a4/tkfly/tkimg/libpngtclstub1638.a
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a4/tkfly/tkimg/libtifftclstub440.a
+-rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a4/tkfly/tkimg/libtkimgstub1414.a
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a4/tkfly/tkimg/libzlibtclstub1213.a
+-rw-r--r--   0        0        0     6851 2022-11-24 07:55:44.000000 tkfly-0.1.0a4/tkfly/tkimg/pkgIndex.tcl
+-rw-r--r--   0        0        0   231950 2022-11-24 07:55:52.000000 tkfly-0.1.0a4/tkfly/tkimg/pngtcl1638.dll
+-rw-r--r--   0        0        0   416782 2022-11-24 07:55:52.000000 tkfly-0.1.0a4/tkfly/tkimg/tifftcl440.dll
+-rw-r--r--   0        0        0    40462 2022-11-24 07:55:54.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimg1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:54.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgbmp1414.dll
+-rw-r--r--   0        0        0    22030 2022-11-24 07:55:54.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgdted1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:56.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgflir1414.dll
+-rw-r--r--   0        0        0    24590 2022-11-24 07:55:56.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimggif1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:56.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgico1414.dll
+-rw-r--r--   0        0        0    23054 2022-11-24 07:55:56.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgjpeg1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgpcx1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:58.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgpixmap1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgpng1414.dll
+-rw-r--r--   0        0        0    25102 2022-11-24 07:56:00.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgppm1414.dll
+-rw-r--r--   0        0        0    21006 2022-11-24 07:56:00.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgps1414.dll
+-rw-r--r--   0        0        0    31758 2022-11-24 07:56:00.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgraw1414.dll
+-rw-r--r--   0        0        0    28174 2022-11-24 07:56:02.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgsgi1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:56:02.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgsun1414.dll
+-rw-r--r--   0        0        0    25102 2022-11-24 07:56:02.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgtga1414.dll
+-rw-r--r--   0        0        0    70158 2022-11-24 07:56:04.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgtiff1414.dll
+-rw-r--r--   0        0        0    17934 2022-11-24 07:56:04.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgwindow1414.dll
+-rw-r--r--   0        0        0    19470 2022-11-24 07:56:04.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgxbm1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:56:06.000000 tkfly-0.1.0a4/tkfly/tkimg/tkimgxpm1414.dll
+-rw-r--r--   0        0        0    91662 2022-11-24 07:56:06.000000 tkfly-0.1.0a4/tkfly/tkimg/zlibtcl1213.dll
+-rw-r--r--   0        0        0        0 2023-04-19 11:17:10.457150 tkfly-0.1.0a4/tkfly/tklib/__init__.py
+-rw-r--r--   0        0        0      141 2023-04-19 12:43:56.373512 tkfly-0.1.0a4/tkfly/tklib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2594 2023-04-29 11:00:59.295786 tkfly-0.1.0a4/tkfly/tklib/__pycache__/datefield.cpython-311.pyc
+-rw-r--r--   0        0        0     8914 2023-04-29 05:02:59.020777 tkfly-0.1.0a4/tkfly/tklib/__pycache__/history.cpython-311.pyc
+-rw-r--r--   0        0        0     3960 2023-04-19 12:45:43.059958 tkfly-0.1.0a4/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0      538 2023-04-29 05:32:30.677805 tkfly-0.1.0a4/tkfly/tklib/autoscroll.py
+-rw-r--r--   0        0        0      573 2023-04-19 14:52:50.309476 tkfly-0.1.0a4/tkfly/tklib/chatwidget.py
+-rw-r--r--   0        0        0     1265 2023-04-29 10:59:14.922692 tkfly-0.1.0a4/tkfly/tklib/datefield.py
+-rw-r--r--   0        0        0     5389 2023-04-29 05:02:58.918925 tkfly-0.1.0a4/tkfly/tklib/history.py
+-rw-r--r--   0        0        0      583 2023-04-19 12:47:17.815625 tkfly-0.1.0a4/tkfly/tklib/menubar.py
+-rw-r--r--   0        0        0     1002 2023-04-29 05:26:07.066657 tkfly-0.1.0a4/tkfly/tklib/notifywindow.py
+-rw-r--r--   0        0        0     1331 2023-04-29 06:07:26.214511 tkfly-0.1.0a4/tkfly/tklib/plotchart.py
+-rw-r--r--   0        0        0     5389 2023-04-29 05:38:33.820659 tkfly-0.1.0a4/tkfly/tklib/shtmlview.py
+-rw-r--r--   0        0        0     2066 2023-04-19 12:45:42.877555 tkfly-0.1.0a4/tkfly/tklib/tooltip.py
+-rw-r--r--   0        0        0      902 2023-04-19 11:28:27.786655 tkfly-0.1.0a4/tkfly/tklib/wcb.py
+-rw-r--r--   0        0        0      523 2023-04-29 05:46:46.161323 tkfly-0.1.0a4/tkfly/tklib/widget.py
+-rw-r--r--   0        0        0      506 2023-04-29 11:29:28.404486 tkfly-0.1.0a4/tkfly/tkscrollutil/__init__.py
+-rw-r--r--   0        0        0      804 2023-04-29 11:29:28.606524 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1165 2023-04-29 11:09:26.181908 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc
+-rw-r--r--   0        0        0     1258 2023-04-29 11:29:43.706687 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc
+-rw-r--r--   0        0        0     3023 2023-04-29 11:14:55.822881 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc
+-rw-r--r--   0        0        0     4204 2023-04-29 11:12:49.744284 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc
+-rw-r--r--   0        0        0     3011 2023-04-29 11:29:28.610040 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc
+-rw-r--r--   0        0        0     2069 2023-04-29 11:34:46.885357 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc
+-rw-r--r--   0        0        0     3060 2023-04-29 11:26:17.297437 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2023-04-29 11:29:28.614038 tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc
+-rw-r--r--   0        0        0      413 2022-10-29 06:29:19.142527 tkfly-0.1.0a4/tkfly/tkscrollutil/attrib.py
+-rw-r--r--   0        0        0      458 2023-04-29 11:29:43.603589 tkfly-0.1.0a4/tkfly/tkscrollutil/load.py
+-rw-r--r--   0        0        0     1793 2023-04-29 13:55:50.749585 tkfly-0.1.0a4/tkfly/tkscrollutil/scrollableframe.py
+-rw-r--r--   0        0        0     1921 2023-04-29 11:14:55.722630 tkfly-0.1.0a4/tkfly/tkscrollutil/scrollarea.py
+-rw-r--r--   0        0        0     2480 2023-04-29 11:10:41.419659 tkfly-0.1.0a4/tkfly/tkscrollutil/scrollsync.py
+-rw-r--r--   0        0        0     1910 2023-04-29 11:29:28.409999 tkfly-0.1.0a4/tkfly/tkscrollutil/ttk_scrollarea.py
+-rw-r--r--   0        0        0     1142 2023-04-29 11:34:46.766705 tkfly-0.1.0a4/tkfly/tkscrollutil/ttk_scrollednotebook.py
+-rw-r--r--   0        0        0     1689 2023-04-29 11:26:17.197236 tkfly-0.1.0a4/tkfly/tkscrollutil/ttk_scrollsync.py
+-rw-r--r--   0        0        0     1435 2023-04-29 11:28:26.430882 tkfly-0.1.0a4/tkfly/tkscrollutil/wheelevent.py
+-rw-r--r--   0        0        0      544 2023-04-29 11:43:18.104764 tkfly-0.1.0a4/tkfly/twapi/__init__.py
+-rw-r--r--   0        0        0     1464 2023-04-29 11:43:18.209994 tkfly-0.1.0a4/tkfly/twapi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      359 2023-04-29 07:58:45.679468 tkfly-0.1.0a4/tkfly/twapi/base.py
+-rw-r--r--   0        0        0      230 2023-04-29 07:58:45.713014 tkfly-0.1.0a4/tkfly/twapi/msi.py
+-rw-r--r--   0        0        0      704 2023-04-29 10:07:46.018924 tkfly-0.1.0a4/tkfly/twapi/ui.py
+-rw-r--r--   0        0        0      585 2023-04-29 08:16:43.020235 tkfly-0.1.0a4/tkfly/twapi/win.py
+-rw-r--r--   0        0        0     8811 1970-01-01 00:00:00.000000 tkfly-0.1.0a4/PKG-INFO
```

### Comparing `tkfly-0.1.0a3/README.md` & `tkfly-0.1.0a4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 ([blend2d -大小约7.6MB](https://wiki.tcl-lang.org/page/Blend2d))
 
 帮助你开发大型高级的程序
 
 ## 教程
 
 ### 开始
-`tkfly`通过`tkinter`调用`tcl`导入`tklib`实现，可以实现`tklib`库所能实现的各种功能。
 ```bash
 # 暂时处于预览版
 python -m pip install tkfly --pre
 ```
 
 ### 工具提示
+`tkfly`通过`tkinter`调用`tcl`导入`tklib`实现，可以实现`tklib`库所能实现的各种功能。
 让我来运行一个最简单工具提示吧！
 (基于[tklib/tooltip](https://core.tcl-lang.org/tklib/doc/trunk/embedded/md/tklib/files/modules/tooltip/tooltip.md))
 ```python
 from tkinter import Tk, ttk
 from tkfly import FlyToolTip
 
 root = Tk()
@@ -108,14 +108,16 @@
 
 root = Tk()
 blend2D = Fly2D()
 surface = blend2D.create_image_surface(
     size=(500, 500)
 )
 
+print("Create ImageSurface", surface.image_name)
+
 surface.surface.fill(
     blend2D.create_circle((150, 150), 50),
     blend2D.get_color("lightblue", alpha=0.5)
 )
 
 surface.surface.fill(
     blend2D.create_circle((250, 250), 60),
@@ -123,50 +125,102 @@
 )
 
 surface.surface.fill(
     blend2D.create_circle((350, 350), 55),
     blend2D.get_color("lightblue", alpha=0.75)
 )
 
+from tkfly.core import fly_local, fly_chdir
+
+with fly_chdir(fly_local() + "\\blend2d"):
+    fontface = blend2D.create_fontface(fontfile="HarmonyOS_Sans_Medium.ttf")
+    font = blend2D.create_font(fontface=fontface, fontsize=20)
+
+print("Create FontFace", fontface._name)
+print("Create Font", font._name)
 
 surface.surface.fill(
-    blend2D.create_text((235, 255), string="Fly2D"),
+    blend2D.create_text((225, 257), string="Fly2D", font=font),
     blend2D.get_color("black")
 )
 
 surface.pack()
 
 surface.surface.save("fly2d.png")
 
 root.mainloop()
 ```
 
-# tkscrollutil
+### 扩展组件
+#### Document
+这是类似`多文档窗口`类的组件，只是暂时布局没想到好的方案，会空下大部分的空间
+```python
+from tkinter import *
+from tkinter import ttk
+from tkfly import *
+
+root = Tk()
+
+document = FlyMkDocument()
+
+button = ttk.Button(document)
+button.pack(fill="both", expand="yes")
+
+document.config(title="这是多文档窗口")
+
+root.mainloop()
+```
+
+#### ToolBar
+工具栏组件
+```python
+from tkinter import *
+from tkfly import *
+
+root = Tk()
+
+toolbar = FlyMkToolBar()
+
+button1 = toolbar.add(
+    "button",
+    command=lambda:
+        print(f"toolbutton is {toolbar.get(button1)}")
+)
+button2 = toolbar.add("button", command=lambda: toolbar.delete(button2))
+
+
+toolbar.pack(fill="x", side="top")
+
+root.mainloop()
+```
+
+
+## tkscrollutil
 实际上这就是作者我以前做过的一个项目。
 
-## ScrolllArea
+### ScrolllArea
 可以快速地为水平滚动、垂直滚动组件设置滚动条
 
-### 属性
+#### 属性
 `autohidescrollbars` 设置组件是否自动隐藏滚动条。布尔数值。默认`False`。也就是说，当你把鼠标指针放到滚动条上时，滚动条才会显示。 
 
 `lockinterval` 设置组件滚动条地锁定间隔。整数数值。默认`300`.
 
 `respectheader` 仅当将嵌入到组件内地`tablelist`版本为6.5及以上版本时才能使用，后续等开发出`tablelist`的扩展库时补充
 
 `respecttitlecolumns` 仅当将嵌入到组件内地`tablelist`版本为6.5及以上版本时才能使用，后续等开发出`tablelist`的扩展库时补充
 
 `xscrollbarmode` 设置水平滚动条的模式。可选值为`static` `dynamic` `none`。默认`none`。`static`为常驻滚动条；`dynamic`为自动滚动条；`none`为没有滚动条
 
 `yscrollbarmode` 设置垂直滚动条的模式。可选值为`static` `dynamic` `none`。默认`static`。`static`为常驻滚动条；`dynamic`为自动滚动条；`none`为没有滚动条
 
-### 方法
+#### 方法
 `setwidget` 设置具有滚动条属性的组件，使组件快速设置滚动条。
 
-### 示例
+#### 示例
 ```python
 from tkinter import Tk, Listbox
 from tkfly.tkscrollutil import ScrollArea
 
 Window = Tk()
 
 Area = ScrollArea(Window)
@@ -175,18 +229,18 @@
     List.insert(Item+1, Item+1)
 Area.setwidget(List)
 Area.pack(fill="both", expand="yes")
 
 Window.mainloop()
 ```
 
-## ttkScrollArea
+#### ttkScrollArea
 见上方。与`ScrollArea`不同的是，`ttkScrollArea`具有ttk组件的属性，并且`ScrollArea`和`ttkScrollArea`不能同时使用。
 
-### 示例
+#### 示例
 ```python
 from tkinter import Tk, Listbox
 from tkfly.tkscrollutil import ttkScrollArea
 
 Window = Tk()
 
 Area = ttkScrollArea(Window)
@@ -195,23 +249,23 @@
     List.insert(Item+1, Item+1)
 Area.setwidget(List)
 Area.pack(fill="both", expand="yes")
 
 Window.mainloop()
 ```
 
-## ScrollSync
+#### ScrollSync
 同步滚动条，当其中一个滚动时，另一个也会跟随着移动起来。
 
-### 方法
+#### 方法
 `setwidgets` 设置同步滚动的组件。需输入列表，如 [widget1, widget2] 。
 
 `widgets` 获取同步滚动的组件。
 
-### 示例
+#### 示例
 ```python
 from tkinter import Tk, Listbox, Frame
 from tkfly.tkscrollutil import ScrollArea, ScrollSync
 Window = Tk()
 
 Frame = Frame()
 
@@ -233,18 +287,18 @@
 Sync.setwidgets([List1, List2])
 
 Frame.pack(fill="both", expand="yes")
 
 Window.mainloop()
 ```
 
-## ttkScrollSync
+#### ttkScrollSync
 见上方。与`ScrollSync`不同的是，`ttkScrollSync`具有ttk组件的属性，并且`ScrollSync`和`ttkScrollSync`不能同时使用。
 
-### 示例
+#### 示例
 ```python
 from tkinter import Tk, Listbox, Frame
 from tkfly.tkscrollutil import ttkScrollArea, ttkScrollSync
 Window = Tk()
 
 Frame = Frame()
 
@@ -266,15 +320,15 @@
 Sync.setwidgets([List1, List2])
 
 Frame.pack(fill="both", expand="yes")
 
 Window.mainloop()
 ```
 
-## ttkScrolledNoteBook
+#### ttkScrolledNoteBook
 scrollutil本身不提供ScrolledNoteBook，只有ttk能够提供。
 ```python
 from tkinter import Tk, Frame
 from tkfly.tkscrollutil import ttkScrolledNoteBook, addclosetab
 Window = Tk()
 
 NoteBook = ttkScrolledNoteBook(Window)
```

### Comparing `tkfly-0.1.0a3/tkfly/__main__.py` & `tkfly-0.1.0a4/tkfly/__main__.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libblend2d.dylib` & `tkfly-0.1.0a4/tkfly/_blend2d/darwin-x64/libblend2d.dylib`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libtclb2d.dylib` & `tkfly-0.1.0a4/tkfly/_blend2d/darwin-x64/libtclb2d.dylib`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libtkb2d.dylib` & `tkfly-0.1.0a4/tkfly/_blend2d/darwin-x64/libtkb2d.dylib`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/Blacksword.otf` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/Blacksword.otf`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/CMYK.png` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/CMYK.png`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/CompositionTest.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/CompositionTest.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/PorterDuffInAction.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/PorterDuffInAction.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/RGB.png` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/comp-op/RGB.png`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/demo-tiger.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/demo-tiger.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/bl-qt-tiger.h` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/develTools/bl-qt-tiger.h`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/Ghostscript_Tiger.svg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/develTools/Ghostscript_Tiger.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.cpp` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.cpp`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.exe` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.exe`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/tiger-data.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/demo-tiger/tiger-data.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/greenSlate.jpg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/greenSlate.jpg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/EbuttonColor-1.0.1.tm` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/EbuttonColor-1.0.1.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/Eseparator-1.0.tm` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/Eseparator-1.0.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/hatching-1.0.tm` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/hatching-1.0.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/IKscale-1.0.1.tm` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/IKscale-1.0.1.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/darwin-x64/perlin.dylib` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/darwin-x64/perlin.dylib`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/license.terms` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/license.terms`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x32/perlin.so` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x32/perlin.so`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x64/perlin.so` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x64/perlin.so`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/win-x32/perlin.dll` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/win-x32/perlin.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/win-x64/perlin.dll` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/perlin-1.0/win-x64/perlin.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/sketchline-1.0.tm` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/sketchline-1.0.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/main2.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/main2.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/snit2.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/snit2.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/validate.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/snit.2.3.2/validate.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/Spline-1.0.tm` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/lib/Spline-1.0.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/moby.svg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/moby.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_1.svg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_1.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_2.svg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_2.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_3.svg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_3.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_4.svg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_4.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_5.svg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/Q/layer_5.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/Road_Rage.otf` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/Road_Rage.otf`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample-poly.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample-poly.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample-rect.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample-rect.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample04i.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample04i.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample04ii.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample04ii.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample05.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample05.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample06.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample06.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample07.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample07.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample101.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample101.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample102.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample102.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample103.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103a.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample103a.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103b.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample103b.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample104-handmadelines.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample104-handmadelines.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample105-SVGmoby.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample105-SVGmoby.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample106.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample106.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample107.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample107.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample108.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample108.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample109.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample109.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample110.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample110.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/sample111.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/sample111.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/demo/texture.jpeg` & `tkfly-0.1.0a4/tkfly/_blend2d/demo/texture.jpeg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.html` & `tkfly-0.1.0a4/tkfly/_blend2d/docs/tclBlend2d.html`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.man` & `tkfly-0.1.0a4/tkfly/_blend2d/docs/tclBlend2d.man`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.wiki.txt` & `tkfly-0.1.0a4/tkfly/_blend2d/docs/tclBlend2d.wiki.txt`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/HSB.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/HSB.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libblend2d.so` & `tkfly-0.1.0a4/tkfly/_blend2d/linux-x64/libblend2d.so`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libtclb2d.so` & `tkfly-0.1.0a4/tkfly/_blend2d/linux-x64/libtclb2d.so`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libtkb2d.so` & `tkfly-0.1.0a4/tkfly/_blend2d/linux-x64/libtkb2d.so`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/Mtx.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/Mtx.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/SVGpath.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/SVGpath.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/t2d.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/t2d.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/t2d_filters.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/t2d_filters.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/t2dsvg.tcl` & `tkfly-0.1.0a4/tkfly/_blend2d/t2dsvg.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/tclBlend2D-license.terms` & `tkfly-0.1.0a4/tkfly/_blend2d/tclBlend2D-license.terms`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/win-x64/blend2d.dll` & `tkfly-0.1.0a4/tkfly/_blend2d/win-x64/blend2d.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/win-x64/tclb2d.dll` & `tkfly-0.1.0a4/tkfly/_blend2d/win-x64/tclb2d.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_blend2d/win-x64/tkb2d.dll` & `tkfly-0.1.0a4/tkfly/_blend2d/win-x64/tkb2d.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/CHANGES.txt` & `tkfly-0.1.0a4/tkfly/_mupdf/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/demo/demo.pdf` & `tkfly-0.1.0a4/tkfly/_mupdf/demo/demo.pdf`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/demo/demo.tcl` & `tkfly-0.1.0a4/tkfly/_mupdf/demo/demo.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/demo/demo_sharedPdf.tcl` & `tkfly-0.1.0a4/tkfly/_mupdf/demo/demo_sharedPdf.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/docs/MuPDFWidget.html` & `tkfly-0.1.0a4/tkfly/_mupdf/docs/MuPDFWidget.html`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/docs/MuPDFWidget.man` & `tkfly-0.1.0a4/tkfly/_mupdf/docs/MuPDFWidget.man`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/main2.tcl` & `tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/main2.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/snit2.tcl` & `tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/snit2.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/validate.tcl` & `tkfly-0.1.0a4/tkfly/_mupdf/lib/snit-2.3.2/validate.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_mupdf/MuPDFWidget.tcl` & `tkfly-0.1.0a4/tkfly/_mupdf/MuPDFWidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc` & `tkfly-0.1.0a4/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/autoscroll/autoscroll.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/autoscroll/autoscroll.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/autoscroll/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/autoscroll/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_drag.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_drag.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_epoints.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_epoints.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_epolyline.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_epolyline.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_equad.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_equad.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_gradient.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_gradient.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_highlight.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_highlight.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_mvg.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_mvg.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_snap.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_snap.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_sqmap.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_sqmap.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_tags.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_tags.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_trlines.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_trlines.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_zoom.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/canvas_zoom.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/canvas/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/canvas/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/chatwidget/chatwidget.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/chatwidget/chatwidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/bindDown.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/controlwidget/bindDown.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/led.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/controlwidget/led.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/controlwidget/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/radioMatrix.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/controlwidget/radioMatrix.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/rdial.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/controlwidget/rdial.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/tachometer.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/controlwidget/tachometer.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/vertical_meter.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/controlwidget/vertical_meter.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/voltmeter.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/controlwidget/voltmeter.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/crosshair/crosshair.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/crosshair/crosshair.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/ctext/ctext.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/ctext/ctext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/cursor/cursor.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/cursor/cursor.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/datefield/datefield.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/datefield/datefield.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/application.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/application.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/attributes.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/attributes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/basic.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/basic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/core.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/core.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/diagram.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/diagram.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/direction.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/direction.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/element.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/element.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/navigation.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/navigation.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/diagrams/point.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/diagrams/point.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/getstring/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/getstring/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/getstring/tk_getString.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/getstring/tk_getString.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/history/history.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/history/history.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/history/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/history/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/ico/ico.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/ico/ico.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/ico/ico0.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/ico/ico0.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/ipentry/ipentry.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/ipentry/ipentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/cs.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/cs.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/da.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/da.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/de.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/de.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/en.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/en.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/es.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/es.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/khim.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/khim/khim.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/khim/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/pl.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/pl.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/ROOT.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/ROOT.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/ru.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/ru.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/khim/uk.msg` & `tkfly-0.1.0a4/tkfly/_tklib/khim/uk.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/mentry_tile.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/mentry_tile.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/mentryPublic.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/mentryPublic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryThemes.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryThemes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryWidget.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mentryWidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mwutil.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/tclIndex` & `tkfly-0.1.0a4/tkfly/_tklib/mentry/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/menubar/debug.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/menubar/debug.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/menubar/menubar.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/menubar/menubar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/menubar/node.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/menubar/node.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/menubar/tree.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/menubar/tree.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/notifywindow/notifywindow.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/notifywindow/notifywindow.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/notifywindow/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/notifywindow/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/ntext/ntext.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/ntext/ntext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/persistentSelection/persistentSelection.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/persistentSelection/persistentSelection.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plot3d.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plot3d.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotanim.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotanim.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotannot.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotannot.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotaxis.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotaxis.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotbind.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotbind.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotbusiness.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotbusiness.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotchart.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotchart.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotcombined.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotcombined.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotconfig.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotconfig.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotcontour.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotcontour.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotgantt.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotgantt.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotobject.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotobject.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotpack.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotpack.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotpriv.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotpriv.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotscada.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotscada.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotspecial.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotspecial.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotstatustimeline.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plotstatustimeline.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plottable.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/plottable.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/scaling.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/scaling.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/plotchart/xyplot.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/plotchart/xyplot.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/attrib.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/attrib.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/mwutil.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/pagesman.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/pagesman.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/tclIndex` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutil.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scrollutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutil_tile.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scrollutil_tile.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutilCommon.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/scrollutil/scrollutilCommon.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/style/as.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/style/as.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/style/lobster.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/style/lobster.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/style/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/style/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/style/style.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/style/style.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/swaplist/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/swaplist/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/swaplist/swaplist.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/swaplist/swaplist.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/mwutil.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/pencil.cur` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/pencil.cur`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/repair.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/repair.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tclIndex` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelist_tile.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/tablelist_tile.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelistPublic.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tablelist/tablelistPublic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/boxlabel.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/boxlabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/canlabel.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/canlabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/labarray.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/labarray.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/objselec.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/objselec.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/perilabel.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/perilabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pie.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/pie.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pielabel.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/pielabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/relirect.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/relirect.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/selector.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/selector.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/slice.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/slice.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/tkpiechart.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tkpiechart/tkpiechart.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tooltip/tipstack.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tooltip/tipstack.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/tooltip/tooltip.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/tooltip/tooltip.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/tclIndex` & `tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbCommon.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbCommon.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbEntry.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbEntry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbListbox.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbListbox.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbText.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbText.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/wcb/wcb.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/wcb/wcb.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/arrowb.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/arrowb.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/calendar.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/calendar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/dateentry.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/dateentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/dialog.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/dialog.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/mentry.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/mentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/panelframe.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/panelframe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/ruler.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/ruler.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/scrollw.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/scrollw.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/statusbar.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/statusbar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/stext.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/stext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/superframe.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/superframe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/toolbar.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/toolbar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widget/widget.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widget/widget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widgetl/listentry.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widgetl/listentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widgetl/listsimple.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widgetl/listsimple.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widgetPlus/widgetPlus.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widgetPlus/widgetPlus.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_tklib/widgetv/validator.tcl` & `tkfly-0.1.0a4/tkfly/_tklib/widgetv/validator.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/account.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/account.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/adsi.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/adsi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/apputil.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/apputil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/base.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/base.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/clipboard.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/clipboard.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/com.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/com.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/console.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/console.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/crypto.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/crypto.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/device.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/device.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/etw.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/etw.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/eventlog.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/eventlog.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/evt.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/evt.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/handle.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/handle.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/input.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/input.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/LICENSE` & `tkfly-0.1.0a4/tkfly/_twapi/LICENSE`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/metoo.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/metoo.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/msi.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/msi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/mstask.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/mstask.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/multimedia.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/multimedia.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/namedpipe.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/namedpipe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/network.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/network.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/nls.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/nls.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/os.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/os.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/pdh.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/pdh.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/power.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/power.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/printer.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/printer.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/process.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/process.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/rds.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/rds.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/README.md` & `tkfly-0.1.0a4/tkfly/_twapi/README.md`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/registry.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/registry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/resource.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/resource.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/security.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/security.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/service.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/service.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/share.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/share.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/shell.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/shell.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/sspi.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/sspi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/storage.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/storage.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/synch.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/synch.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/tls.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/tls.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/twapi.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/twapi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/twapi_base.dll` & `tkfly-0.1.0a4/tkfly/_twapi/twapi_base.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/twapi_base64.dll` & `tkfly-0.1.0a4/tkfly/_twapi/twapi_base64.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/ui.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/ui.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/win.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/win.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/winlog.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/winlog.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/winsta.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/winsta.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/_twapi/wmi.tcl` & `tkfly-0.1.0a4/tkfly/_twapi/wmi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/__init__.py` & `tkfly-0.1.0a4/tkfly/blend2d/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,24 @@
     return f"BL::rgb {RR} {GG} {BB} {alpha}"
 
 
 def gradient(type: GRADIENT_TYPE, values, stopList):
     return f"BL::gradient {type} {values} [list {stopList}]"
 
 
-def circle(cx, cy, r=50):
-    return "BL::circle" + " {" + str(cx) + " " + str(cy) + "} " + str(r)
+def circle(circlex, circley, r=50):
+    return "BL::circle" + " {" + str(circlex) + " " + str(circley) + "} " + str(r)
+
+
+def rect(x, y, width, height):
+    return "BL::rect" + f" {str(x)} {str(y)} {str(width)} {str(height)}"
+
+
+def roundrect(x, y, width, height, rx, ry=""):
+    return "BL::roundrect" + f" {str(x)} {str(y)} {str(width)} {str(height)} {str(rx)} {str(ry)}"
 
 
 def text(cx, cy, font, string: str = ""):
     return "BL::text" + " {" + str(cx) + " " + str(cy) + "} " + str(font) + " " + f'"{str(string)}"'
 
 
 def classes():
@@ -51,29 +59,32 @@
 def platform():
     load_blend2d()
     return fly_root().call("BL::platform")
 
 
 def radint_id():
     from random import randint
-    return str(randint(0, 9999) + randint(0, 9999) + randint(0, 9999) + randint(0, 9999))
+    return str(randint(0, 9999) + randint(0, 9999) + randint(0, 9999) + randint(0, 9999) - randint(0, 9999) - randint(0, 9999))
 
 
 class Blend2DImage(Image):
     def __init__(self, surface, cnf={}, master=None, **kw):
         Image.__init__(self, 'blend2d', surface, cnf, **kw)
 
 
 class Surface(object):
     def __init__(self, name: str = ".surface", width: int = 450, height: int = 450, iscreate: bool = True):
         load_blend2d()
         self._name = name+radint_id()
         if iscreate:
             self.create(self._name, width=width, height=height)
 
+    def destory(self):
+        fly_root().call(self._name, "destory")
+
     def create(self, name: str = ".surface", width: int = 450, height: int = 450):
         fly_root().eval(f"BL::Surface create {name} -format "+"{ "+str(width)+" "+str(height)+" }")
 
     def clear(self, style="BL::color black"):
         fly_root().eval(f"{self._name} clear -fill.style [{style}]")
 
     def save(self, file: str = "surface.bmp"):
@@ -164,29 +175,37 @@
         Blead2D引擎
         """
 
         load_blend2d()
 
     @staticmethod
     def create_fontface(name: str = ".fontface", fontfile: str = None, id: int = 100):
-        return FontFace(name=name, fontfile=fontfile.replace("\\", "/"), faceIdxL=id)
+        return FontFace(name=name, fontfile=fontfile.replace("\\", "/"), faceIdxL=str(id)+radint_id())
 
     @staticmethod
     def create_font(name: str = ".font", fontface: FontFace = None, fontsize: int = 12):
         return Font(name=name, fontface=fontface._name, fontsize=fontsize)
 
     @staticmethod
     def create_surface(name: str = ".surface", size: tuple = (450, 450)):
         return Surface(name=name, width=size[0], height=size[1])
 
     @staticmethod
     def create_image_surface(name: str = ".surface", image_name: str = ".surface.image", size: tuple = (450, 450)):
         return ImageSurface(name=name, image_name=image_name, width=size[0], height=size[1])
 
     @staticmethod
+    def create_roundrect(x, y, width, height, rx, ry=""):
+        return roundrect(x, y, width, height, rx, ry)
+
+    @staticmethod
+    def create_rect(x, y, width, height):
+        return rect(x, y, width, height)
+
+    @staticmethod
     def create_circle(pos: tuple = (0, 0), size: int or float = 40):
         return circle(pos[0], pos[1], size)
 
     @staticmethod
     def create_text(pos: tuple = (0, 0), font: Font = None, string: str = ""):
         if font is None:
             from tkfly.core import fly_local, fly_chdir
@@ -234,10 +253,12 @@
     from tkfly.core import fly_local, fly_chdir
 
     fontface1 = blend2d.create_fontface(fontfile="HarmonyOS_Sans_Medium.ttf")
     font1 = blend2d.create_font(fontface=fontface1)
 
     surface.surface.fill(circle(150, 225, 50), color("lightblue"))
 
+    surface.surface.fill(roundrect(20, 20, 100, 100, 20), color("orange"))
+
     surface.pack(fill="both")
 
     root.mainloop()
```

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/__pycache__/__init__.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,45 +1,49 @@
 magic:    0xa70d0d0a
-moddate:  0x43ca4d64 (Sun Apr 30 01:54:11 2023 UTC)
-files sz: 7757
+moddate:  0xc6e04d64 (Sun Apr 30 03:30:14 2023 UTC)
+files sz: 8486
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 7
+   stacksize : 9
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a040100640064
       026c056d065a066d075a076d085a080100640064036c096d0a5a0a010064
       0484005a0b64055a0c64065a0d64075a0e02004700640884006409650aa6
-      030000ab0300000000000000005a0f6437640b65106602640c84055a1164
-      38640b65106602640d84055a12640e650f6602640f84045a136439641184
-      015a14643a641365156602641484055a16641584005a17641684005a1864
-      1784005a19641884005a1a0200470064198400641a6507a6030000ab0300
-      000000000000005a1b02004700641b8400641c651ca6030000ab03000000
-      00000000005a1d02004700641d8400641e651ca6030000ab030000000000
-      0000005a1e02004700641f84006420651ca6030000ab0300000000000000
-      005a1f020047006421840064226508a6030000ab0300000000000000005a
-      2002004700642384006424651ca6030000ab0300000000000000005a2165
-      2264256b020000000072ee640064266c056d235a236d245a246d085a0801
-      0002006523a6000000ab0000000000000000005a250200650802006518a6
-      000000ab000000000000000000ac27a6010000ab0100000000000000005a
-      266526a027000000000000000000000000000000000000000064286429ac
-      2aa6020000ab020000000000000000010002006521a6000000ab00000000
-      00000000005a286528a02900000000000000000000000000000000000000
-      00642bac2ca6010000ab0100000000000000005a2a6400642d6c006d035a
-      036d045a0401006528a02b00000000000000000000000000000000000000
-      00642eac2fa6010000ab0100000000000000005a2c6528a02d0000000000
-      000000000000000000000000000000652cac30a6010000ab010000000000
-      0000005a2e652a6a2a0000000000000000a02f0000000000000000000000
-      00000000000000000002006514643164326410a6030000ab030000000000
-      000000020065116433a6010000ab010000000000000000a6020000ab0200
-      000000000000000100652aa0270000000000000000000000000000000000
-      0000006434ac35a6010000ab01000000000000000001006525a030000000
-      0000000000000000000000000000000000a6000000ab0000000000000000
-      0001006436530064365300
+      030000ab0300000000000000005a0f643c640b65106602640c84055a1164
+      3d640b65106602640d84055a12640e650f6602640f84045a13643e641184
+      015a14641284005a15643f641484015a16643f641565176602641684055a
+      18641784005a19641884005a1a641984005a1b641a84005a1c0200470064
+      1b8400641c6507a6030000ab0300000000000000005a1d02004700641d84
+      00641e651ea6030000ab0300000000000000005a1f02004700641f840064
+      20651ea6030000ab0300000000000000005a200200470064218400642265
+      1ea6030000ab0300000000000000005a21020047006423840064246508a6
+      030000ab0300000000000000005a2202004700642584006426651ea60300
+      00ab0300000000000000005a23652464276b02000000009001721f640064
+      286c056d255a256d265a266d085a08010002006525a6000000ab00000000
+      00000000005a27020065080200651aa6000000ab000000000000000000ac
+      29a6010000ab0100000000000000005a286528a029000000000000000000
+      0000000000000000000000642a642bac2ca6020000ab0200000000000000
+      00010002006523a6000000ab0000000000000000005a2a652aa02b000000
+      0000000000000000000000000000000000642dac2ea6010000ab01000000
+      00000000005a2c6400642f6c006d035a036d045a040100652aa02d000000
+      00000000000000000000000000000000006430ac31a6010000ab01000000
+      00000000005a2e652aa02f00000000000000000000000000000000000000
+      00652eac32a6010000ab0100000000000000005a30652c6a2c0000000000
+      000000a03100000000000000000000000000000000000000000200651464
+      3364346410a6030000ab030000000000000000020065116435a6010000ab
+      010000000000000000a6020000ab0200000000000000000100652c6a2c00
+      00000000000000a031000000000000000000000000000000000000000002
+      00651664366436643764376436a6050000ab050000000000000000020065
+      116438a6010000ab010000000000000000a6020000ab0200000000000000
+      000100652ca02900000000000000000000000000000000000000006439ac
+      3aa6010000ab01000000000000000001006527a032000000000000000000
+      0000000000000000000000a6000000ab0000000000000000000100643b53
+      00643b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('fly_load4', 'fly_root', 'fly_local', 'fly_chdir'))
                  6 IMPORT_NAME              0 (tkfly.core)
                  8 IMPORT_FROM              1 (fly_load4)
                 10 STORE_NAME               1 (fly_load4)
@@ -88,244 +92,275 @@
                 82 MAKE_FUNCTION            0
                 84 LOAD_CONST               9 ('GRADIENT_TYPE')
                 86 LOAD_NAME               10 (Enum)
                 88 PRECALL                  3
                 92 CALL                     3
                102 STORE_NAME              15 (GRADIENT_TYPE)
    
-    21         104 LOAD_CONST              55 ((1.0,))
+    21         104 LOAD_CONST              60 ((1.0,))
                106 LOAD_CONST              11 ('alpha')
                108 LOAD_NAME               16 (float)
                110 BUILD_TUPLE              2
                112 LOAD_CONST              12 (<code object color, file "D:\tkfly\tkfly\blend2d\__init__.py", line 21>)
                114 MAKE_FUNCTION            5 (defaults, annotations)
                116 STORE_NAME              17 (color)
    
-    25         118 LOAD_CONST              56 ((0, 0, 0, 1.0))
+    25         118 LOAD_CONST              61 ((0, 0, 0, 1.0))
                120 LOAD_CONST              11 ('alpha')
                122 LOAD_NAME               16 (float)
                124 BUILD_TUPLE              2
                126 LOAD_CONST              13 (<code object rgb, file "D:\tkfly\tkfly\blend2d\__init__.py", line 25>)
                128 MAKE_FUNCTION            5 (defaults, annotations)
                130 STORE_NAME              18 (rgb)
    
     29         132 LOAD_CONST              14 ('type')
                134 LOAD_NAME               15 (GRADIENT_TYPE)
                136 BUILD_TUPLE              2
                138 LOAD_CONST              15 (<code object gradient, file "D:\tkfly\tkfly\blend2d\__init__.py", line 29>)
                140 MAKE_FUNCTION            4 (annotations)
                142 STORE_NAME              19 (gradient)
    
-    33         144 LOAD_CONST              57 ((50,))
+    33         144 LOAD_CONST              62 ((50,))
                146 LOAD_CONST              17 (<code object circle, file "D:\tkfly\tkfly\blend2d\__init__.py", line 33>)
                148 MAKE_FUNCTION            1 (defaults)
                150 STORE_NAME              20 (circle)
    
-    37         152 LOAD_CONST              58 (('',))
-               154 LOAD_CONST              19 ('string')
-               156 LOAD_NAME               21 (str)
-               158 BUILD_TUPLE              2
-               160 LOAD_CONST              20 (<code object text, file "D:\tkfly\tkfly\blend2d\__init__.py", line 37>)
-               162 MAKE_FUNCTION            5 (defaults, annotations)
-               164 STORE_NAME              22 (text)
-   
-    41         166 LOAD_CONST              21 (<code object classes, file "D:\tkfly\tkfly\blend2d\__init__.py", line 41>)
-               168 MAKE_FUNCTION            0
-               170 STORE_NAME              23 (classes)
-   
-    46         172 LOAD_CONST              22 (<code object libinfo, file "D:\tkfly\tkfly\blend2d\__init__.py", line 46>)
-               174 MAKE_FUNCTION            0
-               176 STORE_NAME              24 (libinfo)
-   
-    51         178 LOAD_CONST              23 (<code object platform, file "D:\tkfly\tkfly\blend2d\__init__.py", line 51>)
-               180 MAKE_FUNCTION            0
-               182 STORE_NAME              25 (platform)
-   
-    56         184 LOAD_CONST              24 (<code object radint_id, file "D:\tkfly\tkfly\blend2d\__init__.py", line 56>)
-               186 MAKE_FUNCTION            0
-               188 STORE_NAME              26 (radint_id)
-   
-    61         190 PUSH_NULL
-               192 LOAD_BUILD_CLASS
-               194 LOAD_CONST              25 (<code object Blend2DImage, file "D:\tkfly\tkfly\blend2d\__init__.py", line 61>)
-               196 MAKE_FUNCTION            0
-               198 LOAD_CONST              26 ('Blend2DImage')
-               200 LOAD_NAME                7 (Image)
-               202 PRECALL                  3
-               206 CALL                     3
-               216 STORE_NAME              27 (Blend2DImage)
-   
-    66         218 PUSH_NULL
-               220 LOAD_BUILD_CLASS
-               222 LOAD_CONST              27 (<code object Surface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 66>)
-               224 MAKE_FUNCTION            0
-               226 LOAD_CONST              28 ('Surface')
-               228 LOAD_NAME               28 (object)
-               230 PRECALL                  3
-               234 CALL                     3
-               244 STORE_NAME              29 (Surface)
-   
-   112         246 PUSH_NULL
-               248 LOAD_BUILD_CLASS
-               250 LOAD_CONST              29 (<code object FontFace, file "D:\tkfly\tkfly\blend2d\__init__.py", line 112>)
-               252 MAKE_FUNCTION            0
-               254 LOAD_CONST              30 ('FontFace')
-               256 LOAD_NAME               28 (object)
-               258 PRECALL                  3
-               262 CALL                     3
-               272 STORE_NAME              30 (FontFace)
-   
-   123         274 PUSH_NULL
-               276 LOAD_BUILD_CLASS
-               278 LOAD_CONST              31 (<code object Font, file "D:\tkfly\tkfly\blend2d\__init__.py", line 123>)
-               280 MAKE_FUNCTION            0
-               282 LOAD_CONST              32 ('Font')
-               284 LOAD_NAME               28 (object)
-               286 PRECALL                  3
-               290 CALL                     3
-               300 STORE_NAME              31 (Font)
-   
-   137         302 PUSH_NULL
-               304 LOAD_BUILD_CLASS
-               306 LOAD_CONST              33 (<code object ImageSurface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 137>)
-               308 MAKE_FUNCTION            0
-               310 LOAD_CONST              34 ('ImageSurface')
-               312 LOAD_NAME                8 (Label)
-               314 PRECALL                  3
-               318 CALL                     3
-               328 STORE_NAME              32 (ImageSurface)
-   
-   161         330 PUSH_NULL
-               332 LOAD_BUILD_CLASS
-               334 LOAD_CONST              35 (<code object Blend2D, file "D:\tkfly\tkfly\blend2d\__init__.py", line 161>)
-               336 MAKE_FUNCTION            0
-               338 LOAD_CONST              36 ('Blend2D')
-               340 LOAD_NAME               28 (object)
-               342 PRECALL                  3
-               346 CALL                     3
-               356 STORE_NAME              33 (Blend2D)
-   
-   219         358 LOAD_NAME               34 (__name__)
-               360 LOAD_CONST              37 ('__main__')
-               362 COMPARE_OP               2 (==)
-               368 POP_JUMP_FORWARD_IF_FALSE   238 (to 846)
-   
-   220         370 LOAD_CONST               0 (0)
-               372 LOAD_CONST              38 (('Tk', 'PhotoImage', 'Label'))
-               374 IMPORT_NAME              5 (tkinter)
-               376 IMPORT_FROM             35 (Tk)
-               378 STORE_NAME              35 (Tk)
-               380 IMPORT_FROM             36 (PhotoImage)
-               382 STORE_NAME              36 (PhotoImage)
-               384 IMPORT_FROM              8 (Label)
-               386 STORE_NAME               8 (Label)
-               388 POP_TOP
-   
-   222         390 PUSH_NULL
-               392 LOAD_NAME               35 (Tk)
-               394 PRECALL                  0
-               398 CALL                     0
-               408 STORE_NAME              37 (root)
-   
-   224         410 PUSH_NULL
-               412 LOAD_NAME                8 (Label)
-               414 PUSH_NULL
-               416 LOAD_NAME               24 (libinfo)
-               418 PRECALL                  0
-               422 CALL                     0
-               432 KW_NAMES                39
-               434 PRECALL                  1
-               438 CALL                     1
-               448 STORE_NAME              38 (info)
-   
-   225         450 LOAD_NAME               38 (info)
-               452 LOAD_METHOD             39 (pack)
-               474 LOAD_CONST              40 ('x')
-               476 LOAD_CONST              41 ('top')
-               478 KW_NAMES                42
-               480 PRECALL                  2
-               484 CALL                     2
-               494 POP_TOP
-   
-   227         496 PUSH_NULL
-               498 LOAD_NAME               33 (Blend2D)
-               500 PRECALL                  0
-               504 CALL                     0
-               514 STORE_NAME              40 (blend2d)
-   
-   229         516 LOAD_NAME               40 (blend2d)
-               518 LOAD_METHOD             41 (create_image_surface)
-               540 LOAD_CONST              43 ((300, 450))
-               542 KW_NAMES                44
-               544 PRECALL                  1
-               548 CALL                     1
-               558 STORE_NAME              42 (surface)
-   
-   234         560 LOAD_CONST               0 (0)
-               562 LOAD_CONST              45 (('fly_local', 'fly_chdir'))
-               564 IMPORT_NAME              0 (tkfly.core)
-               566 IMPORT_FROM              3 (fly_local)
-               568 STORE_NAME               3 (fly_local)
-               570 IMPORT_FROM              4 (fly_chdir)
-               572 STORE_NAME               4 (fly_chdir)
-               574 POP_TOP
-   
-   236         576 LOAD_NAME               40 (blend2d)
-               578 LOAD_METHOD             43 (create_fontface)
-               600 LOAD_CONST              46 ('HarmonyOS_Sans_Medium.ttf')
-               602 KW_NAMES                47
-               604 PRECALL                  1
-               608 CALL                     1
-               618 STORE_NAME              44 (fontface1)
-   
-   237         620 LOAD_NAME               40 (blend2d)
-               622 LOAD_METHOD             45 (create_font)
-               644 LOAD_NAME               44 (fontface1)
-               646 KW_NAMES                48
-               648 PRECALL                  1
-               652 CALL                     1
-               662 STORE_NAME              46 (font1)
-   
-   239         664 LOAD_NAME               42 (surface)
-               666 LOAD_ATTR               42 (surface)
-               676 LOAD_METHOD             47 (fill)
-               698 PUSH_NULL
-               700 LOAD_NAME               20 (circle)
-               702 LOAD_CONST              49 (150)
-               704 LOAD_CONST              50 (225)
-               706 LOAD_CONST              16 (50)
-               708 PRECALL                  3
-               712 CALL                     3
-               722 PUSH_NULL
-               724 LOAD_NAME               17 (color)
-               726 LOAD_CONST              51 ('lightblue')
-               728 PRECALL                  1
-               732 CALL                     1
-               742 PRECALL                  2
-               746 CALL                     2
-               756 POP_TOP
-   
-   241         758 LOAD_NAME               42 (surface)
-               760 LOAD_METHOD             39 (pack)
-               782 LOAD_CONST              52 ('both')
-               784 KW_NAMES                53
-               786 PRECALL                  1
-               790 CALL                     1
-               800 POP_TOP
-   
-   243         802 LOAD_NAME               37 (root)
-               804 LOAD_METHOD             48 (mainloop)
-               826 PRECALL                  0
-               830 CALL                     0
-               840 POP_TOP
-               842 LOAD_CONST              54 (None)
-               844 RETURN_VALUE
+    37         152 LOAD_CONST              18 (<code object rect, file "D:\tkfly\tkfly\blend2d\__init__.py", line 37>)
+               154 MAKE_FUNCTION            0
+               156 STORE_NAME              21 (rect)
+   
+    41         158 LOAD_CONST              63 (('',))
+               160 LOAD_CONST              20 (<code object roundrect, file "D:\tkfly\tkfly\blend2d\__init__.py", line 41>)
+               162 MAKE_FUNCTION            1 (defaults)
+               164 STORE_NAME              22 (roundrect)
+   
+    45         166 LOAD_CONST              63 (('',))
+               168 LOAD_CONST              21 ('string')
+               170 LOAD_NAME               23 (str)
+               172 BUILD_TUPLE              2
+               174 LOAD_CONST              22 (<code object text, file "D:\tkfly\tkfly\blend2d\__init__.py", line 45>)
+               176 MAKE_FUNCTION            5 (defaults, annotations)
+               178 STORE_NAME              24 (text)
+   
+    49         180 LOAD_CONST              23 (<code object classes, file "D:\tkfly\tkfly\blend2d\__init__.py", line 49>)
+               182 MAKE_FUNCTION            0
+               184 STORE_NAME              25 (classes)
+   
+    54         186 LOAD_CONST              24 (<code object libinfo, file "D:\tkfly\tkfly\blend2d\__init__.py", line 54>)
+               188 MAKE_FUNCTION            0
+               190 STORE_NAME              26 (libinfo)
+   
+    59         192 LOAD_CONST              25 (<code object platform, file "D:\tkfly\tkfly\blend2d\__init__.py", line 59>)
+               194 MAKE_FUNCTION            0
+               196 STORE_NAME              27 (platform)
+   
+    64         198 LOAD_CONST              26 (<code object radint_id, file "D:\tkfly\tkfly\blend2d\__init__.py", line 64>)
+               200 MAKE_FUNCTION            0
+               202 STORE_NAME              28 (radint_id)
+   
+    69         204 PUSH_NULL
+               206 LOAD_BUILD_CLASS
+               208 LOAD_CONST              27 (<code object Blend2DImage, file "D:\tkfly\tkfly\blend2d\__init__.py", line 69>)
+               210 MAKE_FUNCTION            0
+               212 LOAD_CONST              28 ('Blend2DImage')
+               214 LOAD_NAME                7 (Image)
+               216 PRECALL                  3
+               220 CALL                     3
+               230 STORE_NAME              29 (Blend2DImage)
+   
+    74         232 PUSH_NULL
+               234 LOAD_BUILD_CLASS
+               236 LOAD_CONST              29 (<code object Surface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 74>)
+               238 MAKE_FUNCTION            0
+               240 LOAD_CONST              30 ('Surface')
+               242 LOAD_NAME               30 (object)
+               244 PRECALL                  3
+               248 CALL                     3
+               258 STORE_NAME              31 (Surface)
+   
+   123         260 PUSH_NULL
+               262 LOAD_BUILD_CLASS
+               264 LOAD_CONST              31 (<code object FontFace, file "D:\tkfly\tkfly\blend2d\__init__.py", line 123>)
+               266 MAKE_FUNCTION            0
+               268 LOAD_CONST              32 ('FontFace')
+               270 LOAD_NAME               30 (object)
+               272 PRECALL                  3
+               276 CALL                     3
+               286 STORE_NAME              32 (FontFace)
+   
+   134         288 PUSH_NULL
+               290 LOAD_BUILD_CLASS
+               292 LOAD_CONST              33 (<code object Font, file "D:\tkfly\tkfly\blend2d\__init__.py", line 134>)
+               294 MAKE_FUNCTION            0
+               296 LOAD_CONST              34 ('Font')
+               298 LOAD_NAME               30 (object)
+               300 PRECALL                  3
+               304 CALL                     3
+               314 STORE_NAME              33 (Font)
+   
+   148         316 PUSH_NULL
+               318 LOAD_BUILD_CLASS
+               320 LOAD_CONST              35 (<code object ImageSurface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 148>)
+               322 MAKE_FUNCTION            0
+               324 LOAD_CONST              36 ('ImageSurface')
+               326 LOAD_NAME                8 (Label)
+               328 PRECALL                  3
+               332 CALL                     3
+               342 STORE_NAME              34 (ImageSurface)
+   
+   172         344 PUSH_NULL
+               346 LOAD_BUILD_CLASS
+               348 LOAD_CONST              37 (<code object Blend2D, file "D:\tkfly\tkfly\blend2d\__init__.py", line 172>)
+               350 MAKE_FUNCTION            0
+               352 LOAD_CONST              38 ('Blend2D')
+               354 LOAD_NAME               30 (object)
+               356 PRECALL                  3
+               360 CALL                     3
+               370 STORE_NAME              35 (Blend2D)
+   
+   238         372 LOAD_NAME               36 (__name__)
+               374 LOAD_CONST              39 ('__main__')
+               376 COMPARE_OP               2 (==)
+               382 EXTENDED_ARG             1
+               384 POP_JUMP_FORWARD_IF_FALSE   287 (to 960)
+   
+   239         386 LOAD_CONST               0 (0)
+               388 LOAD_CONST              40 (('Tk', 'PhotoImage', 'Label'))
+               390 IMPORT_NAME              5 (tkinter)
+               392 IMPORT_FROM             37 (Tk)
+               394 STORE_NAME              37 (Tk)
+               396 IMPORT_FROM             38 (PhotoImage)
+               398 STORE_NAME              38 (PhotoImage)
+               400 IMPORT_FROM              8 (Label)
+               402 STORE_NAME               8 (Label)
+               404 POP_TOP
+   
+   241         406 PUSH_NULL
+               408 LOAD_NAME               37 (Tk)
+               410 PRECALL                  0
+               414 CALL                     0
+               424 STORE_NAME              39 (root)
+   
+   243         426 PUSH_NULL
+               428 LOAD_NAME                8 (Label)
+               430 PUSH_NULL
+               432 LOAD_NAME               26 (libinfo)
+               434 PRECALL                  0
+               438 CALL                     0
+               448 KW_NAMES                41
+               450 PRECALL                  1
+               454 CALL                     1
+               464 STORE_NAME              40 (info)
+   
+   244         466 LOAD_NAME               40 (info)
+               468 LOAD_METHOD             41 (pack)
+               490 LOAD_CONST              42 ('x')
+               492 LOAD_CONST              43 ('top')
+               494 KW_NAMES                44
+               496 PRECALL                  2
+               500 CALL                     2
+               510 POP_TOP
+   
+   246         512 PUSH_NULL
+               514 LOAD_NAME               35 (Blend2D)
+               516 PRECALL                  0
+               520 CALL                     0
+               530 STORE_NAME              42 (blend2d)
+   
+   248         532 LOAD_NAME               42 (blend2d)
+               534 LOAD_METHOD             43 (create_image_surface)
+               556 LOAD_CONST              45 ((300, 450))
+               558 KW_NAMES                46
+               560 PRECALL                  1
+               564 CALL                     1
+               574 STORE_NAME              44 (surface)
+   
+   253         576 LOAD_CONST               0 (0)
+               578 LOAD_CONST              47 (('fly_local', 'fly_chdir'))
+               580 IMPORT_NAME              0 (tkfly.core)
+               582 IMPORT_FROM              3 (fly_local)
+               584 STORE_NAME               3 (fly_local)
+               586 IMPORT_FROM              4 (fly_chdir)
+               588 STORE_NAME               4 (fly_chdir)
+               590 POP_TOP
+   
+   255         592 LOAD_NAME               42 (blend2d)
+               594 LOAD_METHOD             45 (create_fontface)
+               616 LOAD_CONST              48 ('HarmonyOS_Sans_Medium.ttf')
+               618 KW_NAMES                49
+               620 PRECALL                  1
+               624 CALL                     1
+               634 STORE_NAME              46 (fontface1)
+   
+   256         636 LOAD_NAME               42 (blend2d)
+               638 LOAD_METHOD             47 (create_font)
+               660 LOAD_NAME               46 (fontface1)
+               662 KW_NAMES                50
+               664 PRECALL                  1
+               668 CALL                     1
+               678 STORE_NAME              48 (font1)
+   
+   258         680 LOAD_NAME               44 (surface)
+               682 LOAD_ATTR               44 (surface)
+               692 LOAD_METHOD             49 (fill)
+               714 PUSH_NULL
+               716 LOAD_NAME               20 (circle)
+               718 LOAD_CONST              51 (150)
+               720 LOAD_CONST              52 (225)
+               722 LOAD_CONST              16 (50)
+               724 PRECALL                  3
+               728 CALL                     3
+               738 PUSH_NULL
+               740 LOAD_NAME               17 (color)
+               742 LOAD_CONST              53 ('lightblue')
+               744 PRECALL                  1
+               748 CALL                     1
+               758 PRECALL                  2
+               762 CALL                     2
+               772 POP_TOP
+   
+   260         774 LOAD_NAME               44 (surface)
+               776 LOAD_ATTR               44 (surface)
+               786 LOAD_METHOD             49 (fill)
+               808 PUSH_NULL
+               810 LOAD_NAME               22 (roundrect)
+               812 LOAD_CONST              54 (20)
+               814 LOAD_CONST              54 (20)
+               816 LOAD_CONST              55 (100)
+               818 LOAD_CONST              55 (100)
+               820 LOAD_CONST              54 (20)
+               822 PRECALL                  5
+               826 CALL                     5
+               836 PUSH_NULL
+               838 LOAD_NAME               17 (color)
+               840 LOAD_CONST              56 ('orange')
+               842 PRECALL                  1
+               846 CALL                     1
+               856 PRECALL                  2
+               860 CALL                     2
+               870 POP_TOP
+   
+   262         872 LOAD_NAME               44 (surface)
+               874 LOAD_METHOD             41 (pack)
+               896 LOAD_CONST              57 ('both')
+               898 KW_NAMES                58
+               900 PRECALL                  1
+               904 CALL                     1
+               914 POP_TOP
+   
+   264         916 LOAD_NAME               39 (root)
+               918 LOAD_METHOD             50 (mainloop)
+               940 PRECALL                  0
+               944 CALL                     0
+               954 POP_TOP
+               956 LOAD_CONST              59 (None)
+               958 RETURN_VALUE
    
-   219     >>  846 LOAD_CONST              54 (None)
-               848 RETURN_VALUE
+   238     >>  960 LOAD_CONST              59 (None)
+               962 RETURN_VALUE
    consts
       0
       ('fly_load4', 'fly_root', 'fly_local', 'fly_chdir')
       ('Widget', 'Image', 'Label')
       ('Enum',)
       code
          argcount  : 0
@@ -514,22 +549,22 @@
             0000007a00000064027a0000007401000000000000000000007c01a60100
             00ab0100000000000000007a00000064037a000000740100000000000000
             0000007c02a6010000ab0100000000000000007a0000005300
           33           0 RESUME                   0
          
           34           2 LOAD_CONST               1 ('BL::circle {')
                        4 LOAD_GLOBAL              1 (NULL + str)
-                      16 LOAD_FAST                0 (cx)
+                      16 LOAD_FAST                0 (circlex)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 BINARY_OP                0 (+)
                       36 LOAD_CONST               2 (' ')
                       38 BINARY_OP                0 (+)
                       42 LOAD_GLOBAL              1 (NULL + str)
-                      54 LOAD_FAST                1 (cy)
+                      54 LOAD_FAST                1 (circley)
                       56 PRECALL                  1
                       60 CALL                     1
                       70 BINARY_OP                0 (+)
                       74 LOAD_CONST               3 ('} ')
                       76 BINARY_OP                0 (+)
                       80 LOAD_GLOBAL              1 (NULL + str)
                       92 LOAD_FAST                2 (r)
@@ -539,38 +574,158 @@
                      112 RETURN_VALUE
          consts
             None
             'BL::circle {'
             ' '
             '} '
          names      ('str',)
-         varnames   ('cx', 'cy', 'r')
+         varnames   ('circlex', 'circley', 'r')
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'circle'
          firstlineno 33
          lnotab 0x0201
+      code
+         argcount  : 4
+         nlocals   : 4
+         stacksize : 11
+         flags     : 3
+         code
+            0x9700640164027401000000000000000000007c00a6010000ab01000000
+            00000000009b0064027401000000000000000000007c01a6010000ab0100
+            000000000000009b0064027401000000000000000000007c02a6010000ab
+            0100000000000000009b0064027401000000000000000000007c03a60100
+            00ab0100000000000000009b009d087a0000005300
+          37           0 RESUME                   0
+         
+          38           2 LOAD_CONST               1 ('BL::rect')
+                       4 LOAD_CONST               2 (' ')
+                       6 LOAD_GLOBAL              1 (NULL + str)
+                      18 LOAD_FAST                0 (x)
+                      20 PRECALL                  1
+                      24 CALL                     1
+                      34 FORMAT_VALUE             0
+                      36 LOAD_CONST               2 (' ')
+                      38 LOAD_GLOBAL              1 (NULL + str)
+                      50 LOAD_FAST                1 (y)
+                      52 PRECALL                  1
+                      56 CALL                     1
+                      66 FORMAT_VALUE             0
+                      68 LOAD_CONST               2 (' ')
+                      70 LOAD_GLOBAL              1 (NULL + str)
+                      82 LOAD_FAST                2 (width)
+                      84 PRECALL                  1
+                      88 CALL                     1
+                      98 FORMAT_VALUE             0
+                     100 LOAD_CONST               2 (' ')
+                     102 LOAD_GLOBAL              1 (NULL + str)
+                     114 LOAD_FAST                3 (height)
+                     116 PRECALL                  1
+                     120 CALL                     1
+                     130 FORMAT_VALUE             0
+                     132 BUILD_STRING             8
+                     134 BINARY_OP                0 (+)
+                     138 RETURN_VALUE
+         consts
+            None
+            'BL::rect'
+            ' '
+         names      ('str',)
+         varnames   ('x', 'y', 'width', 'height')
+         freevars   ()
+         cellvars   ()
+         filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
+         name       'rect'
+         firstlineno 37
+         lnotab 0x0201
       ''
+      code
+         argcount  : 6
+         nlocals   : 6
+         stacksize : 15
+         flags     : 3
+         code
+            0x9700640164027401000000000000000000007c00a6010000ab01000000
+            00000000009b0064027401000000000000000000007c01a6010000ab0100
+            000000000000009b0064027401000000000000000000007c02a6010000ab
+            0100000000000000009b0064027401000000000000000000007c03a60100
+            00ab0100000000000000009b0064027401000000000000000000007c04a6
+            010000ab0100000000000000009b0064027401000000000000000000007c
+            05a6010000ab0100000000000000009b009d0c7a0000005300
+          41           0 RESUME                   0
+         
+          42           2 LOAD_CONST               1 ('BL::roundrect')
+                       4 LOAD_CONST               2 (' ')
+                       6 LOAD_GLOBAL              1 (NULL + str)
+                      18 LOAD_FAST                0 (x)
+                      20 PRECALL                  1
+                      24 CALL                     1
+                      34 FORMAT_VALUE             0
+                      36 LOAD_CONST               2 (' ')
+                      38 LOAD_GLOBAL              1 (NULL + str)
+                      50 LOAD_FAST                1 (y)
+                      52 PRECALL                  1
+                      56 CALL                     1
+                      66 FORMAT_VALUE             0
+                      68 LOAD_CONST               2 (' ')
+                      70 LOAD_GLOBAL              1 (NULL + str)
+                      82 LOAD_FAST                2 (width)
+                      84 PRECALL                  1
+                      88 CALL                     1
+                      98 FORMAT_VALUE             0
+                     100 LOAD_CONST               2 (' ')
+                     102 LOAD_GLOBAL              1 (NULL + str)
+                     114 LOAD_FAST                3 (height)
+                     116 PRECALL                  1
+                     120 CALL                     1
+                     130 FORMAT_VALUE             0
+                     132 LOAD_CONST               2 (' ')
+                     134 LOAD_GLOBAL              1 (NULL + str)
+                     146 LOAD_FAST                4 (rx)
+                     148 PRECALL                  1
+                     152 CALL                     1
+                     162 FORMAT_VALUE             0
+                     164 LOAD_CONST               2 (' ')
+                     166 LOAD_GLOBAL              1 (NULL + str)
+                     178 LOAD_FAST                5 (ry)
+                     180 PRECALL                  1
+                     184 CALL                     1
+                     194 FORMAT_VALUE             0
+                     196 BUILD_STRING            12
+                     198 BINARY_OP                0 (+)
+                     202 RETURN_VALUE
+         consts
+            None
+            'BL::roundrect'
+            ' '
+         names      ('str',)
+         varnames   ('x', 'y', 'width', 'height', 'rx', 'ry')
+         freevars   ()
+         cellvars   ()
+         filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
+         name       'roundrect'
+         firstlineno 41
+         lnotab 0x0201
       'string'
       code
          argcount  : 4
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
             0x970064017401000000000000000000007c00a6010000ab010000000000
             0000007a00000064027a0000007401000000000000000000007c01a60100
             00ab0100000000000000007a00000064037a000000740100000000000000
             0000007c02a6010000ab0100000000000000007a00000064027a00000064
             047401000000000000000000007c03a6010000ab0100000000000000009b
             0064049d037a0000005300
-          37           0 RESUME                   0
+          45           0 RESUME                   0
          
-          38           2 LOAD_CONST               1 ('BL::text {')
+          46           2 LOAD_CONST               1 ('BL::text {')
                        4 LOAD_GLOBAL              1 (NULL + str)
                       16 LOAD_FAST                0 (cx)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 BINARY_OP                0 (+)
                       36 LOAD_CONST               2 (' ')
                       38 BINARY_OP                0 (+)
@@ -606,34 +761,34 @@
             '"'
          names      ('str',)
          varnames   ('cx', 'cy', 'font', 'string')
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'text'
-         firstlineno 37
+         firstlineno 45
          lnotab 0x0201
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab00000000000000000001
             00740300000000000000000000a6000000ab000000000000000000a00200
             000000000000000000000000000000000000006401a6010000ab01000000
             00000000005300
-          41           0 RESUME                   0
+          49           0 RESUME                   0
          
-          42           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
+          50           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 POP_TOP
          
-          43          30 LOAD_GLOBAL              3 (NULL + fly_root)
+          51          30 LOAD_GLOBAL              3 (NULL + fly_root)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 LOAD_METHOD              2 (call)
                       78 LOAD_CONST               1 ('BL::classes')
                       80 PRECALL                  1
                       84 CALL                     1
                       94 RETURN_VALUE
@@ -642,34 +797,34 @@
             'BL::classes'
          names      ('load_blend2d', 'fly_root', 'call')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'classes'
-         firstlineno 41
+         firstlineno 49
          lnotab 0x02011c01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab00000000000000000001
             00740300000000000000000000a6000000ab000000000000000000a00200
             000000000000000000000000000000000000006401a6010000ab01000000
             00000000005300
-          46           0 RESUME                   0
+          54           0 RESUME                   0
          
-          47           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
+          55           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 POP_TOP
          
-          48          30 LOAD_GLOBAL              3 (NULL + fly_root)
+          56          30 LOAD_GLOBAL              3 (NULL + fly_root)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 LOAD_METHOD              2 (call)
                       78 LOAD_CONST               1 ('BL::libinfo')
                       80 PRECALL                  1
                       84 CALL                     1
                       94 RETURN_VALUE
@@ -678,34 +833,34 @@
             'BL::libinfo'
          names      ('load_blend2d', 'fly_root', 'call')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'libinfo'
-         firstlineno 46
+         firstlineno 54
          lnotab 0x02011c01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab00000000000000000001
             00740300000000000000000000a6000000ab000000000000000000a00200
             000000000000000000000000000000000000006401a6010000ab01000000
             00000000005300
-          51           0 RESUME                   0
+          59           0 RESUME                   0
          
-          52           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
+          60           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 POP_TOP
          
-          53          30 LOAD_GLOBAL              3 (NULL + fly_root)
+          61          30 LOAD_GLOBAL              3 (NULL + fly_root)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 LOAD_METHOD              2 (call)
                       78 LOAD_CONST               1 ('BL::platform')
                       80 PRECALL                  1
                       84 CALL                     1
                       94 RETURN_VALUE
@@ -714,37 +869,39 @@
             'BL::platform'
          names      ('load_blend2d', 'fly_root', 'call')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'platform'
-         firstlineno 51
+         firstlineno 59
          lnotab 0x02011c01
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 7
          flags     : 3
          code
             0x9700640164026c006d017d00010074050000000000000000000002007c
             0064016403a6020000ab02000000000000000002007c0064016403a60200
             00ab0200000000000000007a00000002007c0064016403a6020000ab0200
             000000000000007a00000002007c0064016403a6020000ab020000000000
-            0000007a000000a6010000ab0100000000000000005300
-          56           0 RESUME                   0
+            0000007a00000002007c0064016403a6020000ab0200000000000000007a
+            0a000002007c0064016403a6020000ab0200000000000000007a0a0000a6
+            010000ab0100000000000000005300
+          64           0 RESUME                   0
          
-          57           2 LOAD_CONST               1 (0)
+          65           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('randint',))
                        6 IMPORT_NAME              0 (random)
                        8 IMPORT_FROM              1 (randint)
                       10 STORE_FAST               0 (randint)
                       12 POP_TOP
          
-          58          14 LOAD_GLOBAL              5 (NULL + str)
+          66          14 LOAD_GLOBAL              5 (NULL + str)
                       26 PUSH_NULL
                       28 LOAD_FAST                0 (randint)
                       30 LOAD_CONST               1 (0)
                       32 LOAD_CONST               3 (9999)
                       34 PRECALL                  2
                       38 CALL                     2
                       48 PUSH_NULL
@@ -764,46 +921,60 @@
                      100 PUSH_NULL
                      102 LOAD_FAST                0 (randint)
                      104 LOAD_CONST               1 (0)
                      106 LOAD_CONST               3 (9999)
                      108 PRECALL                  2
                      112 CALL                     2
                      122 BINARY_OP                0 (+)
-                     126 PRECALL                  1
-                     130 CALL                     1
-                     140 RETURN_VALUE
+                     126 PUSH_NULL
+                     128 LOAD_FAST                0 (randint)
+                     130 LOAD_CONST               1 (0)
+                     132 LOAD_CONST               3 (9999)
+                     134 PRECALL                  2
+                     138 CALL                     2
+                     148 BINARY_OP               10 (-)
+                     152 PUSH_NULL
+                     154 LOAD_FAST                0 (randint)
+                     156 LOAD_CONST               1 (0)
+                     158 LOAD_CONST               3 (9999)
+                     160 PRECALL                  2
+                     164 CALL                     2
+                     174 BINARY_OP               10 (-)
+                     178 PRECALL                  1
+                     182 CALL                     1
+                     192 RETURN_VALUE
          consts
             None
             0
             ('randint',)
             9999
          names      ('random', 'randint', 'str')
          varnames   ('randint',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'radint_id'
-         firstlineno 56
+         firstlineno 64
          lnotab 0x02010c01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code 0x970065005a0164005a02690064016602640284015a0364015300
-          61           0 RESUME                   0
+          69           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Blend2DImage')
                        8 STORE_NAME               2 (__qualname__)
          
-          62          10 BUILD_MAP                0
+          70          10 BUILD_MAP                0
                       12 LOAD_CONST               1 (None)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 62>)
+                      16 LOAD_CONST               2 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 70>)
                       18 MAKE_FUNCTION            1 (defaults)
                       20 STORE_NAME               3 (__init__)
                       22 LOAD_CONST               1 (None)
                       24 RETURN_VALUE
          consts
             'Blend2DImage'
             None
@@ -811,17 +982,17 @@
                argcount  : 4
                nlocals   : 5
                stacksize : 6
                flags     : 11
                code
                   0x97007401000000000000000000006a0100000000000000007c0064017c
                   017c02660469007c04a4018e01010064005300
-                62           0 RESUME                   0
+                70           0 RESUME                   0
                
-                63           2 LOAD_GLOBAL              1 (NULL + Image)
+                71           2 LOAD_GLOBAL              1 (NULL + Image)
                             14 LOAD_ATTR                1 (__init__)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_CONST               1 ('blend2d')
                             28 LOAD_FAST                1 (surface)
                             30 LOAD_FAST                2 (cnf)
                             32 BUILD_TUPLE              4
                             34 BUILD_MAP                0
@@ -836,111 +1007,115 @@
                   'blend2d'
                names      ('Image', '__init__')
                varnames   ('self', 'surface', 'cnf', 'master', 'kw')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       '__init__'
-               firstlineno 62
+               firstlineno 70
                lnotab 0x0201
          names      ('__name__', '__module__', '__qualname__', '__init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'Blend2DImage'
-         firstlineno 61
+         firstlineno 69
          lnotab 0x0a01
       'Blend2DImage'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
-            0x970065005a0164005a0264186404650364056504640665046407650566
-            08640884055a0664196404650364056504640665046606640984055a0764
-            1a640b84015a08641b640d65036602640e84055a09640f84005a0a641084
-            005a0b641184005a0c641c641384015a0d641484005a0e641584005a0f64
-            1684005a1064175300
-          66           0 RESUME                   0
+            0x970065005a0164005a0264196404650364056504640665046407650566
+            08640884055a06640984005a07641a640465036405650464066504660664
+            0a84055a08641b640c84015a09641c640e65036602640f84055a0a641084
+            005a0b641184005a0c641284005a0d641d641484015a0e641584005a0f64
+            1684005a10641784005a1164185300
+          74           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Surface')
                        8 STORE_NAME               2 (__qualname__)
          
-          67          10 LOAD_CONST              24 (('.surface', 450, 450, True))
+          75          10 LOAD_CONST              25 (('.surface', 450, 450, True))
                       12 LOAD_CONST               4 ('name')
                       14 LOAD_NAME                3 (str)
                       16 LOAD_CONST               5 ('width')
                       18 LOAD_NAME                4 (int)
                       20 LOAD_CONST               6 ('height')
                       22 LOAD_NAME                4 (int)
                       24 LOAD_CONST               7 ('iscreate')
                       26 LOAD_NAME                5 (bool)
                       28 BUILD_TUPLE              8
-                      30 LOAD_CONST               8 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 67>)
+                      30 LOAD_CONST               8 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 75>)
                       32 MAKE_FUNCTION            5 (defaults, annotations)
                       34 STORE_NAME               6 (__init__)
          
-          73          36 LOAD_CONST              25 (('.surface', 450, 450))
-                      38 LOAD_CONST               4 ('name')
-                      40 LOAD_NAME                3 (str)
-                      42 LOAD_CONST               5 ('width')
-                      44 LOAD_NAME                4 (int)
-                      46 LOAD_CONST               6 ('height')
-                      48 LOAD_NAME                4 (int)
-                      50 BUILD_TUPLE              6
-                      52 LOAD_CONST               9 (<code object create, file "D:\tkfly\tkfly\blend2d\__init__.py", line 73>)
-                      54 MAKE_FUNCTION            5 (defaults, annotations)
-                      56 STORE_NAME               7 (create)
-         
-          76          58 LOAD_CONST              26 (('BL::color black',))
-                      60 LOAD_CONST              11 (<code object clear, file "D:\tkfly\tkfly\blend2d\__init__.py", line 76>)
-                      62 MAKE_FUNCTION            1 (defaults)
-                      64 STORE_NAME               8 (clear)
-         
-          79          66 LOAD_CONST              27 (('surface.bmp',))
-                      68 LOAD_CONST              13 ('file')
-                      70 LOAD_NAME                3 (str)
-                      72 BUILD_TUPLE              2
-                      74 LOAD_CONST              14 (<code object save, file "D:\tkfly\tkfly\blend2d\__init__.py", line 79>)
-                      76 MAKE_FUNCTION            5 (defaults, annotations)
-                      78 STORE_NAME               9 (save)
-         
-          82          80 LOAD_CONST              15 (<code object flush, file "D:\tkfly\tkfly\blend2d\__init__.py", line 82>)
-                      82 MAKE_FUNCTION            0
-                      84 STORE_NAME              10 (flush)
+          81          36 LOAD_CONST               9 (<code object destory, file "D:\tkfly\tkfly\blend2d\__init__.py", line 81>)
+                      38 MAKE_FUNCTION            0
+                      40 STORE_NAME               7 (destory)
+         
+          84          42 LOAD_CONST              26 (('.surface', 450, 450))
+                      44 LOAD_CONST               4 ('name')
+                      46 LOAD_NAME                3 (str)
+                      48 LOAD_CONST               5 ('width')
+                      50 LOAD_NAME                4 (int)
+                      52 LOAD_CONST               6 ('height')
+                      54 LOAD_NAME                4 (int)
+                      56 BUILD_TUPLE              6
+                      58 LOAD_CONST              10 (<code object create, file "D:\tkfly\tkfly\blend2d\__init__.py", line 84>)
+                      60 MAKE_FUNCTION            5 (defaults, annotations)
+                      62 STORE_NAME               8 (create)
+         
+          87          64 LOAD_CONST              27 (('BL::color black',))
+                      66 LOAD_CONST              12 (<code object clear, file "D:\tkfly\tkfly\blend2d\__init__.py", line 87>)
+                      68 MAKE_FUNCTION            1 (defaults)
+                      70 STORE_NAME               9 (clear)
+         
+          90          72 LOAD_CONST              28 (('surface.bmp',))
+                      74 LOAD_CONST              14 ('file')
+                      76 LOAD_NAME                3 (str)
+                      78 BUILD_TUPLE              2
+                      80 LOAD_CONST              15 (<code object save, file "D:\tkfly\tkfly\blend2d\__init__.py", line 90>)
+                      82 MAKE_FUNCTION            5 (defaults, annotations)
+                      84 STORE_NAME              10 (save)
          
-          85          86 LOAD_CONST              16 (<code object reset, file "D:\tkfly\tkfly\blend2d\__init__.py", line 85>)
+          93          86 LOAD_CONST              16 (<code object flush, file "D:\tkfly\tkfly\blend2d\__init__.py", line 93>)
                       88 MAKE_FUNCTION            0
-                      90 STORE_NAME              11 (reset)
+                      90 STORE_NAME              11 (flush)
          
-          88          92 LOAD_CONST              17 (<code object photo, file "D:\tkfly\tkfly\blend2d\__init__.py", line 88>)
+          96          92 LOAD_CONST              17 (<code object reset, file "D:\tkfly\tkfly\blend2d\__init__.py", line 96>)
                       94 MAKE_FUNCTION            0
-                      96 STORE_NAME              12 (photo)
+                      96 STORE_NAME              12 (reset)
          
-          94          98 LOAD_CONST              28 (('BL::color red',))
-                     100 LOAD_CONST              19 (<code object fill, file "D:\tkfly\tkfly\blend2d\__init__.py", line 94>)
-                     102 MAKE_FUNCTION            1 (defaults)
-                     104 STORE_NAME              13 (fill)
-         
-          97         106 LOAD_CONST              20 (<code object size, file "D:\tkfly\tkfly\blend2d\__init__.py", line 97>)
-                     108 MAKE_FUNCTION            0
-                     110 STORE_NAME              14 (size)
+          99          98 LOAD_CONST              18 (<code object photo, file "D:\tkfly\tkfly\blend2d\__init__.py", line 99>)
+                     100 MAKE_FUNCTION            0
+                     102 STORE_NAME              13 (photo)
+         
+         105         104 LOAD_CONST              29 (('BL::color red',))
+                     106 LOAD_CONST              20 (<code object fill, file "D:\tkfly\tkfly\blend2d\__init__.py", line 105>)
+                     108 MAKE_FUNCTION            1 (defaults)
+                     110 STORE_NAME              14 (fill)
          
-         100         112 LOAD_CONST              21 (<code object configure, file "D:\tkfly\tkfly\blend2d\__init__.py", line 100>)
+         108         112 LOAD_CONST              21 (<code object size, file "D:\tkfly\tkfly\blend2d\__init__.py", line 108>)
                      114 MAKE_FUNCTION            0
-                     116 STORE_NAME              15 (configure)
+                     116 STORE_NAME              15 (size)
          
-         107         118 LOAD_CONST              22 (<code object cget, file "D:\tkfly\tkfly\blend2d\__init__.py", line 107>)
+         111         118 LOAD_CONST              22 (<code object configure, file "D:\tkfly\tkfly\blend2d\__init__.py", line 111>)
                      120 MAKE_FUNCTION            0
-                     122 STORE_NAME              16 (cget)
-                     124 LOAD_CONST              23 (None)
-                     126 RETURN_VALUE
+                     122 STORE_NAME              16 (configure)
+         
+         118         124 LOAD_CONST              23 (<code object cget, file "D:\tkfly\tkfly\blend2d\__init__.py", line 118>)
+                     126 MAKE_FUNCTION            0
+                     128 STORE_NAME              17 (cget)
+                     130 LOAD_CONST              24 (None)
+                     132 RETURN_VALUE
          consts
             'Surface'
             '.surface'
             450
             True
             'name'
             'width'
@@ -953,73 +1128,107 @@
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000001
                   007c01740300000000000000000000a6000000ab0000000000000000007a
                   0000007c005f0200000000000000007c04721f7c00a00300000000000000
                   000000000000000000000000007c006a0200000000000000007c027c03ac
                   01a6030000ab03000000000000000001006400530064005300
-                67           0 RESUME                   0
+                75           0 RESUME                   0
                
-                68           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
+                76           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 POP_TOP
                
-                69          30 LOAD_FAST                1 (name)
+                77          30 LOAD_FAST                1 (name)
                             32 LOAD_GLOBAL              3 (NULL + radint_id)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 BINARY_OP                0 (+)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               2 (_name)
                
-                70          74 LOAD_FAST                4 (iscreate)
+                78          74 LOAD_FAST                4 (iscreate)
                             76 POP_JUMP_FORWARD_IF_FALSE    31 (to 140)
                
-                71          78 LOAD_FAST                0 (self)
+                79          78 LOAD_FAST                0 (self)
                             80 LOAD_METHOD              3 (create)
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                2 (_name)
                            114 LOAD_FAST                2 (width)
                            116 LOAD_FAST                3 (height)
                            118 KW_NAMES                 1
                            120 PRECALL                  3
                            124 CALL                     3
                            134 POP_TOP
                            136 LOAD_CONST               0 (None)
                            138 RETURN_VALUE
                
-                70     >>  140 LOAD_CONST               0 (None)
+                78     >>  140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                consts
                   None
                   ('width', 'height')
                names      ('load_blend2d', 'radint_id', '_name', 'create')
                varnames   ('self', 'name', 'width', 'height', 'iscreate')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       '__init__'
-               firstlineno 67
+               firstlineno 75
                lnotab 0x02011c012c0104013eff
             code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 4
+               flags     : 3
+               code
+                  0x9700740100000000000000000000a6000000ab000000000000000000a0
+                  0100000000000000000000000000000000000000007c006a020000000000
+                  0000006401a6020000ab020000000000000000010064005300
+                81           0 RESUME                   0
+               
+                82           2 LOAD_GLOBAL              1 (NULL + fly_root)
+                            14 PRECALL                  0
+                            18 CALL                     0
+                            28 LOAD_METHOD              1 (call)
+                            50 LOAD_FAST                0 (self)
+                            52 LOAD_ATTR                2 (_name)
+                            62 LOAD_CONST               1 ('destory')
+                            64 PRECALL                  2
+                            68 CALL                     2
+                            78 POP_TOP
+                            80 LOAD_CONST               0 (None)
+                            82 RETURN_VALUE
+               consts
+                  None
+                  'destory'
+               names      ('fly_root', 'call', '_name')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
+               name       'destory'
+               firstlineno 81
+               lnotab 0x0201
+            code
                argcount  : 4
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   01000000000000000000000000000000000000000064017c019b0064029d
                   0364037a0000007405000000000000000000007c02a6010000ab01000000
                   00000000007a00000064047a0000007405000000000000000000007c03a6
                   010000ab0100000000000000007a00000064057a000000a6010000ab0100
                   00000000000000010064005300
-                73           0 RESUME                   0
+                84           0 RESUME                   0
                
-                74           2 LOAD_GLOBAL              1 (NULL + fly_root)
+                85           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (eval)
                             50 LOAD_CONST               1 ('BL::Surface create ')
                             52 LOAD_FAST                1 (name)
                             54 FORMAT_VALUE             0
                             56 LOAD_CONST               2 (' -format ')
@@ -1054,30 +1263,30 @@
                   ' }'
                names      ('fly_root', 'eval', 'str')
                varnames   ('self', 'name', 'width', 'height')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create'
-               firstlineno 73
+               firstlineno 84
                lnotab 0x0201
             'BL::color black'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   0100000000000000000000000000000000000000007c006a020000000000
                   0000009b0064017c019b0064029d04a6010000ab01000000000000000001
                   0064005300
-                76           0 RESUME                   0
+                87           0 RESUME                   0
                
-                77           2 LOAD_GLOBAL              1 (NULL + fly_root)
+                88           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (eval)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                2 (_name)
                             62 FORMAT_VALUE             0
                             64 LOAD_CONST               1 (' clear -fill.style [')
@@ -1096,30 +1305,30 @@
                   ']'
                names      ('fly_root', 'eval', '_name')
                varnames   ('self', 'style')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'clear'
-               firstlineno 76
+               firstlineno 87
                lnotab 0x0201
             'surface.bmp'
             'file'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   0100000000000000000000000000000000000000007c006a020000000000
                   00000064017c01a6030000ab030000000000000000010064005300
-                79           0 RESUME                   0
+                90           0 RESUME                   0
                
-                80           2 LOAD_GLOBAL              1 (NULL + fly_root)
+                91           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (call)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                2 (_name)
                             62 LOAD_CONST               1 ('save')
                             64 LOAD_FAST                1 (file)
@@ -1133,28 +1342,28 @@
                   'save'
                names      ('fly_root', 'call', '_name')
                varnames   ('self', 'file')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'save'
-               firstlineno 79
+               firstlineno 90
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   0100000000000000000000000000000000000000007c006a020000000000
                   0000006401a6020000ab020000000000000000010064005300
-                82           0 RESUME                   0
+                93           0 RESUME                   0
                
-                83           2 LOAD_GLOBAL              1 (NULL + fly_root)
+                94           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (call)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                2 (_name)
                             62 LOAD_CONST               1 ('flush')
                             64 PRECALL                  2
@@ -1167,28 +1376,28 @@
                   'flush'
                names      ('fly_root', 'call', '_name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'flush'
-               firstlineno 82
+               firstlineno 93
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   0100000000000000000000000000000000000000007c006a020000000000
                   0000006401a6020000ab020000000000000000010064005300
-                85           0 RESUME                   0
+                96           0 RESUME                   0
                
-                86           2 LOAD_GLOBAL              1 (NULL + fly_root)
+                97           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (call)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                2 (_name)
                             62 LOAD_CONST               1 ('reset')
                             64 PRECALL                  2
@@ -1201,84 +1410,84 @@
                   'reset'
                names      ('fly_root', 'call', '_name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'reset'
-               firstlineno 85
+               firstlineno 96
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x9700640164026c006d017d02010002007c027c01a6010000ab01000000
                   00000000007d03740500000000000000000000a6000000ab000000000000
                   000000a00300000000000000000000000000000000000000007c006a0400
                   0000000000000064037c01a6030000ab03000000000000000001007c0353
                   00
-                88           0 RESUME                   0
+                99           0 RESUME                   0
                
-                89           2 LOAD_CONST               1 (0)
+               100           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('PhotoImage',))
                              6 IMPORT_NAME              0 (tkinter)
                              8 IMPORT_FROM              1 (PhotoImage)
                             10 STORE_FAST               2 (PhotoImage)
                             12 POP_TOP
                
-                90          14 PUSH_NULL
+               101          14 PUSH_NULL
                             16 LOAD_FAST                2 (PhotoImage)
                             18 LOAD_FAST                1 (name)
                             20 PRECALL                  1
                             24 CALL                     1
                             34 STORE_FAST               3 (_photo)
                
-                91          36 LOAD_GLOBAL              5 (NULL + fly_root)
+               102          36 LOAD_GLOBAL              5 (NULL + fly_root)
                             48 PRECALL                  0
                             52 CALL                     0
                             62 LOAD_METHOD              3 (call)
                             84 LOAD_FAST                0 (self)
                             86 LOAD_ATTR                4 (_name)
                             96 LOAD_CONST               3 ('writeToTkphoto')
                             98 LOAD_FAST                1 (name)
                            100 PRECALL                  3
                            104 CALL                     3
                            114 POP_TOP
                
-                92         116 LOAD_FAST                3 (_photo)
+               103         116 LOAD_FAST                3 (_photo)
                            118 RETURN_VALUE
                consts
                   None
                   0
                   ('PhotoImage',)
                   'writeToTkphoto'
                names      ('tkinter', 'PhotoImage', 'fly_root', 'call', '_name')
                varnames   ('self', 'name', 'PhotoImage', '_photo')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'photo'
-               firstlineno 88
+               firstlineno 99
                lnotab 0x02010c0116015001
             'BL::color red'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 8
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   0100000000000000000000000000000000000000007c006a020000000000
                   0000009b0064017c019b0064027c029b0064039d06a6010000ab01000000
                   0000000000010064005300
-                94           0 RESUME                   0
+               105           0 RESUME                   0
                
-                95           2 LOAD_GLOBAL              1 (NULL + fly_root)
+               106           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (eval)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                2 (_name)
                             62 FORMAT_VALUE             0
                             64 LOAD_CONST               1 (' fill [')
@@ -1301,28 +1510,28 @@
                   ']'
                names      ('fly_root', 'eval', '_name')
                varnames   ('self', 'geometry', 'style')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'fill'
-               firstlineno 94
+               firstlineno 105
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   0100000000000000000000000000000000000000007c006a020000000000
                   0000006401a6020000ab0200000000000000005300
-                97           0 RESUME                   0
+               108           0 RESUME                   0
                
-                98           2 LOAD_GLOBAL              1 (NULL + fly_root)
+               109           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (call)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                2 (_name)
                             62 LOAD_CONST               1 ('size')
                             64 PRECALL                  2
@@ -1333,15 +1542,15 @@
                   'size'
                names      ('fly_root', 'call', '_name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'size'
-               firstlineno 97
+               firstlineno 108
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 7
                flags     : 11
                code
@@ -1354,22 +1563,22 @@
                   00000000007d02740100000000000000000000a6000000ab000000000000
                   000000a00100000000000000000000000000000000000000007c006a0200
                   000000000000009b0064059d0264067a0000007409000000000000000000
                   007c02640719000000000000000000a6010000ab0100000000000000007a
                   00000064087a0000007409000000000000000000007c0264091900000000
                   0000000000a6010000ab0100000000000000007a000000640a7a000000a6
                   010000ab01000000000000000001006400530064005300
-               100           0 RESUME                   0
+               111           0 RESUME                   0
                
-               101           2 LOAD_CONST               1 ('fillstyle')
+               112           2 LOAD_CONST               1 ('fillstyle')
                              4 LOAD_FAST                1 (kwargs)
                              6 CONTAINS_OP              0
                              8 POP_JUMP_FORWARD_IF_FALSE    63 (to 136)
                
-               102          10 LOAD_GLOBAL              1 (NULL + fly_root)
+               113          10 LOAD_GLOBAL              1 (NULL + fly_root)
                             22 PRECALL                  0
                             26 CALL                     0
                             36 LOAD_METHOD              1 (eval)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (_name)
                             70 FORMAT_VALUE             0
                             72 LOAD_CONST               2 (' configure -fill.style [')
@@ -1381,27 +1590,27 @@
                            114 FORMAT_VALUE             0
                            116 LOAD_CONST               3 (']')
                            118 BUILD_STRING             4
                            120 PRECALL                  1
                            124 CALL                     1
                            134 POP_TOP
                
-               103     >>  136 LOAD_CONST               4 ('size')
+               114     >>  136 LOAD_CONST               4 ('size')
                            138 LOAD_FAST                1 (kwargs)
                            140 CONTAINS_OP              0
                            142 POP_JUMP_FORWARD_IF_FALSE   117 (to 378)
                
-               104         144 LOAD_FAST                1 (kwargs)
+               115         144 LOAD_FAST                1 (kwargs)
                            146 LOAD_METHOD              3 (pop)
                            168 LOAD_CONST               4 ('size')
                            170 PRECALL                  1
                            174 CALL                     1
                            184 STORE_FAST               2 (size)
                
-               105         186 LOAD_GLOBAL              1 (NULL + fly_root)
+               116         186 LOAD_GLOBAL              1 (NULL + fly_root)
                            198 PRECALL                  0
                            202 CALL                     0
                            212 LOAD_METHOD              1 (eval)
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                2 (_name)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               5 (' configure -format ')
@@ -1428,15 +1637,15 @@
                            354 BINARY_OP                0 (+)
                            358 PRECALL                  1
                            362 CALL                     1
                            372 POP_TOP
                            374 LOAD_CONST               0 (None)
                            376 RETURN_VALUE
                
-               103     >>  378 LOAD_CONST               0 (None)
+               114     >>  378 LOAD_CONST               0 (None)
                            380 RETURN_VALUE
                consts
                   None
                   'fillstyle'
                   ' configure -fill.style ['
                   ']'
                   'size'
@@ -1448,113 +1657,113 @@
                   ' }'
                names      ('fly_root', 'eval', '_name', 'pop', 'str')
                varnames   ('self', 'kwargs', 'size')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'configure'
-               firstlineno 100
+               firstlineno 111
                lnotab 0x020108017e0108012a01c0fe
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c0164016b02000000007229740100000000000000000000a60000
                   00ab000000000000000000a0010000000000000000000000000000000000
                   0000007c006a0200000000000000009b0064029d02a6010000ab01000000
                   0000000000530064005300
-               107           0 RESUME                   0
+               118           0 RESUME                   0
                
-               108           2 LOAD_FAST                1 (optionName)
+               119           2 LOAD_FAST                1 (optionName)
                              4 LOAD_CONST               1 ('fillstyle')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE    41 (to 96)
                
-               109          14 LOAD_GLOBAL              1 (NULL + fly_root)
+               120          14 LOAD_GLOBAL              1 (NULL + fly_root)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 LOAD_METHOD              1 (eval)
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                2 (_name)
                             74 FORMAT_VALUE             0
                             76 LOAD_CONST               2 (' cget -fill.style')
                             78 BUILD_STRING             2
                             80 PRECALL                  1
                             84 CALL                     1
                             94 RETURN_VALUE
                
-               108     >>   96 LOAD_CONST               0 (None)
+               119     >>   96 LOAD_CONST               0 (None)
                             98 RETURN_VALUE
                consts
                   None
                   'fillstyle'
                   ' cget -fill.style'
                names      ('fly_root', 'eval', '_name')
                varnames   ('self', 'optionName')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'cget'
-               firstlineno 107
+               firstlineno 118
                lnotab 0x02010c0152ff
             None
             ('.surface', 450, 450, True)
             ('.surface', 450, 450)
             ('BL::color black',)
             ('surface.bmp',)
             ('BL::color red',)
-         names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'bool', '__init__', 'create', 'clear', 'save', 'flush', 'reset', 'photo', 'fill', 'size', 'configure', 'cget')
+         names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'bool', '__init__', 'destory', 'create', 'clear', 'save', 'flush', 'reset', 'photo', 'fill', 'size', 'configure', 'cget')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'Surface'
-         firstlineno 66
-         lnotab 0x0a011a06160308030e03060306030606080306030607
+         firstlineno 74
+         lnotab 0x0a011a060603160308030e03060306030606080306030607
       'Surface'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02640c6404650364056504640665036407650566
             08640884055a06640d6404650364056504640665036606640a84055a0764
             0b5300
-         112           0 RESUME                   0
+         123           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('FontFace')
                        8 STORE_NAME               2 (__qualname__)
          
-         113          10 LOAD_CONST              12 ((145, '.fontface', True))
+         124          10 LOAD_CONST              12 ((145, '.fontface', True))
                       12 LOAD_CONST               4 ('fontfile')
                       14 LOAD_NAME                3 (str)
                       16 LOAD_CONST               5 ('faceIdxL')
                       18 LOAD_NAME                4 (int)
                       20 LOAD_CONST               6 ('name')
                       22 LOAD_NAME                3 (str)
                       24 LOAD_CONST               7 ('iscreate')
                       26 LOAD_NAME                5 (bool)
                       28 BUILD_TUPLE              8
-                      30 LOAD_CONST               8 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 113>)
+                      30 LOAD_CONST               8 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 124>)
                       32 MAKE_FUNCTION            5 (defaults, annotations)
                       34 STORE_NAME               6 (__init__)
          
-         119          36 LOAD_CONST              13 (('.surface',))
+         130          36 LOAD_CONST              13 (('.surface',))
                       38 LOAD_CONST               4 ('fontfile')
                       40 LOAD_NAME                3 (str)
                       42 LOAD_CONST               5 ('faceIdxL')
                       44 LOAD_NAME                4 (int)
                       46 LOAD_CONST               6 ('name')
                       48 LOAD_NAME                3 (str)
                       50 BUILD_TUPLE              6
-                      52 LOAD_CONST              10 (<code object create, file "D:\tkfly\tkfly\blend2d\__init__.py", line 119>)
+                      52 LOAD_CONST              10 (<code object create, file "D:\tkfly\tkfly\blend2d\__init__.py", line 130>)
                       54 MAKE_FUNCTION            5 (defaults, annotations)
                       56 STORE_NAME               7 (create)
                       58 LOAD_CONST              11 (None)
                       60 RETURN_VALUE
          consts
             'FontFace'
             145
@@ -1571,72 +1780,72 @@
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000001
                   007c03740300000000000000000000a6000000ab0000000000000000007a
                   0000007c005f0200000000000000007c04721f7c00a00300000000000000
                   000000000000000000000000007c006a0200000000000000007c017c02ac
                   01a6030000ab03000000000000000001006400530064005300
-               113           0 RESUME                   0
+               124           0 RESUME                   0
                
-               114           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
+               125           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 POP_TOP
                
-               115          30 LOAD_FAST                3 (name)
+               126          30 LOAD_FAST                3 (name)
                             32 LOAD_GLOBAL              3 (NULL + radint_id)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 BINARY_OP                0 (+)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               2 (_name)
                
-               116          74 LOAD_FAST                4 (iscreate)
+               127          74 LOAD_FAST                4 (iscreate)
                             76 POP_JUMP_FORWARD_IF_FALSE    31 (to 140)
                
-               117          78 LOAD_FAST                0 (self)
+               128          78 LOAD_FAST                0 (self)
                             80 LOAD_METHOD              3 (create)
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                2 (_name)
                            114 LOAD_FAST                1 (fontfile)
                            116 LOAD_FAST                2 (faceIdxL)
                            118 KW_NAMES                 1
                            120 PRECALL                  3
                            124 CALL                     3
                            134 POP_TOP
                            136 LOAD_CONST               0 (None)
                            138 RETURN_VALUE
                
-               116     >>  140 LOAD_CONST               0 (None)
+               127     >>  140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                consts
                   None
                   ('name', 'fontfile', 'faceIdxL')
                names      ('load_blend2d', 'radint_id', '_name', 'create')
                varnames   ('self', 'fontfile', 'faceIdxL', 'name', 'iscreate')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       '__init__'
-               firstlineno 113
+               firstlineno 124
                lnotab 0x02011c012c0104013eff
             '.surface'
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 8
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   01000000000000000000000000000000000000000064017c039b0064027c
                   019b0064037c029b009d06a6010000ab0100000000000000000100640053
                   00
-               119           0 RESUME                   0
+               130           0 RESUME                   0
                
-               120           2 LOAD_GLOBAL              1 (NULL + fly_root)
+               131           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (eval)
                             50 LOAD_CONST               1 ('BL::FontFace create ')
                             52 LOAD_FAST                3 (name)
                             54 FORMAT_VALUE             0
                             56 LOAD_CONST               2 (' "')
@@ -1658,70 +1867,70 @@
                   '" '
                names      ('fly_root', 'eval')
                varnames   ('self', 'fontfile', 'faceIdxL', 'name')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create'
-               firstlineno 119
+               firstlineno 130
                lnotab 0x0201
             None
             (145, '.fontface', True)
             ('.surface',)
          names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'bool', '__init__', 'create')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'FontFace'
-         firstlineno 112
+         firstlineno 123
          lnotab 0x0a011a06
       'FontFace'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02640d6404650364056504640665056407650666
             08640884055a07640e6404650364066505640565046606640a84055a0864
             0b84005a09640c5300
-         123           0 RESUME                   0
+         134           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Font')
                        8 STORE_NAME               2 (__qualname__)
          
-         124          10 LOAD_CONST              13 ((12, '.font', True))
+         135          10 LOAD_CONST              13 ((12, '.font', True))
                       12 LOAD_CONST               4 ('fontface')
                       14 LOAD_NAME                3 (FontFace)
                       16 LOAD_CONST               5 ('fontsize')
                       18 LOAD_NAME                4 (int)
                       20 LOAD_CONST               6 ('name')
                       22 LOAD_NAME                5 (str)
                       24 LOAD_CONST               7 ('iscreate')
                       26 LOAD_NAME                6 (bool)
                       28 BUILD_TUPLE              8
-                      30 LOAD_CONST               8 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 124>)
+                      30 LOAD_CONST               8 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 135>)
                       32 MAKE_FUNCTION            5 (defaults, annotations)
                       34 STORE_NAME               7 (__init__)
          
-         130          36 LOAD_CONST              14 (('.surface', 12))
+         141          36 LOAD_CONST              14 (('.surface', 12))
                       38 LOAD_CONST               4 ('fontface')
                       40 LOAD_NAME                3 (FontFace)
                       42 LOAD_CONST               6 ('name')
                       44 LOAD_NAME                5 (str)
                       46 LOAD_CONST               5 ('fontsize')
                       48 LOAD_NAME                4 (int)
                       50 BUILD_TUPLE              6
-                      52 LOAD_CONST              10 (<code object create, file "D:\tkfly\tkfly\blend2d\__init__.py", line 130>)
+                      52 LOAD_CONST              10 (<code object create, file "D:\tkfly\tkfly\blend2d\__init__.py", line 141>)
                       54 MAKE_FUNCTION            5 (defaults, annotations)
                       56 STORE_NAME               8 (create)
          
-         133          58 LOAD_CONST              11 (<code object names, file "D:\tkfly\tkfly\blend2d\__init__.py", line 133>)
+         144          58 LOAD_CONST              11 (<code object names, file "D:\tkfly\tkfly\blend2d\__init__.py", line 144>)
                       60 MAKE_FUNCTION            0
                       62 STORE_NAME               9 (names)
                       64 LOAD_CONST              12 (None)
                       66 RETURN_VALUE
          consts
             'Font'
             12
@@ -1738,72 +1947,72 @@
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000001
                   007c03740300000000000000000000a6000000ab0000000000000000007a
                   0000007c005f0200000000000000007c04721f7c00a00300000000000000
                   000000000000000000000000007c006a0200000000000000007c017c02ac
                   01a6030000ab03000000000000000001006400530064005300
-               124           0 RESUME                   0
+               135           0 RESUME                   0
                
-               125           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
+               136           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 POP_TOP
                
-               126          30 LOAD_FAST                3 (name)
+               137          30 LOAD_FAST                3 (name)
                             32 LOAD_GLOBAL              3 (NULL + radint_id)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 BINARY_OP                0 (+)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               2 (_name)
                
-               127          74 LOAD_FAST                4 (iscreate)
+               138          74 LOAD_FAST                4 (iscreate)
                             76 POP_JUMP_FORWARD_IF_FALSE    31 (to 140)
                
-               128          78 LOAD_FAST                0 (self)
+               139          78 LOAD_FAST                0 (self)
                             80 LOAD_METHOD              3 (create)
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                2 (_name)
                            114 LOAD_FAST                1 (fontface)
                            116 LOAD_FAST                2 (fontsize)
                            118 KW_NAMES                 1
                            120 PRECALL                  3
                            124 CALL                     3
                            134 POP_TOP
                            136 LOAD_CONST               0 (None)
                            138 RETURN_VALUE
                
-               127     >>  140 LOAD_CONST               0 (None)
+               138     >>  140 LOAD_CONST               0 (None)
                            142 RETURN_VALUE
                consts
                   None
                   ('name', 'fontface', 'fontsize')
                names      ('load_blend2d', 'radint_id', '_name', 'create')
                varnames   ('self', 'fontface', 'fontsize', 'name', 'iscreate')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       '__init__'
-               firstlineno 124
+               firstlineno 135
                lnotab 0x02011c012c0104013eff
             '.surface'
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 8
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   01000000000000000000000000000000000000000064017c029b0064027c
                   019b0064027c039b009d06a6010000ab0100000000000000000100640053
                   00
-               130           0 RESUME                   0
+               141           0 RESUME                   0
                
-               131           2 LOAD_GLOBAL              1 (NULL + fly_root)
+               142           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (eval)
                             50 LOAD_CONST               1 ('BL::Font create ')
                             52 LOAD_FAST                2 (name)
                             54 FORMAT_VALUE             0
                             56 LOAD_CONST               2 (' ')
@@ -1824,28 +2033,28 @@
                   ' '
                names      ('fly_root', 'eval')
                varnames   ('self', 'fontface', 'name', 'fontsize')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create'
-               firstlineno 130
+               firstlineno 141
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab000000000000000000a0
                   01000000000000000000000000000000000000000064016402a6020000ab
                   0200000000000000005300
-               133           0 RESUME                   0
+               144           0 RESUME                   0
                
-               134           2 LOAD_GLOBAL              1 (NULL + fly_root)
+               145           2 LOAD_GLOBAL              1 (NULL + fly_root)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_METHOD              1 (call)
                             50 LOAD_CONST               1 ('BL::Font')
                             52 LOAD_CONST               2 ('names')
                             54 PRECALL                  2
                             58 CALL                     2
@@ -1856,46 +2065,46 @@
                   'names'
                names      ('fly_root', 'call')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'names'
-               firstlineno 133
+               firstlineno 144
                lnotab 0x0201
             None
             (12, '.font', True)
             ('.surface', 12)
          names      ('__name__', '__module__', '__qualname__', 'FontFace', 'int', 'str', 'bool', '__init__', 'create', 'names')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'Font'
-         firstlineno 123
+         firstlineno 134
          lnotab 0x0a011a061603
       'Font'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x8700970065005a0164005a026401640264036403640464059c05640665
             0364076503640865046606880066016409840e5a05640a84005a06880078
             015a075300
                        0 MAKE_CELL                0 (__class__)
          
-         137           2 RESUME                   0
+         148           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ImageSurface')
                       10 STORE_NAME               2 (__qualname__)
          
-         138          12 LOAD_CONST               1 ('.surface.image')
+         149          12 LOAD_CONST               1 ('.surface.image')
                       14 LOAD_CONST               2 ('.surface.image.image')
                       16 LOAD_CONST               3 (450)
                       18 LOAD_CONST               3 (450)
                       20 LOAD_CONST               4 (True)
                       22 LOAD_CONST               5 (('name', 'image_name', 'width', 'height', 'iscreate'))
                       24 BUILD_CONST_KEY_MAP      5
                       26 LOAD_CONST               6 ('width')
@@ -1903,19 +2112,19 @@
                       30 LOAD_CONST               7 ('height')
                       32 LOAD_NAME                3 (int)
                       34 LOAD_CONST               8 ('iscreate')
                       36 LOAD_NAME                4 (bool)
                       38 BUILD_TUPLE              6
                       40 LOAD_CLOSURE             0 (__class__)
                       42 BUILD_TUPLE              1
-                      44 LOAD_CONST               9 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 138>)
+                      44 LOAD_CONST               9 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 149>)
                       46 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
                       48 STORE_NAME               5 (__init__)
          
-         152          50 LOAD_CONST              10 (<code object update_image, file "D:\tkfly\tkfly\blend2d\__init__.py", line 152>)
+         163          50 LOAD_CONST              10 (<code object update_image, file "D:\tkfly\tkfly\blend2d\__init__.py", line 163>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME               6 (update_image)
                       56 LOAD_CLOSURE             0 (__class__)
                       58 COPY                     1
                       60 STORE_NAME               7 (__classcell__)
                       62 RETURN_VALUE
          consts
@@ -1948,90 +2157,90 @@
                   0000000000000000000000000000000000000064038800660164048408a6
                   020000ab02000000000000000001008900a00a0000000000000000000000
                   00000000000000000064058800660164068408a6020000ab020000000000
                   000000010064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (self)
                
-               138           4 RESUME                   0
+               149           4 RESUME                   0
                
-               139           6 LOAD_GLOBAL              1 (NULL + Surface)
+               150           6 LOAD_GLOBAL              1 (NULL + Surface)
                             18 LOAD_FAST                1 (name)
                             20 LOAD_FAST                5 (iscreate)
                             22 LOAD_FAST                3 (width)
                             24 LOAD_FAST                4 (height)
                             26 KW_NAMES                 1
                             28 PRECALL                  4
                             32 CALL                     4
                             42 LOAD_DEREF               0 (self)
                             44 STORE_ATTR               1 (surface)
                
-               140          54 LOAD_DEREF               0 (self)
+               151          54 LOAD_DEREF               0 (self)
                             56 LOAD_ATTR                1 (surface)
                             66 LOAD_METHOD              2 (clear)
                             88 PRECALL                  0
                             92 CALL                     0
                            102 POP_TOP
                
-               142         104 LOAD_FAST                2 (image_name)
+               153         104 LOAD_FAST                2 (image_name)
                            106 LOAD_GLOBAL              7 (NULL + radint_id)
                            118 PRECALL                  0
                            122 CALL                     0
                            132 BINARY_OP                0 (+)
                            136 LOAD_DEREF               0 (self)
                            138 STORE_ATTR               4 (image_name)
                
-               144         148 PUSH_NULL
+               155         148 PUSH_NULL
                            150 LOAD_GLOBAL             11 (NULL + super)
                            162 PRECALL                  0
                            166 CALL                     0
                            176 LOAD_ATTR                6 (__init__)
                            186 LOAD_FAST                6 (args)
                            188 BUILD_MAP                0
                            190 LOAD_FAST                7 (kwargs)
                            192 DICT_MERGE               1
                            194 CALL_FUNCTION_EX         1
                            196 POP_TOP
                
-               146         198 LOAD_DEREF               0 (self)
+               157         198 LOAD_DEREF               0 (self)
                            200 LOAD_ATTR                1 (surface)
                            210 LOAD_METHOD              7 (photo)
                            232 LOAD_DEREF               0 (self)
                            234 LOAD_ATTR                4 (image_name)
                            244 PRECALL                  1
                            248 CALL                     1
                            258 LOAD_DEREF               0 (self)
                            260 STORE_ATTR               8 (image)
                
-               147         270 LOAD_DEREF               0 (self)
+               158         270 LOAD_DEREF               0 (self)
                            272 LOAD_METHOD              9 (configure)
                            294 LOAD_DEREF               0 (self)
                            296 LOAD_ATTR                8 (image)
                            306 KW_NAMES                 2
                            308 PRECALL                  1
                            312 CALL                     1
                            322 POP_TOP
                
-               149         324 LOAD_DEREF               0 (self)
+               160         324 LOAD_DEREF               0 (self)
                            326 LOAD_METHOD             10 (bind)
                            348 LOAD_CONST               3 ('<Map>')
                            350 LOAD_CLOSURE             0 (self)
                            352 BUILD_TUPLE              1
-                           354 LOAD_CONST               4 (<code object <lambda>, file "D:\tkfly\tkfly\blend2d\__init__.py", line 149>)
+                           354 LOAD_CONST               4 (<code object <lambda>, file "D:\tkfly\tkfly\blend2d\__init__.py", line 160>)
                            356 MAKE_FUNCTION            8 (closure)
                            358 PRECALL                  2
                            362 CALL                     2
                            372 POP_TOP
                
-               150         374 LOAD_DEREF               0 (self)
+               161         374 LOAD_DEREF               0 (self)
                            376 LOAD_METHOD             10 (bind)
                            398 LOAD_CONST               5 ('<Configure>')
                            400 LOAD_CLOSURE             0 (self)
                            402 BUILD_TUPLE              1
-                           404 LOAD_CONST               6 (<code object <lambda>, file "D:\tkfly\tkfly\blend2d\__init__.py", line 150>)
+                           404 LOAD_CONST               6 (<code object <lambda>, file "D:\tkfly\tkfly\blend2d\__init__.py", line 161>)
                            406 MAKE_FUNCTION            8 (closure)
                            408 PRECALL                  2
                            412 CALL                     2
                            422 POP_TOP
                            424 LOAD_CONST               0 (None)
                            426 RETURN_VALUE
                consts
@@ -2045,64 +2254,64 @@
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     149           2 RESUME                   0
+                     160           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (update_image)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('update_image',)
                      varnames   ('_',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                      name       '<lambda>'
-                     firstlineno 149
+                     firstlineno 160
                      lnotab 0x
                   '<Configure>'
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     150           2 RESUME                   0
+                     161           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (update_image)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('update_image',)
                      varnames   ('_',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                      name       '<lambda>'
-                     firstlineno 150
+                     firstlineno 161
                      lnotab 0x
                names      ('Surface', 'surface', 'clear', 'radint_id', 'image_name', 'super', '__init__', 'photo', 'image', 'configure', 'bind')
                varnames   ('self', 'name', 'image_name', 'width', 'height', 'iscreate', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ('self',)
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       '__init__'
-               firstlineno 138
+               firstlineno 149
                lnotab 0x0601300132022c023202480136023201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
@@ -2110,354 +2319,386 @@
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000001007c006a020000000000000000a0040000000000000000000000
                   0000000000000000007c006a05000000000000000064037a000000740d00
                   000000000000000000a6000000ab0000000000000000007a000000a60100
                   00ab0100000000000000007d027c027c005f0700000000000000007c00a0
                   0800000000000000000000000000000000000000007c02ac04a6010000ab
                   01000000000000000001007c025300
-               152           0 RESUME                   0
+               163           0 RESUME                   0
                
-               153           2 LOAD_CONST               1 (0)
+               164           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('randint',))
                              6 IMPORT_NAME              0 (random)
                              8 IMPORT_FROM              1 (randint)
                             10 STORE_FAST               1 (randint)
                             12 POP_TOP
                
-               154          14 LOAD_FAST                0 (self)
+               165          14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                2 (surface)
                             26 LOAD_METHOD              3 (flush)
                             48 PRECALL                  0
                             52 CALL                     0
                             62 POP_TOP
                
-               155          64 LOAD_FAST                0 (self)
+               166          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                2 (surface)
                             76 LOAD_METHOD              4 (photo)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                5 (image_name)
                            110 LOAD_CONST               3 ('.')
                            112 BINARY_OP                0 (+)
                            116 LOAD_GLOBAL             13 (NULL + radint_id)
                            128 PRECALL                  0
                            132 CALL                     0
                            142 BINARY_OP                0 (+)
                            146 PRECALL                  1
                            150 CALL                     1
                            160 STORE_FAST               2 (image)
                
-               156         162 LOAD_FAST                2 (image)
+               167         162 LOAD_FAST                2 (image)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR               7 (image)
                
-               157         176 LOAD_FAST                0 (self)
+               168         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD              8 (configure)
                            200 LOAD_FAST                2 (image)
                            202 KW_NAMES                 4
                            204 PRECALL                  1
                            208 CALL                     1
                            218 POP_TOP
                
-               158         220 LOAD_FAST                2 (image)
+               169         220 LOAD_FAST                2 (image)
                            222 RETURN_VALUE
                consts
                   None
                   0
                   ('randint',)
                   '.'
                   ('image',)
                names      ('random', 'randint', 'surface', 'flush', 'photo', 'image_name', 'radint_id', 'image', 'configure')
                varnames   ('self', 'randint', 'image')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'update_image'
-               firstlineno 152
+               firstlineno 163
                lnotab 0x02010c01320162010e012c01
          names      ('__name__', '__module__', '__qualname__', 'int', 'bool', '__init__', 'update_image', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'ImageSurface'
-         firstlineno 137
+         firstlineno 148
          lnotab 0x0c01260e
       'ImageSurface'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
          code
-            0x970065005a0164005a02640184005a0365046426640565056406650564
-            076506660664088405a6000000ab0000000000000000005a076504642764
+            0x970065005a0164005a02640184005a0365046428640565056406650564
+            076506660664088405a6000000ab0000000000000000005a076504642964
             056505640b6508640c65066606640d8405a6000000ab0000000000000000
-            005a0965046428640565056410650a660464118405a6000000ab00000000
-            00000000005a0b6504642964056505641365056410650a660664148405a6
-            000000ab0000000000000000005a0c6504642a6417650a64106506700165
-            0d660464188405a6000000ab0000000000000000005a0e6504642b641765
-            0a641a650f641b65056606641c8405a6000000ab0000000000000000005a
-            106504642c641f650d660264208405a6000000ab0000000000000000005a
-            116504642d6422650a641f650d660464238405a6000000ab000000000000
-            0000005a12651364248400a6000000ab0000000000000000005a14651364
-            258400a6000000ab0000000000000000005a1564035300
-         161           0 RESUME                   0
+            005a096504642a640565056410650a660464118405a6000000ab00000000
+            00000000005a0b6504642b64056505641365056410650a660664148405a6
+            000000ab0000000000000000005a0c6504642c64168401a6000000ab0000
+            000000000000005a0d650464178400a6000000ab0000000000000000005a
+            0e6504642d641a650a641065067001650f6604641b8405a6000000ab0000
+            000000000000005a106504642e641a650a641c6511641d65056606641e84
+            05a6000000ab0000000000000000005a126504642f6421650f6602642284
+            05a6000000ab0000000000000000005a13650464306424650a6421650f66
+            0464258405a6000000ab0000000000000000005a14651564268400a60000
+            00ab0000000000000000005a16651564278400a6000000ab000000000000
+            0000005a1764035300
+         172           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Blend2D')
                        8 STORE_NAME               2 (__qualname__)
          
-         162          10 LOAD_CONST               1 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 162>)
+         173          10 LOAD_CONST               1 (<code object __init__, file "D:\tkfly\tkfly\blend2d\__init__.py", line 173>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-         169          16 LOAD_NAME                4 (staticmethod)
+         180          16 LOAD_NAME                4 (staticmethod)
          
-         170          18 LOAD_CONST              38 (('.fontface', None, 100))
+         181          18 LOAD_CONST              40 (('.fontface', None, 100))
                       20 LOAD_CONST               5 ('name')
                       22 LOAD_NAME                5 (str)
                       24 LOAD_CONST               6 ('fontfile')
                       26 LOAD_NAME                5 (str)
                       28 LOAD_CONST               7 ('id')
                       30 LOAD_NAME                6 (int)
                       32 BUILD_TUPLE              6
-                      34 LOAD_CONST               8 (<code object create_fontface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 169>)
+                      34 LOAD_CONST               8 (<code object create_fontface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 180>)
                       36 MAKE_FUNCTION            5 (defaults, annotations)
          
-         169          38 PRECALL                  0
+         180          38 PRECALL                  0
                       42 CALL                     0
          
-         170          52 STORE_NAME               7 (create_fontface)
+         181          52 STORE_NAME               7 (create_fontface)
          
-         173          54 LOAD_NAME                4 (staticmethod)
+         184          54 LOAD_NAME                4 (staticmethod)
          
-         174          56 LOAD_CONST              39 (('.font', None, 12))
+         185          56 LOAD_CONST              41 (('.font', None, 12))
                       58 LOAD_CONST               5 ('name')
                       60 LOAD_NAME                5 (str)
                       62 LOAD_CONST              11 ('fontface')
                       64 LOAD_NAME                8 (FontFace)
                       66 LOAD_CONST              12 ('fontsize')
                       68 LOAD_NAME                6 (int)
                       70 BUILD_TUPLE              6
-                      72 LOAD_CONST              13 (<code object create_font, file "D:\tkfly\tkfly\blend2d\__init__.py", line 173>)
+                      72 LOAD_CONST              13 (<code object create_font, file "D:\tkfly\tkfly\blend2d\__init__.py", line 184>)
                       74 MAKE_FUNCTION            5 (defaults, annotations)
          
-         173          76 PRECALL                  0
+         184          76 PRECALL                  0
                       80 CALL                     0
          
-         174          90 STORE_NAME               9 (create_font)
+         185          90 STORE_NAME               9 (create_font)
          
-         177          92 LOAD_NAME                4 (staticmethod)
+         188          92 LOAD_NAME                4 (staticmethod)
          
-         178          94 LOAD_CONST              40 (('.surface', (450, 450)))
+         189          94 LOAD_CONST              42 (('.surface', (450, 450)))
                       96 LOAD_CONST               5 ('name')
                       98 LOAD_NAME                5 (str)
                      100 LOAD_CONST              16 ('size')
                      102 LOAD_NAME               10 (tuple)
                      104 BUILD_TUPLE              4
-                     106 LOAD_CONST              17 (<code object create_surface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 177>)
+                     106 LOAD_CONST              17 (<code object create_surface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 188>)
                      108 MAKE_FUNCTION            5 (defaults, annotations)
          
-         177         110 PRECALL                  0
+         188         110 PRECALL                  0
                      114 CALL                     0
          
-         178         124 STORE_NAME              11 (create_surface)
+         189         124 STORE_NAME              11 (create_surface)
          
-         181         126 LOAD_NAME                4 (staticmethod)
+         192         126 LOAD_NAME                4 (staticmethod)
          
-         182         128 LOAD_CONST              41 (('.surface', '.surface.image', (450, 450)))
+         193         128 LOAD_CONST              43 (('.surface', '.surface.image', (450, 450)))
                      130 LOAD_CONST               5 ('name')
                      132 LOAD_NAME                5 (str)
                      134 LOAD_CONST              19 ('image_name')
                      136 LOAD_NAME                5 (str)
                      138 LOAD_CONST              16 ('size')
                      140 LOAD_NAME               10 (tuple)
                      142 BUILD_TUPLE              6
-                     144 LOAD_CONST              20 (<code object create_image_surface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 181>)
+                     144 LOAD_CONST              20 (<code object create_image_surface, file "D:\tkfly\tkfly\blend2d\__init__.py", line 192>)
                      146 MAKE_FUNCTION            5 (defaults, annotations)
          
-         181         148 PRECALL                  0
+         192         148 PRECALL                  0
                      152 CALL                     0
          
-         182         162 STORE_NAME              12 (create_image_surface)
+         193         162 STORE_NAME              12 (create_image_surface)
+         
+         196         164 LOAD_NAME                4 (staticmethod)
+         
+         197         166 LOAD_CONST              44 (('',))
+                     168 LOAD_CONST              22 (<code object create_roundrect, file "D:\tkfly\tkfly\blend2d\__init__.py", line 196>)
+                     170 MAKE_FUNCTION            1 (defaults)
+         
+         196         172 PRECALL                  0
+                     176 CALL                     0
+         
+         197         186 STORE_NAME              13 (create_roundrect)
          
-         185         164 LOAD_NAME                4 (staticmethod)
+         200         188 LOAD_NAME                4 (staticmethod)
          
-         186         166 LOAD_CONST              42 (((0, 0), 40))
-                     168 LOAD_CONST              23 ('pos')
-                     170 LOAD_NAME               10 (tuple)
-                     172 LOAD_CONST              16 ('size')
-                     174 LOAD_NAME                6 (int)
-                     176 JUMP_IF_TRUE_OR_POP      1 (to 180)
-                     178 LOAD_NAME               13 (float)
-                 >>  180 BUILD_TUPLE              4
-                     182 LOAD_CONST              24 (<code object create_circle, file "D:\tkfly\tkfly\blend2d\__init__.py", line 185>)
-                     184 MAKE_FUNCTION            5 (defaults, annotations)
+         201         190 LOAD_CONST              23 (<code object create_rect, file "D:\tkfly\tkfly\blend2d\__init__.py", line 200>)
+                     192 MAKE_FUNCTION            0
          
-         185         186 PRECALL                  0
-                     190 CALL                     0
+         200         194 PRECALL                  0
+                     198 CALL                     0
          
-         186         200 STORE_NAME              14 (create_circle)
+         201         208 STORE_NAME              14 (create_rect)
          
-         189         202 LOAD_NAME                4 (staticmethod)
+         204         210 LOAD_NAME                4 (staticmethod)
          
-         190         204 LOAD_CONST              43 (((0, 0), None, ''))
-                     206 LOAD_CONST              23 ('pos')
-                     208 LOAD_NAME               10 (tuple)
-                     210 LOAD_CONST              26 ('font')
-                     212 LOAD_NAME               15 (Font)
-                     214 LOAD_CONST              27 ('string')
-                     216 LOAD_NAME                5 (str)
-                     218 BUILD_TUPLE              6
-                     220 LOAD_CONST              28 (<code object create_text, file "D:\tkfly\tkfly\blend2d\__init__.py", line 189>)
-                     222 MAKE_FUNCTION            5 (defaults, annotations)
+         205         212 LOAD_CONST              45 (((0, 0), 40))
+                     214 LOAD_CONST              26 ('pos')
+                     216 LOAD_NAME               10 (tuple)
+                     218 LOAD_CONST              16 ('size')
+                     220 LOAD_NAME                6 (int)
+                     222 JUMP_IF_TRUE_OR_POP      1 (to 226)
+                     224 LOAD_NAME               15 (float)
+                 >>  226 BUILD_TUPLE              4
+                     228 LOAD_CONST              27 (<code object create_circle, file "D:\tkfly\tkfly\blend2d\__init__.py", line 204>)
+                     230 MAKE_FUNCTION            5 (defaults, annotations)
          
-         189         224 PRECALL                  0
-                     228 CALL                     0
+         204         232 PRECALL                  0
+                     236 CALL                     0
          
-         190         238 STORE_NAME              16 (create_text)
+         205         246 STORE_NAME              16 (create_circle)
          
-         202         240 LOAD_NAME                4 (staticmethod)
+         208         248 LOAD_NAME                4 (staticmethod)
          
-         203         242 LOAD_CONST              44 (('red', 1.0))
-                     244 LOAD_CONST              31 ('alpha')
-                     246 LOAD_NAME               13 (float)
-                     248 BUILD_TUPLE              2
-                     250 LOAD_CONST              32 (<code object get_color, file "D:\tkfly\tkfly\blend2d\__init__.py", line 202>)
-                     252 MAKE_FUNCTION            5 (defaults, annotations)
+         209         250 LOAD_CONST              46 (((0, 0), None, ''))
+                     252 LOAD_CONST              26 ('pos')
+                     254 LOAD_NAME               10 (tuple)
+                     256 LOAD_CONST              28 ('font')
+                     258 LOAD_NAME               17 (Font)
+                     260 LOAD_CONST              29 ('string')
+                     262 LOAD_NAME                5 (str)
+                     264 BUILD_TUPLE              6
+                     266 LOAD_CONST              30 (<code object create_text, file "D:\tkfly\tkfly\blend2d\__init__.py", line 208>)
+                     268 MAKE_FUNCTION            5 (defaults, annotations)
          
-         202         254 PRECALL                  0
-                     258 CALL                     0
+         208         270 PRECALL                  0
+                     274 CALL                     0
          
-         203         268 STORE_NAME              17 (get_color)
+         209         284 STORE_NAME              18 (create_text)
          
-         206         270 LOAD_NAME                4 (staticmethod)
+         221         286 LOAD_NAME                4 (staticmethod)
          
-         207         272 LOAD_CONST              45 (((0, 0, 0), 1.0))
-                     274 LOAD_CONST              34 ('rgb')
-                     276 LOAD_NAME               10 (tuple)
-                     278 LOAD_CONST              31 ('alpha')
-                     280 LOAD_NAME               13 (float)
-                     282 BUILD_TUPLE              4
-                     284 LOAD_CONST              35 (<code object get_rgb, file "D:\tkfly\tkfly\blend2d\__init__.py", line 206>)
-                     286 MAKE_FUNCTION            5 (defaults, annotations)
+         222         288 LOAD_CONST              47 (('red', 1.0))
+                     290 LOAD_CONST              33 ('alpha')
+                     292 LOAD_NAME               15 (float)
+                     294 BUILD_TUPLE              2
+                     296 LOAD_CONST              34 (<code object get_color, file "D:\tkfly\tkfly\blend2d\__init__.py", line 221>)
+                     298 MAKE_FUNCTION            5 (defaults, annotations)
          
-         206         288 PRECALL                  0
-                     292 CALL                     0
+         221         300 PRECALL                  0
+                     304 CALL                     0
          
-         207         302 STORE_NAME              18 (get_rgb)
+         222         314 STORE_NAME              19 (get_color)
          
-         210         304 LOAD_NAME               19 (property)
+         225         316 LOAD_NAME                4 (staticmethod)
          
-         211         306 LOAD_CONST              36 (<code object platform, file "D:\tkfly\tkfly\blend2d\__init__.py", line 210>)
-                     308 MAKE_FUNCTION            0
+         226         318 LOAD_CONST              48 (((0, 0, 0), 1.0))
+                     320 LOAD_CONST              36 ('rgb')
+                     322 LOAD_NAME               10 (tuple)
+                     324 LOAD_CONST              33 ('alpha')
+                     326 LOAD_NAME               15 (float)
+                     328 BUILD_TUPLE              4
+                     330 LOAD_CONST              37 (<code object get_rgb, file "D:\tkfly\tkfly\blend2d\__init__.py", line 225>)
+                     332 MAKE_FUNCTION            5 (defaults, annotations)
          
-         210         310 PRECALL                  0
-                     314 CALL                     0
+         225         334 PRECALL                  0
+                     338 CALL                     0
          
-         211         324 STORE_NAME              20 (platform)
+         226         348 STORE_NAME              20 (get_rgb)
          
-         214         326 LOAD_NAME               19 (property)
+         229         350 LOAD_NAME               21 (property)
          
-         215         328 LOAD_CONST              37 (<code object libinfo, file "D:\tkfly\tkfly\blend2d\__init__.py", line 214>)
-                     330 MAKE_FUNCTION            0
+         230         352 LOAD_CONST              38 (<code object platform, file "D:\tkfly\tkfly\blend2d\__init__.py", line 229>)
+                     354 MAKE_FUNCTION            0
          
-         214         332 PRECALL                  0
-                     336 CALL                     0
+         229         356 PRECALL                  0
+                     360 CALL                     0
          
-         215         346 STORE_NAME              21 (libinfo)
-                     348 LOAD_CONST               3 (None)
-                     350 RETURN_VALUE
+         230         370 STORE_NAME              22 (platform)
+         
+         233         372 LOAD_NAME               21 (property)
+         
+         234         374 LOAD_CONST              39 (<code object libinfo, file "D:\tkfly\tkfly\blend2d\__init__.py", line 233>)
+                     376 MAKE_FUNCTION            0
+         
+         233         378 PRECALL                  0
+                     382 CALL                     0
+         
+         234         392 STORE_NAME              23 (libinfo)
+                     394 LOAD_CONST               3 (None)
+                     396 RETURN_VALUE
          consts
             'Blend2D'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000001
                   0064015300
-               162           0 RESUME                   0
+               173           0 RESUME                   0
                
-               167           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
+               178           2 LOAD_GLOBAL              1 (NULL + load_blend2d)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 POP_TOP
                             30 LOAD_CONST               1 (None)
                             32 RETURN_VALUE
                consts
                   '\n        Blead2D引擎\n        '
                   None
                names      ('load_blend2d',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       '__init__'
-               firstlineno 162
+               firstlineno 173
                lnotab 0x0205
             '.fontface'
             None
             100
             'name'
             'fontfile'
             'id'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000007c007c01a001000000000000000000
-                  000000000000000000000064016402a6020000ab0200000000000000007c
-                  02ac03a6030000ab0300000000000000005300
-               169           0 RESUME                   0
+                  000000000000000000000064016402a6020000ab02000000000000000074
+                  05000000000000000000007c02a6010000ab010000000000000000740700
+                  000000000000000000a6000000ab0000000000000000007a000000ac03a6
+                  030000ab0300000000000000005300
+               180           0 RESUME                   0
                
-               171           2 LOAD_GLOBAL              1 (NULL + FontFace)
+               182           2 LOAD_GLOBAL              1 (NULL + FontFace)
                             14 LOAD_FAST                0 (name)
                             16 LOAD_FAST                1 (fontfile)
                             18 LOAD_METHOD              1 (replace)
                             40 LOAD_CONST               1 ('\\')
                             42 LOAD_CONST               2 ('/')
                             44 PRECALL                  2
                             48 CALL                     2
-                            58 LOAD_FAST                2 (id)
-                            60 KW_NAMES                 3
-                            62 PRECALL                  3
-                            66 CALL                     3
-                            76 RETURN_VALUE
+                            58 LOAD_GLOBAL              5 (NULL + str)
+                            70 LOAD_FAST                2 (id)
+                            72 PRECALL                  1
+                            76 CALL                     1
+                            86 LOAD_GLOBAL              7 (NULL + radint_id)
+                            98 PRECALL                  0
+                           102 CALL                     0
+                           112 BINARY_OP                0 (+)
+                           116 KW_NAMES                 3
+                           118 PRECALL                  3
+                           122 CALL                     3
+                           132 RETURN_VALUE
                consts
                   None
                   '\\'
                   '/'
                   ('name', 'fontfile', 'faceIdxL')
-               names      ('FontFace', 'replace')
+               names      ('FontFace', 'replace', 'str', 'radint_id')
                varnames   ('name', 'fontfile', 'id')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create_fontface'
-               firstlineno 169
+               firstlineno 180
                lnotab 0x0202
             '.font'
             12
             'fontface'
             'fontsize'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007c007c016a0100000000000000007c
                   02ac01a6030000ab0300000000000000005300
-               173           0 RESUME                   0
+               184           0 RESUME                   0
                
-               175           2 LOAD_GLOBAL              1 (NULL + Font)
+               186           2 LOAD_GLOBAL              1 (NULL + Font)
                             14 LOAD_FAST                0 (name)
                             16 LOAD_FAST                1 (fontface)
                             18 LOAD_ATTR                1 (_name)
                             28 LOAD_FAST                2 (fontsize)
                             30 KW_NAMES                 1
                             32 PRECALL                  3
                             36 CALL                     3
@@ -2467,31 +2708,31 @@
                   ('name', 'fontface', 'fontsize')
                names      ('Font', '_name')
                varnames   ('name', 'fontface', 'fontsize')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create_font'
-               firstlineno 173
+               firstlineno 184
                lnotab 0x0202
             '.surface'
             (450, 450)
             'size'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000007c007c016401190000000000000000
                   007c01640219000000000000000000ac03a6030000ab0300000000000000
                   005300
-               177           0 RESUME                   0
+               188           0 RESUME                   0
                
-               179           2 LOAD_GLOBAL              1 (NULL + Surface)
+               190           2 LOAD_GLOBAL              1 (NULL + Surface)
                             14 LOAD_FAST                0 (name)
                             16 LOAD_FAST                1 (size)
                             18 LOAD_CONST               1 (0)
                             20 BINARY_SUBSCR
                             30 LOAD_FAST                1 (size)
                             32 LOAD_CONST               2 (1)
                             34 BINARY_SUBSCR
@@ -2506,30 +2747,30 @@
                   ('name', 'width', 'height')
                names      ('Surface',)
                varnames   ('name', 'size')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create_surface'
-               firstlineno 177
+               firstlineno 188
                lnotab 0x0202
             '.surface.image'
             'image_name'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000007c007c017c02640119000000000000
                   0000007c02640219000000000000000000ac03a6040000ab040000000000
                   0000005300
-               181           0 RESUME                   0
+               192           0 RESUME                   0
                
-               183           2 LOAD_GLOBAL              1 (NULL + ImageSurface)
+               194           2 LOAD_GLOBAL              1 (NULL + ImageSurface)
                             14 LOAD_FAST                0 (name)
                             16 LOAD_FAST                1 (image_name)
                             18 LOAD_FAST                2 (size)
                             20 LOAD_CONST               1 (0)
                             22 BINARY_SUBSCR
                             32 LOAD_FAST                2 (size)
                             34 LOAD_CONST               2 (1)
@@ -2545,31 +2786,90 @@
                   ('name', 'image_name', 'width', 'height')
                names      ('ImageSurface',)
                varnames   ('name', 'image_name', 'size')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create_image_surface'
-               firstlineno 181
+               firstlineno 192
+               lnotab 0x0202
+            ''
+            code
+               argcount  : 6
+               nlocals   : 6
+               stacksize : 8
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c007c017c027c037c047c05a60600
+                  00ab0600000000000000005300
+               196           0 RESUME                   0
+               
+               198           2 LOAD_GLOBAL              1 (NULL + roundrect)
+                            14 LOAD_FAST                0 (x)
+                            16 LOAD_FAST                1 (y)
+                            18 LOAD_FAST                2 (width)
+                            20 LOAD_FAST                3 (height)
+                            22 LOAD_FAST                4 (rx)
+                            24 LOAD_FAST                5 (ry)
+                            26 PRECALL                  6
+                            30 CALL                     6
+                            40 RETURN_VALUE
+               consts
+                  None
+               names      ('roundrect',)
+               varnames   ('x', 'y', 'width', 'height', 'rx', 'ry')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
+               name       'create_roundrect'
+               firstlineno 196
+               lnotab 0x0202
+            code
+               argcount  : 4
+               nlocals   : 4
+               stacksize : 6
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c007c017c027c03a6040000ab0400
+                  000000000000005300
+               200           0 RESUME                   0
+               
+               202           2 LOAD_GLOBAL              1 (NULL + rect)
+                            14 LOAD_FAST                0 (x)
+                            16 LOAD_FAST                1 (y)
+                            18 LOAD_FAST                2 (width)
+                            20 LOAD_FAST                3 (height)
+                            22 PRECALL                  4
+                            26 CALL                     4
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('rect',)
+               varnames   ('x', 'y', 'width', 'height')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
+               name       'create_rect'
+               firstlineno 200
                lnotab 0x0202
             (0, 0)
             40
             'pos'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007c006401190000000000000000007c
                   006402190000000000000000007c01a6030000ab03000000000000000053
                   00
-               185           0 RESUME                   0
+               204           0 RESUME                   0
                
-               187           2 LOAD_GLOBAL              1 (NULL + circle)
+               206           2 LOAD_GLOBAL              1 (NULL + circle)
                             14 LOAD_FAST                0 (pos)
                             16 LOAD_CONST               1 (0)
                             18 BINARY_SUBSCR
                             28 LOAD_FAST                0 (pos)
                             30 LOAD_CONST               2 (1)
                             32 BINARY_SUBSCR
                             42 LOAD_FAST                1 (size)
@@ -2582,17 +2882,16 @@
                   1
                names      ('circle',)
                varnames   ('pos', 'size')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create_circle'
-               firstlineno 185
+               firstlineno 204
                lnotab 0x0202
-            ''
             'font'
             'string'
             code
                argcount  : 3
                nlocals   : 7
                stacksize : 6
                flags     : 3
@@ -2602,59 +2901,59 @@
                   000000000035000100740700000000000000000000640464056406ac07a6
                   030000ab0300000000000000007d057409000000000000000000007c056a
                   050000000000000000ac08a6010000ab0100000000000000007d06640064
                   006400a6020000ab02000000000000000001006e0b230031007304770278
                   035900770101005900010001007c067d01740d000000000000000000007c
                   006401190000000000000000007c006405190000000000000000007c016a
                   0500000000000000007c02a6040000ab0400000000000000005300
-               189           0 RESUME                   0
+               208           0 RESUME                   0
                
-               191           2 LOAD_FAST                1 (font)
+               210           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE    95 (to 196)
                
-               192           6 LOAD_CONST               1 (0)
+               211           6 LOAD_CONST               1 (0)
                              8 LOAD_CONST               2 (('fly_local', 'fly_chdir'))
                             10 IMPORT_NAME              0 (tkfly.core)
                             12 IMPORT_FROM              1 (fly_local)
                             14 STORE_FAST               3 (fly_local)
                             16 IMPORT_FROM              2 (fly_chdir)
                             18 STORE_FAST               4 (fly_chdir)
                             20 POP_TOP
                
-               194          22 PUSH_NULL
+               213          22 PUSH_NULL
                             24 LOAD_FAST                4 (fly_chdir)
                             26 PUSH_NULL
                             28 LOAD_FAST                3 (fly_local)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 LOAD_CONST               3 ('\\blend2d')
                             46 BINARY_OP                0 (+)
                             50 PRECALL                  1
                             54 CALL                     1
                             64 BEFORE_WITH
                             66 POP_TOP
                
-               195          68 LOAD_GLOBAL              7 (NULL + FontFace)
+               214          68 LOAD_GLOBAL              7 (NULL + FontFace)
                             80 LOAD_CONST               4 ('HarmonyOS_Sans_Medium.ttf')
                             82 LOAD_CONST               5 (1)
                             84 LOAD_CONST               6 ('.fontface.road_page')
                             86 KW_NAMES                 7
                             88 PRECALL                  3
                             92 CALL                     3
                            102 STORE_FAST               5 (_fontface)
                
-               196         104 LOAD_GLOBAL              9 (NULL + Font)
+               215         104 LOAD_GLOBAL              9 (NULL + Font)
                            116 LOAD_FAST                5 (_fontface)
                            118 LOAD_ATTR                5 (_name)
                            128 KW_NAMES                 8
                            130 PRECALL                  1
                            134 CALL                     1
                            144 STORE_FAST               6 (_font)
                
-               194         146 LOAD_CONST               0 (None)
+               213         146 LOAD_CONST               0 (None)
                            148 LOAD_CONST               0 (None)
                            150 LOAD_CONST               0 (None)
                            152 PRECALL                  2
                            156 CALL                     2
                            166 POP_TOP
                            168 JUMP_FORWARD            11 (to 192)
                        >>  170 PUSH_EXC_INFO
@@ -2665,18 +2964,18 @@
                            180 POP_EXCEPT
                            182 RERAISE                  1
                        >>  184 POP_TOP
                            186 POP_EXCEPT
                            188 POP_TOP
                            190 POP_TOP
                
-               198     >>  192 LOAD_FAST                6 (_font)
+               217     >>  192 LOAD_FAST                6 (_font)
                            194 STORE_FAST               1 (font)
                
-               200     >>  196 LOAD_GLOBAL             13 (NULL + text)
+               219     >>  196 LOAD_GLOBAL             13 (NULL + text)
                            208 LOAD_FAST                0 (pos)
                            210 LOAD_CONST               1 (0)
                            212 BINARY_SUBSCR
                            222 LOAD_FAST                0 (pos)
                            224 LOAD_CONST               5 (1)
                            226 BINARY_SUBSCR
                            236 LOAD_FAST                1 (font)
@@ -2701,59 +3000,59 @@
                   ('fontface',)
                names      ('tkfly.core', 'fly_local', 'fly_chdir', 'FontFace', 'Font', '_name', 'text')
                varnames   ('pos', 'font', 'string', 'fly_local', 'fly_chdir', '_fontface', '_font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'create_text'
-               firstlineno 189
+               firstlineno 208
                lnotab 0x0202040110022e0124012afe2e040402
             'red'
             1.0
             'alpha'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c007c01a6020000ab020000000000
                   0000005300
-               202           0 RESUME                   0
+               221           0 RESUME                   0
                
-               204           2 LOAD_GLOBAL              1 (NULL + color)
+               223           2 LOAD_GLOBAL              1 (NULL + color)
                             14 LOAD_FAST                0 (name)
                             16 LOAD_FAST                1 (alpha)
                             18 PRECALL                  2
                             22 CALL                     2
                             32 RETURN_VALUE
                consts
                   None
                names      ('color',)
                varnames   ('name', 'alpha')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'get_color'
-               firstlineno 202
+               firstlineno 221
                lnotab 0x0202
             (0, 0, 0)
             'rgb'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000007c006401190000000000000000007c
                   006402190000000000000000007c006403190000000000000000007c01a6
                   040000ab0400000000000000005300
-               206           0 RESUME                   0
+               225           0 RESUME                   0
                
-               208           2 LOAD_GLOBAL              1 (NULL + color)
+               227           2 LOAD_GLOBAL              1 (NULL + color)
                             14 LOAD_FAST                0 (rgb)
                             16 LOAD_CONST               1 (0)
                             18 BINARY_SUBSCR
                             28 LOAD_FAST                0 (rgb)
                             30 LOAD_CONST               2 (1)
                             32 BINARY_SUBSCR
                             42 LOAD_FAST                0 (rgb)
@@ -2770,83 +3069,85 @@
                   2
                names      ('color',)
                varnames   ('rgb', 'alpha')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'get_rgb'
-               firstlineno 206
+               firstlineno 225
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000053
                   00
-               210           0 RESUME                   0
+               229           0 RESUME                   0
                
-               212           2 LOAD_GLOBAL              1 (NULL + platform)
+               231           2 LOAD_GLOBAL              1 (NULL + platform)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 RETURN_VALUE
                consts
                   None
                names      ('platform',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'platform'
-               firstlineno 210
+               firstlineno 229
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000053
                   00
-               214           0 RESUME                   0
+               233           0 RESUME                   0
                
-               216           2 LOAD_GLOBAL              1 (NULL + libinfo)
+               235           2 LOAD_GLOBAL              1 (NULL + libinfo)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 RETURN_VALUE
                consts
                   None
                names      ('libinfo',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
                name       'libinfo'
-               firstlineno 214
+               firstlineno 233
                lnotab 0x0202
             ('.fontface', None, 100)
             ('.font', None, 12)
             ('.surface', (450, 450))
             ('.surface', '.surface.image', (450, 450))
+            ('',)
             ((0, 0), 40)
             ((0, 0), None, '')
             ('red', 1.0)
             ((0, 0, 0), 1.0)
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'staticmethod', 'str', 'int', 'create_fontface', 'FontFace', 'create_font', 'tuple', 'create_surface', 'create_image_surface', 'float', 'create_circle', 'Font', 'create_text', 'get_color', 'get_rgb', 'property', 'platform', 'libinfo')
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'staticmethod', 'str', 'int', 'create_fontface', 'FontFace', 'create_font', 'tuple', 'create_surface', 'create_image_surface', 'create_roundrect', 'create_rect', 'float', 'create_circle', 'Font', 'create_text', 'get_color', 'get_rgb', 'property', 'platform', 'libinfo')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
          name       'Blend2D'
-         firstlineno 161
+         firstlineno 172
          lnotab
             0x0a010607020114ff0e010203020114ff0e010203020110ff0e01020302
-            0114ff0e010203020114ff0e010203020114ff0e01020c02010cff0e0102
-            03020110ff0e010203020104ff0e010203020104ff0e01
+            0114ff0e010203020106ff0e010203020104ff0e010203020114ff0e0102
+            03020114ff0e01020c02010cff0e010203020110ff0e010203020104ff0e
+            010203020104ff0e01
       'Blend2D'
       '__main__'
       ('Tk', 'PhotoImage', 'Label')
       ('text',)
       'x'
       'top'
       ('fill', 'side')
@@ -2855,25 +3156,28 @@
       ('fly_local', 'fly_chdir')
       'HarmonyOS_Sans_Medium.ttf'
       ('fontfile',)
       ('fontface',)
       150
       225
       'lightblue'
+      20
+      100
+      'orange'
       'both'
       ('fill',)
       None
       (1.0,)
       (0, 0, 0, 1.0)
       (50,)
       ('',)
-   names      ('tkfly.core', 'fly_load4', 'fly_root', 'fly_local', 'fly_chdir', 'tkinter', 'Widget', 'Image', 'Label', 'enum', 'Enum', 'load_blend2d', 'LINEAR', 'RADIAL', 'CONICAL', 'GRADIENT_TYPE', 'float', 'color', 'rgb', 'gradient', 'circle', 'str', 'text', 'classes', 'libinfo', 'platform', 'radint_id', 'Blend2DImage', 'object', 'Surface', 'FontFace', 'Font', 'ImageSurface', 'Blend2D', '__name__', 'Tk', 'PhotoImage', 'root', 'info', 'pack', 'blend2d', 'create_image_surface', 'surface', 'create_fontface', 'fontface1', 'create_font', 'font1', 'fill', 'mainloop')
+   names      ('tkfly.core', 'fly_load4', 'fly_root', 'fly_local', 'fly_chdir', 'tkinter', 'Widget', 'Image', 'Label', 'enum', 'Enum', 'load_blend2d', 'LINEAR', 'RADIAL', 'CONICAL', 'GRADIENT_TYPE', 'float', 'color', 'rgb', 'gradient', 'circle', 'rect', 'roundrect', 'str', 'text', 'classes', 'libinfo', 'platform', 'radint_id', 'Blend2DImage', 'object', 'Surface', 'FontFace', 'Font', 'ImageSurface', 'Blend2D', '__name__', 'Tk', 'PhotoImage', 'root', 'info', 'pack', 'blend2d', 'create_image_surface', 'surface', 'create_fontface', 'fontface1', 'create_font', 'font1', 'fill', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkfly\\tkfly\\blend2d\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201180114010c0306040401040104031c060e040e040c0408040e
-      0406050605060506051c051c2e1c0b1c0e1c181c3a0c011402140228012e
-      0214022c0510022c012c025e022c022ce8
+      0x00ff0201180114010c0306040401040104031c060e040e040c04080406
+      0408040e0406050605060506051c051c311c0b1c0e1c181c420e01140214
+      0228012e0214022c0510022c012c025e0262022c022ce6
```

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d1.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d101.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d101.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d102.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d102.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d2.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d3.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d4_1.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d4_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d4_2.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d4_2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d5.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d5.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d6.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d6.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d7.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/d7.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/dct.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/dct.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/dpda.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/blend2d/demos/__pycache__/dpda.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/Blacksword.otf` & `tkfly-0.1.0a4/tkfly/blend2d/demos/Blacksword.otf`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/CMYK.png` & `tkfly-0.1.0a4/tkfly/blend2d/demos/CMYK.png`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/CompositionTest.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/CompositionTest.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/d101.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/d101.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/d102.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/d102.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/d110.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/d110.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/d4_1.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/d4_1.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/d4_2.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/d4_2.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/d5.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/d5.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/d6.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/d6.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/d7.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/d7.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/dct.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/dct.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/demo-tiger.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/demo-tiger.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/dpda.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/dpda.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/drect.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/drect.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/dtiger.py` & `tkfly-0.1.0a4/tkfly/blend2d/demos/dtiger.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/greenSlate.jpg` & `tkfly-0.1.0a4/tkfly/blend2d/demos/greenSlate.jpg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/IKscale-1.0.1.tm` & `tkfly-0.1.0a4/tkfly/blend2d/demos/IKscale-1.0.1.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/EbuttonColor-1.0.1.tm` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/EbuttonColor-1.0.1.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/Eseparator-1.0.tm` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/Eseparator-1.0.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/hatching-1.0.tm` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/hatching-1.0.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/IKscale-1.0.1.tm` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/IKscale-1.0.1.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/darwin-x64/perlin.dylib` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/darwin-x64/perlin.dylib`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/license.terms` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/license.terms`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/linux-x32/perlin.so` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/linux-x32/perlin.so`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/linux-x64/perlin.so` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/linux-x64/perlin.so`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/win-x32/perlin.dll` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/win-x32/perlin.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/win-x64/perlin.dll` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/perlin-1.0/win-x64/perlin.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/sketchline-1.0.tm` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/sketchline-1.0.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/main2.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/main2.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/snit2.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/snit2.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/validate.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/snit.2.3.2/validate.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/lib/Spline-1.0.tm` & `tkfly-0.1.0a4/tkfly/blend2d/demos/lib/Spline-1.0.tm`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/moby.svg` & `tkfly-0.1.0a4/tkfly/blend2d/demos/moby.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/PorterDuffInAction.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/PorterDuffInAction.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_1.svg` & `tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_1.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_2.svg` & `tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_2.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_3.svg` & `tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_3.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_4.svg` & `tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_4.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_5.svg` & `tkfly-0.1.0a4/tkfly/blend2d/demos/Q/layer_5.svg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/RGB.png` & `tkfly-0.1.0a4/tkfly/blend2d/demos/RGB.png`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/Road_Rage.otf` & `tkfly-0.1.0a4/tkfly/blend2d/demos/Road_Rage.otf`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/texture.jpeg` & `tkfly-0.1.0a4/tkfly/blend2d/demos/texture.jpeg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/demos/tiger-data.tcl` & `tkfly-0.1.0a4/tkfly/blend2d/demos/tiger-data.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/HarmonyOS_Sans_Medium.ttf` & `tkfly-0.1.0a4/tkfly/blend2d/HarmonyOS_Sans_Medium.ttf`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/blend2d/surface.bmp` & `tkfly-0.1.0a4/tkfly/blend2d/surface.bmp`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/core.py` & `tkfly-0.1.0a4/tkfly/core.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/jpegtcl950.dll` & `tkfly-0.1.0a4/tkfly/tkimg/jpegtcl950.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/libjpegtclstub950.a` & `tkfly-0.1.0a4/tkfly/tkimg/libjpegtclstub950.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/libpngtclstub1638.a` & `tkfly-0.1.0a4/tkfly/tkimg/libpngtclstub1638.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/libtifftclstub440.a` & `tkfly-0.1.0a4/tkfly/tkimg/libtifftclstub440.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/libtkimgstub1414.a` & `tkfly-0.1.0a4/tkfly/tkimg/libtkimgstub1414.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/libzlibtclstub1213.a` & `tkfly-0.1.0a4/tkfly/tkimg/libzlibtclstub1213.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/pkgIndex.tcl` & `tkfly-0.1.0a4/tkfly/tkimg/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/pngtcl1638.dll` & `tkfly-0.1.0a4/tkfly/tkimg/pngtcl1638.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tifftcl440.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tifftcl440.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimg1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimg1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgbmp1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgbmp1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgdted1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgdted1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgflir1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgflir1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimggif1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimggif1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgico1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgico1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgjpeg1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgjpeg1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgpcx1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgpcx1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgpixmap1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgpixmap1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgpng1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgpng1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgppm1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgppm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgps1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgps1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgraw1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgraw1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgsgi1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgsgi1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgsun1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgsun1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgtga1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgtga1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgtiff1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgtiff1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgwindow1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgwindow1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgxbm1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgxbm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/tkimgxpm1414.dll` & `tkfly-0.1.0a4/tkfly/tkimg/tkimgxpm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkimg/zlibtcl1213.dll` & `tkfly-0.1.0a4/tkfly/tkimg/zlibtcl1213.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/__pycache__/datefield.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tklib/__pycache__/datefield.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/__pycache__/history.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tklib/__pycache__/history.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/autoscroll.py` & `tkfly-0.1.0a4/tkfly/tklib/autoscroll.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/chatwidget.py` & `tkfly-0.1.0a4/tkfly/tklib/chatwidget.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/datefield.py` & `tkfly-0.1.0a4/tkfly/tklib/datefield.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/history.py` & `tkfly-0.1.0a4/tkfly/tklib/history.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/menubar.py` & `tkfly-0.1.0a4/tkfly/tklib/menubar.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/notifywindow.py` & `tkfly-0.1.0a4/tkfly/tklib/notifywindow.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/plotchart.py` & `tkfly-0.1.0a4/tkfly/tklib/plotchart.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/shtmlview.py` & `tkfly-0.1.0a4/tkfly/tklib/shtmlview.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/tooltip.py` & `tkfly-0.1.0a4/tkfly/tklib/tooltip.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/wcb.py` & `tkfly-0.1.0a4/tkfly/tklib/wcb.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tklib/widget.py` & `tkfly-0.1.0a4/tkfly/tklib/widget.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/scrollableframe.py` & `tkfly-0.1.0a4/tkfly/tkscrollutil/scrollableframe.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/scrollarea.py` & `tkfly-0.1.0a4/tkfly/tkscrollutil/scrollarea.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/scrollsync.py` & `tkfly-0.1.0a4/tkfly/tkscrollutil/scrollsync.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollarea.py` & `tkfly-0.1.0a4/tkfly/tkscrollutil/ttk_scrollarea.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollednotebook.py` & `tkfly-0.1.0a4/tkfly/tkscrollutil/ttk_scrollednotebook.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollsync.py` & `tkfly-0.1.0a4/tkfly/tkscrollutil/ttk_scrollsync.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/tkscrollutil/wheelevent.py` & `tkfly-0.1.0a4/tkfly/tkscrollutil/wheelevent.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/twapi/__init__.py` & `tkfly-0.1.0a4/tkfly/twapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/twapi/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a4/tkfly/twapi/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/twapi/ui.py` & `tkfly-0.1.0a4/tkfly/twapi/ui.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/tkfly/twapi/win.py` & `tkfly-0.1.0a4/tkfly/twapi/win.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a3/PKG-INFO` & `tkfly-0.1.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfly
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: 
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -26,21 +26,21 @@
 ([blend2d -大小约7.6MB](https://wiki.tcl-lang.org/page/Blend2d))
 
 帮助你开发大型高级的程序
 
 ## 教程
 
 ### 开始
-`tkfly`通过`tkinter`调用`tcl`导入`tklib`实现，可以实现`tklib`库所能实现的各种功能。
 ```bash
 # 暂时处于预览版
 python -m pip install tkfly --pre
 ```
 
 ### 工具提示
+`tkfly`通过`tkinter`调用`tcl`导入`tklib`实现，可以实现`tklib`库所能实现的各种功能。
 让我来运行一个最简单工具提示吧！
 (基于[tklib/tooltip](https://core.tcl-lang.org/tklib/doc/trunk/embedded/md/tklib/files/modules/tooltip/tooltip.md))
 ```python
 from tkinter import Tk, ttk
 from tkfly import FlyToolTip
 
 root = Tk()
@@ -124,14 +124,16 @@
 
 root = Tk()
 blend2D = Fly2D()
 surface = blend2D.create_image_surface(
     size=(500, 500)
 )
 
+print("Create ImageSurface", surface.image_name)
+
 surface.surface.fill(
     blend2D.create_circle((150, 150), 50),
     blend2D.get_color("lightblue", alpha=0.5)
 )
 
 surface.surface.fill(
     blend2D.create_circle((250, 250), 60),
@@ -139,50 +141,102 @@
 )
 
 surface.surface.fill(
     blend2D.create_circle((350, 350), 55),
     blend2D.get_color("lightblue", alpha=0.75)
 )
 
+from tkfly.core import fly_local, fly_chdir
+
+with fly_chdir(fly_local() + "\\blend2d"):
+    fontface = blend2D.create_fontface(fontfile="HarmonyOS_Sans_Medium.ttf")
+    font = blend2D.create_font(fontface=fontface, fontsize=20)
+
+print("Create FontFace", fontface._name)
+print("Create Font", font._name)
 
 surface.surface.fill(
-    blend2D.create_text((235, 255), string="Fly2D"),
+    blend2D.create_text((225, 257), string="Fly2D", font=font),
     blend2D.get_color("black")
 )
 
 surface.pack()
 
 surface.surface.save("fly2d.png")
 
 root.mainloop()
 ```
 
-# tkscrollutil
+### 扩展组件
+#### Document
+这是类似`多文档窗口`类的组件，只是暂时布局没想到好的方案，会空下大部分的空间
+```python
+from tkinter import *
+from tkinter import ttk
+from tkfly import *
+
+root = Tk()
+
+document = FlyMkDocument()
+
+button = ttk.Button(document)
+button.pack(fill="both", expand="yes")
+
+document.config(title="这是多文档窗口")
+
+root.mainloop()
+```
+
+#### ToolBar
+工具栏组件
+```python
+from tkinter import *
+from tkfly import *
+
+root = Tk()
+
+toolbar = FlyMkToolBar()
+
+button1 = toolbar.add(
+    "button",
+    command=lambda:
+        print(f"toolbutton is {toolbar.get(button1)}")
+)
+button2 = toolbar.add("button", command=lambda: toolbar.delete(button2))
+
+
+toolbar.pack(fill="x", side="top")
+
+root.mainloop()
+```
+
+
+## tkscrollutil
 实际上这就是作者我以前做过的一个项目。
 
-## ScrolllArea
+### ScrolllArea
 可以快速地为水平滚动、垂直滚动组件设置滚动条
 
-### 属性
+#### 属性
 `autohidescrollbars` 设置组件是否自动隐藏滚动条。布尔数值。默认`False`。也就是说，当你把鼠标指针放到滚动条上时，滚动条才会显示。 
 
 `lockinterval` 设置组件滚动条地锁定间隔。整数数值。默认`300`.
 
 `respectheader` 仅当将嵌入到组件内地`tablelist`版本为6.5及以上版本时才能使用，后续等开发出`tablelist`的扩展库时补充
 
 `respecttitlecolumns` 仅当将嵌入到组件内地`tablelist`版本为6.5及以上版本时才能使用，后续等开发出`tablelist`的扩展库时补充
 
 `xscrollbarmode` 设置水平滚动条的模式。可选值为`static` `dynamic` `none`。默认`none`。`static`为常驻滚动条；`dynamic`为自动滚动条；`none`为没有滚动条
 
 `yscrollbarmode` 设置垂直滚动条的模式。可选值为`static` `dynamic` `none`。默认`static`。`static`为常驻滚动条；`dynamic`为自动滚动条；`none`为没有滚动条
 
-### 方法
+#### 方法
 `setwidget` 设置具有滚动条属性的组件，使组件快速设置滚动条。
 
-### 示例
+#### 示例
 ```python
 from tkinter import Tk, Listbox
 from tkfly.tkscrollutil import ScrollArea
 
 Window = Tk()
 
 Area = ScrollArea(Window)
@@ -191,18 +245,18 @@
     List.insert(Item+1, Item+1)
 Area.setwidget(List)
 Area.pack(fill="both", expand="yes")
 
 Window.mainloop()
 ```
 
-## ttkScrollArea
+#### ttkScrollArea
 见上方。与`ScrollArea`不同的是，`ttkScrollArea`具有ttk组件的属性，并且`ScrollArea`和`ttkScrollArea`不能同时使用。
 
-### 示例
+#### 示例
 ```python
 from tkinter import Tk, Listbox
 from tkfly.tkscrollutil import ttkScrollArea
 
 Window = Tk()
 
 Area = ttkScrollArea(Window)
@@ -211,23 +265,23 @@
     List.insert(Item+1, Item+1)
 Area.setwidget(List)
 Area.pack(fill="both", expand="yes")
 
 Window.mainloop()
 ```
 
-## ScrollSync
+#### ScrollSync
 同步滚动条，当其中一个滚动时，另一个也会跟随着移动起来。
 
-### 方法
+#### 方法
 `setwidgets` 设置同步滚动的组件。需输入列表，如 [widget1, widget2] 。
 
 `widgets` 获取同步滚动的组件。
 
-### 示例
+#### 示例
 ```python
 from tkinter import Tk, Listbox, Frame
 from tkfly.tkscrollutil import ScrollArea, ScrollSync
 Window = Tk()
 
 Frame = Frame()
 
@@ -249,18 +303,18 @@
 Sync.setwidgets([List1, List2])
 
 Frame.pack(fill="both", expand="yes")
 
 Window.mainloop()
 ```
 
-## ttkScrollSync
+#### ttkScrollSync
 见上方。与`ScrollSync`不同的是，`ttkScrollSync`具有ttk组件的属性，并且`ScrollSync`和`ttkScrollSync`不能同时使用。
 
-### 示例
+#### 示例
 ```python
 from tkinter import Tk, Listbox, Frame
 from tkfly.tkscrollutil import ttkScrollArea, ttkScrollSync
 Window = Tk()
 
 Frame = Frame()
 
@@ -282,15 +336,15 @@
 Sync.setwidgets([List1, List2])
 
 Frame.pack(fill="both", expand="yes")
 
 Window.mainloop()
 ```
 
-## ttkScrolledNoteBook
+#### ttkScrolledNoteBook
 scrollutil本身不提供ScrolledNoteBook，只有ttk能够提供。
 ```python
 from tkinter import Tk, Frame
 from tkfly.tkscrollutil import ttkScrolledNoteBook, addclosetab
 Window = Tk()
 
 NoteBook = ttkScrolledNoteBook(Window)
```

