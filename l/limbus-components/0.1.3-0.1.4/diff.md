# Comparing `tmp/limbus-components-0.1.3.tar.gz` & `tmp/limbus-components-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limbus-components-0.1.3.tar", last modified: Wed Mar 15 23:55:00 2023, max compression
+gzip compressed data, was "limbus-components-0.1.4.tar", last modified: Sun Apr 30 16:44:37 2023, max compression
```

## Comparing `limbus-components-0.1.3.tar` & `limbus-components-0.1.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.350833 limbus-components-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-15 23:52:47.000000 limbus-components-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-15 23:55:00.350833 limbus-components-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-15 23:52:47.000000 limbus-components-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.194831 limbus-components-0.1.3/limbus_components/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.198831 limbus-components-0.1.3/limbus_components/base/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/base/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.198831 limbus-components-0.1.3/limbus_components/kornia/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.202831 limbus-components-0.1.3/limbus_components/kornia/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/augmentation/RandomCrop.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.202831 limbus-components-0.1.3/limbus_components/kornia/color/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/color/hls_to_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/color/rgb_to_hls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.214831 limbus-components-0.1.3/limbus_components/kornia/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/contrib/FaceDetector.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/contrib/contrib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/contrib/histogram_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.242832 limbus-components-0.1.3/limbus_components/kornia/enhance/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/enhance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/enhance/equalize_clahe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/enhance/image_histogram2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/enhance/normalize_min_max.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.246832 limbus-components-0.1.3/limbus_components/kornia/feature/
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/feature/LoFTR.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/feature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.250832 limbus-components-0.1.3/limbus_components/kornia/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.298832 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Hflip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/HomographyWarper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/PyrDown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/PyrUp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Rot180.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/ScalePyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Shear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Vflip.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/crop_and_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/kornia/geometry/transform/warp_perspective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.310832 limbus-components-0.1.3/limbus_components/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/torch/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/torch/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/torch/squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/torch/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/torch/unbind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components/torch/unsqueeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.346833 limbus-components-0.1.3/limbus_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-15 23:54:59.000000 limbus-components-0.1.3/limbus_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-15 23:54:59.000000 limbus-components-0.1.3/limbus_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 23:54:59.000000 limbus-components-0.1.3/limbus_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-15 23:54:59.000000 limbus-components-0.1.3/limbus_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-15 23:54:59.000000 limbus-components-0.1.3/limbus_components.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.310832 limbus-components-0.1.3/limbus_components_dev/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components_dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.338833 limbus-components-0.1.3/limbus_components_dev/base/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components_dev/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components_dev/base/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.342833 limbus-components-0.1.3/limbus_components_dev/kornia/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components_dev/kornia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.346833 limbus-components-0.1.3/limbus_components_dev/kornia/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components_dev/kornia/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-03-15 23:52:47.000000 limbus-components-0.1.3/limbus_components_dev/kornia/contrib/contrib.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-15 23:55:00.350833 limbus-components-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-15 23:52:47.000000 limbus-components-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:55:00.346833 limbus-components-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-03-15 23:52:47.000000 limbus-components-0.1.3/tests/test_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.388913 limbus-components-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 16:42:22.000000 limbus-components-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-30 16:44:37.388913 limbus-components-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-30 16:42:22.000000 limbus-components-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.280913 limbus-components-0.1.4/limbus_components/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.284913 limbus-components-0.1.4/limbus_components/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15714 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/base/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.284913 limbus-components-0.1.4/limbus_components/kornia/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.288913 limbus-components-0.1.4/limbus_components/kornia/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/augmentation/RandomCrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.340913 limbus-components-0.1.4/limbus_components/kornia/color/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/color/hls_to_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/color/rgb_to_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.348913 limbus-components-0.1.4/limbus_components/kornia/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/contrib/FaceDetector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/contrib/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/contrib/histogram_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.352913 limbus-components-0.1.4/limbus_components/kornia/enhance/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/enhance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/enhance/equalize_clahe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/enhance/image_histogram2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/enhance/normalize_min_max.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.360913 limbus-components-0.1.4/limbus_components/kornia/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/feature/LoFTR.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/feature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.360913 limbus-components-0.1.4/limbus_components/kornia/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.376913 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Hflip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/HomographyWarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/PyrDown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/PyrUp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Rot180.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/ScalePyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Shear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Vflip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/crop_and_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/kornia/geometry/transform/warp_perspective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.380913 limbus-components-0.1.4/limbus_components/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/torch/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/torch/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/torch/squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/torch/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/torch/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components/torch/unsqueeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.388913 limbus-components-0.1.4/limbus_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-30 16:44:37.000000 limbus-components-0.1.4/limbus_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-30 16:44:37.000000 limbus-components-0.1.4/limbus_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:44:37.000000 limbus-components-0.1.4/limbus_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-30 16:44:37.000000 limbus-components-0.1.4/limbus_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-30 16:44:37.000000 limbus-components-0.1.4/limbus_components.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.384913 limbus-components-0.1.4/limbus_components_dev/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components_dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.384913 limbus-components-0.1.4/limbus_components_dev/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components_dev/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15714 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components_dev/base/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.384913 limbus-components-0.1.4/limbus_components_dev/kornia/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components_dev/kornia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.384913 limbus-components-0.1.4/limbus_components_dev/kornia/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components_dev/kornia/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-04-30 16:42:22.000000 limbus-components-0.1.4/limbus_components_dev/kornia/contrib/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-30 16:44:37.388913 limbus-components-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-30 16:42:22.000000 limbus-components-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:44:37.388913 limbus-components-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-30 16:42:22.000000 limbus-components-0.1.4/tests/test_components.py
```

### Comparing `limbus-components-0.1.3/LICENSE` & `limbus-components-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/PKG-INFO` & `limbus-components-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limbus-components
-Version: 0.1.3
+Version: 0.1.4
 Summary: Components to be used with limbus.
 Home-page: https://github.com/kornia/limbus-components
 Author: Luis Ferraz
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -39,7 +39,13 @@
 ```python
     from . import <component_module>  # to import modules
     from .<component_module> import <component_class0>, <component_class1>, ...  # to import components
     # IMPORTANT NOTE: imports with () are not allowed
 ```
 
 if they are not following these patterns, the `release` script will fail. Check examples in the folder `limbus_components_dev`.
