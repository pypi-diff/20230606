# Comparing `tmp/hello2-1.8.6.tar.gz` & `tmp/hello2-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello2-1.8.6.tar", last modified: Thu Jun  1 06:42:37 2023, max compression
+gzip compressed data, was "hello2-1.8.7.tar", last modified: Tue Jun  6 07:49:48 2023, max compression
```

## Comparing `hello2-1.8.6.tar` & `hello2-1.8.7.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0      550 2022-11-04 08:45:52.036893 hello2-1.8.6/.gitignore
--rw-r--r--   0        0        0      715 2022-11-04 17:06:29.116576 hello2-1.8.6/.readthedocs.yaml
--rw-r--r--   0        0        0    11357 2022-06-27 01:46:45.026108 hello2-1.8.6/LICENSE
--rw-r--r--   0        0        0      351 2022-12-20 05:58:10.658183 hello2-1.8.6/README.md
--rw-r--r--   0        0        0      638 2022-11-04 13:36:31.980929 hello2-1.8.6/docs/Makefile
--rw-r--r--   0        0        0      804 2022-11-04 13:36:31.980929 hello2-1.8.6/docs/make.bat
--rw-r--r--   0        0        0      163 2022-11-06 11:07:57.505182 hello2-1.8.6/docs/requirements.txt
--rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.8.6/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.8.6/docs/source/_templates/.gitkeep
--rw-r--r--   0        0        0     1365 2022-11-06 12:23:09.043638 hello2-1.8.6/docs/source/conf.py
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.770149 hello2-1.8.6/docs/source/hello.data.coco2yolo.rst
--rw-r--r--   0        0        0      231 2022-11-04 14:14:10.770149 hello2-1.8.6/docs/source/hello.data.rst
--rw-r--r--   0        0        0      187 2022-12-14 01:38:29.403883 hello2-1.8.6/docs/source/hello.experimental.albu.detection.rst
--rw-r--r--   0        0        0      283 2022-12-14 01:38:29.403883 hello2-1.8.6/docs/source/hello.experimental.albu.rst
--rw-r--r--   0        0        0      260 2022-12-14 01:38:29.393883 hello2-1.8.6/docs/source/hello.experimental.rst
--rw-r--r--   0        0        0      157 2023-04-20 14:38:58.196102 hello2-1.8.6/docs/source/hello.fiftyone.annotate.rst
--rw-r--r--   0        0        0      148 2022-12-14 09:04:35.414160 hello2-1.8.6/docs/source/hello.fiftyone.brain.rst
--rw-r--r--   0        0        0      145 2023-05-04 10:28:37.375287 hello2-1.8.6/docs/source/hello.fiftyone.coco.rst
--rw-r--r--   0        0        0      165 2023-05-29 00:31:35.816394 hello2-1.8.6/docs/source/hello.fiftyone.coco_utils.rst
--rw-r--r--   0        0        0      160 2023-04-29 13:47:19.060767 hello2-1.8.6/docs/source/hello.fiftyone.connected.rst
--rw-r--r--   0        0        0      160 2022-11-18 12:12:27.461051 hello2-1.8.6/docs/source/hello.fiftyone.copypaste.rst
--rw-r--r--   0        0        0      145 2022-11-04 14:14:10.780149 hello2-1.8.6/docs/source/hello.fiftyone.core.rst
--rw-r--r--   0        0        0      154 2022-11-04 14:14:10.780149 hello2-1.8.6/docs/source/hello.fiftyone.dataset.rst
--rw-r--r--   0        0        0      183 2022-11-04 14:14:10.780149 hello2-1.8.6/docs/source/hello.fiftyone.dataset_annotate.rst
--rw-r--r--   0        0        0      189 2022-11-04 14:14:10.780149 hello2-1.8.6/docs/source/hello.fiftyone.dataset_detections.rst
--rw-r--r--   0        0        0      198 2022-11-04 14:14:10.790149 hello2-1.8.6/docs/source/hello.fiftyone.dataset_segmentations.rst
--rw-r--r--   0        0        0      177 2022-11-04 14:14:10.790149 hello2-1.8.6/docs/source/hello.fiftyone.dataset_yolov5.rst
--rw-r--r--   0        0        0      168 2022-11-04 14:14:10.790149 hello2-1.8.6/docs/source/hello.fiftyone.dataset_zoo.rst
--rw-r--r--   0        0        0      157 2022-11-04 14:14:10.790149 hello2-1.8.6/docs/source/hello.fiftyone.evaluate.rst
--rw-r--r--   0        0        0      192 2022-11-04 14:14:10.790149 hello2-1.8.6/docs/source/hello.fiftyone.evaluate_detections.rst
--rw-r--r--   0        0        0      201 2022-11-04 14:14:10.790149 hello2-1.8.6/docs/source/hello.fiftyone.evaluate_segmentations.rst
--rw-r--r--   0        0        0      171 2022-11-18 12:12:27.481051 hello2-1.8.6/docs/source/hello.fiftyone.gen_examples.rst
--rw-r--r--   0        0        0      168 2022-11-18 12:12:27.481051 hello2-1.8.6/docs/source/hello.fiftyone.mask_ignore.rst
--rw-r--r--   0        0        0      145 2022-11-04 14:14:10.790149 hello2-1.8.6/docs/source/hello.fiftyone.miou.rst
--rw-r--r--   0        0        0      154 2022-11-18 12:12:27.481051 hello2-1.8.6/docs/source/hello.fiftyone.patches.rst
--rw-r--r--   0        0        0      905 2023-05-29 00:31:35.816394 hello2-1.8.6/docs/source/hello.fiftyone.rst
--rw-r--r--   0        0        0      154 2022-12-16 13:39:47.530383 hello2-1.8.6/docs/source/hello.fiftyone.tarinfo.rst
--rw-r--r--   0        0        0      151 2022-11-04 14:14:10.800149 hello2-1.8.6/docs/source/hello.fiftyone.unique.rst
--rw-r--r--   0        0        0      148 2022-11-22 16:10:13.239568 hello2-1.8.6/docs/source/hello.fiftyone.utils.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.800149 hello2-1.8.6/docs/source/hello.fiftyone.video.rst
--rw-r--r--   0        0        0      145 2022-11-22 16:10:13.239568 hello2-1.8.6/docs/source/hello.fiftyone.view.rst
--rw-r--r--   0        0        0      139 2023-04-29 13:47:19.090767 hello2-1.8.6/docs/source/hello.fvcore.core.rst
--rw-r--r--   0        0        0      234 2023-04-29 13:47:19.090767 hello2-1.8.6/docs/source/hello.fvcore.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.800149 hello2-1.8.6/docs/source/hello.io.image.rst
--rw-r--r--   0        0        0      237 2022-11-04 14:14:10.800149 hello2-1.8.6/docs/source/hello.io.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.810149 hello2-1.8.6/docs/source/hello.io.utils.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.810149 hello2-1.8.6/docs/source/hello.mmdet.export.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.810149 hello2-1.8.6/docs/source/hello.mmdet.flop.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.820149 hello2-1.8.6/docs/source/hello.mmdet.infer.rst
--rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.8.6/docs/source/hello.mmdet.log.rst
--rw-r--r--   0        0        0      136 2022-11-25 07:45:47.915124 hello2-1.8.6/docs/source/hello.mmdet.plot.rst
--rw-r--r--   0        0        0      312 2022-11-25 07:45:47.915124 hello2-1.8.6/docs/source/hello.mmdet.rst
--rw-r--r--   0        0        0      142 2023-05-29 00:31:35.816394 hello2-1.8.6/docs/source/hello.mmlab.mmdet3.rst
--rw-r--r--   0        0        0      139 2023-05-29 00:31:35.816394 hello2-1.8.6/docs/source/hello.mmlab.mmseg.rst
--rw-r--r--   0        0        0      253 2023-05-29 00:31:35.816394 hello2-1.8.6/docs/source/hello.mmlab.rst
--rw-r--r--   0        0        0      139 2022-11-07 02:04:44.756679 hello2-1.8.6/docs/source/hello.mmseg.infer.rst
--rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.8.6/docs/source/hello.mmseg.log.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.820149 hello2-1.8.6/docs/source/hello.mmseg.lr.rst
--rw-r--r--   0        0        0      268 2022-11-07 02:04:44.756679 hello2-1.8.6/docs/source/hello.mmseg.rst
--rw-r--r--   0        0        0      145 2023-04-20 14:38:58.266102 hello2-1.8.6/docs/source/hello.nanodet.infer.rst
--rw-r--r--   0        0        0      239 2023-04-20 14:38:58.266102 hello2-1.8.6/docs/source/hello.nanodet.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.830149 hello2-1.8.6/docs/source/hello.onnx.export.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.830149 hello2-1.8.6/docs/source/hello.onnx.infer.rst
--rw-r--r--   0        0        0      248 2022-11-04 14:14:10.830149 hello2-1.8.6/docs/source/hello.onnx.rst
--rw-r--r--   0        0        0      415 2023-05-29 00:31:35.826394 hello2-1.8.6/docs/source/hello.rst
--rw-r--r--   0        0        0      256 2022-11-04 14:14:10.840149 hello2-1.8.6/docs/source/hello.transforms.rst
--rw-r--r--   0        0        0      169 2022-11-04 14:14:10.840149 hello2-1.8.6/docs/source/hello.transforms.transforms.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.8.6/docs/source/hello.utils.colors.rst
--rw-r--r--   0        0        0      145 2023-05-29 00:31:35.826394 hello2-1.8.6/docs/source/hello.utils.compare.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.850149 hello2-1.8.6/docs/source/hello.utils.cuda.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.850149 hello2-1.8.6/docs/source/hello.utils.importer.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.850149 hello2-1.8.6/docs/source/hello.utils.plots.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.8.6/docs/source/hello.utils.points.rst
--rw-r--r--   0        0        0      365 2023-05-29 00:31:35.826394 hello2-1.8.6/docs/source/hello.utils.rst
--rw-r--r--   0        0        0      145 2022-11-30 10:15:09.976399 hello2-1.8.6/docs/source/hello.utils.strtime.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.860149 hello2-1.8.6/docs/source/hello.video.align.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.8.6/docs/source/hello.video.clip.rst
--rw-r--r--   0        0        0      145 2023-04-20 14:38:58.306102 hello2-1.8.6/docs/source/hello.video.fisheye.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.8.6/docs/source/hello.video.frames.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.8.6/docs/source/hello.video.info.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.8.6/docs/source/hello.video.resize.rst
--rw-r--r--   0        0        0      425 2023-04-20 14:38:58.296102 hello2-1.8.6/docs/source/hello.video.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.870149 hello2-1.8.6/docs/source/hello.video.rtsp.rst
--rw-r--r--   0        0        0      153 2022-11-29 06:30:33.931961 hello2-1.8.6/docs/source/hello.video.rtsp_pull.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.8.6/docs/source/hello.video.split.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.870149 hello2-1.8.6/docs/source/hello.video.unwarp.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.8.6/docs/source/hello.video.utils.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.880149 hello2-1.8.6/docs/source/hello.x3m.config.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.8.6/docs/source/hello.x3m.preprocess.rst
--rw-r--r--   0        0        0      272 2022-11-04 14:14:10.870149 hello2-1.8.6/docs/source/hello.x3m.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.8.6/docs/source/hello.x3m.transforms.rst
--rw-r--r--   0        0        0      572 2022-11-04 15:19:50.508765 hello2-1.8.6/docs/source/index.rst
--rw-r--r--   0        0        0       52 2022-11-04 14:40:30.829573 hello2-1.8.6/docs/source/modules.rst
--rw-r--r--   0        0        0     3270 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/README.md
--rw-r--r--   0        0        0      773 2023-06-01 06:40:36.380242 hello2-1.8.6/hello/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.6/hello/__main__.py
--rw-r--r--   0        0        0      471 2022-11-06 13:38:11.482015 hello2-1.8.6/hello/data/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.6/hello/data/__main__.py
--rw-r--r--   0        0        0     3426 2022-08-30 01:19:13.615222 hello2-1.8.6/hello/data/coco2yolo.py
--rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.8.6/hello/experimental/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.8.6/hello/experimental/albu/__init__.py
--rw-r--r--   0        0        0      111 2022-12-11 06:23:09.504528 hello2-1.8.6/hello/experimental/albu/detection.py
--rw-r--r--   0        0        0     1047 2022-11-06 13:38:17.442013 hello2-1.8.6/hello/fiftyone/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.6/hello/fiftyone/__main__.py
--rw-r--r--   0        0        0     4742 2023-05-30 03:46:30.923445 hello2-1.8.6/hello/fiftyone/annotate.py
--rw-r--r--   0        0        0    10588 2023-05-30 15:55:41.469982 hello2-1.8.6/hello/fiftyone/brain.py
--rw-r--r--   0        0        0     8233 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/fiftyone/coco.py
--rw-r--r--   0        0        0     3945 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/fiftyone/coco_utils.py
--rw-r--r--   0        0        0      912 2023-04-25 01:47:26.910695 hello2-1.8.6/hello/fiftyone/connected.py
--rw-r--r--   0        0        0       36 2022-11-18 04:25:30.455378 hello2-1.8.6/hello/fiftyone/copypaste.py
--rw-r--r--   0        0        0    18009 2023-05-24 08:55:42.705839 hello2-1.8.6/hello/fiftyone/core.py
--rw-r--r--   0        0        0    20251 2023-06-01 06:34:06.690322 hello2-1.8.6/hello/fiftyone/dataset.py
--rw-r--r--   0        0        0     7502 2022-12-30 03:41:16.092249 hello2-1.8.6/hello/fiftyone/dataset_detections.py
--rw-r--r--   0        0        0     5693 2022-12-30 03:45:01.362177 hello2-1.8.6/hello/fiftyone/dataset_segmentations.py
--rw-r--r--   0        0        0     1402 2022-11-30 01:50:37.091070 hello2-1.8.6/hello/fiftyone/dataset_yolov5.py
--rw-r--r--   0        0        0      889 2022-12-02 08:54:06.970245 hello2-1.8.6/hello/fiftyone/dataset_zoo.py
--rw-r--r--   0        0        0     1169 2022-07-18 00:56:40.761934 hello2-1.8.6/hello/fiftyone/evaluate.py
--rw-r--r--   0        0        0     5157 2023-03-07 04:04:15.369663 hello2-1.8.6/hello/fiftyone/evaluate_detections.py
--rw-r--r--   0        0        0     4544 2023-03-07 04:04:11.609664 hello2-1.8.6/hello/fiftyone/evaluate_segmentations.py
--rw-r--r--   0        0        0      103 2022-09-19 06:15:49.337504 hello2-1.8.6/hello/fiftyone/examples/README.md
--rw-r--r--   0        0        0     2975 2022-11-30 01:46:25.831120 hello2-1.8.6/hello/fiftyone/examples/examples.py
--rw-r--r--   0        0        0    12021 2023-01-09 09:33:51.046594 hello2-1.8.6/hello/fiftyone/examples/utils.py
--rw-r--r--   0        0        0     3241 2023-05-19 07:54:24.980385 hello2-1.8.6/hello/fiftyone/gen_examples.py
--rw-r--r--   0        0        0     2328 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/fiftyone/mask_ignore.py
--rw-r--r--   0        0        0     5683 2022-12-30 03:42:18.702230 hello2-1.8.6/hello/fiftyone/miou.py
--rw-r--r--   0        0        0     2639 2022-11-18 06:29:39.594231 hello2-1.8.6/hello/fiftyone/patches.py
--rw-r--r--   0        0        0     9311 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/fiftyone/tarinfo.py
--rw-r--r--   0        0        0     4094 2023-03-15 08:42:32.674825 hello2-1.8.6/hello/fiftyone/unique.py
--rw-r--r--   0        0        0     8090 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/fiftyone/utils.py
--rw-r--r--   0        0        0      781 2022-12-01 14:14:43.560707 hello2-1.8.6/hello/fiftyone/video.py
--rw-r--r--   0        0        0     8268 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/fiftyone/view.py
--rw-r--r--   0        0        0      435 2022-10-20 14:18:34.575285 hello2-1.8.6/hello/fvcore/README.md
--rw-r--r--   0        0        0        0 2022-11-04 14:49:06.729395 hello2-1.8.6/hello/fvcore/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-29 13:43:43.400786 hello2-1.8.6/hello/fvcore/core.py
--rw-r--r--   0        0        0      135 2022-06-27 01:46:45.026108 hello2-1.8.6/hello/io/__init__.py
--rw-r--r--   0        0        0     1382 2022-08-23 09:20:12.751790 hello2-1.8.6/hello/io/image.py
--rw-r--r--   0        0        0      989 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/io/utils.py
--rw-r--r--   0        0        0      851 2022-11-25 07:46:45.875120 hello2-1.8.6/hello/mmdet/__init__.py
--rw-r--r--   0        0        0       67 2022-10-17 07:49:46.479528 hello2-1.8.6/hello/mmdet/__main__.py
--rw-r--r--   0        0        0       97 2022-10-17 08:00:01.479443 hello2-1.8.6/hello/mmdet/export.py
--rw-r--r--   0        0        0     1736 2022-10-20 16:17:29.762828 hello2-1.8.6/hello/mmdet/flop.py
--rw-r--r--   0        0        0     5446 2023-03-03 15:16:46.611009 hello2-1.8.6/hello/mmdet/infer.py
--rw-r--r--   0        0        0     3273 2023-04-11 07:00:00.274582 hello2-1.8.6/hello/mmdet/log.py
--rw-r--r--   0        0        0     5976 2023-04-12 11:23:04.178651 hello2-1.8.6/hello/mmdet/plot.py
--rw-r--r--   0        0        0      563 2023-05-12 07:19:19.396722 hello2-1.8.6/hello/mmlab/__init__.py
--rw-r--r--   0        0        0       67 2023-05-12 07:16:55.756771 hello2-1.8.6/hello/mmlab/__main__.py
--rw-r--r--   0        0        0      110 2023-05-12 07:26:47.136571 hello2-1.8.6/hello/mmlab/mmdet3.py
--rw-r--r--   0        0        0     6549 2023-05-15 09:18:13.003946 hello2-1.8.6/hello/mmlab/mmseg.py
--rw-r--r--   0        0        0      645 2022-11-07 02:04:01.296693 hello2-1.8.6/hello/mmseg/__init__.py
--rw-r--r--   0        0        0       67 2022-10-31 01:39:47.674470 hello2-1.8.6/hello/mmseg/__main__.py
--rw-r--r--   0        0        0     6040 2022-11-09 01:29:31.447414 hello2-1.8.6/hello/mmseg/infer.py
--rw-r--r--   0        0        0     2368 2023-04-11 07:03:55.124501 hello2-1.8.6/hello/mmseg/log.py
--rw-r--r--   0        0        0     7006 2022-12-01 12:09:30.751861 hello2-1.8.6/hello/mmseg/lr.py
--rw-r--r--   0        0        0      462 2023-03-29 08:04:38.934968 hello2-1.8.6/hello/nanodet/__init__.py
--rw-r--r--   0        0        0       67 2023-03-29 08:03:09.784974 hello2-1.8.6/hello/nanodet/__main__.py
--rw-r--r--   0        0        0     7410 2023-04-06 10:19:32.462564 hello2-1.8.6/hello/nanodet/infer.py
--rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.8.6/hello/onnx/__init__.py
--rw-r--r--   0        0        0      213 2022-06-27 02:15:25.376085 hello2-1.8.6/hello/onnx/examples/README.md
--rw-r--r--   0        0        0     1879 2022-06-27 01:46:45.026108 hello2-1.8.6/hello/onnx/examples/test_sigmoid.py
--rw-r--r--   0        0        0     3024 2022-08-30 07:45:32.884923 hello2-1.8.6/hello/onnx/export.py
--rw-r--r--   0        0        0     1707 2022-08-22 07:09:07.802604 hello2-1.8.6/hello/onnx/infer.py
--rw-r--r--   0        0        0     1334 2022-11-21 14:14:37.239473 hello2-1.8.6/hello/transforms/README.md
--rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.8.6/hello/transforms/__init__.py
--rw-r--r--   0        0        0     2655 2022-11-21 15:01:54.364062 hello2-1.8.6/hello/transforms/transforms.py
--rw-r--r--   0        0        0        0 2022-07-20 06:21:09.967902 hello2-1.8.6/hello/utils/__init__.py
--rw-r--r--   0        0        0     2133 2023-05-19 03:21:05.796070 hello2-1.8.6/hello/utils/colors.py
--rw-r--r--   0        0        0     1349 2023-05-29 00:31:35.826394 hello2-1.8.6/hello/utils/compare.py
--rw-r--r--   0        0        0     1815 2022-10-14 02:36:42.461531 hello2-1.8.6/hello/utils/cuda.py
--rw-r--r--   0        0        0      356 2022-07-20 06:43:22.727885 hello2-1.8.6/hello/utils/importer.py
--rw-r--r--   0        0        0      612 2022-08-23 06:44:50.231910 hello2-1.8.6/hello/utils/plots.py
--rw-r--r--   0        0        0     2999 2022-11-06 13:40:43.281966 hello2-1.8.6/hello/utils/points.py
--rw-r--r--   0        0        0      195 2022-11-30 01:25:21.821313 hello2-1.8.6/hello/utils/strtime.py
--rw-r--r--   0        0        0     1135 2023-02-20 08:24:47.078416 hello2-1.8.6/hello/video/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.6/hello/video/__main__.py
--rw-r--r--   0        0        0     3428 2022-11-06 13:15:37.862480 hello2-1.8.6/hello/video/align.py
--rw-r--r--   0        0        0     6382 2023-05-17 04:07:48.740198 hello2-1.8.6/hello/video/clip.py
--rw-r--r--   0        0        0     3290 2023-02-20 09:35:59.918194 hello2-1.8.6/hello/video/fisheye.py
--rw-r--r--   0        0        0     1565 2022-11-06 13:15:49.722478 hello2-1.8.6/hello/video/info.py
--rw-r--r--   0        0        0     3502 2022-11-06 13:15:55.532477 hello2-1.8.6/hello/video/resize.py
--rw-r--r--   0        0        0     4716 2022-11-29 07:15:17.421543 hello2-1.8.6/hello/video/rtsp.py
--rw-r--r--   0        0        0     5006 2022-11-29 08:00:32.141119 hello2-1.8.6/hello/video/rtsp_pull.py
--rw-r--r--   0        0        0     3048 2022-11-11 09:35:15.036742 hello2-1.8.6/hello/video/split.py
--rw-r--r--   0        0        0     4066 2023-02-20 08:27:40.638408 hello2-1.8.6/hello/video/unwarp.py
--rw-r--r--   0        0        0      968 2022-08-25 04:09:32.554890 hello2-1.8.6/hello/video/utils.py
--rw-r--r--   0        0        0      576 2022-11-06 13:41:08.801958 hello2-1.8.6/hello/x3m/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.6/hello/x3m/__main__.py
--rw-r--r--   0        0        0     4479 2022-11-06 13:41:19.251954 hello2-1.8.6/hello/x3m/config.py
--rw-r--r--   0        0        0     2592 2022-08-30 01:19:13.615222 hello2-1.8.6/hello/x3m/preprocess.py
--rw-r--r--   0        0        0     6928 2022-06-27 01:46:45.026108 hello2-1.8.6/hello/x3m/transforms.py
--rw-r--r--   0        0        0      808 2022-06-27 01:46:45.026108 hello2-1.8.6/hello_c/CMakeLists.txt
--rw-r--r--   0        0        0      776 2022-06-27 01:46:45.026108 hello2-1.8.6/hello_c/README.md
--rw-r--r--   0        0        0     1375 2022-06-27 01:46:45.026108 hello2-1.8.6/hello_c/main.cpp
--rw-r--r--   0        0        0      262 2022-06-27 01:46:45.026108 hello2-1.8.6/hello_c/trace_model.py
--rw-r--r--   0        0        0      787 2023-05-15 09:28:06.783743 hello2-1.8.6/pyproject.toml
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 hello2-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0      550 2022-11-04 08:45:52.036893 hello2-1.8.7/.gitignore
+-rw-r--r--   0        0        0      715 2022-11-04 17:06:29.116576 hello2-1.8.7/.readthedocs.yaml
+-rw-r--r--   0        0        0    11357 2022-06-27 01:46:45.026108 hello2-1.8.7/LICENSE
+-rw-r--r--   0        0        0      351 2022-12-20 05:58:10.658183 hello2-1.8.7/README.md
+-rw-r--r--   0        0        0      638 2022-11-04 13:36:31.980929 hello2-1.8.7/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-11-04 13:36:31.980929 hello2-1.8.7/docs/make.bat
+-rw-r--r--   0        0        0      163 2022-11-06 11:07:57.505182 hello2-1.8.7/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.8.7/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.8.7/docs/source/_templates/.gitkeep
+-rw-r--r--   0        0        0     1365 2022-11-06 12:23:09.043638 hello2-1.8.7/docs/source/conf.py
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.770149 hello2-1.8.7/docs/source/hello.data.coco2yolo.rst
+-rw-r--r--   0        0        0      231 2022-11-04 14:14:10.770149 hello2-1.8.7/docs/source/hello.data.rst
+-rw-r--r--   0        0        0      187 2022-12-14 01:38:29.403883 hello2-1.8.7/docs/source/hello.experimental.albu.detection.rst
+-rw-r--r--   0        0        0      283 2022-12-14 01:38:29.403883 hello2-1.8.7/docs/source/hello.experimental.albu.rst
+-rw-r--r--   0        0        0      260 2022-12-14 01:38:29.393883 hello2-1.8.7/docs/source/hello.experimental.rst
+-rw-r--r--   0        0        0      157 2023-04-20 14:38:58.196102 hello2-1.8.7/docs/source/hello.fiftyone.annotate.rst
+-rw-r--r--   0        0        0      148 2022-12-14 09:04:35.414160 hello2-1.8.7/docs/source/hello.fiftyone.brain.rst
+-rw-r--r--   0        0        0      145 2023-05-04 10:28:37.375287 hello2-1.8.7/docs/source/hello.fiftyone.coco.rst
+-rw-r--r--   0        0        0      165 2023-05-29 00:31:35.816394 hello2-1.8.7/docs/source/hello.fiftyone.coco_utils.rst
+-rw-r--r--   0        0        0      160 2023-04-29 13:47:19.060767 hello2-1.8.7/docs/source/hello.fiftyone.connected.rst
+-rw-r--r--   0        0        0      160 2022-11-18 12:12:27.461051 hello2-1.8.7/docs/source/hello.fiftyone.copypaste.rst
+-rw-r--r--   0        0        0      145 2022-11-04 14:14:10.780149 hello2-1.8.7/docs/source/hello.fiftyone.core.rst
+-rw-r--r--   0        0        0      154 2022-11-04 14:14:10.780149 hello2-1.8.7/docs/source/hello.fiftyone.dataset.rst
+-rw-r--r--   0        0        0      183 2022-11-04 14:14:10.780149 hello2-1.8.7/docs/source/hello.fiftyone.dataset_annotate.rst
+-rw-r--r--   0        0        0      189 2022-11-04 14:14:10.780149 hello2-1.8.7/docs/source/hello.fiftyone.dataset_detections.rst
+-rw-r--r--   0        0        0      198 2022-11-04 14:14:10.790149 hello2-1.8.7/docs/source/hello.fiftyone.dataset_segmentations.rst
+-rw-r--r--   0        0        0      177 2022-11-04 14:14:10.790149 hello2-1.8.7/docs/source/hello.fiftyone.dataset_yolov5.rst
+-rw-r--r--   0        0        0      168 2022-11-04 14:14:10.790149 hello2-1.8.7/docs/source/hello.fiftyone.dataset_zoo.rst
+-rw-r--r--   0        0        0      157 2022-11-04 14:14:10.790149 hello2-1.8.7/docs/source/hello.fiftyone.evaluate.rst
+-rw-r--r--   0        0        0      192 2022-11-04 14:14:10.790149 hello2-1.8.7/docs/source/hello.fiftyone.evaluate_detections.rst
+-rw-r--r--   0        0        0      201 2022-11-04 14:14:10.790149 hello2-1.8.7/docs/source/hello.fiftyone.evaluate_segmentations.rst
+-rw-r--r--   0        0        0      171 2022-11-18 12:12:27.481051 hello2-1.8.7/docs/source/hello.fiftyone.gen_examples.rst
+-rw-r--r--   0        0        0      168 2022-11-18 12:12:27.481051 hello2-1.8.7/docs/source/hello.fiftyone.mask_ignore.rst
+-rw-r--r--   0        0        0      145 2022-11-04 14:14:10.790149 hello2-1.8.7/docs/source/hello.fiftyone.miou.rst
+-rw-r--r--   0        0        0      154 2022-11-18 12:12:27.481051 hello2-1.8.7/docs/source/hello.fiftyone.patches.rst
+-rw-r--r--   0        0        0      905 2023-05-29 00:31:35.816394 hello2-1.8.7/docs/source/hello.fiftyone.rst
+-rw-r--r--   0        0        0      154 2022-12-16 13:39:47.530383 hello2-1.8.7/docs/source/hello.fiftyone.tarinfo.rst
+-rw-r--r--   0        0        0      151 2022-11-04 14:14:10.800149 hello2-1.8.7/docs/source/hello.fiftyone.unique.rst
+-rw-r--r--   0        0        0      148 2022-11-22 16:10:13.239568 hello2-1.8.7/docs/source/hello.fiftyone.utils.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.800149 hello2-1.8.7/docs/source/hello.fiftyone.video.rst
+-rw-r--r--   0        0        0      145 2022-11-22 16:10:13.239568 hello2-1.8.7/docs/source/hello.fiftyone.view.rst
+-rw-r--r--   0        0        0      139 2023-04-29 13:47:19.090767 hello2-1.8.7/docs/source/hello.fvcore.core.rst
+-rw-r--r--   0        0        0      234 2023-04-29 13:47:19.090767 hello2-1.8.7/docs/source/hello.fvcore.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.800149 hello2-1.8.7/docs/source/hello.io.image.rst
+-rw-r--r--   0        0        0      237 2022-11-04 14:14:10.800149 hello2-1.8.7/docs/source/hello.io.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.810149 hello2-1.8.7/docs/source/hello.io.utils.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.810149 hello2-1.8.7/docs/source/hello.mmdet.export.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.810149 hello2-1.8.7/docs/source/hello.mmdet.flop.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.820149 hello2-1.8.7/docs/source/hello.mmdet.infer.rst
+-rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.8.7/docs/source/hello.mmdet.log.rst
+-rw-r--r--   0        0        0      136 2022-11-25 07:45:47.915124 hello2-1.8.7/docs/source/hello.mmdet.plot.rst
+-rw-r--r--   0        0        0      312 2022-11-25 07:45:47.915124 hello2-1.8.7/docs/source/hello.mmdet.rst
+-rw-r--r--   0        0        0      142 2023-05-29 00:31:35.816394 hello2-1.8.7/docs/source/hello.mmlab.mmdet3.rst
+-rw-r--r--   0        0        0      139 2023-05-29 00:31:35.816394 hello2-1.8.7/docs/source/hello.mmlab.mmseg.rst
+-rw-r--r--   0        0        0      253 2023-05-29 00:31:35.816394 hello2-1.8.7/docs/source/hello.mmlab.rst
+-rw-r--r--   0        0        0      139 2022-11-07 02:04:44.756679 hello2-1.8.7/docs/source/hello.mmseg.infer.rst
+-rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.8.7/docs/source/hello.mmseg.log.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.820149 hello2-1.8.7/docs/source/hello.mmseg.lr.rst
+-rw-r--r--   0        0        0      268 2022-11-07 02:04:44.756679 hello2-1.8.7/docs/source/hello.mmseg.rst
+-rw-r--r--   0        0        0      145 2023-04-20 14:38:58.266102 hello2-1.8.7/docs/source/hello.nanodet.infer.rst
+-rw-r--r--   0        0        0      239 2023-04-20 14:38:58.266102 hello2-1.8.7/docs/source/hello.nanodet.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.830149 hello2-1.8.7/docs/source/hello.onnx.export.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.830149 hello2-1.8.7/docs/source/hello.onnx.infer.rst
+-rw-r--r--   0        0        0      248 2022-11-04 14:14:10.830149 hello2-1.8.7/docs/source/hello.onnx.rst
+-rw-r--r--   0        0        0      415 2023-05-29 00:31:35.826394 hello2-1.8.7/docs/source/hello.rst
+-rw-r--r--   0        0        0      256 2022-11-04 14:14:10.840149 hello2-1.8.7/docs/source/hello.transforms.rst
+-rw-r--r--   0        0        0      169 2022-11-04 14:14:10.840149 hello2-1.8.7/docs/source/hello.transforms.transforms.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.8.7/docs/source/hello.utils.colors.rst
+-rw-r--r--   0        0        0      145 2023-05-29 00:31:35.826394 hello2-1.8.7/docs/source/hello.utils.compare.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.850149 hello2-1.8.7/docs/source/hello.utils.cuda.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.850149 hello2-1.8.7/docs/source/hello.utils.importer.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.850149 hello2-1.8.7/docs/source/hello.utils.plots.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.8.7/docs/source/hello.utils.points.rst
+-rw-r--r--   0        0        0      365 2023-05-29 00:31:35.826394 hello2-1.8.7/docs/source/hello.utils.rst
+-rw-r--r--   0        0        0      145 2022-11-30 10:15:09.976399 hello2-1.8.7/docs/source/hello.utils.strtime.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.860149 hello2-1.8.7/docs/source/hello.video.align.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.8.7/docs/source/hello.video.clip.rst
+-rw-r--r--   0        0        0      145 2023-04-20 14:38:58.306102 hello2-1.8.7/docs/source/hello.video.fisheye.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.8.7/docs/source/hello.video.frames.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.8.7/docs/source/hello.video.info.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.8.7/docs/source/hello.video.resize.rst
+-rw-r--r--   0        0        0      425 2023-04-20 14:38:58.296102 hello2-1.8.7/docs/source/hello.video.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.870149 hello2-1.8.7/docs/source/hello.video.rtsp.rst
+-rw-r--r--   0        0        0      153 2022-11-29 06:30:33.931961 hello2-1.8.7/docs/source/hello.video.rtsp_pull.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.8.7/docs/source/hello.video.split.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.870149 hello2-1.8.7/docs/source/hello.video.unwarp.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.8.7/docs/source/hello.video.utils.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.880149 hello2-1.8.7/docs/source/hello.x3m.config.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.8.7/docs/source/hello.x3m.preprocess.rst
+-rw-r--r--   0        0        0      272 2022-11-04 14:14:10.870149 hello2-1.8.7/docs/source/hello.x3m.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.8.7/docs/source/hello.x3m.transforms.rst
+-rw-r--r--   0        0        0      572 2022-11-04 15:19:50.508765 hello2-1.8.7/docs/source/index.rst
+-rw-r--r--   0        0        0       52 2022-11-04 14:40:30.829573 hello2-1.8.7/docs/source/modules.rst
+-rw-r--r--   0        0        0     3270 2023-06-06 04:22:36.459690 hello2-1.8.7/hello/README.md
+-rw-r--r--   0        0        0      773 2023-06-06 07:25:29.897368 hello2-1.8.7/hello/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.7/hello/__main__.py
+-rw-r--r--   0        0        0      471 2022-11-06 13:38:11.482015 hello2-1.8.7/hello/data/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.7/hello/data/__main__.py
+-rw-r--r--   0        0        0     3426 2022-08-30 01:19:13.615222 hello2-1.8.7/hello/data/coco2yolo.py
+-rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.8.7/hello/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.8.7/hello/experimental/albu/__init__.py
+-rw-r--r--   0        0        0      111 2022-12-11 06:23:09.504528 hello2-1.8.7/hello/experimental/albu/detection.py
+-rw-r--r--   0        0        0     1047 2022-11-06 13:38:17.442013 hello2-1.8.7/hello/fiftyone/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.7/hello/fiftyone/__main__.py
+-rw-r--r--   0        0        0     4742 2023-05-30 03:46:30.923445 hello2-1.8.7/hello/fiftyone/annotate.py
+-rw-r--r--   0        0        0    10588 2023-05-30 15:55:41.469982 hello2-1.8.7/hello/fiftyone/brain.py
+-rw-r--r--   0        0        0     8233 2023-05-29 00:31:35.826394 hello2-1.8.7/hello/fiftyone/coco.py
+-rw-r--r--   0        0        0     3945 2023-05-29 00:31:35.826394 hello2-1.8.7/hello/fiftyone/coco_utils.py
+-rw-r--r--   0        0        0      912 2023-04-25 01:47:26.910695 hello2-1.8.7/hello/fiftyone/connected.py
+-rw-r--r--   0        0        0       36 2022-11-18 04:25:30.455378 hello2-1.8.7/hello/fiftyone/copypaste.py
+-rw-r--r--   0        0        0    18009 2023-05-24 08:55:42.705839 hello2-1.8.7/hello/fiftyone/core.py
+-rw-r--r--   0        0        0    20251 2023-06-01 06:34:06.690322 hello2-1.8.7/hello/fiftyone/dataset.py
+-rw-r--r--   0        0        0     7502 2022-12-30 03:41:16.092249 hello2-1.8.7/hello/fiftyone/dataset_detections.py
+-rw-r--r--   0        0        0     5693 2022-12-30 03:45:01.362177 hello2-1.8.7/hello/fiftyone/dataset_segmentations.py
+-rw-r--r--   0        0        0     1402 2022-11-30 01:50:37.091070 hello2-1.8.7/hello/fiftyone/dataset_yolov5.py
+-rw-r--r--   0        0        0      889 2022-12-02 08:54:06.970245 hello2-1.8.7/hello/fiftyone/dataset_zoo.py
+-rw-r--r--   0        0        0     1169 2022-07-18 00:56:40.761934 hello2-1.8.7/hello/fiftyone/evaluate.py
+-rw-r--r--   0        0        0     5157 2023-03-07 04:04:15.369663 hello2-1.8.7/hello/fiftyone/evaluate_detections.py
+-rw-r--r--   0        0        0     4544 2023-03-07 04:04:11.609664 hello2-1.8.7/hello/fiftyone/evaluate_segmentations.py
+-rw-r--r--   0        0        0      103 2022-09-19 06:15:49.337504 hello2-1.8.7/hello/fiftyone/examples/README.md
+-rw-r--r--   0        0        0     2975 2022-11-30 01:46:25.831120 hello2-1.8.7/hello/fiftyone/examples/examples.py
+-rw-r--r--   0        0        0    12021 2023-01-09 09:33:51.046594 hello2-1.8.7/hello/fiftyone/examples/utils.py
+-rw-r--r--   0        0        0     3241 2023-05-19 07:54:24.980385 hello2-1.8.7/hello/fiftyone/gen_examples.py
+-rw-r--r--   0        0        0     2328 2023-05-29 00:31:35.826394 hello2-1.8.7/hello/fiftyone/mask_ignore.py
+-rw-r--r--   0        0        0     5683 2022-12-30 03:42:18.702230 hello2-1.8.7/hello/fiftyone/miou.py
+-rw-r--r--   0        0        0     2639 2022-11-18 06:29:39.594231 hello2-1.8.7/hello/fiftyone/patches.py
+-rw-r--r--   0        0        0     9311 2023-05-29 00:31:35.826394 hello2-1.8.7/hello/fiftyone/tarinfo.py
+-rw-r--r--   0        0        0     4094 2023-03-15 08:42:32.674825 hello2-1.8.7/hello/fiftyone/unique.py
+-rw-r--r--   0        0        0     8090 2023-05-29 00:31:35.826394 hello2-1.8.7/hello/fiftyone/utils.py
+-rw-r--r--   0        0        0      781 2022-12-01 14:14:43.560707 hello2-1.8.7/hello/fiftyone/video.py
+-rw-r--r--   0        0        0    10678 2023-06-05 03:32:36.498706 hello2-1.8.7/hello/fiftyone/view.py
+-rw-r--r--   0        0        0      435 2022-10-20 14:18:34.575285 hello2-1.8.7/hello/fvcore/README.md
+-rw-r--r--   0        0        0        0 2022-11-04 14:49:06.729395 hello2-1.8.7/hello/fvcore/__init__.py
+-rw-r--r--   0        0        0     1080 2023-04-29 13:43:43.400786 hello2-1.8.7/hello/fvcore/core.py
+-rw-r--r--   0        0        0      135 2022-06-27 01:46:45.026108 hello2-1.8.7/hello/io/__init__.py
+-rw-r--r--   0        0        0     1382 2022-08-23 09:20:12.751790 hello2-1.8.7/hello/io/image.py
+-rw-r--r--   0        0        0      989 2023-05-29 00:31:35.826394 hello2-1.8.7/hello/io/utils.py
+-rw-r--r--   0        0        0      851 2022-11-25 07:46:45.875120 hello2-1.8.7/hello/mmdet/__init__.py
+-rw-r--r--   0        0        0       67 2022-10-17 07:49:46.479528 hello2-1.8.7/hello/mmdet/__main__.py
+-rw-r--r--   0        0        0       97 2022-10-17 08:00:01.479443 hello2-1.8.7/hello/mmdet/export.py
+-rw-r--r--   0        0        0     1736 2022-10-20 16:17:29.762828 hello2-1.8.7/hello/mmdet/flop.py
+-rw-r--r--   0        0        0     5446 2023-03-03 15:16:46.611009 hello2-1.8.7/hello/mmdet/infer.py
+-rw-r--r--   0        0        0     3273 2023-04-11 07:00:00.274582 hello2-1.8.7/hello/mmdet/log.py
+-rw-r--r--   0        0        0     5976 2023-04-12 11:23:04.178651 hello2-1.8.7/hello/mmdet/plot.py
+-rw-r--r--   0        0        0      563 2023-05-12 07:19:19.396722 hello2-1.8.7/hello/mmlab/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-12 07:16:55.756771 hello2-1.8.7/hello/mmlab/__main__.py
+-rw-r--r--   0        0        0      110 2023-05-12 07:26:47.136571 hello2-1.8.7/hello/mmlab/mmdet3.py
+-rw-r--r--   0        0        0     6549 2023-05-15 09:18:13.003946 hello2-1.8.7/hello/mmlab/mmseg.py
+-rw-r--r--   0        0        0      645 2022-11-07 02:04:01.296693 hello2-1.8.7/hello/mmseg/__init__.py
+-rw-r--r--   0        0        0       67 2022-10-31 01:39:47.674470 hello2-1.8.7/hello/mmseg/__main__.py
+-rw-r--r--   0        0        0     6040 2022-11-09 01:29:31.447414 hello2-1.8.7/hello/mmseg/infer.py
+-rw-r--r--   0        0        0     2368 2023-04-11 07:03:55.124501 hello2-1.8.7/hello/mmseg/log.py
+-rw-r--r--   0        0        0     7006 2022-12-01 12:09:30.751861 hello2-1.8.7/hello/mmseg/lr.py
+-rw-r--r--   0        0        0      462 2023-03-29 08:04:38.934968 hello2-1.8.7/hello/nanodet/__init__.py
+-rw-r--r--   0        0        0       67 2023-03-29 08:03:09.784974 hello2-1.8.7/hello/nanodet/__main__.py
+-rw-r--r--   0        0        0     7410 2023-04-06 10:19:32.462564 hello2-1.8.7/hello/nanodet/infer.py
+-rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.8.7/hello/onnx/__init__.py
+-rw-r--r--   0        0        0      213 2022-06-27 02:15:25.376085 hello2-1.8.7/hello/onnx/examples/README.md
+-rw-r--r--   0        0        0     1879 2022-06-27 01:46:45.026108 hello2-1.8.7/hello/onnx/examples/test_sigmoid.py
+-rw-r--r--   0        0        0     3024 2022-08-30 07:45:32.884923 hello2-1.8.7/hello/onnx/export.py
+-rw-r--r--   0        0        0     1707 2022-08-22 07:09:07.802604 hello2-1.8.7/hello/onnx/infer.py
+-rw-r--r--   0        0        0     1334 2022-11-21 14:14:37.239473 hello2-1.8.7/hello/transforms/README.md
+-rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.8.7/hello/transforms/__init__.py
+-rw-r--r--   0        0        0     2655 2022-11-21 15:01:54.364062 hello2-1.8.7/hello/transforms/transforms.py
+-rw-r--r--   0        0        0        0 2022-07-20 06:21:09.967902 hello2-1.8.7/hello/utils/__init__.py
+-rw-r--r--   0        0        0     2133 2023-05-19 03:21:05.796070 hello2-1.8.7/hello/utils/colors.py
+-rw-r--r--   0        0        0     1349 2023-05-29 00:31:35.826394 hello2-1.8.7/hello/utils/compare.py
+-rw-r--r--   0        0        0     1815 2022-10-14 02:36:42.461531 hello2-1.8.7/hello/utils/cuda.py
+-rw-r--r--   0        0        0      356 2022-07-20 06:43:22.727885 hello2-1.8.7/hello/utils/importer.py
+-rw-r--r--   0        0        0      612 2022-08-23 06:44:50.231910 hello2-1.8.7/hello/utils/plots.py
+-rw-r--r--   0        0        0     2999 2022-11-06 13:40:43.281966 hello2-1.8.7/hello/utils/points.py
+-rw-r--r--   0        0        0      195 2022-11-30 01:25:21.821313 hello2-1.8.7/hello/utils/strtime.py
+-rw-r--r--   0        0        0     1135 2023-02-20 08:24:47.078416 hello2-1.8.7/hello/video/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.7/hello/video/__main__.py
+-rw-r--r--   0        0        0     3428 2022-11-06 13:15:37.862480 hello2-1.8.7/hello/video/align.py
+-rw-r--r--   0        0        0     6382 2023-05-17 04:07:48.740198 hello2-1.8.7/hello/video/clip.py
+-rw-r--r--   0        0        0     3290 2023-02-20 09:35:59.918194 hello2-1.8.7/hello/video/fisheye.py
+-rw-r--r--   0        0        0     1565 2022-11-06 13:15:49.722478 hello2-1.8.7/hello/video/info.py
+-rw-r--r--   0        0        0     3502 2022-11-06 13:15:55.532477 hello2-1.8.7/hello/video/resize.py
+-rw-r--r--   0        0        0     4716 2022-11-29 07:15:17.421543 hello2-1.8.7/hello/video/rtsp.py
+-rw-r--r--   0        0        0     5006 2022-11-29 08:00:32.141119 hello2-1.8.7/hello/video/rtsp_pull.py
+-rw-r--r--   0        0        0     3048 2022-11-11 09:35:15.036742 hello2-1.8.7/hello/video/split.py
+-rw-r--r--   0        0        0     4066 2023-02-20 08:27:40.638408 hello2-1.8.7/hello/video/unwarp.py
+-rw-r--r--   0        0        0      968 2022-08-25 04:09:32.554890 hello2-1.8.7/hello/video/utils.py
+-rw-r--r--   0        0        0      576 2022-11-06 13:41:08.801958 hello2-1.8.7/hello/x3m/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.8.7/hello/x3m/__main__.py
+-rw-r--r--   0        0        0     4787 2023-06-06 07:24:27.477380 hello2-1.8.7/hello/x3m/config.py
+-rw-r--r--   0        0        0     2592 2022-08-30 01:19:13.615222 hello2-1.8.7/hello/x3m/preprocess.py
+-rw-r--r--   0        0        0     6928 2022-06-27 01:46:45.026108 hello2-1.8.7/hello/x3m/transforms.py
+-rw-r--r--   0        0        0      808 2022-06-27 01:46:45.026108 hello2-1.8.7/hello_c/CMakeLists.txt
+-rw-r--r--   0        0        0      776 2022-06-27 01:46:45.026108 hello2-1.8.7/hello_c/README.md
+-rw-r--r--   0        0        0     1375 2022-06-27 01:46:45.026108 hello2-1.8.7/hello_c/main.cpp
+-rw-r--r--   0        0        0      262 2022-06-27 01:46:45.026108 hello2-1.8.7/hello_c/trace_model.py
+-rw-r--r--   0        0        0      787 2023-05-15 09:28:06.783743 hello2-1.8.7/pyproject.toml
+-rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 hello2-1.8.7/PKG-INFO
```

### Comparing `hello2-1.8.6/.gitignore` & `hello2-1.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/.readthedocs.yaml` & `hello2-1.8.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/LICENSE` & `hello2-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/docs/Makefile` & `hello2-1.8.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/docs/make.bat` & `hello2-1.8.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/docs/source/conf.py` & `hello2-1.8.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/docs/source/hello.fiftyone.rst` & `hello2-1.8.7/docs/source/hello.fiftyone.rst`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/docs/source/index.rst` & `hello2-1.8.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/README.md` & `hello2-1.8.7/hello/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 # OpenCV
 pip uninstall -y opencv-python-headless
 pip install opencv-python --ignore-installed
 
 # fiftyone
 pip install --upgrade fiftyone
-pip install fiftyone>=0.20.1
+pip install fiftyone>=0.21.0
 
 # pyomniunwarp
 pip install -U pyomniunwarp>=0.2.4
 
 # onnxruntime (optional)
 pip install onnx onnx-simplifier onnxruntime  # CPU
 pip install onnx onnx-simplifier onnxruntime-gpu  # GPU
```

