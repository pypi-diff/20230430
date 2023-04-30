# Comparing `tmp/tumourkit-0.4.1.tar.gz` & `tmp/tumourkit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumourkit-0.4.1.tar", last modified: Tue Mar 28 09:49:06 2023, max compression
+gzip compressed data, was "tumourkit-0.5.0.tar", last modified: Sun Apr 30 10:23:39 2023, max compression
```

## Comparing `tumourkit-0.4.1.tar` & `tumourkit-0.5.0.tar`

### file list

```diff
@@ -1,150 +1,155 @@
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.105674 tumourkit-0.4.1/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.4.1/LICENSE
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-03-28 09:49:06.103187 tumourkit-0.4.1/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.4.1/README.md
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.030576 tumourkit-0.4.1/docs/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.030393 tumourkit-0.4.1/docs/buildenv/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.043132 tumourkit-0.4.1/docs/buildenv/bin/
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2html.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2html4.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2html5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2latex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2man.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2odt.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2s5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2xetex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rst2xml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.4.1/docs/buildenv/bin/rstpep2html.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.043550 tumourkit-0.4.1/docs/source/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1135 2023-03-25 18:12:07.000000 tumourkit-0.4.1/docs/source/conf.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1963 2023-03-27 06:31:58.000000 tumourkit-0.4.1/pyproject.toml
--rw-r--r--   0 joseperezcano   (501) staff       (20)      818 2023-03-23 17:22:35.000000 tumourkit-0.4.1/requirements.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-03-28 09:49:06.105834 tumourkit-0.4.1/setup.cfg
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.053588 tumourkit-0.4.1/tests/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.4.1/tests/centroidspng2csv_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.4.1/tests/conf_matrix_sum_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.4.1/tests/cpairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.4.1/tests/example_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.4.1/tests/generate_centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.4.1/tests/generate_rswoosh.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.4.1/tests/get_conn_comp_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1812 2023-03-20 09:29:59.000000 tumourkit-0.4.1/tests/graph2centroids_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.4.1/tests/graph_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2199 2023-03-23 19:39:56.000000 tumourkit-0.4.1/tests/hov_prob_pipe_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.4.1/tests/hov_prob_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.4.1/tests/hovernet_patches_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.4.1/tests/metrics_pairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.4.1/tests/metrics_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.4.1/tests/png2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.4.1/tests/pngcsv2geojson_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.4.1/tests/pngcsv2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1987 2023-03-06 07:30:43.000000 tumourkit-0.4.1/tests/read_nodes_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.4.1/tests/remove_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.4.1/tests/rswoosh_test.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.056645 tumourkit-0.4.1/tumourkit/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-03-28 09:38:43.000000 tumourkit-0.4.1/tumourkit/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.064304 tumourkit-0.4.1/tumourkit/classification/
--rw-r--r--   0 joseperezcano   (501) staff       (20)       97 2023-03-16 07:35:20.000000 tumourkit-0.4.1/tumourkit/classification/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5932 2023-03-23 17:37:13.000000 tumourkit-0.4.1/tumourkit/classification/calibration_error.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1342 2023-03-23 17:12:54.000000 tumourkit-0.4.1/tumourkit/classification/compute_imbalance.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6811 2023-03-15 08:07:52.000000 tumourkit-0.4.1/tumourkit/classification/evaluate.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4656 2023-03-25 15:54:29.000000 tumourkit-0.4.1/tumourkit/classification/infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.066453 tumourkit-0.4.1/tumourkit/classification/models/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.4.1/tumourkit/classification/models/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.4.1/tumourkit/classification/models/gat.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.4.1/tumourkit/classification/models/gcn.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.4.1/tumourkit/classification/models/hgao.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.4.1/tumourkit/classification/models/norm.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7132 2023-03-25 15:16:17.000000 tumourkit-0.4.1/tumourkit/classification/read_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4315 2023-03-20 12:32:43.000000 tumourkit-0.4.1/tumourkit/classification/read_nodes.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    18940 2023-03-25 15:29:44.000000 tumourkit-0.4.1/tumourkit/classification/train_gnn.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5936 2023-03-27 14:39:30.000000 tumourkit-0.4.1/tumourkit/classification/train_xgboost.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7183 2023-03-28 09:28:12.000000 tumourkit-0.4.1/tumourkit/infer_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3151 2023-03-20 14:38:24.000000 tumourkit-0.4.1/tumourkit/make_dirs.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.069139 tumourkit-0.4.1/tumourkit/postprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      127 2023-03-09 07:25:32.000000 tumourkit-0.4.1/tumourkit/postprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3619 2023-03-09 07:58:38.000000 tumourkit-0.4.1/tumourkit/postprocessing/join_graph_gt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5469 2023-03-22 15:42:53.000000 tumourkit-0.4.1/tumourkit/postprocessing/join_hovprob_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5370 2023-01-14 21:37:27.000000 tumourkit-0.4.1/tumourkit/postprocessing/merge_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1623 2023-01-14 21:36:24.000000 tumourkit-0.4.1/tumourkit/postprocessing/rswoosh.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.074824 tumourkit-0.4.1/tumourkit/preprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      616 2023-03-20 11:26:08.000000 tumourkit-0.4.1/tumourkit/preprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2298 2023-03-23 19:01:53.000000 tumourkit-0.4.1/tumourkit/preprocessing/centroids2png.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4659 2023-03-25 16:07:13.000000 tumourkit-0.4.1/tumourkit/preprocessing/centroidspng2csv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4423 2023-03-23 19:06:24.000000 tumourkit-0.4.1/tumourkit/preprocessing/geojson2pngcsv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3288 2023-03-28 09:36:18.000000 tumourkit-0.4.1/tumourkit/preprocessing/graph2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2844 2023-03-23 19:09:28.000000 tumourkit-0.4.1/tumourkit/preprocessing/hovernet2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3723 2023-03-23 19:11:32.000000 tumourkit-0.4.1/tumourkit/preprocessing/hovernet2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-03-23 19:32:48.000000 tumourkit-0.4.1/tumourkit/preprocessing/png2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2775 2023-03-25 16:11:44.000000 tumourkit-0.4.1/tumourkit/preprocessing/pngcsv2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5532 2023-03-23 19:26:17.000000 tumourkit-0.4.1/tumourkit/preprocessing/pngcsv2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3935 2023-03-23 19:32:30.000000 tumourkit-0.4.1/tumourkit/preprocessing/pngcsv2graph.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.075992 tumourkit-0.4.1/tumourkit/profiling/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2824 2022-12-31 13:07:35.000000 tumourkit-0.4.1/tumourkit/profiling/cpairs_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1946 2022-12-31 13:07:42.000000 tumourkit-0.4.1/tumourkit/profiling/rswoosh_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3823 2023-03-27 07:25:04.000000 tumourkit-0.4.1/tumourkit/research_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.077211 tumourkit-0.4.1/tumourkit/segmentation/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.4.1/tumourkit/segmentation/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    10684 2023-03-15 08:10:41.000000 tumourkit-0.4.1/tumourkit/segmentation/evaluate.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.079859 tumourkit-0.4.1/tumourkit/segmentation/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/config.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.081742 tumourkit-0.4.1/tumourkit/segmentation/hovernet/dataloader/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/dataloader/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-01-10 14:21:32.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/dataloader/augs.py
--rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/dataloader/train_loader.py
--rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/extract_patches.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.083473 tumourkit-0.4.1/tumourkit/segmentation/hovernet/infer/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/infer/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3281 2023-03-22 07:18:47.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/infer/base.py
--rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/infer/tile.py
--rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/infer/wsi.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.084456 tumourkit-0.4.1/tumourkit/segmentation/hovernet/metrics/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/metrics/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/metrics/stats_utils.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.087593 tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/patch_extractor.py
--rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/viz_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/wsi_handler.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.088097 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.093322 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/opt.py
--rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
--rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     5032 2023-03-08 08:51:29.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/targets.py
--rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     8272 2023-03-08 12:23:15.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.094705 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.097211 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/callbacks/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
--rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
--rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
--rwx------   0 joseperezcano   (501) staff       (20)     7185 2022-09-15 10:27:54.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/engine.py
--rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.4.1/tumourkit/segmentation/hovernet/train.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     8895 2023-03-25 15:43:44.000000 tumourkit-0.4.1/tumourkit/train_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.102021 tumourkit-0.4.1/tumourkit/utils/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.4.1/tumourkit/utils/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2524 2023-03-23 18:24:54.000000 tumourkit-0.4.1/tumourkit/utils/classification.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3606 2023-03-23 18:25:35.000000 tumourkit-0.4.1/tumourkit/utils/folder2txt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5254 2023-03-23 18:29:29.000000 tumourkit-0.4.1/tumourkit/utils/nearest.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7022 2023-03-23 18:35:15.000000 tumourkit-0.4.1/tumourkit/utils/postprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    20768 2023-03-25 16:06:07.000000 tumourkit-0.4.1/tumourkit/utils/preprocessing.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-03-28 09:49:06.059882 tumourkit-0.4.1/tumourkit.egg-info/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-03-28 09:49:06.000000 tumourkit-0.4.1/tumourkit.egg-info/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4771 2023-03-28 09:49:06.000000 tumourkit-0.4.1/tumourkit.egg-info/SOURCES.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-03-28 09:49:06.000000 tumourkit-0.4.1/tumourkit.egg-info/dependency_links.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      747 2023-03-28 09:49:06.000000 tumourkit-0.4.1/tumourkit.egg-info/entry_points.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      818 2023-03-28 09:49:06.000000 tumourkit-0.4.1/tumourkit.egg-info/requires.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       26 2023-03-28 09:49:06.000000 tumourkit-0.4.1/tumourkit.egg-info/top_level.txt
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.274073 tumourkit-0.5.0/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.5.0/LICENSE
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-04-30 10:23:39.273084 tumourkit-0.5.0/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.5.0/README.md
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.154916 tumourkit-0.5.0/demo/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      670 2023-04-14 09:43:14.000000 tumourkit-0.5.0/demo/app.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.148006 tumourkit-0.5.0/docs/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.147811 tumourkit-0.5.0/docs/buildenv/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.165438 tumourkit-0.5.0/docs/buildenv/bin/
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2html.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2html4.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2html5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2latex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2man.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2odt.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2s5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2xetex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rst2xml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.5.0/docs/buildenv/bin/rstpep2html.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.166073 tumourkit-0.5.0/docs/source/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.5.0/docs/source/conf.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2132 2023-04-30 10:02:08.000000 tumourkit-0.5.0/pyproject.toml
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      818 2023-03-23 17:22:35.000000 tumourkit-0.5.0/requirements.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-04-30 10:23:39.274204 tumourkit-0.5.0/setup.cfg
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.181707 tumourkit-0.5.0/tests/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.5.0/tests/centroidspng2csv_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.5.0/tests/conf_matrix_sum_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.5.0/tests/cpairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.5.0/tests/example_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.5.0/tests/generate_centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.5.0/tests/generate_rswoosh.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.5.0/tests/get_conn_comp_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.5.0/tests/graph2centroids_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.5.0/tests/graph_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2199 2023-03-23 19:39:56.000000 tumourkit-0.5.0/tests/hov_prob_pipe_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.5.0/tests/hov_prob_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.5.0/tests/hovernet_patches_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.5.0/tests/metrics_pairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.5.0/tests/metrics_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.5.0/tests/png2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.5.0/tests/pngcsv2geojson_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.5.0/tests/pngcsv2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.5.0/tests/read_nodes_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.5.0/tests/remove_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.5.0/tests/rswoosh_test.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.186228 tumourkit-0.5.0/tumourkit/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-04-30 10:23:28.000000 tumourkit-0.5.0/tumourkit/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.194486 tumourkit-0.5.0/tumourkit/classification/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.5.0/tumourkit/classification/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1349 2023-04-12 10:40:08.000000 tumourkit-0.5.0/tumourkit/classification/compute_imbalance.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6072 2023-04-12 10:38:57.000000 tumourkit-0.5.0/tumourkit/classification/evaluate.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5318 2023-04-11 18:31:20.000000 tumourkit-0.5.0/tumourkit/classification/infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.198049 tumourkit-0.5.0/tumourkit/classification/models/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.5.0/tumourkit/classification/models/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.5.0/tumourkit/classification/models/gat.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.5.0/tumourkit/classification/models/gcn.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.5.0/tumourkit/classification/models/hgao.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.5.0/tumourkit/classification/models/norm.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7489 2023-04-12 10:40:12.000000 tumourkit-0.5.0/tumourkit/classification/read_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    20584 2023-04-13 09:56:23.000000 tumourkit-0.5.0/tumourkit/classification/train_graphs.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    10352 2023-04-12 10:40:17.000000 tumourkit-0.5.0/tumourkit/classification/train_xgboost.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5590 2023-04-17 07:53:40.000000 tumourkit-0.5.0/tumourkit/eval_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7511 2023-04-17 15:24:46.000000 tumourkit-0.5.0/tumourkit/infer_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3151 2023-03-20 14:38:24.000000 tumourkit-0.5.0/tumourkit/make_dirs.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.202388 tumourkit-0.5.0/tumourkit/postprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      127 2023-03-09 07:25:32.000000 tumourkit-0.5.0/tumourkit/postprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3619 2023-03-09 07:58:38.000000 tumourkit-0.5.0/tumourkit/postprocessing/join_graph_gt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5469 2023-03-22 15:42:53.000000 tumourkit-0.5.0/tumourkit/postprocessing/join_hovprob_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5332 2023-04-02 17:54:39.000000 tumourkit-0.5.0/tumourkit/postprocessing/merge_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1623 2023-01-14 21:36:24.000000 tumourkit-0.5.0/tumourkit/postprocessing/rswoosh.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.214732 tumourkit-0.5.0/tumourkit/preprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      616 2023-03-20 11:26:08.000000 tumourkit-0.5.0/tumourkit/preprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2298 2023-03-23 19:01:53.000000 tumourkit-0.5.0/tumourkit/preprocessing/centroids2png.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4659 2023-03-25 16:07:13.000000 tumourkit-0.5.0/tumourkit/preprocessing/centroidspng2csv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3894 2023-04-30 09:54:10.000000 tumourkit-0.5.0/tumourkit/preprocessing/geojson2pngcsv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3288 2023-03-28 09:36:18.000000 tumourkit-0.5.0/tumourkit/preprocessing/graph2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2844 2023-03-23 19:09:28.000000 tumourkit-0.5.0/tumourkit/preprocessing/hovernet2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3723 2023-03-23 19:11:32.000000 tumourkit-0.5.0/tumourkit/preprocessing/hovernet2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-03-23 19:32:48.000000 tumourkit-0.5.0/tumourkit/preprocessing/png2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2775 2023-03-25 16:11:44.000000 tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5043 2023-04-30 09:55:47.000000 tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3935 2023-03-23 19:32:30.000000 tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1075 2023-04-30 10:05:05.000000 tumourkit-0.5.0/tumourkit/preprocessing/remove_uncertain.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.216294 tumourkit-0.5.0/tumourkit/profiling/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2824 2022-12-31 13:07:35.000000 tumourkit-0.5.0/tumourkit/profiling/cpairs_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1946 2022-12-31 13:07:42.000000 tumourkit-0.5.0/tumourkit/profiling/rswoosh_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    14758 2023-04-26 19:41:21.000000 tumourkit-0.5.0/tumourkit/research_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.226608 tumourkit-0.5.0/tumourkit/segmentation/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.5.0/tumourkit/segmentation/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12265 2023-04-27 10:59:55.000000 tumourkit-0.5.0/tumourkit/segmentation/evaluate.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.233366 tumourkit-0.5.0/tumourkit/segmentation/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/config.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.237814 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/augs.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/extract_patches.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.243665 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3281 2023-03-22 07:18:47.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/tile.py
+-rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/wsi.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.245970 tumourkit-0.5.0/tumourkit/segmentation/hovernet/metrics/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/metrics/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.249838 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/viz_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.250835 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.256147 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
+-rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8272 2023-03-08 12:23:15.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.258064 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.262961 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/engine.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.5.0/tumourkit/segmentation/hovernet/train.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     9861 2023-04-17 15:13:33.000000 tumourkit-0.5.0/tumourkit/train_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.271797 tumourkit-0.5.0/tumourkit/utils/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.5.0/tumourkit/utils/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5932 2023-03-23 17:37:13.000000 tumourkit-0.5.0/tumourkit/utils/calibration_error.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5628 2023-04-12 10:40:15.000000 tumourkit-0.5.0/tumourkit/utils/classification.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3606 2023-03-23 18:25:35.000000 tumourkit-0.5.0/tumourkit/utils/folder2txt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5254 2023-03-23 18:29:29.000000 tumourkit-0.5.0/tumourkit/utils/nearest.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3094 2023-04-22 10:28:27.000000 tumourkit-0.5.0/tumourkit/utils/pipes.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7022 2023-03-23 18:35:15.000000 tumourkit-0.5.0/tumourkit/utils/postprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    21866 2023-04-30 10:04:39.000000 tumourkit-0.5.0/tumourkit/utils/preprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5670 2023-04-12 10:40:06.000000 tumourkit-0.5.0/tumourkit/utils/read_nodes.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-04-30 10:23:39.189229 tumourkit-0.5.0/tumourkit.egg-info/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4860 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/SOURCES.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/dependency_links.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      910 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/entry_points.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      818 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/requires.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       31 2023-04-30 10:23:39.000000 tumourkit-0.5.0/tumourkit.egg-info/top_level.txt
```

### Comparing `tumourkit-0.4.1/LICENSE` & `tumourkit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/PKG-INFO` & `tumourkit-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.4.1
+Version: 0.5.0
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.4.1/README.md` & `tumourkit-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2html.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2html4.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2html5.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2latex.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2man.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2odt.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2odt_prepstyles.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2pseudoxml.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2s5.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2xetex.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rst2xml.py` & `tumourkit-0.5.0/docs/buildenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/buildenv/bin/rstpep2html.py` & `tumourkit-0.5.0/docs/buildenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/docs/source/conf.py` & `tumourkit-0.5.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
 ]
 autosummary_generate = True
 
 templates_path = ['_templates']
