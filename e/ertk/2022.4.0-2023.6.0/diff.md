# Comparing `tmp/ertk-2022.4.0.tar.gz` & `tmp/ertk-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ertk-2022.4.0.tar", last modified: Sat Apr 23 03:56:02 2022, max compression
+gzip compressed data, was "ertk-2023.6.0.tar", last modified: Tue Jun  6 05:39:14 2023, max compression
```

## Comparing `ertk-2022.4.0.tar` & `ertk-2023.6.0.tar`

### file list

```diff
@@ -1,126 +1,416 @@
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.898007 ertk-2022.4.0/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1075 2022-02-15 23:42:06.000000 ertk-2022.4.0/LICENSE
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2690 2022-04-23 03:56:02.898007 ertk-2022.4.0/PKG-INFO
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1606 2022-02-23 00:14:59.000000 ertk-2022.4.0/README.md
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      630 2022-02-22 01:06:44.000000 ertk-2022.4.0/pyproject.toml
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1467 2022-04-23 03:56:02.898007 ertk-2022.4.0/setup.cfg
--rw-r--r--   0 akee511  (2430749) akee511  (62215)       69 2022-02-15 23:42:06.000000 ertk-2022.4.0/setup.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.890007 ertk-2022.4.0/src/
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)       66 2022-04-23 03:43:58.000000 ertk-2022.4.0/src/ertk/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    11442 2022-04-13 04:06:24.000000 ertk-2022.4.0/src/ertk/classification.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/cli/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      388 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)       56 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/__main__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    12556 2022-04-11 06:12:55.000000 ertk-2022.4.0/src/ertk/cli/class_cv.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    11720 2022-03-18 01:13:54.000000 ertk-2022.4.0/src/ertk/cli/class_tvt.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1576 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/classify.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/cli/dataset/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      789 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/dataset/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)       56 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/dataset/__main__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     3233 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/dataset/annotation_stats.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1579 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/dataset/combine.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1179 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/dataset/convert.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      487 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/dataset/info.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     4384 2022-02-18 02:21:12.000000 ertk-2022.4.0/src/ertk/cli/dataset/process.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1082 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/dataset/remove_instances.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1151 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/dataset/view_features.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     5775 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/cli/train.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/cli/util/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      769 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/cli/util/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)       56 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/cli/util/__main__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1314 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/cli/util/create_cv_dirs.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1183 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/cli/util/grid_to_conf.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      788 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/cli/util/names_to_filenames.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     3235 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/cli/util/parallel_jobs.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1852 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/cli/util/split_chat.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     3463 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/cli/util/split_elan.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2322 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/config.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/dataset/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      318 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/dataset/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1191 2022-03-06 06:30:19.000000 ertk-2022.4.0/src/ertk/dataset/annotation.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    31021 2022-04-23 03:31:30.000000 ertk-2022.4.0/src/ertk/dataset/dataset.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    10742 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/dataset/features.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     3230 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/dataset/utils.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/preprocessing/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      162 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/__init__.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/preprocessing/audioset/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      122 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/__init__.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/preprocessing/audioset/_vggish/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)        0 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/_vggish/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2025 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/_vggish/vggish_params.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     4078 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/_vggish/vggish_postprocess.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     6318 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/_vggish/vggish_slim.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/preprocessing/audioset/_yamnet/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)        0 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/_yamnet/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     8228 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/_yamnet/features.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1896 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/_yamnet/params.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     5484 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/_yamnet/yamnet.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     5091 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/audioset/audioset.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     6717 2022-04-23 03:32:29.000000 ertk-2022.4.0/src/ertk/preprocessing/base.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     3293 2022-03-10 01:18:40.000000 ertk-2022.4.0/src/ertk/preprocessing/fairseq.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     4975 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/keras_apps.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1865 2022-03-12 10:14:29.000000 ertk-2022.4.0/src/ertk/preprocessing/opensmile.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk/preprocessing/openxbow/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)       65 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/openxbow/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2168 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/openxbow/openxbow.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     4604 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/preprocessing/spectrogram.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     4361 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/preprocessing/vad_trim.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.898007 ertk-2022.4.0/src/ertk/pytorch/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)       50 2022-01-25 02:04:40.000000 ertk-2022.4.0/src/ertk/pytorch/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     6189 2022-03-08 07:08:08.000000 ertk-2022.4.0/src/ertk/pytorch/classification.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)     3999 2022-02-22 23:38:27.000000 ertk-2022.4.0/src/ertk/pytorch/dataset.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.898007 ertk-2022.4.0/src/ertk/pytorch/models/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1298 2022-02-22 23:38:27.000000 ertk-2022.4.0/src/ertk/pytorch/models/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     3918 2022-03-07 00:01:04.000000 ertk-2022.4.0/src/ertk/pytorch/models/_base.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1479 2021-11-12 07:14:13.000000 ertk-2022.4.0/src/ertk/pytorch/models/aldeneh2017.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)      519 2021-11-11 04:50:26.000000 ertk-2022.4.0/src/ertk/pytorch/models/layers.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)      679 2022-02-22 23:38:27.000000 ertk-2022.4.0/src/ertk/pytorch/models/mlp.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)     1674 2022-02-04 05:27:58.000000 ertk-2022.4.0/src/ertk/pytorch/models/mtl.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)     2224 2022-02-22 23:38:27.000000 ertk-2022.4.0/src/ertk/pytorch/models/simple_mtl.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)     3289 2022-02-22 23:38:27.000000 ertk-2022.4.0/src/ertk/pytorch/models/test_fit.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)     1921 2022-03-08 04:06:18.000000 ertk-2022.4.0/src/ertk/pytorch/models/wav2vec_ft.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     3417 2022-02-21 05:11:49.000000 ertk-2022.4.0/src/ertk/pytorch/models/zhang2019.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2301 2022-04-23 03:54:55.000000 ertk-2022.4.0/src/ertk/pytorch/utils.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.898007 ertk-2022.4.0/src/ertk/sklearn/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)        0 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/sklearn/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2300 2022-04-13 03:54:31.000000 ertk-2022.4.0/src/ertk/sklearn/classification.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.898007 ertk-2022.4.0/src/ertk/sklearn/models/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      921 2022-03-28 02:18:41.000000 ertk-2022.4.0/src/ertk/sklearn/models/__init__.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)     9905 2022-04-13 10:30:12.000000 ertk-2022.4.0/src/ertk/sklearn/models/mtl.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2771 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/sklearn/models/svm.py
--rw-rw-r--   0 akee511  (2430749) akee511  (62215)     2626 2022-04-23 03:31:23.000000 ertk-2022.4.0/src/ertk/sklearn/utils.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    10029 2022-04-13 03:55:03.000000 ertk-2022.4.0/src/ertk/stats.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.898007 ertk-2022.4.0/src/ertk/tensorflow/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      116 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    11978 2022-02-22 08:01:17.000000 ertk-2022.4.0/src/ertk/tensorflow/classification.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.898007 ertk-2022.4.0/src/ertk/tensorflow/models/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1424 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/tensorflow/models/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1667 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/models/aldeneh2017.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2630 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/models/audeep.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      972 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/models/depinto2020.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1564 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/models/iskhakova2020.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2530 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/models/latif2019.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      589 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/models/layers.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      641 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/models/mlp.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    21899 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/tensorflow/models/rbm.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2578 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/tensorflow/models/test_fit.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1717 2022-01-19 23:43:50.000000 ertk-2022.4.0/src/ertk/tensorflow/models/transformer.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2626 2022-02-15 23:42:06.000000 ertk-2022.4.0/src/ertk/tensorflow/models/zhang2019.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1866 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/tensorflow/models/zhao2019.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    11803 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/tensorflow/utils.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     8379 2022-04-13 04:04:22.000000 ertk-2022.4.0/src/ertk/train.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     5136 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/transform.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.898007 ertk-2022.4.0/src/ertk/utils/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      445 2022-03-06 23:57:51.000000 ertk-2022.4.0/src/ertk/utils/__init__.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)    16354 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/utils/array.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     4688 2022-04-11 04:33:43.000000 ertk-2022.4.0/src/ertk/utils/generic.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     1274 2022-02-20 21:44:11.000000 ertk-2022.4.0/src/ertk/utils/misc.py
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      172 2022-01-20 02:48:02.000000 ertk-2022.4.0/src/ertk/utils/types.py
-drwxr-xr-x   0 akee511  (2430749) akee511  (62215)        0 2022-04-23 03:56:02.894007 ertk-2022.4.0/src/ertk.egg-info/
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     2690 2022-04-23 03:56:02.000000 ertk-2022.4.0/src/ertk.egg-info/PKG-INFO
--rw-r--r--   0 akee511  (2430749) akee511  (62215)     3484 2022-04-23 03:56:02.000000 ertk-2022.4.0/src/ertk.egg-info/SOURCES.txt
--rw-r--r--   0 akee511  (2430749) akee511  (62215)        1 2022-04-23 03:56:02.000000 ertk-2022.4.0/src/ertk.egg-info/dependency_links.txt
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      108 2022-04-23 03:56:02.000000 ertk-2022.4.0/src/ertk.egg-info/entry_points.txt
--rw-r--r--   0 akee511  (2430749) akee511  (62215)      214 2022-04-23 03:56:02.000000 ertk-2022.4.0/src/ertk.egg-info/requires.txt
--rw-r--r--   0 akee511  (2430749) akee511  (62215)        5 2022-04-23 03:56:02.000000 ertk-2022.4.0/src/ertk.egg-info/top_level.txt
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.087041 ertk-2023.6.0/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1075 2022-10-09 21:53:05.000000 ertk-2023.6.0/LICENSE
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       95 2023-06-06 04:29:06.000000 ertk-2023.6.0/MANIFEST.in
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6079 2023-06-06 05:39:14.087041 ertk-2023.6.0/PKG-INFO
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4654 2023-06-06 05:38:35.000000 ertk-2023.6.0/README.md
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.031041 ertk-2023.6.0/conf/
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.031041 ertk-2023.6.0/conf/clf/
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.039041 ertk-2023.6.0/conf/clf/pt/
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)      208 2022-11-11 01:58:54.000000 ertk-2023.6.0/conf/clf/pt/aldeneh2017.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.031041 ertk-2023.6.0/conf/clf/sk/
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.039041 ertk-2023.6.0/conf/clf/sk/knn/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       15 2022-08-12 01:08:58.000000 ertk-2023.6.0/conf/clf/sk/knn/1NN.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.039041 ertk-2023.6.0/conf/clf/sk/knn/grids/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       74 2022-08-12 01:08:58.000000 ertk-2023.6.0/conf/clf/sk/knn/grids/default.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.040041 ertk-2023.6.0/conf/clf/sk/lr/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       89 2022-11-06 22:51:15.000000 ertk-2023.6.0/conf/clf/sk/lr/default.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.040041 ertk-2023.6.0/conf/clf/sk/lr/grids/
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)      200 2023-06-06 02:22:38.000000 ertk-2023.6.0/conf/clf/sk/lr/grids/default.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.040041 ertk-2023.6.0/conf/clf/sk/rf/
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)       34 2022-09-28 22:05:30.000000 ertk-2023.6.0/conf/clf/sk/rf/default.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.040041 ertk-2023.6.0/conf/clf/sk/rf/grids/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       60 2021-08-24 14:00:30.000000 ertk-2023.6.0/conf/clf/sk/rf/grids/default.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.041041 ertk-2023.6.0/conf/clf/sk/svm/
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.042041 ertk-2023.6.0/conf/clf/sk/svm/grids/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      201 2023-06-06 02:22:03.000000 ertk-2023.6.0/conf/clf/sk/svm/grids/linear.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      211 2023-06-06 02:21:52.000000 ertk-2023.6.0/conf/clf/sk/svm/grids/poly2.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      207 2023-06-06 02:21:40.000000 ertk-2023.6.0/conf/clf/sk/svm/grids/poly3.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      278 2023-06-06 02:22:10.000000 ertk-2023.6.0/conf/clf/sk/svm/grids/rbf.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      151 2022-08-31 14:21:37.000000 ertk-2023.6.0/conf/clf/sk/svm/linear.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       39 2021-08-24 01:14:25.000000 ertk-2023.6.0/conf/clf/sk/svm/poly2.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       39 2021-08-24 01:14:17.000000 ertk-2023.6.0/conf/clf/sk/svm/poly3.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       14 2021-08-24 01:14:49.000000 ertk-2023.6.0/conf/clf/sk/svm/rbf.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.031041 ertk-2023.6.0/conf/clf/tf/
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.042041 ertk-2023.6.0/conf/clf/tf/mlp/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       26 2021-08-24 00:45:52.000000 ertk-2023.6.0/conf/clf/tf/mlp/1layer.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       31 2021-08-24 01:15:11.000000 ertk-2023.6.0/conf/clf/tf/mlp/2layer.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       36 2021-08-24 01:15:19.000000 ertk-2023.6.0/conf/clf/tf/mlp/3layer.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.043041 ertk-2023.6.0/conf/mapping/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       24 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/mapping/eesc_joy_happiness.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      137 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/mapping/emodb_binary_arousal.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      137 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/mapping/emodb_binary_valence.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       30 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/mapping/emov-db_amusement_happiness.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       96 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/mapping/iemocap_excitement_happiness.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      117 2021-08-30 04:56:13.000000 ertk-2023.6.0/conf/mapping/smartkom.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.043041 ertk-2023.6.0/conf/opensmile/
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.044041 ertk-2023.6.0/conf/opensmile/IS09/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2657 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/IS09/IS09_emotion.conf
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2251 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/IS09/IS09_emotion_core.func.conf.inc
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4959 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/IS09/IS09_emotion_core.lld.conf.inc
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.045041 ertk-2023.6.0/conf/opensmile/IS13/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1664 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/IS13/IS13_ComParE.conf
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     9760 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/IS13/IS13_ComParE_core.func.conf.inc
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     9767 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/IS13/IS13_ComParE_core.lld.conf.inc
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.045041 ertk-2023.6.0/conf/opensmile/logmel/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      410 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/logmel/logmel.conf
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1518 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/logmel/logmel_IS09_func.conf
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1035 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/logmel/logmel_lld.conf.inc
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.045041 ertk-2023.6.0/conf/opensmile/mean_mfcc/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1686 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/mean_mfcc/mean_mfcc.conf
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.046041 ertk-2023.6.0/conf/opensmile/mfcc_log_energy/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1705 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/mfcc_log_energy/mfcc_log_energy.conf
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     8548 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/openSMILE.LICENSE
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.046041 ertk-2023.6.0/conf/opensmile/shared/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       82 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/shared/BufferMode.conf.inc
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      105 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/shared/BufferModeRb.conf.inc
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      134 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/shared/BufferModeRbLag.conf.inc
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      359 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/opensmile/shared/FrameModeFunctionals.conf.inc
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.048041 ertk-2023.6.0/conf/select/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       43 2021-08-24 13:53:57.000000 ertk-2023.6.0/conf/select/3class.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       36 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/select/demos_prot_neutral.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       55 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/select/iemocap_4class.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       18 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/select/iemocap_test.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       36 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/select/iemocap_train.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       18 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/select/iemocap_valid.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       19 2022-08-12 01:02:47.000000 ertk-2023.6.0/conf/select/mesd_adult.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      102 2022-02-15 23:42:06.000000 ertk-2023.6.0/conf/select/msp-podcast_8class.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.048041 ertk-2023.6.0/datasets/
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.048041 ertk-2023.6.0/datasets/AESDD/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      255 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/AESDD/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1480 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/AESDD/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.049041 ertk-2023.6.0/datasets/ASED/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      275 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/ASED/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4321 2023-05-25 15:18:45.000000 ertk-2023.6.0/datasets/ASED/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.049041 ertk-2023.6.0/datasets/BAVED/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      272 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/BAVED/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1626 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/BAVED/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.050041 ertk-2023.6.0/datasets/CMU-MOSEI/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1046 2023-02-28 03:37:28.000000 ertk-2023.6.0/datasets/CMU-MOSEI/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6898 2023-02-28 03:33:43.000000 ertk-2023.6.0/datasets/CMU-MOSEI/process.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    47683 2022-10-14 04:36:14.000000 ertk-2023.6.0/datasets/CMU-MOSEI/splits.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.050041 ertk-2023.6.0/datasets/CREMA-D/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      392 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/CREMA-D/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6504 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/CREMA-D/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.051041 ertk-2023.6.0/datasets/CaFE/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      231 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/CaFE/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2106 2023-05-25 15:18:45.000000 ertk-2023.6.0/datasets/CaFE/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.051041 ertk-2023.6.0/datasets/DEMoS/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      423 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/DEMoS/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2131 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/DEMoS/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.051041 ertk-2023.6.0/datasets/EESC/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      245 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/EESC/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1485 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/EESC/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.052041 ertk-2023.6.0/datasets/EMO-DB/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      279 2023-06-05 11:22:05.000000 ertk-2023.6.0/datasets/EMO-DB/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2960 2023-06-05 11:22:05.000000 ertk-2023.6.0/datasets/EMO-DB/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.052041 ertk-2023.6.0/datasets/EMOVO/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      245 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/EMOVO/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2319 2023-05-25 15:20:35.000000 ertk-2023.6.0/datasets/EMOVO/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.052041 ertk-2023.6.0/datasets/ESD/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      486 2023-02-28 03:33:43.000000 ertk-2023.6.0/datasets/ESD/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4498 2023-02-28 03:33:43.000000 ertk-2023.6.0/datasets/ESD/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.052041 ertk-2023.6.0/datasets/EmoFilm/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      237 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/EmoFilm/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2675 2022-11-01 09:02:08.000000 ertk-2023.6.0/datasets/EmoFilm/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.053041 ertk-2023.6.0/datasets/EmoV-DB/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      251 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/EmoV-DB/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2177 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/EmoV-DB/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.053041 ertk-2023.6.0/datasets/EmoryNLP/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      457 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/EmoryNLP/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2201 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/EmoryNLP/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.053041 ertk-2023.6.0/datasets/IEMOCAP/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      408 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/IEMOCAP/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6766 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/IEMOCAP/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.054041 ertk-2023.6.0/datasets/JL/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      422 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/JL/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2488 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/JL/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.054041 ertk-2023.6.0/datasets/MELD/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      513 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MELD/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2265 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MELD/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.054041 ertk-2023.6.0/datasets/MESD/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      269 2023-05-25 15:18:45.000000 ertk-2023.6.0/datasets/MESD/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1311 2023-05-25 15:18:45.000000 ertk-2023.6.0/datasets/MESD/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.054041 ertk-2023.6.0/datasets/MESS/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      252 2022-11-01 09:02:08.000000 ertk-2023.6.0/datasets/MESS/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1386 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MESS/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.055041 ertk-2023.6.0/datasets/MLEndSND/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      250 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MLEndSND/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1614 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MLEndSND/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.055041 ertk-2023.6.0/datasets/MSP-IMPROV/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      450 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MSP-IMPROV/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     5990 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MSP-IMPROV/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.055041 ertk-2023.6.0/datasets/MSP-PODCAST/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      590 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MSP-PODCAST/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4611 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/MSP-PODCAST/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.055041 ertk-2023.6.0/datasets/Oréau/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      370 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/Oréau/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1533 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/Oréau/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.056041 ertk-2023.6.0/datasets/Portuguese/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      230 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/Portuguese/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3573 2023-05-25 15:18:45.000000 ertk-2023.6.0/datasets/Portuguese/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.056041 ertk-2023.6.0/datasets/RAVDESS/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      448 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/RAVDESS/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2241 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/RAVDESS/process.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4314 2023-06-05 12:53:26.000000 ertk-2023.6.0/datasets/README.md
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.056041 ertk-2023.6.0/datasets/SAVEE/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      234 2022-11-01 09:02:08.000000 ertk-2023.6.0/datasets/SAVEE/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1750 2023-05-05 02:51:32.000000 ertk-2023.6.0/datasets/SAVEE/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.056041 ertk-2023.6.0/datasets/SEMAINE/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    10753 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/SEMAINE/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.056041 ertk-2023.6.0/datasets/SUBESCO/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      276 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/SUBESCO/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2792 2023-05-25 15:18:45.000000 ertk-2023.6.0/datasets/SUBESCO/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.057041 ertk-2023.6.0/datasets/ShEMO/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      321 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/ShEMO/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2038 2023-05-25 15:18:45.000000 ertk-2023.6.0/datasets/ShEMO/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.057041 ertk-2023.6.0/datasets/SmartKom/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      224 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/SmartKom/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     5102 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/SmartKom/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.057041 ertk-2023.6.0/datasets/TESS/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      222 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/TESS/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1403 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/TESS/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.057041 ertk-2023.6.0/datasets/URDU/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      212 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/URDU/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1205 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/URDU/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.058041 ertk-2023.6.0/datasets/VENEC/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      469 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/VENEC/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4825 2023-02-28 03:33:43.000000 ertk-2023.6.0/datasets/VENEC/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.058041 ertk-2023.6.0/datasets/VIVAE/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      343 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/VIVAE/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1342 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/VIVAE/process.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.058041 ertk-2023.6.0/datasets/eNTERFACE/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      320 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/eNTERFACE/corpus.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2116 2022-10-09 21:53:05.000000 ertk-2023.6.0/datasets/eNTERFACE/process.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1084 2023-06-06 04:37:26.000000 ertk-2023.6.0/pyproject.toml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      168 2023-06-06 03:01:29.000000 ertk-2023.6.0/requirements-dev.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      166 2023-06-06 05:37:29.000000 ertk-2023.6.0/requirements-opt.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      256 2023-06-06 02:30:21.000000 ertk-2023.6.0/requirements.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2883 2023-06-06 05:39:14.088040 ertk-2023.6.0/setup.cfg
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       69 2022-10-09 21:53:05.000000 ertk-2023.6.0/setup.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.034042 ertk-2023.6.0/src/
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.059041 ertk-2023.6.0/src/ertk/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       66 2023-06-06 05:38:57.000000 ertk-2023.6.0/src/ertk/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    15198 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/classification.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.060041 ertk-2023.6.0/src/ertk/cli/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      183 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/cli/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6192 2022-09-07 13:14:13.000000 ertk-2023.6.0/src/ertk/cli/_utils.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.061041 ertk-2023.6.0/src/ertk/cli/cli/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      590 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/cli/cli/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       56 2022-08-12 01:08:58.000000 ertk-2023.6.0/src/ertk/cli/cli/__main__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1576 2022-08-12 01:08:58.000000 ertk-2023.6.0/src/ertk/cli/cli/classify.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    11841 2022-11-06 22:51:15.000000 ertk-2023.6.0/src/ertk/cli/cli/exp.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    11919 2023-05-25 15:18:45.000000 ertk-2023.6.0/src/ertk/cli/cli/exp2.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     5775 2022-08-12 01:08:58.000000 ertk-2023.6.0/src/ertk/cli/cli/train.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.062041 ertk-2023.6.0/src/ertk/cli/dataset/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1217 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/cli/dataset/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       56 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/cli/dataset/__main__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3418 2023-06-01 13:53:05.000000 ertk-2023.6.0/src/ertk/cli/dataset/annotation_stats.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1941 2023-06-01 10:20:41.000000 ertk-2023.6.0/src/ertk/cli/dataset/combine.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1014 2023-06-01 13:14:42.000000 ertk-2023.6.0/src/ertk/cli/dataset/convert.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1236 2022-08-12 01:02:47.000000 ertk-2023.6.0/src/ertk/cli/dataset/filter_clips.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2398 2023-06-01 13:52:39.000000 ertk-2023.6.0/src/ertk/cli/dataset/info.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3955 2023-05-25 15:18:45.000000 ertk-2023.6.0/src/ertk/cli/dataset/process.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1089 2023-06-01 13:30:07.000000 ertk-2023.6.0/src/ertk/cli/dataset/remove_instances.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4800 2022-09-07 13:14:13.000000 ertk-2023.6.0/src/ertk/cli/dataset/vis.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.063041 ertk-2023.6.0/src/ertk/cli/util/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1236 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/cli/util/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       56 2022-02-20 21:44:11.000000 ertk-2023.6.0/src/ertk/cli/util/__main__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      929 2022-08-12 01:02:47.000000 ertk-2023.6.0/src/ertk/cli/util/convert_audeep.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1401 2023-06-01 13:36:37.000000 ertk-2023.6.0/src/ertk/cli/util/create_cv_dirs.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1183 2022-02-20 21:44:11.000000 ertk-2023.6.0/src/ertk/cli/util/grid_to_conf.py
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)      788 2022-09-07 13:19:18.000000 ertk-2023.6.0/src/ertk/cli/util/names_to_filenames.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3736 2022-11-06 22:51:15.000000 ertk-2023.6.0/src/ertk/cli/util/parallel_jobs.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1852 2022-02-20 21:44:11.000000 ertk-2023.6.0/src/ertk/cli/util/split_chat.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3463 2022-02-20 21:44:11.000000 ertk-2023.6.0/src/ertk/cli/util/split_elan.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4395 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/config.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.064041 ertk-2023.6.0/src/ertk/dataset/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1360 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/dataset/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2238 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/dataset/annotation.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    42991 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/dataset/dataset.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    21540 2023-06-06 05:38:05.000000 ertk-2023.6.0/src/ertk/dataset/features.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3402 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/dataset/utils.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.066041 ertk-2023.6.0/src/ertk/preprocessing/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      682 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     9329 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/_base.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4160 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/_pipeline.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.066041 ertk-2023.6.0/src/ertk/preprocessing/audioset/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      379 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/__init__.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.067041 ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    11405 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/LICENSE
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        0 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2025 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/vggish_params.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4078 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/vggish_postprocess.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6318 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/vggish_slim.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.068041 ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    11405 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/LICENSE
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        0 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     8228 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/features.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1896 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/params.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     5491 2022-08-12 01:04:08.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/yamnet.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6890 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/audioset/audioset.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3923 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/encodec.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     9282 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/fairseq.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     8063 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/huggingface.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6539 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/keras_apps.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1051 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/kmeans.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2357 2023-06-05 12:55:24.000000 ertk-2023.6.0/src/ertk/preprocessing/opensmile.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.068041 ertk-2023.6.0/src/ertk/preprocessing/openxbow/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      294 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/openxbow/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    94445 2022-02-15 23:42:06.000000 ertk-2023.6.0/src/ertk/preprocessing/openxbow/openXBOW.jar
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3361 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/openxbow/openxbow.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4178 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/phonemize.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      944 2023-06-05 12:55:24.000000 ertk-2023.6.0/src/ertk/preprocessing/resample.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     7582 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/spectrogram.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3873 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/preprocessing/speechbrain.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6104 2023-06-05 12:55:24.000000 ertk-2023.6.0/src/ertk/preprocessing/vad_trim.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.069041 ertk-2023.6.0/src/ertk/pytorch/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      254 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     7244 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/classification.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6663 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/dataset.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.070041 ertk-2023.6.0/src/ertk/pytorch/models/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1863 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/models/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    10576 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/models/_base.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2109 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/models/aldeneh2017.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    13457 2023-06-06 04:37:04.000000 ertk-2023.6.0/src/ertk/pytorch/models/audeep.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2572 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/models/layers.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      885 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/models/mlp.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2954 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/models/mtl.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2119 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/models/simple_mtl.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3279 2022-08-12 01:08:58.000000 ertk-2023.6.0/src/ertk/pytorch/models/test_fit.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1630 2022-10-17 03:23:29.000000 ertk-2023.6.0/src/ertk/pytorch/models/wav2vec_ft.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2285 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/models/zhang2019.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1387 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/train.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6872 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/pytorch/utils.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.071041 ertk-2023.6.0/src/ertk/sklearn/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      353 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/sklearn/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3637 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/sklearn/classification.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.071041 ertk-2023.6.0/src/ertk/sklearn/models/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1671 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/sklearn/models/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     5890 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/sklearn/models/_base.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    10546 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/sklearn/models/mtl.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2868 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/sklearn/models/svm.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4892 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/sklearn/utils.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    11005 2023-06-05 00:42:02.000000 ertk-2023.6.0/src/ertk/stats.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.072041 ertk-2023.6.0/src/ertk/tensorflow/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      329 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    12690 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/classification.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     8461 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/dataset.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.074041 ertk-2023.6.0/src/ertk/tensorflow/models/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1825 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      709 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/_base.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1679 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/aldeneh2017.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    14037 2023-06-06 04:26:41.000000 ertk-2023.6.0/src/ertk/tensorflow/models/audeep.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      989 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/depinto2020.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1590 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/iskhakova2020.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2555 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/latif2019.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      662 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/layers.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      665 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/mlp.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    25617 2023-06-06 04:21:52.000000 ertk-2023.6.0/src/ertk/tensorflow/models/rbm.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2613 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/test_fit.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1799 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/transformer.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2635 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/zhang2019.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1867 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/models/zhao2019.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      556 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/train.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4737 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/tensorflow/utils.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    14799 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/train.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     5731 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/transform.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.074041 ertk-2023.6.0/src/ertk/utils/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1274 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/utils/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    18089 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/utils/array.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     5219 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/utils/generic.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2635 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/utils/misc.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      239 2023-06-05 12:53:26.000000 ertk-2023.6.0/src/ertk/utils/types.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.060041 ertk-2023.6.0/src/ertk.egg-info/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6079 2023-06-06 05:39:13.000000 ertk-2023.6.0/src/ertk.egg-info/PKG-INFO
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    10609 2023-06-06 05:39:14.000000 ertk-2023.6.0/src/ertk.egg-info/SOURCES.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        1 2023-06-06 05:39:13.000000 ertk-2023.6.0/src/ertk.egg-info/dependency_links.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      924 2023-06-06 05:39:13.000000 ertk-2023.6.0/src/ertk.egg-info/entry_points.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      622 2023-06-06 05:39:13.000000 ertk-2023.6.0/src/ertk.egg-info/requires.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        5 2023-06-06 05:39:13.000000 ertk-2023.6.0/src/ertk.egg-info/top_level.txt
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.075041 ertk-2023.6.0/tests/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      100 2022-10-09 21:53:05.000000 ertk-2023.6.0/tests/README.md
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.075041 ertk-2023.6.0/tests/cli/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        0 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/cli/__init__.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.076041 ertk-2023.6.0/tests/cli/cli/
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)        0 2023-04-27 14:10:06.000000 ertk-2023.6.0/tests/cli/cli/__init__.py
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)      215 2023-06-01 13:41:56.000000 ertk-2023.6.0/tests/cli/cli/exp.yaml
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)      303 2023-04-27 13:14:00.000000 ertk-2023.6.0/tests/cli/cli/test_classify.py
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)      160 2023-04-27 14:10:19.000000 ertk-2023.6.0/tests/cli/cli/test_cli.py
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)      505 2023-04-27 14:02:59.000000 ertk-2023.6.0/tests/cli/cli/test_exp2.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      300 2023-05-31 09:40:02.000000 ertk-2023.6.0/tests/cli/cli/test_train.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.076041 ertk-2023.6.0/tests/cli/dataset/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        0 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/cli/dataset/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      559 2023-06-01 13:43:07.000000 ertk-2023.6.0/tests/cli/dataset/test_annotation_stats.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      992 2023-06-01 13:42:44.000000 ertk-2023.6.0/tests/cli/dataset/test_combine.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1001 2023-06-01 13:49:56.000000 ertk-2023.6.0/tests/cli/dataset/test_convert.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      725 2023-06-01 13:24:47.000000 ertk-2023.6.0/tests/cli/dataset/test_info.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      765 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/cli/dataset/test_process.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      752 2023-06-01 13:30:27.000000 ertk-2023.6.0/tests/cli/dataset/test_remove_instances.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.077041 ertk-2023.6.0/tests/cli/util/
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)        0 2023-04-27 14:03:57.000000 ertk-2023.6.0/tests/cli/util/__init__.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.078041 ertk-2023.6.0/tests/dataset/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        0 2022-10-09 21:53:05.000000 ertk-2023.6.0/tests/dataset/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    59720 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/dataset/constants.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     1156 2022-10-09 21:53:05.000000 ertk-2023.6.0/tests/dataset/generate_test_features.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2241 2023-05-29 15:30:12.000000 ertk-2023.6.0/tests/dataset/test_annotation.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    13685 2023-05-29 15:30:10.000000 ertk-2023.6.0/tests/dataset/test_dataset.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     6028 2023-05-29 15:30:08.000000 ertk-2023.6.0/tests/dataset/test_features.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2012 2023-05-29 15:30:06.000000 ertk-2023.6.0/tests/dataset/test_utils.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.078041 ertk-2023.6.0/tests/preprocessing/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        0 2023-05-25 15:18:45.000000 ertk-2023.6.0/tests/preprocessing/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      535 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/preprocessing/test_plugins.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    10972 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/preprocessing/test_preprocessing.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)       52 2023-05-20 13:22:29.000000 ertk-2023.6.0/tests/test_config.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.079041 ertk-2023.6.0/tests/test_data/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      360 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/all_clips.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      360 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/all_clips_unsorted.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      273 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/annot1.csv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      246 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/annot2_str.csv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      188 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/corpus2.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      179 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/corpus_fail.yaml
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      348 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/corpus_info.yaml
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.083041 ertk-2023.6.0/tests/test_data/data/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)   265922 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1001_DFA_ANG_XX.flv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)   290553 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1001_DFA_DIS_XX.flv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)   266703 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1001_DFA_FEA_XX.flv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)   233278 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1001_DFA_HAP_XX.flv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)   251524 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1001_DFA_NEU_XX.flv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)   249426 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1001_DFA_SAD_XX.flv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    84422 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1002_DFA_ANG_XX.mp3
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    83587 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1002_DFA_DIS_XX.mp3
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    89432 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1002_DFA_FEA_XX.mp3
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    72732 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1002_DFA_HAP_XX.mp3
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    81917 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1002_DFA_NEU_XX.mp3
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    77742 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/data/1002_DFA_SAD_XX.mp3
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.084040 ertk-2023.6.0/tests/test_data/features/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     4181 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_2d.arff
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     3849 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_2d.csv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    74741 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_2d.nc
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    37216 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_3d.arff
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    36884 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_3d.csv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    74741 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_3d.nc
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    18876 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_vlen.arff
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    18544 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_vlen.csv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    74741 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/features/features_vlen.nc
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      320 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/label.csv
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.086040 ertk-2023.6.0/tests/test_data/resampled/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    72804 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1001_DFA_ANG_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    76146 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1001_DFA_DIS_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    71132 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1001_DFA_FEA_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    61100 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1001_DFA_HAP_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    66116 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1001_DFA_NEU_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    65280 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1001_DFA_SAD_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    83670 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1002_DFA_ANG_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    82834 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1002_DFA_DIS_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    88686 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1002_DFA_FEA_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    71968 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1002_DFA_HAP_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    81162 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1002_DFA_NEU_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    76982 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/resampled/1002_DFA_SAD_XX.wav
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      290 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/speaker.csv
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      180 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/subset.txt
+-rw-r--r--   0 akee511   (1020) akee511   (1020)      472 2023-05-29 15:59:02.000000 ertk-2023.6.0/tests/test_data/transcript.csv
+-rw-rw-r--   0 akee511   (1020) akee511   (1020)        0 2022-10-10 06:26:27.000000 ertk-2023.6.0/tests/test_stats.py
+drwxr-xr-x   0 akee511   (1020) akee511   (1020)        0 2023-06-06 05:39:14.087041 ertk-2023.6.0/tests/utils/
+-rw-r--r--   0 akee511   (1020) akee511   (1020)        0 2022-10-09 21:53:05.000000 ertk-2023.6.0/tests/utils/__init__.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)    11017 2022-11-01 09:02:08.000000 ertk-2023.6.0/tests/utils/test_array.py
+-rw-r--r--   0 akee511   (1020) akee511   (1020)     2014 2022-10-09 21:53:05.000000 ertk-2023.6.0/tests/utils/test_generic.py
```

### Comparing `ertk-2022.4.0/LICENSE` & `ertk-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/classification.py` & `ertk-2023.6.0/src/ertk/classification.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+"""
+Classification functions.
+
+This module contains functions for performing classification tasks.
+
+.. autosummary::
+    :toctree: generated/
+
+    binary_accuracy_score
+    standard_class_scoring
+    cross_validate
+    dataset_cross_validation
+    dataset_train_val_test
+    get_balanced_class_weights
+    get_balanced_sample_weights
+    class_ratings_to_probs
+"""
+
 import logging
 import time
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
@@ -12,16 +30,28 @@
     make_scorer,
     precision_score,
     recall_score,
 )
 from sklearn.model_selection import BaseCrossValidator, LeaveOneGroupOut
 from sklearn.utils.multiclass import unique_labels
 