+
+Steps to run the `release` script:
+- If you changed an existing module, first of all you need to remove the module in `limbus_components` folder.
+- Run the `release` script: `python scripts/release.py`
+- Check that the changes in the `limbus_components` folder are the expected ones.
+- commit the changes and push them to the repo.
```

### Comparing `limbus-components-0.1.3/README.md` & `limbus-components-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -29,7 +29,13 @@
 ```python
     from . import <component_module>  # to import modules
     from .<component_module> import <component_class0>, <component_class1>, ...  # to import components
     # IMPORTANT NOTE: imports with () are not allowed
 ```
 
 if they are not following these patterns, the `release` script will fail. Check examples in the folder `limbus_components_dev`.
+
+Steps to run the `release` script:
+- If you changed an existing module, first of all you need to remove the module in `limbus_components` folder.
+- Run the `release` script: `python scripts/release.py`
+- Check that the changes in the `limbus_components` folder are the expected ones.
+- commit the changes and push them to the repo.
```

### Comparing `limbus-components-0.1.3/limbus_components/base/base.py` & `limbus-components-0.1.4/limbus_components/base/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import asyncio
 
 import cv2
 import numpy as np
 import PIL
 import torch
 import kornia
-from limbus.core import Component, ComponentState, Params, InputParams, OutputParams, NoValue, InputParam, OutputParam
+from limbus.core import Component, ComponentState, PropertyParams, InputParams, OutputParams
+from limbus.core import NoValue, InputParam, OutputParam, PropertyParam  # We need to avoid ()
 from limbus.widgets import WidgetState, WidgetComponent, BaseWidgetComponent
 from limbus import widgets
 
 
 log = logging.getLogger(__name__)
 
 
@@ -37,51 +38,55 @@
     WIDGET_STATE: WidgetState = WidgetState.DISABLED
 
     class OutputsTyping(OutputParams):  # noqa: D106
         image: OutputParam
 
     outputs: OutputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        title: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     def __init__(self, name: str, path: Path, batch_size: int = 1):
         super().__init__(name)
         self._value: List[Path] = []
         self._batch_size = batch_size
         self._idx = 0
         if Path(path).is_dir():
             self._value = sorted(list(Path(path).glob("*")))
         else:
             self._value.append(Path(path))
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("image", torch.Tensor)
 
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         properties.declare("title", str, "")
 
     async def forward(self) -> ComponentState:  # noqa: D102
         images: List[torch.Tensor] = []
         batch_size = 0
         while batch_size < self._batch_size:
             if self._idx >= len(self._value):
                 return ComponentState.STOPPED
             try:
                 self._idx += 1
-                images.append(
-                    kornia.image_to_tensor(np.asarray(PIL.Image.open(str(self._value[self._idx]))))
-                )
+                array = np.asarray(PIL.Image.open(str(self._value[self._idx])))
+                images.append(kornia.image_to_tensor(array.copy()))  # to avoid issues with writable arrays
                 batch_size += 1
             except:
                 # avoid crashing the whole pipeline when there is a corrupted image or non-image file
                 pass
         batch = torch.stack(images)
         # images must be in the range [0, 1]
         batch = batch.div(255.).clamp(0, 1)
-        widgets.get().show_images(self, self._properties.get_param("title"), batch)
+        widgets.get().show_images(self, self._properties.title.value, batch)
         await self._outputs.image.send(batch)
         return ComponentState.OK
 
 
 class Webcam(WidgetComponent):
     """Component that read images from a webcam.
 
@@ -100,31 +105,37 @@
     WIDGET_STATE: WidgetState = WidgetState.DISABLED
 
     class OutputsTyping(OutputParams):  # noqa: D106
         image: OutputParam
 
     outputs: OutputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        title: PropertyParam
+        text_title: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     def __init__(self, name: str, batch_size: int = 1):
         super().__init__(name)
         self._batch_size = batch_size
         self._cap = cv2.VideoCapture(0)
         self._width: int = int(self._cap.get(cv2.CAP_PROP_FRAME_WIDTH))
         self._height: int = int(self._cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
         self._fps: float = self._cap.get(cv2.CAP_PROP_FPS)
 
-    def finish_pipeline(self):  # noqa: D102
+    def release(self):  # noqa: D102
         self._cap.release()
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("image", torch.Tensor)
 
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         properties.declare("title", str, "")
         # NOTE: When a widget does not have a title we assing the name of the component, so if we have >1
         # widgets without default title we will have several widgets with the same title and will be overriden.
         # TODO: allow to have several widgets with the same title.
         properties.declare("text_title", str, "txt")
 
     async def forward(self) -> ComponentState:  # noqa: D102
@@ -143,16 +154,16 @@
             batch_size += 1
             if batch_size > 1:
                 time.sleep(1 / self._fps)
 
         batch = torch.stack(images)
         # images must be in the range [0, 1]
         batch = batch.div(255.).clamp(0, 1)
-        widgets.get().show_images(self, self._properties.get_param("title"), batch)
-        widgets.get().show_text(self, self._properties.get_param("text_title"),
+        widgets.get().show_images(self, self._properties.title.value, batch)
+        widgets.get().show_text(self, self._properties.text_title.value,
                                 f"{self._fps} fps, {self._width}x{self._height}")
         await self._outputs.image.send(batch)
         return ComponentState.OK
 
 
 class DrawBoxes(Component):
     """Component that draw boxes on images.
