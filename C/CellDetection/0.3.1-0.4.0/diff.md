# Comparing `tmp/CellDetection-0.3.1.tar.gz` & `tmp/CellDetection-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CellDetection-0.3.1.tar", last modified: Thu Apr 14 18:34:17 2022, max compression
+gzip compressed data, was "CellDetection-0.4.0.tar", last modified: Tue Jun  6 13:32:29 2023, max compression
```

## Comparing `CellDetection-0.3.1.tar` & `CellDetection-0.4.0.tar`

### file list

```diff
@@ -1,60 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.490312 CellDetection-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.486312 CellDetection-0.3.1/CellDetection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12317 2022-04-14 18:34:16.000000 CellDetection-0.3.1/CellDetection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-04-14 18:34:17.000000 CellDetection-0.3.1/CellDetection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-14 18:34:17.000000 CellDetection-0.3.1/CellDetection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-14 18:34:17.000000 CellDetection-0.3.1/CellDetection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-14 18:34:17.000000 CellDetection-0.3.1/CellDetection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-14 18:34:03.000000 CellDetection-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-14 18:34:03.000000 CellDetection-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12317 2022-04-14 18:34:17.490312 CellDetection-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11629 2022-04-14 18:34:03.000000 CellDetection-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.486312 CellDetection-0.3.1/celldetection/
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/__meta__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.486312 CellDetection-0.3.1/celldetection/data/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14623 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/cpn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.486312 CellDetection-0.3.1/celldetection/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/datasets/bbbc039.py
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/datasets/bbbc041.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/datasets/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/datasets/synth.py
--rw-r--r--   0 runner    (1001) docker     (121)     9280 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/instance_eval.py
--rw-r--r--   0 runner    (1001) docker     (121)    10493 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/data/toydata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.490312 CellDetection-0.3.1/celldetection/models/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15118 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/commons.py
--rw-r--r--   0 runner    (1001) docker     (121)    44511 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/cpn.py
--rw-r--r--   0 runner    (1001) docker     (121)     5164 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5388 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/fpn.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/mobilenetv3.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    17631 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/models/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.490312 CellDetection-0.3.1/celldetection/mpi/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10045 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/mpi/mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.490312 CellDetection-0.3.1/celldetection/ops/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/ops/boxes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/ops/commons.py
--rw-r--r--   0 runner    (1001) docker     (121)     6936 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/ops/cpn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/ops/draw.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/ops/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.490312 CellDetection-0.3.1/celldetection/util/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12724 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/util/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/util/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)    27352 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 18:34:17.490312 CellDetection-0.3.1/celldetection/visualization/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6514 2022-04-14 18:34:03.000000 CellDetection-0.3.1/celldetection/visualization/images.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-04-14 18:34:03.000000 CellDetection-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-14 18:34:17.490312 CellDetection-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-04-14 18:34:03.000000 CellDetection-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.727982 CellDetection-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.719982 CellDetection-0.4.0/CellDetection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21695 2023-06-06 13:32:29.000000 CellDetection-0.4.0/CellDetection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-06 13:32:29.000000 CellDetection-0.4.0/CellDetection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:32:29.000000 CellDetection-0.4.0/CellDetection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-06 13:32:29.000000 CellDetection-0.4.0/CellDetection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 13:32:29.000000 CellDetection-0.4.0/CellDetection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 13:32:18.000000 CellDetection-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 13:32:18.000000 CellDetection-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21695 2023-06-06 13:32:29.727982 CellDetection-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-06-06 13:32:18.000000 CellDetection-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.719982 CellDetection-0.4.0/celldetection/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/__meta__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.719982 CellDetection-0.4.0/celldetection/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/callbacks/dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.719982 CellDetection-0.4.0/celldetection/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/cpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.723982 CellDetection-0.4.0/celldetection/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/datasets/bbbc038.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/datasets/bbbc039.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/datasets/bbbc041.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/datasets/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/datasets/synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/instance_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/data/toydata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.723982 CellDetection-0.4.0/celldetection/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27393 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76410 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/cpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/manet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/mobilenetv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/ppm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/smp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/timmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37241 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/models/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.723982 CellDetection-0.4.0/celldetection/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/mpi/mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.723982 CellDetection-0.4.0/celldetection/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/ops/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/ops/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/ops/cpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/ops/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/ops/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/ops/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.727982 CellDetection-0.4.0/celldetection/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/optim/lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.727982 CellDetection-0.4.0/celldetection/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/util/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/util/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42675 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:32:29.727982 CellDetection-0.4.0/celldetection/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/visualization/cmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-06-06 13:32:18.000000 CellDetection-0.4.0/celldetection/visualization/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-06 13:32:18.000000 CellDetection-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:32:29.727982 CellDetection-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-06 13:32:18.000000 CellDetection-0.4.0/setup.py
```

### Comparing `CellDetection-0.3.1/LICENSE` & `CellDetection-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/data/cpn.py` & `CellDetection-0.4.0/celldetection/data/cpn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import warnings
 import cv2
 from skimage.measure import regionprops
 from collections import OrderedDict
 from .segmentation import filter_instances_
 
 
 def efd(contour, order=10, epsilon=1e-6):
@@ -63,49 +62,66 @@
     t_diff = np.diff(t ** 2, axis=-1)
     dt2 = 2 * dt
     a0 = (1 / T_) * np.sum(((dxy[..., 0] / dt2) * t_diff) + xi * dt, axis=-1)
     c0 = (1 / T_) * np.sum(((dxy[..., 1] / dt2) * t_diff) + delta * dt, axis=-1)
     return np.array(coefficients), np.stack((contour[..., 0, 0] + a0, contour[..., 0, 1] + c0), axis=-1)
 
 
-def labels2contours(labels, mode=cv2.RETR_EXTERNAL, method=cv2.CHAIN_APPROX_NONE) -> dict:
-    """
+def labels2contours(labels, mode=cv2.RETR_EXTERNAL, method=cv2.CHAIN_APPROX_NONE, flag_fragmented_inplace=False,
+                    raise_fragmented=True, constant=-1) -> dict:
+    """Labels to contours.
+
+    Notes:
+        - If ``flag_fragmented_inplace is True``, ``labels`` may be modified inplace.
 
     Args:
         labels:
         mode:
         method: Contour method. CHAIN_APPROX_NONE must be used if contours are used for CPN.
+        flag_fragmented_inplace: Whether to flag fragmented labels. Flagging sets labels that consist of more than one
+            connected component to ``constant``.
+        constant: Flagging constant.
+        raise_fragmented: Whether to raise ValueError when encountering fragmented labels.
 
     Returns:
-
+        dict
     """
     crops = []
-    contours = OrderedDict({})
+    contours = OrderedDict()
     for channel in np.split(labels, labels.shape[2], 2):
         crops += [(p.label, p.image) + p.bbox[:2] for p in regionprops(channel)]
     for label, crop, oy, ox in crops:
         crop.dtype = np.uint8
         r = cv2.findContours(crop, mode=mode, method=method, offset=(ox, oy))
         if len(r) == 3:  # be compatible with both existing versions of findContours
             _, c, _ = r
         elif len(r) == 2:
             c, _ = r
         else:
             raise NotImplementedError('try different cv2 version')
-        c, = c
+        try:
+            c, = c
+        except ValueError as ve:
+            if flag_fragmented_inplace:
+                labels[labels == label] = constant
+            elif raise_fragmented:
+                raise ValueError('Object labeled with multiple connected components.')
+            continue
         if len(c) == 1:
             c = np.concatenate((c, c), axis=0)  # min len for other functions to work properly
         contours[label] = c
+    if labels.shape[2] > 1:
+        return OrderedDict(sorted(contours.items()))
     return contours
 
 
-def labels2contour_list(labels) -> list:
+def labels2contour_list(labels, **kwargs) -> list:
     if labels.ndim == 2:
         labels = labels[..., None]
-    return [np.squeeze(i, 1) for i in list(labels2contours(labels).values())]
+    return [np.squeeze(i, 1) for i in list(labels2contours(labels, **kwargs).values())]
 
 
 def masks2labels(masks, connectivity=8, label_axis=2, count=False, reduce=np.max, keepdims=True, **kwargs):
     """Masks to labels.
 
     Notes:
         ~ 11.7 ms for Array[25, 256, 256]. For same array skimage.measure.label takes ~ 17.9 ms.
@@ -171,34 +187,67 @@
 
 
 def contours2fourier(contours: dict, order=5, dtype=np.float32):
     if len(contours) > 0:
         max_label = np.max(list(contours.keys()))
     else:
         max_label = 0
+
     fouriers = np.zeros((max_label, order, 4), dtype=dtype)
     locations = np.zeros((max_label, 2), dtype=dtype)
     for key, contour in contours.items():
         if contour.ndim == 3:
             contour = contour.squeeze(1)
         fourier, location = efd(contour, order)
         fouriers[key - 1] = fourier  # labels start at 1, but indices at 0
         locations[key - 1] = location  # labels start at 1, but indices at 0
     return fouriers, locations
 
 
+def contours2boxes(contours):
+    """Contours to boxes.
+
+    Args:
+        contours: Array[num_contours, num_points, 2]. (x, y) format.
+
+    Returns:
+        Array[num_contours, 4]. (x0, y0, x1, y1) format.
+    """
+    if len(contours):
+        boxes = np.concatenate((contours.min(1), contours.max(1)), 1)
+    else:
+        boxes = np.empty((0, 4))
+    return boxes
+
+
 def render_contour(contour, val=1, dtype='int32'):
     xmin, ymin = np.floor(np.min(contour, axis=0)).astype('int')
     xmax, ymax = np.ceil(np.max(contour, axis=0)).astype('int')
     a = np.zeros((ymax - ymin + 1, xmax - xmin + 1), dtype=dtype)
     a = cv2.drawContours(a, [np.array(contour, dtype=np.int32).reshape((-1, 1, 2))], 0, val, -1,
                          offset=(-xmin, -ymin))
     return a, (xmin, xmax), (ymin, ymax)
 
 
+def filter_contours_by_intensity(img, contours, min_intensity=None, max_intensity=200, aggregate='mean'):
+    keep = np.ones(len(contours), dtype=bool)
+    for idx, con in enumerate(contours):
+        m, (xmin, xmax), (ymin, ymax) = render_contour(con, dtype='uint8')
+        img_crop = img[ymin:ymin + m.shape[0], xmin:xmin + m.shape[1]]
+        m = m[:img_crop.shape[0], :img_crop.shape[1]]
+        assert m.dtype == np.uint8
+        m.dtype = bool
+        mean_intensity = getattr(np, aggregate)(img_crop[m])
+        if max_intensity is not None and mean_intensity > max_intensity:
+            keep[idx] = False
+        elif min_intensity is not None and mean_intensity < min_intensity:
+            keep[idx] = False
+    return keep
+
+
 def clip_contour_(contour, size):
     np.clip(contour[..., 0], 0, size[1], out=contour[..., 0])
     np.clip(contour[..., 1], 0, size[0], out=contour[..., 1])
 
 
 def contours2labels(contours, size, rounded=True, clip=True, initial_depth=1, gap=3, dtype='int32'):
     """Contours to labels.
@@ -238,15 +287,15 @@
     return labels
 
 
 def mask_labels_by_distance_(labels, distances, max_bg_dist, min_fg_dist):
     # Set instance labels to 0 if their distance is <= max_bg_dist
     labels[np.logical_and(np.any(labels > 0, 2), distances <= max_bg_dist)] = 0
 
-    # Set all labels to -1 that have have a distance d with `max_bg_dist < d < min_fg_dist`
+    # Set all labels to -1 that have a distance d with `max_bg_dist < d < min_fg_dist`
     labels[np.logical_and(distances > max_bg_dist, distances < min_fg_dist)] = -1
 
 
 def labels2distances(labels, distance_type=cv2.DIST_L2, overlap_zero=True):
     """Label stacks to distances.
 
     Measures distances from pixel to closest border, relative to largest distance.
@@ -283,76 +332,88 @@
             c = p.coords
             indices = (c[:, 0], c[:, 1])
             dist[indices] /= np.maximum(dist[indices].max(), .000001)
     return dist.clip(0., 1.), labels  # 332 µs ± 24.5 µs for (576, 576)
 
 
 class CPNTargetGenerator:
-    def __init__(self, samples, order, random_sampling=True, remove_partials=False, min_fg_dist=.75, max_bg_dist=.5):
+    def __init__(self, samples, order, random_sampling=True, remove_partials=False, min_fg_dist=.75, max_bg_dist=.5,
+                 flag_fragmented=True, flag_fragmented_constant=-1):
         self.samples = samples
         self.order = order
         self.random_sampling = random_sampling
         self.remove_partials = remove_partials
         self.min_fg_dist = min_fg_dist
         self.max_bg_dist = max_bg_dist
+        self.flag_fragmented = flag_fragmented
+        self.flag_fragmented_constant = flag_fragmented_constant
 
         self.labels = None
-        self.reduced_labels = None
         self.distances = None
         self.partials_mask = None
-        self._sampling, self._contours, self._fourier, self._locations, self._sampled_contours = (None,) * 5
+        self._sampling = self._contours = self._fourier = self._locations = self._sampled_contours = None
         self._sampled_sizes = None
         self._reset()
 
     def _reset(self):
         self._sampling = None
         self._contours = None
         self._fourier = None
         self._locations = None
         self._sampled_contours = None
         self._sampled_sizes = None
 
-    def feed(self, labels, border=1):
+    def feed(self, labels, border=1, min_area=1, max_area=None):
         """
 
+        Notes:
+            - May apply inplace changes to ``labels``.
+
         Args:
             labels: Single label image. E.g. of shape (height, width, channels).
-            classes:
             border:
-
+            min_area:
+            max_area:
         """
         if labels.ndim == 2:
             labels = labels[..., None]
 
         filter_instances_(labels, partials=self.remove_partials, partials_border=border,
-                          min_area=5, max_area=None, constant=-1, continuous=True)
+                          min_area=min_area, max_area=max_area, constant=-1, continuous=True)
 
         self.labels = labels
+        _ = self.contours  # compute contours
 
         self.distances, labels = labels2distances(labels)
         mask_labels_by_distance_(labels, self.distances, self.max_bg_dist, self.min_fg_dist)
 
-        self.reduced_labels = labels.max(2)
         self._reset()
 
     @property
+    def reduced_labels(self):
+        if self.flag_fragmented:
+            _ = self.contours  # Since labels2contours may filter instances, it has to be done before returning labels
+        return self.labels.max(2)
+
+    @property
     def sampling(self):
         if self._sampling is None:
             if self.random_sampling:
                 self._sampling = np.random.uniform(0., 1., self.samples)
 
             else:
                 self._sampling = np.linspace(0., 1., self.samples)
             self._sampling.sort()
         return self._sampling
 
     @property
     def contours(self):
         if self._contours is None:
-            self._contours: dict = labels2contours(self.labels)
+            self._contours: dict = labels2contours(self.labels, flag_fragmented_inplace=self.flag_fragmented,
+                                                   constant=self.flag_fragmented_constant, raise_fragmented=False)
         return self._contours
 
     @property
     def fourier(self):
         if self._fourier is None:
             self._fourier, self._locations = contours2fourier(self.contours, order=self.order)
         return self._fourier
```

### Comparing `CellDetection-0.3.1/celldetection/data/datasets/bbbc039.py` & `CellDetection-0.4.0/celldetection/data/datasets/bbbc039.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/data/datasets/bbbc041.py` & `CellDetection-0.4.0/celldetection/data/datasets/bbbc041.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/data/datasets/generic.py` & `CellDetection-0.4.0/celldetection/data/datasets/generic.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/data/datasets/synth.py` & `CellDetection-0.4.0/celldetection/data/datasets/synth.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/data/instance_eval.py` & `CellDetection-0.4.0/celldetection/data/instance_eval.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/data/misc.py` & `CellDetection-0.4.0/celldetection/data/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import torch
 from collections import OrderedDict
 from skimage import img_as_ubyte
 from ..util.util import get_device
+import cv2
 from skimage import measure
 
 __all__ = ['to_tensor', 'transpose_spatial', 'universal_dict_collate_fn', 'normalize_percentile', 'random_crop',
            'channels_last2channels_first', 'channels_first2channels_last', 'ensure_tensor', 'rgb_to_scalar',
            'padding_stack', 'labels2crops', 'rle2mask', 'resample_contours']
 
 