### Comparing `hello2-1.8.6/hello/__init__.py` & `hello2-1.8.7/hello/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "1.8.6"
+__version__ = "1.8.7"
 
 help_doc_str = """\
 usage: hello [--version] [--help]
 
 shell command:
     hello -h
     hello-data -h
```

### Comparing `hello2-1.8.6/hello/data/coco2yolo.py` & `hello2-1.8.7/hello/data/coco2yolo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/__init__.py` & `hello2-1.8.7/hello/fiftyone/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/annotate.py` & `hello2-1.8.7/hello/fiftyone/annotate.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/brain.py` & `hello2-1.8.7/hello/fiftyone/brain.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/coco.py` & `hello2-1.8.7/hello/fiftyone/coco.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/coco_utils.py` & `hello2-1.8.7/hello/fiftyone/coco_utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/connected.py` & `hello2-1.8.7/hello/fiftyone/connected.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/core.py` & `hello2-1.8.7/hello/fiftyone/core.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/dataset.py` & `hello2-1.8.7/hello/fiftyone/dataset.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/dataset_detections.py` & `hello2-1.8.7/hello/fiftyone/dataset_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/dataset_segmentations.py` & `hello2-1.8.7/hello/fiftyone/dataset_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/dataset_yolov5.py` & `hello2-1.8.7/hello/fiftyone/dataset_yolov5.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/dataset_zoo.py` & `hello2-1.8.7/hello/fiftyone/dataset_zoo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/evaluate.py` & `hello2-1.8.7/hello/fiftyone/evaluate.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/evaluate_detections.py` & `hello2-1.8.7/hello/fiftyone/evaluate_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/evaluate_segmentations.py` & `hello2-1.8.7/hello/fiftyone/evaluate_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/examples/examples.py` & `hello2-1.8.7/hello/fiftyone/examples/examples.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/examples/utils.py` & `hello2-1.8.7/hello/fiftyone/examples/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/gen_examples.py` & `hello2-1.8.7/hello/fiftyone/gen_examples.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/mask_ignore.py` & `hello2-1.8.7/hello/fiftyone/mask_ignore.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/miou.py` & `hello2-1.8.7/hello/fiftyone/miou.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/patches.py` & `hello2-1.8.7/hello/fiftyone/patches.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/tarinfo.py` & `hello2-1.8.7/hello/fiftyone/tarinfo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/unique.py` & `hello2-1.8.7/hello/fiftyone/unique.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/utils.py` & `hello2-1.8.7/hello/fiftyone/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/video.py` & `hello2-1.8.7/hello/fiftyone/video.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/fiftyone/view.py` & `hello2-1.8.7/hello/fiftyone/view.py`

 * *Files 11% similar despite different names*

```diff
@@ -84,24 +84,51 @@
     sorted_ids = [x[1] for x in data]
 
     view = dataset.select(sorted_ids, ordered=True)
 
     return view
 
 
+def match_labels(dataset, labels=None, ids=None, tags=None, filter=None, fields=None, bool=None):
+    """Selects the samples from the collection that contain (or do not
+    contain) at least one label that matches the specified criteria.
+
+    Note that, unlike :meth:`select_labels` and :meth:`filter_labels`, this
+    stage will not filter the labels themselves; it only selects the
+    corresponding samples.
+
+    Args:
+        dataset: a :class:`fiftyone.core.collections.SampleCollection`
+        labels (None): by :meth:`fiftyone.core.session.Session.selected_labels`
+        ids (None): an ID or iterable of IDs of the labels to select
+        tags (None): a tag or iterable of tags of labels to select
+        filter (None): a :class:`fiftyone.core.expressions.ViewExpression`
+        fields (None): a field or iterable of fields from which to select
+        bool (None): have (None or True) or do not have (False) at least one label
+
+    Returns:
+        a :class:`fiftyone.core.view.DatasetView`
+    """
+    view = dataset.match_labels(labels=labels, ids=ids, tags=tags, filter=filter, fields=fields, bool=bool)
+    return view
+
+
 def select_labels(dataset, labels=None, ids=None, tags=None, fields=None, omit_empty=True):
     """Selects only the specified labels from the collection.
 
     Args:
         dataset: a :class:`fiftyone.core.collections.SampleCollection`
         labels (None):  a list of dicts specifying the labels to select in the format returned by :func:`fiftyone.core.session.Session.selected_labels()`
         ids (None): an ID or iterable of IDs of the labels to select
         tags (None): a tag or iterable of tags of labels to select
         fields (None): a field or iterable of fields from which to select
         omit_empty (True): whether to omit samples that have no labels after filtering
