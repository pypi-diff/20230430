# Comparing `tmp/chaos_mesh-1.2.8.tar.gz` & `tmp/chaos_mesh-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaos_mesh-1.2.8.tar", last modified: Thu Feb 23 03:13:51 2023, max compression
+gzip compressed data, was "dist/chaos_mesh-1.2.9.tar", last modified: Fri Feb 24 05:30:03 2023, max compression
```

## Comparing `chaos_mesh-1.2.8.tar` & `chaos_mesh-1.2.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.476605 chaos_mesh-1.2.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5224 2023-02-23 03:13:51.476605 chaos_mesh-1.2.8/PKG-INFO
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaos_mesh.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5224 2023-02-23 03:13:51.000000 chaos_mesh-1.2.8/chaos_mesh.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3036 2023-02-23 03:13:51.000000 chaos_mesh-1.2.8/chaos_mesh.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-23 03:13:51.000000 chaos_mesh-1.2.8/chaos_mesh.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-23 03:13:51.000000 chaos_mesh-1.2.8/chaos_mesh.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-02-23 03:13:51.000000 chaos_mesh-1.2.8/chaos_mesh.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-02-23 03:13:51.000000 chaos_mesh-1.2.8/chaos_mesh.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3254 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1709 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/base/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2242 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2399 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/fill.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1473 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/read_payload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1612 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/write_payload.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/networkattack/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/networkattack/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/stress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2072 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/stress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2855 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/stress/cpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1883 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/stress/memory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/jvmfault/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3014 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/jvmfault/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2088 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/jvmfault/gc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3175 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/jvmfault/raise_exception.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.468605 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/network/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2068 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/network/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3876 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/network/bandwidth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2193 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/network/partition.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2527 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2125 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/container_kill.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      914 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/pod_failure.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      893 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/pod_kill.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/stress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      562 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/stress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2549 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/stress/cpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2160 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/stress/memory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4438 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/factory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/disk/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/disk/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      477 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/disk/fill.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      710 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/disk/read_payload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      618 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/disk/write_payload.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/networkattack/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/networkattack/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/stress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/stress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/stress/cpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      806 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/stress/memory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/jvmfault/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/jvmfault/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/jvmfault/gc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      832 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/jvmfault/raise_exception.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/network/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/network/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      750 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/network/bandwidth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/network/partition.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.472605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/podfault/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/podfault/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/podfault/container_kill.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      736 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_failure.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      934 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_kill.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.476605 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/stress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/stress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/stress/cpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/stress/memory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:51.476605 chaos_mesh-1.2.8/chaosmesh/k8s/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/k8s/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4234 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/k8s/crd.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5054 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/k8s/experiment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      536 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/k8s/k8s_resource.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      305 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/k8s/kubeclient.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      666 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/k8s/manifest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      534 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/chaosmesh/k8s/selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-02-23 03:13:51.476605 chaos_mesh-1.2.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1356 2023-02-23 03:13:33.000000 chaos_mesh-1.2.8/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-02-23 03:13:51.000000 chaos_mesh-1.2.8/version.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.246389 chaos_mesh-1.2.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6322 2023-02-24 05:30:03.246389 chaos_mesh-1.2.9/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.234389 chaos_mesh-1.2.9/chaos_mesh.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6322 2023-02-24 05:30:03.000000 chaos_mesh-1.2.9/chaos_mesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3036 2023-02-24 05:30:03.000000 chaos_mesh-1.2.9/chaos_mesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-24 05:30:03.000000 chaos_mesh-1.2.9/chaos_mesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-24 05:30:03.000000 chaos_mesh-1.2.9/chaos_mesh.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-02-24 05:30:03.000000 chaos_mesh-1.2.9/chaos_mesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-02-24 05:30:03.000000 chaos_mesh-1.2.9/chaos_mesh.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.234389 chaos_mesh-1.2.9/chaosmesh/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3254 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.234389 chaos_mesh-1.2.9/chaosmesh/experiments/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1709 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.234389 chaos_mesh-1.2.9/chaosmesh/experiments/base/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.234389 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.234389 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2242 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2399 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/fill.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1473 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/read_payload.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1612 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/write_payload.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.238389 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/networkattack/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/networkattack/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.238389 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/stress/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2072 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/stress/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2855 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/stress/cpu.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1883 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/stress/memory.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.238389 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.238389 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/jvmfault/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3014 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/jvmfault/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2088 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/jvmfault/gc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3175 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/jvmfault/raise_exception.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.238389 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/network/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2068 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/network/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3876 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/network/bandwidth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2193 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/network/partition.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.238389 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2527 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2125 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/container_kill.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      914 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/pod_failure.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      893 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/pod_kill.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.238389 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/stress/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      562 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/stress/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2549 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/stress/cpu.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2160 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/stress/memory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4438 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/factory.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.242390 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.242390 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.242390 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/disk/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/disk/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      477 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/disk/fill.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      710 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/disk/read_payload.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      618 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/disk/write_payload.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.242390 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/networkattack/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/networkattack/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.242390 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/stress/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/stress/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/stress/cpu.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      806 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/stress/memory.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.242390 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.242390 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/jvmfault/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/jvmfault/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/jvmfault/gc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      832 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/jvmfault/raise_exception.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.242390 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/network/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/network/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      750 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/network/bandwidth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/network/partition.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.246389 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/podfault/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/podfault/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/podfault/container_kill.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      736 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_failure.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      934 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_kill.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.246389 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/stress/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/stress/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/stress/cpu.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/stress/memory.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:30:03.246389 chaos_mesh-1.2.9/chaosmesh/k8s/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/k8s/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4234 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/k8s/crd.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5054 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/k8s/experiment.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      536 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/k8s/k8s_resource.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      305 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/k8s/kubeclient.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      666 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/k8s/manifest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      534 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/chaosmesh/k8s/selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-02-24 05:30:03.246389 chaos_mesh-1.2.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1356 2023-02-24 05:29:45.000000 chaos_mesh-1.2.9/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-02-24 05:30:03.000000 chaos_mesh-1.2.9/version.txt
```

### Comparing `chaos_mesh-1.2.8/PKG-INFO` & `chaos_mesh-1.2.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaos_mesh
-Version: 1.2.8
+Version: 1.2.9
 Summary: A client to create experiments in ChaosMesh
 Home-page: https://github.com/vishrantgupta/chaos-mesh
 Author: Vishrant Gupta
 Author-email: vishrant.gupta@gmail.com
 Description-Content-Type: text/markdown
 
 # Chaos Mesh Client