@@ -178,20 +189,20 @@
     inputs: InputsTyping  # type: ignore
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str):
         super().__init__(name)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("images", torch.Tensor)
         inputs.declare("boxes", List[torch.Tensor])
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("out", torch.Tensor)
 
     def _draw_boxes(self, images: torch.Tensor, boxes: List[torch.Tensor]) -> torch.Tensor:
         imgs: np.ndarray = kornia.tensor_to_image(images, keepdim=True)
         imgs = (imgs * 255).astype(np.uint8)
         res_imgs: List[np.ndarray] = []
         for idx, image in enumerate(imgs):
@@ -232,20 +243,20 @@
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str, size: Tuple[int, int]):
         super().__init__(name)
         self._size: Tuple[int, int] = size
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("images", torch.Tensor)
         inputs.declare("boxes", List[torch.Tensor])
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("crops", torch.Tensor)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         images: torch.Tensor
         boxes_x_image: List[torch.Tensor]
         images, boxes_x_image = await asyncio.gather(self._inputs.images.receive(),
                                                      self._inputs.boxes.receive())
@@ -278,32 +289,38 @@
     """
 
     class InputsTyping(OutputParams):  # noqa: D106
         image: InputParam
 
     inputs: InputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        title: PropertyParam
+        nrow: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         # this line is like super() but for static methods.
         BaseWidgetComponent.register_properties(properties)  # adds the title param
         properties.declare("nrow", Optional[int], value=None)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("image", torch.Tensor)
 
     async def _show(self, title: str) -> None:  # noqa: D102
         images = await self._inputs.image.receive()
         if isinstance(images, NoValue):
             images = torch.empty((0, 0, 0, 0))
         if images.numel() == 0:
             # TODO: temporal solution, replace by something better
             images = torch.zeros((1, 1, max(images.shape[2], 1), max(images.shape[3], 1))).to(images)
-        widgets.get().show_images(self, title, images, nrow=self._properties.get_param("nrow"))
+        widgets.get().show_images(self, title, images, nrow=self._properties.nrow.value)
 
 
 class Constant(Component):
     """Component that holds a constant.
 
     Args:
         name (str): component name.
@@ -319,15 +336,15 @@
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str, value: Any):
         super().__init__(name)
         self._value = value
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("out", Any, arg="value")
 
     async def forward(self) -> ComponentState:  # noqa: D102
         # TODO: next line could be autogenerated since in register_inputs() we are already linking both.
         await self._outputs.out.send(self._value)
         return ComponentState.OK
 
@@ -347,28 +364,34 @@
 
     """
     class InputsTyping(OutputParams):  # noqa: D106
         inp: InputParam
 
     inputs: InputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        title: PropertyParam
+        append: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         # this line is like super() but for static methods.
         BaseWidgetComponent.register_properties(properties)  # adds the title param
         properties.declare("append", bool, value=False)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("inp", Any)
 
     async def _show(self, title: str) -> None:  # noqa: D102
         widgets.get().show_text(self, title,
                                 str(await self._inputs.inp.receive()),
-                                append=self._properties.get_param("append"))
+                                append=self._properties.append.value)
 
 
 class Accumulator(Component):
     """Component to accumulate sequential data.
 
     Args:
         name (str): component name.
@@ -435,19 +458,19 @@
     inputs: InputsTyping  # type: ignore
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str):
         super().__init__(name)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("a", torch.Tensor)
         inputs.declare("b", torch.Tensor)
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("out", torch.Tensor)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         a, b = await asyncio.gather(self.inputs.a.receive(), self.inputs.b.receive())
         await self.outputs.out.send(a + b)
         return ComponentState.OK
```

### Comparing `limbus-components-0.1.3/limbus_components/kornia/augmentation/RandomCrop.py` & `limbus-components-0.1.4/limbus_components/kornia/augmentation/RandomCrop.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/color/hls_to_rgb.py` & `limbus-components-0.1.4/limbus_components/kornia/color/hls_to_rgb.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/color/rgb_to_hls.py` & `limbus-components-0.1.4/limbus_components/kornia/color/rgb_to_hls.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/contrib/FaceDetector.py` & `limbus-components-0.1.4/limbus_components/kornia/contrib/FaceDetector.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/contrib/contrib.py` & `limbus-components-0.1.4/limbus_components/kornia/contrib/contrib.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import logging
 import asyncio
 
 import cv2
 import numpy as np
 import torch
 import kornia
-from limbus.core import Component, InputParams, OutputParams, Params, ComponentState, InputParam, OutputParam
+from limbus.core import Component, InputParams, OutputParams, PropertyParams, ComponentState
+from limbus.core import InputParam, OutputParam, PropertyParam  # we need to avoid ()
 from limbus.widgets import WidgetState, BaseWidgetComponent, WidgetComponent
 from limbus import widgets
 
 
 log = logging.getLogger(__name__)
 
 