+
+    Returns:
+        a :class:`fiftyone.core.view.DatasetView`
     """
     view = dataset.select_labels(labels=labels, ids=ids, tags=tags, fields=fields, omit_empty=omit_empty)
     return view
 
 
 def exclude_labels(dataset, labels=None, ids=None, tags=None, fields=None, omit_empty=True):
     """Excludes the specified labels from the collection.
@@ -109,14 +136,17 @@
     Args:
         dataset: a :class:`fiftyone.core.collections.SampleCollection`
         labels (None):  a list of dicts specifying the labels to exclude in the format returned by :func:`fiftyone.core.session.Session.selected_labels()`
         ids (None): an ID or iterable of IDs of the labels to exclude
         tags (None): a tag or iterable of tags of labels to exclude
         fields (None): a field or iterable of fields from which to exclude
         omit_empty (True): whether to omit samples that have no labels after filtering
+
+    Returns:
+        a :class:`fiftyone.core.view.DatasetView`
     """
     view = dataset.exclude_labels(labels=labels, ids=ids, tags=tags, fields=fields, omit_empty=omit_empty)
     return view
 
 
 def filter_field(dataset, field, a, op, b, only_matches=True):
     """Filters the values of a field or embedded field of each sample in the collection.
@@ -203,7 +233,40 @@
         iscrowd (None): an optional name of a boolean attribute
         classwise (False): different label values as always non-overlapping
     """
     dup_ids = foui.find_duplicates(dataset, label_field, iou_thresh=iou_thresh, method=method, iscrowd=iscrowd, classwise=classwise)
 
     view = dataset.match_labels(ids=dup_ids, fields=label_field)
     return view
+
+
+def set_values(dataset, field_name, values, **kwargs):
+    """Sets the field or embedded field on each sample or frame in the
+    collection to the given values.
+
+    Args:
+        dataset: a :class:`fiftyone.core.collections.SampleCollection`
+        field_name: a field or ``embedded.field.name``
+        values: an iterable of values, one for each sample in the collection
+    """
+    dataset.set_values(field_name, values, **kwargs)
+
+
+def set_label_values(dataset, field_name, values, **kwargs):
+    """Sets the fields of the specified labels in the collection to the
+    given values.
+
+    Examples::
+
+        view = dataset.filter_labels("predictions", F("confidence") > 0.99)
+
+        label_ids = view.values("predictions.detections.id", unwind=True)
+        values = {_id: True for _id in label_ids}
+
+        dataset.set_label_values("predictions.detections.high_conf", values)
+
+    Args:
+        dataset: a :class:`fiftyone.core.collections.SampleCollection`
+        field_name: a field or ``embedded.field.name``
+        values: a dict mapping label IDs to values
+    """
+    dataset.set_label_values(field_name, values, **kwargs)
```

### Comparing `hello2-1.8.6/hello/fvcore/core.py` & `hello2-1.8.7/hello/fvcore/core.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/io/image.py` & `hello2-1.8.7/hello/io/image.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/io/utils.py` & `hello2-1.8.7/hello/io/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmdet/__init__.py` & `hello2-1.8.7/hello/mmdet/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmdet/flop.py` & `hello2-1.8.7/hello/mmdet/flop.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmdet/infer.py` & `hello2-1.8.7/hello/mmdet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmdet/log.py` & `hello2-1.8.7/hello/mmdet/log.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmdet/plot.py` & `hello2-1.8.7/hello/mmdet/plot.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmlab/__init__.py` & `hello2-1.8.7/hello/mmlab/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmlab/mmseg.py` & `hello2-1.8.7/hello/mmlab/mmseg.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmseg/__init__.py` & `hello2-1.8.7/hello/mmseg/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmseg/infer.py` & `hello2-1.8.7/hello/mmseg/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmseg/log.py` & `hello2-1.8.7/hello/mmseg/log.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/mmseg/lr.py` & `hello2-1.8.7/hello/mmseg/lr.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/nanodet/infer.py` & `hello2-1.8.7/hello/nanodet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/onnx/examples/test_sigmoid.py` & `hello2-1.8.7/hello/onnx/examples/test_sigmoid.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/onnx/export.py` & `hello2-1.8.7/hello/onnx/export.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/onnx/infer.py` & `hello2-1.8.7/hello/onnx/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/transforms/README.md` & `hello2-1.8.7/hello/transforms/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/transforms/transforms.py` & `hello2-1.8.7/hello/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/utils/colors.py` & `hello2-1.8.7/hello/utils/colors.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/utils/compare.py` & `hello2-1.8.7/hello/utils/compare.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/utils/cuda.py` & `hello2-1.8.7/hello/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/utils/plots.py` & `hello2-1.8.7/hello/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/utils/points.py` & `hello2-1.8.7/hello/utils/points.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/__init__.py` & `hello2-1.8.7/hello/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/align.py` & `hello2-1.8.7/hello/video/align.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/clip.py` & `hello2-1.8.7/hello/video/clip.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/fisheye.py` & `hello2-1.8.7/hello/video/fisheye.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/info.py` & `hello2-1.8.7/hello/video/info.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/resize.py` & `hello2-1.8.7/hello/video/resize.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/rtsp.py` & `hello2-1.8.7/hello/video/rtsp.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/rtsp_pull.py` & `hello2-1.8.7/hello/video/rtsp_pull.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/split.py` & `hello2-1.8.7/hello/video/split.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/unwarp.py` & `hello2-1.8.7/hello/video/unwarp.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/video/utils.py` & `hello2-1.8.7/hello/video/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/x3m/__init__.py` & `hello2-1.8.7/hello/x3m/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/x3m/config.py` & `hello2-1.8.7/hello/x3m/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 tmpl_f32 = """\
 # X3M SDK: Version_20220512
 # https://developer.horizon.ai/api/v1/fileData/documents/ai_toolchain_develop/horizon_ai_toolchain_user_guide/chapter_3_model_conversion.html#model-conversion
 model_parameters:
   onnx_model: '{onnx_model}'
   march: 'bernoulli2'
