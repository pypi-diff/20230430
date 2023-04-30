# Comparing `tmp/opencv_stubs-0.0.6.tar.gz` & `tmp/opencv_stubs-0.0.7.tar.gz`

## Comparing `opencv_stubs-0.0.6.tar` & `opencv_stubs-0.0.7.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/requirements/requirements.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/__init__.pyi
--rw-r--r--   0        0        0   165718 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/classes.pyi
--rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/constants.pyi
--rw-r--r--   0        0        0   529741 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/functions.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/py.typed
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/__init__.py
--rw-r--r--   0        0        0    34376 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/aruco.pyi
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/barcode.pyi
--rw-r--r--   0        0        0    11107 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/bgsegm.pyi
--rw-r--r--   0        0        0    19750 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/bioinspired.pyi
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ccm.pyi
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/colored_kinfu.pyi
--rw-r--r--   0        0        0    23759 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/cuda.pyi
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/data.pyi
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/datasets.pyi
--rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/detail.pyi
--rw-r--r--   0        0        0    45108 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/dnn.pyi
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/dnn_superres.pyi
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/dpm.pyi
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/dynafu.pyi
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/error.pyi
--rw-r--r--   0        0        0    34295 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/face.pyi
--rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/fisheye.pyi
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/flann.pyi
--rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ft.pyi
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/hfs.pyi
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/img_hash.pyi
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/intensity_transform.pyi
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ipp.pyi
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/large_kinfu.pyi
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/legacy.pyi
--rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/line_descriptor.pyi
--rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/linemod.pyi
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/load_config_py3.pyi
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/mat_wrapper.pyi
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/mcc.pyi
--rw-r--r--   0        0        0    60302 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ml.pyi
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/motempl.pyi
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/multicalib.pyi
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ocl.pyi
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ogl.pyi
--rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/omnidir.pyi
--rw-r--r--   0        0        0    27976 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/optflow.pyi
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/parallel.pyi
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/phase_unwrapping.pyi
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/plot.pyi
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ppf_match_3d.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/qt.pyi
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/quality.pyi
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/rapid.pyi
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/reg.pyi
--rw-r--r--   0        0        0    30043 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/rgbd.pyi
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/saliency.pyi
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/samples.pyi
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/segmentation.pyi
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/stereo.pyi
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/structured_light.pyi
--rw-r--r--   0        0        0    26974 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/text.pyi
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/version.pyi
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/videoio_registry.pyi
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/videostab.pyi
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/wechat_qrcode.pyi
--rw-r--r--   0        0        0    40748 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/xfeatures2d.pyi
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/xphoto.pyi
--rw-r--r--   0        0        0   105878 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/core.pyi
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/ie.pyi
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/oak.pyi
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/onnx.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/own.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/render.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/video.pyi
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/streaming/__init__.pyi
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/__init__.pyi
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/draw.pyi
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/gst.pyi
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/kinfu/__init__.pyi
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/kinfu/detail.pyi
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/misc/__init__.pyi
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/misc/version.pyi
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/__init__.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/fs.pyi
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/nested.pyi
--rw-r--r--   0        0        0    80287 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ximgproc/__init__.pyi
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/src/cv2-stubs/modules/ximgproc/segmentation.pyi
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/add_missing_overloads.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/generate_classes.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/generate_constants.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/generate_modules.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/merge_with_microsoft_stubs.py
--rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/processing_utils.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/utils/undefined_to_any.py
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/LICENSE
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/README.md
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 opencv_stubs-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/requirements/requirements.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/__init__.pyi
+-rw-r--r--   0        0        0   165718 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/classes.pyi
+-rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/constants.pyi
+-rw-r--r--   0        0        0   529741 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/functions.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/py.typed
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/__init__.py
+-rw-r--r--   0        0        0    34376 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/aruco.pyi
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/barcode.pyi
+-rw-r--r--   0        0        0    11107 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/bgsegm.pyi
+-rw-r--r--   0        0        0    19750 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/bioinspired.pyi
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ccm.pyi
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/colored_kinfu.pyi
+-rw-r--r--   0        0        0    23759 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/cuda.pyi
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/data.pyi
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/datasets.pyi
+-rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/detail.pyi
+-rw-r--r--   0        0        0    45108 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/dnn.pyi
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/dnn_superres.pyi
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/dpm.pyi
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/dynafu.pyi
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/error.pyi
+-rw-r--r--   0        0        0    34295 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/face.pyi
+-rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/fisheye.pyi
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/flann.pyi
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ft.pyi
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/hfs.pyi
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/img_hash.pyi
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/intensity_transform.pyi
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ipp.pyi
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/large_kinfu.pyi
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/legacy.pyi
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/line_descriptor.pyi
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/linemod.pyi
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/load_config_py3.pyi
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/mat_wrapper.pyi
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/mcc.pyi
+-rw-r--r--   0        0        0    60302 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ml.pyi
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/motempl.pyi
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/multicalib.pyi
+-rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ocl.pyi
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ogl.pyi
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/omnidir.pyi
+-rw-r--r--   0        0        0    27976 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/optflow.pyi
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/parallel.pyi
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/phase_unwrapping.pyi
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/plot.pyi
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ppf_match_3d.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/qt.pyi
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/quality.pyi
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/rapid.pyi
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/reg.pyi
+-rw-r--r--   0        0        0    30043 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/rgbd.pyi
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/saliency.pyi
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/samples.pyi
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/segmentation.pyi
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/stereo.pyi
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/structured_light.pyi
+-rw-r--r--   0        0        0    26974 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/text.pyi
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/version.pyi
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/videoio_registry.pyi
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/videostab.pyi
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/wechat_qrcode.pyi
+-rw-r--r--   0        0        0    40748 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/xfeatures2d.pyi
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/xphoto.pyi
+-rw-r--r--   0        0        0   105878 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/core.pyi
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/ie.pyi
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/oak.pyi
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/onnx.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/own.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/render.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/video.pyi
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/streaming/__init__.pyi
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/__init__.pyi
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/draw.pyi
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/gst.pyi
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/kinfu/__init__.pyi
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/kinfu/detail.pyi
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/misc/__init__.pyi
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/misc/version.pyi
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/__init__.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/fs.pyi
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/nested.pyi
+-rw-r--r--   0        0        0    80287 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ximgproc/__init__.pyi
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/src/cv2-stubs/modules/ximgproc/segmentation.pyi
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/add_missing_overloads.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/generate_classes.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/generate_constants.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/generate_modules.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/merge_with_microsoft_stubs.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/processing_utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/utils/undefined_to_any.py
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/README.md
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 opencv_stubs-0.0.7/PKG-INFO
```

### Comparing `opencv_stubs-0.0.6/.pre-commit-config.yaml` & `opencv_stubs-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/requirements/requirements-build.txt` & `opencv_stubs-0.0.7/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/requirements/requirements-dev.txt` & `opencv_stubs-0.0.7/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/classes.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/classes.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/constants.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/functions.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/functions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1325,15 +1325,15 @@
     "repeat(src, ny, nx[, dst]) -> dst\n.   @brief Fills the output array with repeated copies of the input array.\n.   \n.   The function cv::repeat duplicates the input array one or more times along each of the two axes:\n.   \\f[\\texttt{dst} _{ij}= \\texttt{src} _{i\\mod src.rows, \\; j\\mod src.cols }\\f]\n.   The second variant of the function is more convenient to use with @ref MatrixExpressions.\n.   @param src input array to replicate.\n.   @param ny Flag to specify how many times the `src` is repeated along the\n.   vertical axis.\n.   @param nx Flag to specify how many times the `src` is repeated along the\n.   horizontal axis.\n.   @param dst output array of the same type as `src`.\n.   @sa cv::reduce"
     ...
 
 def reprojectImageTo3D(disparity, Q, _3dImage=..., handleMissingValues=..., ddepth=...) -> Any:
     "reprojectImageTo3D(disparity, Q[, _3dImage[, handleMissingValues[, ddepth]]]) -> _3dImage\n.   @brief Reprojects a disparity image to 3D space.\n.   \n.   @param disparity Input single-channel 8-bit unsigned, 16-bit signed, 32-bit signed or 32-bit\n.   floating-point disparity image. The values of 8-bit / 16-bit signed formats are assumed to have no\n.   fractional bits. If the disparity is 16-bit signed format, as computed by @ref StereoBM or\n.   @ref StereoSGBM and maybe other algorithms, it should be divided by 16 (and scaled to float) before\n.   being used here.\n.   @param _3dImage Output 3-channel floating-point image of the same size as disparity. Each element of\n.   _3dImage(x,y) contains 3D coordinates of the point (x,y) computed from the disparity map. If one\n.   uses Q obtained by @ref stereoRectify, then the returned points are represented in the first\n.   camera's rectified coordinate system.\n.   @param Q \\f$4 \\times 4\\f$ perspective transformation matrix that can be obtained with\n.   @ref stereoRectify.\n.   @param handleMissingValues Indicates, whether the function should handle missing values (i.e.\n.   points where the disparity was not computed). If handleMissingValues=true, then pixels with the\n.   minimal disparity that corresponds to the outliers (see StereoMatcher::compute ) are transformed\n.   to 3D points with a very large Z value (currently set to 10000).\n.   @param ddepth The optional output array depth. If it is -1, the output image will have CV_32F\n.   depth. ddepth can also be set to CV_16S, CV_32S or CV_32F.\n.   \n.   The function transforms a single-channel disparity map to a 3-channel image representing a 3D\n.   surface. That is, for each pixel (x,y) and the corresponding disparity d=disparity(x,y) , it\n.   computes:\n.   \n.   \\f[\\begin{bmatrix}\n.   X \\\\\n.   Y \\\\\n.   Z \\\\\n.   W\n.   \\end{bmatrix} = Q \\begin{bmatrix}\n.   x \\\\\n.   y \\\\\n.   \\texttt{disparity} (x,y) \\\\\n.   z\n.   \\end{bmatrix}.\\f]\n.   \n.   @sa\n.      To reproject a sparse set of points {(x,y,d),...} to 3D space, use perspectiveTransform."
     ...
 