@@ -178,14 +179,28 @@
     )
     results = [(None if v is None else v[slices]) for v in arrays]
     if len(results) == 1:
         results, = results
     return results
 
 
+def random_pad(*arrays, size, mode='constant', **kwargs):
+    if len(arrays) <= 0:
+        return None
+    reference = arrays[0].shape[:len(size)]
+    padding = [max(size[i] - reference[i], 0) for i in range(len(size))]
+    start = [int(np.random.uniform() * p) for p in padding]
+    end = [p - s for p, s in zip(padding, start)]
+    p = [[a, b] for a, b in zip(start, end)]
+    results = [np.pad(i, p + [[0, 0]] * (i.ndim - len(p)), mode=mode, **kwargs) for i in arrays]
+    if len(results) == 1:
+        results, = results
+    return results
+
+
 def rle2mask(code, shape, transpose=True, min_index=1, constant=1) -> np.ndarray:
     """Run length encoding to mask.
 
     Convert run length encoding to mask image.
 
     Args:
         code: Run length code.
@@ -292,7 +307,12 @@
     ts = np.linspace(0, cumsum[..., -1], num + 1, axis=-1)[..., :-1]
     v = ts[..., :, None] <= cumsum[..., None, :]
     idx = np.where(v.max(-1))[:-1] + (np.argmax(v, axis=-1).ravel(),)
     alpha = ((ts - cumsum0[idx].reshape(*ts.shape)) / dt[idx].reshape(*ts.shape))[..., None]
     shape = contours.shape[:-2] + (num, 2)
     sample = contours[idx].reshape(shape) * (1 - alpha) + contours[idx[:-1] + (idx[-1] + 1,)].reshape(shape) * alpha
     return sample
+
+
+def rescale_image(img, scale, **kwargs):
+    target_size = tuple(np.round(np.array(img.shape[:2]) * scale).astype('int'))
+    return cv2.resize(img, target_size[::-1], **kwargs)
```

### Comparing `CellDetection-0.3.1/celldetection/data/toydata.py` & `CellDetection-0.4.0/celldetection/data/toydata.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/models/commons.py` & `CellDetection-0.4.0/celldetection/models/convnext.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,437 +1,362 @@
-import numpy as np
+from torchvision.models.convnext import CNBlockConfig
+from torchvision.models import convnext as cnx
+from typing import List, Optional, Callable, Sequence
 import torch
-import torch.nn as nn
-from torch import Tensor, tanh, sigmoid
-from ..util.util import lookup_nn, tensor_to
-from ..ops.commons import split_spatially, minibatch_std_layer
-from typing import Type
-
-__all__ = ['TwoConvNormRelu', 'ScaledTanh', 'ScaledSigmoid', 'ReplayCache', 'ConvNormRelu', 'ConvNorm',
-           'ResBlock', 'NoAmp', 'ReadOut', 'BottleneckBlock', 'SpatialSplit', 'MinibatchStdLayer']
-
-
-class ConvNorm(nn.Sequential):
-    def __init__(self, in_channels, out_channels, kernel_size=3, padding=1, stride=1, norm_layer=nn.BatchNorm2d,
-                 **kwargs):
-        """ConvNorm.
+from torch import Tensor, nn
+import torch.nn.functional as F
+from functools import partial
+from torchvision.ops import misc, Permute
+from torchvision.ops.stochastic_depth import StochasticDepth
+from ..util.util import lookup_nn
+from .commons import LayerNorm1d, LayerNorm2d, LayerNorm3d, channels_last_permute, channels_first_permute
+from torch.hub import load_state_dict_from_url
+
+__all__ = ['ConvNeXtBase', 'ConvNeXtTiny', 'ConvNeXtSmall', 'ConvNeXtLarge', 'ConvNeXt']
+
+default_model_urls = dict(
+    ConvNeXtLarge=cnx.ConvNeXt_Large_Weights.IMAGENET1K_V1.url,
+    ConvNeXtBase=cnx.ConvNeXt_Base_Weights.IMAGENET1K_V1.url,
+    ConvNeXtSmall=cnx.ConvNeXt_Small_Weights.IMAGENET1K_V1.url,
+    ConvNeXtTiny=cnx.ConvNeXt_Tiny_Weights.IMAGENET1K_V1.url,
+)
+
+
+def map_state_dict(in_channels, current_state_dict, state_dict, nd=2, fused_initial=False):
+    # Only keep params of features branch
+    selection = {k: v for k, v in state_dict.items() if k.startswith('features.')}
+    assert len(selection) == len(current_state_dict), (len(selection), len(current_state_dict))
+    # Rename
+    mapping = {}
+    for a, b in zip(selection, current_state_dict):
+        params = state_dict[a]
+        if b == ('0.0.0.weight' if fused_initial else '0.0.weight') and params.shape[1] != in_channels:
+            params.data = F.interpolate(params.data[None], (in_channels,) + params.data.shape[-nd:]).squeeze(0)
+        mapping[b] = params
+    return mapping
 
-        Just a convolution and a normalization layer.
 
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels.
-            kernel_size: Kernel size.
-            padding: Padding.
-            stride: Stride.
-            norm_layer: Normalization layer (e.g. ``nn.BatchNorm2d``).
-            **kwargs: Additional keyword arguments.
-        """
+class ConvNormActivation(misc.ConvNormActivation):
+    def __init__(
+            self,
+            in_channels: int,
+            out_channels: int,
+            kernel_size: int = 3,
+            stride: int = 1,
+            padding: Optional[int] = None,
+            groups: int = 1,
+            norm_layer: Optional[Callable[..., torch.nn.Module]] = torch.nn.BatchNorm2d,
+            activation_layer: Optional[Callable[..., torch.nn.Module]] = torch.nn.ReLU,
+            dilation: int = 1,
+            inplace: Optional[bool] = True,
+            bias: Optional[bool] = None,
+            nd=2,
+    ) -> None:
         super().__init__(
-            nn.Conv2d(in_channels, out_channels, kernel_size=kernel_size, padding=padding, stride=stride, **kwargs),
-            norm_layer(out_channels),
+            in_channels,
+            out_channels,
+            kernel_size,
+            stride,
+            padding,
+            groups,
+            norm_layer,
+            activation_layer,
+            dilation,
+            inplace,
+            bias,
+            lookup_nn('Conv2d', nd=nd, call=False),
         )
 
 
-class ConvNormRelu(nn.Sequential):
-    def __init__(self, in_channels, out_channels, kernel_size=3, padding=1, stride=1, norm_layer=nn.BatchNorm2d,
-                 activation='relu', **kwargs):
-        """ConvNormReLU.
-
-        Just a convolution, normalization layer and an activation.
-
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels.
-            kernel_size: Kernel size.
-            padding: Padding.
-            stride: Stride.
-            norm_layer: Normalization layer (e.g. ``nn.BatchNorm2d``).
-            activation: Activation function. (e.g. ``nn.ReLU``, ``'relu'``)
-            **kwargs: Additional keyword arguments.
-        """
-        super().__init__(
-            nn.Conv2d(in_channels, out_channels, kernel_size=kernel_size, padding=padding, stride=stride, **kwargs),
+class CNBlock(nn.Module):  # ported from torchvision.models.convnext to support n-dimensions and add more features
+    def __init__(self, in_channels, out_channels=None, layer_scale: float = 1e-6, stochastic_depth_prob: float = 0,
+                 norm_layer: Optional[Callable[..., nn.Module]] = None, activation='gelu', stride: int = 1,
+                 identity_norm_layer=None, nd: int = 2) -> None:
+        super().__init__()
+        if norm_layer is None:
+            norm_layer = partial(nn.LayerNorm, eps=1e-6)
+        Conv = lookup_nn('Conv2d', nd=nd, call=False)
+        out_channels = in_channels if out_channels is None else out_channels
+        self.identity = None
+        if in_channels != out_channels or stride != 1:
+            if identity_norm_layer is None:
+                identity_norm_layer = [LayerNorm1d, LayerNorm2d, LayerNorm3d][nd - 1]
+            self.identity = nn.Sequential(  # following option (b) in He et al. (2015)
+                Conv(out_channels, out_channels, kernel_size=1, stride=stride, bias=False),
+                identity_norm_layer(out_channels)
+            )
+        self.block = nn.Sequential(
+            Conv(in_channels, out_channels, kernel_size=7, padding=3, groups=out_channels, bias=True),
+            Permute(list(channels_last_permute(nd))),
             norm_layer(out_channels),
-            lookup_nn(activation)
-        )
-
-
-class TwoConvNormRelu(nn.Sequential):
-    def __init__(self, in_channels, out_channels, kernel_size=3, padding=1, stride=1, mid_channels=None,
-                 norm_layer=nn.BatchNorm2d, activation='relu', **kwargs):
-        """TwoConvNormReLU.
-
-        A sequence of conv, norm, activation, conv, norm, activation.
-
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels.
-            kernel_size: Kernel size.
-            padding: Padding.
-            stride: Stride.
-            mid_channels: Mid-channels. Default: Same as ``out_channels``.
-            norm_layer: Normalization layer (e.g. ``nn.BatchNorm2d``).
-            activation: Activation function. (e.g. ``nn.ReLU``, ``'relu'``)
-            **kwargs: Additional keyword arguments.
-        """
-        if mid_channels is None:
-            mid_channels = out_channels
-        super().__init__(
-            nn.Conv2d(in_channels, mid_channels, kernel_size=kernel_size, padding=padding, stride=stride, **kwargs),
-            norm_layer(mid_channels),
+            nn.Linear(in_features=out_channels, out_features=4 * out_channels, bias=True),
             lookup_nn(activation),
-            nn.Conv2d(mid_channels, out_channels, kernel_size=kernel_size, padding=padding, **kwargs),
-            norm_layer(out_channels),
-            lookup_nn(activation)
+            nn.Linear(in_features=4 * out_channels, out_features=out_channels, bias=True),
+            Permute(list(channels_first_permute(nd))),
         )
-
-
-class ScaledX(nn.Module):
-    def __init__(self, fn, factor, shift=0.):
-        super().__init__()
-        self.factor = factor
-        self.shift = shift
-        self.fn = fn
+        self.layer_scale = nn.Parameter(torch.ones(out_channels, *(1,) * nd) * layer_scale)
+        self.stochastic_depth = StochasticDepth(stochastic_depth_prob, "row")
 
     def forward(self, inputs: Tensor) -> Tensor:
-        return self.fn(inputs) * self.factor + self.shift
-
-    def extra_repr(self) -> str:
-        return 'factor={}, shift={}'.format(self.factor, self.shift)
-
-
-class ScaledTanh(ScaledX):
-    def __init__(self, factor, shift=0.):
-        """Scaled Tanh.
-
-        Computes the scaled and shifted hyperbolic tangent:
-
-        .. math:: tanh(x) * factor + shift
-
-        Args:
-            factor: Scaling factor.
-            shift: Shifting constant.
-        """
-        super().__init__(tanh, factor, shift)
-
-
-class ScaledSigmoid(ScaledX):
-    def __init__(self, factor, shift=0.):
-        """Scaled Sigmoid.
-
-        Computes the scaled and shifted sigmoid:
-
-        .. math:: sigmoid(x) * factor + shift
-
-        Args:
-            factor: Scaling factor.
-            shift: Shifting constant.
-        """
-        super().__init__(sigmoid, factor, shift)
-
-
-class ReplayCache:
-    def __init__(self, size=128):
-        """Replay Cache.
-
-        Typical cache that can be used for experience replay in GAN training.
-
-        Notes:
-            - Items remain on their current device.
-
-        Args:
-            size: Number of batch items that fit in cache.
-        """
-        self.cache = []
-        self.size = size
-
-    def __len__(self):
-        return len(self.cache)
-
-    def is_empty(self):
-        return len(self) <= 0
-
-    def add(self, x, fraction=.5):
-        """Add.
-
-        Add a ``fraction`` of batch ``x`` to cache.
-        Drop random items if cache is full.
-
-        Args:
-            x: Batch Tensor[n, ...].
-            fraction: Fraction in 0..1.
-
-        """
-        lx = len(x)
-        for i in np.random.choice(np.arange(lx), int(lx * fraction), replace=False):
-            self.cache.append(x[i].detach())
-        while len(self) > self.size:
-            del self.cache[np.random.randint(0, len(self))]
-
-    def __call__(self, num):
-        """Call.
-
-        Args:
-            num: Batch size / number of returned items.
-
-        Returns:
-            Tensor[num, ...]
-        """
-        if self.is_empty():
-            return None
-        return torch.stack([self.cache[i] for i in np.random.randint(0, len(self), num)], 0)
+        identity = inputs if self.identity is None else self.identity(inputs)
+        result = self.layer_scale * self.block(inputs)
+        result = self.stochastic_depth(result)
+        result += identity
+        return result
 
 
-class _ResBlock(nn.Module):
+class ConvNeXt(nn.Sequential):
     def __init__(
             self,
+            in_channels: int,
+            out_channels: int,
+            block_setting: List[CNBlockConfig],
+            stochastic_depth_prob: float = 0.0,
+            layer_scale: float = 1e-6,
+            block: Optional[Callable[..., nn.Module]] = None,
+            block_kwargs: dict = None,
+            norm_layer: Optional[Callable[..., nn.Module]] = None,
+            pretrained=False,
+            fused_initial=True,
+            final_layer=None,
+            nd=2,
+    ):
+        if not block_setting:
+            raise ValueError("The block_setting should not be empty")
+        elif not (isinstance(block_setting, Sequence) and all([isinstance(s, CNBlockConfig) for s in block_setting])):
+            raise TypeError("The block_setting should be List[CNBlockConfig]")
+
+        block_kwargs = {} if block_kwargs is None else block_kwargs
+        if block is None:
+            block = partial(CNBlock, nd=nd)
+
+        if norm_layer is None:
+            norm_layer = partial([LayerNorm1d, LayerNorm2d, LayerNorm3d][nd - 1], eps=1e-6)
+
+        layers: List[nn.Module] = []
+        firstconv_output_channels = block_setting[0].input_channels
+        fi = 1 + (1 - fused_initial)
+        self.out_channels = [firstconv_output_channels] * fi + [s.out_channels for s in block_setting if
+                                                                s.out_channels is not None]
+        num = len([b for b in block_setting if b.out_channels is not None])
+        self.out_strides = [4] * fi + [4 * (2 ** i) for i in range(1, num + 1)]
+
+        Conv = lookup_nn('Conv2d', nd=nd, call=False)
+        initial = ConvNormActivation(
             in_channels,
-            out_channels,
-            block,
-            activation='ReLU',
-            stride=1,
-            downsample=None,
-    ) -> None:
-        super().__init__()
-        downsample = downsample or ConvNorm
-        if in_channels != out_channels or stride != 1:
-            self.downsample = downsample(in_channels, out_channels, 1, stride=stride, bias=False, padding=0)
-        else:
-            self.downsample = nn.Identity()
-        self.block = block
-        self.activation = lookup_nn(activation)
-
-    def forward(self, x: Tensor) -> Tensor:
-        identity = self.downsample(x)
-        out = self.block(x)
-        out += identity
-        return self.activation(out)
+            firstconv_output_channels,
+            kernel_size=4,
+            stride=4,
+            padding=0,
+            norm_layer=norm_layer,
+            activation_layer=None,
+            bias=True,
+            nd=nd
+        )
+        if not fused_initial:
+            layers.append(initial)
+            initial = None
+
+        total_stage_blocks = sum(cnf.num_layers for cnf in block_setting)
+        stage_block_id = 0
+        down = cnf = None
+        for cnf in block_setting:
+            # Bottlenecks
+            stage: List[nn.Module] = []
+            if initial is not None:
+                stage += [initial]  # fused initial
+                initial = None
+            if down is not None:
+                stage += [down]  # downsampling is part of the stage
+            for _ in range(cnf.num_layers):
+                sd_prob = stochastic_depth_prob * stage_block_id / (total_stage_blocks - 1.0)
+                stage.append(block(cnf.input_channels, layer_scale=layer_scale, stochastic_depth_prob=sd_prob,
+                                   **block_kwargs))
+                stage_block_id += 1
+            layers.append(nn.Sequential(*stage))
+            if cnf.out_channels is not None:
+                # Downsampling
+                down = nn.Sequential(
+                    norm_layer(cnf.input_channels),
+                    Conv(cnf.input_channels, cnf.out_channels, kernel_size=2, stride=2),
+                )
+
+        if out_channels or final_layer is not None:
+
+            if final_layer is None:
+                final_layer = Conv(cnf.out_channels or cnf.input_channels, out_channels, 1)
+            layers.append(final_layer)
+        super().__init__(*layers)
+
+        for m in self.modules():
+            if isinstance(m, (nn.modules.conv._ConvNd, nn.Linear)):
+                nn.init.trunc_normal_(m.weight, std=0.02)
+                if m.bias is not None:
+                    nn.init.zeros_(m.bias)
+
+        if pretrained:
+            if isinstance(pretrained, str):
+                state_dict = load_state_dict_from_url(pretrained)
+                if '.pytorch.org' in pretrained:
+                    state_dict = map_state_dict(in_channels, self.state_dict(), state_dict, nd=nd,
+                                                fused_initial=fused_initial)
+                self.load_state_dict(state_dict)
+            else:
+                raise ValueError('There is no default set of weights for this model. '
+                                 'Please specify a URL using the `pretrained` argument.')
 
 
-class ResBlock(_ResBlock):
+class ConvNeXtTiny(ConvNeXt):
     def __init__(
             self,
-            in_channels,
-            out_channels,
-            kernel_size=3,
-            padding=1,
-            norm_layer='BatchNorm2d',
-            activation='ReLU',
-            stride=1,
-            downsample=None,
+            in_channels: int = 3,
+            out_channels: int = 0,
+            stochastic_depth_prob: float = .1,
+            pretrained: bool = False,
+            nd: int = 2,
             **kwargs
-    ) -> None:
-        """ResBlock.
-
-        Typical ResBlock with variable kernel size and an included mapping of the identity to correct dimensions.
+    ):
+        """ContNeXt Tiny.
 
         References:
-            - https://doi.org/10.1109/CVPR.2016.90
-
-        Notes:
-            - Similar to ``torchvision.models.resnet.BasicBlock``, with different interface and defaults.
-            - Consistent with standard signature ``in_channels, out_channels, kernel_size, ...``.
+            - https://arxiv.org/abs/2201.03545
 
         Args:
             in_channels: Input channels.
-            out_channels: Output channels.
-            kernel_size: Kernel size.
-            padding: Padding.
-            norm_layer: Norm layer.
-            activation: Activation.
-            stride: Stride.
-            downsample: Downsample module that maps identity to correct dimensions. Default is an optionally strided
-                1x1 Conv2d with BatchNorm2d, as per He et al. (2015) (`3.3. Network Architectures`, `Residual Network`,
-                "option (B)").
-            **kwargs: Keyword arguments for Conv2d layers.
+            out_channels: Output channels. If set to ``0``, the output layer is omitted.
+            stochastic_depth_prob: Stochastic depth probability.
+                Base probability of randomly dropping residual connections. Actual probability in blocks is given by
+                ``stochastic_depth_prob * stage_block_id / (total_stage_blocks - 1.0)``.
+            pretrained: Whether to use pretrained weights. By default, weights from ``torchvision`` are used.
+            nd: Number of spatial dimensions.
+            **kwargs: Additional keyword arguments.
         """
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ConvNeXtTiny']
         super().__init__(
-            in_channels, out_channels,
-            block=nn.Sequential(
-                nn.Conv2d(in_channels, out_channels, kernel_size=kernel_size, padding=padding, bias=False,
-                          stride=stride, **kwargs),
-                lookup_nn(norm_layer, out_channels),
-                lookup_nn(activation),
-                nn.Conv2d(out_channels, out_channels, kernel_size=kernel_size, padding=padding, bias=False, **kwargs),
-                lookup_nn(norm_layer, out_channels)
-            ),
-            activation=activation, stride=stride, downsample=downsample
+            in_channels=in_channels,
+            out_channels=out_channels,
+            block_setting=[
+                CNBlockConfig(96, 192, 3),
+                CNBlockConfig(192, 384, 3),
+                CNBlockConfig(384, 768, 9),
+                CNBlockConfig(768, None, 3),
+            ],
+            stochastic_depth_prob=stochastic_depth_prob,
+            pretrained=pretrained,
+            nd=nd,
+            **kwargs
         )
 
 