-exclude_patterns = []
+exclude_patterns = ['**/__init__.py']
 
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_rtd_theme"
```

### Comparing `tumourkit-0.4.1/pyproject.toml` & `tumourkit-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -46,8 +46,11 @@
 pngcsv2geojson = "tumourkit.preprocessing.pngcsv2geojson:main"
 pngcsv2graph = "tumourkit.preprocessing.pngcsv2graph:main"
 graph2centroids = "tumourkit.preprocessing.graph2centroids:main"
 centroidspng2csv = "tumourkit.preprocessing.centroidspng2csv:main"
 make_dirs = "tumourkit.make_dirs:main"
 run_training = "tumourkit.train_pipe:main"
 run_inference = "tumourkit.infer_pipe:main"
-run_research = "tumourkit.research_pipe:main"
+run_research = "tumourkit.research_pipe:main"
+run_evaluation = "tumourkit.eval_pipe:main"
+merge_cells = "tumourkit.postprocessing.merge_cells:main"
+remove_uncertain = "tumourkit.preprocessing.remove_uncertain:main"
```

### Comparing `tumourkit-0.4.1/requirements.txt` & `tumourkit-0.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/centroidspng2csv_test.py` & `tumourkit-0.5.0/tests/centroidspng2csv_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/conf_matrix_sum_test.py` & `tumourkit-0.5.0/tests/conf_matrix_sum_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/cpairs_test.py` & `tumourkit-0.5.0/tests/cpairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/example_test.py` & `tumourkit-0.5.0/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/generate_centroids.py` & `tumourkit-0.5.0/tests/generate_centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/generate_rswoosh.py` & `tumourkit-0.5.0/tests/generate_rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/get_conn_comp_test.py` & `tumourkit-0.5.0/tests/get_conn_comp_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/graph2centroids_test.py` & `tumourkit-0.5.0/tests/graph2centroids_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,12 +40,12 @@
             return False
     return True
 
 
 @pytest.mark.parametrize("name", get_names(GRAPH_DIR, '.nodes.csv'))
 def test_graph2centroids(name):
     graph_file = read_graph(name, GRAPH_DIR)
-    centroids_file = graph2centroids(graph_file)
+    centroids_file = graph2centroids(graph_file, num_classes=2)
     ref_centroids_file = read_centroids(name, CENTROIDS_DIR)
     if not check_equal(centroids_file, ref_centroids_file):
         assert False, name
     assert(True)
```

### Comparing `tumourkit-0.4.1/tests/graph_idx_test.py` & `tumourkit-0.5.0/tests/graph_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/hov_prob_pipe_test.py` & `tumourkit-0.5.0/tests/hov_prob_pipe_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/hov_prob_test.py` & `tumourkit-0.5.0/tests/hov_prob_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/hovernet_patches_test.py` & `tumourkit-0.5.0/tests/hovernet_patches_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/metrics_pairs_test.py` & `tumourkit-0.5.0/tests/metrics_pairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/metrics_test.py` & `tumourkit-0.5.0/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/png2graph_test.py` & `tumourkit-0.5.0/tests/png2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/pngcsv2geojson_test.py` & `tumourkit-0.5.0/tests/pngcsv2geojson_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/pngcsv2graph_test.py` & `tumourkit-0.5.0/tests/pngcsv2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/read_nodes_test.py` & `tumourkit-0.5.0/tests/read_nodes_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 import pytest
 import os
 
