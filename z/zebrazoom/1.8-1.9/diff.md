# Comparing `tmp/zebrazoom-1.8.tar.gz` & `tmp/zebrazoom-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zebrazoom-1.8.tar", last modified: Thu Jul 29 09:02:30 2021, max compression
+gzip compressed data, was "dist\zebrazoom-1.9.tar", last modified: Thu Jul 29 09:11:27 2021, max compression
```

## Comparing `zebrazoom-1.8.tar` & `zebrazoom-1.9.tar`

### file list

```diff
@@ -1,176 +1,179 @@
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.975998 zebrazoom-1.8/
--rw-rw-rw-   0        0        0    35184 2020-07-12 11:39:14.000000 zebrazoom-1.8/LICENSE
--rw-rw-rw-   0        0        0      616 2021-07-29 09:02:30.975998 zebrazoom-1.8/PKG-INFO
--rw-rw-rw-   0        0        0    55910 2021-07-27 07:01:59.000000 zebrazoom-1.8/README.md
--rw-rw-rw-   0        0        0       86 2021-07-29 09:02:30.979999 zebrazoom-1.8/setup.cfg
--rw-rw-rw-   0        0        0     2030 2021-07-29 08:38:16.000000 zebrazoom-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.136722 zebrazoom-1.8/zebrazoom/
--rw-rw-rw-   0        0        0    14232 2021-07-22 09:22:03.000000 zebrazoom-1.8/zebrazoom/GUIAllPy.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.069112 zebrazoom-1.8/zebrazoom/ZZoutput/
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.166737 zebrazoom-1.8/zebrazoom/ZZoutput/example1/
--rw-rw-rw-   0        0        0   805136 2020-08-24 09:53:52.000000 zebrazoom-1.8/zebrazoom/ZZoutput/example1/results_example1.txt
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.168722 zebrazoom-1.8/zebrazoom/ZZoutput/example2/
--rw-rw-rw-   0        0        0   619318 2020-08-24 09:54:43.000000 zebrazoom-1.8/zebrazoom/ZZoutput/example2/results_example2.txt
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.170723 zebrazoom-1.8/zebrazoom/ZZoutput/example3/
--rw-rw-rw-   0        0        0   602989 2020-08-24 09:55:20.000000 zebrazoom-1.8/zebrazoom/ZZoutput/example3/results_example3.txt
--rw-rw-rw-   0        0        0      347 2020-12-13 07:49:23.000000 zebrazoom-1.8/zebrazoom/__init__.py
--rw-rw-rw-   0        0        0     4519 2021-07-29 08:51:15.000000 zebrazoom-1.8/zebrazoom/__main__.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.280091 zebrazoom-1.8/zebrazoom/code/
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.412242 zebrazoom-1.8/zebrazoom/code/GUI/
--rw-rw-rw-   0        0        0    34881 2021-07-16 15:25:27.000000 zebrazoom-1.8/zebrazoom/code/GUI/GUI_InitialClasses.py
--rw-rw-rw-   0        0        0    15732 2021-07-20 09:44:04.000000 zebrazoom-1.8/zebrazoom/code/GUI/GUI_InitialFunctions.py
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/GUI/__init__.py
--rw-rw-rw-   0        0        0     5606 2020-06-26 12:53:00.000000 zebrazoom-1.8/zebrazoom/code/GUI/adjustParameterInsideAlgo.py
--rw-rw-rw-   0        0        0    10825 2021-04-22 06:31:29.000000 zebrazoom-1.8/zebrazoom/code/GUI/adjustParameterInsideAlgoFunctions.py
--rw-rw-rw-   0        0        0    11576 2021-07-16 12:01:47.000000 zebrazoom-1.8/zebrazoom/code/GUI/automaticallyFindOptimalParameters.py
--rw-rw-rw-   0        0        0    18860 2021-06-02 08:22:55.000000 zebrazoom-1.8/zebrazoom/code/GUI/automaticallyFindOptimalParametersFunctions.py
--rw-rw-rw-   0        0        0     8688 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/code/GUI/blobCenter.png
--rw-rw-rw-   0        0        0     8736 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/code/GUI/blobExtremity.png
--rw-rw-rw-   0        0        0    23255 2021-07-16 11:12:20.000000 zebrazoom-1.8/zebrazoom/code/GUI/configFilePrepare.py
--rw-rw-rw-   0        0        0    27789 2021-07-16 11:21:59.000000 zebrazoom-1.8/zebrazoom/code/GUI/configFilePrepareFunctions.py
--rw-rw-rw-   0        0        0     2350 2020-12-08 04:02:11.000000 zebrazoom-1.8/zebrazoom/code/GUI/configFileZebrafish.py
--rw-rw-rw-   0        0        0     1416 2021-03-27 02:43:49.000000 zebrazoom-1.8/zebrazoom/code/GUI/configFileZebrafishFunctions.py
--rw-rw-rw-   0        0        0     9724 2021-07-22 17:10:50.000000 zebrazoom-1.8/zebrazoom/code/GUI/dataAnalysisGUI.py
--rw-rw-rw-   0        0        0     7649 2021-07-22 10:25:15.000000 zebrazoom-1.8/zebrazoom/code/GUI/dataAnalysisGUIFunctions.py
--rw-rw-rw-   0        0        0     1098 2021-06-25 09:21:29.000000 zebrazoom-1.8/zebrazoom/code/GUI/getCoordinates.py
--rw-rw-rw-   0        0        0   331953 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/code/GUI/leftborder.png
--rw-rw-rw-   0        0        0   388432 2020-04-12 09:43:51.000000 zebrazoom-1.8/zebrazoom/code/GUI/no1.png
--rw-rw-rw-   0        0        0   305740 2020-04-12 09:42:07.000000 zebrazoom-1.8/zebrazoom/code/GUI/no2.png
--rw-rw-rw-   0        0        0   312222 2020-04-12 09:43:42.000000 zebrazoom-1.8/zebrazoom/code/GUI/ok1.png
--rw-rw-rw-   0        0        0   330224 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/code/GUI/rightborder.png
--rw-rw-rw-   0        0        0   669352 2020-04-12 09:42:26.000000 zebrazoom-1.8/zebrazoom/code/GUI/savedjustincase.png
--rw-rw-rw-   0        0        0     2731 2021-05-20 03:37:00.000000 zebrazoom-1.8/zebrazoom/code/GUI/troubleshooting.py
--rw-rw-rw-   0        0        0     5958 2020-12-06 03:30:11.000000 zebrazoom-1.8/zebrazoom/code/GUI/troubleshootingFunction.py
--rw-rw-rw-   0        0        0        0 2020-12-09 01:22:02.000000 zebrazoom-1.8/zebrazoom/code/__init__.py
--rw-rw-rw-   0        0        0    10067 2021-06-28 12:32:34.000000 zebrazoom-1.8/zebrazoom/code/adjustHyperparameters.py
--rw-rw-rw-   0        0        0    11880 2021-07-25 12:36:02.000000 zebrazoom-1.8/zebrazoom/code/createSuperStruct.py
--rw-rw-rw-   0        0        0    11491 2021-07-16 15:18:23.000000 zebrazoom-1.8/zebrazoom/code/createValidationVideo.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.450274 zebrazoom-1.8/zebrazoom/code/dataPostProcessing/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/dataPostProcessing/__init__.py
--rw-rw-rw-   0        0        0     3061 2021-03-24 02:59:47.000000 zebrazoom-1.8/zebrazoom/code/dataPostProcessing/computeEyesHeadingPlot.py
--rw-rw-rw-   0        0        0      774 2021-07-22 17:10:50.000000 zebrazoom-1.8/zebrazoom/code/dataPostProcessing/dataPostProcessing.py
--rw-rw-rw-   0        0        0     2997 2021-07-26 12:23:04.000000 zebrazoom-1.8/zebrazoom/code/dataPostProcessing/findSleepVsMoving.py
--rw-rw-rw-   0        0        0      835 2020-04-01 06:39:59.000000 zebrazoom-1.8/zebrazoom/code/dataPostProcessing/generateAllTimeTailAngleGraph.py
--rw-rw-rw-   0        0        0     9063 2021-02-18 03:27:25.000000 zebrazoom-1.8/zebrazoom/code/dataPostProcessing/perBoutOutput.py
--rw-rw-rw-   0        0        0     7874 2021-07-28 13:53:04.000000 zebrazoom-1.8/zebrazoom/code/defaultConfigFile.json
--rw-rw-rw-   0        0        0     8393 2021-07-03 08:10:08.000000 zebrazoom-1.8/zebrazoom/code/detectMovementWithRawVideo.py
--rw-rw-rw-   0        0        0    14953 2021-04-29 02:18:54.000000 zebrazoom-1.8/zebrazoom/code/extractParameters.py
--rw-rw-rw-   0        0        0     7359 2021-07-27 15:49:22.000000 zebrazoom-1.8/zebrazoom/code/fasterMultiprocessing.py
--rw-rw-rw-   0        0        0    21648 2021-07-16 12:27:47.000000 zebrazoom-1.8/zebrazoom/code/findWells.py
--rw-rw-rw-   0        0        0     5572 2021-06-03 02:34:36.000000 zebrazoom-1.8/zebrazoom/code/getBackground.py
--rw-rw-rw-   0        0        0    27463 2021-07-28 13:50:20.000000 zebrazoom-1.8/zebrazoom/code/getHyperparameters.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.520029 zebrazoom-1.8/zebrazoom/code/getImage/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/getImage/__init__.py
--rw-rw-rw-   0        0        0     4331 2021-07-25 07:58:08.000000 zebrazoom-1.8/zebrazoom/code/getImage/getForegroundImage.py
--rw-rw-rw-   0        0        0     4419 2021-07-25 07:58:08.000000 zebrazoom-1.8/zebrazoom/code/getImage/getForegroundImageSequential.py
--rw-rw-rw-   0        0        0     1047 2021-03-27 00:54:06.000000 zebrazoom-1.8/zebrazoom/code/getImage/getImage.py
--rw-rw-rw-   0        0        0     1152 2021-03-27 00:54:21.000000 zebrazoom-1.8/zebrazoom/code/getImage/getImageSequential.py
--rw-rw-rw-   0        0        0     1117 2021-03-27 00:54:45.000000 zebrazoom-1.8/zebrazoom/code/getImage/headEmbededFrame.py
--rw-rw-rw-   0        0        0     1486 2021-03-27 00:54:59.000000 zebrazoom-1.8/zebrazoom/code/getImage/headEmbededFrameBackExtract.py
--rw-rw-rw-   0        0        0     1136 2021-03-27 00:55:11.000000 zebrazoom-1.8/zebrazoom/code/getImage/headEmbededFrameSequential.py
--rw-rw-rw-   0        0        0     1437 2021-03-27 00:53:06.000000 zebrazoom-1.8/zebrazoom/code/getImage/headEmbededFrameSequentialBackExtract.py
--rw-rw-rw-   0        0        0     1440 2021-05-16 04:14:52.000000 zebrazoom-1.8/zebrazoom/code/popUpAlgoFollow.py
--rw-rw-rw-   0        0        0     1166 2020-04-13 11:00:26.000000 zebrazoom-1.8/zebrazoom/code/popUpAlgoFollowOldVersion.py
--rw-rw-rw-   0        0        0     5080 2021-07-24 12:05:17.000000 zebrazoom-1.8/zebrazoom/code/preprocessImage.py
--rw-rw-rw-   0        0        0     8894 2021-07-26 13:16:42.000000 zebrazoom-1.8/zebrazoom/code/readValidationVideo.py
--rw-rw-rw-   0        0        0     1123 2021-06-03 04:10:29.000000 zebrazoom-1.8/zebrazoom/code/resizeImageTooLarge.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.557996 zebrazoom-1.8/zebrazoom/code/trackingFolder/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/__init__.py
--rw-rw-rw-   0        0        0      930 2021-03-27 04:14:32.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/blackFramesDetection.py
--rw-rw-rw-   0        0        0     1686 2021-07-25 18:48:40.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/debugTracking.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.568026 zebrazoom-1.8/zebrazoom/code/trackingFolder/eyeTracking/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/eyeTracking/__init__.py
--rw-rw-rw-   0        0        0    10496 2021-04-30 02:34:25.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/eyeTracking/eyeTracking.py
--rw-rw-rw-   0        0        0     4299 2021-07-20 12:58:55.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/getImages.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.603994 zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/__init__.py
--rw-rw-rw-   0        0        0     4695 2021-04-20 01:18:41.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/calculateHeading.py
--rw-rw-rw-   0        0        0     4507 2021-07-27 14:21:17.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/headTrackingHeadingCalculation.py
--rw-rw-rw-   0        0        0     1698 2021-03-17 02:01:43.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/headTrackingTakeHeadClosestToWellCenter.py
--rw-rw-rw-   0        0        0    17676 2021-07-04 08:32:10.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/multipleAnimalsHeadTracking.py
--rw-rw-rw-   0        0        0    18833 2020-12-06 03:48:25.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/multipleAnimalsHeadTrackingAdvance.py
--rw-rw-rw-   0        0        0     6392 2021-07-28 06:49:04.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/postProcessMultipleTrajectories.py
--rw-rw-rw-   0        0        0     3768 2021-07-21 15:40:17.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTracking.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.648028 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/__init__.py
--rw-rw-rw-   0        0        0     5858 2020-12-06 03:53:06.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/centerOfMassTailTracking.py
--rw-rw-rw-   0        0        0     4703 2021-03-02 06:18:06.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/getTailTipManual.py
--rw-rw-rw-   0        0        0    19033 2021-03-27 02:51:23.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/headEmbededTailTracking.py
--rw-rw-rw-   0        0        0     7895 2021-03-27 04:07:04.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/headEmbededTailTrackingTeresaNicolson.py
--rw-rw-rw-   0        0        0    11338 2020-12-08 01:10:44.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingBlobDescent.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.697996 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/
--rw-rw-rw-   0        0        0     1827 2021-03-14 02:10:07.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/Rotate.py
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/__init__.py
--rw-rw-rw-   0        0        0     4710 2021-06-02 00:55:23.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findBodyContour.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.731995 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/__init__.py
--rw-rw-rw-   0        0        0      935 2021-04-18 01:37:27.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/checkIfMidlineIsInBlob.py
--rw-rw-rw-   0        0        0     6142 2021-03-14 07:04:45.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/findTailExtremete.py
--rw-rw-rw-   0        0        0     2440 2020-12-08 01:12:05.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/functions.py
--rw-rw-rw-   0        0        0     2851 2021-04-28 08:33:28.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/insideTailExtremete.py
--rw-rw-rw-   0        0        0     7147 2021-07-21 15:40:46.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTheTwoSides.py
--rw-rw-rw-   0        0        0     3927 2021-03-13 08:38:26.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/getMidline.py
--rw-rw-rw-   0        0        0     1373 2020-12-08 01:13:10.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/resampleSeqConstPtsPerArcLength.py
--rw-rw-rw-   0        0        0     8314 2021-07-26 06:38:33.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/tailTrackingExtremityDetect.py
--rw-rw-rw-   0        0        0    11696 2021-07-28 07:46:15.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/tracking.py
--rw-rw-rw-   0        0        0      924 2021-03-14 07:10:47.000000 zebrazoom-1.8/zebrazoom/code/trackingFolder/trackingFunctions.py
--rw-rw-rw-   0        0        0      874 2020-07-08 12:50:43.000000 zebrazoom-1.8/zebrazoom/code/vars.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.753999 zebrazoom-1.8/zebrazoom/configuration/
--rw-rw-rw-   0        0        0      568 2021-05-06 04:38:59.000000 zebrazoom-1.8/zebrazoom/configuration/4wellsZebrafishLarvaeEscapeResponses.json
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/configuration/__init__.py
--rw-rw-rw-   0        0        0      568 2020-04-27 07:27:19.000000 zebrazoom-1.8/zebrazoom/configuration/fliesInTube.json
--rw-rw-rw-   0        0        0      725 2021-05-05 02:48:22.000000 zebrazoom-1.8/zebrazoom/configuration/headEmbeddedZebrafishLarva.json
--rw-rw-rw-   0        0        0      767 2021-07-28 08:28:34.000000 zebrazoom-1.8/zebrazoom/configuration/screenFastTrackingConfigFileTemplate.json
--rw-rw-rw-   0        0        0      569 2021-07-28 11:55:25.000000 zebrazoom-1.8/zebrazoom/configuration/testThresholdsForFastScreen.json
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.785997 zebrazoom-1.8/zebrazoom/dataAnalysis/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.785997 zebrazoom-1.8/zebrazoom/dataAnalysis/classifiers/
--rw-rw-rw-   0        0        0        0 2020-09-04 15:06:35.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/classifiers/__init__.py
--rw-rw-rw-   0        0        0     2032 2020-12-14 00:20:56.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/cluster_1a_UsageExample.py
--rw-rw-rw-   0        0        0     1360 2020-12-14 00:21:04.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/cluster_1b_UsageExampleReloadClassifier.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.788003 zebrazoom-1.8/zebrazoom/dataAnalysis/data/
--rw-rw-rw-   0        0        0        0 2020-09-04 15:06:35.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/data/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.824036 zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/__init__.py
--rw-rw-rw-   0        0        0    18511 2021-02-17 12:03:50.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/applyClustering.py
--rw-rw-rw-   0        0        0     3379 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/createSuperClusterVideo.py
--rw-rw-rw-   0        0        0     6735 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/outputValidationVideo.py
--rw-rw-rw-   0        0        0     2252 2021-07-23 16:01:25.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/populationComparaison.py
--rw-rw-rw-   0        0        0     6582 2020-09-03 13:57:12.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/readValidationVideoDataAnalysis.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.954018 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/__init__.py
--rw-rw-rw-   0        0        0    13407 2021-07-23 08:09:43.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/createDataFrame.py
--rw-rw-rw-   0        0        0     1128 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/createDatasetsForExperiments.py
--rw-rw-rw-   0        0        0      750 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getDeltaHead.py
--rw-rw-rw-   0        0        0     2659 2020-09-06 10:08:38.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getDynamicParameters.py
--rw-rw-rw-   0        0        0     2098 2021-07-22 10:34:23.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getGlobalParameters.py
--rw-rw-rw-   0        0        0      932 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getInstaHeadingDiff.py
--rw-rw-rw-   0        0        0     1048 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getInstaHorizontalDisplacement.py
--rw-rw-rw-   0        0        0      993 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getInstaMaxTailBendPos.py
--rw-rw-rw-   0        0        0      737 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getInstaSpeed.py
--rw-rw-rw-   0        0        0     2127 2020-06-17 15:02:46.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated.py
--rw-rw-rw-   0        0        0     1207 2020-12-08 01:15:12.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated2.py
--rw-rw-rw-   0        0        0     1429 2020-09-06 10:14:33.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getTailAngles.py
--rw-rw-rw-   0        0        0      190 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getTailLength.py
--rw-rw-rw-   0        0        0      173 2020-03-24 08:23:13.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getTailLength2.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.957999 zebrazoom-1.8/zebrazoom/dataAnalysis/experimentOrganizationExcel/
--rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/experimentOrganizationExcel/__init__.py
--rw-rw-rw-   0        0        0     8192 2020-08-24 14:40:29.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/experimentOrganizationExcel/example.xls
--rw-rw-rw-   0        0        0     1092 2021-07-22 08:38:38.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/populationCompare_UsageExample.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.959998 zebrazoom-1.8/zebrazoom/dataAnalysis/resultsClustering/
--rw-rw-rw-   0        0        0        0 2020-09-04 15:06:35.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/resultsClustering/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.961998 zebrazoom-1.8/zebrazoom/dataAnalysis/resultsKinematic/
--rw-rw-rw-   0        0        0        0 2020-09-04 15:06:35.000000 zebrazoom-1.8/zebrazoom/dataAnalysis/resultsKinematic/__init__.py
--rw-rw-rw-   0        0        0     1393 2021-07-19 13:48:28.000000 zebrazoom-1.8/zebrazoom/extractZZParametersFromTailAngle.py
--rw-rw-rw-   0        0        0     2809 2021-07-19 13:49:28.000000 zebrazoom-1.8/zebrazoom/getTailExtremityFirstFrame.py
--rw-rw-rw-   0        0        0    14094 2021-07-28 13:59:34.000000 zebrazoom-1.8/zebrazoom/mainZZ.py
--rw-rw-rw-   0        0        0     1731 2021-07-19 13:50:11.000000 zebrazoom-1.8/zebrazoom/recreateSuperStruct.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.973997 zebrazoom-1.8/zebrazoom/videoFormatConversion/
--rw-rw-rw-   0        0        0        0 2020-12-09 01:22:02.000000 zebrazoom-1.8/zebrazoom/videoFormatConversion/__init__.py
--rw-rw-rw-   0        0        0     2663 2021-03-12 04:51:29.000000 zebrazoom-1.8/zebrazoom/videoFormatConversion/seq_to_avi.py
-drwxrwxrwx   0        0        0        0 2021-07-29 09:02:30.164723 zebrazoom-1.8/zebrazoom.egg-info/
--rw-rw-rw-   0        0        0      616 2021-07-29 09:02:29.000000 zebrazoom-1.8/zebrazoom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8186 2021-07-29 09:02:29.000000 zebrazoom-1.8/zebrazoom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-29 09:02:29.000000 zebrazoom-1.8/zebrazoom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2021-07-29 09:02:29.000000 zebrazoom-1.8/zebrazoom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-07-29 09:02:29.000000 zebrazoom-1.8/zebrazoom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.858809 zebrazoom-1.9/
+-rw-rw-rw-   0        0        0    35184 2020-07-12 11:39:14.000000 zebrazoom-1.9/LICENSE
+-rw-rw-rw-   0        0        0      616 2021-07-29 09:11:27.858809 zebrazoom-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    55910 2021-07-27 07:01:59.000000 zebrazoom-1.9/README.md
+-rw-rw-rw-   0        0        0       86 2021-07-29 09:11:27.858809 zebrazoom-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2030 2021-07-29 09:10:17.000000 zebrazoom-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.442036 zebrazoom-1.9/zebrazoom/
+-rw-rw-rw-   0        0        0    14232 2021-07-22 09:22:03.000000 zebrazoom-1.9/zebrazoom/GUIAllPy.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.404242 zebrazoom-1.9/zebrazoom/ZZoutput/
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.488907 zebrazoom-1.9/zebrazoom/ZZoutput/example1/
+-rw-rw-rw-   0        0        0   805136 2020-08-24 09:53:52.000000 zebrazoom-1.9/zebrazoom/ZZoutput/example1/results_example1.txt
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.488907 zebrazoom-1.9/zebrazoom/ZZoutput/example2/
+-rw-rw-rw-   0        0        0   619318 2020-08-24 09:54:43.000000 zebrazoom-1.9/zebrazoom/ZZoutput/example2/results_example2.txt
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.488907 zebrazoom-1.9/zebrazoom/ZZoutput/example3/
+-rw-rw-rw-   0        0        0   602989 2020-08-24 09:55:20.000000 zebrazoom-1.9/zebrazoom/ZZoutput/example3/results_example3.txt
+-rw-rw-rw-   0        0        0      347 2020-12-13 07:49:23.000000 zebrazoom-1.9/zebrazoom/__init__.py
+-rw-rw-rw-   0        0        0     4519 2021-07-29 08:51:15.000000 zebrazoom-1.9/zebrazoom/__main__.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.542325 zebrazoom-1.9/zebrazoom/code/
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.620439 zebrazoom-1.9/zebrazoom/code/GUI/
+-rw-rw-rw-   0        0        0    34881 2021-07-16 15:25:27.000000 zebrazoom-1.9/zebrazoom/code/GUI/GUI_InitialClasses.py
+-rw-rw-rw-   0        0        0    15732 2021-07-20 09:44:04.000000 zebrazoom-1.9/zebrazoom/code/GUI/GUI_InitialFunctions.py
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/GUI/__init__.py
+-rw-rw-rw-   0        0        0     5606 2020-06-26 12:53:00.000000 zebrazoom-1.9/zebrazoom/code/GUI/adjustParameterInsideAlgo.py
+-rw-rw-rw-   0        0        0    10825 2021-04-22 06:31:29.000000 zebrazoom-1.9/zebrazoom/code/GUI/adjustParameterInsideAlgoFunctions.py
+-rw-rw-rw-   0        0        0    11576 2021-07-16 12:01:47.000000 zebrazoom-1.9/zebrazoom/code/GUI/automaticallyFindOptimalParameters.py
+-rw-rw-rw-   0        0        0    18860 2021-06-02 08:22:55.000000 zebrazoom-1.9/zebrazoom/code/GUI/automaticallyFindOptimalParametersFunctions.py
+-rw-rw-rw-   0        0        0     8688 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/code/GUI/blobCenter.png
+-rw-rw-rw-   0        0        0     8736 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/code/GUI/blobExtremity.png
+-rw-rw-rw-   0        0        0    23255 2021-07-16 11:12:20.000000 zebrazoom-1.9/zebrazoom/code/GUI/configFilePrepare.py
+-rw-rw-rw-   0        0        0    27789 2021-07-16 11:21:59.000000 zebrazoom-1.9/zebrazoom/code/GUI/configFilePrepareFunctions.py
+-rw-rw-rw-   0        0        0     2350 2020-12-08 04:02:11.000000 zebrazoom-1.9/zebrazoom/code/GUI/configFileZebrafish.py
+-rw-rw-rw-   0        0        0     1416 2021-03-27 02:43:49.000000 zebrazoom-1.9/zebrazoom/code/GUI/configFileZebrafishFunctions.py
+-rw-rw-rw-   0        0        0     9724 2021-07-22 17:10:50.000000 zebrazoom-1.9/zebrazoom/code/GUI/dataAnalysisGUI.py
+-rw-rw-rw-   0        0        0     7649 2021-07-22 10:25:15.000000 zebrazoom-1.9/zebrazoom/code/GUI/dataAnalysisGUIFunctions.py
+-rw-rw-rw-   0        0        0     1098 2021-06-25 09:21:29.000000 zebrazoom-1.9/zebrazoom/code/GUI/getCoordinates.py
+-rw-rw-rw-   0        0        0   331953 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/code/GUI/leftborder.png
+-rw-rw-rw-   0        0        0   388432 2020-04-12 09:43:51.000000 zebrazoom-1.9/zebrazoom/code/GUI/no1.png
+-rw-rw-rw-   0        0        0   305740 2020-04-12 09:42:07.000000 zebrazoom-1.9/zebrazoom/code/GUI/no2.png
+-rw-rw-rw-   0        0        0   312222 2020-04-12 09:43:42.000000 zebrazoom-1.9/zebrazoom/code/GUI/ok1.png
+-rw-rw-rw-   0        0        0   330224 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/code/GUI/rightborder.png
+-rw-rw-rw-   0        0        0   669352 2020-04-12 09:42:26.000000 zebrazoom-1.9/zebrazoom/code/GUI/savedjustincase.png
+-rw-rw-rw-   0        0        0     2731 2021-05-20 03:37:00.000000 zebrazoom-1.9/zebrazoom/code/GUI/troubleshooting.py
+-rw-rw-rw-   0        0        0     5958 2020-12-06 03:30:11.000000 zebrazoom-1.9/zebrazoom/code/GUI/troubleshootingFunction.py
+-rw-rw-rw-   0        0        0        0 2020-12-09 01:22:02.000000 zebrazoom-1.9/zebrazoom/code/__init__.py
+-rw-rw-rw-   0        0        0    10067 2021-06-28 12:32:34.000000 zebrazoom-1.9/zebrazoom/code/adjustHyperparameters.py
+-rw-rw-rw-   0        0        0    11880 2021-07-25 12:36:02.000000 zebrazoom-1.9/zebrazoom/code/createSuperStruct.py
+-rw-rw-rw-   0        0        0    11491 2021-07-16 15:18:23.000000 zebrazoom-1.9/zebrazoom/code/createValidationVideo.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.626951 zebrazoom-1.9/zebrazoom/code/dataPostProcessing/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/dataPostProcessing/__init__.py
+-rw-rw-rw-   0        0        0     3061 2021-03-24 02:59:47.000000 zebrazoom-1.9/zebrazoom/code/dataPostProcessing/computeEyesHeadingPlot.py
+-rw-rw-rw-   0        0        0      774 2021-07-22 17:10:50.000000 zebrazoom-1.9/zebrazoom/code/dataPostProcessing/dataPostProcessing.py
+-rw-rw-rw-   0        0        0     2997 2021-07-26 12:23:04.000000 zebrazoom-1.9/zebrazoom/code/dataPostProcessing/findSleepVsMoving.py
+-rw-rw-rw-   0        0        0      835 2020-04-01 06:39:59.000000 zebrazoom-1.9/zebrazoom/code/dataPostProcessing/generateAllTimeTailAngleGraph.py
+-rw-rw-rw-   0        0        0     9063 2021-02-18 03:27:25.000000 zebrazoom-1.9/zebrazoom/code/dataPostProcessing/perBoutOutput.py
+-rw-rw-rw-   0        0        0     7874 2021-07-28 13:53:04.000000 zebrazoom-1.9/zebrazoom/code/defaultConfigFile.json
+-rw-rw-rw-   0        0        0     8393 2021-07-03 08:10:08.000000 zebrazoom-1.9/zebrazoom/code/detectMovementWithRawVideo.py
+-rw-rw-rw-   0        0        0    14953 2021-04-29 02:18:54.000000 zebrazoom-1.9/zebrazoom/code/extractParameters.py
+-rw-rw-rw-   0        0        0     7359 2021-07-27 15:49:22.000000 zebrazoom-1.9/zebrazoom/code/fasterMultiprocessing.py
+-rw-rw-rw-   0        0        0    21648 2021-07-16 12:27:47.000000 zebrazoom-1.9/zebrazoom/code/findWells.py
+-rw-rw-rw-   0        0        0     5572 2021-06-03 02:34:36.000000 zebrazoom-1.9/zebrazoom/code/getBackground.py
+-rw-rw-rw-   0        0        0    27463 2021-07-28 13:50:20.000000 zebrazoom-1.9/zebrazoom/code/getHyperparameters.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.658215 zebrazoom-1.9/zebrazoom/code/getImage/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/getImage/__init__.py
+-rw-rw-rw-   0        0        0     4331 2021-07-25 07:58:08.000000 zebrazoom-1.9/zebrazoom/code/getImage/getForegroundImage.py
+-rw-rw-rw-   0        0        0     4419 2021-07-25 07:58:08.000000 zebrazoom-1.9/zebrazoom/code/getImage/getForegroundImageSequential.py
+-rw-rw-rw-   0        0        0     1047 2021-03-27 00:54:06.000000 zebrazoom-1.9/zebrazoom/code/getImage/getImage.py
+-rw-rw-rw-   0        0        0     1152 2021-03-27 00:54:21.000000 zebrazoom-1.9/zebrazoom/code/getImage/getImageSequential.py
+-rw-rw-rw-   0        0        0     1117 2021-03-27 00:54:45.000000 zebrazoom-1.9/zebrazoom/code/getImage/headEmbededFrame.py
+-rw-rw-rw-   0        0        0     1486 2021-03-27 00:54:59.000000 zebrazoom-1.9/zebrazoom/code/getImage/headEmbededFrameBackExtract.py
+-rw-rw-rw-   0        0        0     1136 2021-03-27 00:55:11.000000 zebrazoom-1.9/zebrazoom/code/getImage/headEmbededFrameSequential.py
+-rw-rw-rw-   0        0        0     1437 2021-03-27 00:53:06.000000 zebrazoom-1.9/zebrazoom/code/getImage/headEmbededFrameSequentialBackExtract.py
+-rw-rw-rw-   0        0        0     1440 2021-05-16 04:14:52.000000 zebrazoom-1.9/zebrazoom/code/popUpAlgoFollow.py
+-rw-rw-rw-   0        0        0     1166 2020-04-13 11:00:26.000000 zebrazoom-1.9/zebrazoom/code/popUpAlgoFollowOldVersion.py
+-rw-rw-rw-   0        0        0     5080 2021-07-24 12:05:17.000000 zebrazoom-1.9/zebrazoom/code/preprocessImage.py
+-rw-rw-rw-   0        0        0     8894 2021-07-26 13:16:42.000000 zebrazoom-1.9/zebrazoom/code/readValidationVideo.py
+-rw-rw-rw-   0        0        0     1123 2021-06-03 04:10:29.000000 zebrazoom-1.9/zebrazoom/code/resizeImageTooLarge.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.673852 zebrazoom-1.9/zebrazoom/code/trackingFolder/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/__init__.py
+-rw-rw-rw-   0        0        0      930 2021-03-27 04:14:32.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/blackFramesDetection.py
+-rw-rw-rw-   0        0        0     1686 2021-07-25 18:48:40.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/debugTracking.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.689465 zebrazoom-1.9/zebrazoom/code/trackingFolder/eyeTracking/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/eyeTracking/__init__.py
+-rw-rw-rw-   0        0        0    10496 2021-04-30 02:34:25.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/eyeTracking/eyeTracking.py
+-rw-rw-rw-   0        0        0     4299 2021-07-20 12:58:55.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/getImages.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.689465 zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/__init__.py
+-rw-rw-rw-   0        0        0     4695 2021-04-20 01:18:41.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/calculateHeading.py
+-rw-rw-rw-   0        0        0     4507 2021-07-27 14:21:17.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/headTrackingHeadingCalculation.py
+-rw-rw-rw-   0        0        0     1698 2021-03-17 02:01:43.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/headTrackingTakeHeadClosestToWellCenter.py
+-rw-rw-rw-   0        0        0    17676 2021-07-04 08:32:10.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/multipleAnimalsHeadTracking.py
+-rw-rw-rw-   0        0        0    18833 2020-12-06 03:48:25.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/multipleAnimalsHeadTrackingAdvance.py
+-rw-rw-rw-   0        0        0     6392 2021-07-28 06:49:04.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/postProcessMultipleTrajectories.py
+-rw-rw-rw-   0        0        0     3768 2021-07-21 15:40:17.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTracking.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.705088 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/__init__.py
+-rw-rw-rw-   0        0        0     5858 2020-12-06 03:53:06.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/centerOfMassTailTracking.py
+-rw-rw-rw-   0        0        0     4703 2021-03-02 06:18:06.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/getTailTipManual.py
+-rw-rw-rw-   0        0        0    19033 2021-03-27 02:51:23.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/headEmbededTailTracking.py
+-rw-rw-rw-   0        0        0     7895 2021-03-27 04:07:04.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/headEmbededTailTrackingTeresaNicolson.py
+-rw-rw-rw-   0        0        0    11338 2020-12-08 01:10:44.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingBlobDescent.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.727223 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/
+-rw-rw-rw-   0        0        0     1827 2021-03-14 02:10:07.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/Rotate.py
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/__init__.py
+-rw-rw-rw-   0        0        0     4710 2021-06-02 00:55:23.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findBodyContour.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.742872 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/__init__.py
+-rw-rw-rw-   0        0        0      935 2021-04-18 01:37:27.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/checkIfMidlineIsInBlob.py
+-rw-rw-rw-   0        0        0     6142 2021-03-14 07:04:45.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/findTailExtremete.py
+-rw-rw-rw-   0        0        0     2440 2020-12-08 01:12:05.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/functions.py
+-rw-rw-rw-   0        0        0     2851 2021-04-28 08:33:28.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/insideTailExtremete.py
+-rw-rw-rw-   0        0        0     7147 2021-07-21 15:40:46.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTheTwoSides.py
+-rw-rw-rw-   0        0        0     3927 2021-03-13 08:38:26.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/getMidline.py
+-rw-rw-rw-   0        0        0     1373 2020-12-08 01:13:10.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/resampleSeqConstPtsPerArcLength.py
+-rw-rw-rw-   0        0        0     8314 2021-07-26 06:38:33.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/tailTrackingExtremityDetect.py
+-rw-rw-rw-   0        0        0    11696 2021-07-28 07:46:15.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/tracking.py
+-rw-rw-rw-   0        0        0      924 2021-03-14 07:10:47.000000 zebrazoom-1.9/zebrazoom/code/trackingFolder/trackingFunctions.py
+-rw-rw-rw-   0        0        0      874 2020-07-08 12:50:43.000000 zebrazoom-1.9/zebrazoom/code/vars.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.758485 zebrazoom-1.9/zebrazoom/configuration/
+-rw-rw-rw-   0        0        0      568 2021-05-06 04:38:59.000000 zebrazoom-1.9/zebrazoom/configuration/4wellsZebrafishLarvaeEscapeResponses.json
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/configuration/__init__.py
+-rw-rw-rw-   0        0        0      568 2020-04-27 07:27:19.000000 zebrazoom-1.9/zebrazoom/configuration/fliesInTube.json
+-rw-rw-rw-   0        0        0      725 2021-05-05 02:48:22.000000 zebrazoom-1.9/zebrazoom/configuration/headEmbeddedZebrafishLarva.json
+-rw-rw-rw-   0        0        0      767 2021-07-28 08:28:34.000000 zebrazoom-1.9/zebrazoom/configuration/screenFastTrackingConfigFileTemplate.json
+-rw-rw-rw-   0        0        0      569 2021-07-28 11:55:25.000000 zebrazoom-1.9/zebrazoom/configuration/testThresholdsForFastScreen.json
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.774112 zebrazoom-1.9/zebrazoom/dataAnalysis/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.774112 zebrazoom-1.9/zebrazoom/dataAnalysis/classifiers/
+-rw-rw-rw-   0        0        0        0 2020-09-04 15:06:35.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2032 2020-12-14 00:20:56.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/cluster_1a_UsageExample.py
+-rw-rw-rw-   0        0        0     1360 2020-12-14 00:21:04.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/cluster_1b_UsageExampleReloadClassifier.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.774112 zebrazoom-1.9/zebrazoom/dataAnalysis/data/
+-rw-rw-rw-   0        0        0        0 2020-09-04 15:06:35.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/data/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.789761 zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/__init__.py
+-rw-rw-rw-   0        0        0    18511 2021-02-17 12:03:50.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/applyClustering.py
+-rw-rw-rw-   0        0        0     3379 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/createSuperClusterVideo.py
+-rw-rw-rw-   0        0        0     6735 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/outputValidationVideo.py
+-rw-rw-rw-   0        0        0     2252 2021-07-23 16:01:25.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/populationComparaison.py
+-rw-rw-rw-   0        0        0     6582 2020-09-03 13:57:12.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/readValidationVideoDataAnalysis.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.827531 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/__init__.py
+-rw-rw-rw-   0        0        0    13407 2021-07-23 08:09:43.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/createDataFrame.py
+-rw-rw-rw-   0        0        0     1128 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/createDatasetsForExperiments.py
+-rw-rw-rw-   0        0        0      750 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getDeltaHead.py
+-rw-rw-rw-   0        0        0     2659 2020-09-06 10:08:38.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getDynamicParameters.py
+-rw-rw-rw-   0        0        0     2098 2021-07-22 10:34:23.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getGlobalParameters.py
+-rw-rw-rw-   0        0        0      932 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getInstaHeadingDiff.py
+-rw-rw-rw-   0        0        0     1048 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getInstaHorizontalDisplacement.py
+-rw-rw-rw-   0        0        0      993 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getInstaMaxTailBendPos.py
+-rw-rw-rw-   0        0        0      737 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getInstaSpeed.py
+-rw-rw-rw-   0        0        0     2127 2020-06-17 15:02:46.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated.py
+-rw-rw-rw-   0        0        0     1207 2020-12-08 01:15:12.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated2.py
+-rw-rw-rw-   0        0        0     1429 2020-09-06 10:14:33.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getTailAngles.py
+-rw-rw-rw-   0        0        0      190 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getTailLength.py
+-rw-rw-rw-   0        0        0      173 2020-03-24 08:23:13.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getTailLength2.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.843173 zebrazoom-1.9/zebrazoom/dataAnalysis/experimentOrganizationExcel/
+-rw-rw-rw-   0        0        0        0 2020-07-12 14:46:04.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/experimentOrganizationExcel/__init__.py
+-rw-rw-rw-   0        0        0     8192 2020-08-24 14:40:29.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/experimentOrganizationExcel/example.xls
+-rw-rw-rw-   0        0        0     1092 2021-07-22 08:38:38.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/populationCompare_UsageExample.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.843173 zebrazoom-1.9/zebrazoom/dataAnalysis/postProcessingFromCommandLine/
+-rw-rw-rw-   0        0        0        0 2021-07-29 09:07:45.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/postProcessingFromCommandLine/__init__.py
+-rw-rw-rw-   0        0        0     1758 2021-07-29 08:58:46.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/postProcessingFromCommandLine/postProcessingFromCommandLine.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.843173 zebrazoom-1.9/zebrazoom/dataAnalysis/resultsClustering/
+-rw-rw-rw-   0        0        0        0 2020-09-04 15:06:35.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/resultsClustering/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.843173 zebrazoom-1.9/zebrazoom/dataAnalysis/resultsKinematic/
+-rw-rw-rw-   0        0        0        0 2020-09-04 15:06:35.000000 zebrazoom-1.9/zebrazoom/dataAnalysis/resultsKinematic/__init__.py
+-rw-rw-rw-   0        0        0     1393 2021-07-19 13:48:28.000000 zebrazoom-1.9/zebrazoom/extractZZParametersFromTailAngle.py
+-rw-rw-rw-   0        0        0     2809 2021-07-19 13:49:28.000000 zebrazoom-1.9/zebrazoom/getTailExtremityFirstFrame.py
+-rw-rw-rw-   0        0        0    14094 2021-07-28 13:59:34.000000 zebrazoom-1.9/zebrazoom/mainZZ.py
+-rw-rw-rw-   0        0        0     1731 2021-07-19 13:50:11.000000 zebrazoom-1.9/zebrazoom/recreateSuperStruct.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.843173 zebrazoom-1.9/zebrazoom/videoFormatConversion/
+-rw-rw-rw-   0        0        0        0 2020-12-09 01:22:02.000000 zebrazoom-1.9/zebrazoom/videoFormatConversion/__init__.py
+-rw-rw-rw-   0        0        0     2663 2021-03-12 04:51:29.000000 zebrazoom-1.9/zebrazoom/videoFormatConversion/seq_to_avi.py
+drwxrwxrwx   0        0        0        0 2021-07-29 09:11:27.488907 zebrazoom-1.9/zebrazoom.egg-info/
+-rw-rw-rw-   0        0        0      616 2021-07-29 09:11:27.000000 zebrazoom-1.9/zebrazoom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8337 2021-07-29 09:11:27.000000 zebrazoom-1.9/zebrazoom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-29 09:11:27.000000 zebrazoom-1.9/zebrazoom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2021-07-29 09:11:27.000000 zebrazoom-1.9/zebrazoom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2021-07-29 09:11:27.000000 zebrazoom-1.9/zebrazoom.egg-info/top_level.txt
```

### Comparing `zebrazoom-1.8/LICENSE` & `zebrazoom-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/PKG-INFO` & `zebrazoom-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zebrazoom
-Version: 1.8
+Version: 1.9
 Summary: Track and analyze zebrafish and animal behavior
 Home-page: https://github.com/oliviermirat/ZebraZoom
 Author: Olivier Mirat
 Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0
 Download-URL: https://github.com/oliviermirat/ZebraZoom/archive/v1.0.tar.gz
 Description: UNKNOWN
