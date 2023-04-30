# Comparing `tmp/redisbench-admin-0.9.8.tar.gz` & `tmp/redisbench-admin-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redisbench-admin-0.9.8.tar", max compression
+gzip compressed data, was "redisbench-admin-0.9.9.tar", max compression
```

## Comparing `redisbench-admin-0.9.8.tar` & `redisbench-admin-0.9.9.tar`

### file list

```diff
@@ -1,242 +1,234 @@
--rw-r--r--   0        0        0    10768 2021-06-15 16:29:11.128690 redisbench-admin-0.9.8/LICENSE
--rw-r--r--   0        0        0     3559 2022-03-23 07:37:28.445828 redisbench-admin-0.9.8/README.md
--rw-r--r--   0        0        0     1544 2022-06-18 17:29:43.924103 redisbench-admin-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      473 2021-07-14 10:11:59.920250 redisbench-admin-0.9.8/redisbench_admin/__init__.py
--rw-r--r--   0        0        0     7518 2022-05-16 12:26:06.797206 redisbench-admin-0.9.8/redisbench_admin/cli.py
--rw-r--r--   0        0        0       95 2022-01-07 13:25:54.277123 redisbench-admin-0.9.8/redisbench_admin/commands/__init__.py
--rw-r--r--   0        0        0       95 2022-01-07 13:25:54.277123 redisbench-admin-0.9.8/redisbench_admin/commands/commands.json.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.128690 redisbench-admin-0.9.8/redisbench_admin/compare/__init__.py
--rw-r--r--   0        0        0     3871 2022-04-11 15:12:08.685465 redisbench-admin-0.9.8/redisbench_admin/compare/args.py
--rw-r--r--   0        0        0    15252 2022-06-15 14:53:53.517583 redisbench-admin-0.9.8/redisbench_admin/compare/compare.py
--rw-r--r--   0        0        0      101 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/deploy/__init__.py
--rw-r--r--   0        0        0     1732 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/deploy/args.py
--rw-r--r--   0        0        0     3791 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/deploy/deploy.py
--rw-r--r--   0        0        0       95 2021-07-09 16:09:51.103232 redisbench-admin-0.9.8/redisbench_admin/environments/__init__.py
--rw-r--r--   0        0        0     6681 2022-06-17 08:59:48.838442 redisbench-admin-0.9.8/redisbench_admin/environments/oss_cluster.py
--rw-r--r--   0        0        0     2474 2022-06-17 08:59:48.714443 redisbench-admin-0.9.8/redisbench_admin/environments/oss_standalone.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.128690 redisbench-admin-0.9.8/redisbench_admin/export/__init__.py
--rw-r--r--   0        0        0     3171 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/export/args.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/export/common/__init__.py
--rw-r--r--   0        0        0     4331 2021-11-08 18:09:40.005377 redisbench-admin-0.9.8/redisbench_admin/export/common/common.py
--rw-r--r--   0        0        0     9524 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/export/export.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/export/memtier_benchmark/__init__.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/export/memtier_benchmark/memtier_benchmark_json_format.py
--rw-r--r--   0        0        0      101 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/export/pyperf/__init__.py
--rw-r--r--   0        0        0     1678 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/export/pyperf/pyperf_json_format.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/export/redis_benchmark/__init__.py
--rw-r--r--   0        0        0     2522 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/export/redis_benchmark/metrics_definition.py
--rw-r--r--   0        0        0     5780 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/export/redis_benchmark/redis_benchmark_csv_format.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/extract/__init__.py
--rw-r--r--   0        0        0     1073 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/extract/args.py
--rw-r--r--   0        0        0      770 2021-07-14 10:11:59.924250 redisbench-admin-0.9.8/redisbench_admin/extract/extract.py
--rw-r--r--   0        0        0        0 2021-09-08 23:26:52.177729 redisbench-admin-0.9.8/redisbench_admin/grafana_api/__init__.py
--rw-r--r--   0        0        0     3416 2022-03-16 10:30:20.320291 redisbench-admin-0.9.8/redisbench_admin/grafana_api/app.py
--rw-r--r--   0        0        0     1212 2021-09-08 23:26:52.177729 redisbench-admin-0.9.8/redisbench_admin/grafana_api/args.py
--rw-r--r--   0        0        0     1613 2022-03-16 10:30:20.320291 redisbench-admin-0.9.8/redisbench_admin/grafana_api/grafana_api.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.132690 redisbench-admin-0.9.8/redisbench_admin/profilers/__init__.py
--rw-r--r--   0        0        0    12974 2022-03-16 22:45:51.318383 redisbench-admin-0.9.8/redisbench_admin/profilers/daemon.py
--rwxr-xr-x   0        0        0    35898 2021-06-15 16:29:11.136690 redisbench-admin-0.9.8/redisbench_admin/profilers/flamegraph.pl
--rw-r--r--   0        0        0    27756 2022-05-09 10:42:15.144935 redisbench-admin-0.9.8/redisbench_admin/profilers/perf.py
--rw-r--r--   0        0        0     4949 2022-03-16 22:45:51.318383 redisbench-admin-0.9.8/redisbench_admin/profilers/perf_daemon_caller.py
--rw-r--r--   0        0        0     3949 2022-01-20 13:42:30.830247 redisbench-admin-0.9.8/redisbench_admin/profilers/pprof.py
--rw-r--r--   0        0        0      510 2021-07-23 11:11:38.187080 redisbench-admin-0.9.8/redisbench_admin/profilers/profilers.py
--rw-r--r--   0        0        0    11971 2022-05-09 10:42:15.148934 redisbench-admin-0.9.8/redisbench_admin/profilers/profilers_local.py
--rw-r--r--   0        0        0     2744 2022-01-20 13:42:30.830247 redisbench-admin-0.9.8/redisbench_admin/profilers/profilers_schema.py
--rwxr-xr-x   0        0        0    10307 2021-06-15 16:29:11.136690 redisbench-admin-0.9.8/redisbench_admin/profilers/stackcollapse-perf.pl
--rw-r--r--   0        0        0     4618 2021-09-08 23:26:52.177729 redisbench-admin-0.9.8/redisbench_admin/profilers/vtune.py
--rw-r--r--   0        0        0      920 2022-03-16 10:30:20.320291 redisbench-admin-0.9.8/redisbench_admin/results/glove-100-angular/10/redisearch-hnsw/build_stats.hdf5
--rw-r--r--   0        0        0 18876448 2022-03-16 10:30:20.352292 redisbench-admin-0.9.8/redisbench_admin/results/mnist-784-euclidean/10/redisearch-hnsw/build_stats.hdf5
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.136690 redisbench-admin-0.9.8/redisbench_admin/run/__init__.py
--rw-r--r--   0        0        0      101 2021-06-16 17:00:41.502772 redisbench-admin-0.9.8/redisbench_admin/run/aibench_run_inference_redisai_vision/__init__.py
--rw-r--r--   0        0        0     1829 2021-07-14 10:11:59.924250 redisbench-admin-0.9.8/redisbench_admin/run/aibench_run_inference_redisai_vision/aibench_run_inference_redisai_vision.py
--rw-r--r--   0        0        0      101 2022-03-16 10:30:20.352292 redisbench-admin-0.9.8/redisbench_admin/run/ann/__init__.py
--rw-r--r--   0        0        0     1288 2022-03-16 10:30:20.352292 redisbench-admin-0.9.8/redisbench_admin/run/ann/ann.py
--rw-r--r--   0        0        0       13 2022-03-07 00:43:14.035859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/.dockerignore
--rw-r--r--   0        0        0       62 2022-03-07 00:43:14.035859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/.git
--rw-r--r--   0        0        0     3361 2022-03-07 00:43:14.035859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/.github/workflows/benchmarks.yml
--rw-r--r--   0        0        0      158 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/.gitignore
--rw-r--r--   0        0        0     1074 2022-03-07 00:43:14.035859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/LICENSE
--rw-r--r--   0        0        0    10452 2022-03-07 00:43:14.035859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/README.md
--rw-r--r--   0        0        0    48804 2022-03-07 00:43:31.995887 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/algos.yaml
--rw-r--r--   0        0        0     2316 2022-03-07 00:43:14.035859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/algosP.yaml
--rw-r--r--   0        0        0       75 2022-03-08 16:11:29.713446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/__init__.py
--rw-r--r--   0        0        0      225 2022-03-20 09:25:44.357661 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      197 2022-03-20 09:25:44.981663 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/__pycache__/constants.cpython-36.pyc
--rw-r--r--   0        0        0    17551 2022-03-20 09:25:44.661662 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/__pycache__/datasets.cpython-36.pyc
--rw-r--r--   0        0        0     2033 2022-03-20 09:25:44.873663 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/__pycache__/distance.cpython-36.pyc
--rw-r--r--   0        0        0     8610 2022-03-20 09:25:44.365661 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/__pycache__/main.cpython-36.pyc
--rw-r--r--   0        0        0     2723 2022-03-20 09:25:45.033663 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/__pycache__/results.cpython-36.pyc
--rw-r--r--   0        0        0    10002 2022-03-20 09:25:45.041663 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/__pycache__/runner.cpython-36.pyc
--rw-r--r--   0        0        0        0 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/__init__.py
--rw-r--r--   0        0        0      186 2022-03-20 09:25:44.981663 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0     5131 2022-03-20 09:25:44.985663 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/__pycache__/definitions.cpython-36.pyc
--rw-r--r--   0        0        0      819 2022-03-08 16:11:29.713446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/annoy.py
--rw-r--r--   0        0        0      765 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/balltree.py
--rw-r--r--   0        0        0     1013 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/base.py
--rw-r--r--   0        0        0     4659 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/bruteforce.py
--rw-r--r--   0        0        0      502 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/ckdtree.py
--rw-r--r--   0        0        0     1021 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/datasketch.py
--rw-r--r--   0        0        0     6746 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/definitions.py
--rw-r--r--   0        0        0     7665 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/diskann.py
--rw-r--r--   0        0        0      951 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/dolphinnpy.py
--rw-r--r--   0        0        0      584 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/dummy_algo.py
--rw-r--r--   0        0        0     3874 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/elasticsearch.py
--rw-r--r--   0        0        0     4482 2022-03-08 16:11:29.717445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/elastiknn.py
--rw-r--r--   0        0        0     3992 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss.py
--rw-r--r--   0        0        0     2018 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss_gpu.py
--rw-r--r--   0        0        0     1175 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss_hnsw.py
--rw-r--r--   0        0        0      950 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/flann.py
--rw-r--r--   0        0        0     1277 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/hnswlib.py
--rw-r--r--   0        0        0      759 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/kdtree.py
--rw-r--r--   0        0        0     1280 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/kgraph.py
--rw-r--r--   0        0        0      972 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/lshf.py
--rw-r--r--   0        0        0     3836 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/milvus.py
--rw-r--r--   0        0        0     1495 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/mrpt.py
--rw-r--r--   0        0        0      919 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/n2.py
--rw-r--r--   0        0        0     1739 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/nearpy.py
--rw-r--r--   0        0        0     2936 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/nmslib.py
--rw-r--r--   0        0        0     4421 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/onng_ngt.py
--rw-r--r--   0        0        0     3622 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/opensearchknn.py
--rw-r--r--   0        0        0     2971 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/panng_ngt.py
--rw-r--r--   0        0        0     1669 2022-03-08 16:11:29.721445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/puffinn.py
--rw-r--r--   0        0        0     3995 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/pynndescent.py
--rw-r--r--   0        0        0     4380 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/qg_ngt.py
--rw-r--r--   0        0        0     4061 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/redisearch.py
--rw-r--r--   0        0        0      642 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/rpforest.py
--rw-r--r--   0        0        0     1249 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/scann.py
--rw-r--r--   0        0        0      928 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/sptag.py
--rw-r--r--   0        0        0     7629 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/subprocess.py
--rw-r--r--   0        0        0     4807 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/vald.py
--rw-r--r--   0        0        0     2049 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/vespa.py
--rw-r--r--   0        0        0       22 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/constants.py
--rw-r--r--   0        0        0     1130 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/data.py
--rw-r--r--   0        0        0    24462 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/datasets.py
--rw-r--r--   0        0        0     1679 2022-03-08 16:11:29.725445 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/distance.py
--rw-r--r--   0        0        0    11671 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/main.py
--rw-r--r--   0        0        0       77 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/__init__.py
--rw-r--r--   0        0        0     6971 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/metrics.py
--rw-r--r--   0        0        0      617 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/plot_variants.py
--rw-r--r--   0        0        0     5593 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/utils.py
--rw-r--r--   0        0        0     2497 2022-03-08 16:11:29.729446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/results.py
--rw-r--r--   0        0        0    12752 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/runner.py
--rw-r--r--   0        0        0      346 2022-03-08 16:11:29.729446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/create_dataset.py
--rw-r--r--   0        0        0     6646 2022-03-22 13:18:04.410527 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/create_hybrid_dataset.py
--rw-r--r--   0        0        0     4639 2022-03-10 13:34:18.945512 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/create_text_to_image_ds.py
--rw-r--r--   0        0        0     9582 2022-03-08 16:11:29.729446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/create_website.py
--rw-r--r--   0        0        0      293 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile
--rw-r--r--   0        0        0      139 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.annoy
--rw-r--r--   0        0        0       84 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.datasketch
--rw-r--r--   0        0        0     1728 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.diskann
--rw-r--r--   0        0        0     1930 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.diskann_pq
--rw-r--r--   0        0        0      152 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.dolphinn
--rw-r--r--   0        0        0     1518 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.elasticsearch
--rw-r--r--   0        0        0     2242 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.elastiknn
--rw-r--r--   0        0        0      549 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.faiss
--rw-r--r--   0        0        0      316 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.flann
--rw-r--r--   0        0        0      283 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.hnswlib
--rw-r--r--   0        0        0      318 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.kgraph
--rw-r--r--   0        0        0      186 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.mih
--rw-r--r--   0        0        0     1213 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.milvus
--rw-r--r--   0        0        0      100 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.mrpt
--rw-r--r--   0        0        0       92 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.n2
--rw-r--r--   0        0        0      148 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.nearpy
--rw-r--r--   0        0        0      413 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.ngt
--rw-r--r--   0        0        0      443 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.nmslib
--rw-r--r--   0        0        0     1719 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.opensearchknn
--rw-r--r--   0        0        0      171 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.puffinn
--rw-r--r--   0        0        0      105 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.pynndescent
--rw-r--r--   0        0        0      582 2022-03-07 00:43:31.995887 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.redisearch
--rw-r--r--   0        0        0      145 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.rpforest
--rw-r--r--   0        0        0      105 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.scann
--rw-r--r--   0        0        0       74 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.scipy
--rw-r--r--   0        0        0       83 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.sklearn
--rw-r--r--   0        0        0     1191 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.sptag
--rw-r--r--   0        0        0      227 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.vald
--rw-r--r--   0        0        0      730 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.vespa
--rw-r--r--   0        0        0     2105 2022-03-08 16:11:29.729446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install.py
--rw-r--r--   0        0        0      541 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/logging.conf
--rw-r--r--   0        0        0     9888 2022-06-16 09:38:41.817556 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/multirun.py
--rw-r--r--   0        0        0     5845 2022-03-08 16:11:29.733446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/plot.py
--rwxr-xr-x   0        0        0      207 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/bf-runner
--rw-r--r--   0        0        0     6616 2022-03-08 16:11:29.733446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/bf-runner.py
--rw-r--r--   0        0        0     2638 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/ext-add-query-metric.md
--rw-r--r--   0        0        0     2464 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/ext-batch-queries.md
--rw-r--r--   0        0        0     2988 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/ext-prepared-queries.md
--rw-r--r--   0        0        0     1856 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/ext-query-parameters.md
--rw-r--r--   0        0        0     7539 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/specification.md
--rw-r--r--   0        0        0      150 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/requirements.txt
--rw-r--r--   0        0        0      158 2022-03-07 00:43:14.039859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/requirements_py38.txt
--rwxr-xr-x   0        0        0   215273 2022-03-07 00:43:14.043859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/fashion-mnist-784-euclidean.png
--rwxr-xr-x   0        0        0   122473 2022-03-07 00:43:14.043859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/gist-960-euclidean.png
--rwxr-xr-x   0        0        0   224400 2022-03-07 00:43:14.043859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/glove-100-angular.png
--rwxr-xr-x   0        0        0   226384 2022-03-07 00:43:14.047859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/glove-25-angular.png
--rw-r--r--   0        0        0   235553 2022-03-07 00:43:14.047859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/lastfm-64-dot.png
--rwxr-xr-x   0        0        0   126563 2022-03-07 00:43:14.047859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/mnist-784-euclidean.png
--rwxr-xr-x   0        0        0   192595 2022-03-07 00:43:14.047859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/nytimes-256-angular.png
--rwxr-xr-x   0        0        0   231693 2022-03-07 00:43:14.051859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/sift-128-euclidean.png
--rw-r--r--   0        0        0      299 2022-03-07 00:43:31.995887 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/run.py
--rw-r--r--   0        0        0       71 2022-03-07 00:43:14.051859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/run_algorithm.py
--rw-r--r--   0        0        0     4616 2022-03-07 00:43:14.051859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/chartjs.template
--rw-r--r--   0        0        0      799 2022-03-07 00:43:14.051859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/detail_page.html
--rw-r--r--   0        0        0     3096 2022-03-07 00:43:14.051859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/general.html
--rw-r--r--   0        0        0      891 2022-03-07 00:43:14.051859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/latex.template
--rw-r--r--   0        0        0     3517 2022-03-07 00:43:14.051859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/summary.html
--rw-r--r--   0        0        0        0 2022-03-07 00:43:14.051859 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/test/__init__.py
--rw-r--r--   0        0        0      462 2022-03-08 16:11:29.733446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/test/test-jaccard.py
--rw-r--r--   0        0        0     3057 2022-03-08 16:11:29.733446 redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/test/test-metrics.py
--rw-r--r--   0        0        0     6306 2022-06-16 09:53:47.185531 redisbench-admin-0.9.8/redisbench_admin/run/args.py
--rw-r--r--   0        0        0     6072 2022-06-17 08:59:48.822442 redisbench-admin-0.9.8/redisbench_admin/run/cluster.py
--rw-r--r--   0        0        0    23360 2022-05-09 10:42:15.148934 redisbench-admin-0.9.8/redisbench_admin/run/common.py
--rw-r--r--   0        0        0      101 2021-08-03 19:12:36.062986 redisbench-admin-0.9.8/redisbench_admin/run/ftsb/__init__.py
--rw-r--r--   0        0        0     2247 2021-08-05 08:38:27.814458 redisbench-admin-0.9.8/redisbench_admin/run/ftsb/ftsb.py
--rw-r--r--   0        0        0     3064 2021-09-18 07:47:53.009595 redisbench-admin-0.9.8/redisbench_admin/run/git.py
--rw-r--r--   0        0        0     6655 2022-06-15 14:54:00.641499 redisbench-admin-0.9.8/redisbench_admin/run/grafana.py
--rw-r--r--   0        0        0      101 2021-10-19 07:50:12.437772 redisbench-admin-0.9.8/redisbench_admin/run/memtier_benchmark/__init__.py
--rw-r--r--   0        0        0     4135 2022-03-16 10:30:20.356293 redisbench-admin-0.9.8/redisbench_admin/run/memtier_benchmark/memtier_benchmark.py
--rw-r--r--   0        0        0     7289 2022-03-23 07:37:28.445828 redisbench-admin-0.9.8/redisbench_admin/run/metrics.py
--rw-r--r--   0        0        0     1024 2022-05-09 10:42:15.148934 redisbench-admin-0.9.8/redisbench_admin/run/modules.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.136690 redisbench-admin-0.9.8/redisbench_admin/run/redis_benchmark/__init__.py
--rw-r--r--   0        0        0     6848 2021-12-28 11:19:25.886003 redisbench-admin-0.9.8/redisbench_admin/run/redis_benchmark/redis_benchmark.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.136690 redisbench-admin-0.9.8/redisbench_admin/run/redisgraph_benchmark_go/__init__.py
--rw-r--r--   0        0        0     2241 2021-07-29 17:33:12.809543 redisbench-admin-0.9.8/redisbench_admin/run/redisgraph_benchmark_go/redisgraph_benchmark_go.py
--rw-r--r--   0        0        0    19575 2022-06-15 14:54:00.641499 redisbench-admin-0.9.8/redisbench_admin/run/redistimeseries.py
--rw-r--r--   0        0        0     3046 2022-01-07 13:25:54.277123 redisbench-admin-0.9.8/redisbench_admin/run/run.py
--rw-r--r--   0        0        0      442 2021-07-14 10:11:59.928250 redisbench-admin-0.9.8/redisbench_admin/run/s3.py
--rw-r--r--   0        0        0     2588 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/run/ssh.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.140690 redisbench-admin-0.9.8/redisbench_admin/run/tsbs_run_queries_redistimeseries/__init__.py
--rw-r--r--   0        0        0     2335 2021-09-17 16:16:20.888022 redisbench-admin-0.9.8/redisbench_admin/run/tsbs_run_queries_redistimeseries/tsbs_run_queries_redistimeseries.py
--rw-r--r--   0        0        0        0 2021-04-14 17:04:16.494052 redisbench-admin-0.9.8/redisbench_admin/run/ycsb/__init__.py
--rw-r--r--   0        0        0     3864 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/run/ycsb/ycsb.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.140690 redisbench-admin-0.9.8/redisbench_admin/run_local/__init__.py
--rw-r--r--   0        0        0      438 2022-04-11 15:12:08.689465 redisbench-admin-0.9.8/redisbench_admin/run_local/args.py
--rw-r--r--   0        0        0      124 2021-09-17 16:16:20.888022 redisbench-admin-0.9.8/redisbench_admin/run_local/local_client.py
--rw-r--r--   0        0        0     5691 2022-06-17 08:59:48.762443 redisbench-admin-0.9.8/redisbench_admin/run_local/local_db.py
--rw-r--r--   0        0        0     7026 2022-03-16 10:30:20.356293 redisbench-admin-0.9.8/redisbench_admin/run_local/local_helpers.py
--rw-r--r--   0        0        0    20889 2022-05-09 10:42:15.148934 redisbench-admin-0.9.8/redisbench_admin/run_local/run_local.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.140690 redisbench-admin-0.9.8/redisbench_admin/run_remote/__init__.py
--rw-r--r--   0        0        0     2121 2022-05-16 12:26:06.805205 redisbench-admin-0.9.8/redisbench_admin/run_remote/args.py
--rw-r--r--   0        0        0      386 2022-03-16 10:30:20.356293 redisbench-admin-0.9.8/redisbench_admin/run_remote/consts.py
--rw-r--r--   0        0        0       95 2021-09-17 16:16:20.892022 redisbench-admin-0.9.8/redisbench_admin/run_remote/log.py
--rw-r--r--   0        0        0     1190 2022-05-09 10:42:15.148934 redisbench-admin-0.9.8/redisbench_admin/run_remote/notifications.py
--rw-r--r--   0        0        0    13265 2022-03-31 14:40:15.402165 redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_client.py
--rw-r--r--   0        0        0    11664 2022-06-17 08:59:48.870441 redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_db.py
--rw-r--r--   0        0        0     2143 2022-06-17 08:53:37.526487 redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_env.py
--rw-r--r--   0        0        0     1567 2022-03-16 10:30:20.356293 redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_failures.py
--rw-r--r--   0        0        0     8896 2022-06-15 15:01:22.532214 redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_helpers.py
--rw-r--r--   0        0        0    56308 2022-05-16 12:26:06.809205 redisbench-admin-0.9.8/redisbench_admin/run_remote/run_remote.py
--rw-r--r--   0        0        0     4448 2022-06-18 15:49:51.377540 redisbench-admin-0.9.8/redisbench_admin/run_remote/standalone.py
--rw-r--r--   0        0        0     3944 2022-05-16 12:26:06.809205 redisbench-admin-0.9.8/redisbench_admin/run_remote/terraform.py
--rw-r--r--   0        0        0      101 2021-06-15 16:29:11.140690 redisbench-admin-0.9.8/redisbench_admin/utils/__init__.py
--rw-r--r--   0        0        0    19198 2022-03-16 10:30:20.356293 redisbench-admin-0.9.8/redisbench_admin/utils/benchmark_config.py
--rw-r--r--   0        0        0     3890 2022-03-16 10:30:20.356293 redisbench-admin-0.9.8/redisbench_admin/utils/local.py
--rw-r--r--   0        0        0     1602 2021-06-15 16:29:11.144690 redisbench-admin-0.9.8/redisbench_admin/utils/redisearch.py
--rw-r--r--   0        0        0     2048 2022-03-16 10:30:20.356293 redisbench-admin-0.9.8/redisbench_admin/utils/redisgraph_benchmark_go.py
--rw-r--r--   0        0        0    36693 2022-05-16 12:26:06.809205 redisbench-admin-0.9.8/redisbench_admin/utils/remote.py
--rw-r--r--   0        0        0     3267 2021-07-23 16:27:00.004172 redisbench-admin-0.9.8/redisbench_admin/utils/results.py
--rw-r--r--   0        0        0     6533 2021-06-16 17:00:41.502772 redisbench-admin-0.9.8/redisbench_admin/utils/ssh.py
--rw-r--r--   0        0        0    12382 2022-06-18 17:29:04.612079 redisbench-admin-0.9.8/redisbench_admin/utils/utils.py
--rw-r--r--   0        0        0       95 2021-06-15 16:29:11.144690 redisbench-admin-0.9.8/redisbench_admin/watchdog/__init__.py
--rw-r--r--   0        0        0     1312 2021-06-23 17:00:17.301509 redisbench-admin-0.9.8/redisbench_admin/watchdog/args.py
--rw-r--r--   0        0        0     6043 2022-05-09 10:42:15.148934 redisbench-admin-0.9.8/redisbench_admin/watchdog/watchdog.py
--rw-r--r--   0        0        0     7072 2022-06-18 17:32:59.972762 redisbench-admin-0.9.8/setup.py
--rw-r--r--   0        0        0     5530 2022-06-18 17:32:59.973284 redisbench-admin-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    10768 2022-07-10 18:57:02.185816 redisbench-admin-0.9.9/LICENSE
+-rw-r--r--   0        0        0     3559 2022-07-10 18:57:02.185816 redisbench-admin-0.9.9/README.md
+-rw-r--r--   0        0        0     1544 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      473 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/__init__.py
+-rw-r--r--   0        0        0     7518 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/cli.py
+-rw-r--r--   0        0        0       95 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/commands/__init__.py
+-rw-r--r--   0        0        0       95 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/commands/commands.json.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/compare/__init__.py
+-rw-r--r--   0        0        0     3871 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/compare/args.py
+-rw-r--r--   0        0        0    15252 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/compare/compare.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/deploy/__init__.py
+-rw-r--r--   0        0        0     1732 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/deploy/args.py
+-rw-r--r--   0        0        0     3791 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/deploy/deploy.py
+-rw-r--r--   0        0        0       95 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/environments/__init__.py
+-rw-r--r--   0        0        0     6681 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/environments/oss_cluster.py
+-rw-r--r--   0        0        0     2474 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/environments/oss_standalone.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/__init__.py
+-rw-r--r--   0        0        0     3171 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/args.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/common/__init__.py
+-rw-r--r--   0        0        0     4331 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/common/common.py
+-rw-r--r--   0        0        0     9524 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/export.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/memtier_benchmark/__init__.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/memtier_benchmark/memtier_benchmark_json_format.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/pyperf/__init__.py
+-rw-r--r--   0        0        0     1678 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/pyperf/pyperf_json_format.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/redis_benchmark/__init__.py
+-rw-r--r--   0        0        0     2522 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/redis_benchmark/metrics_definition.py
+-rw-r--r--   0        0        0     5780 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/export/redis_benchmark/redis_benchmark_csv_format.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/extract/__init__.py
+-rw-r--r--   0        0        0     1073 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/extract/args.py
+-rw-r--r--   0        0        0      770 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/extract/extract.py
+-rw-r--r--   0        0        0        0 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/grafana_api/__init__.py
+-rw-r--r--   0        0        0     3416 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/grafana_api/app.py
+-rw-r--r--   0        0        0     1212 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/grafana_api/args.py
+-rw-r--r--   0        0        0     1613 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/grafana_api/grafana_api.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/__init__.py
+-rw-r--r--   0        0        0    12974 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/daemon.py
+-rwxr-xr-x   0        0        0    35898 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/flamegraph.pl
+-rw-r--r--   0        0        0    27756 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/perf.py
+-rw-r--r--   0        0        0     4949 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/perf_daemon_caller.py
+-rw-r--r--   0        0        0     3949 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/pprof.py
+-rw-r--r--   0        0        0      510 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/profilers.py
+-rw-r--r--   0        0        0    11971 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/profilers_local.py
+-rw-r--r--   0        0        0     2744 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/profilers_schema.py
+-rwxr-xr-x   0        0        0    10307 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/stackcollapse-perf.pl
+-rw-r--r--   0        0        0     4618 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/profilers/vtune.py
+-rw-r--r--   0        0        0      920 2022-07-10 18:57:02.197817 redisbench-admin-0.9.9/redisbench_admin/results/glove-100-angular/10/redisearch-hnsw/build_stats.hdf5
+-rw-r--r--   0        0        0 18876448 2022-07-10 18:57:02.245819 redisbench-admin-0.9.9/redisbench_admin/results/mnist-784-euclidean/10/redisearch-hnsw/build_stats.hdf5
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.245819 redisbench-admin-0.9.9/redisbench_admin/run/__init__.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.245819 redisbench-admin-0.9.9/redisbench_admin/run/aibench_run_inference_redisai_vision/__init__.py
+-rw-r--r--   0        0        0     1829 2022-07-10 18:57:02.245819 redisbench-admin-0.9.9/redisbench_admin/run/aibench_run_inference_redisai_vision/aibench_run_inference_redisai_vision.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.245819 redisbench-admin-0.9.9/redisbench_admin/run/ann/__init__.py
+-rw-r--r--   0        0        0     1288 2022-07-10 18:57:02.245819 redisbench-admin-0.9.9/redisbench_admin/run/ann/ann.py
+-rw-r--r--   0        0        0       13 2022-07-10 18:57:13.929645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/.dockerignore
+-rw-r--r--   0        0        0       62 2022-07-10 18:57:13.921646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/.git
+-rw-r--r--   0        0        0     3361 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/.github/workflows/benchmarks.yml
+-rw-r--r--   0        0        0      158 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/.gitignore
+-rw-r--r--   0        0        0     1074 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/LICENSE
+-rw-r--r--   0        0        0    10452 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/README.md
+-rw-r--r--   0        0        0    49113 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/algos.yaml
+-rw-r--r--   0        0        0     2316 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/algosP.yaml
+-rw-r--r--   0        0        0       75 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/__init__.py
+-rw-r--r--   0        0        0      819 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/annoy.py
+-rw-r--r--   0        0        0      765 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/balltree.py
+-rw-r--r--   0        0        0     1013 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/base.py
+-rw-r--r--   0        0        0     4659 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/bruteforce.py
+-rw-r--r--   0        0        0      502 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/ckdtree.py
+-rw-r--r--   0        0        0     1021 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/datasketch.py
+-rw-r--r--   0        0        0     6746 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/definitions.py
+-rw-r--r--   0        0        0     7665 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/diskann.py
+-rw-r--r--   0        0        0      951 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/dolphinnpy.py
+-rw-r--r--   0        0        0      584 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/dummy_algo.py
+-rw-r--r--   0        0        0     3874 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/elasticsearch.py
+-rw-r--r--   0        0        0     4482 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/elastiknn.py
+-rw-r--r--   0        0        0     3992 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss.py
+-rw-r--r--   0        0        0     2018 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss_gpu.py
+-rw-r--r--   0        0        0     1175 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss_hnsw.py
+-rw-r--r--   0        0        0      950 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/flann.py
+-rw-r--r--   0        0        0     1277 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/hnswlib.py
+-rw-r--r--   0        0        0      759 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/kdtree.py
+-rw-r--r--   0        0        0     1280 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/kgraph.py
+-rw-r--r--   0        0        0      972 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/lshf.py
+-rw-r--r--   0        0        0     3836 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/milvus.py
+-rw-r--r--   0        0        0     1495 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/mrpt.py
+-rw-r--r--   0        0        0      919 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/n2.py
+-rw-r--r--   0        0        0     1739 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/nearpy.py
+-rw-r--r--   0        0        0     2936 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/nmslib.py
+-rw-r--r--   0        0        0     4421 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/onng_ngt.py
+-rw-r--r--   0        0        0     3622 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/opensearchknn.py
+-rw-r--r--   0        0        0     2971 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/panng_ngt.py
+-rw-r--r--   0        0        0     1609 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/pinecone.py
+-rw-r--r--   0        0        0     1669 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/puffinn.py
+-rw-r--r--   0        0        0     3995 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/pynndescent.py
+-rw-r--r--   0        0        0     4380 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/qg_ngt.py
+-rw-r--r--   0        0        0     4061 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/redisearch.py
+-rw-r--r--   0        0        0      642 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/rpforest.py
+-rw-r--r--   0        0        0     1249 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/scann.py
+-rw-r--r--   0        0        0      928 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/sptag.py
+-rw-r--r--   0        0        0     7629 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/subprocess.py
+-rw-r--r--   0        0        0     4807 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/vald.py
+-rw-r--r--   0        0        0     2049 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/vespa.py
+-rw-r--r--   0        0        0       22 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/constants.py
+-rw-r--r--   0        0        0     1130 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/data.py
+-rw-r--r--   0        0        0    24462 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/datasets.py
+-rw-r--r--   0        0        0     1679 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/distance.py
+-rw-r--r--   0        0        0    11671 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/main.py
+-rw-r--r--   0        0        0       77 2022-07-10 18:57:13.933645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/__init__.py
+-rw-r--r--   0        0        0     6971 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/metrics.py
+-rw-r--r--   0        0        0      617 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/plot_variants.py
+-rw-r--r--   0        0        0     5593 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/utils.py
+-rw-r--r--   0        0        0     2497 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/results.py
+-rw-r--r--   0        0        0    13075 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/runner.py
+-rw-r--r--   0        0        0      346 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/create_dataset.py
+-rw-r--r--   0        0        0     6646 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/create_hybrid_dataset.py
+-rw-r--r--   0        0        0     4639 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/create_text_to_image_ds.py
+-rw-r--r--   0        0        0     9582 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/create_website.py
+-rw-r--r--   0        0        0      293 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile
+-rw-r--r--   0        0        0      139 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.annoy
+-rw-r--r--   0        0        0       84 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.datasketch
+-rw-r--r--   0        0        0     1728 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.diskann
+-rw-r--r--   0        0        0     1930 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.diskann_pq
+-rw-r--r--   0        0        0      152 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.dolphinn
+-rw-r--r--   0        0        0     1518 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.elasticsearch
+-rw-r--r--   0        0        0     2242 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.elastiknn
+-rw-r--r--   0        0        0      549 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.faiss
+-rw-r--r--   0        0        0      316 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.flann
+-rw-r--r--   0        0        0      283 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.hnswlib
+-rw-r--r--   0        0        0      318 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.kgraph
+-rw-r--r--   0        0        0      186 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.mih
+-rw-r--r--   0        0        0     1213 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.milvus
+-rw-r--r--   0        0        0      100 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.mrpt
+-rw-r--r--   0        0        0       92 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.n2
+-rw-r--r--   0        0        0      148 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.nearpy
+-rw-r--r--   0        0        0      413 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.ngt
+-rw-r--r--   0        0        0      443 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.nmslib
+-rw-r--r--   0        0        0     1719 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.opensearchknn
+-rw-r--r--   0        0        0      171 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.puffinn
+-rw-r--r--   0        0        0      105 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.pynndescent
+-rw-r--r--   0        0        0      582 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.redisearch
+-rw-r--r--   0        0        0      145 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.rpforest
+-rw-r--r--   0        0        0      105 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.scann
+-rw-r--r--   0        0        0       74 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.scipy
+-rw-r--r--   0        0        0       83 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.sklearn
+-rw-r--r--   0        0        0     1191 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.sptag
+-rw-r--r--   0        0        0      227 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.vald
+-rw-r--r--   0        0        0      730 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.vespa
+-rw-r--r--   0        0        0     2105 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install.py
+-rw-r--r--   0        0        0      541 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/logging.conf
+-rw-r--r--   0        0        0    10150 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/multirun.py
+-rw-r--r--   0        0        0     5845 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/plot.py
+-rwxr-xr-x   0        0        0      207 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/bf-runner
+-rw-r--r--   0        0        0     6616 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/bf-runner.py
+-rw-r--r--   0        0        0     2638 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/ext-add-query-metric.md
+-rw-r--r--   0        0        0     2464 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/ext-batch-queries.md
+-rw-r--r--   0        0        0     2988 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/ext-prepared-queries.md
+-rw-r--r--   0        0        0     1856 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/ext-query-parameters.md
+-rw-r--r--   0        0        0     7539 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/specification.md
+-rw-r--r--   0        0        0      203 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/requirements.txt
+-rw-r--r--   0        0        0      158 2022-07-10 18:57:13.937645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/requirements_py38.txt
+-rwxr-xr-x   0        0        0   215273 2022-07-10 18:57:13.941645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/fashion-mnist-784-euclidean.png
+-rwxr-xr-x   0        0        0   122473 2022-07-10 18:57:13.941645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/gist-960-euclidean.png
+-rwxr-xr-x   0        0        0   224400 2022-07-10 18:57:13.941645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/glove-100-angular.png
+-rwxr-xr-x   0        0        0   226384 2022-07-10 18:57:13.945645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/glove-25-angular.png
+-rw-r--r--   0        0        0   235553 2022-07-10 18:57:13.945645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/lastfm-64-dot.png
+-rwxr-xr-x   0        0        0   126563 2022-07-10 18:57:13.945645 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/mnist-784-euclidean.png
+-rwxr-xr-x   0        0        0   192595 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/nytimes-256-angular.png
+-rwxr-xr-x   0        0        0   231693 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/sift-128-euclidean.png
+-rw-r--r--   0        0        0      299 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/run.py
+-rw-r--r--   0        0        0       71 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/run_algorithm.py
+-rw-r--r--   0        0        0     4616 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/chartjs.template
+-rw-r--r--   0        0        0      799 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/detail_page.html
+-rw-r--r--   0        0        0     3096 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/general.html
+-rw-r--r--   0        0        0      891 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/latex.template
+-rw-r--r--   0        0        0     3517 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/summary.html
+-rw-r--r--   0        0        0        0 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/test/__init__.py
+-rw-r--r--   0        0        0      462 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/test/test-jaccard.py
+-rw-r--r--   0        0        0     3057 2022-07-10 18:57:13.949646 redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/test/test-metrics.py
+-rw-r--r--   0        0        0     6306 2022-07-10 18:57:02.245819 redisbench-admin-0.9.9/redisbench_admin/run/args.py
+-rw-r--r--   0        0        0     6072 2022-07-10 18:57:02.245819 redisbench-admin-0.9.9/redisbench_admin/run/cluster.py
+-rw-r--r--   0        0        0    23360 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/common.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/ftsb/__init__.py
+-rw-r--r--   0        0        0     2247 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/ftsb/ftsb.py
+-rw-r--r--   0        0        0     3064 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/git.py
+-rw-r--r--   0        0        0     6655 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/grafana.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/memtier_benchmark/__init__.py
+-rw-r--r--   0        0        0     4135 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/memtier_benchmark/memtier_benchmark.py
+-rw-r--r--   0        0        0     7289 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/metrics.py
+-rw-r--r--   0        0        0     1024 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/modules.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/redis_benchmark/__init__.py
+-rw-r--r--   0        0        0     6848 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/redis_benchmark/redis_benchmark.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/redisgraph_benchmark_go/__init__.py
+-rw-r--r--   0        0        0     2241 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/redisgraph_benchmark_go/redisgraph_benchmark_go.py
+-rw-r--r--   0        0        0    19575 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/redistimeseries.py
+-rw-r--r--   0        0        0     3046 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/run.py
+-rw-r--r--   0        0        0      442 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/s3.py
+-rw-r--r--   0        0        0     2588 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/ssh.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/tsbs_run_queries_redistimeseries/__init__.py
+-rw-r--r--   0        0        0     2335 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/tsbs_run_queries_redistimeseries/tsbs_run_queries_redistimeseries.py
+-rw-r--r--   0        0        0        0 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/ycsb/__init__.py
+-rw-r--r--   0        0        0     3864 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run/ycsb/ycsb.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_local/__init__.py
+-rw-r--r--   0        0        0      438 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_local/args.py
+-rw-r--r--   0        0        0      124 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_local/local_client.py
+-rw-r--r--   0        0        0     5758 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_local/local_db.py
+-rw-r--r--   0        0        0     7026 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_local/local_helpers.py
+-rw-r--r--   0        0        0    20889 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_local/run_local.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/__init__.py
+-rw-r--r--   0        0        0     2121 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/args.py
+-rw-r--r--   0        0        0      386 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/consts.py
+-rw-r--r--   0        0        0       95 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/log.py
+-rw-r--r--   0        0        0     1190 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/notifications.py
+-rw-r--r--   0        0        0    13265 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_client.py
+-rw-r--r--   0        0        0    11664 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_db.py
+-rw-r--r--   0        0        0     2143 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_env.py
+-rw-r--r--   0        0        0     1567 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_failures.py
+-rw-r--r--   0        0        0     8896 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_helpers.py
+-rw-r--r--   0        0        0    56308 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/run_remote.py
+-rw-r--r--   0        0        0     4448 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/standalone.py
+-rw-r--r--   0        0        0     3944 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/run_remote/terraform.py
+-rw-r--r--   0        0        0      101 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/__init__.py
+-rw-r--r--   0        0        0    19198 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/benchmark_config.py
+-rw-r--r--   0        0        0     3890 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/local.py
+-rw-r--r--   0        0        0     1602 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/redisearch.py
+-rw-r--r--   0        0        0     2048 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/redisgraph_benchmark_go.py
+-rw-r--r--   0        0        0    36693 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/remote.py
+-rw-r--r--   0        0        0     3267 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/results.py
+-rw-r--r--   0        0        0     6533 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/ssh.py
+-rw-r--r--   0        0        0    12382 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/utils/utils.py
+-rw-r--r--   0        0        0       95 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/watchdog/__init__.py
+-rw-r--r--   0        0        0     1312 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/watchdog/args.py
+-rw-r--r--   0        0        0     6043 2022-07-10 18:57:02.249820 redisbench-admin-0.9.9/redisbench_admin/watchdog/watchdog.py
+-rw-r--r--   0        0        0     7072 2022-07-10 18:58:52.548795 redisbench-admin-0.9.9/setup.py
+-rw-r--r--   0        0        0     5581 2022-07-10 18:58:52.549661 redisbench-admin-0.9.9/PKG-INFO
```

### Comparing `redisbench-admin-0.9.8/LICENSE` & `redisbench-admin-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/README.md` & `redisbench-admin-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/pyproject.toml` & `redisbench-admin-0.9.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redisbench-admin"
-version = "0.9.8"
+version = "0.9.9"
 description = "Redis benchmark run helper. A wrapper around Redis and Redis Modules benchmark tools ( ftsb_redisearch, memtier_benchmark, redis-benchmark, aibench, etc... )."
 authors = ["filipecosta90 <filipecosta.90@gmail.com>","Redis Performance Group <performance@redis.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 redisbench-admin = "redisbench_admin.cli:main"
 perf-daemon = "redisbench_admin.profilers.daemon:main"
```

### Comparing `redisbench-admin-0.9.8/redisbench_admin/cli.py` & `redisbench-admin-0.9.9/redisbench_admin/cli.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/compare/args.py` & `redisbench-admin-0.9.9/redisbench_admin/compare/args.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/compare/compare.py` & `redisbench-admin-0.9.9/redisbench_admin/compare/compare.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/deploy/args.py` & `redisbench-admin-0.9.9/redisbench_admin/deploy/args.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/deploy/deploy.py` & `redisbench-admin-0.9.9/redisbench_admin/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/environments/oss_cluster.py` & `redisbench-admin-0.9.9/redisbench_admin/environments/oss_cluster.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/environments/oss_standalone.py` & `redisbench-admin-0.9.9/redisbench_admin/environments/oss_standalone.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/export/args.py` & `redisbench-admin-0.9.9/redisbench_admin/export/args.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/export/common/common.py` & `redisbench-admin-0.9.9/redisbench_admin/export/common/common.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/export/export.py` & `redisbench-admin-0.9.9/redisbench_admin/export/export.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/export/pyperf/pyperf_json_format.py` & `redisbench-admin-0.9.9/redisbench_admin/export/pyperf/pyperf_json_format.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/export/redis_benchmark/metrics_definition.py` & `redisbench-admin-0.9.9/redisbench_admin/export/redis_benchmark/metrics_definition.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/export/redis_benchmark/redis_benchmark_csv_format.py` & `redisbench-admin-0.9.9/redisbench_admin/export/redis_benchmark/redis_benchmark_csv_format.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/extract/args.py` & `redisbench-admin-0.9.9/redisbench_admin/extract/args.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/extract/extract.py` & `redisbench-admin-0.9.9/redisbench_admin/extract/extract.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/grafana_api/app.py` & `redisbench-admin-0.9.9/redisbench_admin/grafana_api/app.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/grafana_api/args.py` & `redisbench-admin-0.9.9/redisbench_admin/grafana_api/args.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/grafana_api/grafana_api.py` & `redisbench-admin-0.9.9/redisbench_admin/grafana_api/grafana_api.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/daemon.py` & `redisbench-admin-0.9.9/redisbench_admin/profilers/daemon.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/flamegraph.pl` & `redisbench-admin-0.9.9/redisbench_admin/profilers/flamegraph.pl`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/perf.py` & `redisbench-admin-0.9.9/redisbench_admin/profilers/perf.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/perf_daemon_caller.py` & `redisbench-admin-0.9.9/redisbench_admin/profilers/perf_daemon_caller.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/pprof.py` & `redisbench-admin-0.9.9/redisbench_admin/profilers/pprof.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/profilers_local.py` & `redisbench-admin-0.9.9/redisbench_admin/profilers/profilers_local.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/profilers_schema.py` & `redisbench-admin-0.9.9/redisbench_admin/profilers/profilers_schema.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/stackcollapse-perf.pl` & `redisbench-admin-0.9.9/redisbench_admin/profilers/stackcollapse-perf.pl`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/profilers/vtune.py` & `redisbench-admin-0.9.9/redisbench_admin/profilers/vtune.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/results/glove-100-angular/10/redisearch-hnsw/build_stats.hdf5` & `redisbench-admin-0.9.9/redisbench_admin/results/glove-100-angular/10/redisearch-hnsw/build_stats.hdf5`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/results/mnist-784-euclidean/10/redisearch-hnsw/build_stats.hdf5` & `redisbench-admin-0.9.9/redisbench_admin/results/mnist-784-euclidean/10/redisearch-hnsw/build_stats.hdf5`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/aibench_run_inference_redisai_vision/aibench_run_inference_redisai_vision.py` & `redisbench-admin-0.9.9/redisbench_admin/run/aibench_run_inference_redisai_vision/aibench_run_inference_redisai_vision.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/ann.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/ann.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/.github/workflows/benchmarks.yml` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/LICENSE` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/LICENSE`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/README.md` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/README.md`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/algos.yaml` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/algos.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,24 @@
       module: ann_benchmarks.algorithms.redisearch
       constructor: RediSearch
       base-args: ["FLAT", "@metric", "@connection"]
       run-groups:
         BS-2^20:
           arg-groups:
             - {"BLOCK_SIZE": 1048576}
+    pinecone:
+      docker-tag: ann-benchmarks-pinecone
+      module: ann_benchmarks.algorithms.pinecone
+      constructor: Pinecone
+      base-args: ["@metric", "@dimension", "@connection"]
+      run-groups:
+        approximated:
+          args: [['approximated']]
+        exact:
+          args: [['exact']]
     sptag:
       docker-tag: ann-benchmarks-sptag
       module: ann_benchmarks.algorithms.sptag
       constructor: Sptag
       base-args: ["@metric"]
       run-groups:
         sptag:
```

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/algosP.yaml` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/algosP.yaml`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/annoy.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/annoy.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/balltree.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/balltree.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/base.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/bruteforce.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/bruteforce.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/datasketch.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/datasketch.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/definitions.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/definitions.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/diskann.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/diskann.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/dolphinnpy.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/dolphinnpy.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/dummy_algo.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/dummy_algo.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/elasticsearch.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/elastiknn.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/elastiknn.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss_gpu.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss_gpu.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss_hnsw.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/faiss_hnsw.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/flann.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/flann.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/hnswlib.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/hnswlib.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/kdtree.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/kdtree.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/kgraph.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/kgraph.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/lshf.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/lshf.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/milvus.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/milvus.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/mrpt.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/mrpt.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/n2.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/n2.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/nearpy.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/nearpy.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/nmslib.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/nmslib.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/onng_ngt.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/onng_ngt.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/opensearchknn.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/opensearchknn.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/panng_ngt.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/panng_ngt.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/puffinn.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/puffinn.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/pynndescent.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/pynndescent.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/qg_ngt.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/qg_ngt.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/redisearch.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/redisearch.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/rpforest.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/rpforest.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/scann.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/scann.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/sptag.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/sptag.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/subprocess.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/subprocess.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/vald.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/vald.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/vespa.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/algorithms/vespa.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/data.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/data.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/datasets.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/datasets.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/distance.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/distance.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/main.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/main.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/metrics.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/metrics.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/plot_variants.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/plot_variants.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/utils.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/results.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/results.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/ann_benchmarks/runner.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/ann_benchmarks/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,14 +153,22 @@
         # Make sure that algorithms with no query argument groups still get run
         # once by providing them with a single, empty, harmless group
         if not query_argument_groups:
             query_argument_groups = [[]]
 
         if not build_only:
             print('got %d queries' % len(X_test))
+            per_client = len(X_test) // num_clients
+            offset = per_client * (id - 1)
+            if (num_clients != id):
+                X_test = X_test[offset : offset + per_client]
+            else:
+                X_test = X_test[offset:]
+            print('running %d out of them' % len(X_test))
+            
             for pos, query_arguments in enumerate(query_argument_groups, 1):
                 print("Running query argument group %d of %d..." %
                       (pos, len(query_argument_groups)))
                 if query_arguments:
                     algo.set_query_arguments(*query_arguments)
                 if hybrid_buckets:
                     text = hybrid_buckets[D.attrs['selected_bucket']]['text'].decode()
```

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/create_hybrid_dataset.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/create_hybrid_dataset.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/create_text_to_image_ds.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/create_text_to_image_ds.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/create_website.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/create_website.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.diskann` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.diskann`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.diskann_pq` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.diskann_pq`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.elasticsearch` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.elasticsearch`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.elastiknn` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.elastiknn`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.faiss` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.faiss`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.milvus` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.milvus`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.opensearchknn` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.opensearchknn`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.redisearch` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.redisearch`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.sptag` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.sptag`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install/Dockerfile.vespa` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install/Dockerfile.vespa`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/install.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/install.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/logging.conf` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/logging.conf`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/multirun.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/multirun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from multiprocessing import Process
 import argparse
 import time
 import json
 from numpy import average
-from redis import Redis
-from redis.cluster import RedisCluster
-from pymilvus import utility, connections
 import h5py
 import os
 from watchdog.observers import Observer
 from watchdog.events import PatternMatchingEventHandler
 import pathlib
 from ann_benchmarks.results import get_result_filename
 from ann_benchmarks.algorithms.definitions import get_run_groups
 
+from redis import Redis
+from redis.cluster import RedisCluster
+
+from pymilvus import utility, connections
+
+import pinecone
+
 
 def aggregate_outputs(files, clients):
     different_attrs = set([f.split('client')[0] for f in files])
     groups = [[f + f'client_{i}.hdf5' for i in range(1, clients + 1)] for f in different_attrs]
 
     if len(different_attrs) * clients > len(files):
         print(f'missing files! got {len(files)} but expected {len(different_attrs) * clients}')
@@ -149,26 +153,29 @@
     # given some functions bellow require on relative path to the project
     workdir = pathlib.Path(__file__).parent.absolute()
     print("Changing the workdir to {}".format(workdir))
     os.chdir(workdir)
 
     isredis = True if 'redisearch' in args.algorithm else False
     ismilvus = True if 'milvus' in args.algorithm else False
+    ispinecone = True if 'pinecone' in args.algorithm else False
 
     if args.host is None:
         args.host = 'localhost'
     if args.port is None:
         if isredis: args.port = '6379'
         elif ismilvus: args.port = '19530'
 
     if isredis:
         redis = RedisCluster if args.cluster else Redis
         redis = redis(host=args.host, port=int(args.port), password=args.auth, username=args.user)
     elif ismilvus:
         connections.connect(host=args.host, port=args.port)
+    elif ispinecone:
+        pinecone.init(api_key=args.auth)
 
     if args.run_group is not None:
         run_groups = [args.run_group]
     else:
         run_groups = get_run_groups('algos.yaml', args.algorithm)
 
     base = 'python3 run.py --local --algorithm ' + args.algorithm + ' -k ' + args.count + ' --dataset ' + args.dataset
@@ -207,14 +214,17 @@
 
     for run_group in run_groups:
         if isredis:
             redis.flushall()
         elif ismilvus:
             if utility.has_collection('milvus'):
                 utility.drop_collection('milvus')
+        elif ispinecone:
+            for idx in pinecone.list_indexes():
+                pinecone.delete_index(idx)
 
         results_dict = {}
         curr_base_build = base_build + ' --run-group ' + run_group
         curr_base_test = base_test + ' --run-group ' + run_group
 
         if int(args.build_clients) > 0:
             clients = [Process(target=os.system, args=(curr_base_build + ' --client-id ' + str(i),)) for i in
```

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/plot.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/plot.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/bf-runner.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/bf-runner.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/ext-add-query-metric.md` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/ext-add-query-metric.md`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/ext-batch-queries.md` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/ext-batch-queries.md`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/ext-prepared-queries.md` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/ext-prepared-queries.md`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/ext-query-parameters.md` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/ext-query-parameters.md`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/protocol/specification.md` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/protocol/specification.md`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/fashion-mnist-784-euclidean.png` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/fashion-mnist-784-euclidean.png`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/gist-960-euclidean.png` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/gist-960-euclidean.png`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/glove-100-angular.png` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/glove-100-angular.png`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/glove-25-angular.png` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/glove-25-angular.png`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/lastfm-64-dot.png` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/lastfm-64-dot.png`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/mnist-784-euclidean.png` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/mnist-784-euclidean.png`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/nytimes-256-angular.png` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/nytimes-256-angular.png`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/results/sift-128-euclidean.png` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/results/sift-128-euclidean.png`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/chartjs.template` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/chartjs.template`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/detail_page.html` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/detail_page.html`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/general.html` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/general.html`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/latex.template` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/latex.template`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/templates/summary.html` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/templates/summary.html`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ann/pkg/test/test-metrics.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ann/pkg/test/test-metrics.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/args.py` & `redisbench-admin-0.9.9/redisbench_admin/run/args.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/cluster.py` & `redisbench-admin-0.9.9/redisbench_admin/run/cluster.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/common.py` & `redisbench-admin-0.9.9/redisbench_admin/run/common.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ftsb/ftsb.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ftsb/ftsb.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/git.py` & `redisbench-admin-0.9.9/redisbench_admin/run/git.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/grafana.py` & `redisbench-admin-0.9.9/redisbench_admin/run/grafana.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/memtier_benchmark/memtier_benchmark.py` & `redisbench-admin-0.9.9/redisbench_admin/run/memtier_benchmark/memtier_benchmark.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/metrics.py` & `redisbench-admin-0.9.9/redisbench_admin/run/metrics.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/modules.py` & `redisbench-admin-0.9.9/redisbench_admin/run/modules.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/redis_benchmark/redis_benchmark.py` & `redisbench-admin-0.9.9/redisbench_admin/run/redis_benchmark/redis_benchmark.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/redisgraph_benchmark_go/redisgraph_benchmark_go.py` & `redisbench-admin-0.9.9/redisbench_admin/run/redisgraph_benchmark_go/redisgraph_benchmark_go.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/redistimeseries.py` & `redisbench-admin-0.9.9/redisbench_admin/run/redistimeseries.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/run.py` & `redisbench-admin-0.9.9/redisbench_admin/run/run.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ssh.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ssh.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/tsbs_run_queries_redistimeseries/tsbs_run_queries_redistimeseries.py` & `redisbench-admin-0.9.9/redisbench_admin/run/tsbs_run_queries_redistimeseries/tsbs_run_queries_redistimeseries.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run/ycsb/ycsb.py` & `redisbench-admin-0.9.9/redisbench_admin/run/ycsb/ycsb.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_local/local_db.py` & `redisbench-admin-0.9.9/redisbench_admin/run_local/local_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,23 +121,23 @@
             redis_7,
         )
 
         r = redis.Redis(port=args.port)
         r.ping()
         r.client_setname("redisbench-admin-stadalone")
         redis_conns.append(r)
-
-    for shardn, redis_process in enumerate(redis_processes):
-        logging.info(
-            "Checking if shard #{} process with pid={} is alive".format(
-                shardn + 1, redis_process.pid
+    if setup_type == "oss-cluster":
+        for shardn, redis_process in enumerate(redis_processes):
+            logging.info(
+                "Checking if shard #{} process with pid={} is alive".format(
+                    shardn + 1, redis_process.pid
+                )
             )
-        )
-        if is_process_alive(redis_process) is False:
-            raise Exception("Redis process is not alive. Failing test.")
+            if is_process_alive(redis_process) is False:
+                raise Exception("Redis process is not alive. Failing test.")
 
     if setup_type == "oss-cluster":
 
         cluster_init_steps(clusterconfig, redis_conns, local_module_file)
 
     if check_dbconfig_tool_requirement(benchmark_config):
         logging.info("Detected the requirements to load data via client tool")
```

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_local/local_helpers.py` & `redisbench-admin-0.9.9/redisbench_admin/run_local/local_helpers.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_local/run_local.py` & `redisbench-admin-0.9.9/redisbench_admin/run_local/run_local.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/args.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/args.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/notifications.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/notifications.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_client.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_client.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_db.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_db.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_env.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_env.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_failures.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_failures.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/remote_helpers.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/remote_helpers.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/run_remote.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/run_remote.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/standalone.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/standalone.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/run_remote/terraform.py` & `redisbench-admin-0.9.9/redisbench_admin/run_remote/terraform.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/utils/benchmark_config.py` & `redisbench-admin-0.9.9/redisbench_admin/utils/benchmark_config.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/utils/local.py` & `redisbench-admin-0.9.9/redisbench_admin/utils/local.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/utils/redisearch.py` & `redisbench-admin-0.9.9/redisbench_admin/utils/redisearch.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/utils/redisgraph_benchmark_go.py` & `redisbench-admin-0.9.9/redisbench_admin/utils/redisgraph_benchmark_go.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/utils/remote.py` & `redisbench-admin-0.9.9/redisbench_admin/utils/remote.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/utils/results.py` & `redisbench-admin-0.9.9/redisbench_admin/utils/results.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/utils/ssh.py` & `redisbench-admin-0.9.9/redisbench_admin/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/utils/utils.py` & `redisbench-admin-0.9.9/redisbench_admin/utils/utils.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/watchdog/args.py` & `redisbench-admin-0.9.9/redisbench_admin/watchdog/args.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/redisbench_admin/watchdog/watchdog.py` & `redisbench-admin-0.9.9/redisbench_admin/watchdog/watchdog.py`

 * *Files identical despite different names*

### Comparing `redisbench-admin-0.9.8/setup.py` & `redisbench-admin-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 entry_points = \
 {'console_scripts': ['perf-daemon = redisbench_admin.profilers.daemon:main',
                      'redisbench-admin = redisbench_admin.cli:main']}
 
 setup_kwargs = {
     'name': 'redisbench-admin',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Redis benchmark run helper. A wrapper around Redis and Redis Modules benchmark tools ( ftsb_redisearch, memtier_benchmark, redis-benchmark, aibench, etc... ).',
     'long_description': '[![codecov](https://codecov.io/gh/RedisLabsModules/redisbench-admin/branch/master/graph/badge.svg)](https://codecov.io/gh/RedisLabsModules/redisbench-admin)\n![Actions](https://github.com/RedisLabsModules/redisbench-admin/workflows/Run%20Tests/badge.svg?branch=master)\n![Actions](https://badge.fury.io/py/redisbench-admin.svg)\n\n# [redisbench-admin](https://github.com/RedisLabsModules/redisbench-admin)\n\nRedis benchmark run helper can help you with the following tasks:\n\n- Setup abd teardown of benchmarking infrastructure specified\n  on [RedisLabsModules/testing-infrastructure](https://github.com/RedisLabsModules/testing-infrastructure)\n- Setup and teardown of an Redis and Redis Modules DBs for benchmarking\n- Management of benchmark data and specifications across different setups\n- Running benchmarks and recording results\n- Exporting performance results in several formats (CSV, RedisTimeSeries, JSON)\n- Finding on-cpu, off-cpu, io, and threading performance problems by attaching profiling tools/probers ( perf (a.k.a. perf_events), bpf tooling, vtune )\n- **[SOON]** Finding performance problems by attaching telemetry probes\n\nCurrent supported benchmark tools:\n\n- [redis-benchmark](https://github.com/redis/redis)\n- [memtier_benchmark](https://github.com/RedisLabs/memtier_benchmark)\n- [redis-benchmark-go](https://github.com/filipecosta90/redis-benchmark-go)\n- [YCSB](https://github.com/RediSearch/YCSB)\n- [tsbs](https://github.com/RedisTimeSeries/tsbs)\n- [redisgraph-benchmark-go](https://github.com/RedisGraph/redisgraph-benchmark-go)\n- [ftsb_redisearch](https://github.com/RediSearch/ftsb)\n- [ann-benchmarks](https://github.com/RedisAI/ann-benchmarks)\n- [SOON][aibench](https://github.com/RedisAI/aibench)\n\n## Installation\n\nInstallation is done using pip, the package installer for Python, in the following manner:\n\n```bash\npython3 -m pip install https://codeload.github.com/redis/redis-py/zip/refs/tags/v4.2.0rc3\npython3 -m pip install redisbench-admin\n```\n\n## Profiler daemon\n\nYou can use the profiler daemon by itself in the following manner. \nOn the target machine do as follow:\n\n```bash\npip3 install --upgrade pip\npip3 install redisbench-admin --ignore-installed PyYAML\n\n# install perf\napt install linux-tools-common linux-tools-generic linux-tools-`uname -r` -y\n\n# ensure perf is working\nperf --version\n\n# install awscli\nsnap install aws-cli --classic\n\n\n# configure aws\naws configure\n\n# start the perf-daemon\nperf-daemon start\nWARNING:root:Unable to detected github_actor. caught the following error: No section: \'user\'\nWritting log to /tmp/perf-daemon.log\nStarting perf-daemon. PID file /tmp/perfdaemon.pid. Daemon workdir: /root/RedisGraph\n\n# check daemon is working appropriatelly\ncurl localhost:5000/ping\n\n# start a profile\ncurl -X POST localhost:5000/profiler/perf/start/<pid to profile>\n\n# stop a profile\ncurl -X POST -d \'{"aws_access_key_id":$AWS_ACCESS_KEY_ID,"aws_secret_access_key":$AWS_SECRET_ACCESS_KEY}\' localhost:5000/profiler/perf/stop/<pid to profile>\n```\n\n\n## Development\n\n1. Install [pypoetry](https://python-poetry.org/) to manage your dependencies and trigger tooling.\n```sh\npip install poetry\n```\n\n2. Installing dependencies from lock file\n\n```\npoetry install\n```\n\n### Running formaters\n\n```sh\npoetry run black .\n```\n\n\n### Running linters\n\n```sh\npoetry run flake8\n```\n\n\n### Running tests\n\nA test suite is provided, and can be run with:\n\n```sh\n$ tox\n```\n\nTo run a specific test:\n```sh\n$ tox -- tests/test_redistimeseries.py\n```\n\n## License\n\nredisbench-admin is distributed under the BSD3 license - see [LICENSE](LICENSE)\n',
     'author': 'filipecosta90',
     'author_email': 'filipecosta.90@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `redisbench-admin-0.9.8/PKG-INFO` & `redisbench-admin-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: redisbench-admin
-Version: 0.9.8
+Version: 0.9.9
 Summary: Redis benchmark run helper. A wrapper around Redis and Redis Modules benchmark tools ( ftsb_redisearch, memtier_benchmark, redis-benchmark, aibench, etc... ).
 Author: filipecosta90
 Author-email: filipecosta.90@gmail.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask (>=2.0.1,<3.0.0)
 Requires-Dist: Flask-HTTPAuth (>=4.4.0,<5.0.0)
 Requires-Dist: GitPython (>=3.1.12,<4.0.0)
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
```

