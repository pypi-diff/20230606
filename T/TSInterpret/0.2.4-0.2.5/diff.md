# Comparing `tmp/TSInterpret-0.2.4.tar.gz` & `tmp/TSInterpret-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.2.4.tar", last modified: Tue May 30 08:14:04 2023, max compression
+gzip compressed data, was "TSInterpret-0.2.5.tar", last modified: Tue Jun  6 13:21:36 2023, max compression
```

## Comparing `TSInterpret-0.2.4.tar` & `TSInterpret-0.2.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.814748 TSInterpret-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-30 08:14:04.814748 TSInterpret-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.814748 TSInterpret-0.2.4/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:14:04.814748 TSInterpret-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.464970 TSInterpret-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.456970 TSInterpret-0.2.5/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-06 13:21:36.464970 TSInterpret-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.456970 TSInterpret-0.2.5/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.456970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.456970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.456970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.456970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.456970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.460970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.460970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.460970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.460970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.460970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.460970 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.460970 TSInterpret-0.2.5/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:21:36.456970 TSInterpret-0.2.5/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-06 13:21:36.000000 TSInterpret-0.2.5/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-06 13:21:36.000000 TSInterpret-0.2.5/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:21:36.000000 TSInterpret-0.2.5/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-06 13:21:36.000000 TSInterpret-0.2.5/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 13:21:36.000000 TSInterpret-0.2.5/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:21:36.464970 TSInterpret-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-06 13:21:22.000000 TSInterpret-0.2.5/setup.py
```

### Comparing `TSInterpret-0.2.4/ClassificationModels/CNN.py` & `TSInterpret-0.2.5/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/ClassificationModels/CNN_T.py` & `TSInterpret-0.2.5/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/ClassificationModels/DecisionTree.py` & `TSInterpret-0.2.5/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/ClassificationModels/LSTM.py` & `TSInterpret-0.2.5/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/ClassificationModels/LSTM_T.py` & `TSInterpret-0.2.5/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/ClassificationModels/ResNet.py` & `TSInterpret-0.2.5/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/ClassificationModels/utils.py` & `TSInterpret-0.2.5/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/LICENSE` & `TSInterpret-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/PKG-INFO` & `TSInterpret-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.4
+Version: 0.2.5
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.4 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.5 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.4/README.md` & `TSInterpret-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files 11% similar despite different names*