@@ -31,24 +32,31 @@
     """
     class InputsTyping(OutputParams):  # noqa: D106
         image: InputParam
         landmarks: InputParam
 
     inputs: InputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        nrow: PropertyParam
+        draw_keypoints: PropertyParam
+        threshold: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     # the viz state by default is disabled but can be enabled by the user with the widget_state property.
     WIDGET_STATE: WidgetState = WidgetState.DISABLED
 
     @staticmethod
     def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("image", torch.Tensor)
         inputs.declare("landmarks", torch.Tensor)
 
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         # this line is like super() but for static methods.
         BaseWidgetComponent.register_properties(properties)  # adds the title param
         properties.declare("nrow", Optional[int], value=None)
         properties.declare("draw_keypoints", bool, False)
         properties.declare("threshold", float, 0.8)
 
     def _draw_keypoint(self, img: np.ndarray,
@@ -58,15 +66,15 @@
         return cv2.circle(img, kpt, 2, (255, 0, 0), 2)
 
     def _draw_landmarks(self, image: torch.Tensor, landmarks: torch.Tensor) -> torch.Tensor:
         dets: List[kornia.contrib.FaceDetectorResult] = [kornia.contrib.FaceDetectorResult(o) for o in landmarks]
         frame_vis: np.ndarray = kornia.tensor_to_image(image).copy()
         frame_vis = (frame_vis * 255).astype(np.uint8)
         for b in dets:
-            if b.score < self._properties.get_param("threshold"):
+            if b.score < self._properties.threshold.value:
                 continue
 
             # draw face bounding box
             line_thickness = 4
             line_length = 20
 
             x1, y1 = b.top_left.int().tolist()
@@ -81,29 +89,29 @@
             frame_vis = cv2.line(frame_vis, (x1, y1), (x1 - line_length, y1), (0, 255, 0), thickness=line_thickness)
             frame_vis = cv2.line(frame_vis, (x1, y1), (x1, y1 - line_length), (0, 255, 0), thickness=line_thickness)
 
             x1, y1 = b.bottom_left.int().tolist()
             frame_vis = cv2.line(frame_vis, (x1, y1), (x1 + line_length, y1), (0, 255, 0), thickness=line_thickness)
             frame_vis = cv2.line(frame_vis, (x1, y1), (x1, y1 - line_length), (0, 255, 0), thickness=line_thickness)
 
-            if self._properties.get_param("draw_keypoints"):
+            if self._properties.draw_keypoints.value:
                 # draw facial keypoints
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.EYE_LEFT)
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.EYE_RIGHT)
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.NOSE)
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.MOUTH_LEFT)
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.MOUTH_RIGHT)
 
         return kornia.image_to_tensor(frame_vis)
 
     async def _show(self, title: str) -> None:  # noqa: D102
         images, landmarks = await asyncio.gather(self.inputs.image.receive(),
                                                  self.inputs.landmarks.receive())
         images = self._draw_landmarks(images, landmarks)
-        widgets.get().show_images(self, title, images, nrow=self._properties.get_param("nrow"))
+        widgets.get().show_images(self, title, images, nrow=self._properties.nrow.value)
 
 
 class FaceDetectorToBoxes(Component):
     """Component that get the bounding boxes from the FaceDetector.
 
     Args:
         name (str): component name.
@@ -129,25 +137,25 @@
         inputs.declare("landmarks", torch.Tensor)
 
     @staticmethod
     def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("boxes", torch.Tensor)
 
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         # this line is like super() but for static methods.
         WidgetComponent.register_properties(properties)  # adds the title param
         properties.declare("threshold", float, 0.8)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         landmarks = await self.inputs.landmarks.receive()
         dets: List[kornia.contrib.FaceDetectorResult] = [kornia.contrib.FaceDetectorResult(o) for o in landmarks]
         bboxes: List[torch.Tensor] = []
         for b in dets:
-            if b.score < self._properties.get_param("threshold"):
+            if b.score < self._properties.threshold.value:
                 continue
             # order: top-left, top-right, bottom-right and bottom-left
             bboxes.append(torch.stack((b.top_left, b.top_right, b.bottom_right, b.bottom_left)))
         if len(bboxes) > 0:
             await self.outputs.boxes.send(torch.stack(bboxes))
         else:
             await self.outputs.boxes.send(torch.empty((0, 4, 2)).to(landmarks))
@@ -184,19 +192,19 @@
     def __init__(self, name: str, estimator: str = 'ransac', blending_method: str = 'naive'):
         super().__init__(name)
         gftt_hardnet_matcher = kornia.feature.LocalFeatureMatcher(kornia.feature.GFTTAffNetHardNet(500),
                                                                   kornia.feature.DescriptorMatcher('snn', 0.8))
         self._is = kornia.contrib.ImageStitcher(gftt_hardnet_matcher, estimator, blending_method)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("imgs", torch.Tensor)
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("out", torch.Tensor)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         await self.outputs.out.send(self._is(*((await self._inputs.imgs.receive()).unsqueeze(1))))
         return ComponentState.OK
 
 
@@ -225,20 +233,20 @@
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str):
         super().__init__(name)
         self._ir = kornia.geometry.ImageRegistrator()
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("img_src", torch.Tensor)
         inputs.declare("img_dst", torch.Tensor)
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("homo", torch.Tensor)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         img_src, img_dst = await asyncio.gather(self.inputs.img_src.receive(),
                                                 self.inputs.img_dst.receive())
         await self.outputs.homo.send(self._ir.register(img_src, img_dst))
         return ComponentState.OK