@@ -52,15 +52,21 @@
 - Exception
 
 ### Host Faults
 
 - CPU
 - Memory
 
-### Network Attach
+### Host Disk Fault
+
+- Read payload
+- Write payload
+- Fill
+
+### Network Attack
 
 - Partition
 - Bandwidth
 
 ## Experiment Examples
 
 Here are some examples of how you can create experiments in Chaos Mesh:
@@ -147,14 +153,42 @@
 
 # starting up the host memory stress experiment
 client.start_experiment(Experiment.HOST_STRESS_MEMORY, namespace="default", name=exp_name,
                         address=["10.225.66.224", "10.225.67.213", "10.225.66.231", "10.225.66.138", "10.225.66.192", "10.225.67.52", "10.225.67.103"],
                         size="30GB")
 ```
 
+### Host Disk Fault Read payload
+
+```python
+exp_name = "disk-fault-read-payload-" + random.randint(0, 1000000).__str__()
+
+# starting up the read payload experiment
+client.start_experiment(Experiment.HOST_READ_PAYLOAD, namespace="default", name=exp_name, selector=selector, address=["address"], size="1024K", path="/", payload_process_num=1)
+```
+
+### Host Disk Fault Write payload
+
+```python
+exp_name = "disk-fault-write-payload-" + random.randint(0, 1000000).__str__()
+
+# starting up the write payload experiment
+client.start_experiment(Experiment.HOST_WRITE_PAYLOAD, namespace="default", name=exp_name, selector=selector, address=["address"], size="1024K", path="/",
+                        payload_process_num=1)
+```
+
+### Host Disk Fill
+
+```python
+exp_name = "disk-fault-fill-" + random.randint(0, 1000000).__str__()
+
+# starting up the disk fill experiment
+client.start_experiment(Experiment.HOST_DISK_FILL, namespace="default", name=exp_name, selector=selector, address=["address"], size="1024K", path="/", fill_by_fallocate=True)
+```
+
 ### Network Partition
 
 ```python
 exp_name = "network-partition-" + random.randint(0, 1000000).__str__()
 
 # starting up the network partition experiment
 client.start_experiment(Experiment.NETWORK_PARTITION, namespace="default", name=exp_name, selector=selector, external_targets=["target"], direction="both")