-from ertk.dataset import LabelledDataset
-from ertk.train import get_cv_splitter, scores_to_df
+from ertk.dataset import Dataset
+from ertk.train import ExperimentResult, get_cv_splitter, scores_to_df
+from ertk.utils import ScoreFunction
+
+__all__ = [
+    "binary_accuracy_score",
+    "standard_class_scoring",
+    "cross_validate",
+    "dataset_cross_validation",
+    "dataset_train_val_test",
+    "get_balanced_class_weights",
+    "get_balanced_sample_weights",
+    "class_ratings_to_probs",
+]
 
 
 def binary_accuracy_score(
     y_true, y_pred, *, labels=None, average="binary", sample_weight=None
 ):
     """Calculated binary accuracy. Binary accuracy is the same as
     accuracy considering only a single class.
@@ -117,33 +147,113 @@
                 ),
                 f"{c}_ba": make_scorer(binary_accuracy_score, average=None, labels=[i]),
             }
         )
     return scoring
 
 
+def cross_validate(
+    clf_lib: str,
+    clf,
+    x: np.ndarray,
+    y: Optional[np.ndarray] = None,
+    *,
+    groups: Optional[np.ndarray] = None,
+    cv: BaseCrossValidator = None,
+    scoring: Union[
+        str, List[str], Dict[str, ScoreFunction], Callable[..., float]
+    ] = "accuracy",
+    verbose: int = 0,
+    n_jobs: int = 1,
+    fit_params: Dict[str, Any] = {},
+):
+    """Cross validate a classifier.
+
+    Parameters
+    ----------
+    clf_lib: str
+        Classifier library to use. Must be one of "sk", "tf", or "pt".
+    clf:
+        Classifier to cross validate.
+    x: np.ndarray
+        Input data.
+    y: np.ndarray, optional
+        Target labels.
+    groups: np.ndarray, optional
+        Groups to split data into for cross validation.
+    cv: BaseCrossValidator, optional
+        Cross validation strategy. If None, use StratifiedKFold.
+    scoring: str, list, dict, or callable, optional
+        Scoring metric(s) to use. If a string, must be a valid
+        scikit-learn scorer.
+    verbose: int, optional
+        Verbosity level.
+    n_jobs: int, optional
+        Number of jobs to run in parallel. Only used for scikit-learn.
+    fit_params: dict, optional
+        Parameters to pass to the classifier's fit method.
+
+    Returns
+    -------
+    result: ExperimentResult
+        Cross validation results.
+    """
+    cross_validate_fn: Callable[..., ExperimentResult]
+    if clf_lib == "sk":
+        from ertk.sklearn.classification import sk_cross_validate
+
+        # We have to set n_jobs here because using a
+        # `with joblib.Parallel...` clause doesn't work properly
+        cross_validate_fn = partial(sk_cross_validate, n_jobs=n_jobs)
+    elif clf_lib == "tf":
+        from ertk.tensorflow.classification import tf_cross_validate
+
+        n_jobs = 1
+        cross_validate_fn = tf_cross_validate
+    elif clf_lib == "pt":
+        from ertk.pytorch.classification import pt_cross_validate
+
+        n_jobs = 1
+        cross_validate_fn = pt_cross_validate
+    else:
+        raise ValueError(f"Unknown classifier type: {clf_lib}")
+
+    result = cross_validate_fn(
+        clf,
+        x,
+        y,
+        groups=groups,
+        cv=cv,
+        scoring=scoring,
+        verbose=verbose,
+        n_jobs=n_jobs,
+        fit_params=fit_params,
+    )
+    return result
+
+
 def dataset_cross_validation(
     clf,
-    dataset: LabelledDataset,
-    clf_lib: Optional[str] = None,
+    dataset: Dataset,
+    clf_lib: str,
     partition: Optional[str] = None,
     label: str = "label",
     cv: Union[BaseCrossValidator, int] = 10,
     verbose: int = 0,
     n_jobs: int = 1,
     scoring=None,
     fit_params: Dict[str, Any] = {},
-) -> pd.DataFrame:
+) -> ExperimentResult:
     """Cross validates a `Classifier` instance on a single dataset.
 
     Parameters
     ----------
     clf: class that implements fit() and predict()
         The classifier to test.
-    dataset: LabelledDataset
+    dataset: Dataset
         The dataset for within-corpus cross-validation.
     clf_lib: str
         One of {"sk", "tf", "pt"} to select which library-specific
         cross-validation method to use, since they're not all quite
         compatible.
     partition: str, optional
         The name of the partition to cross-validate over. If None, then
@@ -172,74 +282,59 @@
     """
     groups = None if partition is None else dataset.get_group_indices(partition)
     if isinstance(cv, int):
         cv = get_cv_splitter(bool(partition), cv)
     if scoring is None:
         scoring = standard_class_scoring(dataset.get_group_names(label))
 
-    cross_validate_fn: Callable[..., Dict[str, Any]]
-    if clf_lib == "sk":
-        from ertk.sklearn.classification import sk_cross_validate
-
-        # We have to set n_jobs here because using a
-        # `with joblib.Parallel...` clause doesn't work properly
-        cross_validate_fn = partial(sk_cross_validate, n_jobs=n_jobs)
-    elif clf_lib == "tf":
-        from ertk.tensorflow.classification import tf_cross_validate
-
-        n_jobs = 1
-        cross_validate_fn = tf_cross_validate
-    elif clf_lib == "pt":
-        from ertk.pytorch.classification import pt_cross_validate
-
-        n_jobs = 1
-        cross_validate_fn = pt_cross_validate
-
-    start_time = time.perf_counter()
     logging.info(f"Starting cross-validation with n_jobs={n_jobs}")
-    scores = cross_validate_fn(
+    start_time = time.perf_counter()
+    result = cross_validate(
+        clf_lib,
         clf,
         dataset.x,
         dataset.get_group_indices(label),
+        groups=groups,
         cv=cv,
         scoring=scoring,
-        groups=groups,
         verbose=verbose,
+        n_jobs=n_jobs,
         fit_params=fit_params,
     )
     total_time = time.perf_counter() - start_time
     logging.info(f"Cross-validation complete in {total_time:.2f}s")
 
     index = None
     if isinstance(cv, LeaveOneGroupOut) and partition is not None:
         index = dataset.get_group_names(partition)
-    return scores_to_df(scores, index=index)
+    result.scores_df = scores_to_df(result.scores_dict, index=index)
+    return result
 
 
-def train_val_test(
+def dataset_train_val_test(
     clf,
-    dataset: LabelledDataset,
+    dataset: Dataset,
     train_idx: Union[Sequence[int], np.ndarray],
     valid_idx: Union[Sequence[int], np.ndarray],
     test_idx: Union[Sequence[int], np.ndarray, None] = None,
     label: str = "label",
     clf_lib: Optional[str] = None,
-    sample_weight: np.ndarray = None,
+    sample_weight: Optional[np.ndarray] = None,
     verbose: int = 0,
     scoring=None,
     fit_params: Dict[str, Any] = {},
-) -> pd.DataFrame:
+) -> ExperimentResult:
     """Trains a `Classifier` instance on some training data, optionally
     using validation data, and returns results on given test data.
 
     Parameters
     ----------
     clf: class that implements fit() and predict()
         The classifier to test.
-    dataset: LabelledDataset
+    dataset: Dataset
         The dataset for within-corpus cross-validation.
     clf_lib: str
         One of {"sk", "tf", "pt"} to select which library-specific
         cross-validation method to use, since they're not all quite
         compatible.
     verbose: bool
         Passed to train_val_test().
@@ -255,15 +350,15 @@
     -------
     df: pandas.DataFrame
         A dataframe holding the results from all runs with this model.
     """
     if scoring is None:
         scoring = standard_class_scoring(dataset.get_group_names(label))
 
-    train_val_test_fn: Callable[..., Dict[str, Any]]
+    train_val_test_fn: Callable[..., ExperimentResult]
     if clf_lib == "sk":
         from ertk.sklearn.classification import sk_train_val_test
 
         train_val_test_fn = sk_train_val_test
     elif clf_lib == "tf":
         from ertk.tensorflow.classification import tf_train_val_test
 
@@ -291,27 +386,28 @@
         valid_data = valid_data + (sample_weight[valid_idx],)
     test_data: Tuple = (dataset.x[test_idx], y[test_idx])
     if sample_weight is not None:
         test_data = test_data + (sample_weight[test_idx],)
 
     start_time = time.perf_counter()
     logging.info("Starting train/val/test.")
-    scores = train_val_test_fn(
+    result = train_val_test_fn(
         clf,
         train_data,
         valid_data,
         test_data,
         scoring=scoring,
         verbose=verbose,
         fit_params=fit_params,
     )
     total_time = time.perf_counter() - start_time
     logging.info(f"Train/val/test complete in {total_time:.2f}s")
 
-    return scores_to_df(scores)
+    result.scores_df = scores_to_df(result.scores_dict)
+    return result
 
 
 def get_balanced_sample_weights(labels: Union[List[int], np.ndarray]):
     """Gets sample weights such that each unique label has the same
     total weight across all instances.
 
     Parameters
