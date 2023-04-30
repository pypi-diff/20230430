# Comparing `tmp/opencv_stubs-0.0.5.tar.gz` & `tmp/opencv_stubs-0.0.6.tar.gz`

## Comparing `opencv_stubs-0.0.5.tar` & `opencv_stubs-0.0.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/requirements/requirements.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/__init__.pyi
--rw-r--r--   0        0        0   165718 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/classes.pyi
--rw-r--r--   0        0        0    51441 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/constants.pyi
--rw-r--r--   0        0        0   529741 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/functions.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/py.typed
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/__init__.py
--rw-r--r--   0        0        0    34278 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/aruco.pyi
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/barcode.pyi
--rw-r--r--   0        0        0    11087 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/bgsegm.pyi
--rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/bioinspired.pyi
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ccm.pyi
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/colored_kinfu.pyi
--rw-r--r--   0        0        0    23465 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/cuda.pyi
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/data.pyi
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/datasets.pyi
--rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/detail.pyi
--rw-r--r--   0        0        0    44941 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/dnn.pyi
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/dnn_superres.pyi
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/dpm.pyi
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/dynafu.pyi
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/error.pyi
--rw-r--r--   0        0        0    34295 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/face.pyi
--rw-r--r--   0        0        0    21983 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/fisheye.pyi
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/flann.pyi
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ft.pyi
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/hfs.pyi
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/img_hash.pyi
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/intensity_transform.pyi
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ipp.pyi
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/large_kinfu.pyi
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/legacy.pyi
--rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/line_descriptor.pyi
--rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/linemod.pyi
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/load_config_py3.pyi
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/mat_wrapper.pyi
--rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/mcc.pyi
--rw-r--r--   0        0        0    59687 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ml.pyi
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/motempl.pyi
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/multicalib.pyi
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ocl.pyi
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ogl.pyi
--rw-r--r--   0        0        0    14145 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/omnidir.pyi
--rw-r--r--   0        0        0    27907 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/optflow.pyi
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/parallel.pyi
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/phase_unwrapping.pyi
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/plot.pyi
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ppf_match_3d.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/qt.pyi
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/quality.pyi
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/rapid.pyi
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/reg.pyi
--rw-r--r--   0        0        0    29883 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/rgbd.pyi
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/saliency.pyi
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/samples.pyi
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/segmentation.pyi
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/stereo.pyi
--rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/structured_light.pyi
--rw-r--r--   0        0        0    26786 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/text.pyi
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/version.pyi
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/videoio_registry.pyi
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/videostab.pyi
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/wechat_qrcode.pyi
--rw-r--r--   0        0        0    40532 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/xfeatures2d.pyi
--rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/xphoto.pyi
--rw-r--r--   0        0        0   105662 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/core.pyi
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/ie.pyi
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/oak.pyi
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/onnx.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/own.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/render.pyi
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/video.pyi
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/streaming/__init__.pyi
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/wip/__init__.pyi
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/wip/draw.pyi
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/wip/gst.pyi
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/kinfu/__init__.pyi
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/kinfu/detail.pyi
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/misc/__init__.pyi
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/misc/version.pyi
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/utils/__init__.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/utils/fs.pyi
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/utils/nested.pyi
--rw-r--r--   0        0        0    80008 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ximgproc/__init__.pyi
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ximgproc/segmentation.pyi
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/add_missing_overloads.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/generate_classes.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/generate_constants.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/generate_modules.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/merge_with_microsoft_stubs.py
--rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/processing_utils.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/undefined_to_any.py
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/LICENSE
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/README.md
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/requirements/requirements.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/__init__.pyi
+-rw-r--r--   0        0        0   165718 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/classes.pyi
+-rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/constants.pyi
+-rw-r--r--   0        0        0   529741 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/functions.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/py.typed
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/__init__.py
+-rw-r--r--   0        0        0    34376 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/aruco.pyi
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/barcode.pyi
+-rw-r--r--   0        0        0    11107 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/bgsegm.pyi
+-rw-r--r--   0        0        0    19750 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/bioinspired.pyi
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ccm.pyi
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/colored_kinfu.pyi
+-rw-r--r--   0        0        0    23759 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/cuda.pyi
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/data.pyi
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/datasets.pyi
+-rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/detail.pyi
+-rw-r--r--   0        0        0    45108 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/dnn.pyi
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/dnn_superres.pyi
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/dpm.pyi
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/dynafu.pyi
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/error.pyi
+-rw-r--r--   0        0        0    34295 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/face.pyi
+-rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/fisheye.pyi
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/flann.pyi
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ft.pyi
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/hfs.pyi
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/img_hash.pyi
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/intensity_transform.pyi
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ipp.pyi
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/large_kinfu.pyi
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/legacy.pyi
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/line_descriptor.pyi
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/linemod.pyi
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/load_config_py3.pyi
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/mat_wrapper.pyi
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/mcc.pyi
+-rw-r--r--   0        0        0    60302 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ml.pyi
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/motempl.pyi
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/multicalib.pyi
+-rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ocl.pyi
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ogl.pyi
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/omnidir.pyi
+-rw-r--r--   0        0        0    27976 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/optflow.pyi
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/parallel.pyi
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/phase_unwrapping.pyi
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/plot.pyi
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ppf_match_3d.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/qt.pyi
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/quality.pyi
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/rapid.pyi
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/reg.pyi
+-rw-r--r--   0        0        0    30043 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/rgbd.pyi
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/saliency.pyi
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/samples.pyi
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/segmentation.pyi
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/stereo.pyi
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/structured_light.pyi
+-rw-r--r--   0        0        0    26974 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/text.pyi
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/version.pyi
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/videoio_registry.pyi
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/videostab.pyi
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/wechat_qrcode.pyi
+-rw-r--r--   0        0        0    40748 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/xfeatures2d.pyi
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/xphoto.pyi
+-rw-r--r--   0        0        0   105878 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/core.pyi
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/ie.pyi
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/oak.pyi
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/onnx.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/own.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/render.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/video.pyi
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/streaming/__init__.pyi
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/__init__.pyi
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/draw.pyi
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/gst.pyi
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/kinfu/__init__.pyi
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/kinfu/detail.pyi
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/misc/__init__.pyi
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/misc/version.pyi
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/__init__.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/fs.pyi
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/nested.pyi
+-rw-r--r--   0        0        0    80287 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ximgproc/__init__.pyi
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ximgproc/segmentation.pyi
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/add_missing_overloads.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/generate_classes.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/generate_constants.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/generate_modules.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/merge_with_microsoft_stubs.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/processing_utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/undefined_to_any.py
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/README.md
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/PKG-INFO
```

### Comparing `opencv_stubs-0.0.5/.pre-commit-config.yaml` & `opencv_stubs-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/requirements/requirements-build.txt` & `opencv_stubs-0.0.6/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/requirements/requirements-dev.txt` & `opencv_stubs-0.0.6/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/classes.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/classes.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/functions.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/functions.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/__init__.py` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/aruco.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/aruco.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import builtins
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 from .. import functions as cv2
 
 rvecs: TypeAlias = Any
 detectedCorners: TypeAlias = Any
 image: TypeAlias = Any
 charucoCorners: TypeAlias = Any
@@ -609,20 +609,20 @@
     """
 
 def testCharucoCornersCollinear(board, charucoIds) -> retval:
     """
     @deprecated Use CharucoBoard::checkCharucoCornersCollinear
     """
 
-ARUCO_CCW_CENTER: int
-ARUCO_CW_TOP_LEFT_CORNER: int
-CORNER_REFINE_APRILTAG: int
-CORNER_REFINE_CONTOUR: int
-CORNER_REFINE_NONE: int
-CORNER_REFINE_SUBPIX: int
+ARUCO_CCW_CENTER: Final[int]
+ARUCO_CW_TOP_LEFT_CORNER: Final[int]
+CORNER_REFINE_APRILTAG: Final[int]
+CORNER_REFINE_CONTOUR: Final[int]
+CORNER_REFINE_NONE: Final[int]
+CORNER_REFINE_SUBPIX: Final[int]
 DICT_4X4_100: int
 DICT_4X4_1000: int
 DICT_4X4_250: int
 DICT_4X4_50: int
 DICT_5X5_100: int
 DICT_5X5_1000: int
 DICT_5X5_250: int
@@ -631,16 +631,16 @@
 DICT_6X6_1000: int
 DICT_6X6_250: int
 DICT_6X6_50: int
 DICT_7X7_100: int
 DICT_7X7_1000: int
 DICT_7X7_250: int
 DICT_7X7_50: int
-DICT_APRILTAG_16H5: int
-DICT_APRILTAG_16h5: int
-DICT_APRILTAG_25H9: int
-DICT_APRILTAG_25h9: int
+DICT_APRILTAG_16H5: Final[int]
+DICT_APRILTAG_16h5: Final[int]
+DICT_APRILTAG_25H9: Final[int]
+DICT_APRILTAG_25h9: Final[int]
 DICT_APRILTAG_36H10: int
-DICT_APRILTAG_36H11: int
+DICT_APRILTAG_36H11: Final[int]
 DICT_APRILTAG_36h10: int
-DICT_APRILTAG_36h11: int
-DICT_ARUCO_ORIGINAL: int
+DICT_APRILTAG_36h11: Final[int]
+DICT_ARUCO_ORIGINAL: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/barcode.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/barcode.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import builtins
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 decoded_info: TypeAlias = Any
 points: TypeAlias = Any
 decoded_type: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class BarcodeDetector(builtins.object):
     def decode(self, img, points) -> tuple[retval, decoded_info, decoded_type]:
         """
         @brief Decodes barcode in image once it's found by the detect() method.
         *
@@ -33,13 +32,13 @@
         * @param img grayscale or color (BGR) image containing barcode.
         * @param decoded_info UTF8-encoded output vector of string(s) or empty vector of string if the codes cannot be decoded.
         * @param decoded_type vector of BarcodeType, specifies the type of these barcodes
         * @param points optional output vector of vertices of the found  barcode rectangle. Will be empty if not found.
         """
 
 
-EAN_13: int
-EAN_8: int
-NONE: int
-UPC_A: int
-UPC_E: int
-UPC_EAN_EXTENSION: int
+EAN_13: Final[int]
+EAN_8: Final[int]
+NONE: Final[int]
+UPC_A: Final[int]
+UPC_E: Final[int]
+UPC_EAN_EXTENSION: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/bgsegm.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/bgsegm.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import builtins
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 from .. import functions as cv2
 
 gtMask: TypeAlias = Any
 fgmask: TypeAlias = Any
 backgroundImage: TypeAlias = Any
 frame: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class BackgroundSubtractorCNT(cv2.BackgroundSubtractor):
     def apply(self, image, fgmask = ..., learningRate = ...) -> fgmask:
         """"""
 
     def getBackgroundImage(self, backgroundImage = ...) -> backgroundImage:
@@ -300,9 +299,9 @@
     @param object Object image which will move slowly over the background.
     @param amplitude Amplitude of wave distortion applied to background.
     @param wavelength Length of waves in distortion applied to background.
     @param wavespeed How fast waves will move.
     @param objspeed How fast object will fly over background.
     """
 
-LSBP_CAMERA_MOTION_COMPENSATION_LK: int
-LSBP_CAMERA_MOTION_COMPENSATION_NONE: int
+LSBP_CAMERA_MOTION_COMPENSATION_LK: Final[int]
+LSBP_CAMERA_MOTION_COMPENSATION_NONE: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/bioinspired.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/bioinspired.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 outputToneMappedImage: TypeAlias = Any
 retinaOutput_parvo: TypeAlias = Any
 retinaOutput_magno: TypeAlias = Any
 transientAreas: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class Retina(cv2.Algorithm):
     def activateContoursProcessing(self, activate) -> None:
         """
         @brief Activate/desactivate the Parvocellular pathway processing (contours information extraction), by
         default, it is activated
@@ -341,10 +340,10 @@
 
 def TransientAreasSegmentationModule_create(inputSize) -> retval:
     """
     @brief allocator
         @param inputSize : size of the images input to segment (output will be the same size)
     """
 
-RETINA_COLOR_BAYER: int
-RETINA_COLOR_DIAGONAL: int
-RETINA_COLOR_RANDOM: int
+RETINA_COLOR_BAYER: Final[int]
+RETINA_COLOR_DIAGONAL: Final[int]
+RETINA_COLOR_RANDOM: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/colored_kinfu.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/colored_kinfu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/cuda.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/cuda.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 keypoints: TypeAlias = Any
 descriptors: TypeAlias = Any
 arr: TypeAlias = Any
 dst: TypeAlias = Any
 retval: TypeAlias = Any
 
@@ -822,52 +822,52 @@
 def unregisterPageLocked(m) -> None:
     """
     @brief Unmaps the memory of matrix and makes it pageable again.
 
     @param m Input matrix.
     """
 
-DEVICE_INFO_COMPUTE_MODE_DEFAULT: int
-DEVICE_INFO_COMPUTE_MODE_EXCLUSIVE: int
-DEVICE_INFO_COMPUTE_MODE_EXCLUSIVE_PROCESS: int
-DEVICE_INFO_COMPUTE_MODE_PROHIBITED: int
-DYNAMIC_PARALLELISM: int
-DeviceInfo_ComputeModeDefault: int
-DeviceInfo_ComputeModeExclusive: int
-DeviceInfo_ComputeModeExclusiveProcess: int
-DeviceInfo_ComputeModeProhibited: int
-EVENT_BLOCKING_SYNC: int
-EVENT_DEFAULT: int
-EVENT_DISABLE_TIMING: int
-EVENT_INTERPROCESS: int
-Event_BLOCKING_SYNC: int
-Event_DEFAULT: int
-Event_DISABLE_TIMING: int
-Event_INTERPROCESS: int
+DEVICE_INFO_COMPUTE_MODE_DEFAULT: Final[int]
+DEVICE_INFO_COMPUTE_MODE_EXCLUSIVE: Final[int]
+DEVICE_INFO_COMPUTE_MODE_EXCLUSIVE_PROCESS: Final[int]
+DEVICE_INFO_COMPUTE_MODE_PROHIBITED: Final[int]
+DYNAMIC_PARALLELISM: Final[int]
+DeviceInfo_ComputeModeDefault: Final[int]
+DeviceInfo_ComputeModeExclusive: Final[int]
+DeviceInfo_ComputeModeExclusiveProcess: Final[int]
+DeviceInfo_ComputeModeProhibited: Final[int]
+EVENT_BLOCKING_SYNC: Final[int]
+EVENT_DEFAULT: Final[int]
+EVENT_DISABLE_TIMING: Final[int]
+EVENT_INTERPROCESS: Final[int]
+Event_BLOCKING_SYNC: Final[int]
+Event_DEFAULT: Final[int]
+Event_DISABLE_TIMING: Final[int]
+Event_INTERPROCESS: Final[int]
 FEATURE_SET_COMPUTE_10: int
-FEATURE_SET_COMPUTE_11: int
-FEATURE_SET_COMPUTE_12: int
-FEATURE_SET_COMPUTE_13: int
+FEATURE_SET_COMPUTE_11: Final[int]
+FEATURE_SET_COMPUTE_12: Final[int]
+FEATURE_SET_COMPUTE_13: Final[int]
 FEATURE_SET_COMPUTE_20: int
-FEATURE_SET_COMPUTE_21: int
+FEATURE_SET_COMPUTE_21: Final[int]
 FEATURE_SET_COMPUTE_30: int
-FEATURE_SET_COMPUTE_32: int
-FEATURE_SET_COMPUTE_35: int
+FEATURE_SET_COMPUTE_32: Final[int]
+FEATURE_SET_COMPUTE_35: Final[int]
 FEATURE_SET_COMPUTE_50: int
-GLOBAL_ATOMICS: int
-HOST_MEM_PAGE_LOCKED: int
-HOST_MEM_SHARED: int
-HOST_MEM_WRITE_COMBINED: int
-HostMem_PAGE_LOCKED: int
-HostMem_SHARED: int
-HostMem_WRITE_COMBINED: int
-NATIVE_DOUBLE: int
-SHARED_ATOMICS: int
-SURF_CUDA_ANGLE_ROW: int
-SURF_CUDA_HESSIAN_ROW: int
-SURF_CUDA_LAPLACIAN_ROW: int
-SURF_CUDA_OCTAVE_ROW: int
-SURF_CUDA_ROWS_COUNT: int
-SURF_CUDA_SIZE_ROW: int
-SURF_CUDA_X_ROW: int
-SURF_CUDA_Y_ROW: int
-WARP_SHUFFLE_FUNCTIONS: int
+GLOBAL_ATOMICS: Final[int]
+HOST_MEM_PAGE_LOCKED: Final[int]
+HOST_MEM_SHARED: Final[int]
+HOST_MEM_WRITE_COMBINED: Final[int]
+HostMem_PAGE_LOCKED: Final[int]
+HostMem_SHARED: Final[int]
+HostMem_WRITE_COMBINED: Final[int]
+NATIVE_DOUBLE: Final[int]
+SHARED_ATOMICS: Final[int]
+SURF_CUDA_ANGLE_ROW: Final[int]
+SURF_CUDA_HESSIAN_ROW: Final[int]
+SURF_CUDA_LAPLACIAN_ROW: Final[int]
+SURF_CUDA_OCTAVE_ROW: Final[int]
+SURF_CUDA_ROWS_COUNT: Final[int]
+SURF_CUDA_SIZE_ROW: Final[int]
+SURF_CUDA_X_ROW: Final[int]
+SURF_CUDA_Y_ROW: Final[int]
+WARP_SHUFFLE_FUNCTIONS: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/detail.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/detail.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 matches_info: TypeAlias = Any
 rmats: TypeAlias = Any
 src: TypeAlias = Any
 image: TypeAlias = Any
 weight: TypeAlias = Any
 K: TypeAlias = Any
@@ -13,15 +13,14 @@
 arg1: TypeAlias = Any
 dst_mask: TypeAlias = Any
 masks: TypeAlias = Any
 weight_maps: TypeAlias = Any
 features: TypeAlias = Any
 pairwise_matches: TypeAlias = Any
 cameras: TypeAlias = Any
-
 dst: TypeAlias = Any
 retval: TypeAlias = Any
 
 class AffineBasedEstimator(Estimator):
     ...
 
 
@@ -589,133 +588,133 @@
     """
     @brief Tries to make panorama more horizontal (or vertical).
 
     @param rmats Camera rotation matrices.
     @param kind Correction kind, see detail::WaveCorrectKind.
     """
 
-ARG_KIND_GARRAY: int
-ARG_KIND_GFRAME: int
-ARG_KIND_GMAT: int
-ARG_KIND_GMATP: int
-ARG_KIND_GOBJREF: int
-ARG_KIND_GOPAQUE: int
-ARG_KIND_GSCALAR: int
-ARG_KIND_OPAQUE: int
-ARG_KIND_OPAQUE_VAL: int
-ArgKind_GARRAY: int
-ArgKind_GFRAME: int
-ArgKind_GMAT: int
-ArgKind_GMATP: int
-ArgKind_GOBJREF: int
-ArgKind_GOPAQUE: int
-ArgKind_GSCALAR: int
-ArgKind_OPAQUE: int
-ArgKind_OPAQUE_VAL: int
-BLENDER_FEATHER: int
-BLENDER_MULTI_BAND: int
-BLENDER_NO: int
-Blender_FEATHER: int
-Blender_MULTI_BAND: int
-Blender_NO: int
-CV_FEATURE_PARAMS_HAAR: int
-CV_FEATURE_PARAMS_HOG: int
-CV_FEATURE_PARAMS_LBP: int
-CvFeatureParams_HAAR: int
-CvFeatureParams_HOG: int
-CvFeatureParams_LBP: int
-DP_SEAM_FINDER_COLOR: int
-DP_SEAM_FINDER_COLOR_GRAD: int
-DpSeamFinder_COLOR: int
-DpSeamFinder_COLOR_GRAD: int
-EXPOSURE_COMPENSATOR_CHANNELS: int
-EXPOSURE_COMPENSATOR_CHANNELS_BLOCKS: int
-EXPOSURE_COMPENSATOR_GAIN: int
-EXPOSURE_COMPENSATOR_GAIN_BLOCKS: int
-EXPOSURE_COMPENSATOR_NO: int
-ExposureCompensator_CHANNELS: int
-ExposureCompensator_CHANNELS_BLOCKS: int
-ExposureCompensator_GAIN: int
-ExposureCompensator_GAIN_BLOCKS: int
-ExposureCompensator_NO: int
-GRAPH_CUT_SEAM_FINDER_BASE_COST_COLOR: int
-GRAPH_CUT_SEAM_FINDER_BASE_COST_COLOR_GRAD: int
-GraphCutSeamFinderBase_COST_COLOR: int
-GraphCutSeamFinderBase_COST_COLOR_GRAD: int
-OPAQUE_KIND_CV_BOOL: int
-OPAQUE_KIND_CV_DOUBLE: int
-OPAQUE_KIND_CV_DRAW_PRIM: int
-OPAQUE_KIND_CV_FLOAT: int
-OPAQUE_KIND_CV_INT: int
-OPAQUE_KIND_CV_INT64: int
-OPAQUE_KIND_CV_MAT: int
-OPAQUE_KIND_CV_POINT: int
-OPAQUE_KIND_CV_POINT2F: int
-OPAQUE_KIND_CV_POINT3F: int
-OPAQUE_KIND_CV_RECT: int
-OPAQUE_KIND_CV_SCALAR: int
-OPAQUE_KIND_CV_SIZE: int
-OPAQUE_KIND_CV_STRING: int
-OPAQUE_KIND_CV_UINT64: int
-OPAQUE_KIND_CV_UNKNOWN: int
-OpaqueKind_CV_BOOL: int
-OpaqueKind_CV_DOUBLE: int
-OpaqueKind_CV_DRAW_PRIM: int
-OpaqueKind_CV_FLOAT: int
-OpaqueKind_CV_INT: int
-OpaqueKind_CV_INT64: int
-OpaqueKind_CV_MAT: int
-OpaqueKind_CV_POINT: int
-OpaqueKind_CV_POINT2F: int
-OpaqueKind_CV_POINT3F: int
-OpaqueKind_CV_RECT: int
-OpaqueKind_CV_SCALAR: int
-OpaqueKind_CV_SIZE: int
-OpaqueKind_CV_STRING: int
-OpaqueKind_CV_UINT64: int
-OpaqueKind_CV_UNKNOWN: int
-SEAM_FINDER_DP_SEAM: int
-SEAM_FINDER_NO: int
-SEAM_FINDER_VORONOI_SEAM: int
-SeamFinder_DP_SEAM: int
-SeamFinder_NO: int
-SeamFinder_VORONOI_SEAM: int
-TEST_CUSTOM: int
-TEST_EQ: int
-TEST_GE: int
-TEST_GT: int
-TEST_LE: int
-TEST_LT: int
-TEST_NE: int
-TIMELAPSER_AS_IS: int
-TIMELAPSER_CROP: int
-TRACKER_CONTRIB_SAMPLER_CSC_MODE_DETECT: int
-TRACKER_CONTRIB_SAMPLER_CSC_MODE_INIT_NEG: int
-TRACKER_CONTRIB_SAMPLER_CSC_MODE_INIT_POS: int
-TRACKER_CONTRIB_SAMPLER_CSC_MODE_TRACK_NEG: int
-TRACKER_CONTRIB_SAMPLER_CSC_MODE_TRACK_POS: int
-TRACKER_SAMPLER_CSC_MODE_DETECT: int
-TRACKER_SAMPLER_CSC_MODE_INIT_NEG: int
-TRACKER_SAMPLER_CSC_MODE_INIT_POS: int
-TRACKER_SAMPLER_CSC_MODE_TRACK_NEG: int
-TRACKER_SAMPLER_CSC_MODE_TRACK_POS: int
-TRACKER_SAMPLER_CS_MODE_CLASSIFY: int
-TRACKER_SAMPLER_CS_MODE_NEGATIVE: int
-TRACKER_SAMPLER_CS_MODE_POSITIVE: int
-Timelapser_AS_IS: int
-Timelapser_CROP: int
-TrackerContribSamplerCSC_MODE_DETECT: int
-TrackerContribSamplerCSC_MODE_INIT_NEG: int
-TrackerContribSamplerCSC_MODE_INIT_POS: int
-TrackerContribSamplerCSC_MODE_TRACK_NEG: int
-TrackerContribSamplerCSC_MODE_TRACK_POS: int
-TrackerSamplerCSC_MODE_DETECT: int
-TrackerSamplerCSC_MODE_INIT_NEG: int
-TrackerSamplerCSC_MODE_INIT_POS: int
-TrackerSamplerCSC_MODE_TRACK_NEG: int
-TrackerSamplerCSC_MODE_TRACK_POS: int
-TrackerSamplerCS_MODE_CLASSIFY: int
-TrackerSamplerCS_MODE_NEGATIVE: int
-TrackerSamplerCS_MODE_POSITIVE: int
-WAVE_CORRECT_AUTO: int
-WAVE_CORRECT_HORIZ: int
-WAVE_CORRECT_VERT: int
+ARG_KIND_GARRAY: Final[int]
+ARG_KIND_GFRAME: Final[int]
+ARG_KIND_GMAT: Final[int]
+ARG_KIND_GMATP: Final[int]
+ARG_KIND_GOBJREF: Final[int]
+ARG_KIND_GOPAQUE: Final[int]
+ARG_KIND_GSCALAR: Final[int]
+ARG_KIND_OPAQUE: Final[int]
+ARG_KIND_OPAQUE_VAL: Final[int]
+ArgKind_GARRAY: Final[int]
+ArgKind_GFRAME: Final[int]
+ArgKind_GMAT: Final[int]
+ArgKind_GMATP: Final[int]
+ArgKind_GOBJREF: Final[int]
+ArgKind_GOPAQUE: Final[int]
+ArgKind_GSCALAR: Final[int]
+ArgKind_OPAQUE: Final[int]
+ArgKind_OPAQUE_VAL: Final[int]
+BLENDER_FEATHER: Final[int]
+BLENDER_MULTI_BAND: Final[int]
+BLENDER_NO: Final[int]
+Blender_FEATHER: Final[int]
+Blender_MULTI_BAND: Final[int]
+Blender_NO: Final[int]
+CV_FEATURE_PARAMS_HAAR: Final[int]
+CV_FEATURE_PARAMS_HOG: Final[int]
+CV_FEATURE_PARAMS_LBP: Final[int]
+CvFeatureParams_HAAR: Final[int]
+CvFeatureParams_HOG: Final[int]
+CvFeatureParams_LBP: Final[int]
+DP_SEAM_FINDER_COLOR: Final[int]
+DP_SEAM_FINDER_COLOR_GRAD: Final[int]
+DpSeamFinder_COLOR: Final[int]
+DpSeamFinder_COLOR_GRAD: Final[int]
+EXPOSURE_COMPENSATOR_CHANNELS: Final[int]
+EXPOSURE_COMPENSATOR_CHANNELS_BLOCKS: Final[int]
+EXPOSURE_COMPENSATOR_GAIN: Final[int]
+EXPOSURE_COMPENSATOR_GAIN_BLOCKS: Final[int]
+EXPOSURE_COMPENSATOR_NO: Final[int]
+ExposureCompensator_CHANNELS: Final[int]
+ExposureCompensator_CHANNELS_BLOCKS: Final[int]
+ExposureCompensator_GAIN: Final[int]
+ExposureCompensator_GAIN_BLOCKS: Final[int]
+ExposureCompensator_NO: Final[int]
+GRAPH_CUT_SEAM_FINDER_BASE_COST_COLOR: Final[int]
+GRAPH_CUT_SEAM_FINDER_BASE_COST_COLOR_GRAD: Final[int]
+GraphCutSeamFinderBase_COST_COLOR: Final[int]
+GraphCutSeamFinderBase_COST_COLOR_GRAD: Final[int]
+OPAQUE_KIND_CV_BOOL: Final[int]
+OPAQUE_KIND_CV_DOUBLE: Final[int]
+OPAQUE_KIND_CV_DRAW_PRIM: Final[int]
+OPAQUE_KIND_CV_FLOAT: Final[int]
+OPAQUE_KIND_CV_INT: Final[int]
+OPAQUE_KIND_CV_INT64: Final[int]
+OPAQUE_KIND_CV_MAT: Final[int]
+OPAQUE_KIND_CV_POINT: Final[int]
+OPAQUE_KIND_CV_POINT2F: Final[int]
+OPAQUE_KIND_CV_POINT3F: Final[int]
+OPAQUE_KIND_CV_RECT: Final[int]
+OPAQUE_KIND_CV_SCALAR: Final[int]
+OPAQUE_KIND_CV_SIZE: Final[int]
+OPAQUE_KIND_CV_STRING: Final[int]
+OPAQUE_KIND_CV_UINT64: Final[int]
+OPAQUE_KIND_CV_UNKNOWN: Final[int]
+OpaqueKind_CV_BOOL: Final[int]
+OpaqueKind_CV_DOUBLE: Final[int]
+OpaqueKind_CV_DRAW_PRIM: Final[int]
+OpaqueKind_CV_FLOAT: Final[int]
+OpaqueKind_CV_INT: Final[int]
+OpaqueKind_CV_INT64: Final[int]
+OpaqueKind_CV_MAT: Final[int]
+OpaqueKind_CV_POINT: Final[int]
+OpaqueKind_CV_POINT2F: Final[int]
+OpaqueKind_CV_POINT3F: Final[int]
+OpaqueKind_CV_RECT: Final[int]
+OpaqueKind_CV_SCALAR: Final[int]
+OpaqueKind_CV_SIZE: Final[int]
+OpaqueKind_CV_STRING: Final[int]
+OpaqueKind_CV_UINT64: Final[int]
+OpaqueKind_CV_UNKNOWN: Final[int]
+SEAM_FINDER_DP_SEAM: Final[int]
+SEAM_FINDER_NO: Final[int]
+SEAM_FINDER_VORONOI_SEAM: Final[int]
+SeamFinder_DP_SEAM: Final[int]
+SeamFinder_NO: Final[int]
+SeamFinder_VORONOI_SEAM: Final[int]
+TEST_CUSTOM: Final[int]
+TEST_EQ: Final[int]
+TEST_GE: Final[int]
+TEST_GT: Final[int]
+TEST_LE: Final[int]
+TEST_LT: Final[int]
+TEST_NE: Final[int]
+TIMELAPSER_AS_IS: Final[int]
+TIMELAPSER_CROP: Final[int]
+TRACKER_CONTRIB_SAMPLER_CSC_MODE_DETECT: Final[int]
+TRACKER_CONTRIB_SAMPLER_CSC_MODE_INIT_NEG: Final[int]
+TRACKER_CONTRIB_SAMPLER_CSC_MODE_INIT_POS: Final[int]
+TRACKER_CONTRIB_SAMPLER_CSC_MODE_TRACK_NEG: Final[int]
+TRACKER_CONTRIB_SAMPLER_CSC_MODE_TRACK_POS: Final[int]
+TRACKER_SAMPLER_CSC_MODE_DETECT: Final[int]
+TRACKER_SAMPLER_CSC_MODE_INIT_NEG: Final[int]
+TRACKER_SAMPLER_CSC_MODE_INIT_POS: Final[int]
+TRACKER_SAMPLER_CSC_MODE_TRACK_NEG: Final[int]
+TRACKER_SAMPLER_CSC_MODE_TRACK_POS: Final[int]
+TRACKER_SAMPLER_CS_MODE_CLASSIFY: Final[int]
+TRACKER_SAMPLER_CS_MODE_NEGATIVE: Final[int]
+TRACKER_SAMPLER_CS_MODE_POSITIVE: Final[int]
+Timelapser_AS_IS: Final[int]
+Timelapser_CROP: Final[int]
+TrackerContribSamplerCSC_MODE_DETECT: Final[int]
+TrackerContribSamplerCSC_MODE_INIT_NEG: Final[int]
+TrackerContribSamplerCSC_MODE_INIT_POS: Final[int]
+TrackerContribSamplerCSC_MODE_TRACK_NEG: Final[int]
+TrackerContribSamplerCSC_MODE_TRACK_POS: Final[int]
+TrackerSamplerCSC_MODE_DETECT: Final[int]
+TrackerSamplerCSC_MODE_INIT_NEG: Final[int]
+TrackerSamplerCSC_MODE_INIT_POS: Final[int]
+TrackerSamplerCSC_MODE_TRACK_NEG: Final[int]
+TrackerSamplerCSC_MODE_TRACK_POS: Final[int]
+TrackerSamplerCS_MODE_CLASSIFY: Final[int]
+TrackerSamplerCS_MODE_NEGATIVE: Final[int]
+TrackerSamplerCS_MODE_POSITIVE: Final[int]
+WAVE_CORRECT_AUTO: Final[int]
+WAVE_CORRECT_HORIZ: Final[int]
+WAVE_CORRECT_VERT: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/dnn.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/dnn.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 timings: TypeAlias = Any
 layersTypes: TypeAlias = Any
 images_: TypeAlias = Any
 inLayersShapes: TypeAlias = Any
@@ -23,15 +23,14 @@
 boxes: TypeAlias = Any
 conf: TypeAlias = Any
 outLayersShapes: TypeAlias = Any
 mask: TypeAlias = Any
 indices: TypeAlias = Any
 classIds: TypeAlias = Any
 results: TypeAlias = Any
-
 dst: TypeAlias = Any
 retval: TypeAlias = Any
 
 class ClassificationModel(Model):
     def classify(self, frame) -> tuple[classId, conf]:
         """
         @overload
@@ -976,30 +975,30 @@
     @brief Create a text representation for a binary network stored in protocol buffer format.
          *  @param[in] model  A path to binary network.
          *  @param[in] output A path to output text file to be created.
          *
          *  @note To reduce output file size, trained weights are not included.
     """
 
-DNN_BACKEND_CANN: int
-DNN_BACKEND_CUDA: int
-DNN_BACKEND_DEFAULT: int
-DNN_BACKEND_HALIDE: int
-DNN_BACKEND_INFERENCE_ENGINE: int
-DNN_BACKEND_OPENCV: int
-DNN_BACKEND_TIMVX: int
-DNN_BACKEND_VKCOM: int
-DNN_BACKEND_WEBNN: int
-DNN_TARGET_CPU: int
-DNN_TARGET_CUDA: int
-DNN_TARGET_CUDA_FP16: int
-DNN_TARGET_FPGA: int
-DNN_TARGET_HDDL: int
-DNN_TARGET_MYRIAD: int
-DNN_TARGET_NPU: int
-DNN_TARGET_OPENCL: int
-DNN_TARGET_OPENCL_FP16: int
-DNN_TARGET_VULKAN: int
-SOFT_NMSMETHOD_SOFTNMS_GAUSSIAN: int
-SOFT_NMSMETHOD_SOFTNMS_LINEAR: int
-SoftNMSMethod_SOFTNMS_GAUSSIAN: int
-SoftNMSMethod_SOFTNMS_LINEAR: int
+DNN_BACKEND_CANN: Final[int]
+DNN_BACKEND_CUDA: Final[int]
+DNN_BACKEND_DEFAULT: Final[int]
+DNN_BACKEND_HALIDE: Final[int]
+DNN_BACKEND_INFERENCE_ENGINE: Final[int]
+DNN_BACKEND_OPENCV: Final[int]
+DNN_BACKEND_TIMVX: Final[int]
+DNN_BACKEND_VKCOM: Final[int]
+DNN_BACKEND_WEBNN: Final[int]
+DNN_TARGET_CPU: Final[int]
+DNN_TARGET_CUDA: Final[int]
+DNN_TARGET_CUDA_FP16: Final[int]
+DNN_TARGET_FPGA: Final[int]
+DNN_TARGET_HDDL: Final[int]
+DNN_TARGET_MYRIAD: Final[int]
+DNN_TARGET_NPU: Final[int]
+DNN_TARGET_OPENCL: Final[int]
+DNN_TARGET_OPENCL_FP16: Final[int]
+DNN_TARGET_VULKAN: Final[int]
+SOFT_NMSMETHOD_SOFTNMS_GAUSSIAN: Final[int]
+SOFT_NMSMETHOD_SOFTNMS_LINEAR: Final[int]
+SoftNMSMethod_SOFTNMS_GAUSSIAN: Final[int]
+SoftNMSMethod_SOFTNMS_LINEAR: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/dnn_superres.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/dnn_superres.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/dynafu.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/dynafu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/face.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/face.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/fisheye.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/fisheye.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 rvecs: TypeAlias = Any
 K2: TypeAlias = Any
 D1: TypeAlias = Any
 R1: TypeAlias = Any
 map1: TypeAlias = Any
 T: TypeAlias = Any
@@ -456,19 +456,19 @@
         @param R Rectification transformation in the object space: 3x3 1-channel, or vector: 3x1/1x3
         1-channel or 1x1 3-channel
         @param P New camera intrinsic matrix (3x3) or new projection matrix (3x4)
         @param criteria Termination criteria
         @param undistorted Output array of image points, 1xN/Nx1 2-channel, or vector\<Point2f\> .
     """
 
-CALIB_CHECK_COND: int
-CALIB_FIX_FOCAL_LENGTH: int
-CALIB_FIX_INTRINSIC: int
-CALIB_FIX_K1: int
-CALIB_FIX_K2: int
-CALIB_FIX_K3: int
-CALIB_FIX_K4: int
-CALIB_FIX_PRINCIPAL_POINT: int
-CALIB_FIX_SKEW: int
-CALIB_RECOMPUTE_EXTRINSIC: int
-CALIB_USE_INTRINSIC_GUESS: int
-CALIB_ZERO_DISPARITY: int
+CALIB_CHECK_COND: Final[int]
+CALIB_FIX_FOCAL_LENGTH: Final[int]
+CALIB_FIX_INTRINSIC: Final[int]
+CALIB_FIX_K1: Final[int]
+CALIB_FIX_K2: Final[int]
+CALIB_FIX_K3: Final[int]
+CALIB_FIX_K4: Final[int]
+CALIB_FIX_PRINCIPAL_POINT: Final[int]
+CALIB_FIX_SKEW: Final[int]
+CALIB_RECOMPUTE_EXTRINSIC: Final[int]
+CALIB_USE_INTRINSIC_GUESS: Final[int]
+CALIB_ZERO_DISPARITY: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/flann.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/flann.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import builtins
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 indices: TypeAlias = Any
 dists: TypeAlias = Any
 
 retval: TypeAlias = Any
 
 class Index(builtins.object):
@@ -28,18 +28,18 @@
     def release(self) -> None:
         """"""
 
     def save(self, filename) -> None:
         """"""
 
 
-FLANN_INDEX_TYPE_16S: int
-FLANN_INDEX_TYPE_16U: int
-FLANN_INDEX_TYPE_32F: int
-FLANN_INDEX_TYPE_32S: int
-FLANN_INDEX_TYPE_64F: int
-FLANN_INDEX_TYPE_8S: int
-FLANN_INDEX_TYPE_8U: int
-FLANN_INDEX_TYPE_ALGORITHM: int
-FLANN_INDEX_TYPE_BOOL: int
-FLANN_INDEX_TYPE_STRING: int
-LAST_VALUE_FLANN_INDEX_TYPE: int
+FLANN_INDEX_TYPE_16S: Final[int]
+FLANN_INDEX_TYPE_16U: Final[int]
+FLANN_INDEX_TYPE_32F: Final[int]
+FLANN_INDEX_TYPE_32S: Final[int]
+FLANN_INDEX_TYPE_64F: Final[int]
+FLANN_INDEX_TYPE_8S: Final[int]
+FLANN_INDEX_TYPE_8U: Final[int]
+FLANN_INDEX_TYPE_ALGORITHM: Final[int]
+FLANN_INDEX_TYPE_BOOL: Final[int]
+FLANN_INDEX_TYPE_STRING: Final[int]
+LAST_VALUE_FLANN_INDEX_TYPE: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/ft.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/ft.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 c01: TypeAlias = Any
 components: TypeAlias = Any
 output: TypeAlias = Any
 maskOutput: TypeAlias = Any
 c00: TypeAlias = Any
 kernel: TypeAlias = Any
 matrix: TypeAlias = Any
 c10: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 @overload
 def FT02D_FL_process(matrix, radius, output = ...) -> output:
     """
     @brief Sligtly less accurate version of \f$F^0\f$-transfrom computation optimized for higher speed. The methods counts with linear basic function.
         @param matrix Input 3 channels matrix.
@@ -261,12 +260,12 @@
 def inpaint(image, mask, radius, function, algorithm, output = ...) -> output:
     """
 
         @note
             The algorithms are described in paper @cite Perf:rec.
     """
 
-ITERATIVE: int
-LINEAR: int
-MULTI_STEP: int
-ONE_STEP: int
-SINUS: int
+ITERATIVE: Final[int]
+LINEAR: Final[int]
+MULTI_STEP: Final[int]
+ONE_STEP: Final[int]
+SINUS: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/hfs.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/hfs.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/img_hash.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/img_hash.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 outputArr: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class AverageHash(ImgHashBase):
     def create(self) -> retval:
         """"""
 
 
@@ -202,8 +201,8 @@
     """
         @param outputArr Hash value of input
         @param sigma Gaussian kernel standard deviation
         @param numOfAngleLine The number of angles to consider
     """
 
 BLOCK_MEAN_HASH_MODE_0: int
-BLOCK_MEAN_HASH_MODE_1: int
+BLOCK_MEAN_HASH_MODE_1: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/intensity_transform.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/intensity_transform.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/large_kinfu.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/large_kinfu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/legacy.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/legacy.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/line_descriptor.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/line_descriptor.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/linemod.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/linemod.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/mcc.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/mcc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import builtins
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 from .. import functions as cv2
 
 img: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class CChecker(builtins.object):
     def getBox(self) -> retval:
         """"""
 
     def getCenter(self) -> retval:
@@ -181,10 +180,10 @@
     """
 
 def DetectorParameters_create() -> retval:
     """
         .
     """
 
-MCC24: int
+MCC24: Final[int]
 SG140: int
-VINYL18: int
+VINYL18: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/ml.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/ml.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 outputs: TypeAlias = Any
 svidx: TypeAlias = Any
 neighborResponses: TypeAlias = Any
 covs: TypeAlias = Any
@@ -11,15 +11,14 @@
 probs: TypeAlias = Any
 outputProbs: TypeAlias = Any
 dist: TypeAlias = Any
 alpha: TypeAlias = Any
 labels: TypeAlias = Any
 results: TypeAlias = Any
 logLikelihoods: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class ANN_MLP(StatModel):
     def getAnnealCoolingRatio(self) -> retval:
         """
         @see setAnnealCoolingRatio
         """
@@ -1597,94 +1596,94 @@
 def TrainData_getSubVector(vec, idx) -> retval:
     """
     @brief Extract from 1D vector elements specified by passed indexes.
         @param vec input vector (supported types: CV_32S, CV_32F, CV_64F)
         @param idx 1D index vector
     """
 
-ANN_MLP_ANNEAL: int
-ANN_MLP_BACKPROP: int
-ANN_MLP_GAUSSIAN: int
-ANN_MLP_IDENTITY: int
-ANN_MLP_LEAKYRELU: int
-ANN_MLP_NO_INPUT_SCALE: int
-ANN_MLP_NO_OUTPUT_SCALE: int
-ANN_MLP_RELU: int
-ANN_MLP_RPROP: int
-ANN_MLP_SIGMOID_SYM: int
-ANN_MLP_UPDATE_WEIGHTS: int
-BOOST_DISCRETE: int
-BOOST_GENTLE: int
-BOOST_LOGIT: int
-BOOST_REAL: int
-Boost_DISCRETE: int
-Boost_GENTLE: int
-Boost_LOGIT: int
-Boost_REAL: int
-COL_SAMPLE: int
-DTREES_PREDICT_AUTO: int
-DTREES_PREDICT_MASK: int
-DTREES_PREDICT_MAX_VOTE: int
-DTREES_PREDICT_SUM: int
-DTrees_PREDICT_AUTO: int
-DTrees_PREDICT_MASK: int
-DTrees_PREDICT_MAX_VOTE: int
-DTrees_PREDICT_SUM: int
-EM_COV_MAT_DEFAULT: int
-EM_COV_MAT_DIAGONAL: int
-EM_COV_MAT_GENERIC: int
-EM_COV_MAT_SPHERICAL: int
-EM_DEFAULT_MAX_ITERS: int
-EM_DEFAULT_NCLUSTERS: int
-EM_START_AUTO_STEP: int
-EM_START_E_STEP: int
-EM_START_M_STEP: int
-KNEAREST_BRUTE_FORCE: int
-KNEAREST_KDTREE: int
-KNearest_BRUTE_FORCE: int
-KNearest_KDTREE: int
-LOGISTIC_REGRESSION_BATCH: int
-LOGISTIC_REGRESSION_MINI_BATCH: int
-LOGISTIC_REGRESSION_REG_DISABLE: int
-LOGISTIC_REGRESSION_REG_L1: int
-LOGISTIC_REGRESSION_REG_L2: int
-LogisticRegression_BATCH: int
-LogisticRegression_MINI_BATCH: int
-LogisticRegression_REG_DISABLE: int
-LogisticRegression_REG_L1: int
-LogisticRegression_REG_L2: int
-ROW_SAMPLE: int
-STAT_MODEL_COMPRESSED_INPUT: int
-STAT_MODEL_PREPROCESSED_INPUT: int
-STAT_MODEL_RAW_OUTPUT: int
-STAT_MODEL_UPDATE_MODEL: int
-SVMSGD_ASGD: int
-SVMSGD_HARD_MARGIN: int
-SVMSGD_SGD: int
-SVMSGD_SOFT_MARGIN: int
-SVM_C: int
-SVM_CHI2: int
-SVM_COEF: int
-SVM_CUSTOM: int
-SVM_C_SVC: int
-SVM_DEGREE: int
-SVM_EPS_SVR: int
-SVM_GAMMA: int
-SVM_INTER: int
-SVM_LINEAR: int
-SVM_NU: int
-SVM_NU_SVC: int
-SVM_NU_SVR: int
-SVM_ONE_CLASS: int
-SVM_P: int
-SVM_POLY: int
-SVM_RBF: int
-SVM_SIGMOID: int
-StatModel_COMPRESSED_INPUT: int
-StatModel_PREPROCESSED_INPUT: int
-StatModel_RAW_OUTPUT: int
-StatModel_UPDATE_MODEL: int
-TEST_ERROR: int
-TRAIN_ERROR: int
-VAR_CATEGORICAL: int
-VAR_NUMERICAL: int
-VAR_ORDERED: int
+ANN_MLP_ANNEAL: Final[int]
+ANN_MLP_BACKPROP: Final[int]
+ANN_MLP_GAUSSIAN: Final[int]
+ANN_MLP_IDENTITY: Final[int]
+ANN_MLP_LEAKYRELU: Final[int]
+ANN_MLP_NO_INPUT_SCALE: Final[int]
+ANN_MLP_NO_OUTPUT_SCALE: Final[int]
+ANN_MLP_RELU: Final[int]
+ANN_MLP_RPROP: Final[int]
+ANN_MLP_SIGMOID_SYM: Final[int]
+ANN_MLP_UPDATE_WEIGHTS: Final[int]
+BOOST_DISCRETE: Final[int]
+BOOST_GENTLE: Final[int]
+BOOST_LOGIT: Final[int]
+BOOST_REAL: Final[int]
+Boost_DISCRETE: Final[int]
+Boost_GENTLE: Final[int]
+Boost_LOGIT: Final[int]
+Boost_REAL: Final[int]
+COL_SAMPLE: Final[int]
+DTREES_PREDICT_AUTO: Final[int]
+DTREES_PREDICT_MASK: Final[int]
+DTREES_PREDICT_MAX_VOTE: Final[int]
+DTREES_PREDICT_SUM: Final[int]
+DTrees_PREDICT_AUTO: Final[int]
+DTrees_PREDICT_MASK: Final[int]
+DTrees_PREDICT_MAX_VOTE: Final[int]
+DTrees_PREDICT_SUM: Final[int]
+EM_COV_MAT_DEFAULT: Final[int]
+EM_COV_MAT_DIAGONAL: Final[int]
+EM_COV_MAT_GENERIC: Final[int]
+EM_COV_MAT_SPHERICAL: Final[int]
+EM_DEFAULT_MAX_ITERS: Final[int]
+EM_DEFAULT_NCLUSTERS: Final[int]
+EM_START_AUTO_STEP: Final[int]
+EM_START_E_STEP: Final[int]
+EM_START_M_STEP: Final[int]
+KNEAREST_BRUTE_FORCE: Final[int]
+KNEAREST_KDTREE: Final[int]
+KNearest_BRUTE_FORCE: Final[int]
+KNearest_KDTREE: Final[int]
+LOGISTIC_REGRESSION_BATCH: Final[int]
+LOGISTIC_REGRESSION_MINI_BATCH: Final[int]
+LOGISTIC_REGRESSION_REG_DISABLE: Final[int]
+LOGISTIC_REGRESSION_REG_L1: Final[int]
+LOGISTIC_REGRESSION_REG_L2: Final[int]
+LogisticRegression_BATCH: Final[int]
+LogisticRegression_MINI_BATCH: Final[int]
+LogisticRegression_REG_DISABLE: Final[int]
+LogisticRegression_REG_L1: Final[int]
+LogisticRegression_REG_L2: Final[int]
+ROW_SAMPLE: Final[int]
+STAT_MODEL_COMPRESSED_INPUT: Final[int]
+STAT_MODEL_PREPROCESSED_INPUT: Final[int]
+STAT_MODEL_RAW_OUTPUT: Final[int]
+STAT_MODEL_UPDATE_MODEL: Final[int]
+SVMSGD_ASGD: Final[int]
+SVMSGD_HARD_MARGIN: Final[int]
+SVMSGD_SGD: Final[int]
+SVMSGD_SOFT_MARGIN: Final[int]
+SVM_C: Final[int]
+SVM_CHI2: Final[int]
+SVM_COEF: Final[int]
+SVM_CUSTOM: Final[int]
+SVM_C_SVC: Final[int]
+SVM_DEGREE: Final[int]
+SVM_EPS_SVR: Final[int]
+SVM_GAMMA: Final[int]
+SVM_INTER: Final[int]
+SVM_LINEAR: Final[int]
+SVM_NU: Final[int]
+SVM_NU_SVC: Final[int]
+SVM_NU_SVR: Final[int]
+SVM_ONE_CLASS: Final[int]
+SVM_P: Final[int]
+SVM_POLY: Final[int]
+SVM_RBF: Final[int]
+SVM_SIGMOID: Final[int]
+StatModel_COMPRESSED_INPUT: Final[int]
+StatModel_PREPROCESSED_INPUT: Final[int]
+StatModel_RAW_OUTPUT: Final[int]
+StatModel_UPDATE_MODEL: Final[int]
+TEST_ERROR: Final[int]
+TRAIN_ERROR: Final[int]
+VAR_CATEGORICAL: Final[int]
+VAR_NUMERICAL: Final[int]
+VAR_ORDERED: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/motempl.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/motempl.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/ocl.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/ocl.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import builtins
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 retval: TypeAlias = Any
 
 class Device(builtins.object):
     def OpenCLVersion(self) -> retval:
         """"""
 
@@ -257,78 +257,78 @@
     """
 
 def useOpenCL() -> retval:
     """
         .
     """
 
-DEVICE_EXEC_KERNEL: int
-DEVICE_EXEC_NATIVE_KERNEL: int
-DEVICE_FP_CORRECTLY_ROUNDED_DIVIDE_SQRT: int
-DEVICE_FP_DENORM: int
-DEVICE_FP_FMA: int
-DEVICE_FP_INF_NAN: int
-DEVICE_FP_ROUND_TO_INF: int
-DEVICE_FP_ROUND_TO_NEAREST: int
-DEVICE_FP_ROUND_TO_ZERO: int
-DEVICE_FP_SOFT_FLOAT: int
-DEVICE_LOCAL_IS_GLOBAL: int
-DEVICE_LOCAL_IS_LOCAL: int
-DEVICE_NO_CACHE: int
-DEVICE_NO_LOCAL_MEM: int
-DEVICE_READ_ONLY_CACHE: int
-DEVICE_READ_WRITE_CACHE: int
-DEVICE_TYPE_ACCELERATOR: int
-DEVICE_TYPE_ALL: int
-DEVICE_TYPE_CPU: int
-DEVICE_TYPE_DEFAULT: int
-DEVICE_TYPE_DGPU: int
-DEVICE_TYPE_GPU: int
-DEVICE_TYPE_IGPU: int
-DEVICE_UNKNOWN_VENDOR: int
-DEVICE_VENDOR_AMD: int
-DEVICE_VENDOR_INTEL: int
-DEVICE_VENDOR_NVIDIA: int
-Device_EXEC_KERNEL: int
-Device_EXEC_NATIVE_KERNEL: int
-Device_FP_CORRECTLY_ROUNDED_DIVIDE_SQRT: int
-Device_FP_DENORM: int
-Device_FP_FMA: int
-Device_FP_INF_NAN: int
-Device_FP_ROUND_TO_INF: int
-Device_FP_ROUND_TO_NEAREST: int
-Device_FP_ROUND_TO_ZERO: int
-Device_FP_SOFT_FLOAT: int
-Device_LOCAL_IS_GLOBAL: int
-Device_LOCAL_IS_LOCAL: int
-Device_NO_CACHE: int
-Device_NO_LOCAL_MEM: int
-Device_READ_ONLY_CACHE: int
-Device_READ_WRITE_CACHE: int
-Device_TYPE_ACCELERATOR: int
-Device_TYPE_ALL: int
-Device_TYPE_CPU: int
-Device_TYPE_DEFAULT: int
-Device_TYPE_DGPU: int
-Device_TYPE_GPU: int
-Device_TYPE_IGPU: int
-Device_UNKNOWN_VENDOR: int
-Device_VENDOR_AMD: int
-Device_VENDOR_INTEL: int
-Device_VENDOR_NVIDIA: int
-KERNEL_ARG_CONSTANT: int
-KERNEL_ARG_LOCAL: int
-KERNEL_ARG_NO_SIZE: int
-KERNEL_ARG_PTR_ONLY: int
-KERNEL_ARG_READ_ONLY: int
-KERNEL_ARG_READ_WRITE: int
-KERNEL_ARG_WRITE_ONLY: int
-KernelArg_CONSTANT: int
-KernelArg_LOCAL: int
-KernelArg_NO_SIZE: int
-KernelArg_PTR_ONLY: int
-KernelArg_READ_ONLY: int
-KernelArg_READ_WRITE: int
-KernelArg_WRITE_ONLY: int
-OCL_VECTOR_DEFAULT: int
-OCL_VECTOR_MAX: int
-OCL_VECTOR_OWN: int
+DEVICE_EXEC_KERNEL: Final[int]
+DEVICE_EXEC_NATIVE_KERNEL: Final[int]
+DEVICE_FP_CORRECTLY_ROUNDED_DIVIDE_SQRT: Final[int]
+DEVICE_FP_DENORM: Final[int]
+DEVICE_FP_FMA: Final[int]
+DEVICE_FP_INF_NAN: Final[int]
+DEVICE_FP_ROUND_TO_INF: Final[int]
+DEVICE_FP_ROUND_TO_NEAREST: Final[int]
+DEVICE_FP_ROUND_TO_ZERO: Final[int]
+DEVICE_FP_SOFT_FLOAT: Final[int]
+DEVICE_LOCAL_IS_GLOBAL: Final[int]
+DEVICE_LOCAL_IS_LOCAL: Final[int]
+DEVICE_NO_CACHE: Final[int]
+DEVICE_NO_LOCAL_MEM: Final[int]
+DEVICE_READ_ONLY_CACHE: Final[int]
+DEVICE_READ_WRITE_CACHE: Final[int]
+DEVICE_TYPE_ACCELERATOR: Final[int]
+DEVICE_TYPE_ALL: Final[int]
+DEVICE_TYPE_CPU: Final[int]
+DEVICE_TYPE_DEFAULT: Final[int]
+DEVICE_TYPE_DGPU: Final[int]
+DEVICE_TYPE_GPU: Final[int]
+DEVICE_TYPE_IGPU: Final[int]
+DEVICE_UNKNOWN_VENDOR: Final[int]
+DEVICE_VENDOR_AMD: Final[int]
+DEVICE_VENDOR_INTEL: Final[int]
+DEVICE_VENDOR_NVIDIA: Final[int]
+Device_EXEC_KERNEL: Final[int]
+Device_EXEC_NATIVE_KERNEL: Final[int]
+Device_FP_CORRECTLY_ROUNDED_DIVIDE_SQRT: Final[int]
+Device_FP_DENORM: Final[int]
+Device_FP_FMA: Final[int]
+Device_FP_INF_NAN: Final[int]
+Device_FP_ROUND_TO_INF: Final[int]
+Device_FP_ROUND_TO_NEAREST: Final[int]
+Device_FP_ROUND_TO_ZERO: Final[int]
+Device_FP_SOFT_FLOAT: Final[int]
+Device_LOCAL_IS_GLOBAL: Final[int]
+Device_LOCAL_IS_LOCAL: Final[int]
+Device_NO_CACHE: Final[int]
+Device_NO_LOCAL_MEM: Final[int]
+Device_READ_ONLY_CACHE: Final[int]
+Device_READ_WRITE_CACHE: Final[int]
+Device_TYPE_ACCELERATOR: Final[int]
+Device_TYPE_ALL: Final[int]
+Device_TYPE_CPU: Final[int]
+Device_TYPE_DEFAULT: Final[int]
+Device_TYPE_DGPU: Final[int]
+Device_TYPE_GPU: Final[int]
+Device_TYPE_IGPU: Final[int]
+Device_UNKNOWN_VENDOR: Final[int]
+Device_VENDOR_AMD: Final[int]
+Device_VENDOR_INTEL: Final[int]
+Device_VENDOR_NVIDIA: Final[int]
+KERNEL_ARG_CONSTANT: Final[int]
+KERNEL_ARG_LOCAL: Final[int]
+KERNEL_ARG_NO_SIZE: Final[int]
+KERNEL_ARG_PTR_ONLY: Final[int]
+KERNEL_ARG_READ_ONLY: Final[int]
+KERNEL_ARG_READ_WRITE: Final[int]
+KERNEL_ARG_WRITE_ONLY: Final[int]
+KernelArg_CONSTANT: Final[int]
+KernelArg_LOCAL: Final[int]
+KernelArg_NO_SIZE: Final[int]
+KernelArg_PTR_ONLY: Final[int]
+KernelArg_READ_ONLY: Final[int]
+KernelArg_READ_WRITE: Final[int]
+KernelArg_WRITE_ONLY: Final[int]
+OCL_VECTOR_DEFAULT: Final[int]
+OCL_VECTOR_MAX: Final[int]
+OCL_VECTOR_OWN: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/omnidir.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/omnidir.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 rvecs: TypeAlias = Any
 K2: TypeAlias = Any
 xi2: TypeAlias = Any
 xi1: TypeAlias = Any
 disparity: TypeAlias = Any
 R1: TypeAlias = Any
@@ -26,15 +26,14 @@
 K: TypeAlias = Any
 imagePoints: TypeAlias = Any
 image2Rec: TypeAlias = Any
 pointCloud: TypeAlias = Any
 tvecs: TypeAlias = Any
 objectPoints: TypeAlias = Any
 undistorted: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 @overload
 def calibrate(objectPoints, imagePoints, size, K, xi, D, flags, criteria, rvecs = ..., tvecs = ..., idx = ...) -> tuple[retval, K, xi, D, rvecs, tvecs, idx]:
     """
     @brief Perform omnidirectional camera calibration, the default depth of outputs is CV_64F.
 
@@ -267,22 +266,22 @@
     """
 
 @overload
 def undistortPoints(distorted, K, D, xi, R, undistorted = ...) -> undistorted:
     """
     """
 
-CALIB_FIX_CENTER: int
-CALIB_FIX_GAMMA: int
-CALIB_FIX_K1: int
-CALIB_FIX_K2: int
-CALIB_FIX_P1: int
-CALIB_FIX_P2: int
-CALIB_FIX_SKEW: int
-CALIB_FIX_XI: int
-CALIB_USE_GUESS: int
-RECTIFY_CYLINDRICAL: int
-RECTIFY_LONGLATI: int
-RECTIFY_PERSPECTIVE: int
-RECTIFY_STEREOGRAPHIC: int
-XYZ: int
-XYZRGB: int
+CALIB_FIX_CENTER: Final[int]
+CALIB_FIX_GAMMA: Final[int]
+CALIB_FIX_K1: Final[int]
+CALIB_FIX_K2: Final[int]
+CALIB_FIX_P1: Final[int]
+CALIB_FIX_P2: Final[int]
+CALIB_FIX_SKEW: Final[int]
+CALIB_FIX_XI: Final[int]
+CALIB_USE_GUESS: Final[int]
+RECTIFY_CYLINDRICAL: Final[int]
+RECTIFY_LONGLATI: Final[int]
+RECTIFY_PERSPECTIVE: Final[int]
+RECTIFY_STEREOGRAPHIC: Final[int]
+XYZ: Final[int]
+XYZRGB: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/optflow.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/optflow.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 status: TypeAlias = Any
 nextPts: TypeAlias = Any
 flow: TypeAlias = Any
 err: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class DenseRLOFOpticalFlow(cv2.DenseOpticalFlow):
     def getEPICK(self) -> retval:
         """
         K is a number of nearest-neighbor matches considered, when fitting a locally affine
         *    model. Usually it should be around 128. However, lower values would make the interpolation noticeably faster.
@@ -718,16 +717,16 @@
     """
 
 def createOptFlow_SparseToDense() -> retval:
     """
         .
     """
 
-GPC_DESCRIPTOR_DCT: int
-GPC_DESCRIPTOR_WHT: int
-INTERP_EPIC: int
-INTERP_GEO: int
-INTERP_RIC: int
-SR_CROSS: int
-SR_FIXED: int
-ST_BILINEAR: int
-ST_STANDART: int
+GPC_DESCRIPTOR_DCT: Final[int]
+GPC_DESCRIPTOR_WHT: Final[int]
+INTERP_EPIC: Final[int]
+INTERP_GEO: Final[int]
+INTERP_RIC: Final[int]
+SR_CROSS: Final[int]
+SR_FIXED: Final[int]
+ST_BILINEAR: Final[int]
+ST_STANDART: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/phase_unwrapping.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/phase_unwrapping.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/plot.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/plot.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/ppf_match_3d.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/ppf_match_3d.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/quality.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/quality.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/rapid.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/rapid.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/reg.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/reg.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/rgbd.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/rgbd.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 depth: TypeAlias = Any
 mask: TypeAlias = Any
 normals: TypeAlias = Any
 out: TypeAlias = Any
 plane_coefficients: TypeAlias = Any
 Rt: TypeAlias = Any
 warpedMask: TypeAlias = Any
 points3d: TypeAlias = Any
 warpedImage: TypeAlias = Any
 registeredDepth: TypeAlias = Any
 warpedDepth: TypeAlias = Any
-
 dst: TypeAlias = Any
 retval: TypeAlias = Any
 
 class DepthCleaner(cv2.Algorithm):
     def apply(self, points, depth = ...) -> depth:
         """
         Given a set of 3d points in a depth image, compute the normals at each point.
@@ -760,29 +759,29 @@
        * @param cameraMatrix Camera matrix
        * @param distCoeff Distortion coefficients
        * @param warpedImage The warped image.
        * @param warpedDepth The warped depth.
        * @param warpedMask The warped mask.
     """
 
-DEPTH_CLEANER_DEPTH_CLEANER_NIL: int
-DepthCleaner_DEPTH_CLEANER_NIL: int
-ODOMETRY_FRAME_CACHE_ALL: int
-ODOMETRY_FRAME_CACHE_DST: int
-ODOMETRY_FRAME_CACHE_SRC: int
-ODOMETRY_RIGID_BODY_MOTION: int
-ODOMETRY_ROTATION: int
-ODOMETRY_TRANSLATION: int
-OdometryFrame_CACHE_ALL: int
-OdometryFrame_CACHE_DST: int
-OdometryFrame_CACHE_SRC: int
-Odometry_RIGID_BODY_MOTION: int
-Odometry_ROTATION: int
-Odometry_TRANSLATION: int
-RGBD_NORMALS_RGBD_NORMALS_METHOD_FALS: int
-RGBD_NORMALS_RGBD_NORMALS_METHOD_LINEMOD: int
-RGBD_NORMALS_RGBD_NORMALS_METHOD_SRI: int
-RGBD_PLANE_RGBD_PLANE_METHOD_DEFAULT: int
-RgbdNormals_RGBD_NORMALS_METHOD_FALS: int
-RgbdNormals_RGBD_NORMALS_METHOD_LINEMOD: int
-RgbdNormals_RGBD_NORMALS_METHOD_SRI: int
-RgbdPlane_RGBD_PLANE_METHOD_DEFAULT: int
+DEPTH_CLEANER_DEPTH_CLEANER_NIL: Final[int]
+DepthCleaner_DEPTH_CLEANER_NIL: Final[int]
+ODOMETRY_FRAME_CACHE_ALL: Final[int]
+ODOMETRY_FRAME_CACHE_DST: Final[int]
+ODOMETRY_FRAME_CACHE_SRC: Final[int]
+ODOMETRY_RIGID_BODY_MOTION: Final[int]
+ODOMETRY_ROTATION: Final[int]
+ODOMETRY_TRANSLATION: Final[int]
+OdometryFrame_CACHE_ALL: Final[int]
+OdometryFrame_CACHE_DST: Final[int]
+OdometryFrame_CACHE_SRC: Final[int]
+Odometry_RIGID_BODY_MOTION: Final[int]
+Odometry_ROTATION: Final[int]
+Odometry_TRANSLATION: Final[int]
+RGBD_NORMALS_RGBD_NORMALS_METHOD_FALS: Final[int]
+RGBD_NORMALS_RGBD_NORMALS_METHOD_LINEMOD: Final[int]
+RGBD_NORMALS_RGBD_NORMALS_METHOD_SRI: Final[int]
+RGBD_PLANE_RGBD_PLANE_METHOD_DEFAULT: Final[int]
+RgbdNormals_RGBD_NORMALS_METHOD_FALS: Final[int]
+RgbdNormals_RGBD_NORMALS_METHOD_LINEMOD: Final[int]
+RgbdNormals_RGBD_NORMALS_METHOD_SRI: Final[int]
+RgbdPlane_RGBD_PLANE_METHOD_DEFAULT: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/saliency.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/saliency.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/samples.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/samples.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/segmentation.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/segmentation.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/stereo.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/stereo.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import builtins
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 sMatches: TypeAlias = Any
 denseMatches: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class MatchQuasiDense(builtins.object):
     def apply(self, rhs) -> retval:
         """"""
 
 
@@ -72,30 +71,30 @@
 
 
 def QuasiDenseStereo_create(monoImgSize, paramFilepath = ...) -> retval:
     """
         .
     """
 
-CV_CS_CENSUS: int
-CV_DENSE_CENSUS: int
-CV_MEAN_VARIATION: int
-CV_MODIFIED_CENSUS_TRANSFORM: int
-CV_MODIFIED_CS_CENSUS: int
-CV_QUADRATIC_INTERPOLATION: int
-CV_SIMETRICV_INTERPOLATION: int
-CV_SPARSE_CENSUS: int
-CV_SPECKLE_REMOVAL_ALGORITHM: int
-CV_SPECKLE_REMOVAL_AVG_ALGORITHM: int
-CV_STAR_KERNEL: int
-STEREO_BINARY_BM_PREFILTER_NORMALIZED_RESPONSE: int
-STEREO_BINARY_BM_PREFILTER_XSOBEL: int
-STEREO_BINARY_SGBM_MODE_HH: int
-STEREO_BINARY_SGBM_MODE_SGBM: int
-STEREO_MATCHER_DISP_SCALE: int
-STEREO_MATCHER_DISP_SHIFT: int
-StereoBinaryBM_PREFILTER_NORMALIZED_RESPONSE: int
-StereoBinaryBM_PREFILTER_XSOBEL: int
-StereoBinarySGBM_MODE_HH: int
-StereoBinarySGBM_MODE_SGBM: int
-StereoMatcher_DISP_SCALE: int
-StereoMatcher_DISP_SHIFT: int
+CV_CS_CENSUS: Final[int]
+CV_DENSE_CENSUS: Final[int]
+CV_MEAN_VARIATION: Final[int]
+CV_MODIFIED_CENSUS_TRANSFORM: Final[int]
+CV_MODIFIED_CS_CENSUS: Final[int]
+CV_QUADRATIC_INTERPOLATION: Final[int]
+CV_SIMETRICV_INTERPOLATION: Final[int]
+CV_SPARSE_CENSUS: Final[int]
+CV_SPECKLE_REMOVAL_ALGORITHM: Final[int]
+CV_SPECKLE_REMOVAL_AVG_ALGORITHM: Final[int]
+CV_STAR_KERNEL: Final[int]
+STEREO_BINARY_BM_PREFILTER_NORMALIZED_RESPONSE: Final[int]
+STEREO_BINARY_BM_PREFILTER_XSOBEL: Final[int]
+STEREO_BINARY_SGBM_MODE_HH: Final[int]
+STEREO_BINARY_SGBM_MODE_SGBM: Final[int]
+STEREO_MATCHER_DISP_SCALE: Final[int]
+STEREO_MATCHER_DISP_SHIFT: Final[int]
+StereoBinaryBM_PREFILTER_NORMALIZED_RESPONSE: Final[int]
+StereoBinaryBM_PREFILTER_XSOBEL: Final[int]
+StereoBinarySGBM_MODE_HH: Final[int]
+StereoBinarySGBM_MODE_SGBM: Final[int]
+StereoMatcher_DISP_SCALE: Final[int]
+StereoMatcher_DISP_SHIFT: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/structured_light.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/structured_light.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 from .. import functions as cv2
 
 wrappedPhaseMap: TypeAlias = Any
 whiteImage: TypeAlias = Any
 patternImages: TypeAlias = Any
 disparityMap: TypeAlias = Any
 dataModulationTerm: TypeAlias = Any
 shadowMask: TypeAlias = Any
 unwrappedPhaseMap: TypeAlias = Any
 projPix: TypeAlias = Any
 matches: TypeAlias = Any
 blackImage: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class GrayCodePattern(StructuredLightPattern):
     def getImagesForShadowMasks(self, blackImage, whiteImage) -> tuple[blackImage, whiteImage]:
         """
         @brief Generates the all-black and all-white images needed for shadowMasks computation.
         *
@@ -145,11 +144,11 @@
 def SinusoidalPattern_create(parameters = ...) -> retval:
     """
     * @brief Constructor.
          * @param parameters SinusoidalPattern parameters SinusoidalPattern::Params: width, height of the projector and patterns parameters.
          *
     """
 
-DECODE_3D_UNDERWORLD: int
-FAPS: int
-FTP: int
-PSP: int
+DECODE_3D_UNDERWORLD: Final[int]
+FAPS: Final[int]
+FTP: Final[int]
+PSP: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/text.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/text.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 groups_rects: TypeAlias = Any
 confidence: TypeAlias = Any
 regions: TypeAlias = Any
 draw: TypeAlias = Any
 chainBBs: TypeAlias = Any
 result: TypeAlias = Any
 Bbox: TypeAlias = Any
 _channels: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class BaseOCR(builtins.object):
     ...
 
 
 class ERFilter(cv2.Algorithm):
@@ -523,33 +522,33 @@
     based on gradient orientations along the chain-code of its perimeter. Then, the region is classified
     using a KNN model trained with synthetic data of rendered characters with different standard font
     types.
 
     @deprecated loadOCRHMMClassifier instead
     """
 
-ERFILTER_NM_IHSGRAD: int
-ERFILTER_NM_IHSGrad: int
-ERFILTER_NM_RGBLGRAD: int
-ERFILTER_NM_RGBLGrad: int
-ERGROUPING_ORIENTATION_ANY: int
-ERGROUPING_ORIENTATION_HORIZ: int
-OCR_CNN_CLASSIFIER: int
-OCR_DECODER_VITERBI: int
-OCR_KNN_CLASSIFIER: int
-OCR_LEVEL_TEXTLINE: int
-OCR_LEVEL_WORD: int
-OEM_CUBE_ONLY: int
-OEM_DEFAULT: int
-OEM_TESSERACT_CUBE_COMBINED: int
-OEM_TESSERACT_ONLY: int
-PSM_AUTO: int
-PSM_AUTO_ONLY: int
-PSM_AUTO_OSD: int
-PSM_CIRCLE_WORD: int
-PSM_OSD_ONLY: int
-PSM_SINGLE_BLOCK: int
-PSM_SINGLE_BLOCK_VERT_TEXT: int
-PSM_SINGLE_CHAR: int
-PSM_SINGLE_COLUMN: int
-PSM_SINGLE_LINE: int
-PSM_SINGLE_WORD: int
+ERFILTER_NM_IHSGRAD: Final[int]
+ERFILTER_NM_IHSGrad: Final[int]
+ERFILTER_NM_RGBLGRAD: Final[int]
+ERFILTER_NM_RGBLGrad: Final[int]
+ERGROUPING_ORIENTATION_ANY: Final[int]
+ERGROUPING_ORIENTATION_HORIZ: Final[int]
+OCR_CNN_CLASSIFIER: Final[int]
+OCR_DECODER_VITERBI: Final[int]
+OCR_KNN_CLASSIFIER: Final[int]
+OCR_LEVEL_TEXTLINE: Final[int]
+OCR_LEVEL_WORD: Final[int]
+OEM_CUBE_ONLY: Final[int]
+OEM_DEFAULT: Final[int]
+OEM_TESSERACT_CUBE_COMBINED: Final[int]
+OEM_TESSERACT_ONLY: Final[int]
+PSM_AUTO: Final[int]
+PSM_AUTO_ONLY: Final[int]
+PSM_AUTO_OSD: Final[int]
+PSM_CIRCLE_WORD: Final[int]
+PSM_OSD_ONLY: Final[int]
+PSM_SINGLE_BLOCK: Final[int]
+PSM_SINGLE_BLOCK_VERT_TEXT: Final[int]
+PSM_SINGLE_CHAR: Final[int]
+PSM_SINGLE_COLUMN: Final[int]
+PSM_SINGLE_LINE: Final[int]
+PSM_SINGLE_WORD: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/videoio_registry.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/videoio_registry.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/wechat_qrcode.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/wechat_qrcode.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/xfeatures2d.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/xfeatures2d.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 result: TypeAlias = Any
 signature: TypeAlias = Any
 matchesGMS: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class AffineFeature2D(cv2.Feature2D):
     ...
 
 
 class BEBLID(cv2.Feature2D):
@@ -1036,41 +1035,41 @@
         @param matches1to2 Matches returned by the LOGOS matching strategy.
         @note
             This matching strategy is suitable for features matching against large scale database.
             First step consists in constructing the bag-of-words (BoW) from a representative image database.
             Image descriptors are then represented by their closest codevector (nearest BoW centroid).
     """
 
-BEBLID_SIZE_256_BITS: int
-BEBLID_SIZE_512_BITS: int
-DAISY_NRM_FULL: int
-DAISY_NRM_NONE: int
-DAISY_NRM_PARTIAL: int
-DAISY_NRM_SIFT: int
-PCTSIGNATURES_GAUSSIAN: int
-PCTSIGNATURES_HEURISTIC: int
+BEBLID_SIZE_256_BITS: Final[int]
+BEBLID_SIZE_512_BITS: Final[int]
+DAISY_NRM_FULL: Final[int]
+DAISY_NRM_NONE: Final[int]
+DAISY_NRM_PARTIAL: Final[int]
+DAISY_NRM_SIFT: Final[int]
+PCTSIGNATURES_GAUSSIAN: Final[int]
+PCTSIGNATURES_HEURISTIC: Final[int]
 PCTSIGNATURES_L0_25: int
 PCTSIGNATURES_L0_5: int
-PCTSIGNATURES_L1: int
-PCTSIGNATURES_L2: int
-PCTSIGNATURES_L2SQUARED: int
-PCTSIGNATURES_L5: int
-PCTSIGNATURES_L_INFINITY: int
-PCTSIGNATURES_MINUS: int
-PCTSIGNATURES_NORMAL: int
-PCTSIGNATURES_REGULAR: int
-PCTSIGNATURES_UNIFORM: int
-PCTSignatures_GAUSSIAN: int
-PCTSignatures_HEURISTIC: int
+PCTSIGNATURES_L1: Final[int]
+PCTSIGNATURES_L2: Final[int]
+PCTSIGNATURES_L2SQUARED: Final[int]
+PCTSIGNATURES_L5: Final[int]
+PCTSIGNATURES_L_INFINITY: Final[int]
+PCTSIGNATURES_MINUS: Final[int]
+PCTSIGNATURES_NORMAL: Final[int]
+PCTSIGNATURES_REGULAR: Final[int]
+PCTSIGNATURES_UNIFORM: Final[int]
+PCTSignatures_GAUSSIAN: Final[int]
+PCTSignatures_HEURISTIC: Final[int]
 PCTSignatures_L0_25: int
 PCTSignatures_L0_5: int
-PCTSignatures_L1: int
-PCTSignatures_L2: int
-PCTSignatures_L2SQUARED: int
-PCTSignatures_L5: int
-PCTSignatures_L_INFINITY: int
-PCTSignatures_MINUS: int
-PCTSignatures_NORMAL: int
-PCTSignatures_REGULAR: int
-PCTSignatures_UNIFORM: int
-TEBLID_SIZE_256_BITS: int
-TEBLID_SIZE_512_BITS: int
+PCTSignatures_L1: Final[int]
+PCTSignatures_L2: Final[int]
+PCTSignatures_L2SQUARED: Final[int]
+PCTSignatures_L5: Final[int]
+PCTSignatures_L_INFINITY: Final[int]
+PCTSignatures_MINUS: Final[int]
+PCTSignatures_NORMAL: Final[int]
+PCTSignatures_REGULAR: Final[int]
+PCTSignatures_UNIFORM: Final[int]
+TEBLID_SIZE_256_BITS: Final[int]
+TEBLID_SIZE_512_BITS: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/xphoto.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/xphoto.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from .. import functions as cv2
 
 dstStep2: TypeAlias = Any
 dstStep1: TypeAlias = Any
-
 dst: TypeAlias = Any
 retval: TypeAlias = Any
 
 class GrayworldWB(WhiteBalancer):
     def getSaturationThreshold(self) -> retval:
         """
         @brief Maximum saturation for a pixel to be included in the
@@ -368,14 +367,14 @@
     See the book @cite Holzmann1988 for details.
     @param src Input three-channel or one channel image (either CV_8UC3 or CV_8UC1)
     @param dst Output image of the same size and type as src.
     @param size neighbouring size is 2-size+1
     @param dynRatio image is divided by dynRatio before histogram processing
     """
 
-BM3D_STEP1: int
-BM3D_STEP2: int
-BM3D_STEPALL: int
-HAAR: int
-INPAINT_FSR_BEST: int
-INPAINT_FSR_FAST: int
-INPAINT_SHIFTMAP: int
+BM3D_STEP1: Final[int]
+BM3D_STEP2: Final[int]
+BM3D_STEPALL: Final[int]
+HAAR: Final[int]
+INPAINT_FSR_BEST: Final[int]
+INPAINT_FSR_FAST: Final[int]
+INPAINT_SHIFTMAP: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/__init__.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from . import core, cv, ie, oak, onnx, own, render, streaming, video, wip
 
 GKernelPackage: TypeAlias = Any
-
 dst: TypeAlias = Any
 retval: TypeAlias = Any
 
 class GArray(builtins.object):
     ...
 
 
@@ -2443,39 +2442,39 @@
     \f$\texttt{dst}\rightarrow\texttt{src}\f$ ).
     @param borderMode pixel extrapolation method (#BORDER_CONSTANT or #BORDER_REPLICATE).
     @param borderValue value used in case of a constant border; by default, it equals 0.
 
     @sa  warpAffine, resize, remap, getRectSubPix, perspectiveTransform
     """
 
-CV_ANY: int
-CV_BOOL: int
-CV_DOUBLE: int
-CV_DRAW_PRIM: int
-CV_FLOAT: int
-CV_GMAT: int
-CV_INT: int
-CV_INT64: int
-CV_MAT: int
-CV_POINT: int
-CV_POINT2F: int
-CV_POINT3F: int
-CV_RECT: int
-CV_SCALAR: int
-CV_SIZE: int
-CV_STRING: int
-STEREO_OUTPUT_FORMAT_DEPTH_16F: int
-STEREO_OUTPUT_FORMAT_DEPTH_32F: int
-STEREO_OUTPUT_FORMAT_DEPTH_FLOAT16: int
-STEREO_OUTPUT_FORMAT_DEPTH_FLOAT32: int
+CV_ANY: Final[int]
+CV_BOOL: Final[int]
+CV_DOUBLE: Final[int]
+CV_DRAW_PRIM: Final[int]
+CV_FLOAT: Final[int]
+CV_GMAT: Final[int]
+CV_INT: Final[int]
+CV_INT64: Final[int]
+CV_MAT: Final[int]
+CV_POINT: Final[int]
+CV_POINT2F: Final[int]
+CV_POINT3F: Final[int]
+CV_RECT: Final[int]
+CV_SCALAR: Final[int]
+CV_SIZE: Final[int]
+CV_STRING: Final[int]
+STEREO_OUTPUT_FORMAT_DEPTH_16F: Final[int]
+STEREO_OUTPUT_FORMAT_DEPTH_32F: Final[int]
+STEREO_OUTPUT_FORMAT_DEPTH_FLOAT16: Final[int]
+STEREO_OUTPUT_FORMAT_DEPTH_FLOAT32: Final[int]
 STEREO_OUTPUT_FORMAT_DISPARITY_16Q_10_5: int
-STEREO_OUTPUT_FORMAT_DISPARITY_16Q_11_4: int
-STEREO_OUTPUT_FORMAT_DISPARITY_FIXED16_11_5: int
-STEREO_OUTPUT_FORMAT_DISPARITY_FIXED16_12_4: int
-StereoOutputFormat_DEPTH_16F: int
-StereoOutputFormat_DEPTH_32F: int
-StereoOutputFormat_DEPTH_FLOAT16: int
-StereoOutputFormat_DEPTH_FLOAT32: int
+STEREO_OUTPUT_FORMAT_DISPARITY_16Q_11_4: Final[int]
+STEREO_OUTPUT_FORMAT_DISPARITY_FIXED16_11_5: Final[int]
+STEREO_OUTPUT_FORMAT_DISPARITY_FIXED16_12_4: Final[int]
+StereoOutputFormat_DEPTH_16F: Final[int]
+StereoOutputFormat_DEPTH_32F: Final[int]
+StereoOutputFormat_DEPTH_FLOAT16: Final[int]
+StereoOutputFormat_DEPTH_FLOAT32: Final[int]
 StereoOutputFormat_DISPARITY_16Q_10_5: int
-StereoOutputFormat_DISPARITY_16Q_11_4: int
-StereoOutputFormat_DISPARITY_FIXED16_11_5: int
-StereoOutputFormat_DISPARITY_FIXED16_12_4: int
+StereoOutputFormat_DISPARITY_16Q_11_4: Final[int]
+StereoOutputFormat_DISPARITY_FIXED16_11_5: Final[int]
+StereoOutputFormat_DISPARITY_FIXED16_12_4: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/oak.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/oak.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from typing import Final
 
-COLOR_CAMERA_PARAMS_BOARD_SOCKET_BGR: int
-COLOR_CAMERA_PARAMS_BOARD_SOCKET_RGB: int
+COLOR_CAMERA_PARAMS_BOARD_SOCKET_BGR: Final[int]
+COLOR_CAMERA_PARAMS_BOARD_SOCKET_RGB: Final[int]
 COLOR_CAMERA_PARAMS_RESOLUTION_THE_1080_P: int
-ColorCameraParams_BoardSocket_BGR: int
-ColorCameraParams_BoardSocket_RGB: int
+ColorCameraParams_BoardSocket_BGR: Final[int]
+ColorCameraParams_BoardSocket_RGB: Final[int]
 ColorCameraParams_Resolution_THE_1080_P: int
-ENCODER_CONFIG_PROFILE_H264_BASELINE: int
-ENCODER_CONFIG_PROFILE_H264_HIGH: int
-ENCODER_CONFIG_PROFILE_H264_MAIN: int
-ENCODER_CONFIG_PROFILE_H265_MAIN: int
-ENCODER_CONFIG_PROFILE_MJPEG: int
-ENCODER_CONFIG_RATE_CONTROL_MODE_CBR: int
-ENCODER_CONFIG_RATE_CONTROL_MODE_VBR: int
-EncoderConfig_Profile_H264_BASELINE: int
-EncoderConfig_Profile_H264_HIGH: int
-EncoderConfig_Profile_H264_MAIN: int
-EncoderConfig_Profile_H265_MAIN: int
-EncoderConfig_Profile_MJPEG: int
-EncoderConfig_RateControlMode_CBR: int
-EncoderConfig_RateControlMode_VBR: int
+ENCODER_CONFIG_PROFILE_H264_BASELINE: Final[int]
+ENCODER_CONFIG_PROFILE_H264_HIGH: Final[int]
+ENCODER_CONFIG_PROFILE_H264_MAIN: Final[int]
+ENCODER_CONFIG_PROFILE_H265_MAIN: Final[int]
+ENCODER_CONFIG_PROFILE_MJPEG: Final[int]
+ENCODER_CONFIG_RATE_CONTROL_MODE_CBR: Final[int]
+ENCODER_CONFIG_RATE_CONTROL_MODE_VBR: Final[int]
+EncoderConfig_Profile_H264_BASELINE: Final[int]
+EncoderConfig_Profile_H264_HIGH: Final[int]
+EncoderConfig_Profile_H264_MAIN: Final[int]
+EncoderConfig_Profile_H265_MAIN: Final[int]
+EncoderConfig_Profile_MJPEG: Final[int]
+EncoderConfig_RateControlMode_CBR: Final[int]
+EncoderConfig_RateControlMode_VBR: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/streaming/__init__.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/nested.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, TypeAlias
 
 retval: TypeAlias = Any
 
-class queue_capacity(builtins.object):
-    ...
+class ExportClassName(builtins.object):
+    def getFloatParam(self) -> retval:
+        """"""
 
+    def getIntParam(self) -> retval:
+        """"""
+
+    def create(self, params = ...) -> retval:
+        """"""
+
+    def originalName(self) -> retval:
+        """"""
+
+    class Params(builtins.object):
+        float_value: float = 3.5
+        int_value: int = 123
+
+        def __init__(self, /, *args, **kwargs):
+            """Initialize self.  See help(type(self)) for accurate signature."""
+
+        def __repr__(self, /):
+            """Return repr(self)."""
 
-def desync(g) -> retval:
-    """
-        .
-    """
 
-def seqNo(arg1) -> retval:
+def ExportClassName_create(params = ...) -> retval:
     """
         .
     """
 
-def seq_id(arg1) -> retval:
+def ExportClassName_originalName() -> retval:
     """
         .
     """
 
-@overload
-def size(src) -> retval:
+def OriginalClassName_create(params = ...) -> retval:
     """
-    @brief Gets dimensions from Mat.
-
-    @note Function textual ID is "org.opencv.streaming.size"
-
-    @param src Input tensor
-    @return Size (tensor dimensions).
+        .
     """
 
-@overload
-def size(src) -> retval:
+def OriginalClassName_originalName() -> retval:
     """
-    @overload
-    Gets dimensions from rectangle.
-
-    @note Function textual ID is "org.opencv.streaming.sizeR"
-
-    @param r Input rectangle.
-    @return Size (rectangle dimensions).
+        .
     """
 
-def timestamp(arg1) -> retval:
+def testEchoBooleanFunction(flag) -> retval:
     """
         .
     """
-
-SYNC_POLICY_DONT_SYNC: int
-SYNC_POLICY_DROP: int
-sync_policy_dont_sync: int
-sync_policy_drop: int
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/wip/__init__.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/wip/draw.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/draw.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/kinfu/__init__.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/kinfu/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import builtins
-from typing import Any, overload, TypeAlias
+from typing import Any, Final, overload, TypeAlias
 
 from . import detail
 
 normals: TypeAlias = Any
 points: TypeAlias = Any
 image: TypeAlias = Any
-
 retval: TypeAlias = Any
 
 class KinFu(builtins.object):
     def getCloud(self, points = ..., normals = ...) -> tuple[points, normals]:
         """
         @brief Gets points and normals of current 3d mesh
 
@@ -195,13 +194,13 @@
     """
 
 def makeVolume(_volumeType, _voxelSize, _pose, _raycastStepFactor, _truncDist, _maxWeight, _truncateThreshold, _resolution) -> retval:
     """
         .
     """
 
-VOLUME_TYPE_COLOREDTSDF: int
-VOLUME_TYPE_HASHTSDF: int
-VOLUME_TYPE_TSDF: int
-VolumeType_COLOREDTSDF: int
-VolumeType_HASHTSDF: int
-VolumeType_TSDF: int
+VOLUME_TYPE_COLOREDTSDF: Final[int]
+VOLUME_TYPE_HASHTSDF: Final[int]
+VOLUME_TYPE_TSDF: Final[int]
+VolumeType_COLOREDTSDF: Final[int]
+VolumeType_HASHTSDF: Final[int]
+VolumeType_TSDF: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/utils/__init__.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/ximgproc/__init__.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/ximgproc/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import builtins
-from typing import Any, TypeAlias
+from typing import Any, Final, TypeAlias
 
 import numpy as _np
 import numpy.typing as _npt
 
 from ... import functions as cv2
 from . import segmentation
 
@@ -19,15 +19,14 @@
 ellipses: TypeAlias = Any
 boxes: TypeAlias = Any
 scores: TypeAlias = Any
 qimg: TypeAlias = Any
 result: TypeAlias = Any
 qcimg: TypeAlias = Any
 _dst: TypeAlias = Any
-
 dst: TypeAlias = Any
 retval: TypeAlias = Any
 
 class AdaptiveManifoldFilter(cv2.Algorithm):
     def collectGarbage(self) -> None:
         """"""
 
@@ -1780,50 +1779,50 @@
     * @param   weightType  weightType The type of weight definition, see WMFWeightType
     * @param   mask        A 0-1 mask that has the same size with I. This mask is used to ignore the effect of some pixels. If the pixel value on mask is 0,
     *                           the pixel will be ignored when maintaining the joint-histogram. This is useful for applications like optical flow occlusion handling.
     *
     * @sa medianBlur, jointBilateralFilter
     """
 
-AM_FILTER: int
+AM_FILTER: Final[int]
 ARO_0_45: int
 ARO_315_0: int
-ARO_315_135: int
-ARO_315_45: int
-ARO_45_135: int
+ARO_315_135: Final[int]
+ARO_315_45: Final[int]
+ARO_45_135: Final[int]
 ARO_45_90: int
 ARO_90_135: int
-ARO_CTR_HOR: int
-ARO_CTR_VER: int
-BINARIZATION_NIBLACK: int
-BINARIZATION_NICK: int
-BINARIZATION_SAUVOLA: int
-BINARIZATION_WOLF: int
-DTF_IC: int
-DTF_NC: int
-DTF_RF: int
-EDGE_DRAWING_LSD: int
-EDGE_DRAWING_PREWITT: int
-EDGE_DRAWING_SCHARR: int
-EDGE_DRAWING_SOBEL: int
-EdgeDrawing_LSD: int
-EdgeDrawing_PREWITT: int
-EdgeDrawing_SCHARR: int
-EdgeDrawing_SOBEL: int
-FHT_ADD: int
-FHT_AVE: int
-FHT_MAX: int
-FHT_MIN: int
-GUIDED_FILTER: int
-HDO_DESKEW: int
-HDO_RAW: int
-MSLIC: int
-SLIC: int
-SLICO: int
-THINNING_GUOHALL: int
-THINNING_ZHANGSUEN: int
-WMF_COS: int
-WMF_EXP: int
-WMF_IV1: int
-WMF_IV2: int
-WMF_JAC: int
-WMF_OFF: int
+ARO_CTR_HOR: Final[int]
+ARO_CTR_VER: Final[int]
+BINARIZATION_NIBLACK: Final[int]
+BINARIZATION_NICK: Final[int]
+BINARIZATION_SAUVOLA: Final[int]
+BINARIZATION_WOLF: Final[int]
+DTF_IC: Final[int]
+DTF_NC: Final[int]
+DTF_RF: Final[int]
+EDGE_DRAWING_LSD: Final[int]
+EDGE_DRAWING_PREWITT: Final[int]
+EDGE_DRAWING_SCHARR: Final[int]
+EDGE_DRAWING_SOBEL: Final[int]
+EdgeDrawing_LSD: Final[int]
+EdgeDrawing_PREWITT: Final[int]
+EdgeDrawing_SCHARR: Final[int]
+EdgeDrawing_SOBEL: Final[int]
+FHT_ADD: Final[int]
+FHT_AVE: Final[int]
+FHT_MAX: Final[int]
+FHT_MIN: Final[int]
+GUIDED_FILTER: Final[int]
+HDO_DESKEW: Final[int]
+HDO_RAW: Final[int]
+MSLIC: Final[int]
+SLIC: Final[int]
+SLICO: Final[int]
+THINNING_GUOHALL: Final[int]
+THINNING_ZHANGSUEN: Final[int]
+WMF_COS: Final[int]
+WMF_EXP: Final[int]
+WMF_IV1: Final[int]
+WMF_IV2: Final[int]
+WMF_JAC: Final[int]
+WMF_OFF: Final[int]
```