-def resize(src: npt.NDArray[_TImg], dsize: tuple[int, int], dst: npt.NDArray[_TImg] = ..., fx: int = ..., fy: int = ..., interpolation: int = ...) -> npt.NDArray[_TImg]:
+def resize(src: npt.NDArray[_TImg], dsize: _TSize, dst: npt.NDArray[_TImg] = ..., fx: float = 0, fy: float = 0, interpolation: int = INTER_LINEAR) -> npt.NDArray[_TImg]:
     "resize(src, dsize[, dst[, fx[, fy[, interpolation]]]]) -> dst\n.   @brief Resizes an image.\n.   \n.   The function resize resizes the image src down to or up to the specified size. Note that the\n.   initial dst type or size are not taken into account. Instead, the size and type are derived from\n.   the `src`,`dsize`,`fx`, and `fy`. If you want to resize src so that it fits the pre-created dst,\n.   you may call the function as follows:\n.   @code\n.       // explicitly specify dsize=dst.size(); fx and fy will be computed from that.\n.       resize(src, dst, dst.size(), 0, 0, interpolation);\n.   @endcode\n.   If you want to decimate the image by factor of 2 in each direction, you can call the function this\n.   way:\n.   @code\n.       // specify fx and fy and let the function compute the destination image size.\n.       resize(src, dst, Size(), 0.5, 0.5, interpolation);\n.   @endcode\n.   To shrink an image, it will generally look best with #INTER_AREA interpolation, whereas to\n.   enlarge an image, it will generally look best with c#INTER_CUBIC (slow) or #INTER_LINEAR\n.   (faster but still looks OK).\n.   \n.   @param src input image.\n.   @param dst output image; it has the size dsize (when it is non-zero) or the size computed from\n.   src.size(), fx, and fy; the type of dst is the same as of src.\n.   @param dsize output image size; if it equals zero, it is computed as:\n.    \\f[\\texttt{dsize = Size(round(fx*src.cols), round(fy*src.rows))}\\f]\n.    Either dsize or both fx and fy must be non-zero.\n.   @param fx scale factor along the horizontal axis; when it equals 0, it is computed as\n.   \\f[\\texttt{(double)dsize.width/src.cols}\\f]\n.   @param fy scale factor along the vertical axis; when it equals 0, it is computed as\n.   \\f[\\texttt{(double)dsize.height/src.rows}\\f]\n.   @param interpolation interpolation method, see #InterpolationFlags\n.   \n.   @sa  warpAffine, warpPerspective, remap."
     ...
 
 def resizeWindow(winname, width, height) -> Any:
     "resizeWindow(winname, width, height) -> None\n.   @brief Resizes window to the specified size\n.   \n.   @note\n.   \n.   -   The specified window size is for the image area. Toolbars are not counted.\n.   -   Only windows created without cv::WINDOW_AUTOSIZE flag can be resized.\n.   \n.   @param winname Window name.\n.   @param width The new window width.\n.   @param height The new window height.\n\n\n\nresizeWindow(winname, size) -> None\n.   @overload\n.   @param winname Window name.\n.   @param size The new window size."
     ...