-from tumourkit.classification.read_nodes import create_node_splits
+from tumourkit.utils.read_nodes import create_node_splits
 from tumourkit.utils.preprocessing import parse_path 
 
 TEST_DIR = os.path.dirname(os.path.abspath(__file__))
 GRAPHS_DIR = parse_path(TEST_DIR) + 'graphs/'
 
 
 @pytest.mark.parametrize("val_size,test_size", [
```

### Comparing `tumourkit-0.4.1/tests/remove_idx_test.py` & `tumourkit-0.5.0/tests/remove_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tests/rswoosh_test.py` & `tumourkit-0.5.0/tests/rswoosh_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/classification/calibration_error.py` & `tumourkit-0.5.0/tumourkit/utils/calibration_error.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/classification/compute_imbalance.py` & `tumourkit-0.5.0/tumourkit/classification/compute_imbalance.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 import argparse
-from .read_nodes import read_all_nodes
+from ..utils.read_nodes import read_all_nodes
 import os
 import numpy as np
 
 FILE_DIR = os.path.dirname(os.path.abspath(__file__))
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--graph-dir', type=str, required=True,
```

### Comparing `tumourkit-0.4.1/tumourkit/classification/evaluate.py` & `tumourkit-0.5.0/tumourkit/classification/evaluate.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,39 +16,24 @@
 
 Contact information: joseperez2000@hotmail.es
 """
 from typing import Dict, List, Optional
 import os
 import pandas as pd
 import numpy as np
-from sklearn.metrics import roc_auc_score, f1_score, accuracy_score
 from sklearn.calibration import calibration_curve
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 
 from ..utils.preprocessing import parse_path, create_dir
-from .calibration_error import calibration_error
+from ..utils.classification import metrics_from_predictions
 
 import argparse
 
 
-def check_imbalance(labels: np.ndarray) -> bool:
-    """
-    Returns true if there are at least two classes, and false otherwise.
-    """
-    return len(np.unique(labels)) > 1
-
-def percentage_error(labels: np.ndarray, preds: np.ndarray) -> float:
-    """
-    Computes the deviation in the percentage of tumoral cells.
-    """
-    gt_perc = (labels==1).sum() / len(labels)
-    pred_perc = (preds==1).sum() / len(preds)
-    return abs(gt_perc - pred_perc)
-
 def abline(slope: float, intercept: float, axes: Axes) -> None:
     """
     Plot a line from slope and intercept on current axis.
     """
     x_vals = np.array(axes.get_xlim())
     y_vals = intercept + slope * x_vals
     axes.plot(x_vals, y_vals, linestyle='dotted', color='k')
@@ -97,25 +82,19 @@
     Dataframe must contain columns class and prob1.
     Class columns must have 1 for negative and 2 for positive.
     """
     labels = nodes_df['class'].to_numpy()-1
     probs = nodes_df['prob1'].to_numpy()
     preds = (probs > 0.5) * 1
 
+    acc, f1, auc, perc_error, ece = metrics_from_predictions(labels, preds, probs, 2)
+
     if draw_on is not None:
         draw_reliability_diagram(labels, probs, draw_on, method_name)
 
-    acc = accuracy_score(labels, preds)
-    f1 = f1_score(labels, preds, zero_division=0)
-    if check_imbalance(labels):
-        auc = roc_auc_score(labels, probs)
-    else:
-        auc = -1
-    perc_error = percentage_error(labels, preds)
-    ece = calibration_error(labels, probs, norm='l1', reduce_bias=False)
     return {'Accuracy': acc, 'F1-score': f1, 'ROC AUC': auc, 'Error percentage': perc_error, 'ECE': ece}
 
 def save_metrics(metrics: Dict[str, float], save_name):
     """
     Saves metrics into csv file.
     """
     metrics_df = pd.DataFrame(metrics)
```

### Comparing `tumourkit-0.4.1/tumourkit/classification/infer.py` & `tumourkit-0.5.0/tumourkit/classification/infer.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,35 +19,35 @@
 Contact information: joseperez2000@hotmail.es
 """
 from typing import Dict, Tuple, Any
 from ..utils.preprocessing import parse_path, create_dir
 import torch
 from torch import nn
 import torch.nn.functional as F
-from .train_gnn import load_model
+from .train_graphs import load_model
 from .read_graph import GraphDataset
 import dgl
 from dgl.dataloading import GraphDataLoader
 import json
 import pickle
 import numpy as np
 import pandas as pd
 import argparse
 import os
                   
 
-def load_saved_model(weights_path: str, conf_path: str, num_classes: int) -> nn.Module:
+def load_saved_model(weights_path: str, conf_path: str, num_classes: int, num_feats: int) -> nn.Module:
     """
     Loads state_dict into a torch module.
     Configuration file must match with state_dict.
     """
     state_dict = torch.load(weights_path, map_location='cpu')
     with open(conf_path, 'r') as f:
         conf = json.load(f)
-    model = load_model(conf, num_classes)
+    model = load_model(conf, num_classes, num_feats)
     model.load_state_dict(state_dict)
     return model
 
 def load_normalizer(norm_path: str) -> Tuple[Any]:
     """
     Returns normalizers used in training save at norm_path.
     """
@@ -99,27 +99,37 @@
     parser.add_argument('--weights', type=str, required=True,
                         help='Path to model weights.')  
     parser.add_argument('--conf', type=str, required=True,
                         help='Configuration file for the model.')
     parser.add_argument('--normalizers', type=str, required=True,
                         help='Path to normalizer objects for the model.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
+    parser.add_argument('--disable-prior', action='store_true', help='If True, remove hovernet probabilities from node features.')
+    parser.add_argument('--disable-morph-feats', action='store_true', help='If True, remove morphological features from node features.')
     return parser
 
 
 def main_with_args(args):
     node_dir = parse_path(args.node_dir)
     output_dir = parse_path(args.output_dir)
     create_dir(output_dir)
     normalizers = load_normalizer(args.normalizers)
     eval_dataset = GraphDataset(
         node_dir=node_dir, return_names=True, is_inference=True,
-        max_dist=200, max_degree=10, normalizers=normalizers)
+        max_dist=200, max_degree=10, normalizers=normalizers,
+        remove_morph=args.disable_morph_feats, remove_prior=args.disable_prior)
     eval_dataloader = GraphDataLoader(eval_dataset, batch_size=1, shuffle=False)
-    model = load_saved_model(args.weights, args.conf, args.num_classes)
+    num_feats = 18 + (1 if args.num_classes == 2 else args.num_classes)
+    if args.disable_morph_feats:
+        num_feats -= 18
+    if args.disable_prior:
+        num_feats -= (1 if args.num_classes == 2 else args.num_classes)
+    if num_feats == 0:
+        num_feats = 1
+    model = load_saved_model(args.weights, args.conf, args.num_classes, num_feats)
     model.eval()
     probs = run_inference(model, eval_dataloader, 'cpu', args.num_classes)
     save_probs(probs, node_dir, output_dir, args.num_classes)
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
```

### Comparing `tumourkit-0.4.1/tumourkit/classification/models/gat.py` & `tumourkit-0.5.0/tumourkit/classification/models/gat.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/classification/models/gcn.py` & `tumourkit-0.5.0/tumourkit/classification/models/gcn.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/classification/models/hgao.py` & `tumourkit-0.5.0/tumourkit/classification/models/hgao.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/classification/models/norm.py` & `tumourkit-0.5.0/tumourkit/classification/models/norm.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/classification/read_graph.py` & `tumourkit-0.5.0/tumourkit/classification/read_graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from itertools import tee
 from typing import Tuple, List, Optional, Callable, Any
 import os
 import numpy as np
 from ..utils.preprocessing import get_names
 from ..utils.nearest import generate_tree
 from ..utils.classification import fit_column_normalizer
-from .read_nodes import read_node_matrix
+from ..utils.read_nodes import read_node_matrix
 import torch
 from torch.utils.data import Dataset
 import dgl
 from sklearn.preprocessing import Normalizer
 
 class GraphDataset(Dataset):
     """
@@ -43,15 +43,18 @@
     def __init__(self, node_dir: str, max_dist: float, max_degree: int,
         files: Optional[List[str]] = None,
         transform: Optional[Callable[[np.ndarray], np.ndarray]] = None,
         column_normalize: Optional[bool] = False,
         row_normalize: Optional[bool] = False,
         normalizers: Optional[Tuple[Any]] = None,
         return_names: Optional[bool] = False,
-        is_inference: Optional[bool] = False):
+        is_inference: Optional[bool] = False,
+        remove_prior: Optional[bool] = False,
+        remove_morph: Optional[bool] = False,
+        ):
         """
         node_dir: Path to .nodes.csv files.
         max_dist: Maximum distance to consider two nodes as neighbours.
         max_degree: Maximum degree for each node.
         files: List of names to include in the dataset. If None all names are included.
         column_normalize: Whether to subtract mean and divide by standard deviation each feature.
         row_normalize: Whether to apply row normalization. Reference: https://pytorch-geometric.readthedocs.io/en/latest/_modules/torch_geometric/transforms/normalize_features.html#NormalizeFeatures
@@ -66,21 +69,26 @@
             self.node_names = sorted(get_names(node_dir, '.nodes.csv'))
         self.max_dist = max_dist
         self.max_degree = max_degree
         self.transform = transform
         self.column_normalize = column_normalize
         self.row_normalize = row_normalize
         self.normalizers = normalizers
+        self.remove_prior = remove_prior
+        self.remove_morph = remove_morph
         self.initialize_normalizers()
         self.return_names = return_names
         self.is_inference = is_inference
 
     def __getitem__(self, idx):
         file_name = self.node_names[idx] + '.nodes.csv'
-        X, y, xx, yy = read_node_matrix(os.path.join(self.node_dir, file_name), return_coordinates=True, return_class=not self.is_inference)
+        X, y, xx, yy = read_node_matrix(
+            os.path.join(self.node_dir, file_name), return_coordinates=True, return_class=not self.is_inference,
+            remove_prior=self.remove_prior, remove_morph=self.remove_morph
+            )
         if self.column_normalize:
             X = self.col_sc.transform(X)
         if self.row_normalize:
             X = self.row_sc.transform(X)
         if self.normalizers is not None:
             for normalizer in self.normalizers:
                 X = normalizer.transform(X)
@@ -132,15 +140,15 @@
         Fits normalizers for later use and also checks they contain transform method.
         """
         if self.normalizers is not None:
             for normalizer in self.normalizers:
                 assert callable(getattr(normalizer, "transform", None)), \
                     'Normalizers provided must have transform method.'
         if self.column_normalize:
-            self.col_sc = fit_column_normalizer(self.node_dir, self.node_names)
+            self.col_sc = fit_column_normalizer(self.node_dir, self.node_names, remove_morph=self.remove_morph, remove_prior=self.remove_prior)
             assert callable(getattr(self.col_sc, "transform", None)), \
             'Error loading column normalizer.'
         if self.row_normalize:
             self.row_sc = Normalizer(norm='l1')
             assert callable(getattr(self.row_sc, "transform", None)), \
             'Error loading row normalizer.'
```

### Comparing `tumourkit-0.4.1/tumourkit/classification/read_nodes.py` & `tumourkit-0.5.0/tumourkit/utils/read_nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,62 +21,104 @@
 """
 from typing import List, Optional, Tuple
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
 import random
 import os
-from ..utils.preprocessing import *
+from .preprocessing import *
 
 
-def read_node_matrix(file: str, return_coordinates: Optional[bool] = False, return_class: Optional[bool] = True) -> Tuple[np.ndarray, np.ndarray]:
+def read_node_matrix(
+        file: str,
+        return_coordinates: Optional[bool] = False,
+        return_class: Optional[bool] = True,
+        remove_prior: Optional[bool] = False,
+        remove_morph: Optional[bool] = False,
+        ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Read csv and creates X and y matrices.
     Centroids coordinates are removed.
     Labels are subtracted 1 to be in 0-1 range.
     """
     df = pd.read_csv(file)
+    remove_vars = ['id', 'class', 'X', 'Y']
+    if remove_morph:
+        remove_vars.extend([
+            'area','perimeter','std','red0','red1','red2','red3','red4','green0','green1','green2','green3','green4','blue0','blue1','blue2','blue3','blue4'
+        ])
+    if remove_prior:
+        remove_vars.extend(list(filter(lambda x: 'prob' in x, df.columns)))
     if return_class:
         y = df['class'].to_numpy() - 1
-        X = df.drop(['id', 'class', 'X', 'Y'], axis=1).to_numpy()
+        X = df.drop(remove_vars, axis=1).to_numpy()
+        if remove_morph and remove_prior:
+            X = np.zeros((len(y), 1))
         if not return_coordinates:
             return X, y
         else:
             xx = df['X'].to_numpy()
             yy = df['Y'].to_numpy()
             return X, y, xx, yy
     else:
-        X = df.drop(['id', 'X', 'Y'], axis=1).to_numpy()
+        X = df.drop(remove_vars, axis=1).to_numpy()
+        if remove_morph and remove_prior:
+            X = np.zeros((len(y), 1))
         if not return_coordinates:
             return X, None
         else:
             xx = df['X'].to_numpy()
             yy = df['Y'].to_numpy()
             return X, None, xx, yy
 
-def read_all_nodes(node_dir: str, names: List[str]) -> List[np.ndarray]:
+def _read_all_nodes(
+        node_dir: str,
+        names: List[str],
+        remove_prior: Optional[bool] = False,
+        remove_morph: Optional[bool] = False,
+        ) -> List[np.ndarray]:
     """
     Input
       node_dir: Path to folder with csv files containing node features.
       names: List of files to read. Must have file extension.
     Output
       X: Input data in array format.
       y: Labels in array format.
     """
     X, y = None, None
     for name in names:
-        X_, y_ = read_node_matrix(os.path.join(node_dir, name))
+        X_, y_ = read_node_matrix(os.path.join(node_dir, name), remove_morph=remove_morph, remove_prior=remove_prior)
         if X is None: 
             X = X_ # Shape (n_samples, n_features)
             y = y_ # Shape (n_samples,)
         else:
             X = np.vstack([X, X_])
             y = np.hstack([y, y_])
     return X, y
 
+
+def read_all_nodes(
+        node_dir: str,
+        remove_prior: Optional[bool] = False,
+        remove_morph: Optional[bool] = False,
+        ) -> List[np.ndarray]:
+    """
+    Input
+      node_dir: Path to folder with csv files containing node features.
+    Output
+      X: Input data in array format.
+      y: Labels in array format.
+    """
+    ext = '.nodes.csv'
+    names = get_names(node_dir, ext)
+    names = [x+ext for x in names]
+    X, y = _read_all_nodes(node_dir, names, remove_morph=remove_morph, remove_prior=remove_prior)
+    return X, y
+
+
 def create_node_splits(
     node_dir: str, val_size: float, test_size: float, 
     seed: Optional[int] = None,
     mode: Optional[str] = 'total') -> List[np.ndarray]:
     """
     Input
       node_dir: Path to folder with csv files containing node features.
@@ -87,15 +129,15 @@
     Output
       X_train, X_val, X_test, y_train, y_val, y_test: Node features and labels.
     """
     ext = '.nodes.csv'
     names = get_names(node_dir, ext)
     names = [x+ext for x in names]
     if mode == 'total':
-        X, y = read_all_nodes(node_dir, names)
+        X, y = _read_all_nodes(node_dir, names)
         X_tr_val, X_test, y_tr_val, y_test = train_test_split(
             X, y, test_size=test_size, stratify=y, random_state=seed
         )
         X_train, X_val, y_train, y_val = train_test_split(
             X_tr_val, y_tr_val, test_size=val_size / (1-test_size), 
             stratify=y_tr_val, random_state=seed
         )
@@ -106,13 +148,13 @@
         N = len(names)
         N_ts = int(N * test_size)
         N_val = int(N * val_size)
         N_tr = N - N_val - N_ts
         train_names = names[:N_tr]
         val_names = names[N_tr:N_val+N_tr]
         test_names = names[N_val+N_tr:]
-        X_train, y_train = read_all_nodes(node_dir, train_names)
-        X_val, y_val = read_all_nodes(node_dir, val_names)
-        X_test, y_test = read_all_nodes(node_dir, test_names)
+        X_train, y_train = _read_all_nodes(node_dir, train_names)
+        X_val, y_val = _read_all_nodes(node_dir, val_names)
+        X_test, y_test = _read_all_nodes(node_dir, test_names)
         return X_train, X_val, X_test, y_train, y_val, y_test
     else:
         assert False, 'Wrong mode.'
```

### Comparing `tumourkit-0.4.1/tumourkit/classification/train_gnn.py` & `tumourkit-0.5.0/tumourkit/classification/train_graphs.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,71 +37,72 @@
 from torch.utils.tensorboard import SummaryWriter
 import warnings
 import os
 from concurrent.futures import ThreadPoolExecutor
 import json
 import pickle
 from ..utils.preprocessing import parse_path, create_dir
-from sklearn.metrics import roc_auc_score, f1_score, accuracy_score
+from ..utils.classification import metrics_from_predictions
 warnings.filterwarnings('ignore')
 
 def evaluate(
         loader: GraphDataLoader,
         model: nn.Module,
         device: str,
         writer: Optional[SummaryWriter] = None,
         epoch: Optional[int] = None,
         log_suffix: Optional[str] = None,
         num_classes: Optional[str] = 2,
-        ) -> Tuple[float, float, float]:
+        ) -> List[float]:
     """
     Evaluates model in loader.
     Logs to tensorboard with suffix log_suffix.
     Returns the model in evaluation mode.
     """
     model.eval()