```

### Comparing `limbus-components-0.1.3/limbus_components/kornia/contrib/histogram_matching.py` & `limbus-components-0.1.4/limbus_components/kornia/contrib/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/enhance/equalize_clahe.py` & `limbus-components-0.1.4/limbus_components/kornia/enhance/equalize_clahe.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/enhance/image_histogram2d.py` & `limbus-components-0.1.4/limbus_components/kornia/enhance/image_histogram2d.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/enhance/normalize_min_max.py` & `limbus-components-0.1.4/limbus_components/kornia/enhance/normalize_min_max.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/feature/LoFTR.py` & `limbus-components-0.1.4/limbus_components/kornia/feature/LoFTR.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Affine.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Affine.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Hflip.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Hflip.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/HomographyWarper.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/HomographyWarper.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/PyrDown.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/PyrDown.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/PyrUp.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/PyrUp.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Rescale.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Rescale.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Resize.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Resize.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Rot180.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Rot180.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Rotate.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Rotate.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Scale.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Scale.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/ScalePyramid.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/ScalePyramid.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Shear.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Shear.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Translate.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Translate.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/Vflip.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/Vflip.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/__init__.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/center_crop.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/center_crop.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/crop_and_resize.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/crop_and_resize.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/kornia/geometry/transform/warp_perspective.py` & `limbus-components-0.1.4/limbus_components/kornia/geometry/transform/warp_perspective.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/torch/cat.py` & `limbus-components-0.1.4/limbus_components/torch/cat.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/torch/select.py` & `limbus-components-0.1.4/limbus_components/torch/select.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/torch/squeeze.py` & `limbus-components-0.1.4/limbus_components/torch/squeeze.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/torch/stack.py` & `limbus-components-0.1.4/limbus_components/torch/stack.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/torch/unbind.py` & `limbus-components-0.1.4/limbus_components/torch/unbind.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components/torch/unsqueeze.py` & `limbus-components-0.1.4/limbus_components/torch/unsqueeze.py`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components.egg-info/PKG-INFO` & `limbus-components-0.1.4/limbus_components.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limbus-components
-Version: 0.1.3
+Version: 0.1.4
 Summary: Components to be used with limbus.
 Home-page: https://github.com/kornia/limbus-components
 Author: Luis Ferraz
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -39,7 +39,13 @@
 ```python
     from . import <component_module>  # to import modules
     from .<component_module> import <component_class0>, <component_class1>, ...  # to import components
     # IMPORTANT NOTE: imports with () are not allowed
 ```
 
 if they are not following these patterns, the `release` script will fail. Check examples in the folder `limbus_components_dev`.
+
+Steps to run the `release` script:
+- If you changed an existing module, first of all you need to remove the module in `limbus_components` folder.
+- Run the `release` script: `python scripts/release.py`
+- Check that the changes in the `limbus_components` folder are the expected ones.
+- commit the changes and push them to the repo.
```

### Comparing `limbus-components-0.1.3/limbus_components.egg-info/SOURCES.txt` & `limbus-components-0.1.4/limbus_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/limbus_components_dev/base/base.py` & `limbus-components-0.1.4/limbus_components_dev/base/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import asyncio
 
 import cv2
 import numpy as np
 import PIL
 import torch
 import kornia
-from limbus.core import Component, ComponentState, Params, InputParams, OutputParams, NoValue, InputParam, OutputParam
+from limbus.core import Component, ComponentState, PropertyParams, InputParams, OutputParams
+from limbus.core import NoValue, InputParam, OutputParam, PropertyParam  # We need to avoid ()
 from limbus.widgets import WidgetState, WidgetComponent, BaseWidgetComponent
 from limbus import widgets
 
 
 log = logging.getLogger(__name__)
 
 
@@ -37,51 +38,55 @@
     WIDGET_STATE: WidgetState = WidgetState.DISABLED
 
     class OutputsTyping(OutputParams):  # noqa: D106
         image: OutputParam
 
     outputs: OutputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        title: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     def __init__(self, name: str, path: Path, batch_size: int = 1):
         super().__init__(name)
         self._value: List[Path] = []
         self._batch_size = batch_size
         self._idx = 0
         if Path(path).is_dir():
             self._value = sorted(list(Path(path).glob("*")))
         else:
             self._value.append(Path(path))
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("image", torch.Tensor)
 
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         properties.declare("title", str, "")
 
     async def forward(self) -> ComponentState:  # noqa: D102
         images: List[torch.Tensor] = []
         batch_size = 0
         while batch_size < self._batch_size:
             if self._idx >= len(self._value):
                 return ComponentState.STOPPED
             try:
                 self._idx += 1
-                images.append(
-                    kornia.image_to_tensor(np.asarray(PIL.Image.open(str(self._value[self._idx]))))
-                )
+                array = np.asarray(PIL.Image.open(str(self._value[self._idx])))
+                images.append(kornia.image_to_tensor(array.copy()))  # to avoid issues with writable arrays
                 batch_size += 1
             except:
                 # avoid crashing the whole pipeline when there is a corrupted image or non-image file
                 pass
         batch = torch.stack(images)
         # images must be in the range [0, 1]
         batch = batch.div(255.).clamp(0, 1)
-        widgets.get().show_images(self, self._properties.get_param("title"), batch)
+        widgets.get().show_images(self, self._properties.title.value, batch)
         await self._outputs.image.send(batch)
         return ComponentState.OK
 
 
 class Webcam(WidgetComponent):
     """Component that read images from a webcam.
 
@@ -100,31 +105,37 @@
     WIDGET_STATE: WidgetState = WidgetState.DISABLED
 
     class OutputsTyping(OutputParams):  # noqa: D106
         image: OutputParam
 
     outputs: OutputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        title: PropertyParam
+        text_title: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     def __init__(self, name: str, batch_size: int = 1):
         super().__init__(name)
         self._batch_size = batch_size
         self._cap = cv2.VideoCapture(0)
         self._width: int = int(self._cap.get(cv2.CAP_PROP_FRAME_WIDTH))
         self._height: int = int(self._cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
         self._fps: float = self._cap.get(cv2.CAP_PROP_FPS)
 
-    def finish_pipeline(self):  # noqa: D102
+    def release(self):  # noqa: D102
         self._cap.release()
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("image", torch.Tensor)
 
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         properties.declare("title", str, "")
         # NOTE: When a widget does not have a title we assing the name of the component, so if we have >1
         # widgets without default title we will have several widgets with the same title and will be overriden.
         # TODO: allow to have several widgets with the same title.
         properties.declare("text_title", str, "txt")
 
     async def forward(self) -> ComponentState:  # noqa: D102
@@ -143,16 +154,16 @@
             batch_size += 1
             if batch_size > 1:
                 time.sleep(1 / self._fps)
 
         batch = torch.stack(images)
         # images must be in the range [0, 1]
         batch = batch.div(255.).clamp(0, 1)
-        widgets.get().show_images(self, self._properties.get_param("title"), batch)
-        widgets.get().show_text(self, self._properties.get_param("text_title"),
+        widgets.get().show_images(self, self._properties.title.value, batch)
+        widgets.get().show_text(self, self._properties.text_title.value,
                                 f"{self._fps} fps, {self._width}x{self._height}")
         await self._outputs.image.send(batch)
         return ComponentState.OK
 
 
 class DrawBoxes(Component):
     """Component that draw boxes on images.