```diff
@@ -111,15 +111,16 @@
         inputMask[:, :, :] = mask
         inputMask = torch.from_numpy(inputMask).to(self.device)
         mask_single = torch.from_numpy(mask).to(self.device)
         mask_single = mask_single.reshape(1, self.NumTimeSteps, self.NumFeatures).to(
             self.device
         )
         # input = samples.reshape(-1, args.NumTimeSteps, args.NumFeatures).to(device)
-        input = input.reshape(-1, self.NumFeatures, self.NumTimeSteps)
+        if self.mode == "feat":
+            input = input.reshape(-1, self.NumFeatures, self.NumTimeSteps)
         baseline_single = (
             torch.from_numpy(np.random.random(input.shape)).float().to(self.device)
         )
         baseline_multiple = (
             torch.from_numpy(
                 np.random.random((input.shape[0] * 5, input.shape[1], input.shape[2]))
             )
@@ -163,18 +164,22 @@
             )
         # elif(self.method=='FP'):
         #    attributions = self.Grad.attribute(input, target=labels, perturbations_per_eval= input.shape[0],feature_mask=mask_single)
         elif self.method == "FA":
             attributions = self.Grad.attribute(input, target=labels)
         elif self.method == "FO":
             base = baseline_single
-            has_sliding_window = (1, self.NumFeatures)
+            if self.mode == "feat":
+                has_sliding_window = (1, self.NumFeatures)
+            else:
+                has_sliding_window = (self.NumFeatures, 1)
+            # has_sliding_window = (1, self.NumFeatures)
             attributions = self.Grad.attribute(
                 input,
-                sliding_window_shapes=(1, self.NumFeatures),
+                sliding_window_shapes=has_sliding_window,
                 target=labels,
                 baselines=baseline_single,
             )
         if TSR is not None:
             self.tsr = TSR
 
         if self.tsr:
@@ -207,18 +212,25 @@
         hasBaseline=None,
         hasFeatureMask=None,
         hasSliding_window_shapes=None,
     ):
         sequence_length = self.NumTimeSteps
         input_size = self.NumFeatures
         assignment = input[0, 0, 0]
+        # TODO IS THIS CORRECT TO BE PUT HERE
+        # if self.mode == "feat":
+        #    hasSliding_window_shapes = (1, self.NumFeatures)
+        # else:
+        #    hasSliding_window_shapes = (self.NumFeatures, 1)
         timeGrad = np.zeros((1, sequence_length))
         inputGrad = np.zeros((input_size, 1))
         newGrad = np.zeros((input_size, sequence_length))
         # print("has Sliding Window", hasSliding_window_shapes)
+        if self.mode == "time":
+            input = input.reshape(-1, sequence_length, input_size)
         if hasBaseline is None:
             ActualGrad = (
                 self.Grad.attribute(input, target=TestingLabel).data.cpu().numpy()
             )
         else:
             if hasFeatureMask is not None:
                 ActualGrad = (
@@ -247,17 +259,28 @@
                 ActualGrad = (
                     self.Grad.attribute(
                         input, baselines=hasBaseline, target=TestingLabel
                     )
                     .data.cpu()
                     .numpy()
                 )
+        if self.mode == "time":
+            ActualGrad = ActualGrad.reshape(-1, input_size, sequence_length)
         for t in range(sequence_length):
+            if self.mode == "time":
+                input = input.reshape(-1, input_size, sequence_length)
             newInput = input.clone()
+            # if newInput.shape[-1] == self.NumTimeSteps:
+            #    print('A')
             newInput[:, :, t] = assignment
+            # else:
+            #    print('B')
+            #    newInput[:, t,:] = assignment
+            if self.mode == "time":
+                newInput = newInput.reshape(-1, sequence_length, input_size)
 
             if hasBaseline is None:
                 timeGrad_perTime = (
                     self.Grad.attribute(newInput, target=TestingLabel)
                     .data.cpu()
                     .numpy()
                 )
@@ -289,26 +312,34 @@
                     timeGrad_perTime = (
                         self.Grad.attribute(
                             newInput, baselines=hasBaseline, target=TestingLabel
                         )
                         .data.cpu()
                         .numpy()
                     )
+            # import sys
+            # sys.exit(1)
+            if self.mode == "time":
+                timeGrad_perTime = timeGrad_perTime.reshape(
+                    -1, input_size, sequence_length
+                )
 
             timeGrad_perTime = np.absolute(ActualGrad - timeGrad_perTime)
             timeGrad[:, t] = np.sum(timeGrad_perTime)
 
         timeContibution = preprocessing.minmax_scale(timeGrad, axis=1)
         meanTime = np.quantile(timeContibution, 0.55)
 
         for t in range(sequence_length):
             if timeContibution[0, t] > meanTime:
                 for c in range(input_size):
                     newInput = input.clone()
                     newInput[:, c, t] = assignment
+                    if self.mode == "time":
+                        newInput = newInput.reshape(-1, sequence_length, input_size)
 
                     if hasBaseline is None:
                         inputGrad_perInput = (
                             self.Grad.attribute(newInput, target=TestingLabel)
                             .data.cpu()
                             .numpy()
                         )
@@ -339,23 +370,30 @@
                             inputGrad_perInput = (
                                 self.Grad.attribute(
                                     newInput, baselines=hasBaseline, target=TestingLabel
                                 )
                                 .data.cpu()
                                 .numpy()
                             )
-
+                    inputGrad_perInput = inputGrad_perInput.reshape(
+                        -1, input_size, sequence_length
+                    )
                     inputGrad_perInput = np.absolute(ActualGrad - inputGrad_perInput)
                     inputGrad[c, :] = np.sum(inputGrad_perInput)
                 featureContibution = preprocessing.minmax_scale(inputGrad, axis=0)
             else:
                 featureContibution = np.ones((input_size, 1)) * 0.1
+            # print('FC',featureContibution)
+            # print('TC',timeContibution)
+            # print(input_size)
 
             for c in range(input_size):
                 newGrad[c, t] = timeContibution[0, t] * featureContibution[c, 0]
+            if self.mode == "time":
+                newGrad = newGrad.reshape(-1, sequence_length, input_size)
         # print('NewGrad',newGrad.shape)
         return newGrad
 
     def _givenAttGetRescaledSaliency(self, attributions, isTensor=True):
         if isTensor:
             saliency = np.absolute(attributions.data.cpu().numpy())
         else:
```

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/Ates.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,39 @@
     ----------
      [1] Höllig, Jacqueline , et al.
      "TSEvo: Evolutionary Counterfactual Explanations for Time Series Classification."
      21st IEEE International Conference on Machine Learning and Applications (ICMLA). IEEE, 2022.
     ----------
     """
 
-    def __init__(self, model, data, mode="time", backend="PYT", verbose=0):
+    def __init__(
+        self,
+        model,
+        data,
+        transformer="authentic_opposing_information",
+        epochs=500,
+        mode="time",
+        backend="PYT",
+        verbose=0,
+    ):
         """
         Arguments:
             model [torch.nn.Module, Callable, tf.keras.model]: Model to be interpreted.
             data Tuple: Reference Dataset as Tuple (x,y).