-    preds, labels, probs = np.array([]).reshape(0,1), np.array([]).reshape(0,1), np.array([]).reshape(0,1)
+    preds, labels, probs = np.array([]).reshape(0,1), np.array([]).reshape(0,1), np.array([]).reshape(0,1 if num_classes == 2 else num_classes)
     for g in loader:
         g = g.to(device)
         # self-loops
         g = dgl.remove_self_loop(g)
         g = dgl.add_self_loop(g)
         # data
         features = g.ndata['X']
         # Forward
         logits = model(g, features)
         pred = logits.argmax(1).detach().cpu().numpy().reshape(-1,1)
         preds = np.vstack((preds, pred))
         if num_classes == 2:
             prob = F.softmax(logits, dim=1).detach().cpu().numpy()[:,1].reshape(-1,1)
-            probs = np.vstack((probs, prob))
+        else:
+            prob = F.softmax(logits, dim=1).detach().cpu().numpy()
+        probs = np.vstack((probs, prob))
         label = g.ndata['y'].detach().cpu().numpy().reshape(-1,1)
         labels = np.vstack((labels, label))
     # Compute metrics on validation  
     if num_classes == 2:
-        f1 = f1_score(labels, preds)  
-        acc = accuracy_score(labels, preds)
-        auc = roc_auc_score(labels, probs)
+        acc, f1, auc, perc_err, ece = metrics_from_predictions(labels, preds, probs, 2)
         # Tensorboard
         if writer is not None:
             assert(log_suffix is not None and epoch is not None)
             writer.add_scalar('Accuracy/' + log_suffix, acc, epoch)
             writer.add_scalar('F1/' + log_suffix, f1, epoch)
             writer.add_scalar('ROC_AUC/' + log_suffix, auc, epoch)
-        return f1, acc, auc
+            writer.add_scalar('Percentage error/' + log_suffix, perc_err, epoch)
+            writer.add_scalar('ECE/' + log_suffix, ece, epoch)
+        return f1, acc, auc, perc_err, ece
     else:
-        micro = f1_score(labels, preds, average='micro')
-        macro = f1_score(labels, preds, average='macro')
-        weighted = f1_score(labels, preds, average='weighted')
+        micro, macro, weighted, ece = metrics_from_predictions(labels, preds, probs, num_classes)
         # Tensorboard
         if writer is not None:
             writer.add_scalar('Accuracy/' + log_suffix, micro, epoch)
             writer.add_scalar('Macro F1/' + log_suffix, macro, epoch)
             writer.add_scalar('Weighted F1/' + log_suffix, weighted, epoch)