-class BottleneckBlock(_ResBlock):
+class ConvNeXtSmall(ConvNeXt):
     def __init__(
             self,
-            in_channels,
-            out_channels,
-            kernel_size=3,
-            padding=1,
-            mid_channels=None,
-            compression=4,
-            base_channels=64,
-            norm_layer='BatchNorm2d',
-            activation='ReLU',
-            stride=1,
-            downsample=None,
+            in_channels: int = 3,
+            out_channels: int = 0,
+            stochastic_depth_prob: float = .1,
+            pretrained: bool = False,
+            nd: int = 2,
             **kwargs
-    ) -> None:
-        """Bottleneck Block.
+    ):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ConvNeXtSmall']
+        super().__init__(
+            in_channels=in_channels,
+            out_channels=out_channels,
+            block_setting=[
+                CNBlockConfig(96, 192, 3),
+                CNBlockConfig(192, 384, 3),
+                CNBlockConfig(384, 768, 27),
+                CNBlockConfig(768, None, 3),
+            ],
+            stochastic_depth_prob=stochastic_depth_prob,
+            pretrained=pretrained,
+            nd=nd,
+            **kwargs
+        )
 
-        Typical Bottleneck Block with variable kernel size and an included mapping of the identity to correct
-        dimensions.
+    __init__.__doc__ = ConvNeXtTiny.__init__.__doc__.replace('ContNeXt Tiny.', 'ContNeXt Small.')
 
-        References:
-            - https://doi.org/10.1109/CVPR.2016.90
-            - https://catalog.ngc.nvidia.com/orgs/nvidia/resources/resnet_50_v1_5_for_pytorch
 
-        Notes:
-            - Similar to ``torchvision.models.resnet.Bottleneck``, with different interface and defaults.
-            - Consistent with standard signature ``in_channels, out_channels, kernel_size, ...``.
-            - Stride handled in bottleneck.
+class ConvNeXtBase(ConvNeXt):
+    def __init__(
+            self,
+            in_channels: int = 3,
+            out_channels: int = 0,
+            stochastic_depth_prob: float = .1,
+            pretrained: bool = False,
+            nd: int = 2,
+            **kwargs
+    ):
+        """ContNeXt Base.
 
         Args:
             in_channels: Input channels.
-            out_channels: Output channels.
-            kernel_size: Kernel size.
-            padding: Padding.
-            mid_channels:
-            compression: Compression rate of the bottleneck. The default 4 compresses 256 channels to 64=256/4.
-            base_channels: Minimum number of ``mid_channels``.
-            norm_layer: Norm layer.
-            activation: Activation.
-            stride: Stride.
-            downsample: Downsample module that maps identity to correct dimensions. Default is an optionally strided
-                1x1 Conv2d with BatchNorm2d, as per He et al. (2015) (`3.3. Network Architectures`, `Residual Network`,
-                "option (B)").
-            **kwargs: Keyword arguments for Conv2d layers.
+            out_channels: Output channels. If set to ``0``, the output layer is omitted.
+            stochastic_depth_prob: Stochastic depth probability.
+                Base probability of randomly dropping residual connections. Actual probability in blocks is given by
+                ``stochastic_depth_prob * stage_block_id / (total_stage_blocks - 1.0)``.
+            pretrained: Whether to use pretrained weights. By default, weights from ``torchvision`` are used.
+            nd: Number of spatial dimensions.
+            **kwargs: Additional keyword arguments.
         """
-        mid_channels = mid_channels or np.max([base_channels, out_channels // compression, in_channels // compression])
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ConvNeXtBase']
         super().__init__(
-            in_channels, out_channels,
-            block=nn.Sequential(
-                nn.Conv2d(in_channels, mid_channels, kernel_size=1, padding=0, bias=False, **kwargs),
-                lookup_nn(norm_layer, mid_channels),
-                lookup_nn(activation),
-
-                nn.Conv2d(mid_channels, mid_channels, kernel_size=kernel_size, padding=padding, bias=False,
-                          stride=stride, **kwargs),
-                lookup_nn(norm_layer, mid_channels),
-                lookup_nn(activation),
-
-                nn.Conv2d(mid_channels, out_channels, kernel_size=1, padding=0, bias=False, **kwargs),
-                lookup_nn(norm_layer, out_channels)
-            ),
-            activation=activation, stride=stride, downsample=downsample
+            in_channels=in_channels,
+            out_channels=out_channels,
+            block_setting=[
+                CNBlockConfig(128, 256, 3),
+                CNBlockConfig(256, 512, 3),
+                CNBlockConfig(512, 1024, 27),
+                CNBlockConfig(1024, None, 3),
+            ],
+            stochastic_depth_prob=stochastic_depth_prob,
+            pretrained=pretrained,
+            nd=nd,
+            **kwargs
         )
 
+    __init__.__doc__ = ConvNeXtTiny.__init__.__doc__.replace('ContNeXt Tiny.', 'ContNeXt Base.')
 
-class NoAmp(nn.Module):
-    def __init__(self, module: Type[nn.Module]):
-        """No AMP.
-
-        Wrap a ``Module`` object and disable ``torch.cuda.amp.autocast`` during forward pass if it is enabled.
-
-        Examples:
-            >>> import celldetection as cd
-            ... model = cd.models.CpnU22(1)
-            ... # Wrap all ReadOut modules in model with NoAmp, thus disabling autocast for those modules
-            ... cd.wrap_module_(model, cd.models.ReadOut, cd.models.NoAmp)
 
-        Args:
-            module: Module.
-        """
-        super().__init__()
-        self.module = module
-
-    def forward(self, *args, **kwargs):
-        if torch.is_autocast_enabled():
-            with torch.cuda.amp.autocast(enabled=False):
-                result = self.module(*tensor_to(args, torch.float32), **tensor_to(kwargs, torch.float32))
-        else:
-            result = self.module(*args, **kwargs)
-        return result
-
-
-class ReadOut(nn.Module):
+class ConvNeXtLarge(ConvNeXt):
     def __init__(
             self,
-            channels_in,
-            channels_out,
-            kernel_size=3,
-            padding=1,
-            activation='relu',
-            norm='batchnorm2d',
-            final_activation=None,
-            dropout=0.1,
-            channels_mid=None,
-            stride=1
+            in_channels: int = 3,
+            out_channels: int = 0,
+            stochastic_depth_prob: float = .1,
+            pretrained: bool = False,
+            nd: int = 2,
+            **kwargs
     ):
-        super().__init__()
-        self.channels_out = channels_out
-        if channels_mid is None:
-            channels_mid = channels_in
-
-        self.block = nn.Sequential(
-            nn.Conv2d(channels_in, channels_mid, kernel_size, padding=padding, stride=stride),
-            lookup_nn(norm, channels_mid),
-            lookup_nn(activation),
-            nn.Dropout2d(p=dropout) if dropout else nn.Identity(),
-            nn.Conv2d(channels_mid, channels_out, 1),
-        )
-
-        if final_activation is ...:
-            self.activation = lookup_nn(activation)
-        else:
-            self.activation = lookup_nn(final_activation)
-
-    def forward(self, x):
-        out = self.block(x)
-        return self.activation(out)
-
-
-class SpatialSplit(nn.Module):
-    def __init__(self, height, width=None):
-        """Spatial split.
-
-        Splits spatial dimensions of input Tensor into patches of size ``(height, width)`` and adds the patches
-        to the batch dimension.
-
-        Args:
-            height: Patch height.
-            width: Patch width.
-        """
-        super().__init__()
-        self.height = height
-        self.width = width or height
-
-    def forward(self, x):
-        return split_spatially(x, self.height, self.width)
-
-
-class MinibatchStdLayer(torch.nn.Module):
-    def __init__(self, channels=1, group_channels=None, epsilon=1e-8):
-        """Minibatch standard deviation layer.
-
-        The minibatch standard deviation layer first splits the batch dimension into slices of size ``group_channels``.
-        The channel dimension is split into ``channels`` slices. For the groups the standard deviation is calculated and
-        averaged over spatial dimensions and channel slice depth. The result is broadcasted to the spatial dimensions,
-        repeated for the batch dimension and then concatenated to the channel dimension of ``x``.
-
-        References:
-            - https://arxiv.org/pdf/1710.10196.pdf
+        """ContNeXt Large.
 
         Args:
-            channels: Number of averaged standard deviation channels.
-            group_channels: Number of channels per group. Default: batch size.
-            epsilon: Epsilon.
+            in_channels: Input channels.
+            out_channels: Output channels. If set to ``0``, the output layer is omitted.
+            stochastic_depth_prob: Stochastic depth probability.
+                Base probability of randomly dropping residual connections. Actual probability in blocks is given by
+                ``stochastic_depth_prob * stage_block_id / (total_stage_blocks - 1.0)``.
+            pretrained: Whether to use pretrained weights. By default, weights from ``torchvision`` are used.
+            nd: Number of spatial dimensions.
+            **kwargs: Additional keyword arguments.
         """
-        super().__init__()
-        self.channels = channels
-        self.group_channels = group_channels
-        self.epsilon = epsilon
-
-    def forward(self, x):
-        return minibatch_std_layer(x, self.channels, self.group_channels, epsilon=self.epsilon)
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ConvNeXtLarge']
+        super().__init__(
+            in_channels=in_channels,
+            out_channels=out_channels,
+            block_setting=[
+                CNBlockConfig(192, 384, 3),
+                CNBlockConfig(384, 768, 3),
+                CNBlockConfig(768, 1536, 27),
+                CNBlockConfig(1536, None, 3),
+            ],
+            stochastic_depth_prob=stochastic_depth_prob,
+            pretrained=pretrained,
+            nd=nd,
+            **kwargs
+        )
 
-    def extra_repr(self) -> str:
-        return f'channels={self.channels}, group_channels={self.group_channels}'
+    __init__.__doc__ = ConvNeXtTiny.__init__.__doc__.replace('ContNeXt Tiny.', 'ContNeXt Large.')
```

### Comparing `CellDetection-0.3.1/celldetection/models/inference.py` & `CellDetection-0.4.0/celldetection/models/inference.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/models/mobilenetv3.py` & `CellDetection-0.4.0/celldetection/models/mobilenetv3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import torch.nn as nn
 from torchvision.models.mobilenetv3 import InvertedResidualConfig, InvertedResidual, _mobilenet_v3_conf
-from torchvision.models.mobilenetv2 import ConvBNActivation
 from typing import Any, Callable, List, Optional, Sequence
 from functools import partial
 
+try:
+    from torchvision.ops.misc import Conv2dNormActivation as ConvBNActivation
+except ImportError:
+    from torchvision.models.mobilenetv2 import ConvBNActivation  # for older versions
+
 __all__ = ['MobileNetV3Large', 'MobileNetV3Small']
 
 
 def init_modules_(mod: nn.Module):
     for m in mod.modules():
         if isinstance(m, nn.Conv2d):
             nn.init.kaiming_normal_(m.weight, mode='fan_out')
@@ -42,21 +46,24 @@
 
         if block is None:
             block = InvertedResidual
         if norm_layer is None:
             norm_layer = partial(nn.BatchNorm2d, eps=0.001, momentum=0.01)
 
         layers: List[nn.Sequential] = [nn.Sequential()]
+        cbna_kw = {}  # needed because torchvision changed behaviour
+        if norm_layer is not None:
+            cbna_kw['norm_layer'] = norm_layer
 
         # building first layer
         firstconv_output_channels = inverted_residual_setting[0].input_channels
         self.out_channels = [firstconv_output_channels]
         layers[-1].add_module(str(len(layers[-1])),
                               ConvBNActivation(in_channels, firstconv_output_channels, kernel_size=3, stride=2,
-                                               norm_layer=norm_layer, activation_layer=nn.Hardswish))
+                                               activation_layer=nn.Hardswish, **cbna_kw))
 
         # building inverted residual blocks
         for cnf in inverted_residual_setting:
             if cnf.stride > 1:
                 layers.append(nn.Sequential())
                 self.out_channels.append(cnf.out_channels)
             else:
@@ -66,15 +73,15 @@
         # building last several layers
         lastconv_input_channels = inverted_residual_setting[-1].out_channels
         lastconv_output_channels = 6 * lastconv_input_channels
         self.out_channels[-1] = lastconv_output_channels
         assert len(self.out_channels) == len(layers)
         layers[-1].add_module(str(len(layers[-1])),
                               ConvBNActivation(lastconv_input_channels, lastconv_output_channels, kernel_size=1,
-                                               norm_layer=norm_layer, activation_layer=nn.Hardswish))
+                                               activation_layer=nn.Hardswish, **cbna_kw))
 
         super().__init__(*layers)
         init_modules_(self)
 
 
 class MobileNetV3Large(MobileNetV3Base):
     def __init__(self, in_channels, width_mult: float = 1.0, reduced_tail: bool = False, dilated: bool = False):
```

### Comparing `CellDetection-0.3.1/celldetection/models/normalization.py` & `CellDetection-0.4.0/celldetection/models/normalization.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/models/unet.py` & `CellDetection-0.4.0/celldetection/models/resnet.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,393 +1,412 @@
-import torch
-import torch.nn as nn
-from torch import Tensor
+from torch import nn
 from torch.nn import functional as F
-from torchvision.models._utils import IntermediateLayerGetter
-from torchvision.ops.feature_pyramid_network import FeaturePyramidNetwork
-from collections import OrderedDict
-from typing import List, Dict, Type
-from .commons import TwoConvNormRelu, ResBlock
-from .resnet import *
-from .mobilenetv3 import *
-from ..util.util import lookup_nn
-
-__all__ = [
-    'UNetEncoder', 'UNet', 'U12', 'U17', 'U22', 'SlimU22', 'WideU22', 'MobileNetV3SmallUNet', 'MobileNetV3LargeUNet',
-    'ResNet18UNet', 'ResNet34UNet', 'ResNet50UNet', 'ResNet101UNet', 'ResNet152UNet', 'ResNeXt50UNet', 'ResNeXt101UNet',
-    'ResNeXt152UNet', 'WideResNet50UNet', 'WideResNet101UNet', 'ResUNet'
-]
-
-
-class UNetEncoder(nn.Sequential):
-    def __init__(self, in_channels, depth=5, base_channels=64, factor=2, pool=True, block_cls: Type[nn.Module] = None):
-        """U-Net Encoder.
+from torchvision.models import resnet as tvr
+from ..util.util import Dict, lookup_nn, get_nd_conv
+from torch.hub import load_state_dict_from_url
+from .ppm import append_pyramid_pooling_
+from typing import Type, Union, Optional
+
+__all__ = ['get_resnet', 'ResNet50', 'ResNet34', 'ResNet18', 'ResNet152', 'ResNet101', 'WideResNet101_2',
+           'WideResNet50_2', 'ResNeXt152_32x8d', 'ResNeXt101_32x8d', 'ResNeXt50_32x4d']
+
+default_model_urls = {
+    'ResNet18': 'https://download.pytorch.org/models/resnet18-f37072fd.pth',  # IMAGENET1K_V1
+    'ResNet34': 'https://download.pytorch.org/models/resnet34-b627a593.pth',  # IMAGENET1K_V1
+    'ResNet50': 'https://download.pytorch.org/models/resnet50-11ad3fa6.pth',  # IMAGENET1K_V2
+    'ResNet101': 'https://download.pytorch.org/models/resnet101-cd907fc2.pth',  # IMAGENET1K_V2
+    'ResNet152': 'https://download.pytorch.org/models/resnet152-f82ba261.pth',  # IMAGENET1K_V2
+    'ResNeXt50_32x4d': 'https://download.pytorch.org/models/resnext50_32x4d-1a0047aa.pth',  # IMAGENET1K_V2
+    'ResNeXt101_32x8d': 'https://download.pytorch.org/models/resnext101_32x8d-8ba56ff5.pth',  # IMAGENET1K_V2
+    'WideResNet50_2': 'https://download.pytorch.org/models/wide_resnet50_2-9ba9bcbe.pth',  # IMAGENET1K_V2
+    'WideResNet101_2': 'https://download.pytorch.org/models/wide_resnet101_2-d733dc28.pth',  # IMAGENET1K_V2
+}
+
+
+def conv3x3(in_planes: int, out_planes: int, stride: int = 1, groups: int = 1, dilation: int = 1,
+            nd=2) -> nn.Conv2d:
+    """3x3 convolution with padding"""
+    return get_nd_conv(nd)(
+        in_planes,
+        out_planes,
+        kernel_size=3,
+        stride=stride,
+        padding=dilation,
+        groups=groups,
+        bias=False,
+        dilation=dilation,
+    )
+
+
+def conv1x1(in_planes: int, out_planes: int, stride: int = 1, nd=2) -> nn.Conv2d:
+    """1x1 convolution"""
+    return get_nd_conv(nd)(in_planes, out_planes, kernel_size=1, stride=stride, bias=False)
+
+
+class BasicBlock(nn.Module):
+    expansion: int = tvr.BasicBlock.expansion
+    forward = tvr.BasicBlock.forward
 
-        Args:
-            in_channels: Input channels.
-            depth: Model depth.
-            base_channels: Base channels.
-            factor: Growth factor of base_channels.
-            pool: Whether to use max pooling or stride 2 for downsampling.
-            block_cls: Block class. Callable as `block_cls(in_channels, out_channels, stride=stride)`.
-        """
-        block_cls = block_cls or TwoConvNormRelu
-        layers = []
-        self.out_channels = []
-        for i in range(depth):
-            in_c = base_channels * int(factor ** (i - 1)) * int(i > 0) + int(i <= 0) * in_channels
-            out_c = base_channels * (factor ** i)
-            self.out_channels.append(out_c)
-            block = block_cls(in_c, out_c, stride=int((not pool and i > 0) + 1))
-            if i > 0 and pool:
-                block = nn.Sequential(nn.MaxPool2d(2, stride=2), block)
-            layers.append(block)
-        super().__init__(*layers)
-
-
-class GeneralizedUNet(FeaturePyramidNetwork):
-    def __init__(
+    def __init__(  # Port from torchvision (to support 3d and add more features)
             self,
-            in_channels_list,
-            out_channels: int,
-            block_cls: nn.Module,
-            final_activation=None
-    ):
-        super().__init__([], 0)
-        self.out_channels = out_channels
-        for j, in_channels in enumerate(in_channels_list):
-            if in_channels == 0:
-                raise ValueError("in_channels=0 is currently not supported")
-            oc = out_channels if j <= 0 else in_channels_list[j - 1]
-            inner_block_module = nn.Identity() if oc <= 0 else nn.Conv2d(in_channels, oc, (1, 1))
-            self.inner_blocks.append(inner_block_module)
-            if j <= 0 or oc <= 0:
-                layer_block_module = nn.Identity()
-            else:
-                layer_block_module = block_cls(in_channels, oc)
-            self.layer_blocks.append(layer_block_module)
+            inplanes: int,
+            planes: int,
+            stride: int = 1,
+            downsample: Optional[nn.Module] = None,
+            groups: int = 1,
+            base_width: int = 64,
+            dilation: int = 1,
+            norm_layer='batchnorm2d',
+            nd=2
+    ) -> None:
+        super().__init__()
+        norm_layer = lookup_nn(norm_layer, call=False, nd=nd)
+        if groups != 1 or base_width != 64:
+            raise ValueError("BasicBlock only supports groups=1 and base_width=64")
+        if dilation > 1:
+            raise NotImplementedError("Dilation > 1 not supported in BasicBlock")
+        self.conv1 = conv3x3(inplanes, planes, stride, nd=nd)
+        self.bn1 = norm_layer(planes)
+        self.relu = nn.ReLU(inplace=True)
+        self.conv2 = conv3x3(planes, planes, nd=nd)
+        self.bn2 = norm_layer(planes)
+        self.downsample = downsample
+        self.stride = stride
+
+
+class Bottleneck(nn.Module):
+    expansion: int = tvr.Bottleneck.expansion
+    forward = tvr.Bottleneck.forward
 
