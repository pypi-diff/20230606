# Comparing `tmp/SoccerNet-0.1.8.tar.gz` & `tmp/SoccerNet-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SoccerNet-0.1.8.tar", last modified: Thu Oct  7 13:50:43 2021, max compression
+gzip compressed data, was "SoccerNet-0.1.9.tar", last modified: Thu Jan  6 09:07:05 2022, max compression
```

## Comparing `SoccerNet-0.1.8.tar` & `SoccerNet-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2021-10-07 13:50:43.741943 SoccerNet-0.1.8/
--rw-r--r--   0 giancos  (47541975) 1840429327      655 2021-09-29 08:49:20.000000 SoccerNet-0.1.8/MANIFEST.in
--rw-r--r--   0 giancos  (47541975) 1840429327     9930 2021-10-07 13:50:43.742208 SoccerNet-0.1.8/PKG-INFO
--rw-r--r--   0 giancos  (47541975) 1840429327     3051 2021-10-07 13:31:31.000000 SoccerNet-0.1.8/README.md
-drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2021-10-07 13:50:43.730258 SoccerNet-0.1.8/SoccerNet/
--rw-r--r--   0 giancos  (47541975) 1840429327    14172 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/DataLoader.py
--rw-r--r--   0 giancos  (47541975) 1840429327     1839 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/DataLoaderTensorFlow.py
--rw-r--r--   0 giancos  (47541975) 1840429327    11501 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/DataLoaderTorch.py
--rw-r--r--   0 giancos  (47541975) 1840429327    15467 2021-10-07 13:35:05.000000 SoccerNet-0.1.8/SoccerNet/Downloader.py
-drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2021-10-07 13:50:43.733959 SoccerNet-0.1.8/SoccerNet/Evaluation/
--rw-r--r--   0 giancos  (47541975) 1840429327    19166 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/Evaluation/ActionSpotting.py
--rw-r--r--   0 giancos  (47541975) 1840429327    14545 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/Evaluation/ReplayGrounding.py
--rw-r--r--   0 giancos  (47541975) 1840429327     6330 2021-09-29 08:49:20.000000 SoccerNet-0.1.8/SoccerNet/Evaluation/utils.py
--rw-r--r--   0 giancos  (47541975) 1840429327     8993 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/Feature.py
--rw-r--r--   0 giancos  (47541975) 1840429327     1308 2021-10-07 13:48:53.000000 SoccerNet-0.1.8/SoccerNet/__init__.py
-drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2021-10-07 13:50:43.741600 SoccerNet-0.1.8/SoccerNet/data/
--rw-r--r--   0 giancos  (47541975) 1840429327     3338 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetCameraChangesChallenge.json
--rw-r--r--   0 giancos  (47541975) 1840429327     3057 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetCameraChangesTest.json
--rw-r--r--   0 giancos  (47541975) 1840429327     7913 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetCameraChangesTrain.json
--rw-r--r--   0 giancos  (47541975) 1840429327     3035 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetCameraChangesValid.json
--rw-r--r--   0 giancos  (47541975) 1840429327     3199 2021-09-29 08:49:20.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetFramesChallenge.json
--rw-r--r--   0 giancos  (47541975) 1840429327     4076 2021-09-29 08:49:20.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetFramesTest.json
--rw-r--r--   0 giancos  (47541975) 1840429327    18269 2021-09-29 08:49:20.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetFramesTrain.json
--rw-r--r--   0 giancos  (47541975) 1840429327     3946 2021-09-29 08:49:20.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetFramesValid.json
--rw-r--r--   0 giancos  (47541975) 1840429327     3338 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetGamesChallenge.json
--rw-r--r--   0 giancos  (47541975) 1840429327     6762 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetGamesTest.json
--rw-r--r--   0 giancos  (47541975) 1840429327    18769 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetGamesTrain.json
--rw-r--r--   0 giancos  (47541975) 1840429327     6808 2021-06-21 12:40:47.000000 SoccerNet-0.1.8/SoccerNet/data/SoccerNetGamesValid.json
--rw-r--r--   0 giancos  (47541975) 1840429327     2763 2021-09-29 09:42:55.000000 SoccerNet-0.1.8/SoccerNet/utils.py
-drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2021-10-07 13:50:43.731760 SoccerNet-0.1.8/SoccerNet.egg-info/
--rw-r--r--   0 giancos  (47541975) 1840429327     9930 2021-10-07 13:50:42.000000 SoccerNet-0.1.8/SoccerNet.egg-info/PKG-INFO
--rw-r--r--   0 giancos  (47541975) 1840429327     1011 2021-10-07 13:50:42.000000 SoccerNet-0.1.8/SoccerNet.egg-info/SOURCES.txt
--rw-r--r--   0 giancos  (47541975) 1840429327        1 2021-10-07 13:50:42.000000 SoccerNet-0.1.8/SoccerNet.egg-info/dependency_links.txt
--rw-r--r--   0 giancos  (47541975) 1840429327       46 2021-10-07 13:50:42.000000 SoccerNet-0.1.8/SoccerNet.egg-info/requires.txt
--rw-r--r--   0 giancos  (47541975) 1840429327       10 2021-10-07 13:50:42.000000 SoccerNet-0.1.8/SoccerNet.egg-info/top_level.txt
--rw-r--r--   0 giancos  (47541975) 1840429327       79 2021-10-07 13:50:43.742875 SoccerNet-0.1.8/setup.cfg
--rw-r--r--   0 giancos  (47541975) 1840429327     3890 2021-10-07 13:36:21.000000 SoccerNet-0.1.8/setup.py
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2022-01-06 09:07:05.886833 SoccerNet-0.1.9/
+-rw-r--r--   0 giancos  (47541975) 1840429327     1068 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/LICENSE.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327      655 2021-09-29 08:49:20.000000 SoccerNet-0.1.9/MANIFEST.in
+-rw-r--r--   0 giancos  (47541975) 1840429327     9952 2022-01-06 09:07:05.887230 SoccerNet-0.1.9/PKG-INFO
+-rw-r--r--   0 giancos  (47541975) 1840429327     3110 2022-01-06 09:03:56.000000 SoccerNet-0.1.9/README.md
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2022-01-06 09:07:05.862326 SoccerNet-0.1.9/SoccerNet/
+-rw-r--r--   0 giancos  (47541975) 1840429327    14172 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/DataLoader.py
+-rw-r--r--   0 giancos  (47541975) 1840429327     1839 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/DataLoaderTensorFlow.py
+-rw-r--r--   0 giancos  (47541975) 1840429327    11501 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/DataLoaderTorch.py
+-rw-r--r--   0 giancos  (47541975) 1840429327    15467 2021-10-07 13:35:05.000000 SoccerNet-0.1.9/SoccerNet/Downloader.py
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2022-01-06 09:07:05.869640 SoccerNet-0.1.9/SoccerNet/Evaluation/
+-rw-r--r--   0 giancos  (47541975) 1840429327    19166 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/Evaluation/ActionSpotting.py
+-rw-r--r--   0 giancos  (47541975) 1840429327    14545 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/Evaluation/ReplayGrounding.py
+-rw-r--r--   0 giancos  (47541975) 1840429327     6330 2021-09-29 08:49:20.000000 SoccerNet-0.1.9/SoccerNet/Evaluation/utils.py
+-rw-r--r--   0 giancos  (47541975) 1840429327     8993 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/Feature.py
+-rw-r--r--   0 giancos  (47541975) 1840429327     1308 2022-01-06 09:05:32.000000 SoccerNet-0.1.9/SoccerNet/__init__.py
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2022-01-06 09:07:05.885120 SoccerNet-0.1.9/SoccerNet/data/
+-rw-r--r--   0 giancos  (47541975) 1840429327     3338 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetCameraChangesChallenge.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     3057 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetCameraChangesTest.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     7913 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetCameraChangesTrain.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     3035 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetCameraChangesValid.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     3199 2021-09-29 08:49:20.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetFramesChallenge.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     4076 2021-09-29 08:49:20.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetFramesTest.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    18269 2021-09-29 08:49:20.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetFramesTrain.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     3946 2021-09-29 08:49:20.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetFramesValid.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     3338 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetGamesChallenge.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     6762 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetGamesTest.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    18769 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetGamesTrain.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     6808 2021-06-21 12:40:47.000000 SoccerNet-0.1.9/SoccerNet/data/SoccerNetGamesValid.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     2763 2021-09-29 09:42:55.000000 SoccerNet-0.1.9/SoccerNet/utils.py
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2022-01-06 09:07:05.866351 SoccerNet-0.1.9/SoccerNet.egg-info/
+-rw-r--r--   0 giancos  (47541975) 1840429327     9952 2022-01-06 09:07:05.000000 SoccerNet-0.1.9/SoccerNet.egg-info/PKG-INFO
+-rw-r--r--   0 giancos  (47541975) 1840429327     1023 2022-01-06 09:07:05.000000 SoccerNet-0.1.9/SoccerNet.egg-info/SOURCES.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327        1 2022-01-06 09:07:05.000000 SoccerNet-0.1.9/SoccerNet.egg-info/dependency_links.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327       46 2022-01-06 09:07:05.000000 SoccerNet-0.1.9/SoccerNet.egg-info/requires.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327       10 2022-01-06 09:07:05.000000 SoccerNet-0.1.9/SoccerNet.egg-info/top_level.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327       79 2022-01-06 09:07:05.888514 SoccerNet-0.1.9/setup.cfg
+-rw-r--r--   0 giancos  (47541975) 1840429327     3890 2021-10-07 13:36:21.000000 SoccerNet-0.1.9/setup.py
```

### Comparing `SoccerNet-0.1.8/MANIFEST.in` & `SoccerNet-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/PKG-INFO` & `SoccerNet-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,15 @@
 Metadata-Version: 2.1
 Name: SoccerNet
