# Comparing `tmp/tkfly-0.1.0a2.tar.gz` & `tmp/tkfly-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfly-0.1.0a2.tar", max compression
+gzip compressed data, was "tkfly-0.1.0a3.tar", max compression
```

## Comparing `tkfly-0.1.0a2.tar` & `tkfly-0.1.0a3.tar`

### file list

```diff
@@ -1,328 +1,499 @@
--rw-r--r--   0        0        0      280 2023-04-29 10:08:50.067612 tkfly-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     6483 2023-04-29 11:37:28.438767 tkfly-0.1.0a2/README.md
--rw-r--r--   0        0        0      713 2023-04-29 11:43:39.636888 tkfly-0.1.0a2/tkfly/__init__.py
--rw-r--r--   0        0        0      673 2023-04-29 10:25:40.967581 tkfly-0.1.0a2/tkfly/__main__.py
--rw-r--r--   0        0        0      224 2023-04-19 11:06:45.090485 tkfly-0.1.0a2/tkfly/_tklib/__init__.py
--rw-r--r--   0        0        0      677 2023-04-19 11:08:58.393781 tkfly-0.1.0a2/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1667 2023-04-14 12:45:42.167394 tkfly-0.1.0a2/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7112 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/autoscroll/autoscroll.tcl
--rw-r--r--   0        0        0      611 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/autoscroll/pkgIndex.tcl
--rw-r--r--   0        0        0     7344 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_drag.tcl
--rw-r--r--   0        0        0    10374 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_epoints.tcl
--rw-r--r--   0        0        0    12828 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_epolyline.tcl
--rw-r--r--   0        0        0    11211 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_equad.tcl
--rw-r--r--   0        0        0     7467 2014-08-11 05:20:11.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_gradient.tcl
--rw-r--r--   0        0        0     2947 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_highlight.tcl
--rw-r--r--   0        0        0     9922 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_mvg.tcl
--rw-r--r--   0        0        0     2964 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_snap.tcl
--rw-r--r--   0        0        0    21321 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_sqmap.tcl
--rw-r--r--   0        0        0     1545 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_tags.tcl
--rw-r--r--   0        0        0     2195 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_trlines.tcl
--rw-r--r--   0        0        0     5161 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_zoom.tcl
--rw-r--r--   0        0        0     1295 2014-08-11 05:20:11.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/pkgIndex.tcl
--rw-r--r--   0        0        0    26671 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/chatwidget/chatwidget.tcl
--rw-r--r--   0        0        0       80 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/chatwidget/pkgIndex.tcl
--rw-r--r--   0        0        0     1365 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/bindDown.tcl
--rw-r--r--   0        0        0      381 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/controlwidget.tcl
--rw-r--r--   0        0        0     3401 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/led.tcl
--rw-r--r--   0        0        0      903 2018-05-11 03:56:07.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/pkgIndex.tcl
--rw-r--r--   0        0        0     7666 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/radioMatrix.tcl
--rw-r--r--   0        0        0    16186 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/rdial.tcl
--rw-r--r--   0        0        0    12150 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/tachometer.tcl
--rw-r--r--   0        0        0    48034 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/vertical_meter.tcl
--rw-r--r--   0        0        0    11332 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/voltmeter.tcl
--rw-r--r--   0        0        0    16207 2014-08-11 05:20:11.000000 tkfly-0.1.0a2/tkfly/_tklib/crosshair/crosshair.tcl
--rw-r--r--   0        0        0      138 2013-05-10 05:18:16.000000 tkfly-0.1.0a2/tkfly/_tklib/crosshair/pkgIndex.tcl
--rw-r--r--   0        0        0    27293 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ctext/ctext.tcl
--rw-r--r--   0        0        0       68 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ctext/pkgIndex.tcl
--rw-r--r--   0        0        0     3924 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/cursor/cursor.tcl
--rw-r--r--   0        0        0       72 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/cursor/pkgIndex.tcl
--rw-r--r--   0        0        0    12481 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/datefield/datefield.tcl
--rw-r--r--   0        0        0       76 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/datefield/pkgIndex.tcl
--rw-r--r--   0        0        0    12537 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/application.tcl
--rw-r--r--   0        0        0    10383 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/attributes.tcl
--rw-r--r--   0        0        0    37096 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/basic.tcl
--rw-r--r--   0        0        0    32433 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/core.tcl
--rw-r--r--   0        0        0     1557 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/diagram.tcl
--rw-r--r--   0        0        0     7807 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/direction.tcl
--rw-r--r--   0        0        0     7931 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/element.tcl
--rw-r--r--   0        0        0     3423 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/navigation.tcl
--rw-r--r--   0        0        0      847 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/pkgIndex.tcl
--rw-r--r--   0        0        0     4837 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/point.tcl
--rw-r--r--   0        0        0      612 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/getstring/pkgIndex.tcl
--rw-r--r--   0        0        0     4224 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/getstring/tk_getString.tcl
--rw-r--r--   0        0        0     3187 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/history/history.tcl
--rw-r--r--   0        0        0      605 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/history/pkgIndex.tcl
--rw-r--r--   0        0        0    44954 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ico/ico.tcl
--rw-r--r--   0        0        0    35176 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ico/ico0.tcl
--rw-r--r--   0        0        0      292 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ico/pkgIndex.tcl
--rw-r--r--   0        0        0    29231 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ipentry/ipentry.tcl
--rw-r--r--   0        0        0      139 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ipentry/pkgIndex.tcl
--rw-r--r--   0        0        0     3795 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/cs.msg
--rw-r--r--   0        0        0     3718 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/da.msg
--rw-r--r--   0        0        0     4409 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/de.msg
--rw-r--r--   0        0        0     3918 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/en.msg
--rw-r--r--   0        0        0     3979 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/es.msg
--rw-r--r--   0        0        0    56665 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/khim.tcl
--rw-r--r--   0        0        0      534 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/pkgIndex.tcl
--rw-r--r--   0        0        0     4124 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/pl.msg
--rw-r--r--   0        0        0     2937 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/ROOT.msg
--rw-r--r--   0        0        0     6679 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/ru.msg
--rw-r--r--   0        0        0     6361 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/uk.msg
--rw-r--r--   0        0        0      444 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/mentry.tcl
--rw-r--r--   0        0        0      737 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/mentry_tile.tcl
--rw-r--r--   0        0        0     2592 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/mentryPublic.tcl
--rw-r--r--   0        0        0      860 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/pkgIndex.tcl
--rw-r--r--   0        0        0    25858 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl
--rw-r--r--   0        0        0     4298 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl
--rw-r--r--   0        0        0     5661 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl
--rw-r--r--   0        0        0     6884 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl
--rw-r--r--   0        0        0    18737 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryThemes.tcl
--rw-r--r--   0        0        0    60325 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryWidget.tcl
--rw-r--r--   0        0        0    19506 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mwutil.tcl
--rw-r--r--   0        0        0    10636 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/tclIndex
--rw-r--r--   0        0        0     5469 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/debug.tcl
--rw-r--r--   0        0        0    53951 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/menubar.tcl
--rw-r--r--   0        0        0     3859 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/node.tcl
--rw-r--r--   0        0        0      299 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/pkgIndex.tcl
--rw-r--r--   0        0        0    26016 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/tree.tcl
--rw-r--r--   0        0        0     4015 2023-04-29 05:27:10.370187 tkfly-0.1.0a2/tkfly/_tklib/notifywindow/notifywindow.tcl
--rw-r--r--   0        0        0      548 2016-07-14 05:57:54.000000 tkfly-0.1.0a2/tkfly/_tklib/notifywindow/pkgIndex.tcl
--rw-r--r--   0        0        0   120514 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/ntext/ntext.tcl
--rw-r--r--   0        0        0      132 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/ntext/pkgIndex.tcl
--rw-r--r--   0        0        0    30859 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/persistentSelection/persistentSelection.tcl
--rw-r--r--   0        0        0      160 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/persistentSelection/pkgIndex.tcl
--rw-r--r--   0        0        0     3291 2023-04-14 12:33:32.365933 tkfly-0.1.0a2/tkfly/_tklib/pkgIndex.tcl
--rw-r--r--   0        0        0      321 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/pkgIndex.tcl
--rw-r--r--   0        0        0    13471 2015-04-21 06:10:00.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plot3d.tcl
--rw-r--r--   0        0        0    15740 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotanim.tcl
--rw-r--r--   0        0        0    12916 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotannot.tcl
--rw-r--r--   0        0        0    67951 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotaxis.tcl
--rw-r--r--   0        0        0     6478 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotbind.tcl
--rw-r--r--   0        0        0    11059 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotbusiness.tcl
--rw-r--r--   0        0        0   108162 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotchart.tcl
--rw-r--r--   0        0        0     5721 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotcombined.tcl
--rw-r--r--   0        0        0    16783 2015-04-21 06:10:00.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotconfig.tcl
--rw-r--r--   0        0        0    61163 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotcontour.tcl
--rw-r--r--   0        0        0    10041 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotgantt.tcl
--rw-r--r--   0        0        0     8895 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotobject.tcl
--rw-r--r--   0        0        0     9423 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotpack.tcl
--rw-r--r--   0        0        0   139321 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotpriv.tcl
--rw-r--r--   0        0        0     8072 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotscada.tcl
--rw-r--r--   0        0        0     5697 2016-07-14 05:57:54.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotspecial.tcl
--rw-r--r--   0        0        0     7475 2014-08-11 05:20:12.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotstatustimeline.tcl
--rw-r--r--   0        0        0     9893 2015-04-21 06:10:00.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plottable.tcl
--rw-r--r--   0        0        0     5215 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/scaling.tcl
--rw-r--r--   0        0        0    16372 2014-11-24 17:34:56.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/xyplot.tcl
--rw-r--r--   0        0        0      867 2022-07-14 16:02:02.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/pkgIndex.tcl
--rw-r--r--   0        0        0     2420 2022-08-15 11:36:06.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/attrib.tcl
--rw-r--r--   0        0        0    19506 2020-01-08 04:03:39.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/mwutil.tcl
--rw-r--r--   0        0        0    16416 2022-04-25 10:54:58.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl
--rw-r--r--   0        0        0    25675 2022-08-23 17:53:48.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/pagesman.tcl
--rw-r--r--   0        0        0    53698 2022-08-23 18:08:46.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl
--rw-r--r--   0        0        0    36010 2022-08-17 10:02:40.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl
--rw-r--r--   0        0        0    36693 2022-08-17 10:03:10.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl
--rw-r--r--   0        0        0    57949 2022-09-11 08:36:20.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl
--rw-r--r--   0        0        0    18623 2022-08-17 10:05:36.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl
--rw-r--r--   0        0        0    19056 2022-08-15 19:39:16.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/tclIndex
--rw-r--r--   0        0        0        0 2022-10-29 06:04:07.908293 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/__init__.py
--rw-r--r--   0        0        0    21894 2022-05-20 15:38:54.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl
--rw-r--r--   0        0        0      537 2022-10-19 15:21:54.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl
--rw-r--r--   0        0        0    22642 2022-05-29 18:19:18.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl
--rw-r--r--   0        0        0    51787 2022-10-22 15:11:52.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl
--rw-r--r--   0        0        0    27243 2022-04-10 15:20:18.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl
--rw-r--r--   0        0        0      686 2022-07-14 16:02:24.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutil.tcl
--rw-r--r--   0        0        0     1138 2022-07-14 16:03:16.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutil_tile.tcl
--rw-r--r--   0        0        0     3214 2022-10-18 14:23:10.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutilCommon.tcl
--rw-r--r--   0        0        0    15316 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/style/as.tcl
--rw-r--r--   0        0        0     2848 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/style/lobster.tcl
--rw-r--r--   0        0        0      684 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/style/pkgIndex.tcl
--rw-r--r--   0        0        0      765 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/style/style.tcl
--rw-r--r--   0        0        0      607 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/swaplist/pkgIndex.tcl
--rw-r--r--   0        0        0    13365 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/swaplist/swaplist.tcl
--rw-r--r--   0        0        0      898 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/pkgIndex.tcl
--rw-r--r--   0        0        0    19506 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/mwutil.tcl
--rw-r--r--   0        0        0     4286 2015-04-21 06:10:00.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/pencil.cur
--rw-r--r--   0        0        0     2911 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/repair.tcl
--rw-r--r--   0        0        0   133438 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl
--rw-r--r--   0        0        0   120387 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl
--rw-r--r--   0        0        0    93461 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl
--rw-r--r--   0        0        0   125609 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl
--rw-r--r--   0        0        0    17564 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl
--rw-r--r--   0        0        0    20512 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl
--rw-r--r--   0        0        0    68715 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl
--rw-r--r--   0        0        0   202524 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl
--rw-r--r--   0        0        0   267492 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl
--rw-r--r--   0        0        0    62720 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tclIndex
--rw-r--r--   0        0        0      488 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelist.tcl
--rw-r--r--   0        0        0      763 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelist_tile.tcl
--rw-r--r--   0        0        0     3022 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelistPublic.tcl
--rw-r--r--   0        0        0     4807 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/boxlabel.tcl
--rw-r--r--   0        0        0     7705 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/canlabel.tcl
--rw-r--r--   0        0        0     3303 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/labarray.tcl
--rw-r--r--   0        0        0     1185 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/objselec.tcl
--rw-r--r--   0        0        0     8331 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/perilabel.tcl
--rw-r--r--   0        0        0    15130 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pie.tcl
--rw-r--r--   0        0        0     1231 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pielabel.tcl
--rw-r--r--   0        0        0      154 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pkgIndex.tcl
--rw-r--r--   0        0        0     4150 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/relirect.tcl
--rw-r--r--   0        0        0     4729 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/selector.tcl
--rw-r--r--   0        0        0    13055 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/slice.tcl
--rw-r--r--   0        0        0     4728 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/tkpiechart.tcl
--rw-r--r--   0        0        0      166 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/tooltip/pkgIndex.tcl
--rw-r--r--   0        0        0     4021 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tooltip/tipstack.tcl
--rw-r--r--   0        0        0    14446 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/tooltip/tooltip.tcl
--rw-r--r--   0        0        0      427 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/pkgIndex.tcl
--rw-r--r--   0        0        0     3561 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/tclIndex
--rw-r--r--   0        0        0    14936 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbCommon.tcl
--rw-r--r--   0        0        0    11684 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbEntry.tcl
--rw-r--r--   0        0        0     2174 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbListbox.tcl
--rw-r--r--   0        0        0     3247 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl
--rw-r--r--   0        0        0     6860 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbText.tcl
--rw-r--r--   0        0        0     2701 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl
--rw-r--r--   0        0        0     1839 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/wcb.tcl
--rw-r--r--   0        0        0     3866 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/arrowb.tcl
--rw-r--r--   0        0        0    20697 2013-03-26 03:28:23.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/calendar.tcl
--rw-r--r--   0        0        0    10039 2013-03-26 03:28:23.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/dateentry.tcl
--rw-r--r--   0        0        0    14200 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/dialog.tcl
--rw-r--r--   0        0        0     9158 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/mentry.tcl
--rw-r--r--   0        0        0     6617 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/panelframe.tcl
--rw-r--r--   0        0        0     1144 2013-03-26 03:28:23.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/pkgIndex.tcl
--rw-r--r--   0        0        0    18647 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/ruler.tcl
--rw-r--r--   0        0        0     7563 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/scrollw.tcl
--rw-r--r--   0        0        0     8025 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/statusbar.tcl
--rw-r--r--   0        0        0     2093 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/stext.tcl
--rw-r--r--   0        0        0     3927 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/superframe.tcl
--rw-r--r--   0        0        0     7915 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/toolbar.tcl
--rw-r--r--   0        0        0     4374 2023-04-29 05:46:59.130164 tkfly-0.1.0a2/tkfly/_tklib/widget/widget.tcl
--rw-r--r--   0        0        0    32987 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetl/listentry.tcl
--rw-r--r--   0        0        0    18733 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetl/listsimple.tcl
--rw-r--r--   0        0        0      237 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetl/pkgIndex.tcl
--rw-r--r--   0        0        0      142 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetPlus/pkgIndex.tcl
--rw-r--r--   0        0        0    57846 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetPlus/widgetPlus.tcl
--rw-r--r--   0        0        0      146 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetv/pkgIndex.tcl
--rw-r--r--   0        0        0    12031 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetv/validator.tcl
--rw-r--r--   0        0        0      224 2023-04-29 07:23:36.893330 tkfly-0.1.0a2/tkfly/_twapi/__init__.py
--rw-r--r--   0        0        0      677 2023-04-29 07:27:32.485989 tkfly-0.1.0a2/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    35822 2021-11-07 07:09:24.000000 tkfly-0.1.0a2/tkfly/_twapi/account.tcl
--rw-r--r--   0        0        0      721 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/adsi.tcl
--rw-r--r--   0        0        0     3004 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/apputil.tcl
--rw-r--r--   0        0        0    63943 2021-11-09 02:43:04.000000 tkfly-0.1.0a2/tkfly/_twapi/base.tcl
--rw-r--r--   0        0        0     7099 2022-06-04 05:48:24.000000 tkfly-0.1.0a2/tkfly/_twapi/clipboard.tcl
--rw-r--r--   0        0        0   149879 2021-11-02 05:34:50.000000 tkfly-0.1.0a2/tkfly/_twapi/com.tcl
--rw-r--r--   0        0        0    24031 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/console.tcl
--rw-r--r--   0        0        0   118653 2022-06-03 06:01:30.000000 tkfly-0.1.0a2/tkfly/_twapi/crypto.tcl
--rw-r--r--   0        0        0    22667 2022-06-04 15:03:22.000000 tkfly-0.1.0a2/tkfly/_twapi/device.tcl
--rw-r--r--   0        0        0    51643 2020-10-09 10:08:22.000000 tkfly-0.1.0a2/tkfly/_twapi/etw.tcl
--rw-r--r--   0        0        0    14722 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/eventlog.tcl
--rw-r--r--   0        0        0    23130 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/evt.tcl
--rw-r--r--   0        0        0     7268 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/handle.tcl
--rw-r--r--   0        0        0    24383 2020-06-24 02:08:54.000000 tkfly-0.1.0a2/tkfly/_twapi/input.tcl
--rw-r--r--   0        0        0     1480 2019-07-25 11:50:02.000000 tkfly-0.1.0a2/tkfly/_twapi/LICENSE
--rw-r--r--   0        0        0    23492 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/metoo.tcl
--rw-r--r--   0        0        0    37265 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/msi.tcl
--rw-r--r--   0        0        0    22693 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/mstask.tcl
--rw-r--r--   0        0        0     1793 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/multimedia.tcl
--rw-r--r--   0        0        0     3535 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/namedpipe.tcl
--rw-r--r--   0        0        0    37061 2020-10-14 07:59:02.000000 tkfly-0.1.0a2/tkfly/_twapi/network.tcl
--rw-r--r--   0        0        0    17196 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/nls.tcl
--rw-r--r--   0        0        0    43660 2022-06-04 00:12:28.000000 tkfly-0.1.0a2/tkfly/_twapi/os.tcl
--rw-r--r--   0        0        0    34543 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/pdh.tcl
--rw-r--r--   0        0        0     7293 2022-06-22 13:03:38.000000 tkfly-0.1.0a2/tkfly/_twapi/pkgIndex.tcl
--rw-r--r--   0        0        0     3758 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/power.tcl
--rw-r--r--   0        0        0     1802 2020-06-23 03:12:46.000000 tkfly-0.1.0a2/tkfly/_twapi/printer.tcl
--rw-r--r--   0        0        0    69738 2022-06-03 07:57:36.000000 tkfly-0.1.0a2/tkfly/_twapi/process.tcl
--rw-r--r--   0        0        0     6602 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/rds.tcl
--rw-r--r--   0        0        0     2037 2022-06-22 09:04:10.000000 tkfly-0.1.0a2/tkfly/_twapi/README.md
--rw-r--r--   0        0        0    13900 2022-06-03 13:37:40.000000 tkfly-0.1.0a2/tkfly/_twapi/registry.tcl
--rw-r--r--   0        0        0    18583 2022-06-04 12:13:10.000000 tkfly-0.1.0a2/tkfly/_twapi/resource.tcl
--rw-r--r--   0        0        0    76964 2021-11-06 08:18:08.000000 tkfly-0.1.0a2/tkfly/_twapi/security.tcl
--rw-r--r--   0        0        0    40542 2022-06-04 14:46:44.000000 tkfly-0.1.0a2/tkfly/_twapi/service.tcl
--rw-r--r--   0        0        0    30062 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/share.tcl
--rw-r--r--   0        0        0    19297 2020-12-15 00:37:00.000000 tkfly-0.1.0a2/tkfly/_twapi/shell.tcl
--rw-r--r--   0        0        0    28334 2022-06-04 12:24:36.000000 tkfly-0.1.0a2/tkfly/_twapi/sspi.tcl
--rw-r--r--   0        0        0    20059 2022-06-05 01:39:28.000000 tkfly-0.1.0a2/tkfly/_twapi/storage.tcl
--rw-r--r--   0        0        0     2632 2020-07-01 00:57:00.000000 tkfly-0.1.0a2/tkfly/_twapi/synch.tcl
--rw-r--r--   0        0        0    49870 2022-06-22 10:37:46.000000 tkfly-0.1.0a2/tkfly/_twapi/tls.tcl
--rw-r--r--   0        0        0    26955 2020-06-22 09:54:26.000000 tkfly-0.1.0a2/tkfly/_twapi/twapi.tcl
--rw-r--r--   0        0        0   389718 2022-06-22 13:03:36.000000 tkfly-0.1.0a2/tkfly/_twapi/twapi_base.dll
--rw-r--r--   0        0        0   516096 2022-06-22 12:59:36.000000 tkfly-0.1.0a2/tkfly/_twapi/twapi_base64.dll
--rw-r--r--   0        0        0    42512 2022-06-04 14:52:14.000000 tkfly-0.1.0a2/tkfly/_twapi/ui.tcl
--rw-r--r--   0        0        0     4286 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/win.tcl
--rw-r--r--   0        0        0    10975 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/winlog.tcl
--rw-r--r--   0        0        0     3148 2022-06-04 03:20:02.000000 tkfly-0.1.0a2/tkfly/_twapi/winsta.tcl
--rw-r--r--   0        0        0     6978 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/wmi.tcl
--rw-r--r--   0        0        0     2217 2023-04-19 11:11:33.981831 tkfly-0.1.0a2/tkfly/core.py
--rw-r--r--   0        0        0      222 2023-04-14 12:59:16.512351 tkfly-0.1.0a2/tkfly/tkimg/__init__.py
--rw-r--r--   0        0        0   221710 2022-11-24 07:55:52.000000 tkfly-0.1.0a2/tkfly/tkimg/jpegtcl950.dll
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libjpegtclstub950.a
--rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libpngtclstub1638.a
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libtifftclstub440.a
--rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libtkimgstub1414.a
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libzlibtclstub1213.a
--rw-r--r--   0        0        0     6851 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/pkgIndex.tcl
--rw-r--r--   0        0        0   231950 2022-11-24 07:55:52.000000 tkfly-0.1.0a2/tkfly/tkimg/pngtcl1638.dll
--rw-r--r--   0        0        0   416782 2022-11-24 07:55:52.000000 tkfly-0.1.0a2/tkfly/tkimg/tifftcl440.dll
--rw-r--r--   0        0        0    40462 2022-11-24 07:55:54.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimg1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:54.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgbmp1414.dll
--rw-r--r--   0        0        0    22030 2022-11-24 07:55:54.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgdted1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:56.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgflir1414.dll
--rw-r--r--   0        0        0    24590 2022-11-24 07:55:56.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimggif1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:56.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgico1414.dll
--rw-r--r--   0        0        0    23054 2022-11-24 07:55:56.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgjpeg1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgpcx1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:58.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgpixmap1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgpng1414.dll
--rw-r--r--   0        0        0    25102 2022-11-24 07:56:00.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgppm1414.dll
--rw-r--r--   0        0        0    21006 2022-11-24 07:56:00.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgps1414.dll
--rw-r--r--   0        0        0    31758 2022-11-24 07:56:00.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgraw1414.dll
--rw-r--r--   0        0        0    28174 2022-11-24 07:56:02.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgsgi1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:56:02.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgsun1414.dll
--rw-r--r--   0        0        0    25102 2022-11-24 07:56:02.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgtga1414.dll
--rw-r--r--   0        0        0    70158 2022-11-24 07:56:04.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgtiff1414.dll
--rw-r--r--   0        0        0    17934 2022-11-24 07:56:04.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgwindow1414.dll
--rw-r--r--   0        0        0    19470 2022-11-24 07:56:04.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgxbm1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:56:06.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgxpm1414.dll
--rw-r--r--   0        0        0    91662 2022-11-24 07:56:06.000000 tkfly-0.1.0a2/tkfly/tkimg/zlibtcl1213.dll
--rw-r--r--   0        0        0        0 2023-04-19 11:17:10.457150 tkfly-0.1.0a2/tkfly/tklib/__init__.py
--rw-r--r--   0        0        0      141 2023-04-19 12:43:56.373512 tkfly-0.1.0a2/tkfly/tklib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2594 2023-04-29 11:00:59.295786 tkfly-0.1.0a2/tkfly/tklib/__pycache__/datefield.cpython-311.pyc
--rw-r--r--   0        0        0     8914 2023-04-29 05:02:59.020777 tkfly-0.1.0a2/tkfly/tklib/__pycache__/history.cpython-311.pyc
--rw-r--r--   0        0        0     3960 2023-04-19 12:45:43.059958 tkfly-0.1.0a2/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc
--rw-r--r--   0        0        0      538 2023-04-29 05:32:30.677805 tkfly-0.1.0a2/tkfly/tklib/autoscroll.py
--rw-r--r--   0        0        0      573 2023-04-19 14:52:50.309476 tkfly-0.1.0a2/tkfly/tklib/chatwidget.py
--rw-r--r--   0        0        0     1265 2023-04-29 10:59:14.922692 tkfly-0.1.0a2/tkfly/tklib/datefield.py
--rw-r--r--   0        0        0     5389 2023-04-29 05:02:58.918925 tkfly-0.1.0a2/tkfly/tklib/history.py
--rw-r--r--   0        0        0      583 2023-04-19 12:47:17.815625 tkfly-0.1.0a2/tkfly/tklib/menubar.py
--rw-r--r--   0        0        0     1002 2023-04-29 05:26:07.066657 tkfly-0.1.0a2/tkfly/tklib/notifywindow.py
--rw-r--r--   0        0        0     1331 2023-04-29 06:07:26.214511 tkfly-0.1.0a2/tkfly/tklib/plotchart.py
--rw-r--r--   0        0        0     5389 2023-04-29 05:38:33.820659 tkfly-0.1.0a2/tkfly/tklib/shtmlview.py
--rw-r--r--   0        0        0     2066 2023-04-19 12:45:42.877555 tkfly-0.1.0a2/tkfly/tklib/tooltip.py
--rw-r--r--   0        0        0      902 2023-04-19 11:28:27.786655 tkfly-0.1.0a2/tkfly/tklib/wcb.py
--rw-r--r--   0        0        0      523 2023-04-29 05:46:46.161323 tkfly-0.1.0a2/tkfly/tklib/widget.py
--rw-r--r--   0        0        0      506 2023-04-29 11:29:28.404486 tkfly-0.1.0a2/tkfly/tkscrollutil/__init__.py
--rw-r--r--   0        0        0      804 2023-04-29 11:29:28.606524 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1165 2023-04-29 11:09:26.181908 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc
--rw-r--r--   0        0        0     1258 2023-04-29 11:29:43.706687 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc
--rw-r--r--   0        0        0     3023 2023-04-29 11:14:55.822881 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc
--rw-r--r--   0        0        0     4204 2023-04-29 11:12:49.744284 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc
--rw-r--r--   0        0        0     3011 2023-04-29 11:29:28.610040 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc
--rw-r--r--   0        0        0     2069 2023-04-29 11:34:46.885357 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc
--rw-r--r--   0        0        0     3060 2023-04-29 11:26:17.297437 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2023-04-29 11:29:28.614038 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc
--rw-r--r--   0        0        0      413 2022-10-29 06:29:19.142527 tkfly-0.1.0a2/tkfly/tkscrollutil/attrib.py
--rw-r--r--   0        0        0      458 2023-04-29 11:29:43.603589 tkfly-0.1.0a2/tkfly/tkscrollutil/load.py
--rw-r--r--   0        0        0     1886 2023-04-29 11:24:25.427936 tkfly-0.1.0a2/tkfly/tkscrollutil/scrollableframe.py
--rw-r--r--   0        0        0     1921 2023-04-29 11:14:55.722630 tkfly-0.1.0a2/tkfly/tkscrollutil/scrollarea.py
--rw-r--r--   0        0        0     2480 2023-04-29 11:10:41.419659 tkfly-0.1.0a2/tkfly/tkscrollutil/scrollsync.py
--rw-r--r--   0        0        0     1910 2023-04-29 11:29:28.409999 tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollarea.py
--rw-r--r--   0        0        0     1142 2023-04-29 11:34:46.766705 tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollednotebook.py
--rw-r--r--   0        0        0     1689 2023-04-29 11:26:17.197236 tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollsync.py
--rw-r--r--   0        0        0     1435 2023-04-29 11:28:26.430882 tkfly-0.1.0a2/tkfly/tkscrollutil/wheelevent.py
--rw-r--r--   0        0        0      544 2023-04-29 11:43:18.104764 tkfly-0.1.0a2/tkfly/twapi/__init__.py
--rw-r--r--   0        0        0     1464 2023-04-29 11:43:18.209994 tkfly-0.1.0a2/tkfly/twapi/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      359 2023-04-29 07:58:45.679468 tkfly-0.1.0a2/tkfly/twapi/base.py
--rw-r--r--   0        0        0      230 2023-04-29 07:58:45.713014 tkfly-0.1.0a2/tkfly/twapi/msi.py
--rw-r--r--   0        0        0      704 2023-04-29 10:07:46.018924 tkfly-0.1.0a2/tkfly/twapi/ui.py
--rw-r--r--   0        0        0      585 2023-04-29 08:16:43.020235 tkfly-0.1.0a2/tkfly/twapi/win.py
--rw-r--r--   0        0        0     6773 1970-01-01 00:00:00.000000 tkfly-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      280 2023-04-30 02:01:10.901849 tkfly-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     7415 2023-04-30 02:00:57.214361 tkfly-0.1.0a3/README.md
+-rw-r--r--   0        0        0      757 2023-04-30 01:01:58.479143 tkfly-0.1.0a3/tkfly/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-29 10:25:40.967581 tkfly-0.1.0a3/tkfly/__main__.py
+-rw-r--r--   0        0        0  1739496 2023-04-15 14:33:36.000000 tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libblend2d.dylib
+-rw-r--r--   0        0        0   150336 2023-04-15 14:33:36.000000 tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libtclb2d.dylib
+-rw-r--r--   0        0        0   168576 2023-04-15 14:33:36.000000 tkfly-0.1.0a3/tkfly/_blend2d/darwin-x64/libtkb2d.dylib
+-rw-r--r--   0        0        0    51952 2018-05-12 08:44:20.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Blacksword.otf
+-rw-r--r--   0        0        0      139 2020-03-05 14:21:50.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/chessboard.png
+-rw-r--r--   0        0        0    10845 2020-03-08 17:01:24.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/CMYK.png
+-rw-r--r--   0        0        0     4335 2020-05-14 16:48:44.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/CompositionTest.tcl
+-rw-r--r--   0        0        0     7576 2020-05-14 16:47:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/PorterDuffInAction.tcl
+-rw-r--r--   0        0        0     9507 2020-03-08 17:06:24.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/comp-op/RGB.png
+-rw-r--r--   0        0        0     5298 2020-08-12 14:00:30.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/demo-tiger.tcl
+-rw-r--r--   0        0        0   175050 2019-10-09 17:27:50.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/bl-qt-tiger.h
+-rw-r--r--   0        0        0    68630 2019-09-16 05:50:56.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/Ghostscript_Tiger.svg
+-rw-r--r--   0        0        0     3368 2019-10-18 06:47:24.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.cpp
+-rwxr-xr-x   0        0        0   174080 2019-10-15 16:30:08.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/develTools/tiger-conversion.exe
+-rw-r--r--   0        0        0   220752 2019-10-15 16:31:28.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/demo-tiger/tiger-data.tcl
+-rw-r--r--   0        0        0     3873 2020-06-23 06:06:42.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/greenSlate.jpg
+-rw-r--r--   0        0        0     5415 2020-09-03 09:32:10.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/EbuttonColor-1.0.1.tm
+-rw-r--r--   0        0        0     4958 2020-09-03 09:38:00.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/Eseparator-1.0.tm
+-rw-r--r--   0        0        0     5965 2020-08-26 14:52:44.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/hatching-1.0.tm
+-rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/IKscale-1.0.1.tm
+-rw-r--r--   0        0        0    33360 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/darwin-x64/perlin.dylib
+-rw-r--r--   0        0        0      513 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/license.terms
+-rw-r--r--   0        0        0    11404 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x32/perlin.so
+-rw-r--r--   0        0        0    12456 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/linux-x64/perlin.so
+-rw-r--r--   0        0        0     1149 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/pkgIndex.tcl
+-rw-r--r--   0        0        0    11776 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/win-x32/perlin.dll
+-rw-r--r--   0        0        0    13312 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/perlin-1.0/win-x64/perlin.dll
+-rw-r--r--   0        0        0    12189 2020-08-28 04:04:42.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/sketchline-1.0.tm
+-rw-r--r--   0        0        0   125189 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/main2.tcl
+-rw-r--r--   0        0        0     1052 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/pkgIndex.tcl
+-rw-r--r--   0        0        0      769 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/snit2.tcl
+-rw-r--r--   0        0        0      510 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/teapot.txt
+-rw-r--r--   0        0        0    18959 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/snit.2.3.2/validate.tcl
+-rw-r--r--   0        0        0    14134 2021-12-02 19:08:46.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/lib/Spline-1.0.tm
+-rw-r--r--   0        0        0    17997 2023-03-14 07:49:04.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/moby.svg
+-rw-r--r--   0        0        0    22057 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_1.svg
+-rw-r--r--   0        0        0    29922 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_2.svg
+-rw-r--r--   0        0        0    22020 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_3.svg
+-rw-r--r--   0        0        0    23936 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_4.svg
+-rw-r--r--   0        0        0    16595 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_5.svg
+-rw-r--r--   0        0        0      279 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Q/layer_6.svg
+-rw-r--r--   0        0        0      436 2016-06-18 19:26:30.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Road_Rage-License.txt
+-rw-r--r--   0        0        0   341760 2016-06-18 17:26:30.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/Road_Rage.otf
+-rw-r--r--   0        0        0     4861 2020-08-12 16:10:38.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample-poly.tcl
+-rw-r--r--   0        0        0     4989 2020-08-12 13:52:06.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample-rect.tcl
+-rw-r--r--   0        0        0      461 2023-04-29 15:43:17.299023 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample01.tcl
+-rw-r--r--   0        0        0      443 2020-04-25 17:15:52.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample02.tcl
+-rw-r--r--   0        0        0      392 2020-04-25 17:15:32.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample03.tcl
+-rw-r--r--   0        0        0      754 2021-08-24 13:22:40.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample04i.tcl
+-rw-r--r--   0        0        0     1660 2020-04-25 17:24:14.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample04ii.tcl
+-rw-r--r--   0        0        0      579 2020-07-16 15:31:02.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample05.tcl
+-rw-r--r--   0        0        0      621 2020-05-07 08:13:30.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample06.tcl
+-rw-r--r--   0        0        0      718 2020-05-14 15:18:06.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample07.tcl
+-rw-r--r--   0        0        0     2161 2020-05-14 15:16:08.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample101.tcl
+-rw-r--r--   0        0        0     6635 2022-12-23 15:25:00.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample102.tcl
+-rw-r--r--   0        0        0     2946 2020-09-02 17:00:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103.tcl
+-rw-r--r--   0        0        0     3074 2021-08-24 13:03:58.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103a.tcl
+-rw-r--r--   0        0        0     4231 2021-08-24 13:07:52.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample103b.tcl
+-rw-r--r--   0        0        0     8403 2020-09-04 06:06:22.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample104-handmadelines.tcl
+-rw-r--r--   0        0        0     3006 2023-04-11 10:02:10.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample105-SVGmoby.tcl
+-rw-r--r--   0        0        0     3392 2022-05-15 17:34:40.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample106.tcl
+-rw-r--r--   0        0        0     2375 2022-01-03 04:49:40.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample107.tcl
+-rw-r--r--   0        0        0     4366 2022-01-03 04:48:10.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample108.tcl
+-rw-r--r--   0        0        0     2992 2023-04-15 16:03:48.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample109.tcl
+-rw-r--r--   0        0        0     4160 2023-04-15 14:44:48.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample110.tcl
+-rw-r--r--   0        0        0     3662 2023-04-15 19:37:46.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/sample111.tcl
+-rw-r--r--   0        0        0    76248 2019-08-19 07:45:32.000000 tkfly-0.1.0a3/tkfly/_blend2d/demo/texture.jpeg
+-rw-r--r--   0        0        0    85398 2023-04-15 17:26:48.000000 tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.html
+-rw-r--r--   0        0        0    47336 2023-04-15 17:26:36.000000 tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.man
+-rw-r--r--   0        0        0    46275 2023-04-15 17:26:50.000000 tkfly-0.1.0a3/tkfly/_blend2d/docs/tclBlend2d.wiki.txt
+-rw-r--r--   0        0        0     3283 2020-06-26 04:05:56.000000 tkfly-0.1.0a3/tkfly/_blend2d/HSB.tcl
+-rw-r--r--   0        0        0  1947176 2023-04-15 14:12:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libblend2d.so
+-rw-r--r--   0        0        0   221592 2023-04-15 14:12:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libtclb2d.so
+-rw-r--r--   0        0        0   235800 2023-04-15 14:12:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/linux-x64/libtkb2d.so
+-rw-r--r--   0        0        0     6274 2020-06-21 16:12:56.000000 tkfly-0.1.0a3/tkfly/_blend2d/Mtx.tcl
+-rw-r--r--   0        0        0     1044 2023-04-08 17:37:10.000000 tkfly-0.1.0a3/tkfly/_blend2d/pkgIndex.tcl
+-rw-r--r--   0        0        0     6003 2023-04-11 14:15:12.000000 tkfly-0.1.0a3/tkfly/_blend2d/SVGpath.tcl
+-rw-r--r--   0        0        0     5983 2023-04-12 14:44:44.000000 tkfly-0.1.0a3/tkfly/_blend2d/t2d.tcl
+-rw-r--r--   0        0        0     7462 2023-04-15 19:35:42.000000 tkfly-0.1.0a3/tkfly/_blend2d/t2d_filters.tcl
+-rw-r--r--   0        0        0     6750 2023-04-08 17:29:54.000000 tkfly-0.1.0a3/tkfly/_blend2d/t2dsvg.tcl
+-rw-r--r--   0        0        0      826 2020-07-09 13:31:32.000000 tkfly-0.1.0a3/tkfly/_blend2d/tclBlend2D-license.terms
+-rw-r--r--   0        0        0  1350656 2023-04-15 11:18:54.000000 tkfly-0.1.0a3/tkfly/_blend2d/win-x64/blend2d.dll
+-rw-r--r--   0        0        0   138240 2023-04-15 15:25:58.000000 tkfly-0.1.0a3/tkfly/_blend2d/win-x64/tclb2d.dll
+-rw-r--r--   0        0        0   146944 2023-04-15 15:25:58.000000 tkfly-0.1.0a3/tkfly/_blend2d/win-x64/tkb2d.dll
+-rw-r--r--   0        0        0     1005 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/CHANGES.txt
+-rw-r--r--   0        0        0   124568 2021-03-11 08:11:16.000000 tkfly-0.1.0a3/tkfly/_mupdf/demo/demo.pdf
+-rw-r--r--   0        0        0     4292 2021-11-07 08:03:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/demo/demo.tcl
+-rw-r--r--   0        0        0     6150 2021-11-07 08:08:52.000000 tkfly-0.1.0a3/tkfly/_mupdf/demo/demo_sharedPdf.tcl
+-rw-r--r--   0        0        0    26755 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/docs/MuPDFWidget.html
+-rw-r--r--   0        0        0    14092 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/docs/MuPDFWidget.man
+-rw-r--r--   0        0        0      314 2021-03-11 08:27:06.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/Readme.txt
+-rw-r--r--   0        0        0   125189 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/main2.tcl
+-rw-r--r--   0        0        0     1052 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/pkgIndex.tcl
+-rw-r--r--   0        0        0      769 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/snit2.tcl
+-rw-r--r--   0        0        0      510 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/teapot.txt
+-rw-r--r--   0        0        0    18959 2012-03-30 13:55:46.000000 tkfly-0.1.0a3/tkfly/_mupdf/lib/snit-2.3.2/validate.tcl
+-rw-r--r--   0        0        0    37749 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/MuPDFWidget.tcl
+-rw-r--r--   0        0        0       69 2021-11-07 07:32:30.000000 tkfly-0.1.0a3/tkfly/_mupdf/pkgIndex.tcl
+-rw-r--r--   0        0        0      224 2023-04-19 11:06:45.090485 tkfly-0.1.0a3/tkfly/_tklib/__init__.py
+-rw-r--r--   0        0        0      677 2023-04-19 11:08:58.393781 tkfly-0.1.0a3/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1667 2023-04-14 12:45:42.167394 tkfly-0.1.0a3/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7112 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/autoscroll/autoscroll.tcl
+-rw-r--r--   0        0        0      611 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/autoscroll/pkgIndex.tcl
+-rw-r--r--   0        0        0     7344 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_drag.tcl
+-rw-r--r--   0        0        0    10374 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_epoints.tcl
+-rw-r--r--   0        0        0    12828 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_epolyline.tcl
+-rw-r--r--   0        0        0    11211 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_equad.tcl
+-rw-r--r--   0        0        0     7467 2014-08-11 05:20:11.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_gradient.tcl
+-rw-r--r--   0        0        0     2947 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_highlight.tcl
+-rw-r--r--   0        0        0     9922 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_mvg.tcl
+-rw-r--r--   0        0        0     2964 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_snap.tcl
+-rw-r--r--   0        0        0    21321 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_sqmap.tcl
+-rw-r--r--   0        0        0     1545 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_tags.tcl
+-rw-r--r--   0        0        0     2195 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_trlines.tcl
+-rw-r--r--   0        0        0     5161 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_zoom.tcl
+-rw-r--r--   0        0        0     1295 2014-08-11 05:20:11.000000 tkfly-0.1.0a3/tkfly/_tklib/canvas/pkgIndex.tcl
+-rw-r--r--   0        0        0    26671 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/chatwidget/chatwidget.tcl
+-rw-r--r--   0        0        0       80 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/chatwidget/pkgIndex.tcl
+-rw-r--r--   0        0        0     1365 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/bindDown.tcl
+-rw-r--r--   0        0        0      381 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/controlwidget.tcl
+-rw-r--r--   0        0        0     3401 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/led.tcl
+-rw-r--r--   0        0        0      903 2018-05-11 03:56:07.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/pkgIndex.tcl
+-rw-r--r--   0        0        0     7666 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/radioMatrix.tcl
+-rw-r--r--   0        0        0    16186 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/rdial.tcl
+-rw-r--r--   0        0        0    12150 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/tachometer.tcl
+-rw-r--r--   0        0        0    48034 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/vertical_meter.tcl
+-rw-r--r--   0        0        0    11332 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/controlwidget/voltmeter.tcl
+-rw-r--r--   0        0        0    16207 2014-08-11 05:20:11.000000 tkfly-0.1.0a3/tkfly/_tklib/crosshair/crosshair.tcl
+-rw-r--r--   0        0        0      138 2013-05-10 05:18:16.000000 tkfly-0.1.0a3/tkfly/_tklib/crosshair/pkgIndex.tcl
+-rw-r--r--   0        0        0    27293 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ctext/ctext.tcl
+-rw-r--r--   0        0        0       68 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ctext/pkgIndex.tcl
+-rw-r--r--   0        0        0     3924 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/cursor/cursor.tcl
+-rw-r--r--   0        0        0       72 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/cursor/pkgIndex.tcl
+-rw-r--r--   0        0        0    12481 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/datefield/datefield.tcl
+-rw-r--r--   0        0        0       76 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/datefield/pkgIndex.tcl
+-rw-r--r--   0        0        0    12537 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/application.tcl
+-rw-r--r--   0        0        0    10383 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/attributes.tcl
+-rw-r--r--   0        0        0    37096 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/basic.tcl
+-rw-r--r--   0        0        0    32433 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/core.tcl
+-rw-r--r--   0        0        0     1557 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/diagram.tcl
+-rw-r--r--   0        0        0     7807 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/direction.tcl
+-rw-r--r--   0        0        0     7931 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/element.tcl
+-rw-r--r--   0        0        0     3423 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/navigation.tcl
+-rw-r--r--   0        0        0      847 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/pkgIndex.tcl
+-rw-r--r--   0        0        0     4837 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/diagrams/point.tcl
+-rw-r--r--   0        0        0      612 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/getstring/pkgIndex.tcl
+-rw-r--r--   0        0        0     4224 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/getstring/tk_getString.tcl
+-rw-r--r--   0        0        0     3187 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/history/history.tcl
+-rw-r--r--   0        0        0      605 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/history/pkgIndex.tcl
+-rw-r--r--   0        0        0    44954 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ico/ico.tcl
+-rw-r--r--   0        0        0    35176 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ico/ico0.tcl
+-rw-r--r--   0        0        0      292 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ico/pkgIndex.tcl
+-rw-r--r--   0        0        0    29231 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ipentry/ipentry.tcl
+-rw-r--r--   0        0        0      139 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/ipentry/pkgIndex.tcl
+-rw-r--r--   0        0        0     3795 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/cs.msg
+-rw-r--r--   0        0        0     3718 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/da.msg
+-rw-r--r--   0        0        0     4409 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/de.msg
+-rw-r--r--   0        0        0     3918 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/en.msg
+-rw-r--r--   0        0        0     3979 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/es.msg
+-rw-r--r--   0        0        0    56665 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/khim.tcl
+-rw-r--r--   0        0        0      534 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/pkgIndex.tcl
+-rw-r--r--   0        0        0     4124 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/pl.msg
+-rw-r--r--   0        0        0     2937 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/ROOT.msg
+-rw-r--r--   0        0        0     6679 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/ru.msg
+-rw-r--r--   0        0        0     6361 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/khim/uk.msg
+-rw-r--r--   0        0        0      444 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/mentry.tcl
+-rw-r--r--   0        0        0      737 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/mentry_tile.tcl
+-rw-r--r--   0        0        0     2592 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/mentryPublic.tcl
+-rw-r--r--   0        0        0      860 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/pkgIndex.tcl
+-rw-r--r--   0        0        0    25858 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl
+-rw-r--r--   0        0        0     4298 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl
+-rw-r--r--   0        0        0     5661 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl
+-rw-r--r--   0        0        0     6884 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl
+-rw-r--r--   0        0        0    18737 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryThemes.tcl
+-rw-r--r--   0        0        0    60325 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryWidget.tcl
+-rw-r--r--   0        0        0    19506 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mwutil.tcl
+-rw-r--r--   0        0        0    10636 2020-01-06 23:27:53.000000 tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/tclIndex
+-rw-r--r--   0        0        0     5469 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/debug.tcl
+-rw-r--r--   0        0        0    53951 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/menubar.tcl
+-rw-r--r--   0        0        0     3859 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/node.tcl
+-rw-r--r--   0        0        0      299 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/pkgIndex.tcl
+-rw-r--r--   0        0        0    26016 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/menubar/tree.tcl
+-rw-r--r--   0        0        0     4015 2023-04-29 05:27:10.370187 tkfly-0.1.0a3/tkfly/_tklib/notifywindow/notifywindow.tcl
+-rw-r--r--   0        0        0      548 2016-07-14 05:57:54.000000 tkfly-0.1.0a3/tkfly/_tklib/notifywindow/pkgIndex.tcl
+-rw-r--r--   0        0        0   120514 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/ntext/ntext.tcl
+-rw-r--r--   0        0        0      132 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/ntext/pkgIndex.tcl
+-rw-r--r--   0        0        0    30859 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/persistentSelection/persistentSelection.tcl
+-rw-r--r--   0        0        0      160 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/persistentSelection/pkgIndex.tcl
+-rw-r--r--   0        0        0     3291 2023-04-14 12:33:32.365933 tkfly-0.1.0a3/tkfly/_tklib/pkgIndex.tcl
+-rw-r--r--   0        0        0      321 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/pkgIndex.tcl
+-rw-r--r--   0        0        0    13471 2015-04-21 06:10:00.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plot3d.tcl
+-rw-r--r--   0        0        0    15740 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotanim.tcl
+-rw-r--r--   0        0        0    12916 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotannot.tcl
+-rw-r--r--   0        0        0    67951 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotaxis.tcl
+-rw-r--r--   0        0        0     6478 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotbind.tcl
+-rw-r--r--   0        0        0    11059 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotbusiness.tcl
+-rw-r--r--   0        0        0   108162 2019-08-21 18:42:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotchart.tcl
+-rw-r--r--   0        0        0     5721 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotcombined.tcl
+-rw-r--r--   0        0        0    16783 2015-04-21 06:10:00.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotconfig.tcl
+-rw-r--r--   0        0        0    61163 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotcontour.tcl
+-rw-r--r--   0        0        0    10041 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotgantt.tcl
+-rw-r--r--   0        0        0     8895 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotobject.tcl
+-rw-r--r--   0        0        0     9423 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotpack.tcl
+-rw-r--r--   0        0        0   139321 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotpriv.tcl
+-rw-r--r--   0        0        0     8072 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotscada.tcl
+-rw-r--r--   0        0        0     5697 2016-07-14 05:57:54.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotspecial.tcl
+-rw-r--r--   0        0        0     7475 2014-08-11 05:20:12.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotstatustimeline.tcl
+-rw-r--r--   0        0        0     9893 2015-04-21 06:10:00.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/plottable.tcl
+-rw-r--r--   0        0        0     5215 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/scaling.tcl
+-rw-r--r--   0        0        0    16372 2014-11-24 17:34:56.000000 tkfly-0.1.0a3/tkfly/_tklib/plotchart/xyplot.tcl
+-rw-r--r--   0        0        0      867 2022-07-14 16:02:02.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/pkgIndex.tcl
+-rw-r--r--   0        0        0     2420 2022-08-15 11:36:06.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/attrib.tcl
+-rw-r--r--   0        0        0    19506 2020-01-08 04:03:39.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/mwutil.tcl
+-rw-r--r--   0        0        0    16416 2022-04-25 10:54:58.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl
+-rw-r--r--   0        0        0    25675 2022-08-23 17:53:48.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/pagesman.tcl
+-rw-r--r--   0        0        0    53698 2022-08-23 18:08:46.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl
+-rw-r--r--   0        0        0    36010 2022-08-17 10:02:40.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl
+-rw-r--r--   0        0        0    36693 2022-08-17 10:03:10.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl
+-rw-r--r--   0        0        0    57949 2022-09-11 08:36:20.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl
+-rw-r--r--   0        0        0    18623 2022-08-17 10:05:36.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl
+-rw-r--r--   0        0        0    19056 2022-08-15 19:39:16.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/tclIndex
+-rw-r--r--   0        0        0        0 2022-10-29 06:04:07.908293 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/__init__.py
+-rw-r--r--   0        0        0    21894 2022-05-20 15:38:54.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl
+-rw-r--r--   0        0        0      537 2022-10-19 15:21:54.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl
+-rw-r--r--   0        0        0    22642 2022-05-29 18:19:18.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl
+-rw-r--r--   0        0        0    51787 2022-10-22 15:11:52.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl
+-rw-r--r--   0        0        0    27243 2022-04-10 15:20:18.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl
+-rw-r--r--   0        0        0      686 2022-07-14 16:02:24.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutil.tcl
+-rw-r--r--   0        0        0     1138 2022-07-14 16:03:16.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutil_tile.tcl
+-rw-r--r--   0        0        0     3214 2022-10-18 14:23:10.000000 tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutilCommon.tcl
+-rw-r--r--   0        0        0    15316 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/style/as.tcl
+-rw-r--r--   0        0        0     2848 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/style/lobster.tcl
+-rw-r--r--   0        0        0      684 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/style/pkgIndex.tcl
+-rw-r--r--   0        0        0      765 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/style/style.tcl
+-rw-r--r--   0        0        0      607 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/swaplist/pkgIndex.tcl
+-rw-r--r--   0        0        0    13365 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/swaplist/swaplist.tcl
+-rw-r--r--   0        0        0      898 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/pkgIndex.tcl
+-rw-r--r--   0        0        0    19506 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/mwutil.tcl
+-rw-r--r--   0        0        0     4286 2015-04-21 06:10:00.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/pencil.cur
+-rw-r--r--   0        0        0     2911 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/repair.tcl
+-rw-r--r--   0        0        0   133438 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl
+-rw-r--r--   0        0        0   120387 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl
+-rw-r--r--   0        0        0    93461 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl
+-rw-r--r--   0        0        0   125609 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl
+-rw-r--r--   0        0        0    17564 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl
+-rw-r--r--   0        0        0    20512 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl
+-rw-r--r--   0        0        0    68715 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl
+-rw-r--r--   0        0        0   202524 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl
+-rw-r--r--   0        0        0   267492 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl
+-rw-r--r--   0        0        0    62720 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tclIndex
+-rw-r--r--   0        0        0      488 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelist.tcl
+-rw-r--r--   0        0        0      763 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelist_tile.tcl
+-rw-r--r--   0        0        0     3022 2020-01-06 23:27:54.000000 tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelistPublic.tcl
+-rw-r--r--   0        0        0     4807 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/boxlabel.tcl
+-rw-r--r--   0        0        0     7705 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/canlabel.tcl
+-rw-r--r--   0        0        0     3303 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/labarray.tcl
+-rw-r--r--   0        0        0     1185 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/objselec.tcl
+-rw-r--r--   0        0        0     8331 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/perilabel.tcl
+-rw-r--r--   0        0        0    15130 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pie.tcl
+-rw-r--r--   0        0        0     1231 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pielabel.tcl
+-rw-r--r--   0        0        0      154 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pkgIndex.tcl
+-rw-r--r--   0        0        0     4150 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/relirect.tcl
+-rw-r--r--   0        0        0     4729 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/selector.tcl
+-rw-r--r--   0        0        0    13055 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/slice.tcl
+-rw-r--r--   0        0        0     4728 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/tkpiechart.tcl
+-rw-r--r--   0        0        0      166 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/tooltip/pkgIndex.tcl
+-rw-r--r--   0        0        0     4021 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/tooltip/tipstack.tcl
+-rw-r--r--   0        0        0    14446 2018-05-11 03:56:08.000000 tkfly-0.1.0a3/tkfly/_tklib/tooltip/tooltip.tcl
+-rw-r--r--   0        0        0      427 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/pkgIndex.tcl
+-rw-r--r--   0        0        0     3561 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/tclIndex
+-rw-r--r--   0        0        0    14936 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbCommon.tcl
+-rw-r--r--   0        0        0    11684 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbEntry.tcl
+-rw-r--r--   0        0        0     2174 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbListbox.tcl
+-rw-r--r--   0        0        0     3247 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl
+-rw-r--r--   0        0        0     6860 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbText.tcl
+-rw-r--r--   0        0        0     2701 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl
+-rw-r--r--   0        0        0     1839 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/wcb/wcb.tcl
+-rw-r--r--   0        0        0     3866 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/arrowb.tcl
+-rw-r--r--   0        0        0    20697 2013-03-26 03:28:23.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/calendar.tcl
+-rw-r--r--   0        0        0    10039 2013-03-26 03:28:23.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/dateentry.tcl
+-rw-r--r--   0        0        0    14200 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/dialog.tcl
+-rw-r--r--   0        0        0     9158 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/mentry.tcl
+-rw-r--r--   0        0        0     6617 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/panelframe.tcl
+-rw-r--r--   0        0        0     1144 2013-03-26 03:28:23.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/pkgIndex.tcl
+-rw-r--r--   0        0        0    18647 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/ruler.tcl
+-rw-r--r--   0        0        0     7563 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/scrollw.tcl
+-rw-r--r--   0        0        0     8025 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/statusbar.tcl
+-rw-r--r--   0        0        0     2093 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/stext.tcl
+-rw-r--r--   0        0        0     3927 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/superframe.tcl
+-rw-r--r--   0        0        0     7915 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widget/toolbar.tcl
+-rw-r--r--   0        0        0     4374 2023-04-29 05:46:59.130164 tkfly-0.1.0a3/tkfly/_tklib/widget/widget.tcl
+-rw-r--r--   0        0        0    32987 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetl/listentry.tcl
+-rw-r--r--   0        0        0    18733 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetl/listsimple.tcl
+-rw-r--r--   0        0        0      237 2019-08-21 18:42:17.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetl/pkgIndex.tcl
+-rw-r--r--   0        0        0      142 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetPlus/pkgIndex.tcl
+-rw-r--r--   0        0        0    57846 2020-02-09 20:50:00.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetPlus/widgetPlus.tcl
+-rw-r--r--   0        0        0      146 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetv/pkgIndex.tcl
+-rw-r--r--   0        0        0    12031 2013-02-14 03:37:16.000000 tkfly-0.1.0a3/tkfly/_tklib/widgetv/validator.tcl
+-rw-r--r--   0        0        0      224 2023-04-29 07:23:36.893330 tkfly-0.1.0a3/tkfly/_twapi/__init__.py
+-rw-r--r--   0        0        0      677 2023-04-29 07:27:32.485989 tkfly-0.1.0a3/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    35822 2021-11-07 07:09:24.000000 tkfly-0.1.0a3/tkfly/_twapi/account.tcl
+-rw-r--r--   0        0        0      721 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/adsi.tcl
+-rw-r--r--   0        0        0     3004 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/apputil.tcl
+-rw-r--r--   0        0        0    63943 2021-11-09 02:43:04.000000 tkfly-0.1.0a3/tkfly/_twapi/base.tcl
+-rw-r--r--   0        0        0     7099 2022-06-04 05:48:24.000000 tkfly-0.1.0a3/tkfly/_twapi/clipboard.tcl
+-rw-r--r--   0        0        0   149879 2021-11-02 05:34:50.000000 tkfly-0.1.0a3/tkfly/_twapi/com.tcl
+-rw-r--r--   0        0        0    24031 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/console.tcl
+-rw-r--r--   0        0        0   118653 2022-06-03 06:01:30.000000 tkfly-0.1.0a3/tkfly/_twapi/crypto.tcl
+-rw-r--r--   0        0        0    22667 2022-06-04 15:03:22.000000 tkfly-0.1.0a3/tkfly/_twapi/device.tcl
+-rw-r--r--   0        0        0    51643 2020-10-09 10:08:22.000000 tkfly-0.1.0a3/tkfly/_twapi/etw.tcl
+-rw-r--r--   0        0        0    14722 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/eventlog.tcl
+-rw-r--r--   0        0        0    23130 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/evt.tcl
+-rw-r--r--   0        0        0     7268 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/handle.tcl
+-rw-r--r--   0        0        0    24383 2020-06-24 02:08:54.000000 tkfly-0.1.0a3/tkfly/_twapi/input.tcl
+-rw-r--r--   0        0        0     1480 2019-07-25 11:50:02.000000 tkfly-0.1.0a3/tkfly/_twapi/LICENSE
+-rw-r--r--   0        0        0    23492 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/metoo.tcl
+-rw-r--r--   0        0        0    37265 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/msi.tcl
+-rw-r--r--   0        0        0    22693 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/mstask.tcl
+-rw-r--r--   0        0        0     1793 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/multimedia.tcl
+-rw-r--r--   0        0        0     3535 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/namedpipe.tcl
+-rw-r--r--   0        0        0    37061 2020-10-14 07:59:02.000000 tkfly-0.1.0a3/tkfly/_twapi/network.tcl
+-rw-r--r--   0        0        0    17196 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/nls.tcl
+-rw-r--r--   0        0        0    43660 2022-06-04 00:12:28.000000 tkfly-0.1.0a3/tkfly/_twapi/os.tcl
+-rw-r--r--   0        0        0    34543 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/pdh.tcl
+-rw-r--r--   0        0        0     7293 2022-06-22 13:03:38.000000 tkfly-0.1.0a3/tkfly/_twapi/pkgIndex.tcl
+-rw-r--r--   0        0        0     3758 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/power.tcl
+-rw-r--r--   0        0        0     1802 2020-06-23 03:12:46.000000 tkfly-0.1.0a3/tkfly/_twapi/printer.tcl
+-rw-r--r--   0        0        0    69738 2022-06-03 07:57:36.000000 tkfly-0.1.0a3/tkfly/_twapi/process.tcl
+-rw-r--r--   0        0        0     6602 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/rds.tcl
+-rw-r--r--   0        0        0     2037 2022-06-22 09:04:10.000000 tkfly-0.1.0a3/tkfly/_twapi/README.md
+-rw-r--r--   0        0        0    13900 2022-06-03 13:37:40.000000 tkfly-0.1.0a3/tkfly/_twapi/registry.tcl
+-rw-r--r--   0        0        0    18583 2022-06-04 12:13:10.000000 tkfly-0.1.0a3/tkfly/_twapi/resource.tcl
+-rw-r--r--   0        0        0    76964 2021-11-06 08:18:08.000000 tkfly-0.1.0a3/tkfly/_twapi/security.tcl
+-rw-r--r--   0        0        0    40542 2022-06-04 14:46:44.000000 tkfly-0.1.0a3/tkfly/_twapi/service.tcl
+-rw-r--r--   0        0        0    30062 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/share.tcl
+-rw-r--r--   0        0        0    19297 2020-12-15 00:37:00.000000 tkfly-0.1.0a3/tkfly/_twapi/shell.tcl
+-rw-r--r--   0        0        0    28334 2022-06-04 12:24:36.000000 tkfly-0.1.0a3/tkfly/_twapi/sspi.tcl
+-rw-r--r--   0        0        0    20059 2022-06-05 01:39:28.000000 tkfly-0.1.0a3/tkfly/_twapi/storage.tcl
+-rw-r--r--   0        0        0     2632 2020-07-01 00:57:00.000000 tkfly-0.1.0a3/tkfly/_twapi/synch.tcl
+-rw-r--r--   0        0        0    49870 2022-06-22 10:37:46.000000 tkfly-0.1.0a3/tkfly/_twapi/tls.tcl
+-rw-r--r--   0        0        0    26955 2020-06-22 09:54:26.000000 tkfly-0.1.0a3/tkfly/_twapi/twapi.tcl
+-rw-r--r--   0        0        0   389718 2022-06-22 13:03:36.000000 tkfly-0.1.0a3/tkfly/_twapi/twapi_base.dll
+-rw-r--r--   0        0        0   516096 2022-06-22 12:59:36.000000 tkfly-0.1.0a3/tkfly/_twapi/twapi_base64.dll
+-rw-r--r--   0        0        0    42512 2022-06-04 14:52:14.000000 tkfly-0.1.0a3/tkfly/_twapi/ui.tcl
+-rw-r--r--   0        0        0     4286 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/win.tcl
+-rw-r--r--   0        0        0    10975 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/winlog.tcl
+-rw-r--r--   0        0        0     3148 2022-06-04 03:20:02.000000 tkfly-0.1.0a3/tkfly/_twapi/winsta.tcl
+-rw-r--r--   0        0        0     6978 2019-07-25 11:50:04.000000 tkfly-0.1.0a3/tkfly/_twapi/wmi.tcl
+-rw-r--r--   0        0        0     7757 2023-04-30 01:54:11.126193 tkfly-0.1.0a3/tkfly/blend2d/__init__.py
+-rw-r--r--   0        0        0    18386 2023-04-30 01:54:11.252535 tkfly-0.1.0a3/tkfly/blend2d/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      279 2023-04-29 15:49:52.339077 tkfly-0.1.0a3/tkfly/blend2d/demos/__init__.py
+-rw-r--r--   0        0        0      967 2023-04-29 15:49:52.453599 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      564 2023-04-29 15:56:22.183150 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d1.cpython-311.pyc
+-rw-r--r--   0        0        0     2310 2023-04-29 16:00:46.536617 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d101.cpython-311.pyc
+-rw-r--r--   0        0        0     6614 2023-04-30 01:28:39.554804 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d102.cpython-311.pyc
+-rw-r--r--   0        0        0      545 2023-04-29 15:56:23.597866 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d2.cpython-311.pyc
+-rw-r--r--   0        0        0      614 2023-04-29 15:50:14.121768 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d3.cpython-311.pyc
+-rw-r--r--   0        0        0      982 2023-04-29 15:56:25.545873 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d4_1.cpython-311.pyc
+-rw-r--r--   0        0        0     1886 2023-04-29 15:56:26.850266 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d4_2.cpython-311.pyc
+-rw-r--r--   0        0        0      800 2023-04-29 15:56:28.253430 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d5.cpython-311.pyc
+-rw-r--r--   0        0        0      840 2023-04-29 15:56:29.505015 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d6.cpython-311.pyc
+-rw-r--r--   0        0        0      939 2023-04-29 16:00:45.037364 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/d7.cpython-311.pyc
+-rw-r--r--   0        0        0     4459 2023-04-30 01:29:00.414309 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/dct.cpython-311.pyc
+-rw-r--r--   0        0        0     7447 2023-04-30 01:34:26.070503 tkfly-0.1.0a3/tkfly/blend2d/demos/__pycache__/dpda.cpython-311.pyc
+-rw-r--r--   0        0        0    51952 2018-05-12 08:44:20.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Blacksword.otf
+-rw-r--r--   0        0        0      139 2020-03-05 14:21:50.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/chessboard.png
+-rw-r--r--   0        0        0    10845 2020-03-08 17:01:24.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/CMYK.png
+-rw-r--r--   0        0        0     4335 2020-05-14 16:48:44.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/CompositionTest.tcl
+-rw-r--r--   0        0        0      151 2023-04-30 01:34:16.617334 tkfly-0.1.0a3/tkfly/blend2d/demos/d.py
+-rw-r--r--   0        0        0      375 2023-04-29 15:45:26.183596 tkfly-0.1.0a3/tkfly/blend2d/demos/d1.py
+-rw-r--r--   0        0        0     2176 2023-04-29 15:59:15.161435 tkfly-0.1.0a3/tkfly/blend2d/demos/d101.py
+-rw-r--r--   0        0        0     6639 2023-04-29 16:01:28.838141 tkfly-0.1.0a3/tkfly/blend2d/demos/d102.py
+-rw-r--r--   0        0        0     4035 2023-04-30 01:41:51.892376 tkfly-0.1.0a3/tkfly/blend2d/demos/d110.py
+-rw-r--r--   0        0        0      350 2023-04-29 15:46:13.786327 tkfly-0.1.0a3/tkfly/blend2d/demos/d2.py
+-rw-r--r--   0        0        0      422 2023-04-29 15:47:21.757569 tkfly-0.1.0a3/tkfly/blend2d/demos/d3.py
+-rw-r--r--   0        0        0      806 2023-04-29 15:52:04.223698 tkfly-0.1.0a3/tkfly/blend2d/demos/d4_1.py
+-rw-r--r--   0        0        0     1733 2023-04-29 15:54:13.375735 tkfly-0.1.0a3/tkfly/blend2d/demos/d4_2.py
+-rw-r--r--   0        0        0      612 2023-04-29 15:54:54.800543 tkfly-0.1.0a3/tkfly/blend2d/demos/d5.py
+-rw-r--r--   0        0        0      663 2023-04-29 15:55:42.846526 tkfly-0.1.0a3/tkfly/blend2d/demos/d6.py
+-rw-r--r--   0        0        0      759 2023-04-29 16:00:16.838813 tkfly-0.1.0a3/tkfly/blend2d/demos/d7.py
+-rw-r--r--   0        0        0     4399 2023-04-30 01:27:49.755083 tkfly-0.1.0a3/tkfly/blend2d/demos/dct.py
+-rw-r--r--   0        0        0     5298 2020-08-12 14:00:30.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/demo-tiger.tcl
+-rw-r--r--   0        0        0     7474 2023-04-30 01:32:16.757048 tkfly-0.1.0a3/tkfly/blend2d/demos/dpda.py
+-rw-r--r--   0        0        0     4972 2023-04-29 16:03:00.011251 tkfly-0.1.0a3/tkfly/blend2d/demos/drect.py
+-rw-r--r--   0        0        0     5302 2023-04-30 01:25:21.918029 tkfly-0.1.0a3/tkfly/blend2d/demos/dtiger.py
+-rw-r--r--   0        0        0     3873 2020-06-23 06:06:42.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/greenSlate.jpg
+-rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/IKscale-1.0.1.tm
+-rw-r--r--   0        0        0     5415 2020-09-03 09:32:10.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/EbuttonColor-1.0.1.tm
+-rw-r--r--   0        0        0     4958 2020-09-03 09:38:00.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/Eseparator-1.0.tm
+-rw-r--r--   0        0        0     5965 2020-08-26 14:52:44.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/hatching-1.0.tm
+-rw-r--r--   0        0        0     9349 2022-01-02 14:35:50.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/IKscale-1.0.1.tm
+-rw-r--r--   0        0        0    33360 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/darwin-x64/perlin.dylib
+-rw-r--r--   0        0        0      513 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/license.terms
+-rw-r--r--   0        0        0    11404 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/linux-x32/perlin.so
+-rw-r--r--   0        0        0    12456 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/linux-x64/perlin.so
+-rw-r--r--   0        0        0     1149 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/pkgIndex.tcl
+-rw-r--r--   0        0        0    11776 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/win-x32/perlin.dll
+-rw-r--r--   0        0        0    13312 2023-04-15 16:05:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/perlin-1.0/win-x64/perlin.dll
+-rw-r--r--   0        0        0    12189 2020-08-28 04:04:42.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/sketchline-1.0.tm
+-rw-r--r--   0        0        0   125189 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/main2.tcl
+-rw-r--r--   0        0        0     1052 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/pkgIndex.tcl
+-rw-r--r--   0        0        0      769 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/snit2.tcl
+-rw-r--r--   0        0        0      510 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/teapot.txt
+-rw-r--r--   0        0        0    18959 2020-09-03 12:26:26.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/snit.2.3.2/validate.tcl
+-rw-r--r--   0        0        0    14134 2021-12-02 19:08:46.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/lib/Spline-1.0.tm
+-rw-r--r--   0        0        0    17997 2023-03-14 07:49:04.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/moby.svg
+-rw-r--r--   0        0        0     7576 2020-05-14 16:47:38.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/PorterDuffInAction.tcl
+-rw-r--r--   0        0        0    22057 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_1.svg
+-rw-r--r--   0        0        0    29922 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_2.svg
+-rw-r--r--   0        0        0    22020 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_3.svg
+-rw-r--r--   0        0        0    23936 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_4.svg
+-rw-r--r--   0        0        0    16595 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_5.svg
+-rw-r--r--   0        0        0      279 2023-03-14 14:01:34.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Q/layer_6.svg
+-rw-r--r--   0        0        0     9507 2020-03-08 17:06:24.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/RGB.png
+-rw-r--r--   0        0        0      436 2016-06-18 19:26:30.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Road_Rage-License.txt
+-rw-r--r--   0        0        0   341760 2016-06-18 17:26:30.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/Road_Rage.otf
+-rw-r--r--   0        0        0    76248 2019-08-19 07:45:32.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/texture.jpeg
+-rw-r--r--   0        0        0   220752 2019-10-15 16:31:28.000000 tkfly-0.1.0a3/tkfly/blend2d/demos/tiger-data.tcl
+-rw-r--r--   0        0        0   146164 2021-05-28 11:22:28.000000 tkfly-0.1.0a3/tkfly/blend2d/HarmonyOS_Sans_Medium.ttf
+-rw-r--r--   0        0        0   640122 2023-04-29 13:45:10.413812 tkfly-0.1.0a3/tkfly/blend2d/surface.bmp
+-rw-r--r--   0        0        0     2217 2023-04-29 15:42:02.761477 tkfly-0.1.0a3/tkfly/core.py
+-rw-r--r--   0        0        0      239 2023-04-29 23:59:46.170477 tkfly-0.1.0a3/tkfly/mupdf/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-14 12:59:16.512351 tkfly-0.1.0a3/tkfly/tkimg/__init__.py
+-rw-r--r--   0        0        0   221710 2022-11-24 07:55:52.000000 tkfly-0.1.0a3/tkfly/tkimg/jpegtcl950.dll
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libjpegtclstub950.a
+-rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libpngtclstub1638.a
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libtifftclstub440.a
+-rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libtkimgstub1414.a
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/libzlibtclstub1213.a
+-rw-r--r--   0        0        0     6851 2022-11-24 07:55:44.000000 tkfly-0.1.0a3/tkfly/tkimg/pkgIndex.tcl
+-rw-r--r--   0        0        0   231950 2022-11-24 07:55:52.000000 tkfly-0.1.0a3/tkfly/tkimg/pngtcl1638.dll
+-rw-r--r--   0        0        0   416782 2022-11-24 07:55:52.000000 tkfly-0.1.0a3/tkfly/tkimg/tifftcl440.dll
+-rw-r--r--   0        0        0    40462 2022-11-24 07:55:54.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimg1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:54.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgbmp1414.dll
+-rw-r--r--   0        0        0    22030 2022-11-24 07:55:54.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgdted1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:56.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgflir1414.dll
+-rw-r--r--   0        0        0    24590 2022-11-24 07:55:56.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimggif1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:56.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgico1414.dll
+-rw-r--r--   0        0        0    23054 2022-11-24 07:55:56.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgjpeg1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgpcx1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:58.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgpixmap1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgpng1414.dll
+-rw-r--r--   0        0        0    25102 2022-11-24 07:56:00.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgppm1414.dll
+-rw-r--r--   0        0        0    21006 2022-11-24 07:56:00.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgps1414.dll
+-rw-r--r--   0        0        0    31758 2022-11-24 07:56:00.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgraw1414.dll
+-rw-r--r--   0        0        0    28174 2022-11-24 07:56:02.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgsgi1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:56:02.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgsun1414.dll
+-rw-r--r--   0        0        0    25102 2022-11-24 07:56:02.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgtga1414.dll
+-rw-r--r--   0        0        0    70158 2022-11-24 07:56:04.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgtiff1414.dll
+-rw-r--r--   0        0        0    17934 2022-11-24 07:56:04.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgwindow1414.dll
+-rw-r--r--   0        0        0    19470 2022-11-24 07:56:04.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgxbm1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:56:06.000000 tkfly-0.1.0a3/tkfly/tkimg/tkimgxpm1414.dll
+-rw-r--r--   0        0        0    91662 2022-11-24 07:56:06.000000 tkfly-0.1.0a3/tkfly/tkimg/zlibtcl1213.dll
+-rw-r--r--   0        0        0        0 2023-04-19 11:17:10.457150 tkfly-0.1.0a3/tkfly/tklib/__init__.py
+-rw-r--r--   0        0        0      141 2023-04-19 12:43:56.373512 tkfly-0.1.0a3/tkfly/tklib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2594 2023-04-29 11:00:59.295786 tkfly-0.1.0a3/tkfly/tklib/__pycache__/datefield.cpython-311.pyc
+-rw-r--r--   0        0        0     8914 2023-04-29 05:02:59.020777 tkfly-0.1.0a3/tkfly/tklib/__pycache__/history.cpython-311.pyc
+-rw-r--r--   0        0        0     3960 2023-04-19 12:45:43.059958 tkfly-0.1.0a3/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0      538 2023-04-29 05:32:30.677805 tkfly-0.1.0a3/tkfly/tklib/autoscroll.py
+-rw-r--r--   0        0        0      573 2023-04-19 14:52:50.309476 tkfly-0.1.0a3/tkfly/tklib/chatwidget.py
+-rw-r--r--   0        0        0     1265 2023-04-29 10:59:14.922692 tkfly-0.1.0a3/tkfly/tklib/datefield.py
+-rw-r--r--   0        0        0     5389 2023-04-29 05:02:58.918925 tkfly-0.1.0a3/tkfly/tklib/history.py
+-rw-r--r--   0        0        0      583 2023-04-19 12:47:17.815625 tkfly-0.1.0a3/tkfly/tklib/menubar.py
+-rw-r--r--   0        0        0     1002 2023-04-29 05:26:07.066657 tkfly-0.1.0a3/tkfly/tklib/notifywindow.py
+-rw-r--r--   0        0        0     1331 2023-04-29 06:07:26.214511 tkfly-0.1.0a3/tkfly/tklib/plotchart.py
+-rw-r--r--   0        0        0     5389 2023-04-29 05:38:33.820659 tkfly-0.1.0a3/tkfly/tklib/shtmlview.py
+-rw-r--r--   0        0        0     2066 2023-04-19 12:45:42.877555 tkfly-0.1.0a3/tkfly/tklib/tooltip.py
+-rw-r--r--   0        0        0      902 2023-04-19 11:28:27.786655 tkfly-0.1.0a3/tkfly/tklib/wcb.py
+-rw-r--r--   0        0        0      523 2023-04-29 05:46:46.161323 tkfly-0.1.0a3/tkfly/tklib/widget.py
+-rw-r--r--   0        0        0      506 2023-04-29 11:29:28.404486 tkfly-0.1.0a3/tkfly/tkscrollutil/__init__.py
+-rw-r--r--   0        0        0      804 2023-04-29 11:29:28.606524 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1165 2023-04-29 11:09:26.181908 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc
+-rw-r--r--   0        0        0     1258 2023-04-29 11:29:43.706687 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc
+-rw-r--r--   0        0        0     3023 2023-04-29 11:14:55.822881 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc
+-rw-r--r--   0        0        0     4204 2023-04-29 11:12:49.744284 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc
+-rw-r--r--   0        0        0     3011 2023-04-29 11:29:28.610040 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc
+-rw-r--r--   0        0        0     2069 2023-04-29 11:34:46.885357 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc
+-rw-r--r--   0        0        0     3060 2023-04-29 11:26:17.297437 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2023-04-29 11:29:28.614038 tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc
+-rw-r--r--   0        0        0      413 2022-10-29 06:29:19.142527 tkfly-0.1.0a3/tkfly/tkscrollutil/attrib.py
+-rw-r--r--   0        0        0      458 2023-04-29 11:29:43.603589 tkfly-0.1.0a3/tkfly/tkscrollutil/load.py
+-rw-r--r--   0        0        0     1793 2023-04-29 13:55:50.749585 tkfly-0.1.0a3/tkfly/tkscrollutil/scrollableframe.py
+-rw-r--r--   0        0        0     1921 2023-04-29 11:14:55.722630 tkfly-0.1.0a3/tkfly/tkscrollutil/scrollarea.py
+-rw-r--r--   0        0        0     2480 2023-04-29 11:10:41.419659 tkfly-0.1.0a3/tkfly/tkscrollutil/scrollsync.py
+-rw-r--r--   0        0        0     1910 2023-04-29 11:29:28.409999 tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollarea.py
+-rw-r--r--   0        0        0     1142 2023-04-29 11:34:46.766705 tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollednotebook.py
+-rw-r--r--   0        0        0     1689 2023-04-29 11:26:17.197236 tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollsync.py
+-rw-r--r--   0        0        0     1435 2023-04-29 11:28:26.430882 tkfly-0.1.0a3/tkfly/tkscrollutil/wheelevent.py
+-rw-r--r--   0        0        0      544 2023-04-29 11:43:18.104764 tkfly-0.1.0a3/tkfly/twapi/__init__.py
+-rw-r--r--   0        0        0     1464 2023-04-29 11:43:18.209994 tkfly-0.1.0a3/tkfly/twapi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      359 2023-04-29 07:58:45.679468 tkfly-0.1.0a3/tkfly/twapi/base.py
+-rw-r--r--   0        0        0      230 2023-04-29 07:58:45.713014 tkfly-0.1.0a3/tkfly/twapi/msi.py
+-rw-r--r--   0        0        0      704 2023-04-29 10:07:46.018924 tkfly-0.1.0a3/tkfly/twapi/ui.py
+-rw-r--r--   0        0        0      585 2023-04-29 08:16:43.020235 tkfly-0.1.0a3/tkfly/twapi/win.py
+-rw-r--r--   0        0        0     7660 1970-01-01 00:00:00.000000 tkfly-0.1.0a3/PKG-INFO
```

### Comparing `tkfly-0.1.0a2/README.md` & `tkfly-0.1.0a3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # tkfly
 基于`tkinter`及`tcl / tk`扩展的中型组件库
 
 `tkfly`指`tkinter`插上翅膀飞翔，意为借助扩展的功能翱翔。
 
 ([tklib -大小约3.7MB](https://core.tcl-lang.org/tklib))
 
-([twapi -大小约2.06MB](https://twapi.magicsplat.com/))
+([twapi -大小约2.0MB](https://twapi.magicsplat.com/))
+
+([blend2d -大小约7.6MB](https://wiki.tcl-lang.org/page/Blend2d))
 
 帮助你开发大型高级的程序
 
 ## 教程
 
 ### 开始
 `tkfly`通过`tkinter`调用`tcl`导入`tklib`实现，可以实现`tklib`库所能实现的各种功能。
 ```bash
 # 暂时处于预览版
 python -m pip install tkfly --pre
 ```
+
 ### 工具提示
 让我来运行一个最简单工具提示吧！
 (基于[tklib/tooltip](https://core.tcl-lang.org/tklib/doc/trunk/embedded/md/tklib/files/modules/tooltip/tooltip.md))
 ```python
 from tkinter import Tk, ttk
 from tkfly import FlyToolTip
 
@@ -91,14 +94,56 @@
 datefield2.pack()
 
 root.mainloop()
 ```
 #### 日期格式
 可以通过`format`参数修改格式，示例`"%Y-%m-%d"`，其中%Y是年号，%m是月份，%d是天。
 
+### 2D渲染
+Blend2D是一个高性能的2D矢量图形引擎，通过调用可以生成图片为label组件设置图片显示
+
+下面有个示例
+```python
+from tkinter import *
+from tkfly import *
+
+root = Tk()
+blend2D = Fly2D()
+surface = blend2D.create_image_surface(
+    size=(500, 500)
+)
+
+surface.surface.fill(
+    blend2D.create_circle((150, 150), 50),
+    blend2D.get_color("lightblue", alpha=0.5)
+)
+
+surface.surface.fill(
+    blend2D.create_circle((250, 250), 60),
+    blend2D.get_color("lightblue", alpha=1.0)
+)
+
+surface.surface.fill(
+    blend2D.create_circle((350, 350), 55),
+    blend2D.get_color("lightblue", alpha=0.75)
+)
+
+
+surface.surface.fill(
+    blend2D.create_text((235, 255), string="Fly2D"),
+    blend2D.get_color("black")
+)
+
+surface.pack()
+
+surface.surface.save("fly2d.png")
+
+root.mainloop()
+```
+
 # tkscrollutil
 实际上这就是作者我以前做过的一个项目。
 
 ## ScrolllArea
 可以快速地为水平滚动、垂直滚动组件设置滚动条
 
 ### 属性
```

### Comparing `tkfly-0.1.0a2/tkfly/__init__.py` & `tkfly-0.1.0a3/tkfly/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,7 +9,9 @@
 from tkfly.tkscrollutil import ScrollSync as FlyScrollSync
 from tkfly.tkscrollutil import ttkScrollSync as FlyTScrollSync
 from tkfly.tkscrollutil import ttkScrolledNoteBook as FlyTScrolledNoteBook
 from tkfly.tkscrollutil import addclosetab as FlyAddCloseTab
 from tkfly.tkscrollutil import removeclosetab as FlyRemoveCloseTab
 
 from tkfly.twapi import get_version as FlyTwapiVersion
+
+from tkfly.blend2d import Blend2D as Fly2D
```

### Comparing `tkfly-0.1.0a2/tkfly/__main__.py` & `tkfly-0.1.0a3/tkfly/__main__.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc` & `tkfly-0.1.0a3/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/autoscroll/autoscroll.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/autoscroll/autoscroll.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/autoscroll/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/autoscroll/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_drag.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_drag.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_epoints.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_epoints.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_epolyline.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_epolyline.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_equad.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_equad.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_gradient.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_gradient.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_highlight.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_highlight.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_mvg.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_mvg.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_snap.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_snap.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_sqmap.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_sqmap.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_tags.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_tags.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_trlines.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_trlines.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_zoom.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/canvas_zoom.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/canvas/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/canvas/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/chatwidget/chatwidget.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/chatwidget/chatwidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/bindDown.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/bindDown.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/led.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/led.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/radioMatrix.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/radioMatrix.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/rdial.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/rdial.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/tachometer.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/tachometer.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/vertical_meter.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/vertical_meter.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/voltmeter.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/controlwidget/voltmeter.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/crosshair/crosshair.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/crosshair/crosshair.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/ctext/ctext.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/ctext/ctext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/cursor/cursor.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/cursor/cursor.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/datefield/datefield.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/datefield/datefield.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/application.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/application.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/attributes.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/attributes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/basic.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/basic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/core.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/core.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/diagram.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/diagram.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/direction.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/direction.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/element.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/element.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/navigation.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/navigation.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/diagrams/point.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/diagrams/point.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/getstring/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/getstring/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/getstring/tk_getString.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/getstring/tk_getString.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/history/history.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/history/history.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/history/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/history/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/ico/ico.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/ico/ico.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/ico/ico0.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/ico/ico0.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/ipentry/ipentry.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/ipentry/ipentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/cs.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/cs.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/da.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/da.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/de.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/de.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/en.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/en.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/es.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/es.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/khim.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/khim/khim.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/khim/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/pl.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/pl.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/ROOT.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/ROOT.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/ru.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/ru.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/khim/uk.msg` & `tkfly-0.1.0a3/tkfly/_tklib/khim/uk.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/mentry_tile.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/mentry_tile.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/mentryPublic.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/mentryPublic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryThemes.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryThemes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryWidget.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mentryWidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mwutil.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/tclIndex` & `tkfly-0.1.0a3/tkfly/_tklib/mentry/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/menubar/debug.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/menubar/debug.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/menubar/menubar.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/menubar/menubar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/menubar/node.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/menubar/node.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/menubar/tree.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/menubar/tree.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/notifywindow/notifywindow.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/notifywindow/notifywindow.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/notifywindow/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/notifywindow/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/ntext/ntext.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/ntext/ntext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/persistentSelection/persistentSelection.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/persistentSelection/persistentSelection.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plot3d.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plot3d.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotanim.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotanim.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotannot.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotannot.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotaxis.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotaxis.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotbind.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotbind.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotbusiness.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotbusiness.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotchart.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotchart.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotcombined.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotcombined.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotconfig.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotconfig.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotcontour.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotcontour.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotgantt.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotgantt.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotobject.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotobject.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotpack.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotpack.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotpriv.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotpriv.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotscada.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotscada.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotspecial.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotspecial.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotstatustimeline.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plotstatustimeline.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plottable.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/plottable.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/scaling.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/scaling.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/plotchart/xyplot.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/plotchart/xyplot.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/attrib.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/attrib.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/mwutil.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/pagesman.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/pagesman.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/tclIndex` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutil.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutil_tile.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutil_tile.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutilCommon.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/scrollutil/scrollutilCommon.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/style/as.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/style/as.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/style/lobster.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/style/lobster.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/style/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/style/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/style/style.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/style/style.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/swaplist/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/swaplist/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/swaplist/swaplist.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/swaplist/swaplist.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/mwutil.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/pencil.cur` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/pencil.cur`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/repair.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/repair.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tclIndex` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelist_tile.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelist_tile.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelistPublic.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tablelist/tablelistPublic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/boxlabel.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/boxlabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/canlabel.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/canlabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/labarray.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/labarray.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/objselec.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/objselec.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/perilabel.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/perilabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pie.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pie.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pielabel.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/pielabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/relirect.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/relirect.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/selector.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/selector.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/slice.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/slice.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/tkpiechart.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tkpiechart/tkpiechart.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tooltip/tipstack.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tooltip/tipstack.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/tooltip/tooltip.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/tooltip/tooltip.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/tclIndex` & `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbCommon.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbCommon.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbEntry.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbEntry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbListbox.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbListbox.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbText.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbText.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/wcb/wcb.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/wcb/wcb.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/arrowb.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/arrowb.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/calendar.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/calendar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/dateentry.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/dateentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/dialog.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/dialog.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/mentry.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/mentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/panelframe.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/panelframe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/ruler.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/ruler.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/scrollw.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/scrollw.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/statusbar.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/statusbar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/stext.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/stext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/superframe.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/superframe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/toolbar.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/toolbar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widget/widget.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widget/widget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widgetl/listentry.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widgetl/listentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widgetl/listsimple.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widgetl/listsimple.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widgetPlus/widgetPlus.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widgetPlus/widgetPlus.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_tklib/widgetv/validator.tcl` & `tkfly-0.1.0a3/tkfly/_tklib/widgetv/validator.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/account.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/account.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/adsi.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/adsi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/apputil.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/apputil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/base.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/base.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/clipboard.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/clipboard.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/com.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/com.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/console.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/console.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/crypto.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/crypto.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/device.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/device.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/etw.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/etw.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/eventlog.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/eventlog.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/evt.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/evt.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/handle.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/handle.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/input.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/input.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/LICENSE` & `tkfly-0.1.0a3/tkfly/_twapi/LICENSE`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/metoo.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/metoo.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/msi.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/msi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/mstask.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/mstask.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/multimedia.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/multimedia.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/namedpipe.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/namedpipe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/network.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/network.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/nls.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/nls.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/os.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/os.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/pdh.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/pdh.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/power.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/power.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/printer.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/printer.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/process.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/process.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/rds.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/rds.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/README.md` & `tkfly-0.1.0a3/tkfly/_twapi/README.md`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/registry.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/registry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/resource.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/resource.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/security.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/security.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/service.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/service.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/share.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/share.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/shell.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/shell.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/sspi.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/sspi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/storage.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/storage.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/synch.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/synch.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/tls.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/tls.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/twapi.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/twapi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/twapi_base.dll` & `tkfly-0.1.0a3/tkfly/_twapi/twapi_base.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/twapi_base64.dll` & `tkfly-0.1.0a3/tkfly/_twapi/twapi_base64.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/ui.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/ui.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/win.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/win.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/winlog.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/winlog.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/winsta.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/winsta.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/_twapi/wmi.tcl` & `tkfly-0.1.0a3/tkfly/_twapi/wmi.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/core.py` & `tkfly-0.1.0a3/tkfly/core.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/jpegtcl950.dll` & `tkfly-0.1.0a3/tkfly/tkimg/jpegtcl950.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/libjpegtclstub950.a` & `tkfly-0.1.0a3/tkfly/tkimg/libjpegtclstub950.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/libpngtclstub1638.a` & `tkfly-0.1.0a3/tkfly/tkimg/libpngtclstub1638.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/libtifftclstub440.a` & `tkfly-0.1.0a3/tkfly/tkimg/libtifftclstub440.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/libtkimgstub1414.a` & `tkfly-0.1.0a3/tkfly/tkimg/libtkimgstub1414.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/libzlibtclstub1213.a` & `tkfly-0.1.0a3/tkfly/tkimg/libzlibtclstub1213.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/pkgIndex.tcl` & `tkfly-0.1.0a3/tkfly/tkimg/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/pngtcl1638.dll` & `tkfly-0.1.0a3/tkfly/tkimg/pngtcl1638.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tifftcl440.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tifftcl440.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimg1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimg1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgbmp1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgbmp1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgdted1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgdted1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgflir1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgflir1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimggif1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimggif1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgico1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgico1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgjpeg1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgjpeg1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgpcx1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgpcx1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgpixmap1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgpixmap1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgpng1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgpng1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgppm1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgppm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgps1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgps1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgraw1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgraw1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgsgi1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgsgi1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgsun1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgsun1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgtga1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgtga1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgtiff1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgtiff1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgwindow1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgwindow1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgxbm1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgxbm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/tkimgxpm1414.dll` & `tkfly-0.1.0a3/tkfly/tkimg/tkimgxpm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkimg/zlibtcl1213.dll` & `tkfly-0.1.0a3/tkfly/tkimg/zlibtcl1213.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/__pycache__/datefield.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tklib/__pycache__/datefield.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/__pycache__/history.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tklib/__pycache__/history.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/autoscroll.py` & `tkfly-0.1.0a3/tkfly/tklib/autoscroll.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/chatwidget.py` & `tkfly-0.1.0a3/tkfly/tklib/chatwidget.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/datefield.py` & `tkfly-0.1.0a3/tkfly/tklib/datefield.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/history.py` & `tkfly-0.1.0a3/tkfly/tklib/history.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/menubar.py` & `tkfly-0.1.0a3/tkfly/tklib/menubar.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/notifywindow.py` & `tkfly-0.1.0a3/tkfly/tklib/notifywindow.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/plotchart.py` & `tkfly-0.1.0a3/tkfly/tklib/plotchart.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/shtmlview.py` & `tkfly-0.1.0a3/tkfly/tklib/shtmlview.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/tooltip.py` & `tkfly-0.1.0a3/tkfly/tklib/tooltip.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/wcb.py` & `tkfly-0.1.0a3/tkfly/tklib/wcb.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tklib/widget.py` & `tkfly-0.1.0a3/tkfly/tklib/widget.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/scrollableframe.py` & `tkfly-0.1.0a3/tkfly/tkscrollutil/scrollableframe.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,21 +32,18 @@
         """
         load()
         Widget.__init__(self, master, "scrollutil::scrollableframe", cnf, kw, )
 
     def contentframe(self) -> Frame:
         _frame = self.tk.call(self._w, "contentframe")
 
-        class _Frame(Frame):
-            def __init__(self, master=None):
-                super().__init__(master)
+        _Frame = Frame()
+        _Frame.nametowidget(_frame)
 
-                self._w = _frame
-
-        return _Frame()
+        return _Frame
 
 
 if __name__ == '__main__':
     from tkinter import Tk, Label
     from tkfly.tkscrollutil.scrollarea import ScrollArea
     from tkfly.tkscrollutil.wheelevent import createWheelEventBindings
     root = Tk()
```

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/scrollarea.py` & `tkfly-0.1.0a3/tkfly/tkscrollutil/scrollarea.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/scrollsync.py` & `tkfly-0.1.0a3/tkfly/tkscrollutil/scrollsync.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollarea.py` & `tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollarea.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollednotebook.py` & `tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollednotebook.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollsync.py` & `tkfly-0.1.0a3/tkfly/tkscrollutil/ttk_scrollsync.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/tkscrollutil/wheelevent.py` & `tkfly-0.1.0a3/tkfly/tkscrollutil/wheelevent.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/twapi/__init__.py` & `tkfly-0.1.0a3/tkfly/twapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/twapi/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a3/tkfly/twapi/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/twapi/ui.py` & `tkfly-0.1.0a3/tkfly/twapi/ui.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/tkfly/twapi/win.py` & `tkfly-0.1.0a3/tkfly/twapi/win.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a2/PKG-INFO` & `tkfly-0.1.0a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfly
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: 
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -17,26 +17,29 @@
 # tkfly
 基于`tkinter`及`tcl / tk`扩展的中型组件库
 
 `tkfly`指`tkinter`插上翅膀飞翔，意为借助扩展的功能翱翔。
 
 ([tklib -大小约3.7MB](https://core.tcl-lang.org/tklib))
 
-([twapi -大小约2.06MB](https://twapi.magicsplat.com/))
+([twapi -大小约2.0MB](https://twapi.magicsplat.com/))
+
+([blend2d -大小约7.6MB](https://wiki.tcl-lang.org/page/Blend2d))
 
 帮助你开发大型高级的程序
 
 ## 教程
 
 ### 开始
 `tkfly`通过`tkinter`调用`tcl`导入`tklib`实现，可以实现`tklib`库所能实现的各种功能。
 ```bash
 # 暂时处于预览版
 python -m pip install tkfly --pre
 ```
+
 ### 工具提示
 让我来运行一个最简单工具提示吧！
 (基于[tklib/tooltip](https://core.tcl-lang.org/tklib/doc/trunk/embedded/md/tklib/files/modules/tooltip/tooltip.md))
 ```python
 from tkinter import Tk, ttk
 from tkfly import FlyToolTip
 
@@ -107,14 +110,56 @@
 datefield2.pack()
 
 root.mainloop()
 ```
 #### 日期格式
 可以通过`format`参数修改格式，示例`"%Y-%m-%d"`，其中%Y是年号，%m是月份，%d是天。
 
+### 2D渲染
+Blend2D是一个高性能的2D矢量图形引擎，通过调用可以生成图片为label组件设置图片显示
+
+下面有个示例
+```python
+from tkinter import *
+from tkfly import *
+
+root = Tk()
+blend2D = Fly2D()
+surface = blend2D.create_image_surface(
+    size=(500, 500)
+)
+
+surface.surface.fill(
+    blend2D.create_circle((150, 150), 50),
+    blend2D.get_color("lightblue", alpha=0.5)
+)
+
+surface.surface.fill(
+    blend2D.create_circle((250, 250), 60),
+    blend2D.get_color("lightblue", alpha=1.0)
+)
+
+surface.surface.fill(
+    blend2D.create_circle((350, 350), 55),
+    blend2D.get_color("lightblue", alpha=0.75)
+)
+
+
+surface.surface.fill(
+    blend2D.create_text((235, 255), string="Fly2D"),
+    blend2D.get_color("black")
+)
+
+surface.pack()
+
+surface.surface.save("fly2d.png")
+
+root.mainloop()
+```
+
 # tkscrollutil
 实际上这就是作者我以前做过的一个项目。
 
 ## ScrolllArea
 可以快速地为水平滚动、垂直滚动组件设置滚动条
 
 ### 属性
```