-        # initialize parameters now to avoid modifying the initialization of top_blocks
-        for m in self.children():
-            if isinstance(m, nn.Conv2d):
-                nn.init.kaiming_uniform_(m.weight, a=1)
-                nn.init.constant_(m.bias, 0)
-        self.final_activation = lookup_nn(final_activation)
-
-    def forward(self, x: Dict[str, Tensor], size: List[int]) -> Dict[str, Tensor]:
-        """
-
-        Args:
-            x: Input dictionary. E.g. {
-                    0: Tensor[1, 64, 128, 128]
-                    1: Tensor[1, 128, 64, 64]
-                    2: Tensor[1, 256, 32, 32]
-                    3: Tensor[1, 512, 16, 16]
-                }
-            size: Desired final output size. If set to None output remains as it is.
-
-        Returns:
-            Output dictionary. For each key in `x` a corresponding output is returned; the final output
-            has the key `'out'`.
-            E.g. {
-                out: Tensor[1, 2, 128, 128]
-                0: Tensor[1, 64, 128, 128]
-                1: Tensor[1, 128, 64, 64]
-                2: Tensor[1, 256, 32, 32]
-                3: Tensor[1, 512, 16, 16]
-            }
-        """
-        # unpack OrderedDict into two lists for easier handling
-        names = list(x.keys())
-        x = list(x.values())
-        last_inner = x[-1]
-        results = [last_inner]
-        idx = -1
-        for idx in range(len(x) - 2, -1, -1):
-            inner_lateral = x[idx]
-            feat_shape = inner_lateral.shape[-2:]
-            inner_top_down = F.interpolate(last_inner, size=feat_shape, mode="nearest")  # adjust size
-            inner_top_down = self.get_result_from_inner_blocks(inner_top_down, idx + 1)  # reduce channels
-            last_inner = torch.cat((inner_lateral, inner_top_down), 1)  # concat
-            last_inner = self.get_result_from_layer_blocks(last_inner, idx + 1)  # apply layer
-            results.insert(0, last_inner)
-
-        if self.extra_blocks is not None:
-            results, names = self.extra_blocks(results, x, names)
-        if size is None:
-            final = results[0]
-        else:
-            final = F.interpolate(last_inner, size=size, mode="bilinear", align_corners=False)
-        final = self.get_result_from_inner_blocks(final, idx)
-        final = self.final_activation(final)
-        if self.out_channels:
-            return final
-        results.insert(0, final)
-        names.insert(0, 'out')
-        out = OrderedDict([(k, v) for k, v in zip(names, results)])
-        return out
-
-
-class BackboneAsUNet(nn.Module):
-    def __init__(self, backbone, return_layers, in_channels_list, out_channels, block, final_activation=None):
-        super(BackboneAsUNet, self).__init__()
-        block = block or TwoConvNormRelu
-        self.body = IntermediateLayerGetter(backbone, return_layers=return_layers)
-        self.unet = GeneralizedUNet(
-            in_channels_list=in_channels_list,
-            out_channels=out_channels,
-            block_cls=block,
-            # extra_blocks=LastLevelMaxPool(),
-            final_activation=final_activation
+    def __init__(  # Port from torchvision (to support 3d and add more features)
+            self,
+            inplanes: int,
+            planes: int,
+            stride: int = 1,
+            downsample: Optional[nn.Module] = None,
+            groups: int = 1,
+            base_width: int = 64,
+            dilation: int = 1,
+            norm_layer='batchnorm2d',
+            nd=2
+    ) -> None:
+        super().__init__()
+        norm_layer = lookup_nn(norm_layer, call=False, nd=nd)
+        width = int(planes * (base_width / 64.0)) * groups
+        self.conv1 = conv1x1(inplanes, width, nd=nd)
+        self.bn1 = norm_layer(width)
+        self.conv2 = conv3x3(width, width, stride, groups, dilation, nd=nd)
+        self.bn2 = norm_layer(width)
+        self.conv3 = conv1x1(width, planes * self.expansion, nd=nd)
+        self.bn3 = norm_layer(planes * self.expansion)
+        self.relu = nn.ReLU(inplace=True)
+        self.downsample = downsample
+        self.stride = stride
+
+
+def _make_layer(  # Port from torchvision (to support 3d)
+        self,
+        block: Type[Union[BasicBlock, Bottleneck]],
+        planes: int,
+        blocks: int,
+        stride: int = 1,
+        dilate: bool = False,
+        nd=2,
+) -> nn.Sequential:
+    norm_layer = self._norm_layer
+    downsample = None
+    previous_dilation = self.dilation
+    if dilate:
+        self.dilation *= stride
+        stride = 1
+    if stride != 1 or self.inplanes != planes * block.expansion:
+        downsample = nn.Sequential(
+            conv1x1(self.inplanes, planes * block.expansion, stride, nd=nd),
+            norm_layer(planes * block.expansion),
         )
-        self.out_channels = list(in_channels_list)
-
-    def forward(self, inputs):
-        x = self.body(inputs)
-        x = self.unet(x, size=inputs.shape[-2:])
-        return x
-
-
-class UNet(BackboneAsUNet):
-    def __init__(self, backbone, out_channels: int, return_layers: dict = None,
-                 block: Type[nn.Module] = TwoConvNormRelu, final_activation=None):
-        """U-Net.
-
-        Examples:
-            >>> model = UNet(UNetEncoder(in_channels=3), out_channels=2)
-
-            >>> model = UNet(UNetEncoder(in_channels=3, base_channels=16), out_channels=2)
-            >>> o = model(torch.rand(1, 3, 256, 256))
-            >>> for k, v in o.items():
-            ...     print(k, "\t", v.shape)
-            out 	 torch.Size([1, 2, 256, 256])
-            0 	 torch.Size([1, 16, 256, 256])
-            1 	 torch.Size([1, 32, 128, 128])
-            2 	 torch.Size([1, 64, 64, 64])
-            3 	 torch.Size([1, 128, 32, 32])
-            4 	 torch.Size([1, 256, 16, 16])
 
-        Args:
-            backbone: Backbone instance.
-            out_channels: Output channels.
-            return_layers: Dictionary like `{backbone_layer_name: out_name}`.
-                Note that this influences how outputs are computed, as the input for the upsampling
-                is gathered by `IntermediateLayerGetter` based on given dict keys.
-            block: Module class. Default is `block=TwoConvNormRelu`. Must be callable: block(in_channels, out_channels).
-            final_activation: Final activation function.
-        """
-        names = [name for name, _ in backbone.named_children()]  # assuming ordered
-        if return_layers is None:
-            return_layers = {n: str(i) for i, n in enumerate(names)}
-        layers = {str(k): (str(names[v]) if isinstance(v, int) else str(v)) for k, v in return_layers.items()}
-        super(UNet, self).__init__(
-            backbone=backbone,
-            return_layers=layers,
-            in_channels_list=list(backbone.out_channels),
-            out_channels=out_channels,
-            block=block,
-            final_activation=final_activation if out_channels else None
+    layers = []
+    layers.append(
+        block(self.inplanes, planes, stride, downsample, self.groups, self.base_width, previous_dilation, norm_layer,
+              nd=nd))
+    self.inplanes = planes * block.expansion
+    for _ in range(1, blocks):
+        layers.append(block(
+            self.inplanes,
+            planes,
+            groups=self.groups,
+            base_width=self.base_width,
+            dilation=self.dilation,
+            norm_layer=norm_layer,
+            nd=nd,
+        ))
+    return nn.Sequential(*layers)
+
+
+def make_res_layer(block, inplanes, planes, blocks, norm_layer=nn.BatchNorm2d, base_width=64, groups=1, stride=1,
+                   dilation=1, dilate=False, nd=2, **kwargs) -> nn.Module:
+    """
+
+    Args:
+        block: Module class. For example `BasicBlock` or `Bottleneck`.
+        inplanes: Number of in planes
+        planes: Number of planes
+        blocks: Number of blocks
+        norm_layer: Norm Module class
+        base_width: Base width. Acts as a factor of the bottleneck size of the Bottleneck block and is used with groups.
+        groups:
+        stride:
+        dilation:
+        dilate:
+
+    Returns:
+
+    """
+    norm_layer = lookup_nn(norm_layer, nd=nd, call=False)
+    d = Dict(inplanes=inplanes, _norm_layer=norm_layer, base_width=base_width,
+             groups=groups, dilation=dilation)  # almost a ResNet
+
+    return _make_layer(self=d, block=block, planes=planes, blocks=blocks, stride=stride, dilate=dilate, nd=nd)
+
+
+def _apply_mapping_rules(key, rules: dict):
+    for prefix, repl in rules.items():
+        if key.startswith(prefix):
+            key = key.replace(prefix, repl, 1)
+    return key
+
+
+def map_state_dict(in_channels, state_dict, fused_initial):
+    """Map state dict.
+
+    Map state dict from torchvision format to celldetection format.
+
+    Args:
+        in_channels: Number of input channels.
+        state_dict: State dict.
+        fused_initial:
+
+    Returns:
+        State dict in celldetection format.
+    """
+    mapping = {}
+    for k, v in state_dict.items():
+        if 'fc' in k:  # skip fc
+            continue
+        if k.startswith('conv1.') and v.data.shape[1] != in_channels:  # initial layer, img channels might differ
+            v.data = F.interpolate(v.data[None], (in_channels,) + v.data.shape[-2:]).squeeze(0)
+        if fused_initial:
+            rules = {'conv1.': '0.0.', 'bn1.': '0.1.', 'layer1.': '0.4.', 'layer2.': '1.', 'layer3.': '2.',
+                     'layer4.': '3.', 'layer5.': '4.'}
+        else:
+            rules = {'conv1.': '0.0.', 'bn1.': '0.1.', 'layer1.': '1.1.', 'layer2.': '2.', 'layer3.': '3.',
+                     'layer4.': '4.', 'layer5.': '5.'}
+        mapping[_apply_mapping_rules(k, rules)] = v
+    return mapping
+
+
+class ResNet(nn.Sequential):
+    def __init__(self, in_channels, *body: nn.Module, initial_strides=2, base_channel=64, initial_pooling=True,
+                 final_layer=None, final_activation=None, fused_initial=True, pretrained=False,
+                 pyramid_pooling=False, pyramid_pooling_channels=64, pyramid_pooling_kwargs=None, nd=2, **kwargs):
+        assert len(body) > 0
+        body = list(body)
+        Conv = get_nd_conv(nd)
+        Norm = lookup_nn(nn.BatchNorm2d, nd=nd, call=False)
+        MaxPool = lookup_nn(nn.MaxPool2d, nd=nd, call=False)
+        initial = [
+            Conv(in_channels, base_channel, 7, padding=3, bias=False, stride=initial_strides),
+            Norm(base_channel),
+            nn.ReLU(inplace=True)
+        ]
+        pool = MaxPool(kernel_size=3, stride=2, padding=1) if initial_pooling else nn.Identity()
+        if fused_initial:
+            initial += [pool, body[0]]
+        else:
+            body[0] = nn.Sequential(pool, body[0])
+        initial = nn.Sequential(*initial)
+        components = [initial] + list(body[1:] if fused_initial else body)
+        if final_layer is not None:
+            components += [final_layer]
+        if final_activation is not None:
+            components += [lookup_nn(final_activation)]
+        super(ResNet, self).__init__(*components)
+        if pretrained:
+            if isinstance(pretrained, str):
+                state_dict = load_state_dict_from_url(pretrained)
+                if '.pytorch.org' in pretrained:
+                    state_dict = map_state_dict(in_channels, state_dict, fused_initial=fused_initial)
+                self.load_state_dict(state_dict)
+            else:
+                raise ValueError('There is no default set of weights for this model. '
+                                 'Please specify a URL using the `pretrained` argument.')
+        if pyramid_pooling:
+            pyramid_pooling_kwargs = {} if pyramid_pooling_kwargs is None else pyramid_pooling_kwargs
+            append_pyramid_pooling_(self, pyramid_pooling_channels, **pyramid_pooling_kwargs)
+
+
+class VanillaResNet(ResNet):
+    def __init__(self, in_channels, out_channels=0, layers=(2, 2, 2, 2), base_channel=64, fused_initial=True, nd=2,
+                 **kwargs):
+        self.out_channels = oc = (base_channel, base_channel * 2, base_channel * 4, base_channel * 8)
+        self.out_strides = (4, 8, 16, 32)
+        if out_channels and 'final_layer' not in kwargs.keys():
+            kwargs['final_layer'] = get_nd_conv(nd)(self.out_channels[-1], out_channels, 1)
+        super(VanillaResNet, self).__init__(
+            in_channels,
+            make_res_layer(BasicBlock, base_channel, oc[0], layers[0], stride=1, nd=nd, **kwargs),
+            make_res_layer(BasicBlock, oc[0], oc[1], layers[1], stride=2, nd=nd, **kwargs),
+            make_res_layer(BasicBlock, oc[1], oc[2], layers[2], stride=2, nd=nd, **kwargs),
+            make_res_layer(BasicBlock, oc[2], oc[3], layers[3], stride=2, nd=nd, **kwargs),
+            base_channel=base_channel, fused_initial=fused_initial, nd=nd, **kwargs
         )
+        if not fused_initial:
+            self.out_channels = (base_channel,) + self.out_channels
+            self.out_strides = (2,) + self.out_strides
 
 
-class U22(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, block_cls=None):
-        """U-Net 22.
-
-        U-Net with 22 convolutions on 5 feature resolutions (1, 1/2, 1/4, 1/8, 1/16) and one final output layer.
-
-        References:
-            https://arxiv.org/abs/1505.04597
-
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels. If set to 0, the output layer is omitted.
-        """
-        super().__init__(UNetEncoder(in_channels=in_channels, block_cls=block_cls), out_channels=out_channels,
-                         final_activation=final_activation, block=block_cls)
-
-
-class ResUNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, **kwargs):
-        """Residual U-Net.
-
-        U-Net with residual blocks.
-
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels. If set to 0, the output layer is omitted.
-            final_activation: Final activation function.
-            **kwargs: Keyword arguments for `UNetEncoder`.
-        """
-        super().__init__(UNetEncoder(in_channels=in_channels, block_cls=ResBlock, **kwargs), out_channels=out_channels,
-                         final_activation=final_activation, block=ResBlock)
-
-
-class SlimU22(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, block_cls=None):
-        """Slim U-Net 22.
-
-        U-Net with 22 convolutions on 5 feature resolutions (1, 1/2, 1/4, 1/8, 1/16) and one final output layer.
-        Like U22, but number of feature channels reduce by half.
-
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels. If set to 0, the output layer is omitted.
-            final_activation: Final activation function. Only used if ``out_channels > 0``.
-            block_cls: Module class that defines a convolutional block. Default: ``TwoConvNormRelu``.
-        """
-        super().__init__(UNetEncoder(in_channels=in_channels, base_channels=32, block_cls=block_cls),
-                         out_channels=out_channels, final_activation=final_activation, block=block_cls)
-
+class ResNet18(VanillaResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        """ResNet 18.
 
-class WideU22(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, block_cls=None):
-        """Slim U-Net 22.
-
-        U-Net with 22 convolutions on 5 feature resolutions (1, 1/2, 1/4, 1/8, 1/16) and one final output layer.
-        Like U22, but number of feature channels doubled.
+        ResNet 18 encoder.
 
         Args:
             in_channels: Number of input channels.
             out_channels: Number of output channels. If set to 0, the output layer is omitted.
-            final_activation: Final activation function. Only used if ``out_channels > 0``.
-            block_cls: Module class that defines a convolutional block. Default: ``TwoConvNormRelu``.
-        """
-        super().__init__(UNetEncoder(in_channels=in_channels, base_channels=128, block_cls=block_cls),
-                         out_channels=out_channels, final_activation=final_activation, block=block_cls)
-
-
-class U17(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, block_cls=None):
-        """U-Net 17.
-
-        U-Net with 17 convolutions on 4 feature resolutions (1, 1/2, 1/4, 1/8) and one final output layer.
-
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels. If set to 0, the output layer is omitted.
-            final_activation: Final activation function. Only used if ``out_channels > 0``.
-            block_cls: Module class that defines a convolutional block. Default: ``TwoConvNormRelu``.
-        """
-        super().__init__(UNetEncoder(in_channels=in_channels, depth=4, block_cls=block_cls), out_channels=out_channels,
-                         final_activation=final_activation, block=block_cls)
-
-
-class U12(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, block_cls=None):
-        """U-Net 12.
-
-        U-Net with 12 convolutions on 3 feature resolutions (1, 1/2, 1/4) and one final output layer.
-
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels. If set to 0, the output layer is omitted.
-            final_activation: Final activation function. Only used if ``out_channels > 0``.
-            block_cls: Module class that defines a convolutional block. Default: ``TwoConvNormRelu``.
-        """
-        super().__init__(UNetEncoder(in_channels=in_channels, depth=3, block_cls=block_cls), out_channels=out_channels,
-                         final_activation=final_activation, block=block_cls)
-
-
-class ResNet18UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        """ResNet 18 U-Net.
-
-        A U-Net with ResNet 18 encoder.
-
-        Args:
-            in_channels: Number of input channels.
-            out_channels: Number of output channels. If set to 0, the output layer is omitted.
-            final_activation: Final activation function. Only used if ``out_channels > 0``.
-            res_kwargs: Keyword arguments for encoder.
-            **kwargs:
-        """
-        super().__init__(ResNet18(in_channels, **(res_kwargs or {})), out_channels, final_activation=final_activation,
-                         **kwargs)
-
-
-class ResNet34UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(ResNet34(in_channels, **(res_kwargs or {})), out_channels, final_activation=final_activation,
-                         **kwargs)
-
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'ResNet 34')
-
-
-class ResNet50UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(ResNet50(in_channels, **(res_kwargs or {})), out_channels, final_activation=final_activation,
-                         **kwargs)
+            final_layer: Final output layer. Default: 1x1 Conv2d if ``out_channels >= 1``, ``None`` otherwise.
+            final_activation: Final activation layer (e.g. ``nn.ReLU`` or ``'relu'``). Default: ``None``.
+            pretrained: Whether to load weights from a pretrained network. If True default weights are used.
+                Alternatively, ``pretrained`` can be a URL of a ``state_dict`` that is hosted online.
+            **kwargs: Additional keyword arguments.
+        """
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ResNet18']
+        super(ResNet18, self).__init__(in_channels, out_channels=out_channels, layers=(2, 2, 2, 2),
+                                       pretrained=pretrained, nd=nd, **kwargs)
+
+
+class ResNet34(VanillaResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ResNet34']
+        super(ResNet34, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 6, 3),
+                                       pretrained=pretrained, nd=nd, **kwargs)
+
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNet 34')
+
+
+class BottleResNet(ResNet):
+    def __init__(self, in_channels, out_channels=0, layers=(3, 4, 6, 3), base_channel=64, fused_initial=True, nd=2,
+                 **kwargs):
+        ex = Bottleneck.expansion
+        self.out_channels = oc = (base_channel * 4, base_channel * 8, base_channel * 16, base_channel * 32)
+        self.out_strides = (4, 8, 16, 32)
+        if out_channels and 'final_layer' not in kwargs.keys():
+            kwargs['final_layer'] = nn.Conv2d(self.out_channels[-1], out_channels, 1)
+        super(BottleResNet, self).__init__(
+            in_channels,
+            make_res_layer(Bottleneck, base_channel, oc[0] // ex, layers[0], stride=1, nd=nd, **kwargs),
+            make_res_layer(Bottleneck, base_channel * 4, oc[1] // ex, layers[1], stride=2, nd=nd, **kwargs),
+            make_res_layer(Bottleneck, base_channel * 8, oc[2] // ex, layers[2], stride=2, nd=nd, **kwargs),
+            make_res_layer(Bottleneck, base_channel * 16, oc[3] // ex, layers[3], stride=2, nd=nd, **kwargs),
+            base_channel=base_channel, fused_initial=fused_initial, nd=nd, **kwargs
+        )
+        if not fused_initial:
+            self.out_channels = (base_channel,) + self.out_channels
+            self.out_strides = (2,) + self.out_strides
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'ResNet 50')
 
+class ResNet50(BottleResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ResNet50']
+        super(ResNet50, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 6, 3),
+                                       pretrained=pretrained, nd=nd, **kwargs)
 
-class ResNet101UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(ResNet101(in_channels, **(res_kwargs or {})), out_channels, final_activation=final_activation,
-                         **kwargs)
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNet 50')
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'ResNet 101')
 
+class ResNet101(BottleResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ResNet101']
+        super(ResNet101, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 23, 3),
+                                        pretrained=pretrained, nd=nd, **kwargs)
 
-class ResNet152UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(ResNet152(in_channels, **(res_kwargs or {})), out_channels, final_activation=final_activation,
-                         **kwargs)
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNet 101')
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'ResNet 152')
 
+class ResNet152(BottleResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ResNet152']
+        super(ResNet152, self).__init__(in_channels, out_channels=out_channels, layers=(3, 8, 36, 3),
+                                        pretrained=pretrained, nd=nd, **kwargs)
 
-class ResNeXt50UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(ResNeXt50_32x4d(in_channels, **(res_kwargs or {})), out_channels,
-                         final_activation=final_activation, **kwargs)
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNet 152')
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'ResNeXt 50')
 
+class ResNeXt50_32x4d(BottleResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ResNeXt50_32x4d']
+        super(ResNeXt50_32x4d, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 6, 3), groups=32,
+                                              base_width=4, pretrained=pretrained, nd=nd, **kwargs)
 
-class ResNeXt101UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(ResNeXt101_32x8d(in_channels, **(res_kwargs or {})), out_channels,
-                         final_activation=final_activation, **kwargs)
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNeXt 50')
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'ResNeXt 101')
 
+class ResNeXt101_32x8d(BottleResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['ResNeXt101_32x8d']
+        super(ResNeXt101_32x8d, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 23, 3), groups=32,
+                                               base_width=8, pretrained=pretrained, nd=nd, **kwargs)
 
-class ResNeXt152UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(ResNeXt152_32x8d(in_channels, **(res_kwargs or {})), out_channels,
-                         final_activation=final_activation, **kwargs)
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNeXt 101')
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'ResNeXt 152')
 
+class ResNeXt152_32x8d(BottleResNet):
+    def __init__(self, in_channels, out_channels=0, nd=2, **kwargs):
+        super(ResNeXt152_32x8d, self).__init__(in_channels, out_channels=out_channels, layers=(3, 8, 36, 3), groups=32,
+                                               base_width=8, nd=nd, **kwargs)
 
-class WideResNet50UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(WideResNet50_2(in_channels, **(res_kwargs or {})), out_channels,
-                         final_activation=final_activation, **kwargs)
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'ResNeXt 152')
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'Wide ResNet 50')
 
+class WideResNet50_2(BottleResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['WideResNet50_2']
+        super(WideResNet50_2, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 6, 3),
+                                             base_width=64 * 2, pretrained=pretrained, nd=nd, **kwargs)
 
-class WideResNet101UNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(WideResNet101_2(in_channels, **(res_kwargs or {})), out_channels,
-                         final_activation=final_activation, **kwargs)
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'Wide ResNet 50')
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'Wide ResNet 101')
 
+class WideResNet101_2(BottleResNet):
+    def __init__(self, in_channels, out_channels=0, pretrained=False, nd=2, **kwargs):
+        if pretrained is True and nd == 2:
+            pretrained = default_model_urls['WideResNet101_2']
+        super(WideResNet101_2, self).__init__(in_channels, out_channels=out_channels, layers=(3, 4, 23, 3),
+                                              base_width=64 * 2, pretrained=pretrained, nd=nd, **kwargs)
 
-class MobileNetV3SmallUNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(MobileNetV3Small(in_channels, **(res_kwargs or {})), out_channels,
-                         final_activation=final_activation, **kwargs)
+    __init__.__doc__ = ResNet18.__init__.__doc__.replace('ResNet 18', 'Wide ResNet 101')
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'Small MobileNet V3')
 
+models_by_name = {
+    'resnet18': ResNet18,
+    'resnet34': ResNet34,
+    'resnet50': ResNet50,
+    'resnet101': ResNet101,
+    'resnet152': ResNet152,
+    'resnext50_32x4d': ResNeXt50_32x4d,
+    'resnext101_32x8d': ResNeXt101_32x8d,
+    'resnext152_32x8d': ResNeXt152_32x8d,
+    'wideresnet50_2': WideResNet50_2,
+    'wideresnet101_2': WideResNet101_2
+}
 
-class MobileNetV3LargeUNet(UNet):
-    def __init__(self, in_channels, out_channels, final_activation=None, res_kwargs=None, **kwargs):
-        super().__init__(MobileNetV3Large(in_channels, **(res_kwargs or {})), out_channels,
-                         final_activation=final_activation, **kwargs)
 