-Version: 0.1.8
+Version: 0.1.9
 Summary: SoccerNet SDK
 Home-page: https://github.com/SilvioGiancola/SoccerNetv2
 Author: Silvio Giancola
 Author-email: silvio.giancola@kaust.edu.sa
 License: MIT
-Description: # SOCCERNETV2
-        
-        ```bash
-        conda create -n SoccerNet python pip
-        pip install SoccerNet
-        ```
-        
-        ## Structure of the data data for each game
-        
-        - SoccerNet main folder
-          - Leagues (england_epl/europe_uefa-champions-league/france_ligue-1/...)
-            - Seasons (2014-2015/2015-2016/2016-2017)
-              - Games (format: "{Date} - {Time} - {HomeTeam} {Score} {AwayTeam}")
-                - SoccerNet-v2 - Labels / Manual Annotations
-                  - **video.ini**: information on start/duration for each half of the game in the HQ video, in second
-                  - **Labels-v2.json**: Labels from SoccerNet-v2 - action spotting
-                  - **Labels-cameras.json**: Labels from SoccerNet-v1 - camera shot segmentation
-        
-                - SoccerNet-v2 - Videos / Automatically Extracted Features
-                  - **1_HQ.mkv**: HQ video 1st half
-                  - **2_HQ.mkv**: HQ video 2nd half
-                  - **1.mkv**: LQ video 1st half - timmed with start/duration from HQ video - resolution 224*398 - 25 fps
-                  - **2.mkv**: LQ video 2nd half - timmed with start/duration from HQ video - resolution 224*398 - 25 fps
-                  - **1_ResNET_TF2.npy**: ResNET features @2fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **2_ResNET_TF2.npy**: ResNET features @2fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **1_ResNET_TF2_PCA512.npy**: ResNET features @2fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
-                  - **2_ResNET_TF2_PCA512.npy**: ResNET features @2fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
-                  - **1_ResNET_5fps_TF2.npy**: ResNET features @5fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **2_ResNET_5fps_TF2.npy**: ResNET features @5fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **1_ResNET_5fps_TF2_PCA512.npy**: ResNET features @5fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
-                  - **2_ResNET_5fps_TF2_PCA512.npy**: ResNET features @5fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
-                  - **1_ResNET_25fps_TF2.npy**: ResNET features @25fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **2_ResNET_25fps_TF2.npy**: ResNET features @25fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **1_player_boundingbox_maskrcnn.json**: Player Bounding Boxes @2fps for 1st half, extracted with MaskRCNN
-                  - **2_player_boundingbox_maskrcnn.json**: Player Bounding Boxes @2fps for 2nd half, extracted with MaskRCNN
-                  - **1_field_calib_ccbv.json**: Field Camera Calibration @2fps for 1st half, extracted with CCBV
-                  - **2_field_calib_ccbv.json**: Field Camera Calibration @2fps for 2nd half, extracted with CCBV
-        
-                - Legacy from SoccerNet-v1
-                  - **Labels.json**: Labels from SoccerNet-v1 - action spotting for goals/cards/subs only
-                  - **1_C3D.npy**: C3D features @2fps for 1st half from SoccerNet-v1
-                  - **2_C3D.npy**: C3D features @2fps for 2nd half from SoccerNet-v1
-                  - **1_C3D_PCA512.npy**: C3D features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **2_C3D_PCA512.npy**: C3D features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **1_I3D.npy**: I3D features @2fps for 1st half from SoccerNet-v1
-                  - **2_I3D.npy**: I3D features @2fps for 2nd half from SoccerNet-v1
-                  - **1_I3D_PCA512.npy**: I3D features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **2_I3D_PCA512.npy**: I3D features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **1_ResNET.npy**: ResNET features @2fps for 1st half from SoccerNet-v1
-                  - **2_ResNET.npy**: ResNET features @2fps for 2nd half from SoccerNet-v1
-                  - **1_ResNET_PCA512.npy**: ResNET features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **2_ResNET_PCA512.npy**: ResNET features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-        
-        
-        ## How to Download Games (Python)
-        
-        ```python
-        from SoccerNet.Downloader import SoccerNetDownloader
-        
-        mySoccerNetDownloader = SoccerNetDownloader(LocalDirectory="path/to/soccernet")
-        
-        # Download SoccerNet labels
-        mySoccerNetDownloader.downloadGames(files=["Labels.json"], split=["train","valid","test"]) # download labels
-        mySoccerNetDownloader.downloadGames(files=["Labels-v2.json"], split=["train","valid","test"]) # download labels SN v2
-        mySoccerNetDownloader.downloadGames(files=["Labels-cameras.json"], split=["train","valid","test"]) # download labels for camera shot
-        
-        # Download SoccerNet features
-        mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2.npy", "2_ResNET_TF2.npy"], split=["train","valid","test"]) # download Features
-        mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2_PCA512.npy", "2_ResNET_TF2_PCA512.npy"], split=["train","valid","test"]) # download Features reduced with PCA
-        mySoccerNetDownloader.downloadGames(files=["1_player_boundingbox_maskrcnn.json", "2_player_boundingbox_maskrcnn.json"], split=["train","valid","test"]) # download Player Bounding Boxes inferred with MaskRCNN
-        mySoccerNetDownloader.downloadGames(files=["1_field_calib_ccbv.json", "2_field_calib_ccbv.json"], split=["train","valid","test"]) # download Field Calibration inferred with CCBV
-        
-        # Download SoccerNet videos (require password from NDA to download videos)
-        mySoccerNetDownloader.password = input("Password for videos? (contact the author):\n")
-        mySoccerNetDownloader.downloadGames(files=["1.mkv", "2.mkv"], split=["train","valid","test"]) # download LQ Videos
-        mySoccerNetDownloader.downloadGames(files=["1_HQ.mkv", "2_HQ.mkv", "video.ini"], split=["train","valid","test"]) # download HQ Videos
-        
-        # Download SoccerNet Challenge set (require password from NDA to download videos)
-        mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2.npy", "2_ResNET_TF2.npy"], split=["challenge"]) # download ResNET Features
-        mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2_PCA512.npy", "2_ResNET_TF2_PCA512.npy"], split=["challenge"]) # download ResNET Features reduced with PCA
-        mySoccerNetDownloader.downloadGames(files=["1.mkv", "2.mkv", "video.ini"], split=["challenge"]) # download LQ Videos (require password from NDA)
-        mySoccerNetDownloader.downloadGames(files=["1_HQ.mkv", "2_HQ.mkv", "video.ini"], split=["challenge"]) # download HQ Videos (require password from NDA)
-        mySoccerNetDownloader.downloadGames(files=["1_player_boundingbox_maskrcnn.json", "2_player_boundingbox_maskrcnn.json"], split=["challenge"]) # download Player Bounding Boxes inferred with MaskRCNN 
-        mySoccerNetDownloader.downloadGames(files=["1_field_calib_ccbv.json", "2_field_calib_ccbv.json"], split=["challenge"]) # download Field Calibration inferred with CCBV 
-        
-        ```
-        
-        ## How to read the list Games (Python)
-        
-        ```python
-        from SoccerNet.utils import getListGames
-        print(getListGames(split="train")) # return list of games recommended for training
-        print(getListGames(split="valid")) # return list of games recommended for validation
-        print(getListGames(split="test")) # return list of games recommended for testing
-        print(getListGames(split="challenge")) # return list of games recommended for challenge
-        print(getListGames(split=["train", "valid", "test", "challenge"])) # return list of games for training, validation and testing
-        print(getListGames(split="v1")) # return list of games from SoccerNetv1 (train/valid/test)
-        ```
-        
-        
-        
 Keywords: SoccerNet,SDK,Spotting,Football,Soccer,Video
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -118,7 +17,115 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# SOCCERNETV2
+
+```bash
+conda create -n SoccerNet python pip
+pip install SoccerNet
+```
+
+## Structure of the data data for each game
+
+- SoccerNet main folder
+  - Leagues (england_epl/europe_uefa-champions-league/france_ligue-1/...)
+    - Seasons (2014-2015/2015-2016/2016-2017)
+      - Games (format: "{Date} - {Time} - {HomeTeam} {Score} {AwayTeam}")
+        - SoccerNet-v2 - Labels / Manual Annotations
+          - **video.ini**: information on start/duration for each half of the game in the HQ video, in second
+          - **Labels-v2.json**: Labels from SoccerNet-v2 - action spotting
+          - **Labels-cameras.json**: Labels from SoccerNet-v1 - camera shot segmentation
+
+        - SoccerNet-v2 - Videos / Automatically Extracted Features
+          - **1_HQ.mkv**: HQ video 1st half
+          - **2_HQ.mkv**: HQ video 2nd half
+          - **1.mkv**: LQ video 1st half - timmed with start/duration from HQ video - resolution 224*398 - 25 fps
+          - **2.mkv**: LQ video 2nd half - timmed with start/duration from HQ video - resolution 224*398 - 25 fps
+          - **1_ResNET_TF2.npy**: ResNET features @2fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **2_ResNET_TF2.npy**: ResNET features @2fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **1_ResNET_TF2_PCA512.npy**: ResNET features @2fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
+          - **2_ResNET_TF2_PCA512.npy**: ResNET features @2fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
+          - **1_ResNET_5fps_TF2.npy**: ResNET features @5fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **2_ResNET_5fps_TF2.npy**: ResNET features @5fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **1_ResNET_5fps_TF2_PCA512.npy**: ResNET features @5fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
+          - **2_ResNET_5fps_TF2_PCA512.npy**: ResNET features @5fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
+          - **1_ResNET_25fps_TF2.npy**: ResNET features @25fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **2_ResNET_25fps_TF2.npy**: ResNET features @25fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **1_player_boundingbox_maskrcnn.json**: Player Bounding Boxes @2fps for 1st half, extracted with MaskRCNN
+          - **2_player_boundingbox_maskrcnn.json**: Player Bounding Boxes @2fps for 2nd half, extracted with MaskRCNN
+          - **1_field_calib_ccbv.json**: Field Camera Calibration @2fps for 1st half, extracted with CCBV
+          - **2_field_calib_ccbv.json**: Field Camera Calibration @2fps for 2nd half, extracted with CCBV
+          - **1_baidu_soccer_embeddings.npy**: Frame Embeddings for 1st half from [https://github.com/baidu-research/vidpress-sports](https://github.com/baidu-research/vidpress-sports)
+          - **2_baidu_soccer_embeddings.npy**: Frame Embeddings for 2nd half from [https://github.com/baidu-research/vidpress-sports](https://github.com/baidu-research/vidpress-sports)
+
+        - Legacy from SoccerNet-v1
+          - **Labels.json**: Labels from SoccerNet-v1 - action spotting for goals/cards/subs only
+          - **1_C3D.npy**: C3D features @2fps for 1st half from SoccerNet-v1
+          - **2_C3D.npy**: C3D features @2fps for 2nd half from SoccerNet-v1
+          - **1_C3D_PCA512.npy**: C3D features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **2_C3D_PCA512.npy**: C3D features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **1_I3D.npy**: I3D features @2fps for 1st half from SoccerNet-v1
+          - **2_I3D.npy**: I3D features @2fps for 2nd half from SoccerNet-v1
+          - **1_I3D_PCA512.npy**: I3D features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **2_I3D_PCA512.npy**: I3D features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **1_ResNET.npy**: ResNET features @2fps for 1st half from SoccerNet-v1
+          - **2_ResNET.npy**: ResNET features @2fps for 2nd half from SoccerNet-v1
+          - **1_ResNET_PCA512.npy**: ResNET features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **2_ResNET_PCA512.npy**: ResNET features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+
+
+## How to Download Games (Python)
+
+```python
+from SoccerNet.Downloader import SoccerNetDownloader
+
+mySoccerNetDownloader = SoccerNetDownloader(LocalDirectory="path/to/soccernet")
+
+# Download SoccerNet labels
+mySoccerNetDownloader.downloadGames(files=["Labels.json"], split=["train","valid","test"]) # download labels
+mySoccerNetDownloader.downloadGames(files=["Labels-v2.json"], split=["train","valid","test"]) # download labels SN v2
+mySoccerNetDownloader.downloadGames(files=["Labels-cameras.json"], split=["train","valid","test"]) # download labels for camera shot
+
+# Download SoccerNet features
+mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2.npy", "2_ResNET_TF2.npy"], split=["train","valid","test"]) # download Features
+mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2_PCA512.npy", "2_ResNET_TF2_PCA512.npy"], split=["train","valid","test"]) # download Features reduced with PCA
+mySoccerNetDownloader.downloadGames(files=["1_player_boundingbox_maskrcnn.json", "2_player_boundingbox_maskrcnn.json"], split=["train","valid","test"]) # download Player Bounding Boxes inferred with MaskRCNN
+mySoccerNetDownloader.downloadGames(files=["1_field_calib_ccbv.json", "2_field_calib_ccbv.json"], split=["train","valid","test"]) # download Field Calibration inferred with CCBV
+mySoccerNetDownloader.downloadGames(files=["1_baidu_soccer_embeddings.npy","2_baidu_soccer_embeddings.npy"], split=["train","valid","test"]) # download Frame Embeddings from https://github.com/baidu-research/vidpress-sports
+
+# Download SoccerNet videos (require password from NDA to download videos)
+mySoccerNetDownloader.password = input("Password for videos? (contact the author):\n")
+mySoccerNetDownloader.downloadGames(files=["1.mkv", "2.mkv"], split=["train","valid","test"]) # download LQ Videos
+mySoccerNetDownloader.downloadGames(files=["1_HQ.mkv", "2_HQ.mkv", "video.ini"], split=["train","valid","test"]) # download HQ Videos
+
+# Download SoccerNet Challenge set (require password from NDA to download videos)
+mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2.npy", "2_ResNET_TF2.npy"], split=["challenge"]) # download ResNET Features
+mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2_PCA512.npy", "2_ResNET_TF2_PCA512.npy"], split=["challenge"]) # download ResNET Features reduced with PCA
+mySoccerNetDownloader.downloadGames(files=["1.mkv", "2.mkv", "video.ini"], split=["challenge"]) # download LQ Videos (require password from NDA)
+mySoccerNetDownloader.downloadGames(files=["1_HQ.mkv", "2_HQ.mkv", "video.ini"], split=["challenge"]) # download HQ Videos (require password from NDA)
+mySoccerNetDownloader.downloadGames(files=["1_player_boundingbox_maskrcnn.json", "2_player_boundingbox_maskrcnn.json"], split=["challenge"]) # download Player Bounding Boxes inferred with MaskRCNN 
+mySoccerNetDownloader.downloadGames(files=["1_field_calib_ccbv.json", "2_field_calib_ccbv.json"], split=["challenge"]) # download Field Calibration inferred with CCBV 
+mySoccerNetDownloader.downloadGames(files=["1_baidu_soccer_embeddings.npy","2_baidu_soccer_embeddings.npy"], split=["challenge"]) # download Frame Embeddings from https://github.com/baidu-research/vidpress-sports
+
+```
+
+## How to read the list Games (Python)
+
+```python
+from SoccerNet.utils import getListGames
+print(getListGames(split="train")) # return list of games recommended for training
+print(getListGames(split="valid")) # return list of games recommended for validation
+print(getListGames(split="test")) # return list of games recommended for testing
+print(getListGames(split="challenge")) # return list of games recommended for challenge
+print(getListGames(split=["train", "valid", "test", "challenge"])) # return list of games for training, validation and testing
+print(getListGames(split="v1")) # return list of games from SoccerNetv1 (train/valid/test)
+```
+
+
+
+
```

### Comparing `SoccerNet-0.1.8/README.md` & `SoccerNet-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -81,7 +81,13 @@
 # pip cudnn cudatoolkit=10.1
 pip install tensorflow
 pip install pytorch torchvision cudatoolkit=10.1
 pip install av
 
 # conda install pytorch torchvision cudatoolkit=10.1 -c pytorch
 ```
+
+## Update pip package
+
+```bash
+python setup.py upload
+```
```

### Comparing `SoccerNet-0.1.8/SoccerNet/DataLoader.py` & `SoccerNet-0.1.9/SoccerNet/DataLoader.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/DataLoaderTensorFlow.py` & `SoccerNet-0.1.9/SoccerNet/DataLoaderTensorFlow.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/DataLoaderTorch.py` & `SoccerNet-0.1.9/SoccerNet/DataLoaderTorch.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/Downloader.py` & `SoccerNet-0.1.9/SoccerNet/Downloader.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/Evaluation/ActionSpotting.py` & `SoccerNet-0.1.9/SoccerNet/Evaluation/ActionSpotting.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/Evaluation/ReplayGrounding.py` & `SoccerNet-0.1.9/SoccerNet/Evaluation/ReplayGrounding.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/Evaluation/utils.py` & `SoccerNet-0.1.9/SoccerNet/Evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/Feature.py` & `SoccerNet-0.1.9/SoccerNet/Feature.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/__init__.py` & `SoccerNet-0.1.9/SoccerNet/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version_info__ = ('0', '1', '8')
+__version_info__ = ('0', '1', '9')
 __version__ = '.'.join(__version_info__)
 __authors__ = "Silvio Giancola"
 __authors_username__ = "giancos"
 __author_email__ = "silvio.giancola@kaust.edu.sa"
 __github__ = 'https://github.com/SilvioGiancola/SoccerNetv2'
```

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetCameraChangesChallenge.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetCameraChangesChallenge.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetCameraChangesTest.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetCameraChangesTest.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetCameraChangesTrain.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetCameraChangesTrain.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetCameraChangesValid.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetCameraChangesValid.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetFramesChallenge.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetFramesChallenge.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetFramesTest.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetFramesTest.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetFramesTrain.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetFramesTrain.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetFramesValid.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetFramesValid.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetGamesChallenge.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetGamesChallenge.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetGamesTest.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetGamesTest.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetGamesTrain.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetGamesTrain.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/data/SoccerNetGamesValid.json` & `SoccerNet-0.1.9/SoccerNet/data/SoccerNetGamesValid.json`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet/utils.py` & `SoccerNet-0.1.9/SoccerNet/utils.py`

 * *Files identical despite different names*

### Comparing `SoccerNet-0.1.8/SoccerNet.egg-info/PKG-INFO` & `SoccerNet-0.1.9/SoccerNet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,15 @@
 Metadata-Version: 2.1
 Name: SoccerNet
-Version: 0.1.8
+Version: 0.1.9
 Summary: SoccerNet SDK
 Home-page: https://github.com/SilvioGiancola/SoccerNetv2
 Author: Silvio Giancola
 Author-email: silvio.giancola@kaust.edu.sa
 License: MIT
-Description: # SOCCERNETV2
-        
-        ```bash
-        conda create -n SoccerNet python pip
-        pip install SoccerNet
-        ```
-        
-        ## Structure of the data data for each game
-        
-        - SoccerNet main folder
-          - Leagues (england_epl/europe_uefa-champions-league/france_ligue-1/...)
-            - Seasons (2014-2015/2015-2016/2016-2017)
-              - Games (format: "{Date} - {Time} - {HomeTeam} {Score} {AwayTeam}")
-                - SoccerNet-v2 - Labels / Manual Annotations
-                  - **video.ini**: information on start/duration for each half of the game in the HQ video, in second
-                  - **Labels-v2.json**: Labels from SoccerNet-v2 - action spotting
-                  - **Labels-cameras.json**: Labels from SoccerNet-v1 - camera shot segmentation
-        
-                - SoccerNet-v2 - Videos / Automatically Extracted Features
-                  - **1_HQ.mkv**: HQ video 1st half
-                  - **2_HQ.mkv**: HQ video 2nd half
-                  - **1.mkv**: LQ video 1st half - timmed with start/duration from HQ video - resolution 224*398 - 25 fps
-                  - **2.mkv**: LQ video 2nd half - timmed with start/duration from HQ video - resolution 224*398 - 25 fps
-                  - **1_ResNET_TF2.npy**: ResNET features @2fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **2_ResNET_TF2.npy**: ResNET features @2fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **1_ResNET_TF2_PCA512.npy**: ResNET features @2fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
-                  - **2_ResNET_TF2_PCA512.npy**: ResNET features @2fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
-                  - **1_ResNET_5fps_TF2.npy**: ResNET features @5fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **2_ResNET_5fps_TF2.npy**: ResNET features @5fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **1_ResNET_5fps_TF2_PCA512.npy**: ResNET features @5fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
-                  - **2_ResNET_5fps_TF2_PCA512.npy**: ResNET features @5fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
-                  - **1_ResNET_25fps_TF2.npy**: ResNET features @25fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **2_ResNET_25fps_TF2.npy**: ResNET features @25fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
-                  - **1_player_boundingbox_maskrcnn.json**: Player Bounding Boxes @2fps for 1st half, extracted with MaskRCNN
-                  - **2_player_boundingbox_maskrcnn.json**: Player Bounding Boxes @2fps for 2nd half, extracted with MaskRCNN
-                  - **1_field_calib_ccbv.json**: Field Camera Calibration @2fps for 1st half, extracted with CCBV
-                  - **2_field_calib_ccbv.json**: Field Camera Calibration @2fps for 2nd half, extracted with CCBV
-        
-                - Legacy from SoccerNet-v1
-                  - **Labels.json**: Labels from SoccerNet-v1 - action spotting for goals/cards/subs only
-                  - **1_C3D.npy**: C3D features @2fps for 1st half from SoccerNet-v1
-                  - **2_C3D.npy**: C3D features @2fps for 2nd half from SoccerNet-v1
-                  - **1_C3D_PCA512.npy**: C3D features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **2_C3D_PCA512.npy**: C3D features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **1_I3D.npy**: I3D features @2fps for 1st half from SoccerNet-v1
-                  - **2_I3D.npy**: I3D features @2fps for 2nd half from SoccerNet-v1
-                  - **1_I3D_PCA512.npy**: I3D features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **2_I3D_PCA512.npy**: I3D features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **1_ResNET.npy**: ResNET features @2fps for 1st half from SoccerNet-v1
-                  - **2_ResNET.npy**: ResNET features @2fps for 2nd half from SoccerNet-v1
-                  - **1_ResNET_PCA512.npy**: ResNET features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-                  - **2_ResNET_PCA512.npy**: ResNET features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
-        
-        
-        ## How to Download Games (Python)
-        
-        ```python
-        from SoccerNet.Downloader import SoccerNetDownloader
-        
-        mySoccerNetDownloader = SoccerNetDownloader(LocalDirectory="path/to/soccernet")
-        
-        # Download SoccerNet labels
-        mySoccerNetDownloader.downloadGames(files=["Labels.json"], split=["train","valid","test"]) # download labels
-        mySoccerNetDownloader.downloadGames(files=["Labels-v2.json"], split=["train","valid","test"]) # download labels SN v2
-        mySoccerNetDownloader.downloadGames(files=["Labels-cameras.json"], split=["train","valid","test"]) # download labels for camera shot
-        
-        # Download SoccerNet features
-        mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2.npy", "2_ResNET_TF2.npy"], split=["train","valid","test"]) # download Features
-        mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2_PCA512.npy", "2_ResNET_TF2_PCA512.npy"], split=["train","valid","test"]) # download Features reduced with PCA
-        mySoccerNetDownloader.downloadGames(files=["1_player_boundingbox_maskrcnn.json", "2_player_boundingbox_maskrcnn.json"], split=["train","valid","test"]) # download Player Bounding Boxes inferred with MaskRCNN
-        mySoccerNetDownloader.downloadGames(files=["1_field_calib_ccbv.json", "2_field_calib_ccbv.json"], split=["train","valid","test"]) # download Field Calibration inferred with CCBV
-        
-        # Download SoccerNet videos (require password from NDA to download videos)
-        mySoccerNetDownloader.password = input("Password for videos? (contact the author):\n")
-        mySoccerNetDownloader.downloadGames(files=["1.mkv", "2.mkv"], split=["train","valid","test"]) # download LQ Videos
-        mySoccerNetDownloader.downloadGames(files=["1_HQ.mkv", "2_HQ.mkv", "video.ini"], split=["train","valid","test"]) # download HQ Videos
-        
-        # Download SoccerNet Challenge set (require password from NDA to download videos)
-        mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2.npy", "2_ResNET_TF2.npy"], split=["challenge"]) # download ResNET Features
-        mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2_PCA512.npy", "2_ResNET_TF2_PCA512.npy"], split=["challenge"]) # download ResNET Features reduced with PCA
-        mySoccerNetDownloader.downloadGames(files=["1.mkv", "2.mkv", "video.ini"], split=["challenge"]) # download LQ Videos (require password from NDA)
-        mySoccerNetDownloader.downloadGames(files=["1_HQ.mkv", "2_HQ.mkv", "video.ini"], split=["challenge"]) # download HQ Videos (require password from NDA)
-        mySoccerNetDownloader.downloadGames(files=["1_player_boundingbox_maskrcnn.json", "2_player_boundingbox_maskrcnn.json"], split=["challenge"]) # download Player Bounding Boxes inferred with MaskRCNN 
-        mySoccerNetDownloader.downloadGames(files=["1_field_calib_ccbv.json", "2_field_calib_ccbv.json"], split=["challenge"]) # download Field Calibration inferred with CCBV 
-        
-        ```
-        
-        ## How to read the list Games (Python)
-        
-        ```python
-        from SoccerNet.utils import getListGames
-        print(getListGames(split="train")) # return list of games recommended for training
-        print(getListGames(split="valid")) # return list of games recommended for validation
-        print(getListGames(split="test")) # return list of games recommended for testing
-        print(getListGames(split="challenge")) # return list of games recommended for challenge
-        print(getListGames(split=["train", "valid", "test", "challenge"])) # return list of games for training, validation and testing
-        print(getListGames(split="v1")) # return list of games from SoccerNetv1 (train/valid/test)
-        ```
-        
-        
-        
 Keywords: SoccerNet,SDK,Spotting,Football,Soccer,Video
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -118,7 +17,115 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# SOCCERNETV2
+
+```bash
+conda create -n SoccerNet python pip
+pip install SoccerNet
+```
+
+## Structure of the data data for each game
+
+- SoccerNet main folder
+  - Leagues (england_epl/europe_uefa-champions-league/france_ligue-1/...)
+    - Seasons (2014-2015/2015-2016/2016-2017)
+      - Games (format: "{Date} - {Time} - {HomeTeam} {Score} {AwayTeam}")
+        - SoccerNet-v2 - Labels / Manual Annotations
+          - **video.ini**: information on start/duration for each half of the game in the HQ video, in second
+          - **Labels-v2.json**: Labels from SoccerNet-v2 - action spotting
+          - **Labels-cameras.json**: Labels from SoccerNet-v1 - camera shot segmentation
+
+        - SoccerNet-v2 - Videos / Automatically Extracted Features
+          - **1_HQ.mkv**: HQ video 1st half
+          - **2_HQ.mkv**: HQ video 2nd half
+          - **1.mkv**: LQ video 1st half - timmed with start/duration from HQ video - resolution 224*398 - 25 fps
+          - **2.mkv**: LQ video 2nd half - timmed with start/duration from HQ video - resolution 224*398 - 25 fps
+          - **1_ResNET_TF2.npy**: ResNET features @2fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **2_ResNET_TF2.npy**: ResNET features @2fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **1_ResNET_TF2_PCA512.npy**: ResNET features @2fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
+          - **2_ResNET_TF2_PCA512.npy**: ResNET features @2fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
+          - **1_ResNET_5fps_TF2.npy**: ResNET features @5fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **2_ResNET_5fps_TF2.npy**: ResNET features @5fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **1_ResNET_5fps_TF2_PCA512.npy**: ResNET features @5fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
+          - **2_ResNET_5fps_TF2_PCA512.npy**: ResNET features @5fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit), with dimensionality reduced to 512 using PCA
+          - **1_ResNET_25fps_TF2.npy**: ResNET features @25fps for 1st half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **2_ResNET_25fps_TF2.npy**: ResNET features @25fps for 2nd half from SoccerNet-v2, [extracted using TF2](https://github.com/SilvioGiancola/SoccerNetv2-DevKit)
+          - **1_player_boundingbox_maskrcnn.json**: Player Bounding Boxes @2fps for 1st half, extracted with MaskRCNN
+          - **2_player_boundingbox_maskrcnn.json**: Player Bounding Boxes @2fps for 2nd half, extracted with MaskRCNN
+          - **1_field_calib_ccbv.json**: Field Camera Calibration @2fps for 1st half, extracted with CCBV
+          - **2_field_calib_ccbv.json**: Field Camera Calibration @2fps for 2nd half, extracted with CCBV
+          - **1_baidu_soccer_embeddings.npy**: Frame Embeddings for 1st half from [https://github.com/baidu-research/vidpress-sports](https://github.com/baidu-research/vidpress-sports)
+          - **2_baidu_soccer_embeddings.npy**: Frame Embeddings for 2nd half from [https://github.com/baidu-research/vidpress-sports](https://github.com/baidu-research/vidpress-sports)
+
+        - Legacy from SoccerNet-v1
+          - **Labels.json**: Labels from SoccerNet-v1 - action spotting for goals/cards/subs only
+          - **1_C3D.npy**: C3D features @2fps for 1st half from SoccerNet-v1
+          - **2_C3D.npy**: C3D features @2fps for 2nd half from SoccerNet-v1
+          - **1_C3D_PCA512.npy**: C3D features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **2_C3D_PCA512.npy**: C3D features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **1_I3D.npy**: I3D features @2fps for 1st half from SoccerNet-v1
+          - **2_I3D.npy**: I3D features @2fps for 2nd half from SoccerNet-v1
+          - **1_I3D_PCA512.npy**: I3D features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **2_I3D_PCA512.npy**: I3D features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **1_ResNET.npy**: ResNET features @2fps for 1st half from SoccerNet-v1
+          - **2_ResNET.npy**: ResNET features @2fps for 2nd half from SoccerNet-v1
+          - **1_ResNET_PCA512.npy**: ResNET features @2fps for 1st half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+          - **2_ResNET_PCA512.npy**: ResNET features @2fps for 2nd half from SoccerNet-v1, with dimensionality reduced to 512 using PCA
+
+
+## How to Download Games (Python)
+
+```python
+from SoccerNet.Downloader import SoccerNetDownloader
+
+mySoccerNetDownloader = SoccerNetDownloader(LocalDirectory="path/to/soccernet")
+
+# Download SoccerNet labels
+mySoccerNetDownloader.downloadGames(files=["Labels.json"], split=["train","valid","test"]) # download labels
+mySoccerNetDownloader.downloadGames(files=["Labels-v2.json"], split=["train","valid","test"]) # download labels SN v2
+mySoccerNetDownloader.downloadGames(files=["Labels-cameras.json"], split=["train","valid","test"]) # download labels for camera shot
+
+# Download SoccerNet features
+mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2.npy", "2_ResNET_TF2.npy"], split=["train","valid","test"]) # download Features
+mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2_PCA512.npy", "2_ResNET_TF2_PCA512.npy"], split=["train","valid","test"]) # download Features reduced with PCA
+mySoccerNetDownloader.downloadGames(files=["1_player_boundingbox_maskrcnn.json", "2_player_boundingbox_maskrcnn.json"], split=["train","valid","test"]) # download Player Bounding Boxes inferred with MaskRCNN
+mySoccerNetDownloader.downloadGames(files=["1_field_calib_ccbv.json", "2_field_calib_ccbv.json"], split=["train","valid","test"]) # download Field Calibration inferred with CCBV
+mySoccerNetDownloader.downloadGames(files=["1_baidu_soccer_embeddings.npy","2_baidu_soccer_embeddings.npy"], split=["train","valid","test"]) # download Frame Embeddings from https://github.com/baidu-research/vidpress-sports
+
+# Download SoccerNet videos (require password from NDA to download videos)
+mySoccerNetDownloader.password = input("Password for videos? (contact the author):\n")
+mySoccerNetDownloader.downloadGames(files=["1.mkv", "2.mkv"], split=["train","valid","test"]) # download LQ Videos
+mySoccerNetDownloader.downloadGames(files=["1_HQ.mkv", "2_HQ.mkv", "video.ini"], split=["train","valid","test"]) # download HQ Videos
+
+# Download SoccerNet Challenge set (require password from NDA to download videos)
+mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2.npy", "2_ResNET_TF2.npy"], split=["challenge"]) # download ResNET Features
+mySoccerNetDownloader.downloadGames(files=["1_ResNET_TF2_PCA512.npy", "2_ResNET_TF2_PCA512.npy"], split=["challenge"]) # download ResNET Features reduced with PCA
+mySoccerNetDownloader.downloadGames(files=["1.mkv", "2.mkv", "video.ini"], split=["challenge"]) # download LQ Videos (require password from NDA)
+mySoccerNetDownloader.downloadGames(files=["1_HQ.mkv", "2_HQ.mkv", "video.ini"], split=["challenge"]) # download HQ Videos (require password from NDA)
+mySoccerNetDownloader.downloadGames(files=["1_player_boundingbox_maskrcnn.json", "2_player_boundingbox_maskrcnn.json"], split=["challenge"]) # download Player Bounding Boxes inferred with MaskRCNN 
+mySoccerNetDownloader.downloadGames(files=["1_field_calib_ccbv.json", "2_field_calib_ccbv.json"], split=["challenge"]) # download Field Calibration inferred with CCBV 
+mySoccerNetDownloader.downloadGames(files=["1_baidu_soccer_embeddings.npy","2_baidu_soccer_embeddings.npy"], split=["challenge"]) # download Frame Embeddings from https://github.com/baidu-research/vidpress-sports
+
+```
+
+## How to read the list Games (Python)
+
+```python
+from SoccerNet.utils import getListGames
+print(getListGames(split="train")) # return list of games recommended for training
+print(getListGames(split="valid")) # return list of games recommended for validation
+print(getListGames(split="test")) # return list of games recommended for testing
+print(getListGames(split="challenge")) # return list of games recommended for challenge
+print(getListGames(split=["train", "valid", "test", "challenge"])) # return list of games for training, validation and testing
+print(getListGames(split="v1")) # return list of games from SoccerNetv1 (train/valid/test)
+```
+
+
+
+
```

### Comparing `SoccerNet-0.1.8/SoccerNet.egg-info/SOURCES.txt` & `SoccerNet-0.1.9/SoccerNet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 SoccerNet/DataLoader.py
 SoccerNet/DataLoaderTensorFlow.py
 SoccerNet/DataLoaderTorch.py
```

### Comparing `SoccerNet-0.1.8/setup.py` & `SoccerNet-0.1.9/setup.py`

 * *Files identical despite different names*