-  layer_out_dump: False
-  log_level: 'debug'
-  working_dir: 'model_output'
   output_model_file_prefix: '{model_prefix}'
+  working_dir: './model_output'
+  layer_out_dump: False
 
 input_parameters:
   input_name: '{input_name}'
   input_type_rt: '{input_type_rt}'
   input_layout_rt: '{input_layout_rt}'
   input_type_train: '{input_type_train}'
   input_layout_train: '{input_layout_train}'
+  input_space_and_range: '{input_space_and_range}'
   input_shape: ''
   input_batch: 1
   norm_type: '{norm_type}'
   mean_value: '{mean_value}'
   scale_value: '{scale_value}'
 
 calibration_parameters:
   cal_data_dir: '{cal_data_dir}'
+  cal_data_type: '{cal_data_type}'
   calibration_type: '{calibration_type}'
   max_percentile: {max_percentile}
   per_channel: {per_channel}
-  preprocess_on: False
 
 compiler_parameters:
   compile_mode: '{compile_mode}'
   debug: {compile_debug}
   core_num: {core_num}
   optimize_level: '{optimize_level}'
 """
@@ -59,33 +59,37 @@
     parser.add_argument("mode", type=str,
                         choices=["f32", "qat"])
     parser.add_argument("onnx_model", type=str,
                         help="the model file of ONNX")
     parser.add_argument("--model-prefix", type=str, default=None,
                         help="model conversion generated name prefix")
 
-    parser.add_argument("--input-name", type=str, default="images",
+    parser.add_argument("--input-name", type=str, default="data",
                         help="node name of model input")
     parser.add_argument("--input-type-rt", type=str, default="nv12",
                         choices=["nv12", "rgb", "bgr", "gray", "featuremap", "yuv444"])
     parser.add_argument("--input-layout-rt", type=str, default="",
                         choices=["NHWC", "NCHW"])
     parser.add_argument("--input-type-train", type=str, default="rgb",
                         choices=["rgb", "bgr", "gray", "featuremap", "yuv444"])
     parser.add_argument("--input-layout-train", type=str, default="NCHW",
                         choices=["NHWC", "NCHW"])
+    parser.add_argument("--input-space-and-range", type=str, default="regular",
+                        choices=["regular", "bt601_video"])
     parser.add_argument("--norm-type", type=str, default="data_scale",
                         choices=["no_preprocess", "data_mean", "data_scale", "data_mean_and_scale"])
     parser.add_argument("--mean-value", type=str, default="",
                         help="values must be seperated by space")
     parser.add_argument("--scale-value", type=str, default="0.003921568627451",
                         help="values must be seperated by space")
 
     parser.add_argument("--cal-data-dir", type=str, default="./calibration_data_rgb_f32",
                         help="reference images of model quantization")
+    parser.add_argument("--cal-data-type", type=str, default="float32",
+                        choices=["float32", "uint8"])
     parser.add_argument("--calibration-type", type=str, default="default",
                         choices=["kl", "max", "default", "load"])
     parser.add_argument("--max-percentile", type=str, default="1.0",
                         help="valid when `calibration_type=max`, range 0.0 - 1.0.")
     parser.add_argument("--per-channel", type=str, default="False",
                         choices=["False", "True"])
```

### Comparing `hello2-1.8.6/hello/x3m/preprocess.py` & `hello2-1.8.7/hello/x3m/preprocess.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello/x3m/transforms.py` & `hello2-1.8.7/hello/x3m/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello_c/CMakeLists.txt` & `hello2-1.8.7/hello_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello_c/README.md` & `hello2-1.8.7/hello_c/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/hello_c/main.cpp` & `hello2-1.8.7/hello_c/main.cpp`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/pyproject.toml` & `hello2-1.8.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hello2-1.8.6/PKG-INFO` & `hello2-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello2
-Version: 1.8.6
+Version: 1.8.7
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: scikit-image
@@ -57,15 +57,15 @@
 
 # OpenCV
 pip uninstall -y opencv-python-headless
 pip install opencv-python --ignore-installed
 
 # fiftyone
 pip install --upgrade fiftyone
-pip install fiftyone>=0.20.1
+pip install fiftyone>=0.21.0
 
 # pyomniunwarp
 pip install -U pyomniunwarp>=0.2.4
 
 # onnxruntime (optional)
 pip install onnx onnx-simplifier onnxruntime  # CPU
 pip install onnx onnx-simplifier onnxruntime-gpu  # GPU
```