@@ -166,15 +200,14 @@
 exp_name = "network-bandwidth-" + random.randint(0, 1000000).__str__()
 
 # starting up the network bandwidth experiment
 client.start_experiment(Experiment.NETWORK_BANDWIDTH, namespace="default", name=exp_name, selector=selector, rate="1bps", buffer=1, limit=1, direction="to",
                         external_targets=["target"])
 ```
 
-
 ## Pause an experiment
 
 In order to pause an experiment you can use the following command
 
 ```python
 # pausing the experiment
 client.pause_experiment(Experiment.POD_STRESS_MEMORY, namespace="default", name=exp_name)
```

### Comparing `chaos_mesh-1.2.8/chaos_mesh.egg-info/PKG-INFO` & `chaos_mesh-1.2.9/chaos_mesh.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaos-mesh
-Version: 1.2.8
+Version: 1.2.9
 Summary: A client to create experiments in ChaosMesh
 Home-page: https://github.com/vishrantgupta/chaos-mesh
 Author: Vishrant Gupta
 Author-email: vishrant.gupta@gmail.com
 Description-Content-Type: text/markdown
 
 # Chaos Mesh Client
@@ -52,15 +52,21 @@
 - Exception
 
 ### Host Faults
 
 - CPU
 - Memory
 
-### Network Attach
+### Host Disk Fault
+
+- Read payload
+- Write payload
+- Fill
+
+### Network Attack
 
 - Partition
 - Bandwidth
 
 ## Experiment Examples
 
 Here are some examples of how you can create experiments in Chaos Mesh:
@@ -147,14 +153,42 @@
 
 # starting up the host memory stress experiment
 client.start_experiment(Experiment.HOST_STRESS_MEMORY, namespace="default", name=exp_name,
                         address=["10.225.66.224", "10.225.67.213", "10.225.66.231", "10.225.66.138", "10.225.66.192", "10.225.67.52", "10.225.67.103"],
                         size="30GB")
 ```
 
+### Host Disk Fault Read payload
+
+```python
+exp_name = "disk-fault-read-payload-" + random.randint(0, 1000000).__str__()
+
+# starting up the read payload experiment
+client.start_experiment(Experiment.HOST_READ_PAYLOAD, namespace="default", name=exp_name, selector=selector, address=["address"], size="1024K", path="/", payload_process_num=1)
+```
+
+### Host Disk Fault Write payload
+
+```python
+exp_name = "disk-fault-write-payload-" + random.randint(0, 1000000).__str__()
+
+# starting up the write payload experiment
+client.start_experiment(Experiment.HOST_WRITE_PAYLOAD, namespace="default", name=exp_name, selector=selector, address=["address"], size="1024K", path="/",
+                        payload_process_num=1)
+```
+
+### Host Disk Fill
+
+```python
+exp_name = "disk-fault-fill-" + random.randint(0, 1000000).__str__()
+
+# starting up the disk fill experiment
+client.start_experiment(Experiment.HOST_DISK_FILL, namespace="default", name=exp_name, selector=selector, address=["address"], size="1024K", path="/", fill_by_fallocate=True)
+```
+
 ### Network Partition
 
 ```python
 exp_name = "network-partition-" + random.randint(0, 1000000).__str__()
 
 # starting up the network partition experiment
 client.start_experiment(Experiment.NETWORK_PARTITION, namespace="default", name=exp_name, selector=selector, external_targets=["target"], direction="both")