@@ -324,7 +420,54 @@
     sample_weights: np.ndarray
         Array of sample weights of length n_samples.
     """
     unique, indices, counts = np.unique(labels, return_counts=True, return_inverse=True)
     class_weight = len(labels) / (len(unique) * counts)
     sample_weights = class_weight[indices].astype(np.float32)
     return sample_weights
+
+
+def get_balanced_class_weights(classes: Union[List[int], np.ndarray]):
+    """Gets class weights such that each class has the same total weight
+    across all instances.
+
+    Parameters
+    ----------
+    classes: list or array
+        Sequence of classes of length n_samples.
+
+    Returns
+    -------
+    class_weights: np.ndarray
+        Array of class weights of length n_classes.
+    """
+    unique, counts = np.unique(classes, return_counts=True)
+    class_weights = len(classes) / (len(unique) * counts)
+    return class_weights
+
+
+def class_ratings_to_probs(
+    ratings: pd.Series, classes: Optional[List[str]] = None
+) -> np.ndarray:
+    """Convert annotator ratings into distribution over classes for each
+    instance.
+
+    Parameters
+    ----------
+    ratings: pd.Series
+        The Pandas `Series` containing the ratings.
+    classes: list of str, optional
+        Limit to these classes.
+
+    Returns
+    -------
+    numpy.ndarray
+        Matrix of shape (n_instances, n_classes) containing
+        probabilities (relative frequencies) for each class.
+    """
+    ratings = ratings.astype("category")
+    if classes:
+        ratings = ratings.cat.set_categories(classes)
+
+    mat = ratings.groupby(level=0).value_counts(sort=False).unstack().to_numpy()
+    mat = mat / np.sum(mat, axis=1, keepdims=True)
+    return mat
```

### Comparing `ertk-2022.4.0/src/ertk/cli/class_cv.py` & `ertk-2023.6.0/src/ertk/cli/cli/exp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,219 +1,128 @@
 import json
 import warnings
-from functools import partial
 from pathlib import Path
 from typing import Tuple
 
 import click
 import numpy as np
 import pandas as pd
-from click_option_group import optgroup
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import MinMaxScaler, StandardScaler
 
-from ertk.classification import dataset_cross_validation, get_balanced_sample_weights
+from ertk.classification import (
+    dataset_cross_validation,
+    dataset_train_val_test,
+    get_balanced_sample_weights,
+)
+from ertk.cli._utils import (
+    dataset_args,
+    debug_args,
+    eval_args,
+    model_args,
+    result_args,
+    train_args,
+)
 from ertk.config import get_arg_mapping
 from ertk.dataset import load_multiple
-from ertk.train import get_cv_splitter
+from ertk.sklearn.utils import GridSearchVal
+from ertk.train import ValidationSplit, get_cv_splitter
 from ertk.transform import SequenceTransformWrapper
 
 
 @click.command()
-@click.argument(
-    "input", type=click.Path(exists=True, dir_okay=False, path_type=Path), nargs=-1
-)
-@click.option("--features", required=True, help="Features to load.")
-@click.option("--clf", "clf_type", required=True, help="Classifier to use.")
-@optgroup.group("Results options")
-@optgroup.option("--results", type=Path, help="Results directory.")
-@optgroup.option("--logdir", type=Path, help="TF/PyTorch logs directory.")
-@optgroup.group("Data options")
-@optgroup.option("--label", default="label", help="Label annotation to use.")
-@optgroup.option(
-    "--subset", multiple=True, default=["default"], help="Subset selection."
-)
-@optgroup.option("--map_groups", multiple=True, help="Group name mapping.")
-@optgroup.option(
-    "--sel_groups",
-    multiple=True,
-    help="Group selection. This is a map from partition to group(s).",
-)
-@optgroup.option(
-    "--clip_seq", type=int, help="Clip sequences to this length (before pad)."
-)
-@optgroup.option(
-    "--pad_seq", type=int, help="Pad sequences to multiple of this length (after clip)."
-)
-@optgroup.group("Cross-validation options")
-@optgroup.option("--partition", help="Partition for LOGO CV.")
-@optgroup.option(
-    "--kfold",
-    type=int,
-    default=5,
-    help="k when using (group) k-fold cross-validation, or leave-one-out.",
-)
-@optgroup.option(
-    "--inner_kfold",
-    type=int,
-    default=2,
-    help="k for inner k-fold CV (where relevant). If -1 then LOGO is used. If 1 then a "
-    "random split is used.",
-)
-@optgroup.option("--test_size", type=float, help="Test size when kfold=1.")
-@optgroup.option(
-    "--inner_part", help="Which partition to use for group-based inner CV."
-)
-@optgroup.group("Training options")
-@optgroup.option("--learning_rate", type=float, default=1e-4, show_default=True)
-@optgroup.option("--batch_size", type=int, default=64, show_default=True)
-@optgroup.option("--epochs", type=int, default=50, show_default=True)
-@optgroup.option(
-    "--balanced/--imbalanced", default=True, help="Balances sample weights."
-)
-@optgroup.option(
-    "--n_gpus", type=int, default=1, show_default=True, help="Number of GPUs to use."
-)
-@optgroup.option(
-    "--reps",
-    type=int,
-    default=1,
-    show_default=True,
-    help="The number of repetitions to do per test.",
-)
-@optgroup.option(
-    "--normalise",
-    default="online",
-    show_default=True,
-    help="Normalisation method. 'online' means use training data for normalisation.",
-)
-@optgroup.option(
-    "--transform",
-    type=click.Choice(["std", "minmax"]),
-    default="std",
-    show_default=True,
-    help="Transformation class.",
-)
-@optgroup.option(
-    "--n_jobs", type=int, default=-1, help="Number of parallel executions."
-)
-@optgroup.group("Misc. options")
-@optgroup.option(
-    "--verbose",
-    type=int,
-    default=0,
-    help="Verbosity. -1=nothing, 0=dataset+results, 1=INFO, 2=DEBUG",
-)
-@optgroup.group("Model-specific options")
-@optgroup.option(
-    "--clf_args",
-    "clf_args_file",
-    type=click.Path(exists=True, dir_okay=False, path_type=Path),
-    multiple=True,
-    help="File containing keyword arguments to give to model initialisation.",
-)
-@optgroup.option(
-    "--param_grid",
-    "param_grid_file",
-    type=click.Path(exists=True, path_type=Path),
-    multiple=True,
-    help="File with parameter grid data.",
-)
-@optgroup.group(
-    "Deprecated options", help="These options are deprecated, don't use them."
-)
-@optgroup.option(
-    "--inner_cv/--noinner_cv",
-    "use_inner_cv",
-    default=True,
-    help="Whether to use inner CV. This is deprecated and only exists for backwards "
-    "compatibility.",
-)
+@dataset_args
+@eval_args
+@model_args
+@result_args
+@train_args
+@debug_args
 def main(
     clf_type: str,
-    input: Tuple[Path],
+    corpus_info: Tuple[Path],
+    data_config: Path,
     features: str,
-    partition: str,
+    cv_part: str,
     label: str,
     kfold: int,
     inner_kfold: int,
     test_size: float,
     inner_part: str,
     results: Path,
     logdir: Path,
     reps: int,
     normalise: str,
     transform: str,
     balanced: bool,
     subset: Tuple[str],
     map_groups: Tuple[str],
     sel_groups: Tuple[str],
+    remove_groups: Tuple[str],
     clip_seq: int,
     pad_seq: int,
     verbose: int,
     clf_args_file: Tuple[Path],
     param_grid_file: Tuple[Path],
     learning_rate: float,
     batch_size: int,
     epochs: int,
     use_inner_cv: bool,
     n_jobs: int,
     n_gpus: int,
+    train: str,
+    valid: str,
+    test: str,
+    train_config_path: Path,
+    seq_transform: str,
+    sample_rate: int,
 ):
-    """Runs cross-validation on the given INPUT datasets. Metrics are
-    optionally written to a results file.
-    """
-
     np.set_printoptions(precision=4, threshold=10)
     if verbose > 0:
         import logging
 
         logging.basicConfig(level=logging.DEBUG if verbose > 1 else logging.INFO)
         np.set_printoptions()
 
-    if len(subset) == 1:
-        dataset = load_multiple(input, features, subsets=subset[0])
+    if (train and kfold) or (not train and not kfold):
+        raise ValueError("Exactly one of train and kfold must be given.")
+
+    read_kwargs = {"sample_rate": sample_rate} if sample_rate else {}
+    if len(subset) == 1 and ":" not in subset[0]:
+        dataset = load_multiple(
+            corpus_info, features, subsets=subset[0], label=label, **read_kwargs
+        )
     else:
         subset_map = {}
         for m in subset:
             subset_map.update(get_arg_mapping(m))
-        dataset = load_multiple(input, features, subsets=subset_map)
+        dataset = load_multiple(
+            corpus_info, features, subsets=subset_map, label=label, **read_kwargs
+        )
 
+    grp_map = {}
     for m in map_groups:
-        mapping = get_arg_mapping(m)
-        for part in mapping:
-            if part not in dataset.partitions:
-                warnings.warn(
-                    f"Partition {part} cannot be mapped as it is not in the dataset."
-                )
-                continue
-            dataset.map_groups(part, mapping[part])
+        grp_map.update(get_arg_mapping(m))
+    grp_sel = {}
     for m in sel_groups:
-        mapping = get_arg_mapping(m)
-        for part in mapping:
-            if part not in dataset.partitions:
-                warnings.warn(
-                    f"Partition {part} cannot be selected as it is not in the dataset."
-                )
-                continue
-            keep = mapping[part]
-            if isinstance(keep, str):
-                keep = [keep]
-            dataset.remove_groups(part, keep=keep)
+        grp_sel.update(get_arg_mapping(m))
+    grp_del = {}
+    for m in remove_groups:
+        grp_del.update(get_arg_mapping(m))
+    dataset.map_and_select(grp_map, grp_sel, grp_del)
 
     if clip_seq:
         dataset.clip_arrays(clip_seq)
     if pad_seq:
         dataset.pad_arrays(pad_seq)
 
     transformer = {"std": StandardScaler, "minmax": MinMaxScaler}[transform]()
     if normalise == "none":
         transformer = None
     elif normalise == "online" and len(dataset.x[0].shape) > 1:
-        transformer = SequenceTransformWrapper(transformer, "feature")
+        transformer = SequenceTransformWrapper(transformer, seq_transform)
     elif normalise != "online":
         dataset.normalise(normaliser=transformer, partition=normalise)
         transformer = None
 
     sample_weight = None
     if balanced:
         sample_weight = get_balanced_sample_weights(dataset.get_annotations(label))
@@ -222,166 +131,228 @@
     model_args = {}
     for file in clf_args_file:
         model_args.update(get_arg_mapping(file))
     param_grid = {}
     for file in param_grid_file:
         param_grid.update(get_arg_mapping(file))
 
-    cv = get_cv_splitter(bool(partition), kfold, test_size=test_size)
-    if not use_inner_cv:
-        warnings.warn(
-            "--noinner_cv is deprecated and only exists for backwards compatibility."
-        )
-        inner_cv = cv
+    if not train:
+        cv = get_cv_splitter(bool(cv_part), kfold, test_size=test_size)
+        if not use_inner_cv:
+            warnings.warn(
+                "--noinner_cv is deprecated and only exists for backwards "
+                "compatibility."
+            )
+            inner_cv = cv
+        else:
+            inner_cv = get_cv_splitter(
+                bool(inner_part), inner_kfold, shuffle=True, random_state=54321
+            )
     else:
-        inner_cv = get_cv_splitter(bool(inner_part), inner_kfold)
+        if not valid:
+            raise ValueError("valid must be specified.")
+        train_indices = dataset.get_idx_for_split(train)
+        valid_indices = dataset.get_idx_for_split(valid)
+        if not test:
+            test = valid
+        test_indices = dataset.get_idx_for_split(test)
+        inner_cv = ValidationSplit(
+            np.arange(len(train_indices), len(train_indices) + len(valid_indices))
+        )
 
     clf_lib, clf_type = clf_type.split("/")
     if clf_lib == "sk":
         from sklearn.model_selection import GridSearchCV
 
         from ertk.sklearn.models import get_sk_model
 
         clf = get_sk_model(clf_type, **model_args)
-        clf = GridSearchCV(
+        if train:
+            # A hack so that the ValidationSplit works properly.
+            train_indices = np.concatenate([train_indices, valid_indices])
+            grid_search = GridSearchVal
+        else:
+            grid_search = GridSearchCV
+        clf = grid_search(
             Pipeline([("transform", transformer), ("clf", clf)]),
             {f"clf__{k}": v for k, v in param_grid.items()},
             scoring="balanced_accuracy",
             cv=inner_cv,
             verbose=max(verbose, 0),
-            n_jobs=1 if use_inner_cv else n_jobs,
+            n_jobs=1 if use_inner_cv and not train else n_jobs,
         )
         if inner_part:
             fit_params["groups"] = dataset.get_group_indices(inner_part)
-        params = param_grid
         if not use_inner_cv:
             # Get best params then pass best to main cross-validation routine
             # XXX: This exists because of mistake in our original implementation.
             clf.fit(
                 dataset.x,
                 dataset.labels,
-                groups=dataset.get_group_indices(partition) if partition else None,
+                groups=dataset.get_group_indices(cv_part) if cv_part else None,
                 clf__sample_weight=sample_weight,
             )
             params = clf.best_params_
             clf = clf.best_estimator_
     elif clf_lib == "tf":
-        from tensorflow.keras.optimizers import Adam
+        from keras.callbacks import TensorBoard
+        from keras.optimizers import get as get_optimizer
 
         from ertk.tensorflow import get_tf_model
         from ertk.tensorflow.classification import tf_classification_metrics
 
+        callbacks = []
+        if logdir is not None:
+            callbacks.append(
+                TensorBoard(
+                    log_dir=logdir,
+                    profile_batch=0,
+                    write_graph=False,
+                    write_images=False,
+                )
+            )
         # No parallel CV to avoid running out of GPU memory
         n_jobs = 1
         fit_params.update(
             {
-                "log_dir": logdir,
                 "epochs": epochs,
+                "callbacks": callbacks,
                 "batch_size": batch_size,
                 "data_fn": None,
                 "n_gpus": n_gpus,
+                "log_dir": logdir,
             }
         )
         model_args.update(
             {"n_features": dataset.n_features, "n_classes": dataset.n_classes}
         )
 
         def model_fn():
             model = get_tf_model(clf_type, **model_args)
             model.compile(
-                Adam(learning_rate=learning_rate),
+                get_optimizer("adam")(learning_rate=learning_rate),
                 loss="sparse_categorical_crossentropy",
                 metrics=tf_classification_metrics(),
             )
             return Pipeline([("transform", transformer), ("clf", model)])
 
         params = {
             "optimiser": "adam",
             "learning_rate": learning_rate,
+            "batch_size": batch_size,
             **model_args,
             **fit_params,
         }
         clf = model_fn
     elif clf_lib == "pt":
-        import torch.optim
+        from omegaconf import OmegaConf
 
-        from ertk.pytorch import get_pt_model
+        from ertk.pytorch.models import PyTorchModelConfig, get_pt_model
+        from ertk.pytorch.train import PyTorchLoggingConfig, PyTorchTrainConfig
 
         n_jobs = 1
-        optim_fn = partial(torch.optim.Adam, lr=learning_rate)
-        fit_params.update(
-            {
-                "log_dir": logdir,
-                "max_epochs": epochs,
-                "batch_size": batch_size,
-                "optim_fn": optim_fn,
-                "n_gpus": n_gpus,
-            }
-        )
-        model_args.update(
-            {"n_features": dataset.n_features, "n_classes": dataset.n_classes}
-        )
+        if train_config_path:
+            train_config = PyTorchTrainConfig.from_file(train_config_path)
+        else:
+            train_config = PyTorchTrainConfig(
+                batch_size=batch_size,
+                n_gpus=n_gpus,
+                epochs=epochs,
+                logging=PyTorchLoggingConfig(log_dir=str(logdir)),
+            )
+        fit_params.update({"train_config": train_config})
+
+        model_config: PyTorchModelConfig = OmegaConf.create(model_args)
+        if model_config.n_features == -1:
+            model_config.n_features = dataset.n_features
+        elif model_config.n_features != dataset.n_features:
+            logging.warning("`n_features` differs between dataset and model_config")
+        if model_config.n_classes == -1:
+            model_config.n_classes = dataset.n_classes
+        elif model_config.n_classes != dataset.n_classes:
+            raise ValueError("`n_classes` differs between dataset and model_config")
 
         def model_fn():
-            model = get_pt_model(clf_type, **model_args)
+            model = get_pt_model(clf_type, config=model_config)
             return model if transformer is None else (transformer, model)
 
         params = {
-            "optimiser": "adam",
-            "learning_rate": learning_rate,
-            **model_args,
-            **fit_params,
+            **PyTorchModelConfig.to_dictconfig(model_config),
+            **PyTorchTrainConfig.to_dictconfig(train_config),
         }
         clf = model_fn
     else:
         raise ValueError(f"Invalid classifier type {clf_type}")
 
     if verbose > -1:
         print("== Dataset ==")
         print(dataset)
-        print("== Cross-validation settings ==")
+        print("== Training/evaluation settings ==")
         print(f"Using {dataset.n_classes}-class classification.")
         print(f"Using {n_jobs} parallel jobs.")
         print(f"Using classifier {clf}.")
         print(f"Using fit_params={fit_params}")
-        print(f"Using {kfold} k-fold CV.")
-        if partition:
-            print(f"Using {partition} as split partition.")
-        if use_inner_cv:
-            if inner_part:
-                print(f"Using {inner_part} as inner split partition.")
-            print(f"Using {inner_cv} as inner CV splitter.")
+        if train:
+            print(f"Training set: {train}")
+            print(f"Validation set: {valid}")
+            print(f"Test set: {test}")
+        else:
+            print(f"Using {kfold} k-fold CV.")
+            if cv_part:
+                print(f"Using {cv_part} as split partition.")
+            if use_inner_cv:
+                if inner_part:
+                    print(f"Using {inner_part} as inner split partition.")
+                print(f"Using {inner_cv} as inner CV splitter.")
         if balanced:
             print("Using balanced sample weights.")
         if normalise == "online":
             print("Using 'online' normalisation.")
-        else:
+        elif normalise != "none":
             print(f"Normalising globally using {normalise} partition.")
+        if normalise != "none":
+            print(f"Using transformer {transformer}")
 
     dfs = []
     for rep in range(1, reps + 1):
         if verbose > -1:
             print(f"Rep {rep}/{reps}")
-        df = dataset_cross_validation(
-            clf,
-            dataset,
-            clf_lib=clf_lib,
-            partition=partition,
-            label=label,
-            cv=cv,
-            verbose=max(verbose, 0),
-            n_jobs=n_jobs,
-            fit_params=fit_params,
-        )
-        df["params"] = [json.dumps(params, default=str)] * len(df)
+        if train:
+            res = dataset_train_val_test(
+                clf,
+                dataset=dataset,
+                train_idx=train_indices,
+                valid_idx=valid_indices,
+                test_idx=test_indices,
+                label=label,
+                clf_lib=clf_lib,
+                sample_weight=sample_weight,
+                verbose=verbose,
+                fit_params=fit_params,
+            )
+        else:
+            res = dataset_cross_validation(
+                clf,
+                dataset,
+                clf_lib=clf_lib,
+                partition=cv_part,
+                label=label,
+                cv=cv,
+                verbose=max(verbose, 0),
+                n_jobs=n_jobs,
+                fit_params=fit_params,
+            )
+        df = res.scores_df
+        if "params" not in df:
+            df["params"] = [json.dumps(params, default=str)] * len(df)
         dfs.append(df)
     df = pd.concat(dfs, keys=list(range(1, reps + 1)), names=["rep"])
     df["clf"] = f"{clf_lib}/{clf_type}"
+    df["features"] = features
     df["corpus"] = dataset.corpus
-    df["features"] = Path(features).stem
     if results:
         results.parent.mkdir(parents=True, exist_ok=True)
         df.to_csv(results)
         print(f"Wrote CSV to {results}")
     else:
         print(df)
     if verbose > -1:
```

### Comparing `ertk-2022.4.0/src/ertk/cli/class_tvt.py` & `ertk-2023.6.0/src/ertk/cli/cli/exp2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,359 +1,323 @@
 import json
-import warnings
-from functools import partial
+import logging
 from pathlib import Path
 from typing import Tuple
 
 import click
 import numpy as np
-from click_option_group import optgroup
+import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import MinMaxScaler, StandardScaler
 
-from ertk.classification import get_balanced_sample_weights, train_val_test
+from ertk.classification import (
+    dataset_cross_validation,
+    dataset_train_val_test,
+    get_balanced_sample_weights,
+)
+from ertk.cli._utils import debug_args
 from ertk.config import get_arg_mapping
-from ertk.dataset import load_multiple
-from ertk.train import ValidationSplit
+from ertk.dataset import load_datasets_config
+from ertk.sklearn.utils import GridSearchVal
+from ertk.train import ExperimentConfig, ValidationSplit, get_cv_splitter
 from ertk.transform import SequenceTransformWrapper
 
 
 @click.command()
 @click.argument(
-    "input", type=click.Path(exists=True, dir_okay=False, path_type=Path), nargs=-1
-)
-@click.option("--features", required=True, help="Features to load.")
-@click.option("--clf", "clf_type", required=True, help="Classifier to use.")
-@click.option("--train", required=True, help="Train data.")
-@click.option("--valid", required=True, help="Validation data.")
-@click.option("--test", required=True, help="Test data.")
-@optgroup.group("Results options")
-@optgroup.option("--results", type=Path, help="Results directory.")
-@optgroup.option("--logdir", type=Path, help="TF/PyTorch logs directory.")
-@optgroup.group("Data options")
-@optgroup.option("--label", default="label", help="Label annotation to use.")
-@optgroup.option(
-    "--subset", multiple=True, default=["default"], help="Subset selection."
-)
-@optgroup.option("--map_groups", multiple=True, help="Group mapping.")
-@optgroup.option(
-    "--sel_groups",
-    multiple=True,
-    help="Group selection. This is a map from partition to group.",
-)
-@optgroup.option(
-    "--clip_seq", type=int, help="Clip sequences to this length (before pad)."
-)
-@optgroup.option(
-    "--pad_seq", type=int, help="Pad sequences to multiple of this length (after clip)."
-)
-@optgroup.group("Experiment options")
-@optgroup.option(
-    "--n_gpus", type=int, default=1, show_default=True, help="Number of GPUs to use."
-)
-@optgroup.option(
-    "--reps",
-    type=int,
-    default=1,
-    show_default=True,
-    help="The number of repetitions to do per test.",
-)
-@optgroup.option(
-    "--normalise",
-    default="online",
-    show_default=True,
-    help="Normalisation method. 'online' means use training data for normalisation.",
-)
-@optgroup.option(
-    "--transform",
-    type=click.Choice(["std", "minmax"]),
-    default="std",
-    show_default=True,
-    help="Transformation class.",
-)
-@optgroup.option(
-    "--balanced/--imbalanced", default=True, help="Balances class weights."
-)
-@optgroup.group("Misc. options")
-@optgroup.option(
-    "--verbose",
-    type=int,
-    default=0,
-    help="Verbosity. -1=nothing, 0=dataset+results, 1=INFO, 2=DEBUG",
+    "config_path", type=click.Path(exists=True, dir_okay=False, path_type=Path)
 )
-@optgroup.group("Model-specific options")
-@optgroup.option(
-    "--clf_args",
-    "clf_args_file",
-    type=click.Path(exists=True, dir_okay=False, path_type=Path),
-    multiple=True,
-    help="File containing keyword arguments to give to model initialisation.",
-)
-@optgroup.option(
-    "--param_grid",
-    "param_grid_file",
-    type=click.Path(exists=True, path_type=Path),
-    multiple=True,
-    help="File with parameter grid data.",
-)
-@optgroup.option("--learning_rate", type=float, default=1e-4, show_default=True)
-@optgroup.option("--batch_size", type=int, default=64, show_default=True)
-@optgroup.option("--epochs", type=int, default=50, show_default=True)
-def main(
-    clf_type: str,
-    input: Tuple[Path],
-    features: str,
-    train: str,
-    valid: str,
-    test: str,
-    label: str,
-    param_grid_file: Tuple[Path],
-    results: Path,
-    logdir: Path,
-    reps: int,
-    normalise: str,
-    transform: str,
-    balanced: bool,
-    subset: Tuple[str],
-    map_groups: Tuple[str],
-    sel_groups: Tuple[str],
-    clip_seq: int,
-    pad_seq: int,
-    verbose: int,
-    clf_args_file: Tuple[Path],
-    learning_rate: float,
-    batch_size: int,
-    epochs: int,
-    n_gpus: int,
-):
-    """Runs training on the given INPUT dataset, using training set.
-    Validation is done on validation set and results reported on test
-    set. Metrics are optionally written to a results file.
-    """
+@click.argument("restargs", type=str, nargs=-1)
+@debug_args
+def main(config_path: Path, restargs: Tuple[str], verbose: int):
+    config = ExperimentConfig.from_file(config_path, override=list(restargs))
 
     np.set_printoptions(precision=4, threshold=10)
     if verbose > 0:
-        import logging
-
         logging.basicConfig(level=logging.DEBUG if verbose > 1 else logging.INFO)
         np.set_printoptions()
+        logging.info(f"Config: {ExperimentConfig.to_string(config)}")
 
-    if len(subset) == 1:
-        dataset = load_multiple(input, features, subsets=subset[0])
-    else:
-        subset_map = {}
-        for m in subset:
-            subset_map.update(get_arg_mapping(m))
-        dataset = load_multiple(input, features, subsets=subset_map)
-
-    for m in map_groups:
-        mapping = get_arg_mapping(m)
-        for part in mapping:
-            if part not in dataset.partitions:
-                warnings.warn(
-                    f"Partition {part} cannot be mapped as it is not in the dataset."
-                )
-                continue
-            dataset.map_groups(part, mapping[part])
-    for m in sel_groups:
-        mapping = get_arg_mapping(m)
-        for part in mapping:
-            if part not in dataset.partitions:
-                warnings.warn(
-                    f"Partition {part} cannot be selected as it is not in the dataset."
-                )
-                continue
-            keep = mapping[part]
-            if isinstance(keep, str):
-                keep = [keep]
-            dataset.remove_groups(part, keep=keep)
-
-    if clip_seq:
-        dataset.clip_arrays(clip_seq)
-    if pad_seq:
-        dataset.pad_arrays(pad_seq)
+    dataset = load_datasets_config(config.data)
 
+    transform = config.training.transform.name
     transformer = {"std": StandardScaler, "minmax": MinMaxScaler}[transform]()
+    normalise = config.training.normalise
     if normalise == "none":
         transformer = None
     elif normalise == "online" and len(dataset.x[0].shape) > 1:
-        transformer = SequenceTransformWrapper(transformer, "feature")
+        transformer = SequenceTransformWrapper(
+            transformer, config.training.seq_transform
+        )
     elif normalise != "online":
         dataset.normalise(normaliser=transformer, partition=normalise)
         transformer = None
 
+    fit_params = {}
+
     sample_weight = None
+    balanced = config.training.balanced
     if balanced:
-        sample_weight = get_balanced_sample_weights(dataset.get_annotations(label))
-    fit_params = {"sample_weight": sample_weight}
+        sample_weight = get_balanced_sample_weights(dataset.y)
 
-    model_args = {}
-    for file in clf_args_file:
-        model_args.update(get_arg_mapping(file))
-    param_grid = {}
-    for file in param_grid_file:
-        param_grid.update(get_arg_mapping(file))
-
-    train_indices = dataset.get_idx_for_split(train)
-    valid_indices = dataset.get_idx_for_split(valid)
-    test_indices = dataset.get_idx_for_split(test)
+    param_grid = config.model.param_grid
+    if config.model.param_grid_path:
+        param_grid.update(get_arg_mapping(config.model.param_grid_path))
+
+    evaluation = config.eval
+    if evaluation is None:
+        raise ValueError("Must specify evaluation to run")
+    cv_conf = evaluation.cv
+
+    if evaluation.inner_kfold is not None:
+        inner_cv = get_cv_splitter(
+            bool(evaluation.inner_part),
+            evaluation.inner_kfold,
+            shuffle=True,
+            random_state=54321,
+        )
+    if cv_conf is not None:
+        fit_params["sample_weight"] = sample_weight
+        cv = get_cv_splitter(
+            bool(cv_conf.part),
+            cv_conf.kfold,
+            test_size=cv_conf.test_size,
+        )
+        if evaluation.inner_kfold is None and not param_grid:
+            raise ValueError(
+                "Need to specify inner_kfold when doing CV with param_grid"
+            )
+    elif evaluation.train:
+        if not evaluation.valid:
+            raise ValueError("valid must be specified.")
+        if not evaluation.test:
+            evaluation.test = evaluation.valid
+        train_indices = dataset.get_idx_for_split(evaluation.train)
+        valid_indices = dataset.get_idx_for_split(evaluation.valid)
+        test_indices = dataset.get_idx_for_split(evaluation.test)
+    else:
+        raise ValueError("Either eval.cv or eval.train must be set.")
+    n_jobs = config.training.n_jobs
 
-    clf_lib, clf_type = clf_type.split("/", maxsplit=1)
+    clf_type = config.model.type
+    clf_lib, clf_type = clf_type.split("/")
     if clf_lib == "sk":
-        from sklearn.base import clone
         from sklearn.model_selection import GridSearchCV
 
         from ertk.sklearn.models import get_sk_model
 
-        class GridSearchWrapper(GridSearchCV):
-            """Simple hack to avoid retraining on train + val data."""
-
-            def fit(self, X, y=None, *, groups=None, **fit_params):
-                self.refit = False
-                super().fit(X, y=y, groups=groups, **fit_params)
-                self.best_estimator_ = clone(
-                    clone(self.estimator).set_params(**self.best_params_)
-                )
-                train, _ = next(iter(self.cv.split(X, y, groups)))
-                self.best_estimator_.fit(X[train], y[train], **fit_params)
-                return self.best_estimator_
-
-        clf = get_sk_model(clf_type, **model_args)
-        clf = GridSearchWrapper(
-            Pipeline([("transform", transformer), ("clf", clf)]),
-            {f"clf__{k}": v for k, v in param_grid.items()},
-            scoring="balanced_accuracy",
-            cv=ValidationSplit(
-                np.arange(len(train_indices), len(train_indices) + len(valid_indices))
-            ),
-            verbose=max(verbose, 0),
-            n_jobs=-1,
-            refit=False,
-        )
-        params = param_grid
-        # A hack so that the ValidationSplit works properly.
-        train_indices = np.concatenate([train_indices, valid_indices])
+        if evaluation.inner_kfold is not None and cv_conf is not None:
+            # Outer and inner cross-validation
+            inner_n_jobs = 1
+        else:
+            # Only inner cross-validation
+            inner_n_jobs = n_jobs
+
+        clf = get_sk_model(clf_type, **config.model.config)
+        if evaluation.train and evaluation.inner_kfold is None:
+            # Predefinted train/val split
+            # This is a hack so that the ValidationSplit works properly.
+            inner_cv = ValidationSplit(
+                np.arange(len(train_indices)),
+                np.arange(len(train_indices), len(train_indices) + len(valid_indices)),
+            )
+            train_indices = np.concatenate([train_indices, valid_indices])
+            grid_search = GridSearchVal
+        else:
+            grid_search = GridSearchCV
+
+        clf = Pipeline([("transform", transformer), ("clf", clf)])
+        if "sample_weight" in fit_params:
+            fit_params["clf__sample_weight"] = fit_params.pop("sample_weight")
+
+        if param_grid:
+            clf = grid_search(
+                clf,
+                {f"clf__{k}": v for k, v in param_grid.items()},
+                scoring="balanced_accuracy",
+                cv=inner_cv,
+                verbose=config.training.verbose,
+                n_jobs=inner_n_jobs,
+            )
+            if evaluation.inner_part:
+                fit_params["groups"] = dataset.get_group_indices(evaluation.inner_part)
     elif clf_lib == "tf":
-        from tensorflow.keras.callbacks import TensorBoard
-        from tensorflow.keras.optimizers import Adam
+        from keras.callbacks import TensorBoard
+        from keras.optimizers import get as get_optimizer
 
-        from ertk.tensorflow import get_tf_model
         from ertk.tensorflow.classification import tf_classification_metrics
+        from ertk.tensorflow.models import TFModelConfig, get_tf_model
+        from ertk.tensorflow.train import TFTrainConfig
+
+        if config.training.tensorflow:
+            tf_config = TFTrainConfig.from_config(config.training.tensorflow)
+        else:
+            tf_config = TFTrainConfig()
 
         callbacks = []
-        if logdir is not None:
+        if tf_config.logging.log_dir is not None:
             callbacks.append(
                 TensorBoard(
-                    log_dir=logdir,
+                    log_dir=tf_config.logging.log_dir,
                     profile_batch=0,
                     write_graph=False,
                     write_images=False,
                 )
             )
+        # No parallel CV to avoid running out of GPU memory
+        n_jobs = 1
         fit_params.update(
             {
-                "epochs": epochs,
+                "epochs": tf_config.epochs,
                 "callbacks": callbacks,
-                "batch_size": batch_size,
-                "data_fn": None,
-                "n_gpus": n_gpus,
+                "batch_size": tf_config.batch_size,
+                "data_fn": tf_config.data_fn,
+                "n_gpus": tf_config.n_gpus,
+                "log_dir": tf_config.logging.log_dir,
             }
         )
-        model_args.update(
-            {"n_features": dataset.n_features, "n_classes": dataset.n_classes}
-        )
+        model_config = config.model.config
+        model_config.n_features = dataset.n_features
+        model_config.n_classes = dataset.n_classes
 
         def model_fn():
-            model = get_tf_model(clf_type, **model_args)
+            model = get_tf_model(clf_type, **model_config)
             model.compile(
-                Adam(learning_rate=learning_rate),
+                get_optimizer("adam", learning_rate=model_config.learning_rate),
                 loss="sparse_categorical_crossentropy",
-                metrics=tf_classification_metrics(),
+                weighted_metrics=tf_classification_metrics(),
             )
             return Pipeline([("transform", transformer), ("clf", model)])
 
         params = {
             "optimiser": "adam",
-            "learning_rate": learning_rate,
-            "batch_size": batch_size,
-            **model_args,
+            "learning_rate": model_config.learning_rate,
+            "batch_size": tf_config.batch_size,
+            **config.model.config,
             **fit_params,
         }
         clf = model_fn
     elif clf_lib == "pt":
-        import torch.optim
+        from ertk.pytorch.models import (
+            ERTKPyTorchModel,
+            PyTorchModelConfig,
+            get_pt_model,
+        )
+        from ertk.pytorch.train import PyTorchTrainConfig
 
-        from ertk.pytorch import get_pt_model
+        pt_config = PyTorchTrainConfig.from_config(config.training.pytorch)
 
-        optim_fn = partial(torch.optim.Adam, lr=learning_rate)
-        fit_params.update(
-            {
-                "log_dir": logdir,
-                "max_epochs": epochs,
-                "batch_size": batch_size,
-                "optim_fn": optim_fn,
-                "n_gpus": n_gpus,
-            }
-        )
-        model_args.update(
-            {"n_features": dataset.n_features, "n_classes": dataset.n_classes}
-        )
+        n_jobs = 1
+        fit_params.update({"train_config": pt_config})
+
+        model_cls = ERTKPyTorchModel.get_model_class(clf_type)
+        model_config = model_cls.get_config_type().from_config(config.model.config)
+        if model_config.n_features == -1:
+            model_config.n_features = dataset.n_features
+        elif model_config.n_features != dataset.n_features:
+            logging.warning("`n_features` differs between dataset and model_config")
+        if model_config.n_classes == -1:
+            model_config.n_classes = dataset.n_classes
+        elif model_config.n_classes != dataset.n_classes:
+            raise ValueError("`n_classes` differs between dataset and model_config")
 
         def model_fn():
-            model = get_pt_model(clf_type, **model_args)
+            model = get_pt_model(clf_type, config=model_config)
             return model if transformer is None else (transformer, model)
 
         params = {
-            "optimiser": "adam",
-            "learning_rate": learning_rate,
-            **model_args,
-            **fit_params,
+            **PyTorchModelConfig.to_dictconfig(model_config),
+            **PyTorchTrainConfig.to_dictconfig(pt_config),
         }
         clf = model_fn
     else:
         raise ValueError(f"Invalid classifier type {clf_type}")
 
     if verbose > -1:
         print("== Dataset ==")
         print(dataset)
-        print("== Train/valid/test settings ==")
+        print("== Training/evaluation settings ==")
         print(f"Using {dataset.n_classes}-class classification.")
+        print(f"Using {n_jobs} parallel jobs.")
         print(f"Using classifier {clf}.")
         print(f"Using fit_params={fit_params}")
-        print(f"Training set: {train}")
-        print(f"Validation set: {valid}")
-        print(f"Test set: {test}")
+        if evaluation.train:
+            print(f"Training set: {evaluation.train} ({len(train_indices)})")
+            print(f"Validation set: {evaluation.valid} ({len(valid_indices)})")
+            print(f"Test set: {evaluation.test} ({len(test_indices)})")
+        elif cv_conf:
+            print(f"Using {cv_conf.kfold} k-fold CV.")
+            if cv_conf.part:
+                print(f"Using {cv_conf.part} as split partition.")
+            if evaluation.inner_kfold is not None:
+                if evaluation.inner_part:
+                    print(f"Using {evaluation.inner_part} as inner split partition.")
+                print(f"Using {evaluation.inner_kfold} as inner CV splitter.")
         if balanced:
             print("Using balanced sample weights.")
         if normalise == "online":
             print("Using 'online' normalisation.")
         elif normalise != "none":
             print(f"Normalising globally using {normalise} partition.")
+        if normalise != "none":
+            print(f"Using transformer {transformer}")
 
-    df = train_val_test(
-        clf,
-        dataset=dataset,
-        train_idx=train_indices,
-        valid_idx=valid_indices,
-        test_idx=test_indices,
-        label=label,
-        clf_lib=clf_lib,
-        sample_weight=sample_weight,
-        verbose=verbose,
-        fit_params=fit_params,
-    )
+    dfs = []
+    _preds = []
+    for rep in range(config.training.reps):
+        if verbose > -1:
+            print(f"Rep {rep}/{config.training.reps}")
+        if evaluation.train:
+            res = dataset_train_val_test(
+                clf,
+                dataset=dataset,
+                train_idx=train_indices,
+                valid_idx=valid_indices,
+                test_idx=test_indices,
+                label=config.training.label,
+                clf_lib=clf_lib,
+                sample_weight=sample_weight,
+                verbose=config.training.verbose,
+                fit_params=fit_params,
+            )
+        elif cv_conf:
+            res = dataset_cross_validation(
+                clf,
+                dataset,
+                clf_lib=clf_lib,
+                partition=cv_conf.part,
+                label=config.training.label,
+                cv=cv,
+                verbose=config.training.verbose,
+                n_jobs=n_jobs,
+                fit_params=fit_params,
+            )
+        else:
+            raise RuntimeError()
+        df = res.scores_df
+        if "params" not in df:
+            df["params"] = [json.dumps(params, default=str)] * len(df)
+        dfs.append(df)
+        if res.predictions is not None:
+            _preds.append(res.predictions)
+    if _preds:
+        preds = np.stack(_preds)
+    else:
+        preds = np.empty(0)
+    df = pd.concat(dfs, keys=pd.RangeIndex(config.training.reps), names=["rep"])
     df["clf"] = f"{clf_lib}/{clf_type}"
-    df["features"] = features
+    df["features"] = config.data.features
     df["corpus"] = dataset.corpus
-    df["params"] = json.dumps(params, default=str)
-    if results:
+    if config.results:
+        results = Path(config.results)
         results.parent.mkdir(parents=True, exist_ok=True)
         df.to_csv(results)
         print(f"Wrote CSV to {results}")
+        if preds.size > 0:
+            np.save(results.with_suffix(".preds.npy"), preds)
     else:
         print(df)
-    if verbose > -1:
-        print(df.mean(numeric_only=True).to_string())
+    print(df.mean(numeric_only=True).to_string())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ertk-2022.4.0/src/ertk/cli/classify.py` & `ertk-2023.6.0/src/ertk/cli/cli/classify.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/cli/dataset/annotation_stats.py` & `ertk-2023.6.0/src/ertk/cli/dataset/annotation_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,30 @@
 )
 @click.option("--plot", is_flag=True, help="Plot histogram/bar chart.")
 @click.option(
     "--files",
     type=click.Path(exists=True, dir_okay=False, path_type=Path),
     help="File with names to include for statistics.",
 )
-def main(input: Tuple[Path], plot: bool, files: Path):
+@click.option("--dtype")
+def main(input: Tuple[Path], plot: bool, files: Path, dtype: str):
     """Calculate statistics from annotations in INPUT(s). If multiple
     INPUTs are given, additional statistics for the other INPUTs are
     shown for each level of INPUT.
     """
 
     dfs: List[pd.DataFrame] = []
+    _dtype = {0: str}
+    if dtype == "str":
+        _dtype[1] = str
+
+    if len(input) == 0:
+        raise click.UsageError("No input files given.")
     for file in input:
-        df = pd.read_csv(file, header=0, converters={0: str}).set_index("name")
+        df = pd.read_csv(file, header=0, dtype=_dtype).set_index("name")
         if files:
             names = {Path(x).stem for x in get_audio_paths(files)}
             df = df[df.index.isin(names)]
         dfs.append(df)
         col = df[df.columns[0]]
         print(f"== Statistics for {col.name} ==")
         print(col.describe().to_string())
@@ -78,15 +85,15 @@
                         print(uniq.to_string())
                 else:
                     print(joined.groupby([refcol])[col].describe())
                     if plot:
                         table = joined.groupby([refcol])[col].hist(
                             bins=5, alpha=0.3, legend=True, ax=ax
                         )
-            else:
+            elif plot:
                 joined.plot(kind="scatter", x=refcol, y=col, ax=ax)
             print()
             if plot:
                 fig.tight_layout()
 
     if plot:
         plt.show()
```

### Comparing `ertk-2022.4.0/src/ertk/cli/dataset/combine.py` & `ertk-2023.6.0/src/ertk/cli/dataset/combine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,61 @@
+from itertools import chain
 from pathlib import Path
 from typing import List, Tuple
 
 import click
 
-from ertk.dataset import read_features, write_features
+from ertk.dataset import read_features_iterable, write_features
 
 
 @click.command()
 @click.argument(
     "input", type=click.Path(exists=True, dir_okay=False, path_type=Path), nargs=-1
 )
 @click.argument("output", type=Path)
 @click.option(
     "--prefix_corpus", is_flag=True, help="Prefix corpus names to instance names."
 )
-def main(input: Tuple[Path], output: Path, prefix_corpus: bool):
+@click.option("--corpus", default="combined", help="Output corpus name.")
+def main(input: Tuple[Path], output: Path, prefix_corpus: bool, corpus: str):
     """Combines multiple INPUT features and writes to OUTPUT."""
 
     if len(input) == 0:
         raise ValueError("No input files specified.")
 
     feature_names: List[str] = []
     features = []
     names = []
+    total_length = 0
     for filename in input:
-        data = read_features(filename)
+        data = read_features_iterable(filename)
+        total_length += len(data)
         if len(feature_names) == 0:
             feature_names = list(data.feature_names)
         elif len(data.feature_names) != len(feature_names):
             raise ValueError("Feature size of all datasets must match.")
-        features += list(data.features)
+        features.append(iter(data))
         if prefix_corpus:
+            if not data.corpus:
+                raise ValueError(
+                    "Some datasets do not have a corpus name, cannot prefix."
+                )
             names += [f"{data.corpus}_{x}" for x in data.names]
         else:
             names += data.names
-    if len(set(names)) != len(features):
+    if len(set(names)) != total_length:
         raise ValueError(
             "Some names are not unique, use --prefix_corpus to generate unique names."
         )
 
     output.parent.mkdir(parents=True, exist_ok=True)
     write_features(
         output,
-        features,
-        corpus="combined",
+        chain.from_iterable(features),
+        corpus=corpus,
         names=names,
         feature_names=feature_names,
     )
     print(f"Wrote combined features to {output}")
 
 
 if __name__ == "__main__":
```

### Comparing `ertk-2022.4.0/src/ertk/cli/dataset/convert.py` & `ertk-2023.6.0/src/ertk/cli/dataset/convert.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 from pathlib import Path
 
 import click
 
-from ertk.dataset import read_features
+from ertk.dataset import read_features_iterable, write_features
 
 
 @click.command()
 @click.argument("input", type=click.Path(exists=True, dir_okay=False, path_type=Path))
 @click.argument("output", type=Path)
 @click.option("--corpus", type=str, help="Corpus attribute to set, if required.")
-@click.option(
-    "--header/--noheader",
-    default=True,
-    help="Input CSV has header/Write output CSV header.",
-    show_default=True,
-)
-@click.option(
-    "--label/--nolabel",
-    default=False,
-    help="Input has label column.",
-    show_default=True,
-)
-def main(input: Path, output: Path, corpus: str, header: bool, label: bool):
+def main(input: Path, output: Path, corpus: str):
     """Convert INPUT dataset format to OUTPUT format. Note that no label
     information is written to OUTPUT.
     """
 
     if input.suffix == output.suffix:
         raise ValueError("Input format must be different to output.")
 
     print(f"Reading {input}")
-    data = read_features(input, header=header, label=label)
+    data = read_features_iterable(input)
     if corpus:
-        data._corpus = corpus
+        data.corpus = corpus
     output.parent.mkdir(parents=True, exist_ok=True)
-    data.write(output, header=header)
+    write_features(
+        output,
+        iter(data),
+        names=data.names,
+        corpus=data.corpus,
+        feature_names=data.feature_names,
+    )
     print(f"Wrote dataset to {output}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ertk-2022.4.0/src/ertk/cli/dataset/process.py` & `ertk-2023.6.0/src/ertk/cli/dataset/process.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 import logging
 import pprint
 from dataclasses import asdict
-from io import StringIO
+from functools import partial
 from pathlib import Path
 from typing import Tuple
 
 import click
-from joblib import delayed
 from omegaconf import OmegaConf
 from tqdm import tqdm
 
-from ertk.dataset import get_audio_paths, read_features, write_features
-from ertk.utils import TqdmParallel
+from ertk.dataset import read_features_iterable, write_features
+from ertk.utils import TqdmMultiprocessing
 
+logger = logging.getLogger(__name__)
 
-def list_processors(ctx, param, val):
+
+def list_processors(ctx: click.Context, param, val):
     from ertk.preprocessing import InstanceProcessor
 
     if not val or ctx.resilient_parsing:
         return
 
-    print(f"\nAvailable processors:\n{InstanceProcessor.valid_preprocessors()}\n")
+    print(f"\nAvailable processors:\n{InstanceProcessor.valid_processors()}\n")
     print(
         "Below are the default configurations for registered feature extractors. Items "
         "with '???' are required to be specified manually.\n"
     )
-    for key in InstanceProcessor.valid_preprocessors():
+    for key in sorted(InstanceProcessor.valid_processors()):
         print(f"[{key}]: ", end="")
         proc_cls = InstanceProcessor.get_processor_class(key)
         print(", ".join([b.__name__ for b in proc_cls.__bases__]))
         config_cls = proc_cls.get_config_type()
         for k, v in asdict(config_cls()).items():
             print(f"  {k} = {v}")
         print()
 
     ctx.exit()
 
 
 @click.command()
 @click.argument("input", type=click.Path(exists=True, path_type=Path))
 @click.argument("output", type=Path)
-@click.option("--features", required=True, help="Features to extract.")
+@click.option("--processor", "--features", required=True, help="Processor to apply.")
 @click.option(
     "--list_processors",
     is_flag=True,
     callback=list_processors,
     expose_value=False,
     is_eager=True,
-    help="Show options for registered feature extractors.",
+    help="Show options for registered processors.",
 )
 @click.option(
     "--config",
     type=click.Path(exists=True, path_type=Path),
     help="Extractor config file.",
 )
 @click.option("--corpus", default="", help="Corpus name to set.")
@@ -59,81 +60,66 @@
     "--batch_size",
     type=int,
     default=1,
     help="Batch size for processing. If batch_size is greater than 1, clips will be "
     "batched together.",
 )
 @click.option(
-    "--sample_rate", type=float, help="Resample to this rate for audio input."
+    "--sample_rate",
+    type=int,
+    default=16000,
+    help="Resample to this rate for audio input.",
 )
-@click.option("--n_jobs", type=int, default=-1, help="Number of parallel jobs to run.")
-@click.option("--verbose", is_flag=True)
+@click.option("--n_jobs", type=int, default=1, help="Number of parallel jobs to run.")
+@click.option("--verbose", type=int, default=0)
 @click.argument("restargs", nargs=-1)
 def main(
     input: Path,
     output: Path,
-    features: str,
+    processor: str,
     config: Path,
     corpus: str,
     batch_size: int,
-    sample_rate: float,
+    sample_rate: int,
     n_jobs: int,
-    verbose: bool,
+    verbose: int,
     restargs: Tuple[str],
 ):
-    """Process features or audio files in INPUT, write features to
-    OUTPUT.
-    """
+    """Process features or audio files in INPUT, write to OUTPUT."""
 
     from ertk.preprocessing import InstanceProcessor
 
-    if verbose:
-        logging.basicConfig(level=logging.INFO)
+    if verbose > 0:
+        logging.basicConfig(level=logging.DEBUG if verbose > 1 else logging.INFO)
 
-    extractor_cls = InstanceProcessor.get_processor_class(features)
+    extractor_cls = InstanceProcessor.get_processor_class(processor)
     config_cls = extractor_cls.get_config_type()
     if config:
         conf = OmegaConf.load(config)
     else:
         conf = extractor_cls.get_default_config()
     conf = OmegaConf.merge(conf, OmegaConf.from_dotlist(list(restargs)))
-    if verbose:
-        print("Using configuration:")
-        pprint.pprint(dict(conf))
+    logger.info("Using configuration:")
+    logger.info(pprint.pformat(dict(conf)))
     extractor = extractor_cls(config_cls.from_config(conf))
 
-    if input.suffix == ".txt":
-        # TODO: unify with read_features()
-        paths = get_audio_paths(input)
-        names = [Path(x).stem for x in paths]
-        if batch_size != 1:
-            feats = list(
-                tqdm(
-                    extractor.process_files(
-                        paths, batch_size=batch_size, sr=sample_rate
-                    ),
-                    total=len(paths),
-                    desc="Processing files",
-                )
-            )
-        else:
-            feats = TqdmParallel(len(paths), "Processing files", n_jobs=n_jobs)(
-                delayed(extractor.process_file)(x, sr=sample_rate) for x in paths
-            )
+    input_data = read_features_iterable(input, sample_rate=sample_rate)
+    corpus = corpus or input_data.corpus
+    names = input_data.names
+    if batch_size != 1:
+        feats = tqdm(
+            extractor.process_all(iter(input_data), batch_size, sr=sample_rate),
+            total=len(input_data),
+            desc="Processing files",
+            disable=None,
+        )
     else:
-        input_data = read_features(input)
-        corpus = corpus or input_data.corpus
-        names = input_data.names
-        if batch_size != 1:
-            feats = list(
-                tqdm(
-                    extractor.process_all(input_data.features, batch_size),
-                    total=len(input_data),
-                    desc="Processing files",
-                )
-            )
-        else:
-            feats = TqdmParallel(len(input_data), "Processing files", n_jobs=n_jobs)(
-                map(delayed(extractor.process_instance), input_data.features)
-            )
-    write_features(output, feats, names=names, corpus=corpus)
+        # TODO: Set back to joblib when
+        # https://github.com/joblib/joblib/pull/588 is merged
+        pool = TqdmMultiprocessing(len(input_data), "Processing files", n_jobs=n_jobs)
+        f = partial(extractor.process_instance, sr=sample_rate)
+        feats = pool.imap(f, input_data)
+    write_features(
+        output, feats, names=names, corpus=corpus, feature_names=extractor.feature_names
+    )
+    extractor.finish()
     print(f"Wrote features to {output}")
```

### Comparing `ertk-2022.4.0/src/ertk/cli/dataset/remove_instances.py` & `ertk-2023.6.0/src/ertk/cli/dataset/remove_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     idx, names = zip(*[(i, n) for i, n in enumerate(data.names) if n in keep_names])
 
     output = output or input
     write_features(
         output,
         corpus=data.corpus,
         names=list(names),
-        features=data.features[idx],
+        features=data.features[list(idx)],
         feature_names=data.feature_names,
     )
-    print(f"Wrote features to {input}")
+    print(f"Wrote features to {output}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ertk-2022.4.0/src/ertk/cli/train.py` & `ertk-2023.6.0/src/ertk/cli/cli/train.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/cli/util/create_cv_dirs.py` & `ertk-2023.6.0/src/ertk/cli/util/create_cv_dirs.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 
 @click.command()
 @click.argument("input", type=click.Path(exists=True, dir_okay=False, path_type=Path))
 @click.argument("output", type=Path)
 @click.option(
     "--label", "label_name", default="label", help="Categorical label to use."
 )
-def main(input: Path, output: Path, label_name: str):
-    """Create directory structure with speaker-independent
-    cross-validation folds. Each speaker has a directory which is
+@click.option("--partition", default="speaker", help="Partition to split on.")
+def main(input: Path, output: Path, label_name: str, partition: str):
+    """Create directory structure with group-independent
+    cross-validation folds. Each group has a directory which is
     patitioned by label.
     """
 
     dataset = Dataset(input)
     paths = get_audio_paths(dataset._subset_paths[dataset.subset])