```

### Comparing `zebrazoom-1.8/README.md` & `zebrazoom-1.9/README.md`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/setup.py` & `zebrazoom-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from distutils.core import setup
 setup(
   name = 'zebrazoom',
-  version = '1.08',
+  version = '1.09',
   license='AGPL-3.0',
   description = 'Track and analyze zebrafish and animal behavior',
   author = 'Olivier Mirat',
   author_email = 'olivier.mirat.om@gmail.com',
   url = 'https://github.com/oliviermirat/ZebraZoom',
   download_url = 'https://github.com/oliviermirat/ZebraZoom/archive/v1.0.tar.gz',
   keywords = ['Animal', 'Behavior', 'Tracking', 'Zebrafish'],
```

### Comparing `zebrazoom-1.8/zebrazoom/GUIAllPy.py` & `zebrazoom-1.9/zebrazoom/GUIAllPy.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/ZZoutput/example1/results_example1.txt` & `zebrazoom-1.9/zebrazoom/ZZoutput/example1/results_example1.txt`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/ZZoutput/example2/results_example2.txt` & `zebrazoom-1.9/zebrazoom/ZZoutput/example2/results_example2.txt`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/ZZoutput/example3/results_example3.txt` & `zebrazoom-1.9/zebrazoom/ZZoutput/example3/results_example3.txt`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/__main__.py` & `zebrazoom-1.9/zebrazoom/__main__.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/GUI_InitialClasses.py` & `zebrazoom-1.9/zebrazoom/code/GUI/GUI_InitialClasses.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/GUI_InitialFunctions.py` & `zebrazoom-1.9/zebrazoom/code/GUI/GUI_InitialFunctions.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/adjustParameterInsideAlgo.py` & `zebrazoom-1.9/zebrazoom/code/GUI/adjustParameterInsideAlgo.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/adjustParameterInsideAlgoFunctions.py` & `zebrazoom-1.9/zebrazoom/code/GUI/adjustParameterInsideAlgoFunctions.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/automaticallyFindOptimalParameters.py` & `zebrazoom-1.9/zebrazoom/code/GUI/automaticallyFindOptimalParameters.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/automaticallyFindOptimalParametersFunctions.py` & `zebrazoom-1.9/zebrazoom/code/GUI/automaticallyFindOptimalParametersFunctions.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/blobCenter.png` & `zebrazoom-1.9/zebrazoom/code/GUI/blobCenter.png`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/blobExtremity.png` & `zebrazoom-1.9/zebrazoom/code/GUI/blobExtremity.png`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/configFilePrepare.py` & `zebrazoom-1.9/zebrazoom/code/GUI/configFilePrepare.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/configFilePrepareFunctions.py` & `zebrazoom-1.9/zebrazoom/code/GUI/configFilePrepareFunctions.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/configFileZebrafish.py` & `zebrazoom-1.9/zebrazoom/code/GUI/configFileZebrafish.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/configFileZebrafishFunctions.py` & `zebrazoom-1.9/zebrazoom/code/GUI/configFileZebrafishFunctions.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/dataAnalysisGUI.py` & `zebrazoom-1.9/zebrazoom/code/GUI/dataAnalysisGUI.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/dataAnalysisGUIFunctions.py` & `zebrazoom-1.9/zebrazoom/code/GUI/dataAnalysisGUIFunctions.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/getCoordinates.py` & `zebrazoom-1.9/zebrazoom/code/GUI/getCoordinates.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/leftborder.png` & `zebrazoom-1.9/zebrazoom/code/GUI/leftborder.png`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/no1.png` & `zebrazoom-1.9/zebrazoom/code/GUI/no1.png`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/no2.png` & `zebrazoom-1.9/zebrazoom/code/GUI/no2.png`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/ok1.png` & `zebrazoom-1.9/zebrazoom/code/GUI/ok1.png`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/rightborder.png` & `zebrazoom-1.9/zebrazoom/code/GUI/rightborder.png`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/savedjustincase.png` & `zebrazoom-1.9/zebrazoom/code/GUI/savedjustincase.png`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/troubleshooting.py` & `zebrazoom-1.9/zebrazoom/code/GUI/troubleshooting.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/GUI/troubleshootingFunction.py` & `zebrazoom-1.9/zebrazoom/code/GUI/troubleshootingFunction.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/adjustHyperparameters.py` & `zebrazoom-1.9/zebrazoom/code/adjustHyperparameters.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/createSuperStruct.py` & `zebrazoom-1.9/zebrazoom/code/createSuperStruct.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/createValidationVideo.py` & `zebrazoom-1.9/zebrazoom/code/createValidationVideo.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/dataPostProcessing/computeEyesHeadingPlot.py` & `zebrazoom-1.9/zebrazoom/code/dataPostProcessing/computeEyesHeadingPlot.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/dataPostProcessing/dataPostProcessing.py` & `zebrazoom-1.9/zebrazoom/code/dataPostProcessing/dataPostProcessing.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/dataPostProcessing/findSleepVsMoving.py` & `zebrazoom-1.9/zebrazoom/code/dataPostProcessing/findSleepVsMoving.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/dataPostProcessing/generateAllTimeTailAngleGraph.py` & `zebrazoom-1.9/zebrazoom/code/dataPostProcessing/generateAllTimeTailAngleGraph.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/dataPostProcessing/perBoutOutput.py` & `zebrazoom-1.9/zebrazoom/code/dataPostProcessing/perBoutOutput.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/defaultConfigFile.json` & `zebrazoom-1.9/zebrazoom/code/defaultConfigFile.json`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/detectMovementWithRawVideo.py` & `zebrazoom-1.9/zebrazoom/code/detectMovementWithRawVideo.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/extractParameters.py` & `zebrazoom-1.9/zebrazoom/code/extractParameters.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/fasterMultiprocessing.py` & `zebrazoom-1.9/zebrazoom/code/fasterMultiprocessing.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/findWells.py` & `zebrazoom-1.9/zebrazoom/code/findWells.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getBackground.py` & `zebrazoom-1.9/zebrazoom/code/getBackground.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getHyperparameters.py` & `zebrazoom-1.9/zebrazoom/code/getHyperparameters.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getImage/getForegroundImage.py` & `zebrazoom-1.9/zebrazoom/code/getImage/getForegroundImage.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getImage/getForegroundImageSequential.py` & `zebrazoom-1.9/zebrazoom/code/getImage/getForegroundImageSequential.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getImage/getImage.py` & `zebrazoom-1.9/zebrazoom/code/getImage/getImage.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getImage/getImageSequential.py` & `zebrazoom-1.9/zebrazoom/code/getImage/getImageSequential.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getImage/headEmbededFrame.py` & `zebrazoom-1.9/zebrazoom/code/getImage/headEmbededFrame.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getImage/headEmbededFrameBackExtract.py` & `zebrazoom-1.9/zebrazoom/code/getImage/headEmbededFrameBackExtract.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getImage/headEmbededFrameSequential.py` & `zebrazoom-1.9/zebrazoom/code/getImage/headEmbededFrameSequential.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/getImage/headEmbededFrameSequentialBackExtract.py` & `zebrazoom-1.9/zebrazoom/code/getImage/headEmbededFrameSequentialBackExtract.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/popUpAlgoFollow.py` & `zebrazoom-1.9/zebrazoom/code/popUpAlgoFollow.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/popUpAlgoFollowOldVersion.py` & `zebrazoom-1.9/zebrazoom/code/popUpAlgoFollowOldVersion.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/preprocessImage.py` & `zebrazoom-1.9/zebrazoom/code/preprocessImage.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/readValidationVideo.py` & `zebrazoom-1.9/zebrazoom/code/readValidationVideo.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/resizeImageTooLarge.py` & `zebrazoom-1.9/zebrazoom/code/resizeImageTooLarge.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/blackFramesDetection.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/blackFramesDetection.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/debugTracking.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/debugTracking.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/eyeTracking/eyeTracking.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/eyeTracking/eyeTracking.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/getImages.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/getImages.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/calculateHeading.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/calculateHeading.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/headTrackingHeadingCalculation.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/headTrackingHeadingCalculation.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/headTrackingTakeHeadClosestToWellCenter.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/headTrackingTakeHeadClosestToWellCenter.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/multipleAnimalsHeadTracking.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/multipleAnimalsHeadTracking.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/multipleAnimalsHeadTrackingAdvance.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/headTrackingHeadingCalculationFolder/multipleAnimalsHeadTrackingAdvance.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/postProcessMultipleTrajectories.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/postProcessMultipleTrajectories.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTracking.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTracking.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/centerOfMassTailTracking.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/centerOfMassTailTracking.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/getTailTipManual.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/getTailTipManual.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/headEmbededTailTracking.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/headEmbededTailTracking.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/headEmbededTailTrackingTeresaNicolson.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/headEmbededTailTrackingTeresaNicolson.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingBlobDescent.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingBlobDescent.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/Rotate.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/Rotate.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findBodyContour.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findBodyContour.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/checkIfMidlineIsInBlob.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/checkIfMidlineIsInBlob.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/findTailExtremete.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/findTailExtremete.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/functions.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/functions.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/insideTailExtremete.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTailExtremeteFolder/insideTailExtremete.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTheTwoSides.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/findTheTwoSides.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/getMidline.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/getMidline.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/resampleSeqConstPtsPerArcLength.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/resampleSeqConstPtsPerArcLength.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/tailTrackingExtremityDetect.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tailTrackingFunctionsFolder/tailTrackingExtremityDetectFolder/tailTrackingExtremityDetect.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/tracking.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/tracking.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/trackingFolder/trackingFunctions.py` & `zebrazoom-1.9/zebrazoom/code/trackingFolder/trackingFunctions.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/code/vars.py` & `zebrazoom-1.9/zebrazoom/code/vars.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/configuration/4wellsZebrafishLarvaeEscapeResponses.json` & `zebrazoom-1.9/zebrazoom/configuration/4wellsZebrafishLarvaeEscapeResponses.json`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/configuration/fliesInTube.json` & `zebrazoom-1.9/zebrazoom/configuration/fliesInTube.json`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/configuration/headEmbeddedZebrafishLarva.json` & `zebrazoom-1.9/zebrazoom/configuration/headEmbeddedZebrafishLarva.json`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/configuration/screenFastTrackingConfigFileTemplate.json` & `zebrazoom-1.9/zebrazoom/configuration/screenFastTrackingConfigFileTemplate.json`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/configuration/testThresholdsForFastScreen.json` & `zebrazoom-1.9/zebrazoom/configuration/testThresholdsForFastScreen.json`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/cluster_1a_UsageExample.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/cluster_1a_UsageExample.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/cluster_1b_UsageExampleReloadClassifier.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/cluster_1b_UsageExampleReloadClassifier.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/applyClustering.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/applyClustering.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/createSuperClusterVideo.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/createSuperClusterVideo.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/outputValidationVideo.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/outputValidationVideo.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/populationComparaison.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/populationComparaison.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/dataanalysis/readValidationVideoDataAnalysis.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/dataanalysis/readValidationVideoDataAnalysis.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/createDataFrame.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/createDataFrame.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/createDatasetsForExperiments.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/createDatasetsForExperiments.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getDeltaHead.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getDeltaHead.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getDynamicParameters.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getDynamicParameters.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getGlobalParameters.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getInstaHeadingDiff.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getInstaHeadingDiff.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getInstaHorizontalDisplacement.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getInstaHorizontalDisplacement.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getInstaMaxTailBendPos.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getInstaMaxTailBendPos.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getInstaSpeed.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getInstaSpeed.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated2.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated2.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/datasetcreation/getTailAngles.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/datasetcreation/getTailAngles.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/experimentOrganizationExcel/example.xls` & `zebrazoom-1.9/zebrazoom/dataAnalysis/experimentOrganizationExcel/example.xls`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/dataAnalysis/populationCompare_UsageExample.py` & `zebrazoom-1.9/zebrazoom/dataAnalysis/populationCompare_UsageExample.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/extractZZParametersFromTailAngle.py` & `zebrazoom-1.9/zebrazoom/extractZZParametersFromTailAngle.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/getTailExtremityFirstFrame.py` & `zebrazoom-1.9/zebrazoom/getTailExtremityFirstFrame.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/mainZZ.py` & `zebrazoom-1.9/zebrazoom/mainZZ.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/recreateSuperStruct.py` & `zebrazoom-1.9/zebrazoom/recreateSuperStruct.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom/videoFormatConversion/seq_to_avi.py` & `zebrazoom-1.9/zebrazoom/videoFormatConversion/seq_to_avi.py`

 * *Files identical despite different names*