-        return micro, macro, weighted
+            writer.add_scalar('ECE/' + log_suffix, ece, epoch)
+        return micro, macro, weighted, ece
     
 
 def train_one_iter(
         tr_loader: GraphDataLoader,
         model: nn.Module,
         device: str,
         optimizer: Optimizer,
@@ -125,37 +126,33 @@
         logits = model(tr_g, features)
         loss = F.cross_entropy(logits, labels)
         # Backward
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
         # Compute metrics on training
-        pred = logits.argmax(1).detach().cpu().numpy()
+        preds = logits.argmax(1).detach().cpu().numpy()
         labels = labels.detach().cpu().numpy()
         if num_classes == 2:
-            train_acc = accuracy_score(labels, pred)
-            train_f1 = f1_score(labels, pred)
             probs = F.softmax(logits, dim=1).detach().cpu().numpy()[:,1]
-            train_auc = None
-            if len(np.unique(labels)) > 1:
-                train_auc = roc_auc_score(labels, probs)
-            
+            train_acc, train_f1, train_auc, train_perc_err, train_ece = metrics_from_predictions(labels, preds, probs, 2)
             # Tensorboard
             writer.add_scalar('Accuracy/train', train_acc, step+len(tr_loader)*epoch)
             writer.add_scalar('F1/train', train_f1, step+len(tr_loader)*epoch)
-            if train_auc is not None:
-                writer.add_scalar('ROC_AUC/train', train_auc, step+len(tr_loader)*epoch)
+            writer.add_scalar('ROC_AUC/train', train_auc, step+len(tr_loader)*epoch)
+            writer.add_scalar('ECE/train', train_ece, step+len(tr_loader)*epoch)
+            writer.add_scalar('Percentage Error/train', train_perc_err, step+len(tr_loader)*epoch)
         else:
-            train_micro = f1_score(labels, pred, average='micro')
-            train_macro = f1_score(labels, pred, average='macro')
-            train_weighted = f1_score(labels, pred, average='weighted')
+            probs = F.softmax(logits, dim=1).detach().cpu().numpy()
+            train_micro, train_macro, train_weighted, train_ece = metrics_from_predictions(labels, preds, probs, num_classes)
             # Tensorboard
             writer.add_scalar('Accuracy/train', train_micro, step+len(tr_loader)*epoch)
             writer.add_scalar('Macro F1/train', train_macro, step+len(tr_loader)*epoch)
             writer.add_scalar('Weighted F1/train', train_weighted, step+len(tr_loader)*epoch)
+            writer.add_scalar('ECE/train', train_ece, step+len(tr_loader)*epoch)
 
 def train(
         save_dir: str,
         save_weights: bool,
         tr_loader: GraphDataLoader, 
         val_loader: GraphDataLoader, 
         model: nn.Module,
@@ -175,17 +172,17 @@
     n_epochs = 1000
     best_val_f1 = 0
     early_stop_rounds = 0
     for epoch in range(n_epochs):
         train_one_iter(tr_loader, model, device, optimizer, epoch, writer, num_classes)
         val_metrics = evaluate(val_loader, model, device, writer, epoch, 'validation', num_classes=num_classes)
         if num_classes == 2:
-            val_f1, val_acc, val_auc = val_metrics
+            val_f1, val_acc, val_auc, val_perc_error, val_ece = val_metrics
         else:
-            val_micro, val_macro, val_f1 = val_metrics
+            val_micro, val_macro, val_f1, val_ece = val_metrics
         # Save checkpoint
         if save_weights and check_iters != -1 and epoch % check_iters == 0:
             save_model(save_dir, model, conf, normalizers, prefix='last_')
         # Early stopping
         if val_f1 > best_val_f1:
             best_val_f1 = val_f1
             early_stop_rounds = 0
@@ -198,14 +195,16 @@
         
 
 def load_dataset(
         train_node_dir: str,
         val_node_dir: str,
         test_node_dir: str,
         bsize: int,
+        remove_prior: Optional[bool] = False,
+        remove_morph: Optional[bool] = False,
         ) -> Tuple[GraphDataLoader, GraphDataLoader, GraphDataLoader]:
     """
     Creates Torch dataloaders for training. 
     Folder structure:
     node_dir:
      - train
       - graphs
@@ -217,23 +216,23 @@
        ...
      - test
       - graphs
        - file1.nodes.csv
        ...
     """
     train_dataset = GraphDataset(
-        node_dir=train_node_dir,
+        node_dir=train_node_dir, remove_morph=remove_morph, remove_prior=remove_prior,
         max_dist=200, max_degree=10, column_normalize=True)
     train_dataloader = GraphDataLoader(train_dataset, batch_size=bsize, shuffle=True)
     val_dataset = GraphDataset(
-        node_dir=val_node_dir,
+        node_dir=val_node_dir, remove_morph=remove_morph, remove_prior=remove_prior,
         max_dist=200, max_degree=10, normalizers=train_dataset.get_normalizers())
     val_dataloader = GraphDataLoader(val_dataset, batch_size=1, shuffle=False)
     test_dataset = GraphDataset(
-        node_dir=test_node_dir,
+        node_dir=test_node_dir, remove_morph=remove_morph, remove_prior=remove_prior,
         max_dist=200, max_degree=10, normalizers=train_dataset.get_normalizers())
     test_dataloader = GraphDataLoader(test_dataset, batch_size=1, shuffle=False)
     return train_dataloader, val_dataloader, test_dataloader
 
 def generate_configurations(max_confs: int, model_name: str) -> List[Dict[str, int]]:
     """
     Generates a grid in the search space with no more than max_confs configurations.
@@ -258,20 +257,19 @@
             conf['MODEL_NAME'] = model_name
             conf['NUM_LAYERS'] = num_layers
             conf['DROPOUT'] = dropout
             conf['NORM_TYPE'] = None
             confs.append(conf)
     return confs
 
-def load_model(conf: Dict[str,Any], num_classes: int) -> nn.Module:
+def load_model(conf: Dict[str,Any], num_classes: int, num_feats: int) -> nn.Module:
     """
     Available models: GCN, ATT, HATT, SAGE, BOOST
     Configuration space: NUM_LAYERS, DROPOUT, NORM_TYPE
     """
-    num_feats = 18 + (1 if num_classes == 2 else num_classes)
     hidden_feats = 100
     if conf['MODEL_NAME'] == 'GCN':
         return GCN(num_feats, hidden_feats, num_classes, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
     if conf['MODEL_NAME'] == 'ATT' or conf['MODEL_NAME'] == 'HATT':
         num_heads = 8
         num_out_heads = 1
         heads = ([num_heads] * conf['NUM_LAYERS']) + [num_out_heads]
@@ -283,28 +281,31 @@
 def create_results_file(filename: str, num_classes: int) -> None:
     """
     Creates header of .csv result file to append results.
     filename must not contain extension.
     """
     if num_classes == 2:
         with open(filename + '.csv', 'w') as f:
-            print('F1 Score,Accuracy,ROC AUC,NUM_LAYERS,DROPOUT,NORM_TYPE', file=f)
+            print('F1 Score,Accuracy,ROC AUC,PERC ERR,ECE,NUM_LAYERS,DROPOUT,NORM_TYPE', file=f)
     else:
         with open(filename + '.csv', 'w') as f:
-            print('Micro F1,Macro F1,Weighted F1,NUM_LAYERS,DROPOUT,NORM_TYPE', file=f)
+            print('Micro F1,Macro F1,Weighted F1,ECE,NUM_LAYERS,DROPOUT,NORM_TYPE', file=f)
 
 def append_results(
-    filename: str, f1: float, acc: float, auc: float, num_layers: int, dropout: float, bn_type: str
+    filename: str, f1: float, acc: float, auc: float, num_layers: int, dropout: float, bn_type: str, ece: float, perc_err: Optional[float] = None
 ) -> None:
     """
     Appends result to given filename.
     filename must not contain extension.
     """
     with open(filename + '.csv', 'a') as f:
-        print(f1, acc, auc, num_layers, dropout, bn_type, file=f, sep=',')
+        if perc_err is not None:
+            print(f1, acc, auc, perc_err, ece, num_layers, dropout, bn_type, file=f, sep=',')
+        else:
+            print(f1, acc, auc, ece, num_layers, dropout, bn_type, file=f, sep=',')
 
 def name_from_conf(conf: Dict[str, Any]) -> str:
     """
     Generates a name from the configuration object.
     """
     return conf['MODEL_NAME'] + '_' + str(conf['NUM_LAYERS']) + '_' \
         + str(conf['DROPOUT']) + '_' + str(conf['NORM_TYPE']) 
@@ -333,35 +334,36 @@
         train_dataloader: GraphDataLoader,
         val_dataloader: GraphDataLoader,
         test_dataloader: GraphDataLoader,
         log_dir: str,
         save_weights: bool,
         save_dir: str,
         num_classes: int,
-        ) -> Tuple[float, float, float, nn.Module, Dict[str, Any]]:
+        num_feats: int
+        ) -> Tuple[List[float], nn.Module, Dict[str, Any]]:
     # Tensorboard logs
     writer = SummaryWriter(log_dir=os.path.join(log_dir, name_from_conf(conf)))
     # Model
-    model = load_model(conf, num_classes)
+    model = load_model(conf, num_classes, num_feats)
     optimizer = torch.optim.Adam(model.parameters(), lr=0.001)
     # Train
     train(
         save_dir, save_weights, train_dataloader, val_dataloader,
         model, optimizer, writer, args.early_stopping_rounds,
         args.device, args.checkpoint_iters, conf, train_dataloader.dataset.get_normalizers(),
         num_classes=num_classes
     )
     test_metrics = evaluate(test_dataloader, model, args.device, num_classes=num_classes)
     model = model.cpu()
     if num_classes == 2:
-        test_f1, test_acc, test_auc = test_metrics
-        return test_f1, test_acc, test_auc, model, conf
+        test_f1, test_acc, test_auc, test_perc_err, test_ece = test_metrics
+        return test_f1, test_acc, test_auc, test_perc_err, test_ece, model, conf
     else:
-        test_micro, test_macro, test_weighted = test_metrics
-        return test_micro, test_macro, test_weighted, model, conf
+        test_micro, test_macro, test_weighted, test_ece = test_metrics
+        return test_micro, test_macro, test_weighted, test_ece, model, conf
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--train-node-dir', type=str, required=True,
                         help='Path to folder containing train folder with .nodes.csv files.')
     parser.add_argument('--validation-node-dir', type=str, required=True,
@@ -385,14 +387,16 @@
     parser.add_argument('--device', type=str, choices=['cpu', 'cuda'], default='cpu',
                         help='Device to execute. Either cpu or cuda. Default: cpu.')
     parser.add_argument('--num-workers', type=int, default=1, 
                         help='Number of processors to use. Default: 1.')
     parser.add_argument('--checkpoint-iters', type=int, default=-1, 
                         help='Number of iterations at which to save model periodically while training. Set to -1 for no checkpointing. Default: -1.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
+    parser.add_argument('--disable-prior', action='store_true', help='If True, remove hovernet probabilities from node features.')
+    parser.add_argument('--disable-morph-feats', action='store_true', help='If True, remove morphological features from node features.')
     return parser
 
 
 def main_with_args(args: Namespace):
     log_dir = parse_path(args.log_dir)
     create_dir(log_dir)
     save_weights = False
@@ -405,48 +409,57 @@
         create_dir(save_dir + 'normalizers')
     # Datasets
     train_dataloader, val_dataloader, test_dataloader = load_dataset(
         train_node_dir=args.train_node_dir,
         val_node_dir=args.validation_node_dir,
         test_node_dir=args.test_node_dir,
         bsize=args.batch_size,
+        remove_prior=args.disable_prior,
+        remove_morph=args.disable_morph_feats
     )
     # Configurations
     confs = generate_configurations(args.num_confs, args.model_name)
     create_results_file(args.save_file, args.num_classes)
+    num_feats = 18 + (1 if args.num_classes == 2 else args.num_classes)
+    if args.disable_morph_feats:
+        num_feats -= 18
+    if args.disable_prior:
+        num_feats -= (1 if args.num_classes == 2 else args.num_classes)
+    if num_feats == 0:
+        num_feats = 1
     if args.num_workers > 0:
         with ThreadPoolExecutor(max_workers=args.num_workers) as executor:
             futures = []
             for conf in confs:
                 future = executor.submit(
                     train_one_conf,
-                    args, conf, train_dataloader, val_dataloader, test_dataloader, log_dir, save_weights, save_dir, args.num_classes
+                    args, conf, train_dataloader, val_dataloader, test_dataloader, log_dir, save_weights, save_dir, args.num_classes, num_feats
                 )
                 futures.append(future)
             for future in futures:
                 if args.num_classes == 2:
-                    test_f1, test_acc, test_auc, model, conf = future.result()
-                    append_results(args.save_file, test_f1, test_acc, test_auc, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
+                    test_f1, test_acc, test_auc, test_perc_err, test_ece, model, conf = future.result()
+                    append_results(args.save_file, test_f1, test_acc, test_auc, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'], test_ece, test_perc_err)
                 else:
-                    test_micro, test_macro, test_weighted, model, conf = future.result()
-                    append_results(args.save_file, test_micro, test_macro, test_weighted, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
+                    test_micro, test_macro, test_weighted, test_ece, model, conf = future.result()
+                    append_results(args.save_file, test_micro, test_macro, test_weighted, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'], test_ece)
                 if save_weights:
                     save_model(save_dir, model, conf, train_dataloader.dataset.get_normalizers(), 'last_')
     else:
         for conf in confs:
             if args.num_classes == 2:
-                test_f1, test_acc, test_auc, model, conf = train_one_conf(
-                    args, conf, train_dataloader, val_dataloader, test_dataloader, log_dir, save_weights, save_dir, args.num_classes
+                test_f1, test_acc, test_auc, test_perc_err, test_ece, model, conf = train_one_conf(
+                    args, conf, train_dataloader, val_dataloader, test_dataloader, log_dir, save_weights, save_dir, args.num_classes, num_feats
                 )
-                append_results(args.save_file, test_f1, test_acc, test_auc, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
+                append_results(args.save_file, test_f1, test_acc, test_auc, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'], test_ece, test_perc_err)
             else:
-                test_micro, test_macro, test_weighted, model, conf = train_one_conf(
-                    args, conf, train_dataloader, val_dataloader, test_dataloader, log_dir, save_weights, save_dir, args.num_classes
+                test_micro, test_macro, test_weighted, test_ece, model, conf = train_one_conf(
+                    args, conf, train_dataloader, val_dataloader, test_dataloader, log_dir, save_weights, save_dir, args.num_classes, num_feats
                 )
-                append_results(args.save_file, test_micro, test_macro, test_weighted, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
+                append_results(args.save_file, test_micro, test_macro, test_weighted, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'], test_ece)
             if save_weights:
                 save_model(save_dir, model, conf, train_dataloader.dataset.get_normalizers(), 'last_')
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
```

### Comparing `tumourkit-0.4.1/tumourkit/infer_pipe.py` & `tumourkit-0.5.0/tumourkit/infer_pipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 from .utils.preprocessing import create_dir
 from .classification import infer_gnn
 import pandas as pd
 
 
 def set_best_configuration(args: Namespace, logger: Logger) -> None:
     logger.info('Configuration not provided, using best configuration from training based on F1 score.')
-    save_file = os.path.join(args.root_dir, 'gnn_logs', 'gnn_results.csv')
+    if args.best_arch == 'GCN':
+        save_file = os.path.join(args.root_dir, 'gnn_logs', 'gcn_results.csv')
+    elif args.best_arch == 'ATT':
+        save_file = os.path.join(args.root_dir, 'gnn_logs', 'gat_results.csv')
+    else:
+        assert False, 'Architecture not supported'
     gnn_results = pd.read_csv(save_file)
     if args.num_classes == 2:
         best_conf = gnn_results.sort_values(by='F1 Score', ascending=False).iloc[0]
     else:
         best_conf = gnn_results.sort_values(by='Weighted F1', ascending=False).iloc[0]
     args.best_num_layers = str(best_conf['NUM_LAYERS'])
     args.best_dropout = str(best_conf['DROPOUT'])
@@ -94,15 +99,17 @@
         + args.best_dropout + '_' + args.best_norm_type
     newargs = Namespace(
         node_dir = os.path.join(args.output_dir, 'graphs', 'hovpreds'),
         output_dir = os.path.join(args.output_dir, 'gnn_preds'),
         weights = os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'weights', model_name + '.pth'),
         conf = os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'confs', model_name + '.json'),
         normalizers = os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'normalizers', model_name + '.pkl'),
-        num_classes = args.num_classes
+        num_classes = args.num_classes,
+        disable_prior = False,
+        disable_morph_feats = False,
     )
     infer_gnn(newargs)
     return
 
 
 def run_postgraphs(args: Namespace, logger: Logger) -> None:
     logger.info('Parsing gnn output.')
@@ -137,15 +144,15 @@
     parser.add_argument('--input-dir', type=str, help='Folder containing patches to process.', required=True)
     parser.add_argument('--output-dir', type=str, help='Folder where to save results. Additional subfolder will be created.', required=True)
     parser.add_argument('--gpu', type=str, default='0')
     parser.add_argument('--num-workers', type=int, default=0)
     parser.add_argument('--best-num-layers', type=str, help='Optimal number of layers when training GNNs.')
     parser.add_argument('--best-dropout', type=str, help='Optimal dropout rate when training GNNs')
     parser.add_argument('--best-norm-type', type=str, help='Optimal type of normalization layers when training GNNs')
-    parser.add_argument('--best-arch', type=str, help='Best architecture (convolutional, attention, ...) when training GNNs', required=True)
+    parser.add_argument('--best-arch', type=str, help='Best architecture (convolutional, attention, ...) when training GNNs', required=True, choices=['GCN', 'ATT', 'HATT', 'SAGE', 'BOOST'])
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
     return parser
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
```

### Comparing `tumourkit-0.4.1/tumourkit/make_dirs.py` & `tumourkit-0.5.0/tumourkit/make_dirs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/postprocessing/join_graph_gt.py` & `tumourkit-0.5.0/tumourkit/postprocessing/join_graph_gt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/postprocessing/join_hovprob_graph.py` & `tumourkit-0.5.0/tumourkit/postprocessing/join_hovprob_graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/postprocessing/merge_cells.py` & `tumourkit-0.5.0/tumourkit/postprocessing/merge_cells.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,36 +15,25 @@
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
+import os
 from typing import Callable, Dict, Tuple
 import numpy as np
 import pandas as pd
 import skimage
-import os
-import sys
-
-PKG_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-sys.path.append(PKG_DIR)
-
-from utils.preprocessing import (
+from ..utils.preprocessing import (
     parse_path, create_dir, get_names, save_pngcsv, read_labels
 )
 import argparse
+from tqdm import tqdm
 
-parser = argparse.ArgumentParser()
-parser.add_argument('--png-dir', type=str, required=True,
-                    help='Path to png files.')
-parser.add_argument('--csv-dir', type=str, required=True,
-                    help='Path to csv files.')
-parser.add_argument('--output-path', type=str, required=True,
-                    help='Path to save files.')
 
 MAX_CELLS = 1500
 
 def create_id_map() -> Tuple[Callable[[np.ndarray], np.ndarray], Dict[int, Tuple[int,int]]]:
     """
     Map index to some function so that difference is unique per pair.
     Also returns the inverse mapping of the differences and the 
@@ -117,28 +106,40 @@
     assert next_ids.difference(curr_ids) == set([0]), "Indices doesn't match"
     remove_ids = curr_ids.difference(next_ids)
     csv.set_index('id', inplace=True)
     csv.drop(remove_ids, axis='index', inplace=True)
     csv.reset_index(inplace=True)
     return csv
 
-if __name__=='__main__':
+
+def _create_parser():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--png-dir', type=str, required=True,
+                        help='Path to png files.')
+    parser.add_argument('--csv-dir', type=str, required=True,
+                        help='Path to csv files.')
+    parser.add_argument('--output-path', type=str, required=True,
+                        help='Path to save files.')
+    return parser
+
+
+def main():
+    parser = _create_parser()
     args = parser.parse_args()
-    PNG_DIR = parse_path(args.png_dir)
-    CSV_DIR = parse_path(args.csv_dir)
-    OUTPUT_PATH = parse_path(args.output_path)
-    PNG_OUT_PATH = OUTPUT_PATH + '/postPNG/'
-    CSV_OUT_PATH = OUTPUT_PATH + '/postCSV/'
-    create_dir(OUTPUT_PATH)
-    create_dir(PNG_OUT_PATH)
-    create_dir(CSV_OUT_PATH)
+    png_dir = parse_path(args.png_dir)
+    csv_dir = parse_path(args.csv_dir)
+    output_path = parse_path(args.output_path)
+    png_out_path = os.path.join(output_path, 'postPNG')
+    csv_out_path = os.path.join(output_path, 'postCSV')
+    create_dir(output_path)
+    create_dir(png_out_path)
+    create_dir(csv_out_path)
 
-    names = get_names(PNG_DIR, '.GT_cells.png')
+    names = get_names(png_dir, '.GT_cells.png')
     vec_mapping, inv_diff_mapping = create_id_map()
-    for k, name in enumerate(names):
-        print('Progress: {:2d}/{}'.format(k+1, len(names)), end="\r")
-        png, csv = read_labels(name, PNG_DIR, CSV_DIR)
+    for k, name in tqdm(enumerate(names)):
+        png, csv = read_labels(name, png_dir, csv_dir)
         if png is None or csv is None: continue
         assert(np.max(csv.id) < MAX_CELLS), "Exceeded maximum number of cells."
         png = merge_cells(png, vec_mapping, inv_diff_mapping)
         csv = remove_lost_ids(png, csv)
-        save_pngcsv(png, csv, PNG_OUT_PATH, CSV_OUT_PATH, name)
+        save_pngcsv(png, csv, png_out_path, csv_out_path, name)
```

### Comparing `tumourkit-0.4.1/tumourkit/postprocessing/rswoosh.py` & `tumourkit-0.5.0/tumourkit/postprocessing/rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/__init__.py` & `tumourkit-0.5.0/tumourkit/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/centroids2png.py` & `tumourkit-0.5.0/tumourkit/preprocessing/centroids2png.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/centroidspng2csv.py` & `tumourkit-0.5.0/tumourkit/preprocessing/centroidspng2csv.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/geojson2pngcsv.py` & `tumourkit-0.5.0/tumourkit/preprocessing/geojson2pngcsv.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,36 +16,19 @@
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 from typing import Dict, Any, Tuple, List, Optional
 import argparse
-import geojson
 from skimage.draw import polygon
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
-from ..utils.preprocessing import parse_path, create_dir, get_names, save_pngcsv
-    
-
-def read_gson(name: str, path: str) -> List[Dict[str,Any]]:
-    """
-    Reads the GeoJSON file at the specified path with the given name.
-
-    :param name: The base name of the file (without extension).
-    :type name: str
-    :param path: The path to the directory containing the file.
-    :type path: str
-    :return: The contents of the GeoJSON file as a list of dictionaries.
-    :rtype: List[Dict[str, Any]]
-    """
-    with open(path + name + '.geojson', 'r') as f:
-        gson = geojson.load(f)
-    return gson
+from ..utils.preprocessing import parse_path, create_dir, get_names, save_pngcsv, read_gson
 
 
 def geojson2pngcsv(gson: List[Dict[str, Any]], num_classes: Optional[int] = 2) -> Tuple[np.ndarray, pd.DataFrame]:
     """
     Computes PNG and CSV labels from GeoJSON.
 
     :param gson: A list of GeoJSON features.
```

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/graph2centroids.py` & `tumourkit-0.5.0/tumourkit/preprocessing/graph2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/hovernet2centroids.py` & `tumourkit-0.5.0/tumourkit/preprocessing/hovernet2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/hovernet2geojson.py` & `tumourkit-0.5.0/tumourkit/preprocessing/hovernet2geojson.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/png2graph.py` & `tumourkit-0.5.0/tumourkit/preprocessing/png2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/pngcsv2centroids.py` & `tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/pngcsv2geojson.py` & `tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2geojson.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,36 +19,21 @@
 Contact information: joseperez2000@hotmail.es
 """
 from typing import List, Dict, Any, Optional
 import argparse
 import pandas as pd
 import cv2
 import numpy as np
-import geojson
 from tqdm import tqdm
 from ..utils.preprocessing import (
     get_names, create_dir, parse_path,
-    format_contour, create_geojson, read_labels
+    format_contour, create_geojson, read_labels,
+    save_geojson
 )
 
-def save_geojson(gson: List[Dict[str, Any]], name: str, path: str) -> None:
-    """
-    Save a list of geojson features to a file with the given name at the
-    specified path.
-
-    :param gson: A list of geojson features to save.
-    :type gson: List[Dict[str, Any]]
-    :param name: The name of the file to save.
-    :type name: str
-    :param path: The path to save the file at.
-    :type path: str
-    """
-    with open(path + name + '.geojson', 'w') as f:
-        geojson.dump(gson, f)
-
 
 def create_mask(png: np.ndarray, csv: pd.DataFrame, label: int) -> np.ndarray:
     """
     Returns an image with only the pixels of the class given in the label.
     
     :param png: Segmentation mask with indices as pixel values.
     :type png: np.ndarray
@@ -79,15 +64,15 @@
     :param num_classes: The number of classes in the segmentation mask, defaults to 2.
     :type num_classes: Optional[int], optional
     :return: A list of dictionaries with the geojson features of the contours of the specified class of cells.
     :rtype: List[Dict[str, Any]]
     """
     mask = create_mask(png, csv, label)
     contours, _ = cv2.findContours(mask, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_SIMPLE)
-    contours = filter(lambda x: len(x[0]) >= 3, [(format_contour(c), label) for c in contours])
+    contours = filter(lambda x: len(x[0]) >= 4, [(format_contour(c), label) for c in contours])
     return create_geojson(contours, num_classes)
 
 
 def pngcsv2geojson(png: np.ndarray, csv: pd.DataFrame, num_classes: Optional[int] = 2) -> List[Dict[str, Any]]:
     """
     Computes the GeoJSON representation of contours in the given PNG image based on the provided CSV labels.
 
@@ -103,15 +88,15 @@
     total_contours = []
     for _, (idx, cell_label) in csv.iterrows():
         mask = png.copy()
         mask[mask != idx] = 0
         mask[mask == idx] = 1
         mask = mask.astype(np.uint8)
         contours, _ = cv2.findContours(mask, mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_SIMPLE)
-        contours = filter(lambda x: len(x[0]) >= 3, [(format_contour(c), cell_label) for c in contours])
+        contours = filter(lambda x: len(x[0]) >= 4, [(format_contour(c), cell_label) for c in contours])
         total_contours.extend(create_geojson(contours, num_classes))
         del mask
     return total_contours
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
```

### Comparing `tumourkit-0.4.1/tumourkit/preprocessing/pngcsv2graph.py` & `tumourkit-0.5.0/tumourkit/preprocessing/pngcsv2graph.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/profiling/cpairs_profile.py` & `tumourkit-0.5.0/tumourkit/profiling/cpairs_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/profiling/rswoosh_profile.py` & `tumourkit-0.5.0/tumourkit/profiling/rswoosh_profile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/evaluate.py` & `tumourkit-0.5.0/tumourkit/segmentation/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,34 +24,49 @@
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 import pandas as pd
 import numpy as np
-from typing import List, Tuple
-from sklearn.metrics import f1_score, accuracy_score, roc_auc_score
+from typing import List, Tuple, Dict
 
 from ..utils.preprocessing import read_names, read_centroids
 from ..utils.nearest import generate_tree, find_nearest
+from ..utils.classification import metrics_from_predictions
 
 import argparse
+from argparse import Namespace
+import logging
+from logging import Logger
 
 
 def get_confusion_matrix(
     gt_centroids: List[Tuple[int,int,int]], 
     pred_centroids: List[Tuple[int,int,int]]
     ) -> np.ndarray:
     """
     Each centroid is represented by a 3-tuple with (X, Y, class).
     Matrix has (N+1)x(N+1) entries, one more for background when no match is found.
     N is the maximum value encountered for class.
     """
+    if len(gt_centroids) == 0 and len(pred_centroids) == 0:
+        return np.array([[0]])
     if len(gt_centroids) == 0:
-        return None
+        N = np.max(pred_centroids[:,2])
+        M = np.zeros((N+1,N+1))
+        classes, freqs = np.unique(pred_centroids[:,2], return_counts=True)
+        M[0, classes] += freqs
+        return M
+    if len(pred_centroids) == 0:
+        N = np.max(gt_centroids[:,2])
+        M = np.zeros((N+1,N+1))
+        classes, freqs = np.unique(gt_centroids[:,2], return_counts=True)
+        M[classes, 0] += freqs
+        return M
     if type(gt_centroids) == list:
         gt_centroids = np.array(gt_centroids)
     if type(pred_centroids) == list:
         pred_centroids = np.array(pred_centroids)
     N = int(max(np.max(gt_centroids[:,2]), np.max(pred_centroids[:,2])))
     assert min(np.min(gt_centroids[:,2]), np.min(pred_centroids[:,2])) > 0, 'Zero should not be a class.'
     gt_tree = generate_tree(gt_centroids[:,:2])
@@ -75,14 +90,15 @@
     gt_centroids: List[Tuple[int,int,int]], 
     pred_centroids: List[Tuple[int,int,int]]
     ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Each centroid is represented by a 3-tuple with (X, Y, class).
     Class is 1=non-tumour, 2=tumour.
     Returns true and predicted labels ordered by their correspondences.
+    Returned labels start at 0.
     """
     if len(gt_centroids) == 0:
         return None, None
 
     gt_tree = generate_tree(gt_centroids[:,:2])
     pred_tree = generate_tree(pred_centroids[:,:2])
     true_labels, pred_labels = [], []
@@ -90,38 +106,14 @@
         closest_id = find_nearest(point[:2], pred_tree)
         closest = pred_centroids[closest_id]
         if closest[2] != -1 and point[2] != -1 and point_id == find_nearest(closest[:2], gt_tree):
             true_labels.append(point[2]-1)
             pred_labels.append(closest[2]-1)
     return np.array(true_labels), np.array(pred_labels)
 
-def compute_percentage(arr: np.ndarray) -> float:
-    """
-    arr is an array of integers representing classes
-    It returns the the percentage of class 2: #2 / (#1 + #2)
-    """
-    n_one = np.sum(arr==1)
-    n_two = np.sum(arr==2)
-    return n_two / (n_one + n_two), n_one, n_two
-
-def compute_metrics(true_labels: np.ndarray, pred_labels: np.ndarray) -> Tuple[float, float, float, float]:
-    """
-    Given arrays of binary prediction and true labels,
-    returns F1 score, Accuracy, ROC AUC and percentage error.
-    """
-    f1 = f1_score(true_labels, pred_labels, zero_division=1)
-    acc = accuracy_score(true_labels, pred_labels)
-    if len(np.unique(true_labels)) > 1:
-        auc = roc_auc_score(true_labels, pred_labels)
-    else:
-        auc = -1
-    true_perc, _, _ = compute_percentage(true_labels+1)
-    pred_perc, _, _ = compute_percentage(pred_labels+1)
-    err = abs(true_perc - pred_perc)
-    return f1, acc, auc, err
 
 def compute_f1_score_from_matrix(conf_mat: np.ndarray, cls: int) -> float:
     """
     Returns f1 score of given class against the rest.
     If no positive or predictive positive classes are found, None is returned.
     """
     if cls == 0:
@@ -181,110 +173,145 @@
         res = np.zeros((n,n))
         res[:m,:m] += B
         res += A
     return res
 
 
 def save_csv(
-    metrics: List[Tuple[str,float,float,float,float,float,float]], 
+    metrics: Dict[str, List[float]], 
     save_path: str
     ) -> None:
     """
     Saves metrics in csv format for later use.
-    Columns: 'name', 'F1', 'Accuracy', 'ROC_AUC', 'Perc_err'
+    Columns depend on dictionary keys.
     """
     metrics_df = pd.DataFrame(metrics)
     metrics_df.to_csv(save_path + '.csv', index=False)
 
 def save_debug_matrix(
     mat: np.ndarray,
     save_path: str
     ) -> None:
     """
-    Saves metrics in csv format for later use.
-    Columns: 'name', 'F1', 'Accuracy', 'ROC_AUC', 'Perc_err'
+    Saves confusion matrices for debug purposes.
     """
-    metrics_df = pd.DataFrame(mat)
-    metrics_df.to_csv(save_path + '.csv')
+    conf_mat_df = pd.DataFrame(mat)
+    conf_mat_df.to_csv(save_path + '.csv')
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--names', type=str, required=True,
                         help='Path to txt file with names.')
     parser.add_argument('--gt-path', type=str, required=True,
                         help='Path to GT files.')
     parser.add_argument('--pred-path', type=str, required=True,
                         help='Path to prediction files.')
     parser.add_argument('--save-name', type=str, required=True,
                         help='Name to save the result, without file type.')
     parser.add_argument('--debug-path', type=str, default=None,
                         help='Name of file where to save confusion matrices (optional).')