-    __init__.__doc__ = ResNet18UNet.__init__.__doc__.replace('ResNet 18', 'Large MobileNet V3')
+def get_resnet(name, in_channels, **kwargs):
+    return models_by_name[name](in_channels=in_channels, **kwargs)
```

### Comparing `CellDetection-0.3.1/celldetection/mpi/mpi.py` & `CellDetection-0.4.0/celldetection/mpi/mpi.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,24 +67,23 @@
 ...         mpi.send(comm, result, sink, tag=idx)  # send result to sink
 
 
 MPI Operations
 --------------
 """
 
-
 import numpy as np
 
 _ERR = None
 try:
     from mpi4py import MPI
 
     ANY_TAG = MPI.ANY_TAG
     ANY_SOURCE = MPI.ANY_SOURCE
-except ModuleNotFoundError as e:
+except (ModuleNotFoundError, ImportError) as e:
     _ERR = e
     MPI = False
     ANY_TAG = -1
     ANY_SOURCE = -2  # may differ depending on MPI implementation
 
 __all__ = ['recv', 'send', 'sink', 'query', 'serve', 'all_filter', 'get_local_comm', 'get_hosts', 'get_comm']
 
@@ -109,23 +108,30 @@
     if return_ranks:
         node_rank = next(i for i, h in enumerate(hosts) if h == host)
         node_ranks = len(list(hosts))
         res += (node_rank, node_ranks)
     return res
 
 
-@assert_mpi
-def get_comm(comm=None, return_ranks=True):
-    comm = comm or MPI.COMM_WORLD
-    res = comm,
-    if return_ranks:
-        rank = comm.Get_rank()
-        ranks = comm.Get_size()
-        res += rank, ranks
-    return res
+if MPI:
+    @assert_mpi
+    def get_comm(comm=None, return_ranks=True):
+        comm = comm or MPI.COMM_WORLD
+        res = comm,
+        if return_ranks:
+            rank = comm.Get_rank()
+            ranks = comm.Get_size()
+            res += rank, ranks
+        return res
+else:
+    def get_comm(comm=None, return_ranks=True):  # dummy
+        if comm is not None:
+            raise NotImplementedError
+        if return_ranks:
+            return None, 0, 1
 
 
 @assert_mpi
 def get_local_comm(comm, return_ranks=False, host=None, node_rank=None):
     """Get local comm.
 
     Split ``comm`` by host. The returned comm is an MPI Comm object that connects ranks from the same host.
```

### Comparing `CellDetection-0.3.1/celldetection/ops/commons.py` & `CellDetection-0.4.0/celldetection/ops/commons.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 from torch import Tensor
 import torch.nn.functional as F
 from typing import List
 
-__all__ = ['downsample_labels', 'padded_stack2d', 'split_spatially', 'minibatch_std_layer', 'strided_upsampling2d']
+__all__ = ['downsample_labels', 'padded_stack2d', 'split_spatially', 'minibatch_std_layer', 'strided_upsampling2d',
+           'interpolate_vector']
 
 
 def downsample_labels(inputs, size: List[int]):
     """
 
     Down-sample via max-pooling and interpolation
 
@@ -50,32 +51,36 @@
         Tensor
     """
     ts = tuple(max((i.shape[j] for i in images)) for j in range(-2, 0))
     images = [F.pad(i, [0, ts[1] - i.shape[-1], 0, ts[0] - i.shape[-2]]) for i in images]
     return torch.stack(images, dim=dim)
 
 
-def split_spatially(x, height, width=None):
+def split_spatially(x, size):
     """Split spatially.
 
-    Splits spatial dimensions of Tensor ``x`` into patches of size ``(height, width)`` and adds the patches
+    Splits spatial dimensions of Tensor ``x`` into patches of given ``size`` and adds the patches
     to the batch dimension.
 
     Args:
-        x: Input Tensor[n, c, h, w].
-        height: Patch height.
-        width: Patch width.
+        x: Input Tensor[n, c, h, w, ...].
+        size: Patch size of the splits.
 
     Returns:
         Tensor[n * h//height * w//width, c, height, width].
     """