@@ -178,20 +189,20 @@
     inputs: InputsTyping  # type: ignore
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str):
         super().__init__(name)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("images", torch.Tensor)
         inputs.declare("boxes", List[torch.Tensor])
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("out", torch.Tensor)
 
     def _draw_boxes(self, images: torch.Tensor, boxes: List[torch.Tensor]) -> torch.Tensor:
         imgs: np.ndarray = kornia.tensor_to_image(images, keepdim=True)
         imgs = (imgs * 255).astype(np.uint8)
         res_imgs: List[np.ndarray] = []
         for idx, image in enumerate(imgs):
@@ -232,20 +243,20 @@
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str, size: Tuple[int, int]):
         super().__init__(name)
         self._size: Tuple[int, int] = size
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("images", torch.Tensor)
         inputs.declare("boxes", List[torch.Tensor])
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("crops", torch.Tensor)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         images: torch.Tensor
         boxes_x_image: List[torch.Tensor]
         images, boxes_x_image = await asyncio.gather(self._inputs.images.receive(),
                                                      self._inputs.boxes.receive())
@@ -278,32 +289,38 @@
     """
 
     class InputsTyping(OutputParams):  # noqa: D106
         image: InputParam
 
     inputs: InputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        title: PropertyParam
+        nrow: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         # this line is like super() but for static methods.
         BaseWidgetComponent.register_properties(properties)  # adds the title param
         properties.declare("nrow", Optional[int], value=None)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("image", torch.Tensor)
 
     async def _show(self, title: str) -> None:  # noqa: D102
         images = await self._inputs.image.receive()
         if isinstance(images, NoValue):
             images = torch.empty((0, 0, 0, 0))
         if images.numel() == 0:
             # TODO: temporal solution, replace by something better
             images = torch.zeros((1, 1, max(images.shape[2], 1), max(images.shape[3], 1))).to(images)
-        widgets.get().show_images(self, title, images, nrow=self._properties.get_param("nrow"))
+        widgets.get().show_images(self, title, images, nrow=self._properties.nrow.value)
 
 
 class Constant(Component):
     """Component that holds a constant.
 
     Args:
         name (str): component name.
@@ -319,15 +336,15 @@
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str, value: Any):
         super().__init__(name)
         self._value = value
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("out", Any, arg="value")
 
     async def forward(self) -> ComponentState:  # noqa: D102
         # TODO: next line could be autogenerated since in register_inputs() we are already linking both.
         await self._outputs.out.send(self._value)
         return ComponentState.OK
 
@@ -347,28 +364,34 @@
 
     """
     class InputsTyping(OutputParams):  # noqa: D106
         inp: InputParam
 
     inputs: InputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        title: PropertyParam
+        append: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         # this line is like super() but for static methods.
         BaseWidgetComponent.register_properties(properties)  # adds the title param
         properties.declare("append", bool, value=False)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("inp", Any)
 
     async def _show(self, title: str) -> None:  # noqa: D102
         widgets.get().show_text(self, title,
                                 str(await self._inputs.inp.receive()),
-                                append=self._properties.get_param("append"))
+                                append=self._properties.append.value)
 
 
 class Accumulator(Component):
     """Component to accumulate sequential data.
 
     Args:
         name (str): component name.
@@ -435,19 +458,19 @@
     inputs: InputsTyping  # type: ignore
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str):
         super().__init__(name)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("a", torch.Tensor)
         inputs.declare("b", torch.Tensor)
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("out", torch.Tensor)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         a, b = await asyncio.gather(self.inputs.a.receive(), self.inputs.b.receive())
         await self.outputs.out.send(a + b)
         return ComponentState.OK
```

### Comparing `limbus-components-0.1.3/limbus_components_dev/kornia/contrib/contrib.py` & `limbus-components-0.1.4/limbus_components_dev/kornia/contrib/contrib.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import logging
 import asyncio
 
 import cv2
 import numpy as np
 import torch
 import kornia
-from limbus.core import Component, InputParams, OutputParams, Params, ComponentState, InputParam, OutputParam
+from limbus.core import Component, InputParams, OutputParams, PropertyParams, ComponentState
+from limbus.core import InputParam, OutputParam, PropertyParam  # we need to avoid ()
 from limbus.widgets import WidgetState, BaseWidgetComponent, WidgetComponent
 from limbus import widgets
 
 
 log = logging.getLogger(__name__)
 
 