+    parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
     return parser
 
 
-def main_with_args(args):
+def main_with_args(args: Namespace, logger: Logger):
     names = read_names(args.names)
-    metrics = {
-        'Name': [], 'F1': [], 'Accuracy': [], 'ROC_AUC': [], 'Perc_err': [],
-        'Macro F1': [], 'Weighted F1': [], 'Micro F1': []
-    }
+    if args.num_classes == 2:
+        metrics = {
+            'Name': [], 'F1': [], 'Accuracy': [], 'ROC_AUC': [], 'Perc_err': [], 'ECE': [],
+            'Macro F1 (bkgr)': [], 'Weighted F1 (bkgr)': [], 'Micro F1 (bkgr)': []
+        }
+    else:
+        metrics = {
+            'Name': [], 'Macro F1': [], 'Weighted F1': [], 'Micro F1': [], 'ECE': [],
+            'Macro F1 (bkgr)': [], 'Weighted F1 (bkgr)': [], 'Micro F1 (bkgr)': []
+        }
     global_conf_mat = None
     global_pred, global_true = [], []
     for k, name in enumerate(names):
-        print('Progress: {:2d}/{}'.format(k+1, len(names)), end="\r")
+        logger.info('Progress: {:2d}/{}'.format(k+1, len(names)))
         metrics['Name'].append(name)
         # Read
         gt_centroids = read_centroids(name, args.gt_path)
         pred_centroids = read_centroids(name, args.pred_path)
         # Compute pairs and confusion matrix
         conf_mat = get_confusion_matrix(gt_centroids, pred_centroids)
         if args.debug_path is not None:
             save_debug_matrix(conf_mat, args.debug_path + '_' + name)