### Comparing `opencv_stubs-0.0.5/src/cv2-stubs/modules/ximgproc/segmentation.pyi` & `opencv_stubs-0.0.6/src/cv2-stubs/modules/ximgproc/segmentation.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/utils/add_missing_overloads.py` & `opencv_stubs-0.0.6/utils/add_missing_overloads.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/utils/generate_classes.py` & `opencv_stubs-0.0.6/utils/generate_classes.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/utils/generate_constants.py` & `opencv_stubs-0.0.6/utils/generate_constants.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/utils/generate_modules.py` & `opencv_stubs-0.0.6/utils/generate_modules.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/utils/merge_with_microsoft_stubs.py` & `opencv_stubs-0.0.6/utils/merge_with_microsoft_stubs.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/utils/processing_utils.py` & `opencv_stubs-0.0.6/utils/processing_utils.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/utils/undefined_to_any.py` & `opencv_stubs-0.0.6/utils/undefined_to_any.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/LICENSE` & `opencv_stubs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/README.md` & `opencv_stubs-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 - `pip install opencv-stubs[opencv]`
 - `pip install opencv-stubs[opencv-contrib]`
 - `pip install opencv-stubs[opencv-headless]`
 
 
 ## Acknowledgements
 
-A stub file with all the cv2 functions can be found on the [Microsoft stubs repo](https://github.com/microsoft/python-type-stubs/tree/main/cv2). This package reused those functions and added typing.
+A stub file with opencv functions can be found on the [Microsoft stubs repo](https://github.com/microsoft/python-type-stubs/tree/main/cv2). This package reused those functions (with some added typing).
 
 
 ## TODO:
-- [ ] Fix missing "..."   (` """\n\n/"""\n    ...\n\n`)
 - [ ] Do something about `cv2.gapi.cv`, `cv2.utils.cv2` and `cv2.mat_wrapper.cv` (do not duplicate everything if possible).
 - [ ] Handle cases like `cv2.misc.version.cv2.misc.version.cv2.misc.get_ocv_version()`.
 - [ ] Only include the `opencv-contrib` specific stubs when using `opencv-stubs[opencv-contrib]`.
```

### Comparing `opencv_stubs-0.0.5/pyproject.toml` & `opencv_stubs-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.5/PKG-INFO` & `opencv_stubs-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv-stubs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unofficial stubs for the opencv-python package.
 Project-URL: Homepage, https://github.com/hoel-bagard/opencv-stubs
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/opencv-stubs/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Keywords: OpenCV,stubs
@@ -79,15 +79,14 @@
 - `pip install opencv-stubs[opencv]`
 - `pip install opencv-stubs[opencv-contrib]`
 - `pip install opencv-stubs[opencv-headless]`
 
 
 ## Acknowledgements
 
-A stub file with all the cv2 functions can be found on the [Microsoft stubs repo](https://github.com/microsoft/python-type-stubs/tree/main/cv2). This package reused those functions and added typing.
+A stub file with opencv functions can be found on the [Microsoft stubs repo](https://github.com/microsoft/python-type-stubs/tree/main/cv2). This package reused those functions (with some added typing).
 
 
 ## TODO:
-- [ ] Fix missing "..."   (` """\n\n/"""\n    ...\n\n`)
 - [ ] Do something about `cv2.gapi.cv`, `cv2.utils.cv2` and `cv2.mat_wrapper.cv` (do not duplicate everything if possible).
 - [ ] Handle cases like `cv2.misc.version.cv2.misc.version.cv2.misc.get_ocv_version()`.
 - [ ] Only include the `opencv-contrib` specific stubs when using `opencv-stubs[opencv-contrib]`.
```