@@ -166,15 +200,14 @@
 exp_name = "network-bandwidth-" + random.randint(0, 1000000).__str__()
 
 # starting up the network bandwidth experiment
 client.start_experiment(Experiment.NETWORK_BANDWIDTH, namespace="default", name=exp_name, selector=selector, rate="1bps", buffer=1, limit=1, direction="to",
                         external_targets=["target"])
 ```
 
-
 ## Pause an experiment
 
 In order to pause an experiment you can use the following command
 
 ```python
 # pausing the experiment
 client.pause_experiment(Experiment.POD_STRESS_MEMORY, namespace="default", name=exp_name)
```

### Comparing `chaos_mesh-1.2.8/chaos_mesh.egg-info/SOURCES.txt` & `chaos_mesh-1.2.9/chaos_mesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/client.py` & `chaos_mesh-1.2.9/chaosmesh/client.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/__init__.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/__init__.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/fill.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/fill.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/read_payload.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/read_payload.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/disk/write_payload.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/disk/write_payload.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/stress/__init__.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/stress/__init__.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/stress/cpu.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/stress/cpu.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/hosts/stress/memory.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/hosts/stress/memory.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/jvmfault/__init__.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/jvmfault/__init__.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/jvmfault/gc.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/jvmfault/gc.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/jvmfault/raise_exception.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/jvmfault/raise_exception.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/network/__init__.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/network/__init__.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/network/bandwidth.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/network/bandwidth.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/network/partition.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/network/partition.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/__init__.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/__init__.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/container_kill.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/container_kill.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/pod_failure.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/pod_failure.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/podfault/pod_kill.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/podfault/pod_kill.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/stress/__init__.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/stress/__init__.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/stress/cpu.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/stress/cpu.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/base/k8s/stress/memory.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/base/k8s/stress/memory.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/factory.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/factory.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/disk/read_payload.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/disk/read_payload.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/disk/write_payload.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/disk/write_payload.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/stress/cpu.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/stress/cpu.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/hosts/stress/memory.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/hosts/stress/memory.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/jvmfault/gc.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/jvmfault/gc.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/jvmfault/raise_exception.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/jvmfault/raise_exception.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/network/bandwidth.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/network/bandwidth.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/podfault/container_kill.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/podfault/container_kill.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_failure.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_failure.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_kill.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_kill.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/stress/cpu.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/stress/cpu.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/experiments/v1alpha1/k8s/stress/memory.py` & `chaos_mesh-1.2.9/chaosmesh/experiments/v1alpha1/k8s/stress/memory.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/k8s/crd.py` & `chaos_mesh-1.2.9/chaosmesh/k8s/crd.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/k8s/experiment.py` & `chaos_mesh-1.2.9/chaosmesh/k8s/experiment.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/k8s/k8s_resource.py` & `chaos_mesh-1.2.9/chaosmesh/k8s/k8s_resource.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/k8s/manifest.py` & `chaos_mesh-1.2.9/chaosmesh/k8s/manifest.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/chaosmesh/k8s/selector.py` & `chaos_mesh-1.2.9/chaosmesh/k8s/selector.py`

 * *Files identical despite different names*

### Comparing `chaos_mesh-1.2.8/setup.py` & `chaos_mesh-1.2.9/setup.py`

 * *Files identical despite different names*