-        if len(conf_mat) == 3:
+        try:
             true_labels, pred_labels = get_pairs(gt_centroids, pred_centroids)
-        else:
+        except Exception as e:
+            logger.error(e)
+            logger.error(name)
+            _metrics = [-1] * 5 if args.num_classes == 2 else [-1] * 4
+            macro_bkgr, weighted_bkgr, micro_bkgr = -1, -1, -1
             true_labels, pred_labels = None, None
         # Save for later
         if true_labels is not None and pred_labels is not None:
             global_true.extend(true_labels)
             global_pred.extend(pred_labels)
         if global_conf_mat is None:
             global_conf_mat = conf_mat
         else:
             global_conf_mat = add_matrices(global_conf_mat, conf_mat)
         # Compute per image scores and percentages
         try:
-            if true_labels is not None and pred_labels is not None:
-                f1, acc, auc, err = compute_metrics(true_labels, pred_labels)
-            else:
-                f1, acc, auc, err = -1, -1, -1, -1
-            macro, weighted, micro = compute_metrics_from_matrix(conf_mat)
+            _metrics = metrics_from_predictions(true_labels, pred_labels, None, args.num_classes)
+            macro_bkgr, weighted_bkgr, micro_bkgr = compute_metrics_from_matrix(conf_mat)
         except Exception as e:
-            print(e)
-            print(name)
-        metrics['F1'].append(f1)
-        metrics['Accuracy'].append(acc)
-        metrics['ROC_AUC'].append(auc)
-        metrics['Perc_err'].append(err)
-        metrics['Macro F1'].append(macro)
-        metrics['Weighted F1'].append(weighted)
-        metrics['Micro F1'].append(micro)
+            logger.error(e)
+            logger.error(name)
+            _metrics = [-1] * 5 if args.num_classes == 2 else [-1] * 4
+            macro_bkgr, weighted_bkgr, micro_bkgr = -1, -1, -1
+        if args.num_classes == 2:
+            acc, f1, auc, perc_error, ece = _metrics
+            metrics['F1'].append(f1)
+            metrics['Accuracy'].append(acc)
+            metrics['ROC_AUC'].append(auc)
+            metrics['Perc_err'].append(perc_error)
+            metrics['ECE'].append(ece)
+            metrics['Macro F1 (bkgr)'].append(macro_bkgr)
+            metrics['Weighted F1 (bkgr)'].append(weighted_bkgr)
+            metrics['Micro F1 (bkgr)'].append(micro_bkgr)
+        else:
+            micro, macro, weighted, ece = _metrics
+            metrics['Macro F1'].append(macro)
+            metrics['Weighted F1'].append(weighted)
+            metrics['Micro F1'].append(micro)
+            metrics['ECE'].append(ece)
+            metrics['Macro F1 (bkgr)'].append(macro_bkgr)
+            metrics['Weighted F1 (bkgr)'].append(weighted_bkgr)
+            metrics['Micro F1 (bkgr)'].append(micro_bkgr)
     if args.debug_path is not None:
         save_debug_matrix(global_conf_mat, args.debug_path + '_global')
     save_csv(metrics, args.save_name)
     # Global scores and percentages
-    if len(global_true) > 0 and len(global_pred) > 0:
-        f1, acc, auc, err = compute_metrics(np.array(global_true), np.array(global_pred))
+    _global_metrics = metrics_from_predictions(np.array(global_true), np.array(global_pred), None, args.num_classes)
+    macro_bkgr, weighted_bkgr, micro_bkgr = compute_metrics_from_matrix(global_conf_mat)
+    if args.num_classes == 2:
+        acc, f1, auc, perc_error, ece = _global_metrics
+        global_metrics = {
+            'Name': ['All'], 'F1': [f1], 'Accuracy': [acc], 'ROC_AUC': [auc], 'Perc_err': [perc_error], 'ECE': [ece],
+            'Macro F1 (bkgr)': [macro_bkgr], 'Weighted F1 (bkgr)': [weighted_bkgr], 'Micro F1 (bkgr)': [micro_bkgr]
+        }
     else:
-        f1, acc, auc, err = -1, -1, -1, -1
-    macro, weighted, micro = compute_metrics_from_matrix(global_conf_mat)
-    global_metrics = {
-        'Name': ['All'], 'F1': [f1], 'Accuracy': [acc], 'ROC_AUC': [auc], 'Perc_err': [err],
-        'Macro F1': [macro], 'Weighted F1': [weighted], 'Micro F1': [micro]
-    }
+        micro, macro, weighted, ece = _global_metrics
+        global_metrics = {
+            'Name': ['All'], 'Macro F1': [macro], 'Weighted F1': [weighted], 'Micro F1': [micro], 'ECE': [ece],
+            'Macro F1 (bkgr)': [macro_bkgr], 'Weighted F1 (bkgr)': [weighted_bkgr], 'Micro F1 (bkgr)': [micro_bkgr]
+        }
     save_csv(global_metrics, args.save_name + '_all')
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
-    main(args)
+
+    logger = logging.getLogger('eval_segment')
+    logger.setLevel(logging.DEBUG)
+    ch = logging.StreamHandler()
+    ch.setLevel(logging.DEBUG)
+    formatter = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
+    ch.setFormatter(formatter)
+    logger.addHandler(ch)
+
+    main(args, logger)
```

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/config.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/config.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/dataloader/augs.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/augs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/dataloader/infer_loader.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/dataloader/train_loader.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/extract_patches.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/extract_patches.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/infer/base.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/infer/tile.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/tile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/infer/wsi.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/infer/wsi.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/metrics/stats_utils.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/patch_extractor.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/utils.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/viz_utils.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/misc/wsi_handler.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/opt.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/targets.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     # TODO: deal with 1 label warning
     crop_ann = morph.remove_small_objects(crop_ann, min_size=30)
 
     x_map = np.zeros(orig_ann.shape[:2], dtype=np.float32)
     y_map = np.zeros(orig_ann.shape[:2], dtype=np.float32)
 
     inst_list = list(np.unique(crop_ann))
-    inst_list.remove(0)  # 0 is background
+    if 0 in inst_list:
+        inst_list.remove(0)  # 0 is background
     for inst_id in inst_list:
         inst_map = np.array(fixed_ann == inst_id, np.uint8)
         inst_box = get_bounding_box(inst_map)
 
         # expand the box by 2px
         # Because we first pad the ann at line 207, the bboxes
         # will remain valid after expansion
@@ -47,16 +48,19 @@
 
         if inst_map.shape[0] < 2 or inst_map.shape[1] < 2:
             continue
 
         # instance center of mass, rounded to nearest pixel
         inst_com = list(measurements.center_of_mass(inst_map))
 
-        inst_com[0] = int(inst_com[0] + 0.5)
-        inst_com[1] = int(inst_com[1] + 0.5)
+        try:
+            inst_com[0] = int(inst_com[0] + 0.5)
+            inst_com[1] = int(inst_com[1] + 0.5)
+        except:
+            continue
 
         inst_x_range = np.arange(1, inst_map.shape[1] + 1)
         inst_y_range = np.arange(1, inst_map.shape[0] + 1)
         # shifting center of pixels grid to instance center of mass
         inst_x_range -= inst_com[1]
         inst_y_range -= inst_com[0]
```

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/models/hovernet/utils.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_infer.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/engine.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,73 +133,76 @@
 
         # TODO: refactor this
         if chained:
             self.state.curr_epoch = 0
         self.state.global_state = shared_state
 
         while self.state.curr_epoch < nr_epoch:
-            self.state.reset_variable()  # * reset all EMA holder per epoch
+            try:
+                self.state.reset_variable()  # * reset all EMA holder per epoch
 
-            if not chained:
-                print("----------------EPOCH %d" % (self.state.curr_epoch + 1))
+                if not chained:
+                    print("----------------EPOCH %d" % (self.state.curr_epoch + 1))
 
-            self.__trigger_events(Events.EPOCH_STARTED)
+                self.__trigger_events(Events.EPOCH_STARTED)
 