### Comparing `zebrazoom-1.8/zebrazoom.egg-info/PKG-INFO` & `zebrazoom-1.9/zebrazoom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zebrazoom
-Version: 1.8
+Version: 1.9
 Summary: Track and analyze zebrafish and animal behavior
 Home-page: https://github.com/oliviermirat/ZebraZoom
 Author: Olivier Mirat
 Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0
 Download-URL: https://github.com/oliviermirat/ZebraZoom/archive/v1.0.tar.gz
 Description: UNKNOWN
```

### Comparing `zebrazoom-1.8/zebrazoom.egg-info/SOURCES.txt` & `zebrazoom-1.9/zebrazoom.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -138,11 +138,13 @@
 zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated.py
 zebrazoom/dataAnalysis/datasetcreation/getTailAngleRecalculated2.py
 zebrazoom/dataAnalysis/datasetcreation/getTailAngles.py
 zebrazoom/dataAnalysis/datasetcreation/getTailLength.py
 zebrazoom/dataAnalysis/datasetcreation/getTailLength2.py
 zebrazoom/dataAnalysis/experimentOrganizationExcel/__init__.py
 zebrazoom/dataAnalysis/experimentOrganizationExcel/example.xls
+zebrazoom/dataAnalysis/postProcessingFromCommandLine/__init__.py
+zebrazoom/dataAnalysis/postProcessingFromCommandLine/postProcessingFromCommandLine.py
 zebrazoom/dataAnalysis/resultsClustering/__init__.py
 zebrazoom/dataAnalysis/resultsKinematic/__init__.py
 zebrazoom/videoFormatConversion/__init__.py
 zebrazoom/videoFormatConversion/seq_to_avi.py
```