-    width = width or height
-    n, c, h, w = x.shape
-    h_, w_ = h // height, w // width
-    return x.view(n, c, h_, height, w_, width).permute(0, 2, 4, 1, 3, 5).reshape(-1, c, height, width)
+    n, c = x.shape[:2]
+    spatial = x.shape[2:]
+    nd = len(spatial)
+    assert len(spatial) == len(size)
+    v = n, c
+    for cur, new in zip(spatial, size):
+        v += (cur // new, new)
+    perm = (0,) + tuple(range(2, nd * 2 + 1, 2)) + tuple(range(1, nd * 3, 2))
+    return x.view(v).permute(perm).reshape((-1, c) + tuple(size))
 
 
 def minibatch_std_layer(x, channels=1, group_channels=None, epsilon=1e-8):
     """Minibatch standard deviation layer.
 
     The minibatch standard deviation layer first splits the batch dimension into slices of size ``group_channels``.
     The channel dimension is split into ``channels`` slices. For the groups the standard deviation is calculated and
@@ -117,7 +122,23 @@
     """
     n, c, h, w = x.shape
     x_ = torch.zeros((n, c, h * factor, w * factor), dtype=x.dtype, device=x.device)
     if const != 0:
         x_.fill_(const)
     x_[..., ::factor, ::factor] = x
     return x_
+
+
+def interpolate_vector(v, size, **kwargs):
+    """Interpolate vector.
+
+    Args:
+        v: Vector as ``Tensor[d]``.
+        size: Target size.
+        **kwargs: Keyword arguments for ``F.interpolate``
+
+    Returns:
+
+    """
+    return torch.squeeze(torch.squeeze(
+        F.interpolate(v[None, None], size, **kwargs), 0
+    ), 0)
```

### Comparing `CellDetection-0.3.1/celldetection/ops/cpn.py` & `CellDetection-0.4.0/celldetection/ops/cpn.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import torch
 from torch import Tensor
-from typing import Union, Tuple, List, Dict
+from typing import Tuple, List, Dict
 
 
 def rel_location2abs_location(locations, cache: Dict[str, Tensor] = None, cache_size: int = 16):
     """
 
     Args:
         locations: Tensor[..., 2, h, w]. In xy format.
@@ -174,14 +174,25 @@
         cons.append(con[indices])
         scos.append(sco[indices])
         for j, res_ in enumerate(it[2:]):
             further[j].append(res_[indices])
     return (cons, scos) + tuple(further)
 
 
+def batched_box_nmsi(
+        boxes: List[Tensor], scores: List[Tensor], iou_threshold: float
+) -> List[Tensor]:
+    assert len(scores) == len(boxes)
+    keeps = []
+    for con, sco in zip(boxes, scores):
+        indices = torch.ops.torchvision.nms(con, sco, iou_threshold=iou_threshold)
+        keeps.append(indices)
+    return keeps
+
+
 def order_weighting(order, max_w=5, min_w=1, spread=None) -> torch.Tensor:
     x = torch.arange(order).float()
     if spread is None:
         spread = order - 1
     y = min_w + (max_w - min_w) * (1 - (x / spread).clamp(0., 1.)) ** 2
     return y[:, None]  # broadcastable to (n, order, 4)
 
@@ -200,7 +211,39 @@
     base_index_int = base_index.long()
     a, b, c = base_index_int - 1, base_index_int, base_index_int + 1
     return (
         (a % num_buckets, refinement_bucket_weight(a, base_index)),
         (b % num_buckets, refinement_bucket_weight(b, base_index)),
         (c % num_buckets, refinement_bucket_weight(c, base_index))
     )
+
+
+def remove_border_contours(contours, size, padding=1, top=True, right=True, bottom=True, left=True):
+    """Remove border contours.
+
+    Remove contours that touch border regions.
+
+    Args:
+        contours: Contours as ``Tensor[num_contours, num_points, 2]``.
+        size: Context size.
+        padding: Padding. Determines the thickness of the border region. ``padding=1`` removes all contours that overlap
+            with the outer 1px frame.
+        top: Whether to test top border.
+        right: Whether to test right border.
+        bottom: Whether to test bottom border.
+        left: Whether to test left border.
+
+    Returns:
+        Keep mask as ``Tensor[num_contours]``.
+    """
+    h, w = size[:2]
+    x, y = contours[..., 0], contours[..., 1]
+    keep = torch.ones(len(contours), dtype=torch.bool, device=contours.device)
+    if top:
+        keep = keep & (y > padding).all(1)
+    if right:
+        keep = keep & (x < (w - padding)).all(1)
+    if bottom:
+        keep = keep & (y < (h - padding)).all(1)
+    if left:
+        keep = keep & (x > padding).all(1)
+    return keep
```

### Comparing `CellDetection-0.3.1/celldetection/ops/draw.py` & `CellDetection-0.4.0/celldetection/ops/draw.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/ops/normalization.py` & `CellDetection-0.4.0/celldetection/ops/normalization.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/util/schedule.py` & `CellDetection-0.4.0/celldetection/util/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from .util import dict_hash, Dict, tweak_module_, lookup_nn
+from .util import dict_hash, Dict, tweak_module_, lookup_nn, print_to_file
+from ..optim import lr_scheduler
 import json
 from itertools import product
 from collections import OrderedDict
 from torch.nn import Module
 from torch import optim
+import inspect
 from typing import Callable, Union
 import albumentations as A
 
 __all__ = ['Config', 'Schedule', 'conf2optimizer', 'conf2scheduler', 'conf2augmentation', 'conf2tweaks_', 'conf2call']
 
 
 def conf2call(settings: Union[dict, str], origin, **kwargs):
@@ -66,16 +68,18 @@
 
     Returns:
 
     """
     return conf2call(settings, optim, params=params)
 
 
-def conf2scheduler(settings: dict, optimizer):
-    return conf2call(settings, optim.lr_scheduler, optimizer=optimizer)
+def conf2scheduler(settings: dict, optimizer, origins=None):
+    if origins is None:
+        origins = (lr_scheduler, optim.lr_scheduler)
+    return conf2call(settings, origins, optimizer=optimizer)
 
 
 def conf2augmentation(settings: dict) -> A.Compose:
     """Config to augmentation.
 
     Maps settings to composed augmentation workflow using ``albumentations``.
 
@@ -86,15 +90,14 @@
         ...     'Transpose': dict(p=.5),
         ... })
         Compose([
           RandomRotate90(always_apply=False, p=0.5),
           Transpose(always_apply=False, p=0.5),
         ], p=1.0, bbox_params=None, keypoint_params=None, additional_targets={})
 
-
     Args:
         settings: Settings dictionary as ``{name: kwargs}``.
 
     Returns:
         ``A.Compose`` object.
     """
     return A.Compose([getattr(A, k)(**v) for k, v in settings.items()])
@@ -181,27 +184,78 @@
     def to_dict(self) -> dict:
         return {k: v for k, v in dict(self).items() if not k.startswith('_')}
 
     def to_json(self, filename):
         with open(filename, 'w') as fp:
             json.dump(self.to_dict(), fp)
 
+    def to_txt(self, filename, mode='w', **kwargs):
+        print_to_file(self, filename=filename, mode=mode, **kwargs)
+
     def __str__(self):
         return repr(self)
 
     def _get_name(self):
         return 'Config'
 
     def extra_repr(self) -> str:
         return ''
 
     def __repr__(self):
         self._modules = self.to_dict()
         return Module.__repr__(self)
 
+    def args(self, fn: Callable):
+        """
+
+        Examples:
+            >>> conf = cd.Config(a=1, b=2, c=42)
+            >>> def f(a, b):
+            ...     return a + b
+            >>> f(*conf.args(f))
+            3
+
+        Args:
+            fn:
+
+        Returns:
+
+        """
+        r = []
+        for k in inspect.signature(fn).parameters.keys():
+            if k == 'args' or k == 'kwargs':
+                break
+            r.append(self[k])
+        return r
+
+    def kwargs(self, fn: Callable):
+        """
+
+        Examples:
+            >>> conf = cd.Config(a=1, b=2, c=42)
+            >>> def f(a, b):
+            ...     return a + b
+            >>> f(**conf.kwargs(f))
+            3
+
+        Args:
+            fn:
+
+        Returns:
+
+        """
+        r = dict()
+        for k in inspect.signature(fn).parameters.keys():
+            if k == 'args' or k == 'kwargs':
+                continue
+            v = self.get(k, None)
+            if v is not None:
+                r[k] = v
+        return r
+
     def __getstate__(self):
         return self.to_dict()
 
     def __setstate__(self, d: dict):
         self.update(d)
 
 
@@ -254,14 +308,17 @@
         self.values = OrderedDict({})
         self.conditions = []
         self.conditioned_values = []
         self.add(kwargs)
         self._iter_conf = None
         self._iter_i = None
 
+    def get_multiples(self, num=2):
+        return {k: v for k, v in self.values.items() if (isinstance(v, (list, tuple, set)) and len(v) >= num)}
+
     def add(self, d: dict = None, conditions: dict = None, **kwargs):
         """Add setting to schedule.
 
         Examples:
             >>> schedule = cd.Schedule(model=('resnet18', 'resnet50'), batch_size=8)
             ... schedule.add(batch_size=(16, 32), conditions={'model': 'resnet18'})
             ... schedule[:]
@@ -387,14 +444,20 @@
     def __len__(self):
         return len(self.configs)
 
     def to_json(self, filename):
         with open(filename, 'w') as fp:
             json.dump(self.values, fp)
 
+    @staticmethod
+    def from_json(filename):
+        c = Schedule()
+        c.load(filename)
+        return c
+
     def load(self, filename):
         with open(filename, 'r') as fp:
             self.values = json.load(fp)
 
     def to_dict(self):
         return dict(self.values)
```

### Comparing `CellDetection-0.3.1/celldetection/util/timer.py` & `CellDetection-0.4.0/celldetection/util/timer.py`

 * *Files identical despite different names*

### Comparing `CellDetection-0.3.1/celldetection/util/util.py` & `CellDetection-0.4.0/celldetection/util/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,70 @@
 import numpy as np
 import inspect
 import torch
 import torch.nn as nn
 import torch.nn.init as init
-from typing import Union, List, Tuple, Any, Dict as TDict, Iterator, Type
+from typing import Union, List, Tuple, Any, Dict as TDict, Iterator, Type, Callable, Iterable, Sequence
 from torch import Tensor
 from torch.hub import load_state_dict_from_url
 import hashlib
 import json
 from tqdm import tqdm
-from os.path import join
+from os.path import join, isfile
 from os import makedirs
 import pynvml as nv
 from cv2 import getGaussianKernel
 import h5py
+from collections import OrderedDict
+import re
+import sys
+from itertools import product
+from inspect import currentframe
+from shutil import copy2
 
 __all__ = ['Dict', 'lookup_nn', 'reduce_loss_dict', 'tensor_to', 'to_device', 'asnumpy', 'fetch_model',
            'random_code_name', 'dict_hash', 'fetch_image', 'random_seed', 'tweak_module_', 'add_to_loss_dict',
            'random_code_name_dir', 'get_device', 'num_params', 'count_submodules', 'train_epoch', 'Bytes', 'Percent',
            'GpuStats', 'trainable_params', 'frozen_params', 'Tiling', 'load_image', 'gaussian_kernel',
            'iter_submodules', 'replace_module_', 'wrap_module_', 'spectral_norm_', 'to_h5', 'to_tiff',
-           'exponential_moving_average_', 'from_json', 'to_json']
+           'to_json', 'from_json', 'exponential_moving_average_', 'weight_norm_', 'inject_extra_repr_',
+           'ensure_num_tuple', 'get_nd_conv', 'get_nd_linear', 'get_nd_dropout', 'get_nd_max_pool', 'get_nd_batchnorm',
+           'get_warmup_factor', 'print_to_file', 'NormProxy', 'num_bytes', 'from_h5', 'update_dict_',
+           'get_tiling_slices', 'get_nn', 'copy_script', 'hash_file', 'append_hash_to_filename', 'save_fetchable_model',
+           'load_model']
+
+
+def copy_script(dst, no_script_okay=True, frame=None, verbose=False):
+    """Copy current script.
+
+    Copies the script from where this function is called to ``dst``.
+    By default, nothing happens if this function is not called from within a script.
+
+    Args:
+        dst: Copy destination. Filename or folder.
+        no_script_okay: If ``False`` raise ``FileNotFoundError`` if no script is found.
+        verbose: Whether to print source and destination when copying.
+
+    """
+    if frame is None:
+        current_frame = currentframe()
+        if current_frame:
+            frame = current_frame.f_back
+    if frame is None:
+        raise ValueError('Invalid frame.')
+
+    src = frame.f_globals.get('__file__')
+    if src is None:
+        if not no_script_okay:
+            raise FileNotFoundError('Could not find current script.')
+        return
+
+    if verbose:
+        print(f'Copy `{src}` to `{dst}`.')
+    copy2(src, dst)
 
 
 class Dict(dict):
     __getattr__ = dict.__getitem__  # alternative: dict.get if KeyError is not desired
     __delattr__ = dict.__delitem__
     __setattr__ = dict.__setitem__
 
@@ -44,15 +84,49 @@
 
         Args:
             **kwargs:
         """
         super().__init__(kwargs)
 
 
-def lookup_nn(item: str, *a, src=None, call=True, inplace=True, **kw):
+def replace_ndim(s: Union[str, type, Callable], dim: int, allowed_dims=(1, 2, 3)):
+    """Replace ndim.
+
+    Replaces dimension statement of ``string``or ``type``.
+
+    Notes:
+        - Dimensions are expected to be at the end of the type name.
+        - If there is no dimension statement, nothing is changed.
+
+    Examples:
+        >>> replace_ndim('BatchNorm2d', 3)
+        'BatchNorm3d'
+        >>> replace_ndim(nn.BatchNorm2d, 3)
+        torch.nn.modules.batchnorm.BatchNorm3d
+        >>> replace_ndim(nn.GroupNorm, 3)
+        torch.nn.modules.normalization.GroupNorm
+        >>> replace_ndim(F.conv2d, 3)
+        <function torch._VariableFunctionsClass.conv3d>
+
+    Args:
+        s: String or type.
+        dim: Desired dimension.
+        allowed_dims: Allowed dimensions to look for.
+
+    Returns:
+        Input with replaced dimension.
+    """
+    if isinstance(s, str) and dim in allowed_dims:
+        return re.sub(f"[1-3]d$", f'{int(dim)}d', s)
+    elif isinstance(s, type) or callable(s):
+        return getattr(sys.modules[s.__module__], replace_ndim(s.__name__, dim))
+    return s
+
+
+def lookup_nn(item: str, *a, src=None, call=True, inplace=True, nd=None, **kw):
     """
 
     Examples:
         >>> lookup_nn('batchnorm2d', 32)
             BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
         >>> lookup_nn(torch.nn.BatchNorm2d, 32)
             BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
@@ -62,44 +136,127 @@
             Tanh()
         >>> lookup_nn('tanh', call=False)
             torch.nn.modules.activation.Tanh
         >>> lookup_nn('relu')
             ReLU(inplace=True)
         >>> lookup_nn('relu', inplace=False)
             ReLU()
+        >>> # Dict notation to contain all keyword arguments for calling in `item`. Always called once.
+        ... lookup_nn(dict(relu=dict(inplace=True)), call=False)
+            ReLU(inplace=True)
+        >>> lookup_nn({'NormProxy': {'norm': 'GroupNorm', 'num_groups': 32}}, call=False)
+            NormProxy(GroupNorm, kwargs={'num_groups': 32})
+        >>> lookup_nn({'NormProxy': {'norm': 'GroupNorm', 'num_groups': 32}}, 32, call=True)
+            GroupNorm(32, 32, eps=1e-05, affine=True)
 
     Args:
         item: Lookup item. None is equivalent to `identity`.
         *a: Arguments passed to item if called.
         src: Lookup source.
         call: Whether to call item.
         inplace: Default setting for items that take an `inplace` argument when called.
             As default is True, `lookup_nn('relu')` returns a ReLu instance with `inplace=True`.
+        nd: If set, replace dimension statement (e.g. '2d' in nn.Conv2d) with ``nd``.
         **kw: Keyword arguments passed to item when it is called.
 
     Returns:
         Looked up item.
     """
-    src = src or nn
+    if src is None:
+        from .. import models
+        src = (nn, models)
+    if isinstance(item, tuple):
+        if len(item) == 1:
+            item, = item
+        elif len(item) == 2:
+            item, _kw = item
+            kw.update(_kw)
+        else:
+            raise ValueError('Allowed formats for item: (item,) or (item, kwargs).')
     if item is None:
         v = nn.Identity
     elif isinstance(item, str):
         l_item = item.lower()
-        v = next((getattr(src, i) for i in dir(src) if i.lower() == l_item))
+        if nd is not None:
+            l_item = replace_ndim(l_item, nd)
+        if not isinstance(src, (list, tuple)):
+            src = src,
+        v = None
+        for src_ in src:
+            try:
+                v = next((getattr(src_, i) for i in dir(src_) if i.lower() == l_item))
+            except StopIteration:
+                continue
+            break
+        if v is None:
+            raise ValueError(f'Could not find `{item}` in {src}.')
     elif isinstance(item, nn.Module):
         return item
+    elif isinstance(item, dict):
+        assert len(item) == 1
+        key, = item
+        val = item[key]
+        assert isinstance(val, dict)
+        v = lookup_nn(key, src=src, call=False, inplace=inplace, nd=nd)(**val)
+    elif isinstance(item, type) and nd is not None:
+        v = replace_ndim(item, nd)
     else:
         v = item
     if call:
         kwargs = {'inplace': inplace} if 'inplace' in inspect.getfullargspec(v).args else {}
         kwargs.update(kw)
         v = v(*a, **kwargs)
     return v
 
 
+def get_nn(item: Union[str, 'nn.Module', Type['nn.Module']], src=None, nd=None):
+    return lookup_nn(item, src=src, nd=nd, call=False)
+
+
+class NormProxy:
+    def __init__(self, norm, **kwargs):
+        """Norm Proxy.
+
+        Examples:
+            >>> GroupNorm = NormProxy('groupnorm', num_groups=32)
+            ... GroupNorm(3)
+            GroupNorm(32, 3, eps=1e-05, affine=True)
+            >>> GroupNorm = NormProxy(nn.GroupNorm, num_groups=32)
+            ... GroupNorm(3)
+            GroupNorm(32, 3, eps=1e-05, affine=True)
+            >>> BatchNorm2d = NormProxy('batchnorm2d', momentum=.2)
+            ... BatchNorm2d(3)
+            BatchNorm2d(3, eps=1e-05, momentum=0.2, affine=True, track_running_stats=True)
+            >>> BatchNorm2d = NormProxy(nn.BatchNorm2d, momentum=.2)
+            ... BatchNorm2d(3)
+            BatchNorm2d(3, eps=1e-05, momentum=0.2, affine=True, track_running_stats=True)
+
+        Args:
+            norm: Norm class or name.
+            **kwargs: Keyword arguments.
+        """
+        self.norm = norm
+        self.kwargs = kwargs
+
+    def __call__(self, num_channels):
+        Norm = lookup_nn(self.norm, call=False)
+        kwargs = dict(self.kwargs)
+        args = inspect.getfullargspec(Norm).args
+        if 'num_features' in args:
+            kwargs['num_features'] = num_channels
+        elif 'num_channels' in args:
+            kwargs['num_channels'] = num_channels
+        return Norm(**kwargs)
+
+    def __repr__(self):
+        return f'NormProxy({self.norm}, kwargs={self.kwargs})'
+
+    __str__ = __repr__
+
+
 def reduce_loss_dict(losses: dict, divisor):
     return sum((i for i in losses.values() if i is not None)) / divisor
 
 
 def add_to_loss_dict(d: dict, key: str, loss: torch.Tensor, weight=None):
     dk = d[key]
     torch.nan_to_num_(loss, 0., 0., 0.)
@@ -124,15 +281,15 @@
         **kwargs: Keyword arguments. See docstring of ``torch.Tensor.to``.
 
     Returns:
         Inputs with Tensors replaced by ``tensor.to(*args, **kwargs)``.
     """
     if isinstance(inputs, Tensor):
         inputs = inputs.to(*args, **kwargs)
-    elif isinstance(inputs, dict):
+    elif isinstance(inputs, (dict, OrderedDict)):
         inputs = {k: tensor_to(b, *args, **kwargs) for k, b in inputs.items()}
     elif isinstance(inputs, (list, tuple)):
         inputs = type(inputs)([tensor_to(b, *args, **kwargs) for b in inputs])
     return inputs
 
 
 def to_device(batch: Union[list, tuple, dict, Tensor], device):
@@ -172,48 +329,105 @@
     """
     if v is None:
         return v
     elif isinstance(v, torch.Tensor):
         if str(v.device) != 'cpu':
             v = v.cpu()
         return v.data.numpy()
-    elif isinstance(v, (np.ndarray, int, float, bool, np.float, np.int, np.bool, str)):
+    elif isinstance(v, (np.ndarray, int, float, bool, str)):
         return v
     elif isinstance(v, (tuple, list)):
         return [asnumpy(val) for val in v]
     elif isinstance(v, dict):
         r = dict()
         for k, val in v.items():
             r[k] = asnumpy(val)
         return r
     else:
         raise ValueError(f'Type not supported: {type(v)}')
 
 
+def _load_cd_format(m, **kwargs):
+    assert isinstance(m, dict) and 'cd.models' in m.keys()
+    state_dict = m['state_dict']
+    from .. import models
+    conf = m['cd.models']
+    kw = {**conf.get('kwargs', conf.get('kw', {})), **kwargs}
+    m = getattr(models, conf['model'])(*conf.get('args', conf.get('a', ())), **kw)
+    m.load_state_dict(state_dict)
+    return m
+
+
+def load_model(filename, map_location=None, **kwargs):
+    assert isfile(filename)
+    m = torch.load(filename, map_location=map_location, **kwargs.pop('load_kwargs', {}))
+    if isinstance(m, dict) and 'cd.models' in m.keys():
+        return _load_cd_format(m, **kwargs)
+    return m
+
+
 def fetch_model(name, map_location=None, **kwargs):
     """Fetch model from URL.
 
     Loads model or state dict from URL.
 
     Args:
         name: Model name hosted on `celldetection.org` or url. Urls must start with 'http'.
         map_location: A function, `torch.device`, string or a dict specifying how to remap storage locations.
         **kwargs: From the doc of `torch.models.utils.load_state_dict_from_url`.
 
     """
     url = name if name.startswith('http') else f'https://celldetection.org/torch/models/{name}.pt'
-    m = load_state_dict_from_url(url, map_location=map_location, **kwargs)
+    m = load_state_dict_from_url(url, map_location=map_location, **kwargs.pop('load_state_dict_kwargs', {}))
     if isinstance(m, dict) and 'cd.models' in m.keys():
-        from .. import models
-        conf = m['cd.models']
-        m = getattr(models, conf['model'])(*conf['a'], **conf['kw'])
-        m.load_state_dict(conf['state_dict'])
+        m = _load_cd_format(m, **kwargs)
     return m
 
 
+def hash_file(filename):
+    import hashlib
+
+    with open(filename, 'rb') as f:
+        sha256 = hashlib.sha256(f.read()).hexdigest()
+    return sha256
+
+
+def append_hash_to_filename(filename, num=None, ext=True):
+    from os import rename
+    prefix = filename
+    postfix = ''
+    if ext:
+        sp = prefix.split('.')
+        prefix = '.'.join(sp[:-1])
+        postfix = f'.{sp[-1]}'
+    sha256 = hash_file(filename)
+    if num is not None:
+        sha256 = sha256[:num]
+    dst = prefix + f'-{sha256}' + postfix
+    rename(filename, dst)
+
+
+def save_fetchable_model(model: 'nn.Module', filename, append_hash=16):
+    model.eval()
+    model = model.to('cpu')
+    kwargs = model.hparams
+    name = model.__class__.__name__
+    torch.save({
+        'cd.models': dict(
+            model=name,
+            kwargs=kwargs,
+        ),
+        'state_dict': model.state_dict(),
+    }, filename)
+    if append_hash:
+        if append_hash is True:
+            append_hash = None
+        append_hash_to_filename(filename, num=append_hash)
+
+
 def random_code_name(chars=4) -> str:
     """Random code name.
 
     Generates random code names that are somewhat pronounceable and memorable.
 
     Examples:
         >>> import celldetection as cd
@@ -228,33 +442,41 @@
     Returns:
         String.
     """
     a, b = [i for i in 'aeiou'], [i for i in 'tskyrhzjgqmxlvnfcpwbd']
     return ''.join([np.random.choice(b if j % 2 == 0 else a) for j in range(chars)])
 
 
-def random_code_name_dir(directory='./out', chars=6):
+def random_code_name_dir(directory='./out', chars=6, comm=None, root_rank=0):
     """Random code name directory.
 
     Creates random code name and creates a subdirectory with said name under `directory`.
     Code names that are already taken (subdirectory already exists) are not reused.
 
     Args:
         directory: Root directory.
         chars: Number of characters for the code name.
+        comm: MPI Comm. If provided, code name and directory is automatically broadcasted to all ranks of `comm`.
+        root_rank: Root rank. Only the root rank creates code name and directory.
 
     Returns:
         Tuple of code name and created directory.
     """
-    try:
-        code_name = random_code_name(chars=chars)
-        out_dir = join(directory, code_name)
-        makedirs(out_dir)
-    except FileExistsError:
-        return random_code_name_dir(directory)
+    rank = code_name = out_dir = None
+    if comm is not None:
+        rank = comm.Get_rank()
+    if rank is None or rank == root_rank:
+        try:
+            code_name = random_code_name(chars=chars)
+            out_dir = join(directory, code_name)
+            makedirs(out_dir)
+        except FileExistsError:
+            return random_code_name_dir(directory, chars=chars)
+    if rank is not None:
+        code_name, out_dir = comm.bcast((code_name, out_dir), root=root_rank)
     return code_name, out_dir
 
 
 def dict_hash(dictionary: TDict[str, Any]) -> str:
     """MD5 hash of a dictionary.
 
     References:
@@ -334,22 +556,24 @@
     """
     from torch import manual_seed
     from torch.backends import cudnn
     import random
     random.seed(seed)
     manual_seed(seed)
     np.random.seed(seed)
+    torch.cuda.manual_seed(seed)
     if backends:
         cudnn.deterministic = True
         cudnn.benchmark = False
     if deterministic_torch and 'use_deterministic_algorithms' in dir(torch):
         torch.use_deterministic_algorithms(True)
 
 
-def train_epoch(model, train_loader, device, optimizer, desc=None, scaler=None, scheduler=None, gpu_stats=False):
+def train_epoch(model, train_loader, device, optimizer, desc=None, scaler=None, scheduler=None, gpu_stats=False,
+                progress=True):
     """Basic train function.
 
     Notes:
         - Model should return dictionary: {'loss': Tensor[], ...}
         - Batch from `train_loader` should be a dictionary: {'inputs': Tensor[...], ...}
         - Model must be callable: `model(batch['inputs'], targets=batch)`
 
@@ -358,36 +582,38 @@
         train_loader: Data loader.
         device: Device.
         optimizer: Optimizer.
         desc: Description, appears in progress print.
         scaler: Gradient scaler. If set PyTorch's autocast feature is used.
         scheduler: Scheduler. Step called after epoch.
         gpu_stats: Whether to print GPU stats.
+        progress: Show progress.
     """
     from torch.cuda.amp import autocast
     model.train()
-    tq = tqdm(train_loader, desc=desc)
+    tq = tqdm(train_loader, desc=desc) if progress else train_loader
     gpu_st = None
     if gpu_stats:
         gpu_st = GpuStats()
     for batch_idx, batch in enumerate(tq):
         batch: dict = to_device(batch, device)
         optimizer.zero_grad()
         with autocast(scaler is not None):
             outputs: dict = model(batch['inputs'], targets=batch)
         loss = outputs['loss']
-        info = [] if desc is None else [desc]
-        if gpu_st is not None:
-            info.append(str(gpu_st))
-        losses = outputs.get('losses')
-        if losses is not None and isinstance(losses, dict):
-            info.append('losses(' + ', '.join(
-                [(f'{k}: %g' % np.round(asnumpy(v), 3)) for k, v in losses.items() if v is not None]) + ')')
-        info.append('loss %g' % np.round(asnumpy(loss), 3))
-        tq.desc = ' - '.join(info)
+        if progress:
+            info = [] if desc is None else [desc]
+            if gpu_st is not None:
+                info.append(str(gpu_st))
+            losses = outputs.get('losses')
+            if losses is not None and isinstance(losses, dict):
+                info.append('losses(' + ', '.join(
+                    [(f'{k}: %g' % np.round(asnumpy(v), 3)) for k, v in losses.items() if v is not None]) + ')')
+            info.append('loss %g' % np.round(asnumpy(loss), 3))
+            tq.desc = ' - '.join(info)
         if scaler is None:
             loss.backward()
             optimizer.step()
         else:
             scaler.scale(loss).backward()
             scaler.step(optimizer)
             scaler.update()
@@ -427,64 +653,154 @@
         for k, v in kwargs.items():
             if must_exist:
                 getattr(mod, k)
             setattr(mod, k, v)
 
 
 def replace_module_(module: nn.Module, class_or_tuple, substitute: Union[Type[nn.Module], nn.Module], recursive=True,
-                    inherit_attr: list = None, **kwargs):
+                    inherit_attr: Union[list, str, dict] = None, **kwargs):
     """Replace module.
 
     Replace all occurrences of `class_or_tuple` in `module` with `substitute`.
 
     Examples:
         >>> # Replace all ReLU activations with LeakyReLU
         ... cd.replace_module_(network, nn.ReLU, nn.LeakyReLU)
 
         >>> # Replace all BatchNorm layers with InstanceNorm and inherit `num_features` attribute
         ... cd.replace_module_(network, nn.BatchNorm2d, nn.InstanceNorm2d, inherit_attr=['num_features'])
 
+        >>> # Replace all BatchNorm layers with GroupNorm and inherit `num_features` attribute
+        ... cd.replace_module_(network, nn.BatchNorm2d, nn.GroupNorm, num_groups=32,
+        ...                    inherit_attr={'num_channels': 'num_features'})
+
     Args:
         module: Module.
         class_or_tuple: Class or tuple of classes that are to be replaced.
         substitute: Substitute class or object.
         recursive: Whether to replace modules recursively.
-        inherit_attr: Attributes to be inherited. List of attribute names. Attribute values are retrieved from replaced
-            module and passed to substitute constructor.
+        inherit_attr: Attributes to be inherited. String, list or dict of attribute names.
+            Attribute values are retrieved from replaced module and passed to substitute constructor.
+            Formats:
+            ``'attr_name'``,
+            ``['attr_name0', 'attr_name1', ...]``,
+            ``{'substitute_kw0': 'attr_name0', ...}``
         **kwargs: Keyword arguments passed to substitute constructor if it is a class.
-
     """
     for handle, k, mod in iter_submodules(module, class_or_tuple, recursive=recursive):
         if isinstance(substitute, nn.Module):
             handle[k] = substitute
         else:
-            inherit_attr = inherit_attr or []
-            handle[k] = substitute(**kwargs, **{k: mod.__dict__[k] for k in inherit_attr})
+            kw = {}
+            if isinstance(inherit_attr, str):
+                inherit_attr = [inherit_attr]
+            if isinstance(inherit_attr, list):
+                kw = {k: mod.__dict__[k] for k in inherit_attr}
+            elif isinstance(inherit_attr, dict):
+                kw = {k: mod.__dict__[v] for k, v in inherit_attr.items()}
+            handle[k] = substitute(**kwargs, **kw)
+
+
+def inject_extra_repr_(module, name, fn):
+    """Inject extra representation.
+
+    Injects additional ``extra_repr`` function to ``module``.
+    This can be helpful to indicate presence of hooks.
+
+    Note:
+        This is an inplace operation.
+
+    Notes:
+        - This op may impair pickling.
+
+    Args:
+        module: Module.
+        name: Name of the injected function (only used to avoid duplicate injection).
+        fn: Callback function.
+
+    """
+
+    def extra_repr(self=module):
+        vals = [self.extra_repr_orig()] + list(f(self) for f in self.extra_repr_funcs.values())
+        return ', '.join([v for v in vals if v])
+
+    if not hasattr(module, 'extra_repr_orig'):
+        module.extra_repr_orig = module.extra_repr
+        module.extra_repr_funcs = {}
+        module.extra_repr = extra_repr
+    module.extra_repr_funcs[name] = fn
 
 
 def wrap_module_(module: nn.Module, class_or_tuple, wrapper, recursive=True, **kwargs):
     for handle, k, mod in iter_submodules(module, class_or_tuple, recursive=recursive):
         handle[k] = wrapper(handle[k], **kwargs)
 
 
-def spectral_norm_(module, class_or_tuple=nn.Conv2d, recursive=True, **kwargs):
+def spectral_norm_(module, class_or_tuple=nn.Conv2d, recursive=True, name='weight', add_repr=False, **kwargs):
     """Spectral normalization.
 
     Applies spectral normalization to parameters of all occurrences of ``class_or_tuple`` in the given module.
 
     Note:
         This is an inplace operation.
 
+    References:
+        - https://arxiv.org/pdf/1802.05957.pdf
+
     Args:
         module: Module.
         class_or_tuple: Class or tuple of classes whose parameters are to be normalized.
         recursive: Whether to search for modules recursively.
+        name: Name of weight parameter.
+        add_repr: Whether to indicate use of spectral norm in a module's representation.
+            Note that this may impair pickling.
         **kwargs: Additional keyword arguments for ``torch.nn.utils.spectral_norm``.
     """
-    wrap_module_(module, class_or_tuple, recursive=recursive, wrapper=nn.utils.spectral_norm, **kwargs)
+
+    def extra_repr(self):
+        if 'torch.nn.utils.spectral_norm.SpectralNorm' in str(list(self._forward_pre_hooks.values())):
+            return 'spectral_norm=True'
+
+    for handle, k, mod in iter_submodules(module, class_or_tuple, recursive=recursive):
+        if mod._parameters.get(name) is not None:
+            handle[k] = nn.utils.spectral_norm(handle[k], name=name, **kwargs)
+            if add_repr:
+                inject_extra_repr_(handle[k], 'spectral_norm', extra_repr)
+
+
+def weight_norm_(module, class_or_tuple=nn.Conv2d, recursive=True, name='weight', add_repr=False, **kwargs):
+    """Weight normalization.
+
+    Applies weight normalization to parameters of all occurrences of ``class_or_tuple`` in the given module.
+
+    Note:
+        This is an inplace operation.
+
+    References:
+        - https://proceedings.neurips.cc/paper/2016/file/ed265bc903a5a097f61d3ec064d96d2e-Paper.pdf
+
+    Args:
+        module: Module.
+        class_or_tuple: Class or tuple of classes whose parameters are to be normalized.
+        recursive: Whether to search for modules recursively.
+        name: Name of weight parameter.
+        add_repr: Whether to indicate use of weight norm in a module's representation.
+            Note that this may impair pickling.
+        **kwargs: Additional keyword arguments for ``torch.nn.utils.weight_norm``.
+    """
+
+    def extra_repr(self):
+        if 'torch.nn.utils.weight_norm.WeightNorm' in str(list(self._forward_pre_hooks.values())):
+            return 'weight_norm=True'
+
+    for handle, k, mod in iter_submodules(module, class_or_tuple, recursive=recursive):
+        if mod._parameters.get(name) is not None:
+            handle[k] = nn.utils.weight_norm(handle[k], name=name, **kwargs)
+            if add_repr:
+                inject_extra_repr_(handle[k], 'weight_norm', extra_repr)
 
 
 def get_device(module: Union[nn.Module, Tensor, torch.device]):
     """Get device.
 
     Get device from Module.
 
@@ -579,39 +895,47 @@
     elif isinstance(v, (list, tuple)):
         pass
     else:
         raise ValueError(msg)
     return v
 
 
-def gaussian_kernel(kernel_size, sigma=-1) -> np.ndarray:
+def gaussian_kernel(kernel_size, sigma=-1, nd=2) -> np.ndarray:
     """Get Gaussian kernel.
 
     Constructs and returns a Gaussian kernel.
 
     Args:
         kernel_size: Kernel size as int or tuple. It should be odd and positive.
         sigma: Gaussian standard deviation as float or tuple. If it is non-positive, it is computed from kernel_size as
             ``sigma = 0.3*((kernel_size-1)*0.5 - 1) + 0.8``.
+        nd: Number of kernel dimensions.
 
     Returns:
         Gaussian Kernel.
     """
-    kernel_size = ensure_num_tuple(kernel_size, msg='kernel_size must be int, tuple or list.')
-    sigma = ensure_num_tuple(sigma, msg='sigma must be int, tuple or list.')
-    return getGaussianKernel(kernel_size[0], sigma[0]) @ getGaussianKernel(kernel_size[1], sigma[1]).T
+    kernel_sizes = ensure_num_tuple(kernel_size, num=nd, msg='kernel_size must be int, tuple or list.')
+    sigmas = ensure_num_tuple(sigma, num=nd, msg='sigma must be int, tuple or list.')
+    y = None
+    for k, s in zip(kernel_sizes, sigmas):
+        y_ = getGaussianKernel(k, s)[:, 0]
+        if y is None:
+            y = y_
+        else:
+            y = y[..., :, None] * y_[..., None, :]
+    return y
 
 
 class Bytes(int):
     """Bytes.
 
     Printable integer that represents Bytes.
 
     """
-    UNITS = ['B', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB', 'BB']
+    UNITS = ['B', 'KiB', 'MiB', 'GiB', 'TiB', 'PiB', 'EiB', 'ZiB', 'YiB', 'BiB']
 
     def __str__(self):
         n = np.log2(int(self)) if self > 0 else 0
         s = None
         for i, tag in enumerate(self.UNITS):
             if n < (i + 1) * 10 or i == len(self.UNITS) - 1:
                 s = str(np.round(float(self) / (2 ** (10 * i)), 2)) + tag
@@ -648,15 +972,15 @@
 
         Args:
             delimiter: Delimiter used for printing.
         """
         try:
             nv.nvmlInit()
             self.num = nv.nvmlDeviceGetCount()
-        except:
+        except Exception:
             self.num = 0
         self.delimiter = delimiter
 
     def __len__(self):
         return self.num
 
     def __getitem__(self, item: int):
@@ -711,15 +1035,50 @@
             start_with_overlap=start_wo,
             stop_with_overlap=stop_wo,
             num_tiles=self.num_tiles,
             num_tiles_per_dim=self.num_tiles_per_dim
         )
 
 
-def to_h5(filename, mode='w', chunks=False, compression=None, overwrite=False, create_dataset_kw: dict = None,
+def get_tiling_slices(
+        size: Sequence[int],
+        crop_size: Union[int, Sequence[int]],
+        strides: Union[int, Sequence[int]]
+) -> Union[Iterable[slice], Tuple[int]]:
+    """Get tiling slices.
+
+    Args:
+        size: Reference size as tuple.
+        crop_size: Crop size.
+        strides: Strides.
+
+    Returns:
+        Iterable[slice], Tuple[int]:
+            Iterator of tiling slices (each slice defining a tile),
+            Number of tiles per dimension as tuple.
+    """
+    assert isinstance(size, (tuple, list))
+    crop_size = ensure_num_tuple(crop_size, len(size))
+    strides = ensure_num_tuple(strides, len(size))
+    slices, shape = [], []
+    for axis in range(len(size)):
+        if crop_size[axis] >= size[axis]:
+            tl = [size[axis]]
+        else:
+            tl = range(crop_size[axis], max(2, 1 + int(np.ceil(size[axis] / strides[axis]))) * strides[axis],
+                       strides[axis])
+        axis_slices = []
+        for t in tl:
+            stop = min(t, size[axis])
+            axis_slices.append(slice(max(0, stop - crop_size[axis]), stop))
+        slices.append(axis_slices), shape.append(len(tl))
+    return product(*slices), shape
+
+
+def to_h5(filename, mode='w', chunks=None, compression=None, overwrite=False, create_dataset_kw: dict = None,
           **kwargs):
     """To hdf5 file.
 
     Write data to hdf5 file.
 
     Args:
         filename: File name.
@@ -741,14 +1100,34 @@
                 del h[k]
             elif exists:
                 h[k][:] = v
             else:
                 h.create_dataset(k, data=v, compression=compression, chunks=chunks, **create_dataset_kw)
 
 
+def from_h5(filename, *keys, **keys_slices):
+    """From h5.
+
+    Reads data from hdf5 file.
+
+    Args:
+        filename: Filename.
+        *keys: Keys to read.
+        **keys_slices: Keys with indices or slices. E.g. `from_h5('file.h5', 'key0', key=slice(0, 42))`.
+
+    Returns:
+        Data from hdf5 file. As tuple if multiple keys are provided.
+    """
+    with h5py.File(filename, 'r') as h:
+        res = tuple(h[k][:] for k in keys) + tuple(h[k][v] for k, v in keys_slices.items())
+    if len(res) == 1:
+        res, = res
+    return res
+
+
 def to_tiff(filename, image, mode='w', method='tile', bigtiff=True):
     """To tiff file.
 
     Write ``image`` to tiff file using ``pytiff``.
     By default, the tiff is tiled, s.t. crops can be read from disk without loading the entire image into memory first.
 
     Notes:
@@ -826,7 +1205,76 @@
 
     Args:
         filename: File name.
     """
     with open(filename, 'r') as fp:
         v = json.load(fp)
     return v
+
+
+def get_nd_conv(dim: int):
+    assert isinstance(dim, int) and dim in (1, 2, 3)
+    return getattr(nn, 'Conv%dd' % dim)
+
+
+def get_nd_max_pool(dim: int):
+    assert isinstance(dim, int) and dim in (1, 2, 3)
+    return getattr(nn, 'MaxPool%dd' % dim)
+
+
+def get_nd_batchnorm(dim: int):
+    assert isinstance(dim, int) and dim in (1, 2, 3)
+    return getattr(nn, 'BatchNorm%dd' % dim)
+
+
+def get_nd_dropout(dim: int):
+    assert isinstance(dim, int) and dim in (1, 2, 3)
+    return getattr(nn, 'Dropout%dd' % dim)
+
+
+def get_nd_linear(dim: int):
+    assert isinstance(dim, int) and dim in (1, 2, 3)
+    return ['', 'bi', 'tri'][dim - 1] + 'linear'
+
+
+def get_warmup_factor(step, steps=1000, factor=0.001, method='linear'):
+    if step >= steps:
+        return 1.
+    if method == 'constant':
+        return factor
+    elif method == 'linear':
+        a = step / steps
+        return factor * (1 - a) + a
+    raise ValueError(f'Unknown method: {method}')
+
+
+def print_to_file(*args, filename, mode='w', **kwargs):
+    with open(filename, mode=mode) as f:
+        print(*args, file=f, **kwargs)
+
+
+def num_bytes(x: Union[np.ndarray, Tensor]):
+    """Num Bytes.
+
+    Returns the size in bytes of the given ndarray or Tensor.
+
+    Args:
+        x: Array or Tensor.
+
+    Returns:
+        Bytes
+    """
+    if isinstance(x, np.ndarray):
+        bts = x.itemsize * x.size
+    elif isinstance(x, Tensor):
+        bts = x.numel() * x.element_size()
+    else:
+        raise ValueError(f'Could not handle type: {type(x)}')
+    return Bytes(bts)
+
+
+def update_dict_(dst, src, override=False, keys: Union[List[str], Tuple[str]] = None):
+    for k, v in src.items():
+        if keys is not None and k not in keys:
+            continue
+        if override or k not in dst:
+            dst[k] = v
```

### Comparing `CellDetection-0.3.1/setup.py` & `CellDetection-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,17 @@
     author_email=m['__email__'],
     name=m['__title__'],
     version=m['__version__'],
     description=m['__summary__'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url=m['__url__'],
-    packages=['celldetection', 'celldetection.data', 'celldetection.data.datasets', 'celldetection.models',
-              'celldetection.mpi', 'celldetection.ops', 'celldetection.util', 'celldetection.visualization'],
+    packages=['celldetection', 'celldetection.data', 'celldetection.callbacks', 'celldetection.optim',
+              'celldetection.data.datasets', 'celldetection.models', 'celldetection.mpi', 'celldetection.ops',
+              'celldetection.util', 'celldetection.visualization'],
     package_data={'': ['LICENSE', 'requirements.txt', 'README.md']},
     include_package_data=True,
     install_requires=requirements,
     license=m['__license__'],
     keywords=['cell', 'detection', 'object', 'segmentation', 'pytorch', 'cpn', 'contour', 'proposal', 'network', 'deep',
               'learning', 'unet', 'fzj', 'julich', 'juelich', 'ai'],
     classifiers=[
```