-            pbar_format = (
-                "Processing: |{bar}| "
-                "{n_fmt}/{total_fmt}[{elapsed}<{remaining},{rate_fmt}]"
-            )
-            if self.engine_name == "train":
-                pbar_format += (
-                    "Batch = {postfix[1][Batch]:0.5f}|" "EMA = {postfix[1][EMA]:0.5f}"
+                pbar_format = (
+                    "Processing: |{bar}| "
+                    "{n_fmt}/{total_fmt}[{elapsed}<{remaining},{rate_fmt}]"
                 )
-                # * changing print char may break the bar so avoid it
-                pbar = tqdm.tqdm(
-                    total=len(self.dataloader),
-                    leave=True,
-                    initial=0,
-                    bar_format=pbar_format,
-                    ascii=True,
-                    postfix=["", dict(Batch=float("NaN"), EMA=float("NaN"))],
-                )
-            else:
-                pbar = tqdm.tqdm(
-                    total=len(self.dataloader),
-                    leave=True,
-                    bar_format=pbar_format,
-                    ascii=True,
-                )
-
-            for data_batch in self.dataloader:
-                self.__trigger_events(Events.STEP_STARTED)
-
-                step_run_info = [
-                    self.state.run_info,
-                    {
-                        "epoch": self.state.curr_epoch,
-                        "step": self.state.curr_global_step,
-                    },
-                ]
-                step_output = self.run_step(data_batch, step_run_info)
-                self.state.step_output = step_output
-
-                self.__trigger_events(Events.STEP_COMPLETED)
-                self.state.curr_global_step += 1
-                self.state.curr_epoch_step += 1
-
                 if self.engine_name == "train":
-                    pbar.postfix[1]["Batch"] = step_output["EMA"]["overall_loss"]
-                    pbar.postfix[1]["EMA"] = self.state.tracked_step_output["scalar"][
-                        "overall_loss"
+                    pbar_format += (
+                        "Batch = {postfix[1][Batch]:0.5f}|" "EMA = {postfix[1][EMA]:0.5f}"
+                    )
+                    # * changing print char may break the bar so avoid it
+                    pbar = tqdm.tqdm(
+                        total=len(self.dataloader),
+                        leave=True,
+                        initial=0,
+                        bar_format=pbar_format,
+                        ascii=True,
+                        postfix=["", dict(Batch=float("NaN"), EMA=float("NaN"))],
+                    )
+                else:
+                    pbar = tqdm.tqdm(
+                        total=len(self.dataloader),
+                        leave=True,
+                        bar_format=pbar_format,
+                        ascii=True,
+                    )
+
+                for data_batch in self.dataloader:
+                    self.__trigger_events(Events.STEP_STARTED)
+
+                    step_run_info = [
+                        self.state.run_info,
+                        {
+                            "epoch": self.state.curr_epoch,
+                            "step": self.state.curr_global_step,
+                        },
                     ]
-                pbar.update()
-            pbar.close()  # to flush out the bar before doing end of epoch reporting
-            self.state.curr_epoch += 1
-            self.__trigger_events(Events.EPOCH_COMPLETED)
-
-            # TODO: [CRITICAL] align the protocol
-            self.state.run_accumulated_output.append(
-                self.state.epoch_accumulated_output
-            )
+                    step_output = self.run_step(data_batch, step_run_info)
+                    self.state.step_output = step_output
+
+                    self.__trigger_events(Events.STEP_COMPLETED)
+                    self.state.curr_global_step += 1
+                    self.state.curr_epoch_step += 1
+
+                    if self.engine_name == "train":
+                        pbar.postfix[1]["Batch"] = step_output["EMA"]["overall_loss"]
+                        pbar.postfix[1]["EMA"] = self.state.tracked_step_output["scalar"][
+                            "overall_loss"
+                        ]
+                    pbar.update()
+                pbar.close()  # to flush out the bar before doing end of epoch reporting
+                self.state.curr_epoch += 1
+                self.__trigger_events(Events.EPOCH_COMPLETED)
+
+                # TODO: [CRITICAL] align the protocol
+                self.state.run_accumulated_output.append(
+                    self.state.epoch_accumulated_output
+                )
+            except Exception as e:
+                print(e)
 
         return
```

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/run_utils/utils.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/run_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/segmentation/hovernet/train.py` & `tumourkit-0.5.0/tumourkit/segmentation/hovernet/train.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/train_pipe.py` & `tumourkit-0.5.0/tumourkit/train_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,23 +149,44 @@
     """
     newargs = Namespace(
         train_node_dir = os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
         validation_node_dir = os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
         test_node_dir = os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
         log_dir = os.path.join(args.root_dir, 'gnn_logs'),
         early_stopping_rounds = 10,
-        batch_size = 10,
+        batch_size = 20,
         model_name = 'GCN',
-        save_file = os.path.join(args.root_dir, 'gnn_logs', 'gnn_results'),
+        save_file = os.path.join(args.root_dir, 'gnn_logs', 'gcn_results'),
         num_confs = 32,
         save_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn'),
         device = 'cpu' if args.gpu == '' else 'cuda',
         num_workers = args.num_workers,
         checkpoint_iters = -1,
-        num_classes = args.num_classes
+        num_classes = args.num_classes,
+        disable_prior = False,
+        disable_morph_feats = False,
+    )
+    train_gnn(newargs)
+    newargs = Namespace(
+        train_node_dir = os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
+        validation_node_dir = os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
+        test_node_dir = os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
+        log_dir = os.path.join(args.root_dir, 'gnn_logs'),
+        early_stopping_rounds = 10,
+        batch_size = 20,
+        model_name = 'ATT',
+        save_file = os.path.join(args.root_dir, 'gnn_logs', 'gat_results'),
+        num_confs = 32,
+        save_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn'),
+        device = 'cpu' if args.gpu == '' else 'cuda',
+        num_workers = args.num_workers,
+        checkpoint_iters = -1,
+        num_classes = args.num_classes,
+        disable_prior = False,
+        disable_morph_feats = False,
     )
     train_gnn(newargs)
     return
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
```

### Comparing `tumourkit-0.4.1/tumourkit/utils/folder2txt.py` & `tumourkit-0.5.0/tumourkit/utils/folder2txt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/utils/nearest.py` & `tumourkit-0.5.0/tumourkit/utils/nearest.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/utils/postprocessing.py` & `tumourkit-0.5.0/tumourkit/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.4.1/tumourkit/utils/preprocessing.py` & `tumourkit-0.5.0/tumourkit/utils/preprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
-
+import geojson
 import os
 from geojson import Feature, Polygon
 import cv2
 import pandas as pd
 import numpy as np
 import numpy.ma as ma
 import json
@@ -129,14 +129,30 @@
         csv = pd.read_csv(os.path.join(csv_dir, name + '.class.csv'), header=None)
         csv.columns = ['id', 'label']
         return csv
     except:
         return None
     
 
+def read_gson(name: str, path: str) -> List[Dict[str,Any]]:
+    """
+    Reads the GeoJSON file at the specified path with the given name.
+
+    :param name: The base name of the file (without extension).
+    :type name: str
+    :param path: The path to the directory containing the file.
+    :type path: str
+    :return: The contents of the GeoJSON file as a list of dictionaries.
+    :rtype: List[Dict[str, Any]]
+    """
+    with open(os.path.join(path, name + '.geojson'), 'r') as f:
+        gson = geojson.load(f)
+    return gson
+    
+
 def read_labels(name: str, png_dir: str, csv_dir: str) -> Tuple[np.ndarray, pd.DataFrame]:
     """
     Reads a PNG and CSV file from the specified directories and returns their contents as a tuple.
 
     :param name: The base name of the files (without extensions).
     :type name: str
     :param png_dir: The directory containing the PNG file.
@@ -187,15 +203,15 @@
     :return: A NumPy array containing the centroids with class -1 removed and coordinates converted to integers.
     :rtype: np.ndarray
 
     This function reads a CSV file from the specified directory containing centroids and returns their contents as a NumPy array.
     The function expects the CSV file to have specific column names: 'X', 'Y', and 'class'.
     Centroids with class -1 are dropped and the coordinates are converted to integers.
     """
-    centroid_csv = pd.read_csv(path + name + '.centroids.csv')
+    centroid_csv = pd.read_csv(os.path.join(path, name + '.centroids.csv'))
     centroid_csv = centroid_csv.drop(centroid_csv[centroid_csv['class']==-1].index)
     return centroid_csv.to_numpy(dtype=int)
 
 
 def read_graph(name: str, graph_dir: str) -> pd.DataFrame:
     """
     Reads a graph in CSV format from the specified directory and returns it as a Pandas DataFrame.
@@ -370,14 +386,31 @@
     :param path: The path to save the graph file to.
     :type path: str
     """
     graph.set_index('id', inplace=True)
     graph.sort_index(inplace=True)
     graph.to_csv(path)
 
+
+def save_geojson(gson: List[Dict[str, Any]], name: str, path: str) -> None:
+    """
+    Save a list of geojson features to a file with the given name at the
+    specified path.
+
+    :param gson: A list of geojson features to save.
+    :type gson: List[Dict[str, Any]]
+    :param name: The name of the file to save.
+    :type name: str
+    :param path: The path to save the file at.
+    :type path: str
+    """
+    with open(os.path.join(path, name + '.geojson'), 'w') as f:
+        geojson.dump(gson, f, sort_keys=True, indent=2)
+
+
 def get_centroid_by_id(img: np.ndarray, idx: int) -> Tuple[int, int]:
     """
     Given an image and an id representing a component, returns the centroid
     of the component as a tuple (x, y).
     
     :param img: A NumPy array representing the image.
     :type img: np.ndarray
```

### Comparing `tumourkit-0.4.1/tumourkit.egg-info/PKG-INFO` & `tumourkit-0.5.0/tumourkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.4.1
+Version: 0.5.0
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.4.1/tumourkit.egg-info/SOURCES.txt` & `tumourkit-0.5.0/tumourkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
+demo/app.py
 docs/buildenv/bin/rst2html.py
 docs/buildenv/bin/rst2html4.py
 docs/buildenv/bin/rst2html5.py
 docs/buildenv/bin/rst2latex.py
 docs/buildenv/bin/rst2man.py
 docs/buildenv/bin/rst2odt.py
 docs/buildenv/bin/rst2odt_prepstyles.py
@@ -32,32 +33,31 @@
 tests/png2graph_test.py
 tests/pngcsv2geojson_test.py
 tests/pngcsv2graph_test.py
 tests/read_nodes_test.py
 tests/remove_idx_test.py
 tests/rswoosh_test.py
 tumourkit/__init__.py
+tumourkit/eval_pipe.py
 tumourkit/infer_pipe.py
 tumourkit/make_dirs.py
 tumourkit/research_pipe.py
 tumourkit/train_pipe.py
 tumourkit.egg-info/PKG-INFO
 tumourkit.egg-info/SOURCES.txt
 tumourkit.egg-info/dependency_links.txt
 tumourkit.egg-info/entry_points.txt
 tumourkit.egg-info/requires.txt
 tumourkit.egg-info/top_level.txt
 tumourkit/classification/__init__.py
-tumourkit/classification/calibration_error.py
 tumourkit/classification/compute_imbalance.py
 tumourkit/classification/evaluate.py
 tumourkit/classification/infer.py
 tumourkit/classification/read_graph.py
-tumourkit/classification/read_nodes.py
-tumourkit/classification/train_gnn.py
+tumourkit/classification/train_graphs.py
 tumourkit/classification/train_xgboost.py
 tumourkit/classification/models/__init__.py
 tumourkit/classification/models/gat.py
 tumourkit/classification/models/gcn.py
 tumourkit/classification/models/hgao.py
 tumourkit/classification/models/norm.py
 tumourkit/postprocessing/__init__.py
@@ -72,14 +72,15 @@
 tumourkit/preprocessing/graph2centroids.py
 tumourkit/preprocessing/hovernet2centroids.py
 tumourkit/preprocessing/hovernet2geojson.py
 tumourkit/preprocessing/png2graph.py
 tumourkit/preprocessing/pngcsv2centroids.py
 tumourkit/preprocessing/pngcsv2geojson.py
 tumourkit/preprocessing/pngcsv2graph.py
+tumourkit/preprocessing/remove_uncertain.py
 tumourkit/profiling/cpairs_profile.py
 tumourkit/profiling/rswoosh_profile.py
 tumourkit/segmentation/__init__.py
 tumourkit/segmentation/evaluate.py
 tumourkit/segmentation/hovernet/__init__.py
 tumourkit/segmentation/hovernet/config.py
 tumourkit/segmentation/hovernet/extract_patches.py
@@ -113,12 +114,15 @@
 tumourkit/segmentation/hovernet/run_utils/engine.py
 tumourkit/segmentation/hovernet/run_utils/utils.py
 tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
 tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
 tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
 tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
 tumourkit/utils/__init__.py
+tumourkit/utils/calibration_error.py
 tumourkit/utils/classification.py
 tumourkit/utils/folder2txt.py
 tumourkit/utils/nearest.py
+tumourkit/utils/pipes.py
 tumourkit/utils/postprocessing.py
-tumourkit/utils/preprocessing.py
+tumourkit/utils/preprocessing.py
+tumourkit/utils/read_nodes.py
```

### Comparing `tumourkit-0.4.1/tumourkit.egg-info/entry_points.txt` & `tumourkit-0.5.0/tumourkit.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,13 +2,16 @@
 centroids2png = tumourkit.preprocessing.centroids2png:main
 centroidspng2csv = tumourkit.preprocessing.centroidspng2csv:main
 geojson2pngcsv = tumourkit.preprocessing.geojson2pngcsv:main
 graph2centroids = tumourkit.preprocessing.graph2centroids:main
 hovernet2centroids = tumourkit.preprocessing.hovernet2centroids:main
 hovernet2geojson = tumourkit.preprocessing.hovernet2geojson:main
 make_dirs = tumourkit.make_dirs:main
+merge_cells = tumourkit.postprocessing.merge_cells:main
 pngcsv2centroids = tumourkit.preprocessing.pngcsv2centroids:main
 pngcsv2geojson = tumourkit.preprocessing.pngcsv2geojson:main
 pngcsv2graph = tumourkit.preprocessing.pngcsv2graph:main
+remove_uncertain = tumourkit.preprocessing.remove_uncertain:main
+run_evaluation = tumourkit.eval_pipe:main
 run_inference = tumourkit.infer_pipe:main
 run_research = tumourkit.research_pipe:main
 run_training = tumourkit.train_pipe:main
```

### Comparing `tumourkit-0.4.1/tumourkit.egg-info/requires.txt` & `tumourkit-0.5.0/tumourkit.egg-info/requires.txt`

 * *Files identical despite different names*