-    speaker_paths: Dict[str, List[Path]] = defaultdict(list)
+    group_paths: Dict[str, List[Path]] = defaultdict(list)
     for path in paths:
-        speaker_paths[dataset.annotations["speaker"][path.stem]].append(path)
+        group_paths[dataset.annotations.loc[path.stem, partition]].append(path)
 
-    for i, speaker in enumerate(speaker_paths.keys()):
-        for path in speaker_paths[speaker]:
-            label = dataset.annotations[label_name][path.stem]
+    for i, group in enumerate(group_paths.keys()):
+        for path in group_paths[group]:
+            label = dataset.annotations.loc[path.stem, label_name]
             fold = f"fold_{i + 1:d}"
             newpath = output / fold / label / path.name
             newpath.parent.mkdir(parents=True, exist_ok=True)
             shutil.copy(str(path), str(newpath))
             print(newpath)
```

### Comparing `ertk-2022.4.0/src/ertk/cli/util/grid_to_conf.py` & `ertk-2023.6.0/src/ertk/cli/util/grid_to_conf.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/cli/util/names_to_filenames.py` & `ertk-2023.6.0/src/ertk/cli/util/names_to_filenames.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/cli/util/parallel_jobs.py` & `ertk-2023.6.0/src/ertk/cli/util/parallel_jobs.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,45 +11,59 @@
 from click_option_group import RequiredMutuallyExclusiveOptionGroup, optgroup
 
 
 @click.command()
 @click.argument(
     "input", type=click.Path(exists=True, dir_okay=False, path_type=Path), nargs=-1
 )
-@click.option("--failed", type=Path, help="Where to log failed commands.")
+@click.option(
+    "--failed", type=Path, help="Where to log failed commands.", required=True
+)
 @optgroup.group("Parallel method", cls=RequiredMutuallyExclusiveOptionGroup)
 @optgroup.option("--cpus", type=int, help="Number of CPU threads to use")
 @optgroup.option("--gpus", help="GPU IDs to run on.")
 def main(input: Tuple[Path], cpus: int, gpus: str, failed: Path):
-    """Runs all commands specified in the INPUT file(s), splitting the
+    """Run all commands specified in the INPUT file(s), splitting the
     work across multiple CPU threads or GPUs such that each command runs
     solely on whichever thread/GPU is next available.
 
-    Each GPU still has it's own thread to run processed using
+    Each GPU still has it's own thread to run processes using
     CUDA_VISIBLE_DEVICES. Each thread reads from a synchronous queue and
     runs the command in a shell.
     """
     if len(input) == 0:
         raise ValueError("No input files specified.")
 
     q: "Queue[str]" = Queue()
+    for file in input:
+        with open(file) as fid:
+            for line in filter(None, map(str.strip, fid)):
+                q.put(line)
+    n_commands = q.qsize()
+    print(f"Loaded {n_commands} commands")
+
     file_lock = Lock()
+    if not failed.exists():
+        failed.parent.mkdir(exist_ok=True, parents=True)
     fail_file = open(failed, "w")
+    n_failed = 0
 
     def worker(t_id: int = None, gpu: int = None):
         env = os.environ.copy()
         env.update({"PYTHONUNBUFFERED": "1"})
         if gpu is not None:
             env.update({"CUDA_VISIBLE_DEVICES": str(gpu)})
+        else:  # CPU
+            env.update({"OMP_NUM_THREADS": "1"})
         print_prefix = f"[T{t_id}]" if gpu is None else f"[GPU{gpu}]"
         while not q.empty():
             cmd = q.get()
             print(
                 datetime.now().isoformat(),
-                f"Executing command on thread {t_id or gpu}: {cmd}",
+                f"Executing command on {print_prefix}: {cmd}",
                 flush=True,
             )
             proc = subprocess.Popen(
                 cmd,
                 env=env,
                 shell=True,
                 text=True,
@@ -61,33 +75,33 @@
                 with proc.stdout:
                     for line in iter(proc.stdout.readline, ""):
                         sys.stdout.write(
                             f"{datetime.now().isoformat()} {print_prefix}:{line}"
                         )
                         sys.stdout.flush()
             if proc.wait() != 0:
+                nonlocal n_failed
                 with file_lock:
+                    n_failed += 1
                     fail_file.write(cmd + "\n")
                     fail_file.flush()
             q.task_done()
 
-    for file in input:
-        with open(file) as fid:
-            for line in list(filter(None, map(str.strip, fid))):
-                q.put(line)
-    print(f"Loaded {q.qsize()} commands")
-
     if cpus is not None:
         threads = [Thread(target=worker, kwargs={"t_id": i}) for i in range(cpus)]
     else:
         _gpus = list(map(int, gpus.split(",")))
         threads = [Thread(target=worker, kwargs={"gpu": i}) for i in _gpus]
     print(f"Starting threads at {datetime.now().isoformat()}")
+    start_time = datetime.now()
     for t in threads:
         t.start()
     for t in threads:
         t.join()
+    total_time = datetime.now() - start_time
     print(f"Finished at {datetime.now().isoformat()}")
+    print(f"Total time: {total_time} ({total_time.total_seconds()} s)")
+    print(f"{n_commands - n_failed} commands succeeded, {n_failed} failed")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ertk-2022.4.0/src/ertk/cli/util/split_chat.py` & `ertk-2023.6.0/src/ertk/cli/util/split_chat.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/cli/util/split_elan.py` & `ertk-2023.6.0/src/ertk/cli/util/split_elan.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/dataset/dataset.py` & `ertk-2023.6.0/src/ertk/dataset/dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+"""Dataset classes and related functions."""
+
 import copy
 import logging
 import os
 import warnings
+from dataclasses import dataclass, field
+from functools import partial, reduce
 from itertools import chain
 from pathlib import Path
 from typing import (
     Any,
     Collection,
     Dict,
     Iterable,
@@ -17,32 +21,121 @@
     Tuple,
     Type,
     Union,
     overload,
 )
 
 import numpy as np
-import yaml
+import pandas as pd
+from numpy.lib.arraysetops import setdiff1d
+from omegaconf import MISSING, OmegaConf
 from sklearn.base import TransformerMixin
 from sklearn.preprocessing import StandardScaler
 from typing_extensions import Literal
 
-from ertk.config import get_arg_mapping
+from ertk.config import ERTKConfig, get_arg_mapping
 from ertk.dataset.annotation import read_annotations
 from ertk.dataset.features import find_features_file, read_features
 from ertk.dataset.utils import get_audio_paths
 from ertk.transform import group_transform
-from ertk.utils import (
-    PathOrStr,
-    clip_arrays,
-    frame_arrays,
-    ordered_intersect,
-    pad_arrays,
-    transpose_time,
-)
+from ertk.utils import PathOrStr, clip_arrays, frame_arrays, pad_arrays, transpose_time
+
+__all__ = [
+    "Dataset",
+    "CombinedDataset",
+    "DatasetConfig",
+    "DataLoadConfig",
+    "DataSelector",
+    "SubsetInfo",
+    "MapGroups",
+    "RemoveGroups",
+    "CorpusInfo",
+    "load_multiple",
+    "load_datasets_config",
+]
+
+logger = logging.getLogger(__name__)
+
+
+@dataclass
+class MapGroups:
+    """Defined a mapping between categorical groups."""
+
+    map: Dict[str, str] = MISSING
+
+
+@dataclass
+class RemoveGroups:
+    """Defines a set of groups to keep or remove from a dataset."""
+
+    drop: List[str] = field(default_factory=list)
+    keep: List[str] = field(default_factory=list)
+
+
+@dataclass
+class SubsetInfo:
+    """Defines a subset of a dataset."""
+
+    clips: str = MISSING
+    description: str = ""
+
+
+@dataclass
+class DataSelector(ERTKConfig):
+    """Defines a selection of data to keep."""
+
+    subset: str = ""
+    groups: Dict[str, RemoveGroups] = field(default_factory=dict)
+
+
+@dataclass
+class CorpusInfo(ERTKConfig):
+    """Defines information about a dataset."""
+
+    name: str = MISSING
+    description: str = ""
+    annotations: List[str] = field(default_factory=list)
+    partitions: List[str] = field(default_factory=list)
+    ratings: List[str] = field(default_factory=list)
+    subsets: Dict[str, SubsetInfo] = field(default_factory=dict)
+    default_subset: str = "all"
+    features_dir: str = "features"
+
+
+@dataclass
+class DatasetConfig(ERTKConfig):
+    """Defines a dataset configuration."""
+
+    path: str = MISSING
+    features: Optional[str] = None
+    read_kwargs: Dict[str, Any] = field(default_factory=dict)
+    subset: str = "default"
+    map_groups: Dict[str, MapGroups] = field(default_factory=dict)
+    remove_groups: Dict[str, RemoveGroups] = field(default_factory=dict)
+    rename_annotations: Dict[str, str] = field(default_factory=dict)
+    select: Optional[DataSelector] = None
+    clip_seq: Optional[int] = None
+    pad_seq: Optional[int] = None
+
+
+@dataclass
+class DataLoadConfig(ERTKConfig):
+    """Defines a configuration for loading one or more datasets."""
+
+    datasets: Dict[str, DatasetConfig] = MISSING
+    features: Optional[str] = None
+    label: Optional[str] = None
+    map_groups: Dict[str, MapGroups] = field(default_factory=dict)
+    remove_groups: Dict[str, RemoveGroups] = field(default_factory=dict)
+    select: Optional[DataSelector] = None
+    clip_seq: Optional[int] = None
+    pad_seq: Optional[int] = None
+
+
+_AUDIO_PATH_KEY = "_audio_path"
 
 
 class Dataset:
     """Class representing a generic dataset, consisting of a set of
     features and optional partitions and annotations. Has various
     preprocessing methods.
 
@@ -61,171 +154,205 @@
     features: Pathlike or str, optional
         Path to features file, or unique name of features in corpus
         features directory.
     subset: str, optional
         The subset of instances to use.
     """
 
-    _annotations: Dict[str, Dict[str, Any]]
+    _annotations: pd.DataFrame
     _corpus: str = ""
     _feature_names: List[str]
-    _names: List[str]
+    _names: pd.Index
     _partitions: Set[str]
     _subset: str = ""
     _subsets: Dict[str, List[str]]
     _x: np.ndarray
+    _label_annot: str = ""
+    _ratings: Dict[str, pd.DataFrame]
+    _description: str = ""
 
     # "Private" vars
     _default_subset: str = ""
     _features: str = ""
-    _features_path: Path
-    _features_dir: Path
+    _features_path: Optional[Path] = None
+    _features_dir: Path = Path()
     _subset_paths: Dict[str, Path]
 
     def __init__(
         self,
         corpus_info: PathOrStr,
         features: Optional[PathOrStr] = None,
         subset: str = "default",
+        label: str = "label",
     ):
         self._init()
         self.init_corpus_info(corpus_info)
         self.use_subset(subset)
         if features is not None:
             self.update_features(features)
+        self._label_annot = label
 
     def _init(self) -> None:
-        self._annotations = {}
+        self._annotations = pd.DataFrame()
         self._feature_names = []
-        self._names = []
+        self._names = pd.Index([])
         self._partitions = set()
         self._subsets = {}
         self._subset_paths = {}
         self._x = np.empty((0, 0), dtype=np.float32)
-
-    @classmethod
-    def _copy(cls, inst: "Dataset"):
-        new_dataset = Dataset.__new__(cls)
-        new_dataset._copy_from_dataset(inst)
-        return new_dataset
+        self._ratings = {}
 
     def _copy_from_dataset(self, other: "Dataset") -> None:
-        self._annotations = copy.deepcopy(other._annotations)
+        self._annotations = other._annotations.copy()
         self._corpus = other._corpus
         self._default_subset = other._default_subset
         self._feature_names = other._feature_names.copy()
         self._features = other._features
         self._features_path = other._features_path
         self._features_dir = other._features_dir
         self._names = other._names.copy()
         self._partitions = other._partitions.copy()
         self._subset = other._subset
         self._subset_paths = other._subset_paths.copy()
         self._subsets = copy.deepcopy(other._subsets)
         self._x = other._x.copy()
+        self._label_annot = other._label_annot
+        self._ratings = copy.deepcopy(other._ratings)
+        self._description = other._description
         if len(self._x.shape) == 1:
             # Non-contiguous array, so copy each contiguous sub-array
             for i in range(len(self._x)):
                 self._x[i] = self._x[i].copy()
 
     def init_corpus_info(self, path: PathOrStr) -> None:
         """Initialise corpus metadata from YAML.
 
         Parameters
         ----------
         path: os.Pathlike or str
             The path to a YAML file containing corpus metadata.
         """
+        logger.debug(f"Initialising corpus from {path}")
+
         path = Path(path)
-        with open(path) as fid:
-            doc = yaml.safe_load(fid)
-        if not isinstance(doc, dict):
-            raise RuntimeError("Corpus info invalid.")
-        self._corpus = next(iter(doc))
-        corpus_info = doc[self.corpus]
-
-        self._features_dir = path.parent / corpus_info["features_dir"]
-        self._default_subset = corpus_info["subsets"]["default"]
-        for subset, subset_info in corpus_info["subsets"].items():
-            if subset == "default":
-                continue
-            clips_file = path.parent / f"{subset_info['clips']}.txt"
+        corpus_info = CorpusInfo.from_file(path)
+        self._corpus = corpus_info.name
+        self._description = corpus_info.description
+        self._features_dir = path.parent / corpus_info.features_dir
+        self._default_subset = corpus_info.default_subset
+        for subset, subset_info in corpus_info.subsets.items():
+            clips_file = path.parent / subset_info.clips
+            if clips_file.suffix == "":
+                clips_file = clips_file.with_suffix(".txt")
             self._subset_paths[subset] = clips_file
-            self.subsets[subset] = [x.stem for x in get_audio_paths(clips_file)]
+            name_to_path = {x.stem: str(x) for x in get_audio_paths(clips_file)}
+            self.subsets[subset] = list(name_to_path.keys())
+            if subset == "all":
+                self._names = pd.Index(self.subsets["all"])
+                # This will initialise the index of self.annotations
+                self._annotations.index = pd.Index(self.subsets["all"])
+                self.update_annotation(_AUDIO_PATH_KEY, list(name_to_path.values()))
+        for partition in corpus_info.partitions:
+            self.update_annotation(
+                partition, path.parent / f"{partition}.csv", dtype="category"
+            )
+        for annotation in corpus_info.annotations:
+            self.update_annotation(annotation, path.parent / f"{annotation}.csv")
+        for ratings in corpus_info.ratings:
+            self.update_ratings(ratings, path.parent / f"{ratings}.csv")
+        self.update_annotation(
+            "corpus", [self.corpus] * len(self._names), dtype="category"
+        )
 
-        if corpus_info["partitions"]:
-            for partition in corpus_info["partitions"]:
-                self.update_annotation(
-                    partition, path.parent / f"{partition}.csv", dtype=str
-                )
-        if corpus_info["annotations"]:
-            for annotation in corpus_info["annotations"]:
-                self.update_annotation(annotation, path.parent / f"{annotation}.csv")
+    def _verify_index(
+        self, df_or_series: Union[pd.DataFrame, pd.Series], msg: Optional[str] = None
+    ):
+        msg = msg or "Incomplete index"
+        try:
+            df_or_series.loc[self.names]
+        except KeyError as e:
+            raise RuntimeError(msg) from e
 
-    def _verify_annotations(self, annot_name: Optional[str] = None):
+    def _verify_annotations(self, msg: Optional[str] = "Incomplete annotation"):
         """Make sure there is a value for each instance for each annotation."""
+        self._verify_index(self.annotations, msg=msg)
 
-        def verify_annotation(annot_name: str):
-            missing = set(self.names) - self.annotations[annot_name].keys()
-            if len(missing) > 0:
-                raise RuntimeError(
-                    f"Incomplete annotation {annot_name}. These names are missing:"
-                    f"{missing}"
-                )
+    def _verify_ratings(self):
+        for name, df in self.ratings.items():
+            try:
+                self._verify_index(df, msg=f"Incomplete ratings for '{name}'")
+            except RuntimeError as e:
+                warnings.warn(str(e), RuntimeWarning)
 
-        to_verify = self.annotations.keys() if annot_name is None else {annot_name}
-        for annot_name in to_verify:
-            verify_annotation(annot_name)
+    def _reset_categorical(self):
+        """Make sure there are no extraneous categories in any
+        partition.
+        """
+        for part in self.partitions:
+            new = self._annotations.loc[self.names, part].cat.remove_unused_categories()
+            self._annotations[part] = new
 
-    def update_features(self, features: PathOrStr) -> None:
+    def update_features(self, features: PathOrStr, **read_kwargs) -> None:
         """Update the features matrix and feature names for this dataset.
 
         Parameters
         ----------
         features: os.PathLike or str
             Path to a set of features or unique name of features in
             corpus features dir.
+        **read_kwargs:
+            Other arguments to pass to `read_features()`.
         """
         if features == "raw_audio":
             self._features = "raw_audio"
             features = self._subset_paths[self.subset or "all"]
         else:
             features = Path(features)
-            if len(features.suffix) == 0:
-                features = find_features_file(self._features_dir.glob(f"{features}.*"))
+            if not features.exists():
+                try:
+                    features = find_features_file(
+                        self._features_dir.glob(f"{features}.*")
+                    )
+                except FileNotFoundError as e:
+                    raise FileNotFoundError(
+                        f"Cannot find features '{features}' in directory "
+                        f"'{self._features_dir}'"
+                    ) from e
             self._features = features.stem
         self._features_path = features
-        data = read_features(features)
+        data = read_features(features, **read_kwargs)
         self._feature_names = data.feature_names
-        if len(self.names) > 0:
-            names = set(self.names)
-            if len(names - set(data.names)) > 0:
-                raise ValueError(
-                    f"Features at {features} don't contain all instances for subset "
-                    f"{self.subset}."
-                )
-            self._x = data.features[[i for i, n in enumerate(data.names) if n in names]]
-            self._names = ordered_intersect(data.names, names)
-        else:
-            self._x = data.features
-            self._names = data.names
+
+        assert len(self.names) > 0
+        missing = self.names.difference(data.names)
+        if len(missing) > 0:
+            raise ValueError(
+                f"Features at {features} don't contain all instances, these are"
+                f"missing: {missing}"
+            )
+        # To avoid reordering the feature matrix, reorder self.names instead
+        data_names = pd.Index(data.names)
+        idx = data_names.isin(self.names)
+        self._x = data.features[idx]
+        self._names = data_names[idx]
 
     def use_subset(self, subset: str = "default") -> None:
         """Use a different subset of the instances.
 
         Parameters
         ----------
         subset: str
             Name of subset to use. Default is "default" which uses the
             default subset specified in corpus_info.
         """
         if subset == "default":
             subset = self._default_subset
         self._subset = subset
-        self._names = self.subsets[subset]
+        self._names = pd.Index(self.subsets[subset])
+        self._reset_categorical()
         self._verify_annotations()
 
     def get_idx_for_names(self, names: Collection[str]) -> np.ndarray:
         """Gets indices of instances corresponding to `names`.
 
         Parameters
         ----------
@@ -233,36 +360,35 @@
             The names to get indices for.
 
         Returns
         -------
         idx: np.ndarray
             The indices corresponding to `names`, in order.
         """
-        names = set(names)
-        return np.array([i for i, x in enumerate(self.names) if x in names])
+        return np.flatnonzero(self.names.isin(names))
 
     @overload
     def get_idx_for_split(
         self,
-        split: Union[str, Dict[str, Union[str, Collection[str]]]],
-        return_complement: Literal[False],
+        split: Union[str, Dict[str, Collection[str]], DataSelector],
+        return_complement: Literal[False] = False,
     ) -> np.ndarray:
         ...
 
     @overload
     def get_idx_for_split(
         self,
-        split: Union[str, Dict[str, Union[str, Collection[str]]]],
+        split: Union[str, Dict[str, Collection[str]], DataSelector],
         return_complement: Literal[True],
     ) -> Tuple[np.ndarray, np.ndarray]:
         ...
 
     def get_idx_for_split(
         self,
-        split: Union[str, Dict[str, Union[str, Collection[str]]]],
+        split: Union[str, Dict[str, Collection[str]], DataSelector],
         return_complement: bool = False,
     ) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
         """Gets indices of instances corresponding to the selection
         given by `split`.
 
         Parameters
         ----------
@@ -278,86 +404,165 @@
         -------
         idx: np.ndarray
             The corresponding indices.
         comp_idx: np.ndarray, optional
             If `return_complement` is True, this is also returned and
             contains the complement indices.
         """
+        subset_idx = None
         if isinstance(split, str):
             if ":" not in split and not Path(split).exists():  # is a subset
                 return self.get_idx_for_names(self.subsets[split])
             mapping = get_arg_mapping(split)
-        else:
+        elif isinstance(split, dict):
             mapping = split
-        indices: Set[int] = set()
+        else:
+            if OmegaConf.get_type(split) is None:
+                raise TypeError("Config is of incorrect type")
+            if split.subset:
+                subset_idx = self.get_idx_for_names(self.subsets[split.subset])
+            mapping = {
+                k: v.keep if v.keep else set(self.get_group_names(k)) - set(v.drop)
+                for k, v in split.groups.items()
+            }
+
+        indices_parts: Dict[str, np.ndarray] = {}
         for part_name in mapping:
-            group_names = self.get_group_names(part_name)
-            group_indices = self.get_group_indices(part_name)
             sel = mapping[part_name]
             sel = [sel] if isinstance(sel, str) else sel
+            group_names = self.get_group_names(part_name)
             sel_idx = [group_names.index(x) for x in sel]
-            indices.update(np.flatnonzero(np.isin(group_indices, sel_idx)))
-        comp_indices = set(range(len(self))) - indices
+            indices_parts[part_name] = np.flatnonzero(
+                np.isin(self.get_group_indices(part_name), sel_idx)
+            )
+
+        all_idx = np.arange(len(self))
+        indices = reduce(
+            partial(np.intersect1d, assume_unique=True), indices_parts.values(), all_idx
+        )
+        if subset_idx is not None:
+            indices = np.intersect1d(indices, subset_idx, assume_unique=True)
+        comp_indices = setdiff1d(all_idx, indices, assume_unique=True)
         if return_complement:
-            return np.array(sorted(indices)), np.array(sorted(comp_indices))
+            return np.sort(indices), np.sort(comp_indices)
         else:
-            return np.array(sorted(indices))
+            return np.sort(indices)
 
     def update_annotation(
         self,
         annot_name: str,
-        annotations: Union[PathOrStr, Mapping[str, Any], Sequence[Any]],
-        dtype: Optional[Type] = None,
+        annotations: Union[PathOrStr, Mapping[str, Any], Sequence[Any], pd.Series],
+        dtype: Optional[Union[Type, Literal["category"]]] = None,
     ) -> None:
         """Add or update an annotation.
 
         Parameters
         ----------
         annot_name: str
             The name of the annotation.
-        annotations: PathLike, str, mapping or sequence
+        annotations: PathLike, str, mapping, DataFrame, Series or sequence
             Annotations to add, similar to update_partition(). If
             PathLike or str, annotations are read from a CSV. If a dict,
             should be of the form {instance: annotation}. If a list,
             should have an annotation for each instance.
         dtype: type, optional
-            The type of annotations for reading from CSV file.
+            The type of annotations for reading from CSV file. If the
+            literal "category" is given the annotations are converted to
+            the Pandas categorical dtype.
         """
         if isinstance(annotations, (os.PathLike, str)):
-            annot_dict = read_annotations(annotations, dtype=dtype)
+            series = read_annotations(annotations, dtype=dtype)
         elif isinstance(annotations, Mapping):
-            annot_dict = dict(annotations)
+            series = pd.DataFrame.from_dict(annotations, orient="index")
+            series = series.squeeze("columns")
+        elif isinstance(annotations, pd.Series):
+            series = annotations
         else:
-            annot_dict = {
-                k: v for k, v in zip(self.names, annotations) if v is not None
-            }
+            series = pd.Series(annotations, index=self.names)
 
-        self._annotations[annot_name] = annot_dict
+        logger.debug(f"Updating annotation {annot_name} ({len(series)} values).")
+
+        try:
+            self._verify_index(series)
+        except RuntimeError as e:
+            raise RuntimeError(f"Annotation {annot_name} is incomplete") from e
+        self._annotations[annot_name] = series
         if (
-            dtype is not None
-            and issubclass(dtype, str)
-            or isinstance(next(iter(annot_dict.values())), str)
+            dtype == "category"
+            or (dtype is not None and issubclass(dtype, str))
+            or series.dtype == object
+            or series.dtype == pd.CategoricalDtype
         ):
             self.partitions.add(annot_name)
-        self._verify_annotations(annot_name)
+            self._annotations[annot_name] = self._annotations[annot_name].astype(
+                "category"
+            )
+
+    def update_ratings(
+        self,
+        rating_set: str,
+        ratings: Union[PathOrStr, Mapping[str, Mapping[str, Any]], pd.Series],
+    ) -> None:
+        """Update a set of ratings.
+
+        Parameters
+        ----------
+        rating_set: str
+            The name for this set of ratings.
+        ratings: PathLike, str, mapping, DataFrame, Series
+            The ratings to add. Must have a joint index where
+        """
+        if isinstance(ratings, (os.PathLike, str)):
+            df = pd.read_csv(ratings, converters={0: str, 1: str})
+            df = df.set_index(list(df.columns[0:2]))
+        elif isinstance(ratings, pd.DataFrame):
+            df = ratings
+        elif isinstance(ratings, pd.Series):
+            df = ratings.to_frame()
+
+        self.ratings[rating_set] = df
+        self._verify_ratings()
+
+    def remove_ratings(self, rating_set: str) -> None:
+        """Delete a set of ratings for this dataset.
+
+        Parameters
+        ----------
+        rating_set: str
+            The name of a set of ratings.
+        """
+        del self.ratings[rating_set]
 
     def map_groups(self, part_name: str, mapping: Mapping[str, str]) -> None:
         """Map group names in a partition.
 
         Parameters
         ----------
         part_name: str
             Name of partition.
         mapping: dict
             Group name mapping.
         """
-        groups = self.get_annotations(part_name)
-        self.update_annotation(
-            part_name, [mapping.get(x, x) for x in groups], dtype=str
-        )
+        logger.debug(f"Mapping {part_name}: {mapping}")
+
+        annot = self._annotations[part_name]
+        try:
+            new = annot.cat.rename_categories(mapping)
+        except ValueError:
+            # Not a 1-1 mapping
+            _map = {x: x for x in annot.cat.categories}
+            _map.update(mapping)
+            new = annot.map(_map).astype("category")
+        new = new.cat.reorder_categories(new.cat.categories.sort_values())
+        self._annotations[part_name] = new
+
+        # groups = self.annotations[part_name]
+        # self.update_annotation(
+        #     part_name, groups.map(lambda x: mapping.get(x, x)), dtype=str
+        # )
 
     def remove_groups(
         self,
         part_name: str,
         *,
         drop: Collection[str] = None,
         keep: Collection[str] = None,
@@ -365,94 +570,171 @@
         """Remove instances corresponding to groups from the given
         partition.
 
         Parameters
         ----------
         part_name: str
             The partition name.
-        groups: collection of str
+        drop: collection of str
             The groups to remove in given partition.
+        keep: collection of str
+            The groups to keep in given partition.
         """
         drop = set([] if drop is None else drop)
         keep = set([] if keep is None else keep)
 
         if (len(drop) == 0) == (len(keep) == 0):
             raise ValueError("Exactly one of drop and keep should be non-empty.")
 
+        all_groups = set(self.get_group_names(part_name))
+        unknown = drop.union(keep) - all_groups
+        if len(unknown) > 0:
+            raise ValueError(f"Cannot drop or keep {unknown} in partition {part_name}.")
+
         if len(keep) == 0:
-            keep = set(self.get_group_names(part_name)) - drop
+            keep = all_groups - drop
+
+        if len(drop) == 0:
+            drop = all_groups - keep
+
+        logger.debug(
+            f"Dropping {len(drop)} and keeping {len(keep)} groups from "
+            f"partition {part_name}."
+        )
+
+        new = self._annotations[part_name].cat.remove_categories(list(drop))
+        self._annotations[part_name] = new
 
-        annotation = self.annotations[part_name]
-        self.remove_instances(keep=[x for x in self.names if annotation[x] in keep])
+        keep_names = new.index[new.isin(keep)]
+        self.remove_instances(keep=keep_names.intersection(self.names))
+
+    def map_and_select(
+        self,
+        map: Mapping[str, Mapping[str, str]],
+        select: Mapping[str, Union[str, Collection[str]]],
+        remove: Mapping[str, Union[str, Collection[str]]],
+    ) -> None:
+        """Convenience function for mapping one or more partitions and
+        then selecting one or more groups.
+
+        Parameters
+        ----------
+        map: mapping
+            The groups mapping. May have one or more partitions.
+        select: mapping
+            Mapping from partitions to groups to select.
+        """
+        for part in map:
+            if part not in self.partitions:
+                warnings.warn(
+                    f"Partition {part} cannot be mapped as it is not in the dataset."
+                )
+                continue
+            self.map_groups(part, map[part])
+        for part in set(select).union(remove):
+            if part not in self.partitions:
+                warnings.warn(
+                    f"Partition {part} cannot be selected/dropped as it is not in the "
+                    "dataset."
+                )
+                continue
+            keep = select.get(part, [])
+            drop = remove.get(part, [])
+            if isinstance(keep, str):
+                keep = [keep]
+            if isinstance(drop, str):
+                drop = [drop]
+            self.remove_groups(part, keep=keep, drop=drop)
 
     def rename_annotation(self, old_name: str, new_name: str) -> None:
         """Renames an annotation. This is useful for example if you want
         to select a different labelling to use. If an annotation already
         exists with the given new_name, then it is replaced
         destructively.
 
         Parameters
         ----------
         old_name: str
             The name of the annotation to rename.
         new_name: str
             The new name of the annotation.
         """
-        self.annotations[new_name] = self.annotations[old_name]
-        del self.annotations[old_name]
+        self._annotations.rename(columns={old_name: new_name}, inplace=True)
         if old_name in self.partitions:
             self.partitions.add(new_name)
             self.partitions.remove(old_name)
 
     def remove_annotation(self, annot_name: str) -> None:
         """Removes a set of annotations from the dataset. This does not
         remove any instances.
 
         Parameters
         ----------
         annot_name: str
             Annotation name.
         """
-        del self.annotations[annot_name]
+        del self._annotations[annot_name]
         # Use difference_update in case annot_name is not already a partition
         self.partitions.difference_update({annot_name})
 
-    def get_annotations(self, annot_name: str) -> List[Any]:
+    def get_annotations(self, annot_name: str) -> np.ndarray:
         """Get a list of annotations, one for each instance currently in
         the dataset.
 
         Parameters
         ----------
         annot_name: str
             Annotation name.
 
         Returns
         -------
-        A list of values, one for each instance in the datset, in the
-        same order they appear in names and x.
+        A pd.Series of values, one for each instance in the datset, in
+        the same order they appear in names and x.
+        """
+        return self.annotations.loc[self.names, annot_name].to_numpy()
+
+    def get_audio_paths(self) -> np.ndarray:
+        return self.get_annotations(_AUDIO_PATH_KEY)
+
+    def get_ratings(self, name: str, rating_set: str = "ratings") -> pd.Series:
+        """Get per-annotator ratings of a specified column, for this
+        dataset.
+
+        Parameters
+        ----------
+        name: str
+            The name of the rating column to get.
+        rating_set: str
+            The name of the rating set to get.
+
+        Returns
+        -------
+        pd.Series
+            Pandas Series with (name, rater) multiindex.
         """
-        return [self.annotations[annot_name][x] for x in self.names]
+        return self.ratings[rating_set].loc[self.names, name]
 
     def annotation_type(self, annot_name: str) -> Type:
-        return type(next(iter(self.annotations[annot_name].values())))
+        return self.annotations[annot_name].dtype
 
     def get_group_indices(self, annot_name: str) -> np.ndarray:
         """Gets the group indices (i.e. indices into the groups array)
         for a given partition.
 
         Parameters
         ----------
         annot_name: str
             The partition name.
 
         Returns
         -------
         A NumPy array of group indices for each instance in the dataset.
         """
-        _, idx = np.unique(self.get_annotations(annot_name), return_inverse=True)
+        # _, idx = np.unique(self.get_annotations(annot_name), return_inverse=True)
+        idx = self.annotations.loc[self.names, annot_name].cat.codes.to_numpy(np.int64)
         return idx
 
     def get_group_counts(self, annot_name: str) -> np.ndarray:
         """Get group counts for a partition.
 
         Parameters
         ----------