+            transformer str: ['authentic_opposing_information','mutate_both','mutate_mean','frequency_band_mapping']
+            epochs int: Maximal Number of Itertions
             mode str: Name of second dimension: time -> (-1, time, feature) or feat -> (-1, feature, time)
             backend str: desired Model Backend ('PYT', 'TF', 'SK').
             verbose int: Logging Level
         """
         super().__init__(model, mode)
         self.backend = backend
         self.verbose = verbose
+        self.transformer = transformer
+        self.epochs = epochs
         if type(data) == tuple:
             self.x, self.y = data
             # print('Len Reference Set ', len(self.x.shape))
             print(type(self.y[0]))
             if not type(self.y[0]) == int and not type(self.y[0]) == np.int64:
                 print("y was one Hot Encoded")
                 self.y = np.argmax(self.y, axis=1)
@@ -47,29 +60,29 @@
         pass
 
     def explain(
         self,
         original_x,
         original_y,
         target_y=None,
-        transformer="authentic_opposing_information",
-        epochs=500,
     ):
         """
         Entry Point to explain a instance.
         Arguments:
             original_x (np.array): The instance to explain. Shape `mode = time` -> `(1,time, feat)` or `mode = time` -> `(1,feat, time)`
             original_y (np.array): Classification Probability of instance.
             target_y int: Class to be targeted
-            transformer str: ['authentic_opposing','mutate_both','gaussian','frequency']
-            epochs int: # Iterations
+
         Returns:
             [np.array, int]: Returns the Counterfactual and the class. Shape of CF : `mode = time` -> `(time, feat)` or `mode = time` -> `(feat, time)`
         """
-        print(len(original_y.shape))
+        transformer = self.transformer
+        epochs = self.epochs
+
+        # print(len(original_y.shape))
         if len(original_x.shape) < 3:
             original_x = np.array([original_x])
         if self.backend == "TF" or self.mode == "time":
             original_x = original_x.reshape(
                 original_x.shape[0], original_x.shape[2], original_x.shape[1]
             )
         neighborhood = []
```

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.2.5/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.2.5/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.2.5/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.2.5/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret/Models/base_model.py` & `TSInterpret-0.2.5/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.2.5/TSInterpret.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.4
+Version: 0.2.5
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.4 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.5 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.4/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.2.5/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.2.5/TSInterpret.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.4/setup.py` & `TSInterpret-0.2.5/setup.py`

 * *Files identical despite different names*