@@ -31,24 +32,31 @@
     """
     class InputsTyping(OutputParams):  # noqa: D106
         image: InputParam
         landmarks: InputParam
 
     inputs: InputsTyping  # type: ignore
 
+    class PropTyping(PropertyParams):  # noqa: D106
+        nrow: PropertyParam
+        draw_keypoints: PropertyParam
+        threshold: PropertyParam
+
+    properties: PropTyping  # type: ignore
+
     # the viz state by default is disabled but can be enabled by the user with the widget_state property.
     WIDGET_STATE: WidgetState = WidgetState.DISABLED
 
     @staticmethod
     def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("image", torch.Tensor)
         inputs.declare("landmarks", torch.Tensor)
 
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         # this line is like super() but for static methods.
         BaseWidgetComponent.register_properties(properties)  # adds the title param
         properties.declare("nrow", Optional[int], value=None)
         properties.declare("draw_keypoints", bool, False)
         properties.declare("threshold", float, 0.8)
 
     def _draw_keypoint(self, img: np.ndarray,
@@ -58,15 +66,15 @@
         return cv2.circle(img, kpt, 2, (255, 0, 0), 2)
 
     def _draw_landmarks(self, image: torch.Tensor, landmarks: torch.Tensor) -> torch.Tensor:
         dets: List[kornia.contrib.FaceDetectorResult] = [kornia.contrib.FaceDetectorResult(o) for o in landmarks]
         frame_vis: np.ndarray = kornia.tensor_to_image(image).copy()
         frame_vis = (frame_vis * 255).astype(np.uint8)
         for b in dets:
-            if b.score < self._properties.get_param("threshold"):
+            if b.score < self._properties.threshold.value:
                 continue
 
             # draw face bounding box
             line_thickness = 4
             line_length = 20
 
             x1, y1 = b.top_left.int().tolist()
@@ -81,29 +89,29 @@
             frame_vis = cv2.line(frame_vis, (x1, y1), (x1 - line_length, y1), (0, 255, 0), thickness=line_thickness)
             frame_vis = cv2.line(frame_vis, (x1, y1), (x1, y1 - line_length), (0, 255, 0), thickness=line_thickness)
 
             x1, y1 = b.bottom_left.int().tolist()
             frame_vis = cv2.line(frame_vis, (x1, y1), (x1 + line_length, y1), (0, 255, 0), thickness=line_thickness)
             frame_vis = cv2.line(frame_vis, (x1, y1), (x1, y1 - line_length), (0, 255, 0), thickness=line_thickness)
 
-            if self._properties.get_param("draw_keypoints"):
+            if self._properties.draw_keypoints.value:
                 # draw facial keypoints
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.EYE_LEFT)
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.EYE_RIGHT)
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.NOSE)
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.MOUTH_LEFT)
                 frame_vis = self._draw_keypoint(frame_vis, b, kornia.contrib.FaceKeypoint.MOUTH_RIGHT)
 
         return kornia.image_to_tensor(frame_vis)
 
     async def _show(self, title: str) -> None:  # noqa: D102
         images, landmarks = await asyncio.gather(self.inputs.image.receive(),
                                                  self.inputs.landmarks.receive())
         images = self._draw_landmarks(images, landmarks)
-        widgets.get().show_images(self, title, images, nrow=self._properties.get_param("nrow"))
+        widgets.get().show_images(self, title, images, nrow=self._properties.nrow.value)
 
 
 class FaceDetectorToBoxes(Component):
     """Component that get the bounding boxes from the FaceDetector.
 
     Args:
         name (str): component name.
@@ -129,25 +137,25 @@
         inputs.declare("landmarks", torch.Tensor)
 
     @staticmethod
     def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("boxes", torch.Tensor)
 
     @staticmethod
-    def register_properties(properties: Params) -> None:  # noqa: D102
+    def register_properties(properties: PropertyParams) -> None:  # noqa: D102
         # this line is like super() but for static methods.
         WidgetComponent.register_properties(properties)  # adds the title param
         properties.declare("threshold", float, 0.8)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         landmarks = await self.inputs.landmarks.receive()
         dets: List[kornia.contrib.FaceDetectorResult] = [kornia.contrib.FaceDetectorResult(o) for o in landmarks]
         bboxes: List[torch.Tensor] = []
         for b in dets:
-            if b.score < self._properties.get_param("threshold"):
+            if b.score < self._properties.threshold.value:
                 continue
             # order: top-left, top-right, bottom-right and bottom-left
             bboxes.append(torch.stack((b.top_left, b.top_right, b.bottom_right, b.bottom_left)))
         if len(bboxes) > 0:
             await self.outputs.boxes.send(torch.stack(bboxes))
         else:
             await self.outputs.boxes.send(torch.empty((0, 4, 2)).to(landmarks))
@@ -184,19 +192,19 @@
     def __init__(self, name: str, estimator: str = 'ransac', blending_method: str = 'naive'):
         super().__init__(name)
         gftt_hardnet_matcher = kornia.feature.LocalFeatureMatcher(kornia.feature.GFTTAffNetHardNet(500),
                                                                   kornia.feature.DescriptorMatcher('snn', 0.8))
         self._is = kornia.contrib.ImageStitcher(gftt_hardnet_matcher, estimator, blending_method)
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("imgs", torch.Tensor)
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("out", torch.Tensor)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         await self.outputs.out.send(self._is(*((await self._inputs.imgs.receive()).unsqueeze(1))))
         return ComponentState.OK
 
 
@@ -225,20 +233,20 @@
     outputs: OutputsTyping  # type: ignore
 
     def __init__(self, name: str):
         super().__init__(name)
         self._ir = kornia.geometry.ImageRegistrator()
 
     @staticmethod
-    def register_inputs(inputs: Params) -> None:  # noqa: D102
+    def register_inputs(inputs: InputParams) -> None:  # noqa: D102
         inputs.declare("img_src", torch.Tensor)
         inputs.declare("img_dst", torch.Tensor)
 
     @staticmethod
-    def register_outputs(outputs: Params) -> None:  # noqa: D102
+    def register_outputs(outputs: OutputParams) -> None:  # noqa: D102
         outputs.declare("homo", torch.Tensor)
 
     async def forward(self) -> ComponentState:  # noqa: D102
         img_src, img_dst = await asyncio.gather(self.inputs.img_src.receive(),
                                                 self.inputs.img_dst.receive())
         await self.outputs.homo.send(self._ir.register(img_src, img_dst))
         return ComponentState.OK
```

### Comparing `limbus-components-0.1.3/setup.cfg` & `limbus-components-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `limbus-components-0.1.3/setup.py` & `limbus-components-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(name='limbus-components',
-      version='0.1.3',
+      version='0.1.4',
       description='Components to be used with limbus.',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       author='Luis Ferraz',
       url='https://github.com/kornia/limbus-components',
       install_requires=[
-          'limbus >= 0.1.4',
+          'limbus >= 0.1.6',
           'torch',
           'numpy',
           'kornia',
           'opencv-python',
           'pillow',
       ],
       extras_require={
```