@@ -460,40 +742,30 @@
             The partition name.
 
         Returns
         -------
         A NumPy array of counts for the corresponding group in this
         partition.
         """
-        _, counts = np.unique(self.get_annotations(annot_name), return_counts=True)
+        counts = (
+            self.annotations.loc[self.names, annot_name]
+            .value_counts(sort=False)
+            .to_numpy()
+        )
         return counts
 
     def get_group_names(self, annot_name: str) -> List[str]:
         """Get the names of groups in a partition.
 
         Parameters
         ----------
         annot_name: str
             Annotation name.
         """
-        return list(np.unique(self.get_annotations(annot_name)))
-
-    def update_speakers(
-        self, speakers: Union[PathOrStr, Mapping[str, str], Sequence[str]]
-    ):
-        """Update the speakers for this dataset.
-
-        Parameters
-        ----------
-        speakers: Path, str, dict or list
-            If Path or str, read speaker info from CSV at given path. If
-            dict, use speaker dict directly. If list, each speakers[i]
-            is the corresponding speaker for instance i.
-        """
-        self.update_annotation("speaker", speakers, dtype=str)
+        return list(self.annotations.loc[self.names, annot_name].cat.categories)
 
     def remove_instances(
         self, *, drop: Collection[str] = None, keep: Collection[str] = None
     ):
         """Remove instances from dataset. Recalculate annotations,
         partitions, etc.
 
@@ -508,32 +780,31 @@
         drop = set([] if drop is None else drop)
         keep = set([] if keep is None else keep)
 
         if (len(drop) == 0) == (len(keep) == 0):
             raise ValueError("Exactly one of drop and keep should be given.")
 
         if len(keep) == 0:
-            keep = set(self.names) - drop
+            keep = self.names.difference(drop, sort=False)
 
+        # Need idx for self.x, instead of ordered_intersect()
         idx = self.get_idx_for_names(keep)
-        self._names = [self.names[i] for i in idx]
+        self._names = self.names[idx]
         if len(self._x) > 0:  # To avoid NumPy DeprecationWarning
             self._x = self.x[idx]
-        try:
-            self._verify_annotations()
-        except RuntimeError as e:
-            raise RuntimeError(
-                "Incomplete annotations after removing instances."
-            ) from e
+        self._reset_categorical()
+        self._verify_annotations(msg="Incomplete annotations after removing instances.")
 
     def clone(self):
         return self.copy()
 
     def copy(self):
-        return self._copy(self)
+        new_dataset = type(self).__new__(type(self))
+        new_dataset._copy_from_dataset(self)
+        return new_dataset
 
     def normalise(
         self, partition: str, normaliser: TransformerMixin = StandardScaler()
     ):
         """Transforms the data matrix of this dataset in-place using
         some (offline) normalisation method.
 
@@ -554,48 +825,53 @@
             groups = self.get_group_indices(partition)
         group_transform(self.x, groups, normaliser, inplace=True)
 
     def pad_arrays(self, pad: int = 32):
         """Pads each array to the nearest multiple of `pad` greater than
         the array size. Assumes axis 0 of x is time.
         """
-        logging.info(f"Padding array lengths to nearest multiple of {pad}.")
+        logger.info(f"Padding array lengths to nearest multiple of {pad}.")
         self._x = pad_arrays(self.x, pad=pad)
 
     def clip_arrays(self, length: int):
         """Clips each array to the specified maximum length."""
-        logging.info(f"Clipping arrays to max length {length}.")
+        logger.info(f"Clipping arrays to max length {length}.")
         self._x = clip_arrays(self.x, length=length, copy=False)
 
     def frame_arrays(
         self,
         frame_size: int,
         frame_shift: int,
         max_frames: Optional[int] = None,
     ):
         """Create a sequence of frames from the raw signal."""
-        logging.info(f"Framing arrays with size {frame_size} and shift {frame_shift}.")
+        logger.info(f"Framing arrays with size {frame_size} and shift {frame_shift}.")
         self._x = frame_arrays(
             self._x,
             frame_size=frame_size,
             frame_shift=frame_shift,
             max_frames=max_frames,
         )
 
     def transpose_time(self):
         """Transpose the time and feature axis of each instance."""
-        logging.info("Transposing time and feature axis of data.")
+        logger.info("Transposing time and feature axis of data.")
         self._x = transpose_time(self._x)
 
     @property
     def corpus(self) -> str:
         """The corpus this dataset represents."""
         return self._corpus
 
     @property
+    def description(self) -> str:
+        """The descriptive name of this corpus"""
+        return self._description
+
+    @property
     def n_instances(self) -> int:
         """Number of instances in this dataset."""
         return len(self.names)
 
     @property
     def feature_names(self) -> List[str]:
         """List of feature names."""
@@ -620,33 +896,38 @@
     def speaker_indices(self) -> np.ndarray:
         """Indices into speakers array of corresponding speaker for each
         instance.
         """
         return self.get_group_indices("speaker")
 
     @property
-    def speakers(self) -> List[str]:
+    def speakers(self) -> np.ndarray:
         return self.get_annotations("speaker")
 
     @property
     def n_speakers(self) -> int:
         return len(self.speaker_names)
 
     @property
     def partitions(self) -> Set[str]:
         """Partitions in this dataset."""
         return self._partitions
 
     @property
-    def annotations(self) -> Dict[str, Dict[str, Any]]:
-        """Each annotation is a mapping from instance name to value."""
-        return self._annotations
+    def annotations(self) -> pd.DataFrame:
+        """Full annotation matrix for dataset."""
+        return self._annotations.loc[self.names]
+
+    @property
+    def ratings(self) -> Dict[str, pd.DataFrame]:
+        """Full ratings for dataset."""
+        return self._ratings
 
     @property
-    def names(self) -> List[str]:
+    def names(self) -> pd.Index:
         """List of instance names."""
         return self._names
 
     @property
     def subset(self) -> str:
         """Name of clip subset used."""
         return self._subset
@@ -660,62 +941,17 @@
     def x(self) -> np.ndarray:
         """The data matrix."""
         return self._x
 
     def __len__(self) -> int:
         return self.n_instances
 
-    def __str__(self):
-        s = f"Corpus: {self.corpus}\n"
-        for part in sorted(self.partitions):
-            group_names = self.get_group_names(part)
-            s += f"partition '{part}' ({len(group_names)} groups)\n"
-            if len(group_names) <= 20:
-                s += f"\t{dict(zip(group_names, self.get_group_counts(part)))}\n"
-        for annot in sorted(self.annotations):
-            if annot in self.partitions:
-                continue
-            s += f"annotation '{annot}'\n"
-            annotations = np.array(self.get_annotations(annot))
-            s += f"\tmin: {annotations.min():.3f}, max: {annotations.max():.3f}, "
-            s += f"mean: {annotations.mean():.3f}\n"
-        s += f"{self.n_instances} instances\n"
-        s += f"subset: {self.subset}\n"
-        s += f"using {self._features} ({self.n_features} features)\n"
-        if self.x.dtype == object or len(self.x.shape) == 3:
-            lengths = [len(x) for x in self.x]
-            s += "Sequences:\n"
-            s += f"min length: {np.min(lengths)}\n"
-            s += f"mean length: {np.mean(lengths)}\n"
-            s += f"max length: {np.max(lengths)}\n"
-        return s
-
-
-class LabelledDataset(Dataset):
-    """Class representing a dataset containing discrete labels for each
-    instance.
-    """
-
-    _label_annot: str
-
-    def __init__(
-        self,
-        corpus_info: PathOrStr,
-        features: Optional[PathOrStr] = None,
-        subset: str = "default",
-        label: str = "label",
+    def update_labels(
+        self, labels: Union[PathOrStr, Mapping[str, str], Sequence[str], pd.Series]
     ):
-        super().__init__(corpus_info, features, subset)
-        self._label_annot = label
-
-    def _copy_from_dataset(self, other: "Dataset") -> None:
-        super()._copy_from_dataset(other)
-        self._label_annot = getattr(other, "_label_annot", "label")
-
-    def update_labels(self, labels: Union[PathOrStr, Mapping[str, str], Sequence[str]]):
         self.update_annotation(self.label_annot, labels, dtype=str)
 
     def map_classes(self, mapping: Mapping[str, str]):
         """Modifies classses based on the mapping in map. Keys not
         corresponding to classes are ignored. The new classes will be
         sorted lexicographically.
         """
@@ -739,168 +975,265 @@
 
     @property
     def class_counts(self) -> np.ndarray:
         """Number of instances for each class."""
         return self.get_group_counts(self.label_annot)
 
     @property
-    def labels(self) -> List[str]:
+    def labels(self) -> np.ndarray:
         """List of labels for instances."""
         return self.get_annotations(self.label_annot)
 
     @property
     def label_annot(self) -> str:
         """The annotation used as target label."""
         return self._label_annot
 
     @label_annot.setter
     def label_annot(self, val: str) -> None:
-        if val not in self.annotations:
-            raise ValueError(f"'{val}' not in annotations.")
         self._label_annot = val
 
     @property
     def y(self) -> np.ndarray:
         """The class label array; one label per instance."""
         if self.label_annot in self.partitions:
             return self.get_group_indices(self.label_annot)
         else:
-            return np.ndarray(self.get_annotations(self.label_annot))
+            return self.get_annotations(self.label_annot)
+
+    def __str__(self):
+        s = f"Corpus: {self.corpus}\n"
+        s += f"Description: {self.description}\n"
+        for part in sorted(self.partitions):
+            if part == _AUDIO_PATH_KEY:
+                continue
+            group_names = self.get_group_names(part)
+            s += f"partition '{part}' ({len(group_names)} groups)"
+            n_invalid = self.annotations.loc[self.names, part].isna().sum()
+            if n_invalid > 0:
+                n_valid = len(self) - n_invalid
+                s += f" (incomplete [{n_valid} valid])"
+            s += "\n"
+            if len(group_names) <= 20:
+                s += f"\t{dict(zip(group_names, self.get_group_counts(part)))}\n"
+        for annot in sorted(self.annotations):
+            if annot in self.partitions:
+                continue
+            s += f"annotation '{annot}'\n"
+            annotations = self.get_annotations(annot)
+            s += f"\tmin: {annotations.min():.3f}, max: {annotations.max():.3f}, "
+            s += f"mean: {annotations.mean():.3f}\n"
+        s += f"{self.n_instances} instances\n"
+        s += "Subsets:\n" if self.subsets else ""
+        for subset, names in self.subsets.items():
+            s += "\t*" if subset == self.subset else "\t "
+            s += f"{subset}: {len(names)} instances\n"
+        s += f"using {self._features} ({self.n_features} features)\n"
+        if self.x.dtype == object or len(self.x.shape) == 3:
+            lengths = [len(x) for x in self.x]
+            s += "Sequences:\n"
+            s += f"min length: {np.min(lengths)}\n"
+            s += f"mean length: {np.mean(lengths)}\n"
+            s += f"max length: {np.max(lengths)}\n"
+        return s
 
 
-class CombinedDataset(LabelledDataset):
+class CombinedDataset(Dataset):
     """A dataset that joins one or more individual datasets together and
     merges annotations.
     """
 
-    def __init__(self, *datasets: LabelledDataset):
+    def __init__(self, *datasets: Dataset):
         if len(datasets) == 0:
             raise ValueError("No datasets provided.")
         if len(datasets) == 1:
             self._copy_from_dataset(datasets[0])
             return
 
         self._init()
 
-        logging.info("Combining " + ", ".join(d.corpus for d in datasets))
+        combined_str = ", ".join(d.corpus for d in datasets)
+        logger.info(f"Combining {combined_str}")
         self._corpus = "combined"
-        self._names = [f"{d.corpus}_{n}" for d in datasets for n in d.names]
+        self._description = f"Combined datasets ({combined_str})"
+        self._names = pd.Index([f"{d.corpus}_{n}" for d in datasets for n in d.names])
         self._feature_names = datasets[0].feature_names
         self._features = datasets[0]._features
         self._x = np.concatenate([d.x for d in datasets])
-
         self.update_annotation(
-            "corpus", [d.corpus for d in datasets for _ in d.names], dtype=str
+            "corpus", [d.corpus for d in datasets for _ in d.names], dtype="category"
         )
 
         all_speakers = {}
         for d in datasets:
-            if "speaker" not in d.annotations:
+            if "speaker" not in d.annotations.columns:
                 all_speakers.update(
                     {f"{d.corpus}_{k}": f"{d.corpus}_unknown" for k in d.names}
                 )
             else:
                 speakers = d.annotations["speaker"]
                 all_speakers.update(
                     {f"{d.corpus}_{k}": f"{d.corpus}_{v}" for k, v in speakers.items()}
                 )
-        self.update_speakers(all_speakers)
+        self.update_annotation("speaker", all_speakers)
 
         # TODO: handle case when only some datasets have a given annotation?
-        all_annotations = set(chain(*(d.annotations for d in datasets)))
-        all_annotations -= {"speaker"}  # assumed to be per-dataset
+        all_annotations = set(chain(*(d.annotations.columns for d in datasets)))
+        all_annotations -= {"speaker", "corpus"}  # assumed to be per-dataset
         common_annotations = {
-            x for x in all_annotations if all(x in d.annotations for d in datasets)
+            x
+            for x in all_annotations
+            if all(x in d.annotations.columns for d in datasets)
         }
-        logging.info(f"All annotations: {all_annotations}")
-        logging.info(f"Common annotations: {common_annotations}")
+        logger.info(f"All annotations: {all_annotations}")
+        logger.info(f"Common annotations: {common_annotations}")
         for annot_name in common_annotations:
             combined_annot = {}
             for dataset in datasets:
                 annotations = dataset.annotations[annot_name]
                 combined_annot.update(
                     {f"{dataset.corpus}_{k}": v for k, v in annotations.items()}
                 )
             self.update_annotation(annot_name, combined_annot)
 
-        # Not common categorical annotations
+        # Non-common categorical annotations
         for annot_name in all_annotations - common_annotations:
             if not any(annot_name in d.partitions for d in datasets):
                 continue
             combined_annot = {}
             for d in datasets:
                 if annot_name not in d.annotations:
-                    combined_annot.update(
-                        {f"{d.corpus}_{k}": "unknown" for k in d.names}
-                    )
+                    combined_annot.update({f"{d.corpus}_{k}": None for k in d.names})
                 else:
                     annotations = d.annotations[annot_name]
                     combined_annot.update(
                         {f"{d.corpus}_{k}": v for k, v in annotations.items()}
                     )
             self.update_annotation(annot_name, combined_annot)
 
+        if any(d.label_annot == "" for d in datasets):
+            return
+
         if any(d.label_annot != datasets[0].label_annot for d in datasets):
             # Try and unify label annotations with different names
             warnings.warn(
                 "label annotation differs between some datasets, attempting to unify."
             )
-            self._label_annot = "_combined_labels"
             combined_labels = {}
             for d in datasets:
                 for name in d.names:
                     label = d.annotations[d.label_annot][name]
                     combined_labels[f"{d.corpus}_{name}"] = label
-            self.update_labels(combined_labels)
+            self.update_annotation("_combined_labels", combined_labels)
+            self.label_annot = "_combined_labels"
         else:
-            self._label_annot = next(d.label_annot for d in datasets)
+            self.label_annot = next(d.label_annot for d in datasets)
 
     @property
-    def corpus_names(self) -> Sequence[str]:
+    def corpus_names(self) -> List[str]:
         """List of corpora in this CombinedDataset."""
         return self.get_group_names("corpus")
 
     @property
     def corpus_indices(self) -> np.ndarray:
         """Indices into corpora list of corresponding corpus for each
         instance.
         """
         return self.get_group_indices("corpus")
 
 
 def load_multiple(
     corpus_files: Iterable[PathOrStr],
-    features: str,
+    features: Optional[str] = None,
     subsets: Union[str, Mapping[str, str]] = "default",
     label: Union[str, Mapping[str, str]] = "label",
+    **read_kwargs,
 ) -> CombinedDataset:
     """Load one or more datasets with the given features.
 
     Parameters
     ----------
     corpus_files: iterable
         The corpus description YAML files to load.
     features: str
         A common set of features to load. This will be found in the
         features directory corresponding to each corpus.
     subsets: str or dict
         A subset name common to all datasets (e.g. "all", "default") or
         a mapping from dataset name to subset name.