```

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/__init__.py` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/aruco.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/aruco.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/barcode.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/barcode.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/bgsegm.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/bgsegm.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/bioinspired.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/bioinspired.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/ccm.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/ccm.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/colored_kinfu.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/colored_kinfu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/cuda.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/cuda.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/datasets.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/datasets.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/detail.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/detail.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/dnn.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/dnn.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/dnn_superres.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/dnn_superres.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/dynafu.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/dynafu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/error.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/error.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/face.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/face.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/fisheye.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/fisheye.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/flann.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/flann.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/ft.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/ft.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/hfs.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/hfs.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/img_hash.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/img_hash.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/intensity_transform.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/intensity_transform.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/large_kinfu.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/large_kinfu.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/legacy.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/legacy.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/line_descriptor.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/line_descriptor.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/linemod.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/linemod.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/mcc.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/mcc.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/ml.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/ml.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/motempl.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/motempl.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/ocl.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/ocl.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/ogl.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/ogl.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/omnidir.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/omnidir.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/optflow.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/optflow.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/phase_unwrapping.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/phase_unwrapping.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/plot.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/plot.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/ppf_match_3d.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/ppf_match_3d.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/quality.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/quality.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/rapid.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/rapid.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/reg.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/reg.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/rgbd.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/rgbd.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/saliency.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/saliency.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/samples.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/samples.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/segmentation.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/segmentation.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/stereo.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/stereo.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/structured_light.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/structured_light.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/text.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/text.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/videoio_registry.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/videoio_registry.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/wechat_qrcode.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/wechat_qrcode.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/xfeatures2d.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/xfeatures2d.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/xphoto.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/xphoto.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/__init__.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/ie.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/ie.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/oak.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/oak.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/streaming/__init__.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/streaming/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/__init__.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/gapi/wip/draw.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/gapi/wip/draw.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/kinfu/__init__.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/kinfu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/__init__.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/utils/nested.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/utils/nested.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/ximgproc/__init__.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/ximgproc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/src/cv2-stubs/modules/ximgproc/segmentation.pyi` & `opencv_stubs-0.0.7/src/cv2-stubs/modules/ximgproc/segmentation.pyi`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/utils/add_missing_overloads.py` & `opencv_stubs-0.0.7/utils/add_missing_overloads.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/utils/generate_classes.py` & `opencv_stubs-0.0.7/utils/generate_classes.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/utils/generate_constants.py` & `opencv_stubs-0.0.7/utils/generate_constants.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/utils/generate_modules.py` & `opencv_stubs-0.0.7/utils/generate_modules.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/utils/merge_with_microsoft_stubs.py` & `opencv_stubs-0.0.7/utils/merge_with_microsoft_stubs.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/utils/processing_utils.py` & `opencv_stubs-0.0.7/utils/processing_utils.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/utils/undefined_to_any.py` & `opencv_stubs-0.0.7/utils/undefined_to_any.py`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/LICENSE` & `opencv_stubs-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/README.md` & `opencv_stubs-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/pyproject.toml` & `opencv_stubs-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.6/PKG-INFO` & `opencv_stubs-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv-stubs
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unofficial stubs for the opencv-python package.
 Project-URL: Homepage, https://github.com/hoel-bagard/opencv-stubs
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/opencv-stubs/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Keywords: OpenCV,stubs
```