### Comparing `limbus-components-0.1.3/tests/test_components.py` & `limbus-components-0.1.4/tests/test_components.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,121 +9,121 @@
 from limbus_components_dev.base import Constant, Adder, ImageShow, Printer
 
 
 class TestConstant:
     @pytest.mark.parametrize("value", ([1, 2., torch.tensor(3.)]))
     def test_smoke(self, value):
         c = Constant("k", value)
-        assert c.state == ComponentState.INITIALIZED
+        assert ComponentState.INITIALIZED in c.state
         assert c.name == "k"
         assert isinstance(c.outputs.out.value, NoValue)
         asyncio.run(c())
-        assert c.state == ComponentState.OK
+        assert ComponentState.OK in c.state
         assert c.outputs.out.value == value
 
 
 class TestAdder:
     def test_smoke(self):
         add = Adder("add")
-        assert add.state == ComponentState.INITIALIZED
+        assert ComponentState.INITIALIZED in add.state
         assert add.name == "add"
-        print(add.outputs.get_param("out"))
-        assert isinstance(add.outputs.get_param("out"), NoValue)
+        print(add.outputs.out.value)
+        assert isinstance(add.outputs.out.value, NoValue)
 
         add.inputs.a.value = torch.tensor(2.)
         add.inputs.b.value = torch.tensor(3.)
         asyncio.run(add())
-        assert add.state == ComponentState.OK
+        assert ComponentState.OK in add.state
         assert add.outputs.out.value == torch.tensor(5.)
 
 
 class TestImageShow:
     def test_viz_enabled(self):
         show = ImageShow("show")
-        assert show.state == ComponentState.INITIALIZED
+        assert ComponentState.INITIALIZED in show.state
         assert show.name == "show"
-        assert show.properties.get_param("title") == ""
-        assert show.properties.get_param("nrow") is None
+        assert show.properties.title.value == ""
+        assert show.properties.nrow.value is None
 
         show.inputs.image.value = torch.zeros((1, 3, 20, 20))
         asyncio.run(show())
         # by default the viz is done in Console. Images cannot be shown in Console and returns a log.warning.
         # log.warning("Console visualization does not show images.")
         # anyway the ComponentState returned is Ok in this case.
-        assert show.state == ComponentState.OK
+        assert ComponentState.OK in show.state
 
     def test_viz_disabled(self):
         # disable the Console visualization
         widgets.get()._enabled = False
 
         try:
             show = ImageShow("show")
-            assert show.state == ComponentState.INITIALIZED
+            assert ComponentState.INITIALIZED in show.state
             show.inputs.image.value = torch.zeros((1, 3, 20, 20))
             asyncio.run(show())
-            assert show.state == ComponentState.DISABLED
+            assert ComponentState.DISABLED in show.state
         except Exception as e:
             raise e
         finally:
             widgets.get()._enabled = True
 
     def test_viz_name(self):
         show = ImageShow("show")
-        show.properties.set_param("title", "my title")
+        show.properties.title.init_property("my title")
         assert show.name == "show"
-        assert show.properties.get_param("title") == "my title"
+        assert show.properties.title.value == "my title"
         asyncio.run(show())
-        assert show.state == ComponentState.OK
+        assert ComponentState.OK in show.state
 
     def test_set_properties(self):
         assert ImageShow.WIDGET_STATE == WidgetState.ENABLED
         show = ImageShow("show")
         show.widget_state = WidgetState.ENABLED
         assert show.name == "show"
-        assert show.set_properties(title="my_title", nrow=2)
-        assert show.properties.get_param("title") == "my_title"
-        assert show.properties.get_param("nrow") == 2
-        assert not show.set_properties(title="my_title", xyz=2)
+        show.properties.title.init_property("my_title")
+        show.properties.nrow.init_property(2)
+        assert show.properties.title.value == "my_title"
+        assert show.properties.nrow.value == 2
 
 
 class TestPrinter:
     def test_viz_enabled(self):
         printer = Printer("printer")
         assert printer.name == "printer"
-        assert printer.properties.get_param("title") == ""
-        assert printer.properties.get_param("append") is False
+        assert printer.properties.title.value == ""
+        assert printer.properties.append.value is False
 
         printer.inputs.inp.value = torch.zeros((1, 3, 20, 20))
         asyncio.run(printer())
-        assert printer.state == ComponentState.OK
+        assert ComponentState.OK in printer.state
 
     def test_viz_disabled(self):
         # disable the Console visualization
         widgets.get()._enabled = False
 
         try:
             printer = Printer("printer")
             printer.inputs.inp.value = torch.zeros((1, 3, 20, 20))
             asyncio.run(printer())
-            assert printer.state == ComponentState.DISABLED
+            assert ComponentState.DISABLED in printer.state
         except Exception as e:
             raise e
         finally:
             widgets.get()._enabled = True
 
     def test_viz_name(self):
         printer = Printer("printer")
-        printer.properties.set_param("title", "my title")
+        printer.properties.title.init_property("my title")
         assert printer.name == "printer"
-        assert printer.properties.get_param("title") == "my title"
+        assert printer.properties.title.value == "my title"
         asyncio.run(printer())
-        assert printer.state == ComponentState.OK
+        assert ComponentState.OK in printer.state
 
     def test_set_properties(self):
         assert Printer.WIDGET_STATE == WidgetState.ENABLED
         printer = Printer("printer")
         printer.widget_state = WidgetState.ENABLED
         assert printer.name == "printer"
-        assert printer.set_properties(title="my_title", append=True)
-        assert printer.properties.get_param("title") == "my_title"
-        assert printer.properties.get_param("append") is True
-        assert not printer.set_properties(title="my_title", xyz=2)
+        printer.properties.title.init_property("my_title")
+        printer.properties.append.init_property(True)
+        assert printer.properties.title.value == "my_title"
+        assert printer.properties.append.value is True
```