+    **read_kwargs:
+        Other args to pass to feature loading.
     """
     corpus_files = list(corpus_files)
     if len(corpus_files) == 0:
         raise RuntimeError("No corpus metadata files given.")
     datasets = []
     for file in corpus_files:
-        logging.info(f"Loading {file}")
-        dataset = LabelledDataset(file, subset="all")
+        logger.info(f"Loading {file}")
+        dataset = Dataset(file, subset="all")
         if isinstance(label, str):
-            dataset.label_annot = label
+            setattr(dataset, "label_annot", label)
         else:
-            dataset.label_annot = label.get(dataset.corpus, "label")
+            setattr(dataset, "label_annot", label.get(dataset.corpus, "label"))
         if isinstance(subsets, str):
             dataset.use_subset(subsets)
         else:
             dataset.use_subset(subsets.get(dataset.corpus, "default"))
-        dataset.update_features(features)
+        if features is not None:
+            dataset.update_features(features, **read_kwargs)
         datasets.append(dataset)
     return CombinedDataset(*datasets)
+
+
+def load_datasets_config(config: Union[PathOrStr, DataLoadConfig]) -> Dataset:
+    """Load one or more datasets from a DataLoadConfig.
+
+    Parameters
+    ----------
+    config: DataLoadConfig
+        The data loading config.
+
+    Returns
+    -------
+    Dataset
+        A dataset that combines one or more datasets according to the
+        given config.
+    """
+    if isinstance(config, (str, os.PathLike)):
+        config = DataLoadConfig.from_file(config)
+    datasets: List[Dataset] = []
+    for corpus, dataset_conf in config.datasets.items():
+        logger.info(f"Loading {dataset_conf.path}")
+        dataset = Dataset(dataset_conf.path, subset=dataset_conf.subset)
+        dataset._corpus = corpus
+        for part, mapping in dataset_conf.map_groups.items():
+            dataset.map_groups(part, mapping.map)
+        for part, remove in dataset_conf.remove_groups.items():
+            dataset.remove_groups(part, drop=remove.drop, keep=remove.keep)
+        for a1, a2 in dataset_conf.rename_annotations.items():
+            # TODO: check for collisions
+            dataset.rename_annotation(a1, a2)
+        if dataset_conf.features:
+            dataset.update_features(dataset_conf.features, **dataset_conf.read_kwargs)
+        elif config.features:
+            dataset.update_features(config.features, **dataset_conf.read_kwargs)
+        if dataset_conf.clip_seq:
+            dataset.clip_arrays(dataset_conf.clip_seq)
+        if dataset_conf.pad_seq:
+            dataset.pad_arrays(dataset_conf.pad_seq)
+        datasets.append(dataset)
+    if len(config.datasets) > 1:
+        dataset = CombinedDataset(*datasets)
+        del datasets
+    else:
+        dataset = datasets[0]
+    for part, mapping in config.map_groups.items():
+        dataset.map_groups(part, mapping.map)
+    for part, remove in config.remove_groups.items():
+        dataset.remove_groups(part, drop=remove.drop, keep=remove.keep)
+    if config.clip_seq:
+        dataset.clip_arrays(config.clip_seq)
+    if config.pad_seq:
+        dataset.pad_arrays(config.pad_seq)
+    if config.label:
+        dataset.label_annot = config.label
+    return dataset
```

### Comparing `ertk-2022.4.0/src/ertk/dataset/utils.py` & `ertk-2023.6.0/src/ertk/dataset/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+"""Utilities for working with audio datasets."""
+
 import logging
 import subprocess
 from pathlib import Path
 from typing import Iterable, List, Mapping
 
 from joblib import delayed
 
 from ertk.utils import PathOrStr, TqdmParallel
 
-# The below is because mypy does not yet support type narrowing upon redefinition
-# mypy: allow-redefinition
+__all__ = [
+    "get_audio_paths",
+    "resample_audio",
+    "resample_rename_clips",
+    "write_filelist",
+]
 
 
 def get_audio_paths(path: PathOrStr, absolute: bool = True) -> List[Path]:
     """Given a path to a dir or list of audio files, return a sequence
     of absolute paths to those files. Note that this method handles
     relative paths but returns absolute paths, and doesn't resolve
     canonical paths (i.e. it doesn't follow symlinks.)
@@ -28,76 +34,81 @@
 
     Returns
     -------
     List of paths to audio files. Paths will be absolute paths if
     `absolute=True`.
     """
     path = Path(path)
+    if absolute:
+        path = path.absolute()
     if path.is_dir():
         paths = [x for x in path.glob("*") if not x.is_dir()]
     else:
+        par_dir = path.parent
         with open(path) as fid:
-            paths = [path.parent / x.strip() for x in fid]
-    if absolute:
-        return [x.absolute() for x in paths]
+            paths = [par_dir / x.strip() for x in fid]
     return paths
 
 
-def resample_rename_clips(mapping: Mapping[Path, Path]):
+def resample_rename_clips(mapping: Mapping[Path, Path], sr: int = 16000):
     """Resample given audio clips to 16 kHz 16-bit WAV.
 
     Parameters
     ----------
     mapping: mapping
         Mapping from source files to destination files.
+    sr: int
+        Sample rate.
     """
     dst_dirs = {x.parent for x in mapping.values()}
     for dir in dst_dirs:
         dir.mkdir(exist_ok=True, parents=True)
 
-    opts = ["-nostdin", "-ar", "16000", "-sample_fmt", "s16", "-ac", "1", "-y"]
+    opts = ["-nostdin", "-ar", f"{sr:d}", "-sample_fmt", "s16", "-ac", "1", "-y"]
     logging.info(f"Resampling {len(mapping)} audio files")
     logging.info(f"Using FFmpeg options: {' '.join(opts)}")
     TqdmParallel(desc="Resampling audio", total=len(mapping), unit="file", n_jobs=-1)(
         delayed(subprocess.run)(
             ["ffmpeg", "-i", str(src), *opts, str(dst)],
             stdout=subprocess.DEVNULL,
             stderr=subprocess.STDOUT,
         )
         for src, dst in mapping.items()
     )
 
 
-def resample_audio(paths: Iterable[PathOrStr], dir: PathOrStr):
+def resample_audio(paths: Iterable[PathOrStr], dir: PathOrStr, sr: int = 16000):
     """Resample given audio clips to 16 kHz 16-bit WAV, and place in
     direcotory given by `dir`.
 
     Parameters
     ----------
     paths: iterable of Path
         A collection of paths to audio files to resample.
     dir: Pathlike or str
         Output directory.
+    sr: int
+        Sample rate.
     """
     paths = list(map(Path, paths))
     if len(paths) == 0:
         raise FileNotFoundError("No audio files found.")
 
-    resample_rename_clips({x: Path(dir, f"{x.stem}.wav") for x in paths})
+    resample_rename_clips({x: Path(dir, f"{x.stem}.wav") for x in paths}, sr=sr)
 
 
 def write_filelist(paths: Iterable[PathOrStr], path: PathOrStr):
     """Write sorted file list.
 
     Parameters
     ----------
     paths: iterable of Path
         Paths to audio clips.
-    name: str
-        Name of resulting file list.
+    path: str
+        Path of resulting file list.
     """
     paths = sorted(map(Path, paths), key=lambda p: p.stem)
     path = Path(path)
     if path.suffix == "":
         path = path.with_suffix(".txt")
     with open(path, "w") as fid:
         fid.write("\n".join(list(map(str, paths))) + "\n")
```

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/audioset/_vggish/vggish_params.py` & `ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/vggish_params.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/audioset/_vggish/vggish_postprocess.py` & `ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/vggish_postprocess.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/audioset/_vggish/vggish_slim.py` & `ertk-2023.6.0/src/ertk/preprocessing/audioset/_vggish/vggish_slim.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/audioset/_yamnet/features.py` & `ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/features.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/audioset/_yamnet/params.py` & `ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/params.py`

 * *Files identical despite different names*

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/audioset/_yamnet/yamnet.py` & `ertk-2023.6.0/src/ertk/preprocessing/audioset/_yamnet/yamnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import csv
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras import Model, layers
 
-import features as features_lib
+from . import features as features_lib
 
 
 def _batch_norm(name, params):
     def _bn_layer(layer_input):
         return layers.BatchNormalization(
             name=name,
             center=params.batchnorm_center,
```

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/base.py` & `ertk-2023.6.0/src/ertk/preprocessing/_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,44 +2,49 @@
 import warnings
 from abc import ABC, abstractmethod
 from itertools import chain, tee
 from typing import ClassVar, Dict, Iterable, List, Optional, Type, Union, cast
 
 import librosa
 import numpy as np
+from importlib_metadata import EntryPoint, entry_points
 from omegaconf import OmegaConf
 
 from ertk.config import ERTKConfig
 from ertk.utils import PathOrStr, batch_iterable
 
 
 class InstanceProcessor(ABC):
     """An instance processor.
 
     Parameters
     ----------
     config: ERTKConfig
-        The configuration for this AudioClipProcessor.
+        The configuration for this processor.
     """
 
     config: ERTKConfig
-    """The configuration for this AudioClipProcessor."""
+    """The configuration for this processor."""
     logger: logging.Logger
+    """The logger for this processor."""
 
     _config_type: ClassVar[Type[ERTKConfig]]
     _friendly_name: ClassVar[str]
     _registry: ClassVar[Dict[str, Type["InstanceProcessor"]]] = {}
+    _plugins: ClassVar[Dict[str, EntryPoint]] = {
+        x.name: x for x in entry_points().select(group="ertk.processors")
+    }
 
     def __init__(self, config: ERTKConfig) -> None:
         self.config = config
-        cls_name = f"{InstanceProcessor.__module__}.{InstanceProcessor.__name__}"
+        cls_name = f"{type(self).__module__}.{type(self).__name__}"
         self.logger = logging.getLogger(cls_name)
 
     def __init_subclass__(
-        cls, fname: str = None, config: Type[ERTKConfig] = None
+        cls, fname: Optional[str] = None, config: Optional[Type[ERTKConfig]] = None
     ) -> None:
         cls._registry = {}
         if fname and config:
             cls._friendly_name = fname
             cls._config_type = config
             for t in cls.mro()[1:-1]:
                 t = cast(Type[InstanceProcessor], t)  # For MyPy
@@ -50,32 +55,100 @@
                     msg = f"Name {fname} already registered with class {prev_cls}."
                     if prev_cls is cls:
                         warnings.warn(msg)
                     else:
                         raise KeyError(msg)
                 t._registry[fname] = cls
 
+    def __repr__(self):
+        return f"{type(self).__name__}({self.config})"
+
+    def __str__(self):
+        yaml = OmegaConf.to_yaml(self.config).strip()
+        yaml = "\t" + yaml.replace("\n", "\n\t")
+        return f"{type(self)._friendly_name}(\n{yaml}\n)"
+
     @classmethod
-    def get_processor_class(cls, name: str) -> Type["InstanceProcessor"]:
+    def friendly_name(cls) -> str:
+        """Get the friendly name for this processor."""
+        return cls._friendly_name
+
+    @classmethod
+    def get_processor_class(cls, name: str) -> "Type[InstanceProcessor]":
+        """Get the class for the named processor.
+
+        Parameters
+        ----------
+        name: str
+            The name of the processor.
+
+        Returns
+        -------
+        processor: Type[InstanceProcessor]
+            The processor class.
+        """
+        if name not in cls._registry:
+            ep = cls._plugins.get(name)
+            if ep is None:
+                raise KeyError(f"Unknown processor: {name}")
+            try:
+                obj = ep.load()
+            except ImportError as e:
+                raise ImportError(f"Plugin {ep.name} could not be loaded.") from e
+            if not issubclass(obj, InstanceProcessor):
+                raise TypeError(
+                    f"Plugin {ep.name} of type {obj} does not subclass "
+                    "InstanceProcessor"
+                )
+            cls._registry[name] = obj
         return cls._registry[name]
 
     @classmethod
     def make_processor(cls, name: str, config: ERTKConfig) -> "InstanceProcessor":
+        """Create an instance of the named processor.
+
+        Parameters
+        ----------
+        name: str
+            The name of the processor to create.
+        config: ERTKConfig
+            The configuration for the processor.
+
+        Returns
+        -------
+        processor: InstanceProcessor
+            The created processor.
+        """
         return cls.get_processor_class(name)(config)
 
     @classmethod
     def get_config_type(cls) -> Type[ERTKConfig]:
+        """Get the configuration type for this processor."""
         return cls._config_type
 
     @classmethod
-    def valid_preprocessors(cls) -> List[str]:
-        return list(cls._registry)
+    def valid_processors(cls) -> List[str]:
+        """Get a list of all registered processor names.
+
+        Returns
+        -------
+        names: list of str
+            The names of all registered processors.
+        """
+        return sorted(cls._registry.keys() | cls._plugins.keys())
 
     @classmethod
-    def get_default_config(cls):
+    def get_default_config(cls) -> ERTKConfig:
+        """Get the default configuration for this processor.
+
+        Returns
+        -------
+        config: ERTKConfig
+            The default configuration.
+        """
         return OmegaConf.structured(cls._config_type)
 
     @abstractmethod
     def process_instance(self, x: np.ndarray, **kwargs) -> np.ndarray:
         """Process a single audio clip.
 
         Parameters
@@ -126,22 +199,33 @@
             A generator that yields each processed instance in order.
         """
         if batch_size == 1:
             for x in xs:
                 yield self.process_instance(x, **kwargs)
         elif batch_size > 1:
             yield from chain.from_iterable(
-                self.process_batch(filter(lambda x: x is not None, b), **kwargs)
-                for b in batch_iterable(xs, batch_size)
+                self.process_batch(batch, **kwargs)
+                for batch in batch_iterable(xs, batch_size)
             )
         elif batch_size < 0:
             yield from self.process_batch(xs, **kwargs)
         else:
             raise ValueError("Batch size cannot be 0.")
 
+    def finish(self) -> None:
+        """Perform any cleanup necesasry (e.g. closing files, unloading
+        models, etc.)
+        """
+
+    @property
+    @abstractmethod
+    def feature_names(self) -> List[str]:
+        """The names of the features produced by this processor."""
+        raise NotImplementedError()
+
 
 class AudioClipProcessor(InstanceProcessor):
     """Processes raw audio data."""
 
     def process_file(self, path: PathOrStr, sr: Optional[float] = None) -> np.ndarray:
         """Process individual audio file.
 
@@ -193,18 +277,19 @@
             paths, tmp = tee(paths)
             _sr = librosa.load(next(tmp), sr=sr, duration=0)[1]
             audios = (librosa.load(path, sr=_sr, mono=True)[0] for path in paths)
             yield from self.process_all(audios, batch_size=batch_size, sr=_sr)
 
 
 class FeatureExtractor(InstanceProcessor):
+    """Extracts features from instances."""
+
     @property
-    @abstractmethod
     def dim(self) -> int:
         """The dimensionality of the extracted features."""
-        raise NotImplementedError()
+        return len(self.feature_names)
 
     @property
     @abstractmethod
     def is_sequence(self) -> bool:
         """Whether this FeatureExtractor yields sequence features."""
         raise NotImplementedError()
```

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/keras_apps.py` & `ertk-2023.6.0/src/ertk/preprocessing/keras_apps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,147 +1,190 @@
+"""Feature extractor using Keras applications."""
+
 from dataclasses import dataclass
 from types import ModuleType
 from typing import Iterable, List, Optional, Union
 
 import numpy as np
 from omegaconf import MISSING
 from scipy.ndimage import zoom
-from tensorflow.keras.applications import (
-    densenet,
-    efficientnet,
-    inception_resnet_v2,
-    inception_v3,
-    mobilenet,
-    mobilenet_v2,
-    mobilenet_v3,
-    nasnet,
-    resnet,
-    vgg16,
-    vgg19,
-    xception,
-)
 
 from ertk.config import ERTKConfig
 from ertk.preprocessing.spectrogram import spectrogram
-from ertk.tensorflow.utils import init_gpu_memory_growth
 from ertk.utils import is_mono_audio
 
-from .base import AudioClipProcessor, FeatureExtractor
+from ._base import AudioClipProcessor, FeatureExtractor
+
+__all__ = ["KerasAppsExtractorConfig", "KerasAppsExtractor"]
 
 
 @dataclass
-class ModelArgs:
+class _ModelArgs:
     module: ModuleType
     funcname: str
     size: int
 
 
-MODEL_MAP = {
-    "densenet121": ModelArgs(densenet, "DenseNet121", 224),
-    "densenet169": ModelArgs(densenet, "DenseNet169", 224),
-    "densenet201": ModelArgs(densenet, "DenseNet201", 224),
-    "efficientnet_b0": ModelArgs(efficientnet, "EfficientNetB0", 224),
-    "efficientnet_b1": ModelArgs(efficientnet, "EfficientNetB1", 240),
-    "efficientnet_b2": ModelArgs(efficientnet, "EfficientNetB2", 260),
-    "efficientnet_b3": ModelArgs(efficientnet, "EfficientNetB3", 300),
-    "efficientnet_b4": ModelArgs(efficientnet, "EfficientNetB4", 380),
-    "efficientnet_b5": ModelArgs(efficientnet, "EfficientNetB5", 456),
-    "efficientnet_b6": ModelArgs(efficientnet, "EfficientNetB6", 528),
-    "efficientnet_b7": ModelArgs(efficientnet, "EfficientNetB7", 600),
-    "inception_resnet_v2": ModelArgs(inception_resnet_v2, "InceptionResNetV2", 299),
-    "inception_v3": ModelArgs(inception_v3, "InceptionV3", 299),
-    "mobilenet": ModelArgs(mobilenet, "MobileNet", 224),
-    "mobilenet_v2": ModelArgs(mobilenet_v2, "MobileNetV2", 224),
-    "mobilenet_v3_large": ModelArgs(mobilenet_v3, "MobileNetV3Large", 224),
-    "mobilenet_v3_small": ModelArgs(mobilenet_v3, "MobileNetV3Small", 224),
-    "nasnet_large": ModelArgs(nasnet, "NASNetLarge", 331),
-    "nasnet_mobile": ModelArgs(nasnet, "NASNetMobile", 224),
-    "resnet50": ModelArgs(resnet, "ResNet50", 224),
-    "resnet50_v2": ModelArgs(resnet, "ResNet50V2", 224),
-    "resnet101": ModelArgs(resnet, "ResNet101", 224),
-    "resnet101_v2": ModelArgs(resnet, "ResNet101V2", 224),
-    "resnet152": ModelArgs(resnet, "ResNet152", 224),
-    "resnet152_v2": ModelArgs(resnet, "ResNet152V2", 224),
-    "vgg16": ModelArgs(vgg16, "VGG16", 224),
-    "vgg19": ModelArgs(vgg19, "VGG19", 224),
-    "xception": ModelArgs(xception, "Xception", 299),
-}
+MODEL_MAP = {}
+
+
+def _init_models():
+    from keras.applications import (
+        densenet,
+        efficientnet,
+        inception_resnet_v2,
+        inception_v3,
+        mobilenet,
+        mobilenet_v2,
+        mobilenet_v3,
+        nasnet,
+        resnet,
+        vgg16,
+        vgg19,
+        xception,
+    )
+
+    global MODEL_MAP
+    MODEL_MAP = {
+        "densenet121": _ModelArgs(densenet, "DenseNet121", 224),
+        "densenet169": _ModelArgs(densenet, "DenseNet169", 224),
+        "densenet201": _ModelArgs(densenet, "DenseNet201", 224),
+        "efficientnet_b0": _ModelArgs(efficientnet, "EfficientNetB0", 224),
+        "efficientnet_b1": _ModelArgs(efficientnet, "EfficientNetB1", 240),
+        "efficientnet_b2": _ModelArgs(efficientnet, "EfficientNetB2", 260),
+        "efficientnet_b3": _ModelArgs(efficientnet, "EfficientNetB3", 300),
+        "efficientnet_b4": _ModelArgs(efficientnet, "EfficientNetB4", 380),
+        "efficientnet_b5": _ModelArgs(efficientnet, "EfficientNetB5", 456),
+        "efficientnet_b6": _ModelArgs(efficientnet, "EfficientNetB6", 528),
+        "efficientnet_b7": _ModelArgs(efficientnet, "EfficientNetB7", 600),
+        "inception_resnet_v2": _ModelArgs(
+            inception_resnet_v2, "InceptionResNetV2", 299
+        ),
+        "inception_v3": _ModelArgs(inception_v3, "InceptionV3", 299),
+        "mobilenet": _ModelArgs(mobilenet, "MobileNet", 224),
+        "mobilenet_v2": _ModelArgs(mobilenet_v2, "MobileNetV2", 224),
+        "mobilenet_v3_large": _ModelArgs(mobilenet_v3, "MobileNetV3Large", 224),
+        "mobilenet_v3_small": _ModelArgs(mobilenet_v3, "MobileNetV3Small", 224),
+        "nasnet_large": _ModelArgs(nasnet, "NASNetLarge", 331),
+        "nasnet_mobile": _ModelArgs(nasnet, "NASNetMobile", 224),
+        "resnet50": _ModelArgs(resnet, "ResNet50", 224),
+        "resnet50_v2": _ModelArgs(resnet, "ResNet50V2", 224),
+        "resnet101": _ModelArgs(resnet, "ResNet101", 224),
+        "resnet101_v2": _ModelArgs(resnet, "ResNet101V2", 224),
+        "resnet152": _ModelArgs(resnet, "ResNet152", 224),
+        "resnet152_v2": _ModelArgs(resnet, "ResNet152V2", 224),
+        "vgg16": _ModelArgs(vgg16, "VGG16", 224),
+        "vgg19": _ModelArgs(vgg19, "VGG19", 224),
+        "xception": _ModelArgs(xception, "Xception", 299),
+    }
 
 
 @dataclass
 class KerasAppsExtractorConfig(ERTKConfig):
+    """Configuration for KerasAppsExtractor."""
+
     model: str = MISSING
+    """Name of the model to use. See https://keras.io/api/applications/
+    for the list of available models.
+    """
     size: Optional[int] = None
+    """Size of the input image. If not specified, the default size of the
+    model will be used.
+    """
     n_mels: int = 128
+    """Number of mel bands for spectrogram extraction."""
     spec_type: str = "mel"
+    """Type of spectrogram to extract. Can be either 'mel' or 'linear'."""
     fmax: int = 8000
+    """Maximum frequency for spectrogram extraction."""
 
 
 class KerasAppsExtractor(
     FeatureExtractor,
     AudioClipProcessor,
     fname="keras_apps",
     config=KerasAppsExtractorConfig,
 ):
+    """Feature extractor using Keras applications."""
+
     config: KerasAppsExtractorConfig
 
     def __init__(self, config: KerasAppsExtractorConfig) -> None:
         super().__init__(config)
 
+        from ertk.tensorflow.utils import init_gpu_memory_growth
+
         init_gpu_memory_growth()
+        _init_models()
 
-        args = {"include_top": False, "weights": "imagenet", "pooling": "avg"}
         model_args = MODEL_MAP[config.model]
         size = config.size or model_args.size
         self.size = size
-        args["input_shape"] = (size, size, 3)
-        func = getattr(model_args.module, model_args.funcname)
-        self.model = func(**args)
-        self.preprocess_input = getattr(model_args.module, "preprocess_input")
+        args = {
+            "include_top": False,
+            "weights": "imagenet",
+            "pooling": "avg",
+            "input_shape": (size, size, 3),
+        }
+        self.model = getattr(model_args.module, model_args.funcname)(**args)
+        self._preprocess_input = getattr(model_args.module, "preprocess_input")
+        _test = self._spectrogram(np.zeros(16000, dtype=np.float32), 16000)
+        _test = self._to_img(_test)
+        _test = self._preprocess_input(_test)
+        _test = self.model(_test[None, :, :, :]).numpy()
+        self._dim = _test.shape[-1]
 
     def _spectrogram(self, x: np.ndarray, sr: float) -> np.ndarray:
         return spectrogram(
             x,
-            sr=16000,
+            sr=sr,
             kind=self.config.spec_type,
             pre_emphasis=0,
             window_size=0.025,
             window_shift=0.01,
             n_mels=self.config.n_mels,
             fmin=0,
             fmax=None,
             power=2,
-            to_db=True,
+            to_log="db",
         )
 
     def _to_img(self, spec: np.ndarray) -> np.ndarray:
+        if spec.ndim > 2:
+            spec = spec.squeeze(0)
         scale = self.size / np.array(spec.shape)
         spec = zoom(spec, scale)
         spec = np.interp(spec, (spec.min(), spec.max()), (0, 255))
         return np.tile(spec[:, :, None], (1, 1, 3))
 
     def process_instance(self, x: np.ndarray, **kwargs) -> np.ndarray:
         if is_mono_audio(x):
-            x = self._spectrogram(x, kwargs.pop("sr"))
+            x = self._spectrogram(x.squeeze(), kwargs.pop("sr"))
         x = self._to_img(x)
-        x = self.preprocess_input(x)
-        return self.model(x).numpy()
+        x = self._preprocess_input(x)
+        return self.model(x[None, :, :, :]).numpy()
 
     def process_batch(
         self, batch: Union[Iterable[np.ndarray], np.ndarray], **kwargs
     ) -> List[np.ndarray]:
         batch = list(batch)
-        if all(is_mono_audio(x) for x in batch):
+        if any(is_mono_audio(x) for x in batch):
+            if any(not is_mono_audio(x) for x in batch):
+                raise RuntimeError("Inconsistent input representation")
             sr = kwargs.pop("sr")
-            batch = [self._spectrogram(x, sr) for x in batch]
+            batch = [self._spectrogram(x.squeeze(), sr) for x in batch]
         batch = [self._to_img(x) for x in batch]
         batch = np.stack(batch)
-        batch = self.preprocess_input(batch)
+        batch = self._preprocess_input(batch)
         return list(self.model(batch).numpy())
 
     @property
     def dim(self) -> int:
-        return super().dim
+        return self._dim
 
     @property
     def is_sequence(self) -> bool:
         return False
+
+    @property
+    def feature_names(self) -> List[str]:
+        return [f"{self.config.model}_{i}" for i in range(self.dim)]
```

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/opensmile.py` & `ertk-2023.6.0/src/ertk/preprocessing/opensmile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,79 @@
+"""OpenSMILE feature extraction."""
+
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, List
 
 import numpy as np
-import opensmile
 from omegaconf import MISSING
 
 from ertk.config import ERTKConfig
+from ertk.utils import is_mono_audio
+
+from ._base import AudioClipProcessor, FeatureExtractor
 
-from .base import AudioClipProcessor, FeatureExtractor
+__all__ = ["OpenSMILEExtractorConfig", "OpenSMILEExtractor"]
 
 
 @dataclass
 class OpenSMILEExtractorConfig(ERTKConfig):
+    """OpenSMILE feature extractor configuration."""
+
     opensmile_config: str = MISSING
+    """OpenSMILE config file."""
     levels: List[str] = field(default_factory=lambda: ["func"])
+    """OpenSMILE levels to extract."""
     opensmile_opts: Dict[str, str] = field(default_factory=dict)
+    """Additional OpenSMILE options."""
 
 
 class OpenSMILEExtractor(
     FeatureExtractor,
     AudioClipProcessor,
     fname="opensmile",
     config=OpenSMILEExtractorConfig,
 ):
+    """OpenSMILE feature extractor."""
+
     config: OpenSMILEExtractorConfig
 
     def __init__(self, config: OpenSMILEExtractorConfig) -> None:
+        import opensmile
+
         super().__init__(config)
 
         opensmile_config = config.opensmile_config
         if not Path(opensmile_config).exists():
             opensmile_config = opensmile.FeatureSet[opensmile_config]
 
         self.levels = config.levels
         self.smiles = [
             opensmile.Smile(
                 opensmile_config, level, options=dict(config.opensmile_opts)
             )
             for level in config.levels
         ]
-        self.feature_names = []
+        self._feature_names = []
         for smile in self.smiles:
-            self.feature_names.extend(smile.feature_names)
+            self._feature_names.extend(smile.feature_names)
 
     def process_instance(self, x: np.ndarray, **kwargs) -> np.ndarray:
-        xs = [smile(x, kwargs.pop("sr")) for smile in self.smiles]
+        sr = kwargs.pop("sr")
+        x = np.squeeze(x)
+        if not is_mono_audio(x):
+            raise ValueError("Audio must be mono")
+        xs = [smile(x, sr) for smile in self.smiles]
         # TODO: allow other window/padding correction options
         cut = min(x.shape[2] for x in xs)
         xs = [x[:, :, :cut] for x in xs]
         x = np.concatenate(xs, axis=1)
         # Get single segment and transpose axes so that frames are first
         return x[0].T
 
     @property
-    def dim(self) -> int:
-        return len(self.feature_names)
-
-    @property
     def is_sequence(self) -> bool:
         return "func" not in self.levels
+
+    @property
+    def feature_names(self) -> List[str]:
+        return self._feature_names
```

### Comparing `ertk-2022.4.0/src/ertk/preprocessing/openxbow/openxbow.py` & `ertk-2023.6.0/src/ertk/preprocessing/openxbow/openxbow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,63 @@
+"""OpenXBOW feature extractor."""
+
 import os
 import subprocess
 import tempfile
 from dataclasses import dataclass
 from importlib.resources import path as res_path
 from typing import Iterable, List, Union
 
 import numpy as np
 import pandas as pd
 from omegaconf import MISSING
 
 from ertk.config import ERTKConfig
 from ertk.dataset import write_features
-from ertk.preprocessing.base import FeatureExtractor
+from ertk.preprocessing._base import FeatureExtractor
+
+__all__ = ["OpenXBOWExtractorConfig", "OpenXBOWExtractor"]
 
 
 @dataclass
 class OpenXBOWExtractorConfig(ERTKConfig):
+    """Configuration for the OpenXBOW feature extractor."""
+
     xbowargs: List[str] = MISSING
+    """The arguments to pass to OpenXBOW."""
 
 
 class OpenXBOWExtractor(
     FeatureExtractor, fname="openxbow", config=OpenXBOWExtractorConfig
 ):
+    """OpenXBOW feature extractor."""
+
     config: OpenXBOWExtractorConfig
+    _dim = None
 
     def __init__(self, config: OpenXBOWExtractorConfig) -> None:
         super().__init__(config)
 
     def process_instance(self, x: np.ndarray, **kwargs) -> np.ndarray:
-        raise NotImplementedError()
+        raise NotImplementedError("Use batch_size=-1 for openxbow.")
 
     def process_batch(
-        self,
-        batch: Union[Iterable[np.ndarray], np.ndarray],
-        **kwargs,
+        self, batch: Union[Iterable[np.ndarray], np.ndarray], **kwargs
     ) -> List[np.ndarray]:
-
         _, tmpin = tempfile.mkstemp(prefix="openxbow_", suffix=".csv")
         _, tmpout = tempfile.mkstemp(prefix="openxbow_", suffix=".csv")
 
         xs = list(batch)
         names = [str(i) for i in range(len(xs))]
-        write_features(tmpin, xs, names=names)
+        self.logger.info(f"Writing temp CSV to {tmpin}")
+        write_features(tmpin, xs, names=names, header=False)
+
+        add_args = []
+        for arg in self.config.xbowargs:
+            add_args.extend(arg.split("=", maxsplit=1))
 
         with res_path("ertk.preprocessing.openxbow", "openXBOW.jar") as jar:
             xbow_args = [
                 "java",
                 "-jar",
                 str(jar),
                 "-i",
@@ -54,27 +66,45 @@
                 tmpout,
                 "-attributes",
                 f"n1[{xs[0].shape[1]}]",
                 "-csvSep",
                 ",",
                 "-writeName",
                 "-noLabels",
-                *self.config.xbowargs,
+                *add_args,
             ]
 
+        self.logger.info(f"Using cmdline: {' '.join(xbow_args)}")
         if subprocess.call(xbow_args) != 0:
             raise RuntimeError("openXBOW returned an error")
         os.remove(tmpin)
         data: pd.DataFrame = pd.read_csv(
             tmpout, header=None, quotechar="'", dtype={0: str}
         )
         os.remove(tmpout)
+        self._dim = data.shape[1] - 1
+        self.logger.debug(data.shape)
+        if not len(data) == len(xs):
+            raise RuntimeError("Got incorrect number of instances from openXBOW.")
 
         return list(data.iloc[:, 1:].to_numpy())
 
     @property
     def dim(self) -> int:
-        return super().dim
+        for i, arg in enumerate(self.config.xbowargs):
+            if arg.startswith("-size"):
+                try:
+                    _, size = arg.split("=", maxsplit=1)
+                except ValueError:
+                    size = self.config.xbowargs[i + 1]
+                return int(size)
+        if self._dim:
+            return self._dim
+        raise ValueError("Cannot determine dim.")
 
     @property
     def is_sequence(self) -> bool:
         return False
+
+    @property
+    def feature_names(self) -> List[str]:
+        return [f"bow_{i}" for i in range(self.dim)]
```

### Comparing `ertk-2022.4.0/src/ertk/pytorch/classification.py` & `ertk-2023.6.0/src/ertk/pytorch/classification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,158 +1,182 @@
+"""PyTorch classification utilities."""
+
 import logging
 import warnings
 from collections import defaultdict
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
-from pytorch_lightning.loggers import CSVLogger, TensorBoardLogger
+from pytorch_lightning.callbacks import Callback, ModelCheckpoint, ModelSummary
+from pytorch_lightning.loggers import CSVLogger, Logger, TensorBoardLogger
 from sklearn.model_selection import BaseCrossValidator, LeaveOneGroupOut
 from torch.utils.data import DataLoader, TensorDataset
 
 from ertk.pytorch.dataset import MTLDataModule
+from ertk.pytorch.models import LightningWrapper
 from ertk.pytorch.models.mtl import MTLModel
-from ertk.pytorch.utils import LightningWrapper
-from ertk.train import get_scores
+from ertk.pytorch.train import PyTorchTrainConfig
+from ertk.train import ExperimentResult, get_scores
 from ertk.utils import ScoreFunction
 
+__all__ = [
+    "pt_cross_validate",
+    "pt_train_val_test",
+    "train_mtl_model",
+]
+
 
 def pt_cross_validate(
     model_fn: Callable[..., Union[nn.Module, pl.LightningModule]],
     x: np.ndarray,
     y: np.ndarray,
     *,
     groups: Optional[np.ndarray] = None,
     cv: BaseCrossValidator = LeaveOneGroupOut(),
     scoring: Union[
         str, List[str], Dict[str, ScoreFunction], Callable[..., float]
     ] = "accuracy",
     verbose: int = 0,
+    n_jobs: int = 1,
     fit_params: Dict[str, Any] = {},
-):
-    batch_size = fit_params.pop("batch_size")
+) -> ExperimentResult:
     sw = fit_params.pop("sample_weight", None)
 
     logging.debug(f"cv={cv}")
     logging.debug(f"sample_weight={sw}")
-    logging.debug(f"fit_params={fit_params}")
 
     n_folds = cv.get_n_splits(x, y, groups)
     scores = defaultdict(list)
+    preds = np.zeros((len(y), len(np.unique(y))), dtype=np.float32)
     for fold, (train, test) in enumerate(cv.split(x, y, groups)):
         if verbose:
             logging.info(f"Fold {fold + 1}/{n_folds}")
 
         x_train = x[train]
         y_train = y[train]
         x_test = x[test]
         y_test = y[test]
         sw_train = sw[train] if sw is not None else None
         sw_test = sw[test] if sw is not None else None
 
-        _scores = pt_train_val_test(
+        result = pt_train_val_test(
             model_fn,
             train_data=(x_train, y_train, sw_train),
             valid_data=(x_test, y_test, sw_test),
             test_data=(x_test, y_test, sw_test),
             scoring=scoring,
             verbose=verbose,
             fit_params=dict(fit_params),
-            batch_size=batch_size,
         )
 
-        for k in _scores:
-            scores[k].append(_scores[k])
-    return {k: np.array(scores[k]) for k in scores}
+        for k, v in result.scores_dict.items():
+            scores[k].append(v)
+        preds[test] = result.predictions
+    return ExperimentResult({k: np.array(scores[k]) for k in scores}, predictions=preds)
 
 
 def pt_train_val_test(
     model_fn: Callable[..., Union[nn.Module, pl.LightningModule]],
     train_data: Tuple[np.ndarray, ...],
     valid_data: Tuple[np.ndarray, ...],
     test_data: Optional[Tuple[np.ndarray, ...]] = None,
     scoring: Union[
         str, List[str], Dict[str, ScoreFunction], Callable[..., float]
     ] = "accuracy",
     verbose: int = 0,
-    batch_size: int = 32,
-    fit_params: Dict[str, Any] = None,
-):
-    fit_params = fit_params or {}
-    log_dir = fit_params.pop("log_dir", None)
-    batch_size = fit_params.pop("batch_size", batch_size)
-    n_gpus = fit_params.pop("n_gpus", 1)
-
-    logging.debug(f"log_dir={log_dir}")
-
-    logger: Union[bool, List] = False
-    if log_dir is not None:
-        logger = [
-            TensorBoardLogger(log_dir, name=None, version=""),
-            CSVLogger(log_dir, name=None, version=""),
-        ]
+    fit_params: Dict[str, Any] = {},
+) -> ExperimentResult:
+    train_config: PyTorchTrainConfig = fit_params.pop("train_config")
+    log_dir = train_config.logging.log_dir
+    batch_size = train_config.batch_size
+
+    logging.debug(f"train_config={train_config}")
+
+    loggers: List[Logger] = []
+    callbacks: List[Callback] = []
+    if verbose:
+        callbacks.append(ModelSummary(5))
+    if log_dir:
+        _logger = TensorBoardLogger(log_dir, name=None)
+        loggers.append(_logger)
+        loggers.append(CSVLogger(_logger.log_dir, name=None, version=""))
+        if train_config.enable_checkpointing:
+            callbacks.append(
+                ModelCheckpoint(
+                    dirpath=_logger.log_dir,
+                    save_last=True,
+                    every_n_epochs=train_config.save_every_n_epochs,
+                    filename="checkpoint-{epoch}_{step}",
+                    verbose=verbose > 0,
+                )
+            )
 
     if test_data is None:
         test_data = valid_data
 
     clf = model_fn()
     logging.debug(clf)
-    if isinstance(clf, tuple):
+    if isinstance(clf, tuple):  # 'pipeline' tuple
         transform = clf[0]
         clf = clf[1]
         transform.fit(train_data[0], y=train_data[1])
         train_data = (transform.transform(train_data[0]), *train_data[1:])
         valid_data = (transform.transform(valid_data[0]), *valid_data[1:])
         test_data = (transform.transform(test_data[0]), *test_data[1:])
 
     if not isinstance(clf, pl.LightningModule):
-        clf = LightningWrapper(
-            clf,
-            nn.CrossEntropyLoss(reduction="none"),
-            optim_fn=fit_params.pop("optim_fn"),
-        )
+        clf = LightningWrapper(clf, train_config.wrapper_model_config)
 
     train_data_pt = tuple(torch.from_numpy(x) for x in train_data)
     valid_data_pt = tuple(torch.from_numpy(x) for x in valid_data)
     test_data_pt = tuple(torch.from_numpy(x) for x in test_data)
 
     train_ds = TensorDataset(*train_data_pt)
+    valid_ds = TensorDataset(*valid_data_pt)
+    test_ds = TensorDataset(*test_data_pt)
     train_dl = DataLoader(
         train_ds, batch_size=batch_size, shuffle=True, pin_memory=True
     )
-    valid_ds = TensorDataset(*valid_data_pt)
     valid_dl = DataLoader(
         valid_ds, batch_size=batch_size, shuffle=False, pin_memory=True
     )
-    test_ds = TensorDataset(*test_data_pt)
     test_dl = DataLoader(test_ds, batch_size=batch_size, shuffle=False, pin_memory=True)
 
     if verbose <= 0:
         logging.getLogger("pytorch_lightning").setLevel(logging.ERROR)
         warnings.simplefilter("ignore", UserWarning)
     trainer = pl.Trainer(
-        gpus=n_gpus,
-        strategy="dp",
-        max_epochs=fit_params.pop("max_epochs"),
-        logger=logger,
+        gpus=train_config.n_gpus,
+        strategy=train_config.dist_strategy,
+        max_epochs=train_config.epochs,
+        logger=loggers if loggers else False,
         enable_progress_bar=bool(verbose),
-        enable_model_summary=bool(verbose),
-        enable_checkpointing=False,
+        enable_checkpointing=train_config.enable_checkpointing,
+        enable_model_summary=False,
+        callbacks=callbacks,
     )
-    trainer.fit(clf, train_dataloaders=train_dl, val_dataloaders=valid_dl)
-    y_pred = torch.argmax(torch.cat(trainer.predict(clf, test_dl)), -1).cpu().numpy()
-    warnings.simplefilter("default", UserWarning)
+    trainer.fit(
+        clf,
+        train_dataloaders=train_dl,
+        val_dataloaders=valid_dl,
+        ckpt_path=train_config.resume_checkpoint,
+    )
+    y_pred = torch.cat(trainer.predict(clf, test_dl)).cpu().numpy()
+    if verbose <= 0:
+        logging.getLogger("pytorch_lightning").setLevel(logging.INFO)
+        warnings.simplefilter("default", UserWarning)
 
     y_true = test_data[1]
-    scores = get_scores(scoring, y_pred, y_true)
+    scores = get_scores(scoring, np.argmax(y_pred, -1), y_true)
     scores = {f"test_{k}": v for k, v in scores.items()}
-    return scores
+    return ExperimentResult(scores, predictions=y_pred)
 
 
 def train_mtl_model(
     model: MTLModel,
     tasks: Dict[int, int],
     data: Optional[MTLDataModule],
     train_data: Optional[DataLoader] = None,
```

### Comparing `ertk-2022.4.0/src/ertk/pytorch/models/mtl.py` & `ertk-2023.6.0/src/ertk/pytorch/models/mtl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,90 @@
+"""Multi-task learning MTL utilities."""
+
 from abc import ABC, abstractmethod
-from typing import Dict
+from dataclasses import dataclass, field
+from typing import Callable, Dict, List
 
-import pytorch_lightning as pl
+import omegaconf
 import torch
 
-from ertk.pytorch.utils import MTLTaskConfig
+from ertk.config import ERTKConfig
+from ertk.pytorch.utils import get_loss
 
+from ._base import ERTKPyTorchModel, PyTorchModelConfig
 
-class MTLModel(pl.LightningModule, ABC):
-    tasks: Dict[str, MTLTaskConfig]
+__all__ = ["MTLModelConfig", "MTLModel", "MTLTaskConfig"]
+
+
+@dataclass
+class MTLTaskConfig(ERTKConfig):
+    output_dim: int = omegaconf.MISSING
+    loss: str = omegaconf.MISSING
+    metrics: List[str] = field(default_factory=list)
+    weight: float = 1
 
-    def __init__(self, tasks: Dict[str, MTLTaskConfig], **kwargs) -> None:
-        super().__init__(**kwargs)
 
-        self.tasks = tasks
+@dataclass
+class MTLModelConfig(PyTorchModelConfig):
+    tasks: Dict[str, MTLTaskConfig] = omegaconf.MISSING
+
+
+class MTLModel(ERTKPyTorchModel, ABC):
+    tasks: Dict[str, MTLTaskConfig]
+    losses: Dict[str, Callable[[torch.Tensor, torch.Tensor], torch.Tensor]]
+    config: MTLModelConfig
+
+    def __init__(self, config: MTLModelConfig) -> None:
+        super().__init__(config)
+        self.tasks = config.tasks
+        self.losses = {n: get_loss(t.loss) for n, t in self.tasks.items()}
 
     @abstractmethod
     def forward(self, x: torch.Tensor, **kwargs) -> Dict[str, torch.Tensor]:
         raise NotImplementedError()
 
     def training_step(self, batch, batch_idx: int) -> torch.Tensor:
         x, ys = batch
         outputs = self.forward(x)
-        loss = 0
+        total_loss = 0
+        accs = {k: 0 for k in self.tasks}
         losses = {k: 0 for k in self.tasks}
         for k, v in outputs.items():
-            losses[k] += self.tasks[k].loss(v, ys[k]) * self.tasks[k].weight
-            loss += losses[k]
-        res = dict(loss=loss, **{f"train_{k}_loss": losses[k].detach() for k in losses})
+            loss = self.losses[k](v, ys[k])
+            losses[k] = loss
+            total_loss = total_loss + loss * self.tasks[k].weight
+            y_pred = v.argmax(1)
+            accs[k] = torch.sum(y_pred == ys[k]).item() / float(len(ys[k]))
+        res = {
+            "loss/train": total_loss,
+            **{f"acc_{k}/train": accs[k] for k in accs},
+            **{f"loss_{k}/train": losses[k] for k in losses},
+        }
         self.log_dict(res)
-        return loss
+        return total_loss
 
     def validation_step(self, batch, batch_idx: int) -> None:
         x, ys = batch
         outputs = self.forward(x)
-        val_loss = 0
+        total_loss = 0
         accs = {k: 0 for k in self.tasks}
         losses = {k: 0 for k in self.tasks}
         for k, v in outputs.items():
-            losses[k] += self.tasks[k].loss(v, ys[k]).item() * self.tasks[k].weight
-            val_loss += losses[k]
+            # print(k, ys[k])
+            loss = self.losses[k](v, ys[k])
+            losses[k] += loss
+            total_loss = total_loss + loss * self.tasks[k].weight
             y_pred = v.argmax(1)
             accs[k] = torch.sum(y_pred == ys[k]).item() / float(len(ys[k]))
         self.log_dict(
-            dict(
-                val_loss=val_loss,
-                **{f"{k}_acc": accs[k] for k in accs},
-                **{f"{k}_loss": losses[k] for k in losses},
-            )
+            {
+                "loss/valid": total_loss,
+                **{f"acc_{k}/valid": accs[k] for k in accs},
+                **{f"loss_{k}/valid": losses[k] for k in losses},
+            }
         )
+
+    def predict_step(self, batch, batch_idx: int) -> torch.Tensor:
+        return self.forward(batch[0])
+
+    def configure_optimizers(self):
+        return torch.optim.Adam(self.parameters(), lr=self.config.learning_rate)
```

### Comparing `ertk-2022.4.0/src/ertk/pytorch/models/simple_mtl.py` & `ertk-2023.6.0/src/ertk/pytorch/models/simple_mtl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,48 @@
+"""Simple MTL model consisting of shared layers followed by
+task-specific layers.
+"""
+
 from collections import OrderedDict
-from typing import Dict, Sequence, Type
+from dataclasses import dataclass, field
+from typing import Dict, List
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from .mtl import MTLModel, MTLTaskConfig
+from .layers import make_fc
+from .mtl import MTLModel, MTLModelConfig
 
+__all__ = ["SimpleMTLModel", "SimpleMTLModelConfig"]
 
-def make_hidden(sizes: Sequence[int], activation: Type[nn.Module]) -> nn.Module:
-    if len(sizes) == 0:
-        return nn.Identity()
-    return nn.Sequential(
-        *(
-            nn.Sequential(
-                nn.Linear(sizes[i], sizes[i + 1]),
-                activation(),
-            )
-            for i in range(len(sizes) - 1)
-        )
-    )
-
-
-class SimpleMTLModel(MTLModel):
-    def __init__(
-        self,
-        tasks: Dict[str, MTLTaskConfig],
-        input_dim: int,
-        opt_lr: float = 0.001,
-        shared_units: Sequence[int] = [512],
-        task_units: Sequence[int] = [512],
-    ):
-        super().__init__(tasks=tasks)
 
-        self.opt_lr = opt_lr
+@dataclass
+class SimpleMTLModelConfig(MTLModelConfig):
+    shared_units: List[int] = field(default_factory=lambda: [512])
+    task_units: List[int] = field(default_factory=lambda: [512])
+
 
-        self.save_hyperparameters("opt_lr", "shared_units", "task_units")
+class SimpleMTLModel(MTLModel, fname="simple_mtl", config=SimpleMTLModelConfig):
+    config: SimpleMTLModelConfig
 
-        shared_sizes = [input_dim] + list(shared_units)
-        self.shared = make_hidden(shared_sizes, nn.ReLU)
+    def __init__(self, config: SimpleMTLModelConfig):
+        super().__init__(config)
+
+        shared_sizes = [config.n_features] + list(config.shared_units)
+        self.shared = make_fc(shared_sizes, activation="relu", dropout=0, norm="none")
+        self.shared.append(nn.Tanh())
         self.add_module("shared", self.shared)
 
         self.task_layer = {}
         self.task_output = {}
-        task_sizes = [shared_sizes[-1]] + list(task_units)
+        task_sizes = [shared_sizes[-1]] + list(config.task_units)
         for name, task in self.tasks.items():
-            self.task_layer[name] = make_hidden(task_sizes, nn.ReLU)
+            self.task_layer[name] = make_fc(task_sizes, activation="relu", dropout=0)
+            self.task_layer[name].append(nn.ReLU())
             self.task_output[name] = nn.Linear(task_sizes[-1], task.output_dim)
             submod = nn.Sequential(
                 OrderedDict(
                     {
                         "embeddings": self.task_layer[name],
                         "output": self.task_output[name],
                     }
@@ -60,10 +53,7 @@
     def forward(self, x: torch.Tensor, **kwargs) -> Dict[str, torch.Tensor]:
         x = F.relu(self.shared(x))
         task_embeddings = {k: self.task_layer[k](x) for k in self.tasks}
         if kwargs.pop("embeddings_only", False):
             return task_embeddings
         out = {k: F.relu(v) for k, v in task_embeddings.items()}
         return {k: self.task_output[k](out[k]) for k in self.tasks}
-
-    def configure_optimizers(self):
-        return torch.optim.Adam(self.parameters(), lr=self.opt_lr)
```

### Comparing `ertk-2022.4.0/src/ertk/pytorch/models/test_fit.py` & `ertk-2023.6.0/src/ertk/pytorch/models/test_fit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,91 @@
 from pathlib import Path
+from typing import List, Tuple
 
 import click
-import numpy as np
 import pytorch_lightning as pl
 import torch
-from torch import nn
-from torch.optim import Adam
-from torch.utils.data import DataLoader, TensorDataset
+from omegaconf import OmegaConf
+from torch.utils.data import DataLoader, Dataset
 
-from ertk.config import get_arg_mapping
 from ertk.pytorch import get_pt_model
-from ertk.pytorch.utils import LightningWrapper
+from ertk.pytorch.models import PyTorchModelConfig
+
+
+class RandomDataset(Dataset[Tuple[torch.Tensor, ...]]):
+    def __init__(
+        self, total: int, shapes: List[Tuple[int]], dtypes: List[torch.dtype]
+    ) -> None:
+        super().__init__()
+        self.total = total
+        self.data = []
+        for shape, dtype in zip(shapes, dtypes):
+            self.data.append(torch.zeros(shape, dtype=dtype))
+
+    def __getitem__(self, index) -> Tuple[torch.Tensor, ...]:
+        return tuple(self.data)
+
+    def __len__(self) -> int:
+        return self.total
 
 
 @click.command()
 @click.argument("model_name")
 @click.option("--batch_size", type=int, default=32, help="Batch size.")
-@click.option("--1D/--2D", "is_1d", default=True, help="Input type.")
+@click.option("--shape", default="[(1024,), ()]", help="Shapes.")
+@click.option("--dtype", default="[torch.float32, torch.int64]", help="Dtypes.")
 @click.option(
     "--summary_only", is_flag=True, help="Print summary but don't train on dummy data."
 )
-@click.option(
-    "--memory/--generated",
-    default=False,
-    help="Have all data in memory or generate batches.",
-)
-@click.option("--model_args", type=click.Path(exists=True, path_type=Path))
+@click.option("--model_config", type=click.Path(exists=True, path_type=Path))
 @click.option("--train", type=int, default=8000, help="Number of training instances.")
 @click.option("--valid", type=int, default=800, help="Number of validation instances.")
-@click.option("--features", type=int, default=1024, help="Dimensionality of input.")
-@click.option("--steps", type=int, default=512, help="Length of sequence.")
+@click.argument("restargs", nargs=-1)
 def test_fit(
     model_name: str,
     batch_size: int,
-    is_1d: bool,
+    shape: str,
+    dtype: str,
     summary_only: bool,
-    memory: bool,
-    model_args: Path,
+    model_config: Path,
     train: int,
     valid: int,
-    features: int,
-    steps: int,
+    restargs: Tuple[str],
 ):
     """Trains a model for 2 epochs with random data and prints timing
-    information for testing purposes. The default number of instances is
-    8000, which is larger than the current largest dataset, MSP-IMPROV.
+    information for testing purposes.
     """
 
-    args = get_arg_mapping(model_args) if model_args else {}
-    model = get_pt_model(model_name, n_features=features, n_classes=4, **args)
-    if not isinstance(model, pl.LightningModule):
-        model = LightningWrapper(model, nn.CrossEntropyLoss(), lambda x: Adam(x, 0.001))
+    config: PyTorchModelConfig
+    if model_config:
+        config = OmegaConf.load(model_config)
+    else:
+        config = PyTorchModelConfig(
+            optimiser="adam", learning_rate=0.001, loss="cross_entropy"
+        )
+
+    cli_args = OmegaConf.from_cli(list(restargs))
+    if cli_args.model_config:
+        config = OmegaConf.merge(config, cli_args.model_config)
+
+    model = get_pt_model(model_name, config=config)
     print(model)
     trainable_params = sum(p.numel() for p in model.parameters() if p.requires_grad)
     total_params = sum(p.numel() for p in model.parameters())
     print("Trainable parameters: {}".format(trainable_params))
     print("Total parameters: {}".format(total_params))
     print()
 
     if summary_only:
         return
 
-    shape = (features,) if is_1d else (steps, features)
-
-    rng = np.random.default_rng()
-    train_x = torch.as_tensor(rng.random((train,) + shape, dtype=np.float32))
-    train_y = torch.as_tensor(rng.integers(4, size=train))
-    valid_x = torch.as_tensor(rng.random((valid,) + shape, dtype=np.float32))
-    valid_y = torch.as_tensor(rng.integers(4, size=valid))
-
-    train_data = TensorDataset(train_x, train_y)
-    valid_data = TensorDataset(valid_x, valid_y)
+    shapes = eval(shape, {})
+    dtypes = eval(dtype, {"torch": torch})
+    train_data = RandomDataset(train, shapes, dtypes)
+    valid_data = RandomDataset(valid, shapes, dtypes)
     train_dl = DataLoader(
         train_data, batch_size=batch_size, shuffle=True, pin_memory=True
     )
     valid_dl = DataLoader(
         valid_data, batch_size=batch_size, shuffle=False, pin_memory=True
     )
 
@@ -83,13 +94,12 @@
         logger=False,
         enable_progress_bar=True,
         enable_model_summary=False,
         enable_checkpointing=False,
         max_epochs=2,
     )
     trainer.fit(model, train_dataloaders=train_dl, val_dataloaders=valid_dl)
-    preds = torch.cat(trainer.predict(model, valid_dl)).cpu().numpy()
-    print(preds)
+    trainer.predict(model, valid_dl)
 
 
 if __name__ == "__main__":
     test_fit()
```

### Comparing `ertk-2022.4.0/src/ertk/pytorch/models/wav2vec_ft.py` & `ertk-2023.6.0/src/ertk/pytorch/models/wav2vec_ft.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,55 @@
-from typing import Any, Dict
+from dataclasses import dataclass
 
+import omegaconf
 import torch
 import torch.nn.functional as F
 from fairseq.checkpoint_utils import load_model_ensemble_and_task
 from torch import nn
-from torch.optim import SGD, Adam, RMSprop
 
-from ._base import SimpleClassificationModel
+from ._base import PyTorchModelConfig, SimpleClassificationModel
 
 
-class Model(SimpleClassificationModel):
+@dataclass
+class Wav2VecFineTuneConfig(PyTorchModelConfig):
+    checkpoint: str = omegaconf.MISSING
+    frozen_layers: int = -1
+
+
+class Model(
+    SimpleClassificationModel, fname="wav2vec_ft", config=Wav2VecFineTuneConfig
+):
     def __init__(
         self,
-        ckpt: str,
-        n_classes: int,
-        n_features: int = 1,
-        opt: str = "sgd",
-        lr: float = 0.1,
-        opt_params: Dict[str, Any] = {},
+        config: Wav2VecFineTuneConfig,
     ) -> None:
-        super().__init__(n_classes=n_classes, n_features=1)
+        super().__init__(config)
 
-        [model], args, task = load_model_ensemble_and_task([ckpt])
+        [model], args, task = load_model_ensemble_and_task([config.checkpoint])
         self.wav2vec = model
         self.w2v_args = args
         # self.w2v_task = task
 
         # Needed for multi-GPU training because of
         # https://github.com/pytorch/fairseq/issues/3482
         self.w2v_cfg = dict(task.cfg)
         if "text_compression_level" in self.w2v_cfg:
             self.w2v_cfg["text_compression_level"] = str(
                 self.w2v_cfg["text_compression_level"]
             )
 
-        self.lr = lr
-        self.opt = opt
-        self.opt_params = dict(opt_params)
-        self.save_hyperparameters("ckpt", "lr", "opt", "opt_params")
-
-        self.final = nn.Linear(512, n_classes)
+        self.final = nn.Linear(512, self.n_classes)
 
     def forward(self, x):
         x = x.squeeze(-1)
         x = self.wav2vec.feature_extractor(x)
         if self.wav2vec.vector_quantizer is not None:
             x, _ = self.wav2vec.vector_quantizer.forward_idx(x)
         x = x.mean(-1)
         x = self.final(x)
         return x
 
-    def configure_optimizers(self):
-        opt_cls = {"adam": Adam, "rmsprop": RMSprop, "sgd": SGD}[self.opt]
-        return opt_cls(self.parameters(), lr=self.lr, **self.opt_params)
-
     def preprocess_input(self, x: torch.Tensor) -> torch.Tensor:
         if self.w2v_cfg["normalize"]:
             with torch.no_grad():
                 x = F.layer_norm(x, x.shape)
         return x
```

### Comparing `ertk-2022.4.0/src/ertk/sklearn/models/mtl.py` & `ertk-2023.6.0/src/ertk/sklearn/models/mtl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,29 @@
+"""Multi-task learning models."""
+
+import warnings
+
 import liblinear.liblinearutil as liblinearutil
 import numpy as np
-from sklearn.base import BaseEstimator, ClassifierMixin, MetaEstimatorMixin
+import scipy.sparse as sp
+from sklearn.base import BaseEstimator, ClassifierMixin, clone
+from sklearn.exceptions import ConvergenceWarning
 from sklearn.linear_model import LogisticRegression
+from sklearn.model_selection import cross_val_predict
+from sklearn.multioutput import ClassifierChain
+from sklearn.preprocessing import OneHotEncoder
+from sklearn.utils import check_random_state
+from sklearn.utils.validation import check_is_fitted
 
-from ertk.sklearn.utils import OneVsRestClassifier
+__all__ = ["BaseMTFL", "MTFLClassifier", "MultiDimensionalCC"]
 
 _EPS = 1e-15
 
 
-class BaseBinaryMTFL(BaseEstimator):
+class BaseMTFL(BaseEstimator):
     """Linear regressor based on MTFL. Code adapted from
     https://github.com/argyriou/multi_task_learning
 
     Parameters
     ----------
     gamma: float
         Gamma value.
@@ -74,15 +85,15 @@
 
     def Dmin(self, a):
         return a / a.sum()
 
     def Dmin_eps(self, a, eps):
         return self.Dmin(np.sqrt(a**2 + eps))
 
-    def fit(self, X, y, tasks):
+    def fit(self, X, y, tasks, sample_weight=None):
         self._fit_feat(X, y, tasks)
         return self
 
     def _fit_feat(self, X, y, tasks):
         task_ids = np.unique(tasks)
         task_idxs = [np.flatnonzero(tasks == t) for t in task_ids]
         dim = X.shape[1]
@@ -126,141 +137,15 @@
         self.D_ = D
         self.costs_ = [_costs]
 
     def predict(self, X):
         return X @ self.W_
 
 
-class MTFLMulticlass(BaseEstimator, ClassifierMixin):
-    """Linear regressor based on MTFL. Code adapted from
-    https://github.com/argyriou/multi_task_learning
-
-    Parameters
-    ----------
-    gamma: float
-        Gamma value.
-    eps_init: float
-        Initial value for epsilon.
-    n_iters: int
-        Number of iterations per step.
-    """
-
-    def __init__(
-        self,
-        gamma: float = 1,
-        epsilon: float = 1e-4,
-        n_iters: int = 10,
-        loss: str = "logistic",
-    ):
-        self.gamma = gamma
-        self.epsilon = epsilon
-        self.n_iters = n_iters
-        self.loss = loss
-
-    def _loss(self, X, y, task_idxs):
-        num_tasks = len(task_idxs)
-        classes = np.unique(y)
-        W = np.zeros((len(classes), X.shape[1], num_tasks))
-        cost = np.zeros(len(classes))
-        err = np.zeros_like(cost)
-        for t_id in range(num_tasks):
-            task_x = X[task_idxs[t_id]]
-            task_y = y[task_idxs[t_id]]
-
-            task_classes = np.unique(task_y)
-            if self.loss == "logistic":
-                model = liblinearutil.train(
-                    task_y, task_x, f"-s 0 -e 1e-3 -c {self.gamma} -q"
-                )
-                for i, c in enumerate(task_classes):
-                    W[c, :, t_id] = model.get_decfun(label_idx=i)[0]
-            elif self.loss == "svm":
-                model = liblinearutil.train(
-                    task_y, task_x, f"-s 2 -e 1e-3 -c {self.gamma} -q"
-                )
-                for i, c in enumerate(task_classes):
-                    W[c, :, t_id] = model.get_decfun(label_idx=i)[0]
-            _cost = self.gamma * (W[:, :, t_id] ** 2).sum(-1)
-            cost += _cost
-        reg = cost - err
-        return W, cost, err, reg
-
-    def Dmin(self, a):
-        return a / a.sum()
-
-    def Dmin_eps(self, a, eps):
-        return self.Dmin(np.sqrt(a**2 + eps))
-
-    def fit(self, X, y, tasks):
-        self.classes_, y = np.unique(y, return_inverse=True)
-        self._fit_feat(X, y, tasks)
-        return self
-
-    def _fit_feat(self, X, y, tasks):
-        task_ids = np.unique(tasks)
-        task_idxs = [np.flatnonzero(tasks == t) for t in task_ids]
-        n_classes = len(self.classes_)
-        dim = X.shape[1]
-        Dini = np.tile(np.eye(dim) / dim, (n_classes, 1, 1))
-
-        def fmeth(a):
-            _a = np.zeros_like(a)
-            _a[a > _EPS] = 1 / a[a > _EPS]
-            return _a
-
-        # train_alternating
-        U, s, _ = np.linalg.svd(Dini, hermitian=True)
-        fS = np.sqrt(fmeth(s))
-        fS[fS > _EPS] = 1 / fS[fS > _EPS]
-        fD_isqrt = U @ np.apply_along_axis(np.diag, 1, fS) @ U.transpose(0, 2, 1)
-
-        _costs = np.empty((self.n_iters, n_classes, 3))
-        for i in range(self.n_iters):
-            W, cost, err, reg = self._loss((X @ fD_isqrt).mean(0), y, task_idxs)
-            W = fD_isqrt @ W
-
-            _costs[i] = np.c_[cost, err, reg]
-
-            U, s, _ = np.linalg.svd(W)
-            if dim > len(task_ids):
-                s = np.c_[
-                    s,
-                    np.zeros(
-                        (
-                            n_classes,
-                            dim - len(task_ids),
-                        )
-                    ),
-                ]
-            Smin = self.Dmin_eps(s, eps=self.epsilon)
-            D = U @ np.apply_along_axis(np.diag, 1, Smin) @ U.transpose(0, 2, 1)
-
-            U, s, _ = np.linalg.svd(D, hermitian=True)
-            fS = np.sqrt(fmeth(s))
-            fS[fS > _EPS] = 1 / fS[fS > _EPS]
-            fD_isqrt = U @ np.apply_along_axis(np.diag, 1, fS) @ U.transpose(0, 2, 1)
-        # train_alternating
-
-        s = np.linalg.svd(D, compute_uv=False)
-        _costs[:, [0, 2]] = (
-            _costs[:, [0, 2]] + self.gamma * self.epsilon * fmeth(s).sum()
-        )
-        self.mineps_ = self.epsilon
-        self.W_ = W
-        self.D_ = D
-        self.costs_ = [_costs]
-
-    def decision_function(self, X):
-        return (X @ self.W_).mean(-1)
-
-    def predict(self, X):
-        return self.classes_[(X @ self.W_).mean(-1).argmax(0)]
-
-
-class MTFLClassifier(BaseBinaryMTFL, ClassifierMixin):
+class MTFLClassifier(BaseMTFL, ClassifierMixin):
     """Classifier based on MTFL. Code adapted from
     https://github.com/argyriou/multi_task_learning
 
     Parameters
     ----------
     gamma: float
         Gamma value.
@@ -285,23 +170,25 @@
     ):
         self.gamma = gamma
         self.epsilon = epsilon
         self.n_iters = n_iters
         self.loss = loss
         self.aggregate = aggregate
 
-    def fit(self, X, y, tasks):
+    def fit(self, X, y, tasks, sample_weight=None):
         if len(np.unique(y)) > 2:
             raise ValueError("`y` should have only two classes")
         y = y.copy()
         y[y == 0] = -1
         self._fit_feat(X, y, tasks)
         if self.aggregate == "logistic":
             self.logistic_ = LogisticRegression(penalty="none")
+            warnings.simplefilter("ignore", ConvergenceWarning)
             self.logistic_.fit(super().predict(X), y)
+            warnings.simplefilter("default", ConvergenceWarning)
         return self
 
     def decision_function(self, X):
         preds = super().predict(X)
         if self.aggregate == "logistic":
             return self.logistic_.decision_function(preds)
         return preds.mean(-1)
@@ -312,7 +199,117 @@
             preds = self.logistic_.predict(preds)
         elif self.aggregate == "weighted":
             preds = np.sign(preds.mean(-1))
         elif self.aggregate == "unweighted":
             preds = np.sign(np.sign(preds).mean(-1))
         preds[preds == -1] = 0
         return preds
+
+
+class MultiDimensionalCC(ClassifierChain):
+    """Classifier chain for multi-dimensional output. Adapted from
+    sklearn's ClassifierChain and _BaseChain.
+
+    Parameters
+    ----------
+    base_estimator: estimator
+        The base estimator from which the classifier chain is built.
+    order: list of lists
+        The order of the outputs in the classifier chain.
+    """
+
+    def __init__(
+        self,
+        base_estimator,
+        *,
+        order=None,
+        cv=None,
+        random_state=None,
+        verbose: bool = False,
+    ) -> None:
+        super().__init__(base_estimator, order=order, cv=cv, random_state=random_state)
+        self.verbose = verbose
+
+    def fit(self, X, Y, **fit_params):
+        X, Y = self._validate_data(X, Y, multi_output=True, accept_sparse=True)
+
+        random_state = check_random_state(self.random_state)
+        self.order_ = self.order
+        if isinstance(self.order_, tuple):
+            self.order_ = np.array(self.order_)
+
+        if self.order_ is None:
+            self.order_ = np.array(range(Y.shape[1]))
+        elif isinstance(self.order_, str):
+            if self.order_ == "random":
+                self.order_ = random_state.permutation(Y.shape[1])
+        elif sorted(self.order_) != list(range(Y.shape[1])):
+            raise ValueError("invalid order")
+
+        self.estimators_ = [clone(self.base_estimator) for _ in range(Y.shape[1])]
+
+        encoder = OneHotEncoder(sparse=False)
+        Y_onehot = encoder.fit_transform(Y[:, self.order_])
+        cat_sizes = np.array([len(x) for x in encoder.categories_])
+        cat_sizes_cumsum = np.concatenate([[0], cat_sizes.cumsum()])
+        total_size = cat_sizes_cumsum[-1]
+
+        if self.cv is None:
+            Y_pred_chain = Y_onehot
+            if sp.issparse(X):
+                X_aug = sp.hstack((X, Y_pred_chain), format="lil")
+                X_aug = X_aug.tocsr()
+            else:
+                X_aug = np.hstack((X, Y_pred_chain))
+        elif sp.issparse(X):
+            Y_pred_chain = sp.lil_matrix((X.shape[0], total_size))
+            X_aug = sp.hstack((X, Y_pred_chain), format="lil")
+        else:
+            Y_pred_chain = np.zeros((X.shape[0], total_size))
+            X_aug = np.hstack((X, Y_pred_chain))
+
+        del Y_pred_chain
+
+        for chain_idx, estimator in enumerate(self.estimators_):
+            y = Y[:, self.order_[chain_idx]]
+            estimator.fit(
+                X_aug[:, : X.shape[1] + cat_sizes_cumsum[chain_idx]], y, **fit_params
+            )
+            if self.cv is not None and chain_idx < len(self.estimators_) - 1:
+                col_start = X.shape[1] + cat_sizes_cumsum[chain_idx]
+                col_end = X.shape[1] + cat_sizes_cumsum[chain_idx + 1]
+                cv_result = cross_val_predict(
+                    self.base_estimator, X_aug[:, :col_start], y=y, cv=self.cv
+                )
+                y_oh = OneHotEncoder(sparse=False).fit_transform(
+                    cv_result.reshape(-1, 1)
+                )
+                if sp.issparse(X_aug):
+                    X_aug[:, col_start:col_end] = y_oh
+                else:
+                    X_aug[:, col_start:col_end] = y_oh
+
+        self.classes_ = [estimator.classes_ for estimator in self.estimators_]
+        return self
+
+    def predict(self, X):
+        check_is_fitted(self)
+        X = self._validate_data(X, accept_sparse=True, reset=False)
+        Y_pred_chain = np.zeros((X.shape[0], len(self.estimators_)))
+
+        X_aug = X
+        for chain_idx, estimator in enumerate(self.estimators_):
+            if chain_idx != 0:
+                y_oh = OneHotEncoder(
+                    sparse=False, categories=[self.classes_[chain_idx - 1]]
+                ).fit_transform(Y_pred_chain[:, chain_idx - 1].reshape(-1, 1))
+                if sp.issparse(X):
+                    X_aug = sp.hstack((X_aug, y_oh))
+                else:
+                    X_aug = np.hstack((X_aug, y_oh))
+            Y_pred_chain[:, chain_idx] = estimator.predict(X_aug)
+
+        inv_order = np.empty_like(self.order_)
+        inv_order[self.order_] = np.arange(len(self.order_))
+        Y_pred = Y_pred_chain[:, inv_order]
+
+        return Y_pred
```

### Comparing `ertk-2022.4.0/src/ertk/sklearn/models/svm.py` & `ertk-2023.6.0/src/ertk/sklearn/models/svm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+"""Support Vector Machine (SVM) models for scikit-learn."""
+
 from functools import partial
 from typing import Any, Dict, Union
 
 from sklearn.base import BaseEstimator
 from sklearn.metrics.pairwise import kernel_metrics
 from sklearn.svm import SVC
 
+__all__ = ["PrecomputedSVC"]
+
 
 def _get_kernel_func(
     kernel: str,
     degree: int = 3,
     gamma: Union[str, float, None] = "auto",
     coef0: float = 0.0,
 ):
@@ -26,16 +30,16 @@
     return partial(f, **params)
 
 
 class PrecomputedSVC(SVC):
     """Class that wraps scikit-learn's SVC to precompute the kernel
     values in order to speed up training. The kernel parameter is a
     string which is transparently mapped to and from the corresponding
-    callable function with the relevant parameters (degree, gamma,
-    coef0). All other parameters are passed directly to SVC.
+    callable function with the relevant parameters (`degree`, `gamma`,
+    `coef0`). All other parameters are passed directly to SVC.
     """
 
     def __init__(
         self,
         *,
         C=1.0,
         kernel="rbf",
```

### Comparing `ertk-2022.4.0/src/ertk/stats.py` & `ertk-2023.6.0/src/ertk/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,74 @@
+"""Statistical functions."""
+
 from functools import partial
 from typing import Callable, List, Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import friedmanchisquare, rankdata
 from sklearn.metrics.pairwise import pairwise_distances
 from statsmodels.stats.libqsturng import qsturng
 
+__all__ = [
+    "holm_bonferroni",
+    "friedman_nemenyi",
+    "bhattacharyya_dist",
+    "corr_ratio",
+    "dunn",
+    "alpha",
+    "kappa",
+]
+
+
 Matrix = List[List[float]]
 
 
+def holm_bonferroni(
+    keys: Union[List[str], np.ndarray],
+    pvals: Union[List[float], np.ndarray],
+    alpha: float = 0.05,
+):
+    """Runs Holm-Bonferroni correction on given p-values.
+
+    Parameters
+    ----------
+    keys: List[str]
+        The keys corresponding to the p-values.
+    pvals: List[float]
+        The p-values to correct.
+    alpha: float
+        Significance level, must be in the range (0, 1), default is
+        0.05.
+
+    Returns
+    -------
+    rejected: List[str]
+        The keys of the hypotheses that were rejected.
+    failed: List[str]
+        The keys of the hypotheses that were not rejected.
+    """
+    keys = np.array(keys)
+    pvals = np.array(pvals)
+    sort = np.argsort(pvals)
+    pvals = pvals[sort]
+    keys = keys[sort]
+
+    n = len(keys)
+    for i in range(n):
+        if pvals[i] >= alpha / (n - i):
+            break
+    else:
+        i = n
+
+    rejected = keys[:i]
+    failed = keys[i:]
+    return rejected, failed
+
+
 def friedman_nemenyi(table: pd.DataFrame, alpha: float = 0.05):
     """Runs Friedman test on given table and optionally graphs a
     critical-difference diagram.
 
     Parameters
     ----------
     table: DataFrame
@@ -31,33 +86,29 @@
         The critical difference from the Nemenyi post-hoc test.
     df: pd.DataFrame
         A table containing statistics relating to ranking and average
         values of the condiions. The dataframe has these columns:
         "mean_rank", "mean", "std", "median", "mad", "effect_size".
     """
     _, pval = friedmanchisquare(*table.transpose().to_numpy())
-    names = list(table.columns)
     avgrank = rankdata(-table.to_numpy(), axis=1).mean(0)
     df = pd.DataFrame(
         {
             "mean_rank": avgrank,
             "mean": table.mean(),
             "std": table.std(),
+            "mad": (table - table.mean()).abs().mean(),
             "median": table.median(),
-            "mad": table.mad(),
         },
-        index=names,
+        index=table.columns,
     ).sort_values("mean_rank")
 
     topclf = df.index[0]
     n, k = table.shape
-    # Effect size is calculated in terms of differences in MAD
-    df["effect_size"] = (df.loc[topclf, "median"] - df["median"]) / np.sqrt(
-        ((n - 1) * df.loc[topclf, "mad"] ** 2 + (n - 1) * df["mad"] ** 2) / (2 * n - 2)
-    )
+    df["effect_size"] = (df.loc[topclf, "mean"] - df["mean"]) / df["std"]
     cd = qsturng(1 - alpha, k, np.inf) * np.sqrt((k * (k + 1)) / (12 * n))
     return pval, cd, df
 
 
 def _get_dist_func(metric: Union[Callable, str], **kwargs):
     if callable(metric):
         return partial(metric, **kwargs)
@@ -213,17 +264,17 @@
     cats = np.unique(data)
     n, N = data.shape
 
     counts = np.stack([np.sum(data == c, 0) for c in cats], 1)
 
     p_j = np.sum(counts, axis=0) / (N * n)
     assert np.isclose(np.sum(p_j), 1)
-    Pe = np.sum(p_j ** 2)
+    Pe = np.sum(p_j**2)
 
-    P = (np.sum(counts ** 2, 1) - n) / (n * (n - 1))
+    P = (np.sum(counts**2, 1) - n) / (n * (n - 1))
     Pbar = np.mean(P)
 
     return (Pbar - Pe) / (1 - Pe)
 
 
 class Deltas:
     @staticmethod
@@ -267,15 +318,15 @@
     def ordinal(c: int, k: int):
         if k < c:
             c, k = k, c
         s = (
             sum(count_sum[g] for g in range(c, k + 1))
             - (count_sum[c] + count_sum[k]) / 2
         )
-        return s ** 2
+        return s**2
 
     if isinstance(delta, str):
         delta = {
             "nominal": Deltas.nominal,
             "ordinal": ordinal,
             "interval": Deltas.interval,
         }[delta]
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/classification.py` & `ertk-2023.6.0/src/ertk/tensorflow/classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,57 @@
+"""TensorFlow classification utils."""
+
 import logging
+import time
 from collections import defaultdict
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import tensorflow as tf
+from keras.callbacks import TensorBoard
+from keras.metrics import SparseCategoricalAccuracy
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.model_selection import BaseCrossValidator
 from sklearn.pipeline import Pipeline
-from tensorflow.keras.callbacks import History, TensorBoard
-from tensorflow.keras.metrics import SparseCategoricalAccuracy
 
-from ertk.tensorflow.utils import (
+from ertk.tensorflow.dataset import (
     DataFunction,
-    TFModelFunction,
-    init_gpu_memory_growth,
+    get_data_fn,
     tf_dataset_gen,
     tf_dataset_mem,
     tf_dataset_mem_ragged,
 )
-from ertk.train import get_scores
+from ertk.tensorflow.utils import TFModelFunction, init_gpu_memory_growth
+from ertk.train import ExperimentResult, get_scores
 from ertk.utils import ScoreFunction, filter_kwargs
 
+__all__ = [
+    "tf_train_val_test",
+    "tf_cross_validate",
+    "tf_classification_metrics",
+    "TFClassifierWrapper",
+    "BalancedSparseCategoricalAccuracy",
+]
+
+logger = logging.getLogger(__name__)
+
 
 def tf_train_val_test(
     model_fn: TFModelFunction,
     train_data: Tuple[np.ndarray, ...],
     valid_data: Tuple[np.ndarray, ...],
     test_data: Optional[Tuple[np.ndarray, ...]] = None,
     scoring: Union[
         str, List[str], Dict[str, ScoreFunction], Callable[..., float]
     ] = "accuracy",
     data_fn: Union[DataFunction, str] = None,
     batch_size: int = 32,
     verbose: int = 0,
     fit_params: Dict[str, Any] = {},
-) -> Dict[str, Union[float, History]]:
+) -> ExperimentResult:
     """Trains on given data, using given validation data, and tests on
     given test data.
 
     Parameters
     ----------
     model_fn: callable
         The function used to create a compiled Model.
@@ -76,39 +89,36 @@
         test_data = valid_data
 
     data_fn = fit_params.pop("data_fn", data_fn)
     batch_size = fit_params.pop("batch_size", batch_size)
     if "sample_weight" in fit_params:
         del fit_params["sample_weight"]  # Part of *_data
 
-    data_fns = {
-        "mem": tf_dataset_mem,
-        "gen": tf_dataset_gen,
-        "mem_ragged": tf_dataset_mem_ragged,
-    }
     if data_fn is None:
         if len(train_data[0].shape) == 3:
             data_fn = tf_dataset_gen
         elif len(train_data[0].shape) == 1:
             data_fn = tf_dataset_mem_ragged
         else:
             data_fn = tf_dataset_mem
     elif isinstance(data_fn, str):
-        data_fn = data_fns[data_fn]
+        data_fn = get_data_fn(data_fn)
     elif not callable(data_fn):
         raise ValueError(f"Unsupported value for data_fn {data_fn}")
 
-    logging.debug(f"fit_params={fit_params}")
-    logging.debug(f"batch_size={batch_size}")
-    logging.debug(f"data_fn={data_fn}")
+    logger.debug(f"fit_params={fit_params}")
+    logger.debug(f"batch_size={batch_size}")
+    logger.debug(f"data_fn={data_fn}")
+    if any(x[2] is not None for x in [train_data, valid_data, test_data]):
+        logger.debug("Using sample weights")
 
     tf.keras.backend.clear_session()
 
     clf = model_fn()
-    logging.debug(clf)
+    logger.debug(clf)
     if isinstance(clf, Pipeline):
         new_pipeline = clf[:-1]
         clf = clf._final_estimator
         new_pipeline.fit(train_data[0], y=train_data[1])
         train_data = (new_pipeline.transform(train_data[0]), *train_data[1:])
         valid_data = (new_pipeline.transform(valid_data[0]), *valid_data[1:])
         test_data = (new_pipeline.transform(test_data[0]), *test_data[1:])
@@ -120,41 +130,48 @@
     train_dataset = data_fn(*train_data, batch_size=batch_size)
     valid_dataset = data_fn(*valid_data, batch_size=batch_size, shuffle=False)
     test_dataset = data_fn(*test_data, batch_size=batch_size, shuffle=False)
 
     clf.summary(print_fn=logging.info)
 
     fit_params = filter_kwargs(fit_params, clf.fit)
-    history = clf.fit(
-        train_dataset, validation_data=valid_dataset, verbose=verbose, **fit_params
-    )
+    start_time = time.perf_counter()
+    clf.fit(train_dataset, validation_data=valid_dataset, verbose=verbose, **fit_params)
+    fit_time = time.perf_counter() - start_time
+
     # Setting y_true is necessary for dataset creation routines that may
     # reorder data on creation (but without shuffling each time).
     y_true = np.concatenate([x[1] for x in test_dataset.as_numpy_iterator()])
-    y_pred = tf.argmax(clf.predict(test_dataset), axis=-1)
-
-    scores = get_scores(scoring, y_pred, y_true)
+    start_time = time.perf_counter()
+    y_pred = np.array(clf.predict(test_dataset))
+    score_time = time.perf_counter() - start_time
+
+    scores: Dict[str, Any] = {
+        "fit_time": fit_time,
+        "score_time": score_time,
+        **get_scores(scoring, np.argmax(y_pred, -1), y_true),
+    }
     scores = {f"test_{k}": v for k, v in scores.items()}
-    scores["history"] = history
-    return scores
+    return ExperimentResult(scores, predictions=y_pred)
 
 
 def tf_cross_validate(
     model_fn: TFModelFunction,
     x: np.ndarray,
     y: np.ndarray,
     *,
     cv: BaseCrossValidator,
     groups: Optional[np.ndarray] = None,
     verbose: int = 0,
     scoring: Union[
         str, List[str], Dict[str, ScoreFunction], Callable[..., float]
     ] = "accuracy",
+    n_jobs: int = 1,
     fit_params: Dict[str, Any] = {},
-):
+) -> ExperimentResult:
     """Performs cross-validation on a TensorFlow model. This works with
     both sequence models and single vector models.
 
     Parameters
     ----------
     model_fn: callable,
         The function used to create a compiled Keras model. This is
@@ -183,25 +200,26 @@
     """
     init_gpu_memory_growth()
 
     log_dir = fit_params.pop("log_dir", None)
     sw = fit_params.pop("sample_weight", None)
     data_fn = fit_params.pop("data_fn", None)
 
-    logging.debug(f"log_dir={log_dir}")
-    logging.debug(f"sample_weight={sw}")
-    logging.debug(f"data_fn={data_fn}")
-    logging.debug(f"cv={cv}")
-    logging.debug(f"fit_params={fit_params}")
+    logger.debug(f"log_dir={log_dir}")
+    logger.debug(f"sample_weight={sw}")
+    logger.debug(f"data_fn={data_fn}")
+    logger.debug(f"cv={cv}")
+    logger.debug(f"fit_params={fit_params}")
 
     n_folds = cv.get_n_splits(x, y, groups)
     scores = defaultdict(list)
+    preds = np.zeros((len(y), len(np.unique(y))), dtype=np.float32)
     for fold, (train, test) in enumerate(cv.split(x, y, groups)):
         if verbose:
-            logging.info(f"Fold {fold + 1}/{n_folds}")
+            logger.info(f"Fold {fold + 1}/{n_folds}")
 
         x_train = x[train]
         y_train = y[train]
         x_test = x[test]
         y_test = y[test]
         sw_train = sw[train] if sw is not None else None
         sw_test = sw[test] if sw is not None else None
@@ -214,28 +232,29 @@
                     profile_batch=0,
                     write_graph=False,
                     write_images=False,
                 )
             )
 
         fit_params["callbacks"] = callbacks
-        _scores = tf_train_val_test(
+        result = tf_train_val_test(
             model_fn,
             train_data=(x_train, y_train, sw_train),
             valid_data=(x_test, y_test, sw_test),
             test_data=(x_test, y_test, sw_test),
             data_fn=data_fn,
             scoring=scoring,
             verbose=verbose,
             fit_params=dict(fit_params),
         )
 
-        for k in _scores:
-            scores[k].append(_scores[k])
-    return {k: np.array(scores[k]) for k in scores}
+        for k, v in result.scores_dict.items():
+            scores[k].append(v)
+        preds[test] = result.predictions
+    return ExperimentResult({k: np.array(scores[k]) for k in scores}, predictions=preds)
 
 
 class TFClassifierWrapper(ClassifierMixin, BaseEstimator):
     """Class wrapper for a TensorFlow Keras classifier model.
 
     Parameters
     ----------
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/aldeneh2017.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/aldeneh2017.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-"""Implementation of the final full model architecture from [1].
+"""Implementation of the model architecture from [1]_.
 
-[1] Z. Aldeneh and E. Mower Provost, 'Using regional saliency for speech
-emotion recognition', in 2017 IEEE International Conference on
-Acoustics, Speech and Signal Processing (ICASSP), Mar. 2017, pp.
-2741–2745, doi: 10.1109/ICASSP.2017.7952655.
+References
+----------
+.. [1] Z. Aldeneh and E. Mower Provost, 'Using regional saliency for
+       speech emotion recognition', in 2017 IEEE International
+       Conference on Acoustics, Speech and Signal Processing (ICASSP),
+       Mar. 2017, pp. 2741-2745, doi: 10.1109/ICASSP.2017.7952655.
 """
 
-from tensorflow.keras import Model
-from tensorflow.keras.layers import Conv1D, Dense, GlobalMaxPool1D, Input, concatenate
+from keras import Model
+from keras.layers import Conv1D, Dense, GlobalMaxPool1D, Input, concatenate
 
 __all__ = ["model"]
 
 
 def model(n_features: int, n_classes: int) -> Model:
     inputs = Input(shape=(None, n_features), name="input")
     x = Conv1D(384, 8, activation="relu", kernel_initializer="he_normal", name="conv8")(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/depinto2020.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/depinto2020.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-"""Implementation of short model from [1].
+"""Implementation of short model from [1]_.
 
-[1] M. G. de Pinto, M. Polignano, P. Lops, and G. Semeraro, 'Emotions
-Understanding Model from Spoken Language using Deep Neural Networks and
-Mel-Frequency Cepstral Coefficients', in 2020 IEEE Conference on
-Evolving and Adaptive Intelligent Systems (EAIS), May 2020, pp. 1–5,
-doi: 10.1109/EAIS48028.2020.9122698.
+References
+----------
+.. [1] M. G. de Pinto, M. Polignano, P. Lops, and G. Semeraro, 'Emotions
+       Understanding Model from Spoken Language using Deep Neural
+       Networks and Mel-Frequency Cepstral Coefficients', in 2020 IEEE
+       Conference on Evolving and Adaptive Intelligent Systems (EAIS),
+       May 2020, pp. 1-5, doi: 10.1109/EAIS48028.2020.9122698.
 """
 
+from keras import Model
+from keras.layers import Conv1D, Dense, Dropout, Flatten, Input, MaxPool1D, Reshape
 
-from tensorflow.keras import Model
-from tensorflow.keras.layers import (
-    Conv1D,
-    Dense,
-    Dropout,
-    Flatten,
-    Input,
-    MaxPool1D,
-    Reshape,
-)
+__all__ = ["model"]
 
 
 def model(n_features: int, n_classes: int) -> Model:
     inputs = Input((n_features,))
     x = Reshape((n_features, 1))(inputs)
     # x = Conv1D(128, 40, activation="relu", padding="same")(x)
     # x = Dropout(0.2)(x)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/iskhakova2020.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/iskhakova2020.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-"""Implementation of model from [1].
+"""Implementation of model from [1]_.
 
-[1] A. O. Iskhakova, D. A. Wolf, R. R. Galin, and M. V. Mamchenko, ‘1-D
-convolutional neural network based on the inner ear principle to
-automatically assess human’s emotional state’, E3S Web Conf., vol. 224,
-p. 01023, 2020, doi: 10.1051/e3sconf/202022401023.
+References
+----------
+.. [1] A. O. Iskhakova, D. A. Wolf, R. R. Galin, and M. V. Mamchenko,
+       '1-D convolutional neural network based on the inner ear
+       principle to automatically assess human's emotional state', E3S
+       Web Conf., vol. 224, p. 01023, 2020, doi:
+       10.1051/e3sconf/202022401023.
 """
 
-from tensorflow.keras import Model
-from tensorflow.keras.layers import (
+from keras import Model
+from keras.layers import (
     BatchNormalization,
     Conv1D,
     Dense,
     Dropout,
     Flatten,
     Input,
     MaxPool1D,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/latif2019.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/latif2019.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-"""Implementation of the model from [1].
+"""Implementation of the model from [1]_.
 
-[1] S. Latif, R. Rana, S. Khalifa, R. Jurdak, and J. Epps, 'Direct
-Modelling of Speech Emotion from Raw Speech', arXiv:1904.03833 [cs,
-eess], Jul. 2019, Accessed: Feb. 10, 2020. [Online]. Available:
-http://arxiv.org/abs/1904.03833.
+References
+----------
+.. [1] S. Latif, R. Rana, S. Khalifa, R. Jurdak, and J. Epps, 'Direct
+       Modelling of Speech Emotion from Raw Speech', arXiv:1904.03833
+       [cs, eess], Jul. 2019, Accessed: Feb. 10, 2020. [Online].
+       Available: http://arxiv.org/abs/1904.03833.
 """
 
 import tensorflow as tf
-from tensorflow.keras.layers import (
+from keras.layers import (
     LSTM,
     BatchNormalization,
     Conv1D,
     Conv2D,
     Dense,
     Dropout,
     Input,
     MaxPool1D,
     MaxPool2D,
     ReLU,
     Reshape,
     concatenate,
 )
-from tensorflow.keras.models import Model
+from keras.models import Model
 
 __all__ = ["model"]
 
 
 def model(n_classes: int, n_features: int = 1):
     if n_features != 1:
         raise ValueError("This model can only accept waveform input.")
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/layers.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/layers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+"""Custom Keras layers for use in TensorFlow models."""
+
 import tensorflow as tf
-from tensorflow.keras.layers import Layer
+from keras.layers import Layer
+
+__all__ = ["Attention1D"]
 
 
 class Attention1D(Layer):
     """Layer that implements simple weighted pooling using softmax
     attention over a sequence of input vectors.
     """
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/mlp.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/mlp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-"""Basic MLP model."""
+"""Basic multi-layer perceptron (MLP) model."""
 
 from typing import Sequence
 
-from tensorflow.keras.layers import Dense, Dropout, Input
-from tensorflow.keras.models import Model
+from keras.layers import Dense, Dropout, Input
+from keras.models import Model
+
+__all__ = ["model"]
 
 
 def model(
     n_features: int,
     n_classes: int,
     units: Sequence[int] = [512],
     dropout: float = 0.5,
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/rbm.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/rbm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,40 @@
+"""Implementation of Restricted Boltzmann Machines (RBMs) [1]_ in
+TensorFlow.
+
+References
+----------
+.. [1] G. E. Hinton, “A Practical Guide to Training Restricted Boltzmann
+       Machines,” in Neural Networks: Tricks of the Trade: Second
+       Edition, G. Montavon, G. B. Orr, and K.-R. Müller, Eds., in
+       Lecture Notes in Computer Science. Berlin, Heidelberg: Springer
+       Berlin Heidelberg, 2012, pp. 599-619. doi:
+       10.1007/978-3-642-35289-8_32.
+"""
+
 from enum import Enum
 from math import pi
 from pathlib import Path
 from typing import Optional, Sequence, Tuple
 
+import click
+import numpy as np
 import tensorflow as tf
 
+from ertk.dataset import Dataset, write_features
 from ertk.utils import PathOrStr
 
 __all__ = ["BBRBM", "GBRBM"]
 
 
-def _sample_bernoulli(p):
+def _sample_bernoulli(p: tf.Tensor):
     return tf.nn.relu(tf.sign(p - tf.random.uniform(tf.shape(p))))
 
 
-def _sample_std_normal(p):
+def _sample_std_normal(p: tf.Tensor):
     return tf.random.normal()
 
 
 class DecayType(Enum):
     STEP = "STEP"
     COSINE = "COSINE"
     EXP = "EXP"
@@ -31,19 +47,19 @@
     """Restricted Boltzmann Machine
 
     This implementation is designed around the work of Hinton et. al.
     [1], [2].
 
     References
     ----------
-    [1] G. E. Hinton and R. R. Salakhutdinov, 'Reducing the
+    .. [1] G. E. Hinton and R. R. Salakhutdinov, 'Reducing the
     Dimensionality of Data with Neural Networks', Science, vol. 313, no.
     5786, pp. 504-507, Jul. 2006, doi: 10.1126/science.1127647.
 
-    [2] G. E. Hinton, 'A Practical Guide to Training Restricted
+    .. [2] G. E. Hinton, 'A Practical Guide to Training Restricted
     Boltzmann Machines', in Neural Networks: Tricks of the Trade: Second
     Edition, G. Montavon, G. B. Orr, and K.-R. Müller, Eds. Berlin,
     Heidelberg: Springer Berlin Heidelberg, 2012, pp. 599-619.
     """
 
     def __init__(
         self,
@@ -281,15 +297,15 @@
 
             with self.train_summary_writer.as_default():
                 tf.summary.scalar("mse", mse_train, step=epoch)
                 tf.print(f"mse: {mse_train:.3f}, ", end="")
 
                 tf.summary.scalar("learining_rate", self.learning_rate, step=epoch)
                 tf.summary.scalar("momentum", self.momentum, step=epoch)
-                weights_l2 = tf.reduce_sum(self.W ** 2)
+                weights_l2 = tf.reduce_sum(self.W**2)
                 tf.summary.scalar("weights_l2", weights_l2, step=epoch)
 
                 if self.output_histograms:
                     tf.summary.histogram("h_bias", self.h_bias, step=epoch)
                     tf.summary.histogram("v_bias", self.v_bias, step=epoch)
                     tf.summary.histogram("weights", self.W, step=epoch)
 
@@ -595,7 +611,97 @@
             Data to reconstruct.
 
         Returns
         -------
         The reconstructed data as a mapped tf.data.Dataset.
         """
         return data.map(self.reconstruct_batch)
+
+
+@click.command()
+@click.argument("input", type=click.Path(exists=True, dir_okay=False, path_type=Path))
+@click.option("--logdir", type=str, default="logs/tf/rbm")
+@click.option("--batch_size", type=int, default=16)
+@click.option("--valid_fraction", type=float, default=0.1)
+@click.option("--epochs", type=int, default=200)
+@click.option("--init_learning_rate", type=float, default=0.005)
+@click.option("--init_momentum", type=float, default=0.5)
+@click.option("--final_learning_rate", type=float, default=0.001)
+@click.option("--final_momentum", type=float, default=0.9)
+@click.option(
+    "--learning_rate_decay",
+    type=click.Choice(DecayType.__members__),
+    default=DecayType.STEP.name,
+)
+@click.option(
+    "--momentum_decay",
+    type=click.Choice(DecayType.__members__),
+    default=DecayType.STEP.name,
+)
+@click.option("--output", type=Path)
+def main(
+    input: Path,
+    logdir: str,
+    batch_size: int,
+    valid_fraction: float,
+    epochs: int,
+    init_learning_rate: float,
+    init_momentum: float,
+    final_learning_rate: float,
+    final_momentum: float,
+    learning_rate_decay: DecayType,
+    momentum_decay: DecayType,
+    output: Path,
+):
+    """Trains RBM on spectrograms in INPUT."""
+
+    learning_rate_decay = DecayType(learning_rate_decay)
+    momentum_decay = DecayType(momentum_decay)
+
+    for gpu in tf.config.list_physical_devices("GPU"):
+        tf.config.experimental.set_memory_growth(gpu, True)
+
+    dataset = Dataset(input)
+    x = dataset.x
+    input_shape = tuple(x[0].shape)
+    xmin = np.min(x, axis=(1, 2), keepdims=True)
+    xmax = np.max(x, axis=(1, 2), keepdims=True)
+    x = (x - xmin) / (xmax - xmin)
+    spectrograms = np.reshape(x, (dataset.n_instances, -1))
+
+    split = int(spectrograms.shape[0] * valid_fraction)
+    train_data = tf.data.Dataset.from_tensor_slices(spectrograms[split:, :])
+    train_data = train_data.shuffle(spectrograms.shape[0])
+    train_data = train_data.batch(batch_size).prefetch(10)
+    valid_data = tf.data.Dataset.from_tensor_slices(spectrograms[:split, :])
+    valid_data = valid_data.batch(batch_size).prefetch(10)
+
+    Path(logdir).mkdir(parents=True, exist_ok=True)
+    rbm = BBRBM(512, input_shape=input_shape, logdir=logdir, output_histograms=True)
+    rbm.train(
+        train_data,
+        valid_data,
+        n_epochs=epochs,
+        init_learning_rate=init_learning_rate,
+        init_momentum=init_momentum,
+        final_learning_rate=final_learning_rate,
+        final_momentum=final_momentum,
+        learning_rate_decay=learning_rate_decay,
+        momentum_decay=momentum_decay,
+    )
+    if output:
+        representations = rbm.representations(
+            tf.data.Dataset.from_tensor_slices(spectrograms).batch(8)
+        )
+        representations = np.concatenate(list(representations.as_numpy_iterator()))
+        feature_names = [f"bbrbm{i + 1}" for i in range(representations.shape[-1])]
+        write_features(
+            output,
+            names=dataset.names,
+            features=representations,
+            corpus=dataset.corpus,
+            feature_names=feature_names,
+        )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/test_fit.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/test_fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 
 import click
 import numpy as np
 
 from ertk.config import get_arg_mapping
 from ertk.tensorflow import get_tf_model
-from ertk.tensorflow.utils import init_gpu_memory_growth, tf_dataset_gen, tf_dataset_mem
+from ertk.tensorflow.dataset import tf_dataset_gen, tf_dataset_mem
+from ertk.tensorflow.utils import init_gpu_memory_growth
 
 
 @click.command()
 @click.argument("model_name")
 @click.option("--batch_size", type=int, default=32, help="Batch size.")
 @click.option(
     "--summary_only", is_flag=True, help="Print summary but don't train on dummy data."
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/transformer.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+"""Basic Transformer model for time series classification."""
+
 import numpy as np
 import tensorflow as tf
-from tensorflow.keras import Model
-from tensorflow.keras.layers import (
-    add,
+from keras import Model
+from keras.layers import (
     Dense,
-    GlobalAvgPool1D,
-    GlobalMaxPool1D,
+    GlobalAveragePooling1D,
+    GlobalMaxPooling1D,
     Input,
-    MultiHeadAttention,
     LayerNormalization,
+    MultiHeadAttention,
     ReLU,
+    add,
 )
 
+__all__ = ["model"]
+
 
 def _encoder_layer(x, num_heads: int, model_dim: int):
     att = MultiHeadAttention(num_heads=num_heads, key_dim=model_dim)(x, x)
     x = LayerNormalization()(x + att)
     ff = Dense(2048)(x)
     ff = ReLU()(ff)
     ff = Dense(model_dim)(ff)
@@ -46,12 +50,12 @@
 ) -> Model:
     inputs = Input((seq_len, n_features))
     x = Dense(model_dim, name="projection")(inputs)
     x = add([x, _positional_encoding(seq_len, model_dim)], name="positional_encoding")
     for _ in range(enc_layers):
         x = _encoder_layer(x, num_heads=num_heads, model_dim=model_dim)
     if pool == "max":
-        x = GlobalMaxPool1D()(x)
+        x = GlobalMaxPooling1D()(x)
     else:
-        x = GlobalAvgPool1D()(x)
+        x = GlobalAveragePooling1D()(x)
     x = Dense(n_classes, activation="softmax")(x)
     return Model(inputs=inputs, outputs=x)
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/zhang2019.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/zhang2019.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-"""Implementation of the model from [1].
+"""Implementation of the model from [1]_.
 
-[1] Z. Zhang, B. Wu, and B. Schuller, 'Attention-augmented End-to-end
-Multi-task Learning for Emotion Prediction from Speech', in ICASSP 2019
-- 2019 IEEE International Conference on Acoustics, Speech and Signal
-Processing (ICASSP), May 2019, pp. 6705–6709, doi:
-10.1109/ICASSP.2019.8682896.
+References
+----------
+.. [1] Z. Zhang, B. Wu, and B. Schuller, 'Attention-augmented End-to-end
+       Multi-task Learning for Emotion Prediction from Speech', in 2019
+       IEEE International Conference on Acoustics, Speech and Signal
+       Processing, May 2019, pp. 6705-6709, doi:
+       10.1109/ICASSP.2019.8682896.
 """
 
 from typing import Optional
 
 import numpy as np
 import tensorflow as tf
-from tensorflow.keras.layers import (
+from keras.layers import (
     GRU,
     RNN,
     Conv1D,
     Dense,
     Dropout,
     GRUCell,
     Input,
     MaxPool1D,
     Reshape,
     TimeDistributed,
 )
-from tensorflow.keras.models import Model, Sequential
+from keras.models import Model, Sequential
 
-from ertk.tensorflow.utils import tf_dataset_mem
+from ertk.tensorflow.dataset import tf_dataset_mem
 
 from .layers import Attention1D
 
 __all__ = ["model", "create_windowed_dataset"]
 
 
 def create_windowed_dataset(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ertk-2022.4.0/src/ertk/tensorflow/models/zhao2019.py` & `ertk-2023.6.0/src/ertk/tensorflow/models/zhao2019.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""Implementation of the model from [1].
+"""Implementation of the model from [1]_.
 
-[1] Z. Zhao et al., "Exploring Deep Spectrum Representations via
-Attention-Based Recurrent and Convolutional Neural Networks for Speech
-Emotion Recognition," IEEE Access, vol. 7, pp. 97515–97525, 2019, doi:
-10.1109/ACCESS.2019.2928625.
+.. [1] Z. Zhao et al., "Exploring Deep Spectrum Representations via
+       Attention-Based Recurrent and Convolutional Neural Networks for
+       Speech Emotion Recognition," IEEE Access, vol. 7, pp.
+       97515-97525, 2019, doi: 10.1109/ACCESS.2019.2928625.
 """
 
 import tensorflow as tf
-from tensorflow.keras.layers import (
+from keras.layers import (
     LSTM,
     RNN,
     BatchNormalization,
     Bidirectional,
     Conv2D,
     Dense,
     Dropout,
     Input,
     LSTMCell,
     MaxPool2D,
     ReLU,
     Reshape,
     concatenate,
 )
-from tensorflow.keras.models import Model
+from keras.models import Model
 
 from .layers import Attention1D
 
 __all__ = ["model"]
 
 
 def model(n_features: int, n_classes: int, steps: int = 512):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ertk-2022.4.0/src/ertk/transform.py` & `ertk-2023.6.0/src/ertk/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,34 @@
+"""Transforms to use in estimators.
+
+.. autosummary::
+    :toctree: generated/
+
+    group_transform
+    instance_transform
+    GroupTransformWrapper
+    InstanceTransformWrapper
+    SequenceTransform
+    SequenceTransformWrapper
+"""
+
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
 
 from ertk.utils import flat_to_inst, inst_to_flat
 
+__all__ = [
+    "group_transform",
+    "instance_transform",
+    "GroupTransformWrapper",
+    "InstanceTransformWrapper",
+    "SequenceTransform",
+    "SequenceTransformWrapper",
+]
+
 
 def group_transform(
     x: np.ndarray,
     groups: np.ndarray,
     transform: TransformerMixin,
     *,
     inplace: bool = False,
@@ -153,7 +175,13 @@
             flat_x = self.transformer.transform(flat_x, **fit_params)
         elif self.method == "global":
             flat_shape = flat_x.shape
             flat_x = self.transformer.transform(
                 flat_x.reshape((-1, 1)), **fit_params
             ).reshape(flat_shape)
         return flat_to_inst(flat_x, slices)
+
+    def __repr__(self, N_CHAR_MAX=700):
+        return (
+            f"{self.__class__.__name__}(transformer={self.transformer}, "
+            f"method={self.method})"
+        )
```

### Comparing `ertk-2022.4.0/src/ertk/utils/array.py` & `ertk-2023.6.0/src/ertk/utils/array.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,84 @@
+"""Utility functions for working with numpy arrays."""
+
 from typing import List, Optional, Sequence, Tuple, Union, overload
 
 import numpy as np
 
+__all__ = [
+    "batch_arrays_by_length",
+    "make_array_array",
+    "check_3d",
+    "is_mono_audio",
+    "frame_array",
+    "frame_arrays",
+    "pad_array",
+    "pad_arrays",
+    "clip_arrays",
+    "inst_to_flat",
+    "flat_to_inst",
+    "transpose_time",
+    "shuffle_multiple",
+]
+
 
 def make_array_array(x: List[np.ndarray]) -> np.ndarray:
-    """Helper function to make an array of arrays. The returned array
-    has `shape==(len(x),)` and `dtype==object`.
+    """Helper function to make an array of arrays.
+
+    Parameters
+    ----------
+    x: list of np.ndarray
+        The arrays to put in the array of arrays.
+
+    Returns
+    -------
+    arr: np.ndarray
+        The array of arrays, with ``shape==(len(x),)``, and
+        ``dtype==object``.
     """
     arr = np.empty(len(x), dtype=object)
     for i, a in enumerate(x):
         arr[i] = a
     return arr
 
 
 def check_3d(arrays: Union[Sequence[np.ndarray], np.ndarray]) -> None:
     """Checks if an array is 3D or each array in a list is 2D. Raises an
     exception if this isn't the case.
+
+    Parameters
+    ----------
+    arrays: np.ndarray or list of np.ndarray
+        The arrays to check.
+
+    Raises
+    ------
+    ValueError
+        If any array is not 3D.
     """
     if any(len(x.shape) != 2 for x in arrays):
         raise ValueError("arrays must be 3D (contiguous or vlen).")
 
 
 def is_mono_audio(x: np.ndarray) -> bool:
     """Checks if an array represents mono audio data. The conditions for
     this are that x can be squeezed to 1D.
 
     Note that this method will also return True for '2D' sequences of
     length 1, so care should be taken for edge cases.
+
+    Parameters
+    ----------
+    x: np.ndarray
+        The array to check.
+
+    Returns
+    -------
+    is_mono: bool
+        Whether the array represents mono audio data.
     """
     return np.squeeze(x).ndim == 1
 
 
 def frame_array(
     x: np.ndarray,
     frame_size: int,
@@ -78,17 +126,21 @@
     if num_frames <= 0:
         if not pad:
             raise ValueError(
                 "The length of the sequence is shorter than frame_size, but pad=False, "
                 "so no frames will be generated."
             )
         num_frames = 0
-    remainder = (x.shape[axis] - frame_size) % frame_shift
+    if frame_size > x.shape[axis]:
+        remainder = frame_size - x.shape[axis]
+    else:
+        remainder = (x.shape[axis] - frame_size) % frame_shift
     if remainder != 0:
         num_frames += 1 if pad else 0
+    assert num_frames > 0
     # Insert new dim before axis with num_frames, and axis is replaced
     # with the size of each frame.
     new_shape = x.shape[:axis] + (num_frames, frame_size) + x.shape[axis + 1 :]
 
     if copy:
         out = np.zeros(new_shape, dtype=x.dtype)
         for i in range(0, x.shape[axis] - frame_size + 1, frame_shift):
@@ -227,18 +279,30 @@
 
 @overload
 def pad_arrays(arrays: np.ndarray, pad: int) -> np.ndarray:
     pass
 
 
 def pad_arrays(arrays: Union[List[np.ndarray], np.ndarray], pad: int = 32):
-    """Pads each array to the nearest multiple of `pad` greater than the
-    array size. Assumes axis 0 of each sub-array, or axis 1 of x, is
-    the time axis. This is mainly a wrapper around `pad_array()` for
-    instance arrays.
+    """Pads each array to the nearest multiple of ``pad`` greater than the
+    array size.  This is mainly a wrapper around `pad_array()` that
+    takes care of padding ragged or non-contiguous arrays.
+
+    Parameters
+    ----------
+    arrays: list of np.ndarray
+        The arrays to process. Assumes axis 0 of each sub-array, or axis
+        1 of ``arrays``, is the time axis.
+    pad: int
+        The multiple to pad to.
+
+    Returns
+    -------
+    padded_arrays:
+        Padded arrays.
     """
     if isinstance(arrays, np.ndarray) and len(arrays.shape) > 1:
         # Contiguous 2D/3D
         return pad_array(arrays, to_multiple=pad, axis=1)
     new_arrays = [pad_array(x, to_multiple=pad, axis=0) for x in arrays]
     if isinstance(arrays, np.ndarray):
         if all(x.shape == new_arrays[0].shape for x in new_arrays):
@@ -259,15 +323,29 @@
 def clip_arrays(arrays: np.ndarray, length: int, copy: bool) -> np.ndarray:
     pass
 
 
 def clip_arrays(
     arrays: Union[List[np.ndarray], np.ndarray], length: int, copy: bool = True
 ):
-    """Clips each array to the specified maximum length."""
+    """Clips each array to the specified maximum sequence length.
+
+    Parameters
+    ----------
+    arrays: list of np.ndarray
+        The arrays to process. Assumes axis 0 of each sub-array, or axis
+        1 of ``arrays``, is the time axis.
+    length: int
+        The maximum length.
+
+    Returns
+    -------
+    clipped_arrays:
+        Clipped arrays.
+    """
     if isinstance(arrays, np.ndarray):
         if len(arrays.shape) > 1:
             return arrays[:, :length, ...].copy() if copy else arrays[:, :length, ...]
         new_arrays = [x[:length].copy() if copy else x[:length] for x in arrays]
         if all(x.shape == new_arrays[0].shape for x in new_arrays):
             # Return contiguous array
             return np.stack(new_arrays)
@@ -286,14 +364,25 @@
 
 
 def transpose_time(arrays: Union[List[np.ndarray], np.ndarray]):
     """Transpose the time and feature axis of each array. Requires each
     array be 2-D.
 
     Note: This function modifies the arrays in-place.
+
+    Parameters
+    ----------
+    arrays: list of np.ndarray
+        The arrays to process. Assumes axis 0 of each sub-array, or axis
+        1 of ``arrays``, is the time axis.
+
+    Returns
+    -------
+    transposed_arrays:
+        Transposed arrays.
     """
     check_3d(arrays)
     if isinstance(arrays, np.ndarray) and len(arrays.shape) == 3:
         arrays = arrays.transpose(0, 2, 1)
     else:
         for i in range(len(arrays)):
             arrays[i] = arrays[i].transpose()
@@ -314,14 +403,15 @@
     arrays, iterable of array-like
         The arrays to shuffle. They must all have the same size of first
         dimension.
     numpy_indexing: bool, default = True
         Whether to use NumPy-style indexing or list comprehension.
 
     Returns:
+    --------
     shuffled_arrays: iterable of array-like
         The shuffled arrays.
     """
     if any(len(arrays[0]) != len(x) for x in arrays):
         raise ValueError("Not all arrays have equal first dimension.")
 
     perm = np.random.default_rng(seed).permutation(len(arrays[0]))
@@ -338,15 +428,15 @@
     shuffle: bool = True,
     uniform_batch_size: bool = False,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Batches a list of arrays of different sizes, grouping them by
     size. This is designed for use with variable length sequences. Each
     batch will have a maximum of batch_size arrays, but may have less if
     there are fewer arrays of the same length. It is recommended to use
-    the pad_arrays() method of the LabelledDataset instance before using
+    the `pad_arrays()` method of the `Dataset` instance before using
     this function, in order to quantise the lengths.
 
     Parameters
     ----------
     arrays_x: list of ndarray
         A list of N-D arrays, possibly of different lengths, to batch.
         The assumption is that all the arrays have the same rank and
@@ -468,15 +558,13 @@
             # Array of 1D arrays
             x = np.stack(x)  # type: ignore
         else:
             slices = np.array([len(_x) for _x in x])
             if len(x.shape) == 3:
                 # Contiguous 3D array
                 x = x.reshape(sum(slices), x.shape[2])
-            elif x[0].base is not None and all(_x.base is x[0].base for _x in x):
-                # Array of views into contiguous array
-                x = x[0].base
             else:
-                # Array of separate arrays
+                # Array of arrays. Cannot assume they are contiguous
+                # views into base array, so need to concatenate.
                 x = np.concatenate(x)
     assert sum(slices) == len(x)
     return x, slices
```

### Comparing `ertk-2022.4.0/src/ertk/utils/generic.py` & `ertk-2023.6.0/src/ertk/utils/generic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+"""General utilities."""
+
 from itertools import chain, combinations, permutations, zip_longest
 from typing import (
     Any,
     Callable,
     Container,
     Dict,
     Iterable,
     List,
     Optional,
     Tuple,
     TypeVar,
     overload,
 )
 
+__all__ = [
+    "itmap",
+    "ordered_intersect",
+    "batch_iterable",
+    "filter_kwargs",
+    "subsets",
+    "ordered_subsets",
+]
+
 T = TypeVar("T")
 T1 = TypeVar("T1")
 T2 = TypeVar("T2")
 
 
 def itmap(s: Callable[[T1], T2]):
     """Returns a new map function that additionally maps tuples to
@@ -72,15 +83,15 @@
     """
     return [x for x in a if x in b]
 
 
 def filter_kwargs(kwargs: Dict[str, Any], method: Callable) -> Dict[str, Any]:
     """Removes incompatible keyword arguments. This ignores any
     `**kwargs` catchall in method signature, and only returns args
-    specifically present as keyhwords in the method signature which are
+    specifically present as keywords in the method signature which are
     also not positional only.
 
     Parameters
     ----------
     params: dict
         Keyword arguments to pass to method.
     method: callable
@@ -100,37 +111,48 @@
             key not in meth_params
             or meth_params[key].kind == inspect.Parameter.POSITIONAL_ONLY
         ):
             del kwargs[key]
     return kwargs
 
 
+_BatchSentinel = object()
+
+
 def batch_iterable(
-    it: Iterable[T], batch_size: int, fillvalue: Any = None
+    it: Iterable[T],
+    batch_size: int,
+    return_last: bool = True,
 ) -> Iterable[Tuple[T, ...]]:
     """Batches an iterable into chunks of size `batch_size`.
 
     Parameters
     ----------
     it: iterable
         The iterable to batch.
     batch_size: int
         The size of each batch/chunk.
-    fillvalue:
-        An optional fill value if the final batch isn't full (i.e.
+    return_last: bool
+        Whether to yield the last batch if it isn't full (i.e.
         `batch_size` doesn't divide the iterable length.)
 
     Yields
-    -------
+    ------
     tuple
         A tuple of length `batch_size` with successive elements from the
-        original iterable.
+        original iterable. If `return_last == False` then the last batch
+        is dropped if it contains less than `batch_size` items.
     """
     # From the itertools recipes, to chunk an iterator
-    yield from zip_longest(*[iter(it)] * batch_size, fillvalue=fillvalue)
+    iterables = [iter(it)] * batch_size
+    if return_last:
+        for batch in zip_longest(*iterables, fillvalue=_BatchSentinel):
+            yield tuple(filter(lambda x: x is not _BatchSentinel, batch))
+    else:
+        yield from zip(*iterables)
 
 
 def subsets(it: Iterable[T], max_size: Optional[int] = None) -> Iterable[Tuple[T, ...]]:
     """Iterate over all subsets of the iterable `it`, up to a given
     maximum size. This will generate subsets in size order and then
     index-sorted order (i.e. the order items appear in `it`).
 
@@ -170,10 +192,11 @@
 
     Yields
     ------
     tuple
         The next generated ordered subset.
     """
     if max_size is None:
-        it = list(it)
+        if not hasattr(it, "__len__"):
+            it = list(it)
         max_size = len(it)
     yield from chain(*(permutations(it, i) for i in range(max_size + 1)))
```

