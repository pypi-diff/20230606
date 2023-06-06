# Comparing `tmp/onvif-gui-1.2.2.tar.gz` & `tmp/onvif-gui-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.2.2.tar", last modified: Tue May 30 18:09:59 2023, max compression
+gzip compressed data, was "onvif-gui-1.2.3.tar", last modified: Tue Jun  6 16:18:04 2023, max compression
```

## Comparing `onvif-gui-1.2.2.tar` & `onvif-gui-1.2.3.tar`

### file list

```diff
@@ -1,307 +1,308 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.045680 onvif-gui-1.2.2/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11558 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      221 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-30 18:09:59.045680 onvif-gui-1.2.2/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8359 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/README.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.021680 onvif-gui-1.2.2/detectron2/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       68 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.021680 onvif-gui-1.2.2/detectron2/checkpoint/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      357 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/checkpoint/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18177 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/checkpoint/c2_model_loading.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5800 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/checkpoint/catalog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5379 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.021680 onvif-gui-1.2.2/detectron2/config/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      623 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/config/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8119 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/config/compat.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9476 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/config/config.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    30158 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/config/defaults.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3103 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/config/instantiate.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15786 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/config/lazy.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.021680 onvif-gui-1.2.2/detectron2/configs/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1360 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/configs/Base-RCNN-FPN.yaml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.021680 onvif-gui-1.2.2/detectron2/configs/COCO-InstanceSegmentation/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/configs/COCO-InstanceSegmentation/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      201 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.021680 onvif-gui-1.2.2/detectron2/configs/COCO-Keypoints/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      542 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/configs/COCO-Keypoints/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      190 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/configs/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.021680 onvif-gui-1.2.2/detectron2/data/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      663 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7603 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/benchmark.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21787 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7460 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/catalog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9406 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/common.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8360 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/dataset_mapper.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.025680 onvif-gui-1.2.2/detectron2/data/datasets/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10433 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/builtin.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    22191 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/builtin_meta.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13496 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/cityscapes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8008 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/cityscapes_panoptic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24004 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/coco.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9205 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/coco_panoptic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9864 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/lvis.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   223770 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   219193 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/lvis_v1_categories.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    39434 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3210 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/pascal_voc.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/datasets/register_coco.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23487 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/detection_utils.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.025680 onvif-gui-1.2.2/detectron2/data/samplers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      429 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/samplers/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12067 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/samplers/distributed_sampler.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1991 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.025680 onvif-gui-1.2.2/detectron2/data/transforms/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      480 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/transforms/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14492 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/transforms/augmentation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23683 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/transforms/augmentation_impl.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12980 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/data/transforms/transform.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.025680 onvif-gui-1.2.2/detectron2/layers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      900 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5908 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/aspp.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12431 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/batch_norm.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3135 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/blocks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17492 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/deform_conv.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4335 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/losses.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11154 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/mask_ops.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6629 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/nms.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3172 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/roi_align.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3393 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/roi_align_rotated.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/rotated_boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      555 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/shape_spec.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5271 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/layers/wrappers.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.025680 onvif-gui-1.2.2/detectron2/modeling/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1632 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15825 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/anchor_generator.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.025680 onvif-gui-1.2.2/detectron2/modeling/backbone/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2586 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/backbone.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1048 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10628 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16434 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/mvit.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17108 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/regnet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24352 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/resnet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25785 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/swin.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6546 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19860 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/backbone/vit.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15492 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/box_regression.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6391 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/matcher.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.029680 onvif-gui-1.2.2/detectron2/modeling/meta_arch/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      524 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/meta_arch/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      839 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/meta_arch/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11940 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/meta_arch/dense_detector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13541 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/meta_arch/fcos.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10676 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14237 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/meta_arch/rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18704 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/meta_arch/retinanet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10173 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/meta_arch/semantic_seg.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11104 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/mmdet_wrapper.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11575 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/poolers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4145 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/postprocessing.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.029680 onvif-gui-1.2.2/detectron2/modeling/proposal_generator/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      236 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/proposal_generator/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      860 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/proposal_generator/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8333 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24347 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/proposal_generator/rpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9016 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.029680 onvif-gui-1.2.2/detectron2/modeling/roi_heads/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      797 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/roi_heads/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4195 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/roi_heads/box_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13289 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25959 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11428 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/roi_heads/keypoint_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12467 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/roi_heads/mask_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    38578 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/roi_heads/roi_heads.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11446 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2388 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/sampling.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12723 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/modeling/test_time_augmentation.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1829 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/predictor.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.029680 onvif-gui-1.2.2/detectron2/structures/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      662 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/structures/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14854 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/structures/boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5649 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/structures/image_list.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6807 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/structures/instances.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9269 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/structures/keypoints.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    20336 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/structures/masks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19356 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/structures/rotated_boxes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2775 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/tracker.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.029680 onvif-gui-1.2.2/detectron2/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       52 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6205 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/analysis.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8633 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/collect_env.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4254 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/colormap.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5807 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/comm.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1911 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/develop.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5814 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/env.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17508 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/events.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1226 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/file_io.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8044 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/logger.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2667 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/memory.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1934 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/registry.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1096 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/serialize.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18576 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/testing.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11606 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/video_visualizer.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    52426 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/detectron2/utils/visualizer.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.029680 onvif-gui-1.2.2/gui/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       28 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.029680 onvif-gui-1.2.2/gui/components/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      286 2023-05-30 01:46:34.000000 onvif-gui-1.2.2/gui/components/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1824 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/components/comboselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2459 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/components/directoryselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2172 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/components/fileselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5508 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/components/labelselector.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4194 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/components/progress.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1962 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/components/thresholdslider.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      831 2023-05-30 01:46:34.000000 onvif-gui-1.2.2/gui/components/waitdialog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/glwidget.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15800 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/gui/main.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.033680 onvif-gui-1.2.2/gui/onvif/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/onvif/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5870 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/onvif/admintab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4051 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/onvif/imagetab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2484 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/onvif/logindialog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5364 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/onvif/networktab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5241 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/onvif/ptztab.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4640 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/onvif/videotab.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.033680 onvif-gui-1.2.2/gui/panels/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      184 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/panels/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3802 2023-05-30 01:46:34.000000 onvif-gui-1.2.2/gui/panels/audiopanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13667 2023-05-30 01:46:34.000000 onvif-gui-1.2.2/gui/panels/camerapanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14756 2023-05-30 01:46:34.000000 onvif-gui-1.2.2/gui/panels/filepanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13666 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/gui/panels/settingspanel.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3806 2023-05-30 01:46:34.000000 onvif-gui-1.2.2/gui/panels/videopanel.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.041680 onvif-gui-1.2.2/gui/resources/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2021 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      252 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/apply.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/apply_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      244 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/apply_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      911 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/audio.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/audio_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      920 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/audio_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      203 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/branch_closed.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      219 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/branch_closed_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      211 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/branch_closed_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      199 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/branch_open.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      168 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/branch_open_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/branch_open_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      267 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/checked.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/checked_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      246 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/checked_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13358 2023-05-30 01:46:34.000000 onvif-gui-1.2.2/gui/resources/darkstyle.qss
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      910 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/discover.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      849 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/discover_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      937 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/discover_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/fast-forward.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      253 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/fast-forward_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      433 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/fast-forward_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/mute.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      346 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/mute_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/mute_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/next.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      225 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/next_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/next_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    46084 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/onvif-gui.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/pause.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      144 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/pause_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/pause_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      321 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/play.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      209 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/play_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/play_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      349 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/previous.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      232 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/previous_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/previous_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/radio-off.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/radio-off_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/radio-off_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      350 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/radio-on.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      263 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/radio-on_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      343 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/radio-on_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      395 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/record.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      394 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/record_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/record_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      408 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/recording.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      435 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/recording_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/recording_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      454 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/rewind.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/rewind_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      457 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/rewind_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      187 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/small_arrow_left.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      183 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/small_arrow_left_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      189 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/small_arrow_left_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/small_arrow_up.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      160 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/small_arrow_up_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      161 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/small_arrow_up_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19236 2023-05-30 01:46:34.000000 onvif-gui-1.2.2/gui/resources/spinner.gif
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      158 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/stop.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      140 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/stop_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/stop_lo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/unchecked.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/unchecked_hi.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/gui/resources/unchecked_lo.png
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.041680 onvif-gui-1.2.2/modules/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/modules/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.041680 onvif-gui-1.2.2/modules/audio/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/modules/audio/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3492 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/modules/audio/sample.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.041680 onvif-gui-1.2.2/modules/video/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/modules/video/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8731 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/modules/video/keypoint.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6117 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/modules/video/retinanet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3244 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/modules/video/sample.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9262 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/modules/video/segment.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12122 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/modules/video/yolov7.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11384 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/modules/video/yolov8.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12692 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/modules/video/yolox.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.041680 onvif-gui-1.2.2/onvif_gui.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-30 18:09:59.000000 onvif-gui-1.2.2/onvif_gui.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8447 2023-05-30 18:09:59.000000 onvif-gui-1.2.2/onvif_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-30 18:09:59.000000 onvif-gui-1.2.2/onvif_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       39 2023-05-30 18:09:59.000000 onvif-gui-1.2.2/onvif_gui.egg-info/entry_points.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       47 2023-05-30 18:09:59.000000 onvif-gui-1.2.2/onvif_gui.egg-info/requires.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       44 2023-05-30 18:09:59.000000 onvif-gui-1.2.2/onvif_gui.egg-info/top_level.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1688 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-30 18:09:59.045680 onvif-gui-1.2.2/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1549 2023-05-30 18:08:51.000000 onvif-gui-1.2.2/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.041680 onvif-gui-1.2.2/tracker/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/tracker/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1003 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/tracker/basetrack.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12632 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/tracker/byte_tracker.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9816 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/tracker/kalman_filter.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6304 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/tracker/matching.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.041680 onvif-gui-1.2.2/yolov7/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.041680 onvif-gui-1.2.2/yolov7/models/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/models/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    86435 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/models/common.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11177 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/models/experimental.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    40895 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/models/yolo.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.045680 onvif-gui-1.2.2/yolov7/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2320 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/activations.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5771 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/add_nms.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7321 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/autoanchor.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    57559 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/datasets.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    37789 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/general.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4996 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/google_utils.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    76741 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/loss.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9537 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/metrics.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21424 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/plots.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15840 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolov7/utils/torch_utils.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.045680 onvif-gui-1.2.2/yolox/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.045680 onvif-gui-1.2.2/yolox/models/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      961 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5019 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/build.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6840 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/darknet.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2372 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/losses.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6944 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/network_blocks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3202 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/yolo_fpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26204 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/yolo_head.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4288 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/yolo_pafpn.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2054 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/models/yolox.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-30 18:09:59.045680 onvif-gui-1.2.2/yolox/utils/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      130 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/utils/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1628 2023-05-25 17:26:34.000000 onvif-gui-1.2.2/yolox/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.531755 onvif-gui-1.2.3/
+-rw-rw-rw-   0        0        0    11558 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      221 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     9056 2023-06-06 16:18:04.530759 onvif-gui-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8359 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.817764 onvif-gui-1.2.3/detectron2/
+-rw-rw-rw-   0        0        0       68 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.832715 onvif-gui-1.2.3/detectron2/checkpoint/
+-rw-rw-rw-   0        0        0      357 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/checkpoint/__init__.py
+-rw-rw-rw-   0        0        0    18177 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/checkpoint/c2_model_loading.py
+-rw-rw-rw-   0        0        0     5800 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/checkpoint/catalog.py
+-rw-rw-rw-   0        0        0     5379 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.855638 onvif-gui-1.2.3/detectron2/config/
+-rw-rw-rw-   0        0        0      623 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/__init__.py
+-rw-rw-rw-   0        0        0     8119 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/compat.py
+-rw-rw-rw-   0        0        0     9476 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/config.py
+-rw-rw-rw-   0        0        0    30158 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/defaults.py
+-rw-rw-rw-   0        0        0     3103 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/instantiate.py
+-rw-rw-rw-   0        0        0    15786 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/config/lazy.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.858628 onvif-gui-1.2.3/detectron2/configs/
+-rw-rw-rw-   0        0        0     1360 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/Base-RCNN-FPN.yaml
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.861618 onvif-gui-1.2.3/detectron2/configs/COCO-InstanceSegmentation/
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.866956 onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/
+-rw-rw-rw-   0        0        0      542 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.891875 onvif-gui-1.2.3/detectron2/data/
+-rw-rw-rw-   0        0        0      663 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/__init__.py
+-rw-rw-rw-   0        0        0     7603 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/benchmark.py
+-rw-rw-rw-   0        0        0    21787 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/build.py
+-rw-rw-rw-   0        0        0     7460 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/catalog.py
+-rw-rw-rw-   0        0        0     9406 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/common.py
+-rw-rw-rw-   0        0        0     8360 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/dataset_mapper.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.938718 onvif-gui-1.2.3/detectron2/data/datasets/
+-rw-rw-rw-   0        0        0      532 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    10433 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/builtin.py
+-rw-rw-rw-   0        0        0    22191 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/builtin_meta.py
+-rw-rw-rw-   0        0        0    13496 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/cityscapes.py
+-rw-rw-rw-   0        0        0     8008 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-rw-rw-   0        0        0    24004 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/coco.py
+-rw-rw-rw-   0        0        0     9205 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/coco_panoptic.py
+-rw-rw-rw-   0        0        0     9864 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/lvis.py
+-rw-rw-rw-   0        0        0   223770 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-rw-rw-   0        0        0   219193 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/lvis_v1_categories.py
+-rw-rw-rw-   0        0        0    39434 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-rw-rw-   0        0        0     3210 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/pascal_voc.py
+-rw-rw-rw-   0        0        0      172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/datasets/register_coco.py
+-rw-rw-rw-   0        0        0    23487 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/detection_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.947688 onvif-gui-1.2.3/detectron2/data/samplers/
+-rw-rw-rw-   0        0        0      429 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/samplers/__init__.py
+-rw-rw-rw-   0        0        0    12067 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/samplers/distributed_sampler.py
+-rw-rw-rw-   0        0        0     1991 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:03.960645 onvif-gui-1.2.3/detectron2/data/transforms/
+-rw-rw-rw-   0        0        0      480 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/transforms/__init__.py
+-rw-rw-rw-   0        0        0    14492 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/transforms/augmentation.py
+-rw-rw-rw-   0        0        0    23683 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/transforms/augmentation_impl.py
+-rw-rw-rw-   0        0        0    12980 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/data/transforms/transform.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.004168 onvif-gui-1.2.3/detectron2/layers/
+-rw-rw-rw-   0        0        0      900 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/__init__.py
+-rw-rw-rw-   0        0        0     5908 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/aspp.py
+-rw-rw-rw-   0        0        0    12431 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/batch_norm.py
+-rw-rw-rw-   0        0        0     3135 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/blocks.py
+-rw-rw-rw-   0        0        0    17492 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/deform_conv.py
+-rw-rw-rw-   0        0        0     4335 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/losses.py
+-rw-rw-rw-   0        0        0    11154 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/mask_ops.py
+-rw-rw-rw-   0        0        0     6629 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/nms.py
+-rw-rw-rw-   0        0        0     3172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/roi_align.py
+-rw-rw-rw-   0        0        0     3393 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/roi_align_rotated.py
+-rw-rw-rw-   0        0        0      673 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/rotated_boxes.py
+-rw-rw-rw-   0        0        0      555 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/shape_spec.py
+-rw-rw-rw-   0        0        0     5271 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/layers/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.033071 onvif-gui-1.2.3/detectron2/modeling/
+-rw-rw-rw-   0        0        0     1632 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/__init__.py
+-rw-rw-rw-   0        0        0    15825 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/anchor_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.068838 onvif-gui-1.2.3/detectron2/modeling/backbone/
+-rw-rw-rw-   0        0        0      618 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/backbone.py
+-rw-rw-rw-   0        0        0     1048 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/build.py
+-rw-rw-rw-   0        0        0    10628 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/fpn.py
+-rw-rw-rw-   0        0        0    16434 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/mvit.py
+-rw-rw-rw-   0        0        0    17108 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/regnet.py
+-rw-rw-rw-   0        0        0    24352 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/resnet.py
+-rw-rw-rw-   0        0        0    25785 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/swin.py
+-rw-rw-rw-   0        0        0     6546 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/utils.py
+-rw-rw-rw-   0        0        0    19860 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/backbone/vit.py
+-rw-rw-rw-   0        0        0    15492 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/box_regression.py
+-rw-rw-rw-   0        0        0     6391 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/matcher.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.100696 onvif-gui-1.2.3/detectron2/modeling/meta_arch/
+-rw-rw-rw-   0        0        0      524 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/__init__.py
+-rw-rw-rw-   0        0        0      839 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/build.py
+-rw-rw-rw-   0        0        0    11940 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/dense_detector.py
+-rw-rw-rw-   0        0        0    13541 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/fcos.py
+-rw-rw-rw-   0        0        0    10676 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-rw-rw-   0        0        0    14237 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/rcnn.py
+-rw-rw-rw-   0        0        0    18704 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/retinanet.py
+-rw-rw-rw-   0        0        0    10173 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-rw-rw-   0        0        0    11104 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/mmdet_wrapper.py
+-rw-rw-rw-   0        0        0    11575 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/poolers.py
+-rw-rw-rw-   0        0        0     4145 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/postprocessing.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.117131 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/
+-rw-rw-rw-   0        0        0      236 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/build.py
+-rw-rw-rw-   0        0        0     8333 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-rw-rw-   0        0        0    24347 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/rpn.py
+-rw-rw-rw-   0        0        0     9016 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.143585 onvif-gui-1.2.3/detectron2/modeling/roi_heads/
+-rw-rw-rw-   0        0        0      797 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/__init__.py
+-rw-rw-rw-   0        0        0     4195 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/box_head.py
+-rw-rw-rw-   0        0        0    13289 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-rw-rw-   0        0        0    25959 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-rw-rw-   0        0        0    11428 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-rw-rw-   0        0        0    12467 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/mask_head.py
+-rw-rw-rw-   0        0        0    38578 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/roi_heads.py
+-rw-rw-rw-   0        0        0    11446 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-rw-rw-   0        0        0     2388 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/sampling.py
+-rw-rw-rw-   0        0        0    12723 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/modeling/test_time_augmentation.py
+-rw-rw-rw-   0        0        0     1829 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/predictor.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.167351 onvif-gui-1.2.3/detectron2/structures/
+-rw-rw-rw-   0        0        0      662 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/__init__.py
+-rw-rw-rw-   0        0        0    14854 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/boxes.py
+-rw-rw-rw-   0        0        0     5649 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/image_list.py
+-rw-rw-rw-   0        0        0     6807 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/instances.py
+-rw-rw-rw-   0        0        0     9269 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/keypoints.py
+-rw-rw-rw-   0        0        0    20336 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/masks.py
+-rw-rw-rw-   0        0        0    19356 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/structures/rotated_boxes.py
+-rw-rw-rw-   0        0        0     2775 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/tracker.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.224177 onvif-gui-1.2.3/detectron2/utils/
+-rw-rw-rw-   0        0        0       52 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/__init__.py
+-rw-rw-rw-   0        0        0     6205 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/analysis.py
+-rw-rw-rw-   0        0        0     8633 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/collect_env.py
+-rw-rw-rw-   0        0        0     4254 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/colormap.py
+-rw-rw-rw-   0        0        0     5807 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/comm.py
+-rw-rw-rw-   0        0        0     1911 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/develop.py
+-rw-rw-rw-   0        0        0     5814 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/env.py
+-rw-rw-rw-   0        0        0    17508 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/events.py
+-rw-rw-rw-   0        0        0     1226 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/file_io.py
+-rw-rw-rw-   0        0        0     8044 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/logger.py
+-rw-rw-rw-   0        0        0     2667 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/memory.py
+-rw-rw-rw-   0        0        0     1934 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/registry.py
+-rw-rw-rw-   0        0        0     1096 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/serialize.py
+-rw-rw-rw-   0        0        0    18576 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/testing.py
+-rw-rw-rw-   0        0        0    11606 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/video_visualizer.py
+-rw-rw-rw-   0        0        0    52426 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/detectron2/utils/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.236097 onvif-gui-1.2.3/gui/
+-rw-rw-rw-   0        0        0       28 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.259860 onvif-gui-1.2.3/gui/components/
+-rw-rw-rw-   0        0        0      286 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/components/__init__.py
+-rw-rw-rw-   0        0        0     1824 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/comboselector.py
+-rw-rw-rw-   0        0        0     2459 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/directoryselector.py
+-rw-rw-rw-   0        0        0     2172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/fileselector.py
+-rw-rw-rw-   0        0        0     6416 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/components/labelselector.py
+-rw-rw-rw-   0        0        0     4194 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/progress.py
+-rw-rw-rw-   0        0        0     1962 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/components/thresholdslider.py
+-rw-rw-rw-   0        0        0      855 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/components/waitdialog.py
+-rw-rw-rw-   0        0        0     2054 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/glwidget.py
+-rw-rw-rw-   0        0        0    17483 2023-06-06 16:00:40.000000 onvif-gui-1.2.3/gui/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.282627 onvif-gui-1.2.3/gui/onvif/
+-rw-rw-rw-   0        0        0      196 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/__init__.py
+-rw-rw-rw-   0        0        0     5870 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/admintab.py
+-rw-rw-rw-   0        0        0     4051 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/imagetab.py
+-rw-rw-rw-   0        0        0     2484 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/logindialog.py
+-rw-rw-rw-   0        0        0     5364 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/networktab.py
+-rw-rw-rw-   0        0        0     5241 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/ptztab.py
+-rw-rw-rw-   0        0        0     4640 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/onvif/videotab.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.300061 onvif-gui-1.2.3/gui/panels/
+-rw-rw-rw-   0        0        0      184 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/panels/__init__.py
+-rw-rw-rw-   0        0        0     3802 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/panels/audiopanel.py
+-rw-rw-rw-   0        0        0    13667 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/panels/camerapanel.py
+-rw-rw-rw-   0        0        0    14756 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/panels/filepanel.py
+-rw-rw-rw-   0        0        0    14134 2023-06-06 15:29:24.000000 onvif-gui-1.2.3/gui/panels/settingspanel.py
+-rw-rw-rw-   0        0        0     3806 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/panels/videopanel.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.341396 onvif-gui-1.2.3/gui/resources/
+-rw-rw-rw-   0        0        0     2021 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/apply.png
+-rw-rw-rw-   0        0        0      245 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/apply_hi.png
+-rw-rw-rw-   0        0        0      244 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/apply_lo.png
+-rw-rw-rw-   0        0        0      911 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/audio.png
+-rw-rw-rw-   0        0        0      536 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/audio_hi.png
+-rw-rw-rw-   0        0        0      920 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/audio_lo.png
+-rw-rw-rw-   0        0        0      203 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_closed.png
+-rw-rw-rw-   0        0        0      219 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_closed_hi.png
+-rw-rw-rw-   0        0        0      211 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_closed_lo.png
+-rw-rw-rw-   0        0        0      199 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_open.png
+-rw-rw-rw-   0        0        0      168 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_open_hi.png
+-rw-rw-rw-   0        0        0      172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/branch_open_lo.png
+-rw-rw-rw-   0        0        0      267 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/checked.png
+-rw-rw-rw-   0        0        0      235 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/checked_hi.png
+-rw-rw-rw-   0        0        0      246 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/checked_lo.png
+-rw-rw-rw-   0        0        0    13358 2023-05-26 17:50:15.000000 onvif-gui-1.2.3/gui/resources/darkstyle.qss
+-rw-rw-rw-   0        0        0      910 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/discover.png
+-rw-rw-rw-   0        0        0      849 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/discover_hi.png
+-rw-rw-rw-   0        0        0      937 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/discover_lo.png
+-rw-rw-rw-   0        0        0      425 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/fast-forward.png
+-rw-rw-rw-   0        0        0      253 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/fast-forward_hi.png
+-rw-rw-rw-   0        0        0      433 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/fast-forward_lo.png
+-rw-rw-rw-   0        0        0      641 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/mute.png
+-rw-rw-rw-   0        0        0      346 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/mute_hi.png
+-rw-rw-rw-   0        0        0      618 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/mute_lo.png
+-rw-rw-rw-   0        0        0      347 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/next.png
+-rw-rw-rw-   0        0        0      225 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/next_hi.png
+-rw-rw-rw-   0        0        0      348 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/next_lo.png
+-rw-rw-rw-   0        0        0   207707 2023-06-04 21:18:37.000000 onvif-gui-1.2.3/gui/resources/onvif-gui.ico
+-rw-rw-rw-   0        0        0    46084 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/onvif-gui.png
+-rw-rw-rw-   0        0        0      172 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/pause.png
+-rw-rw-rw-   0        0        0      144 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/pause_hi.png
+-rw-rw-rw-   0        0        0      149 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/pause_lo.png
+-rw-rw-rw-   0        0        0      321 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/play.png
+-rw-rw-rw-   0        0        0      209 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/play_hi.png
+-rw-rw-rw-   0        0        0      316 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/play_lo.png
+-rw-rw-rw-   0        0        0      349 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/previous.png
+-rw-rw-rw-   0        0        0      232 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/previous_hi.png
+-rw-rw-rw-   0        0        0      348 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/previous_lo.png
+-rw-rw-rw-   0        0        0      324 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-off.png
+-rw-rw-rw-   0        0        0      250 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-off_hi.png
+-rw-rw-rw-   0        0        0      324 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-off_lo.png
+-rw-rw-rw-   0        0        0      350 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-on.png
+-rw-rw-rw-   0        0        0      263 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-on_hi.png
+-rw-rw-rw-   0        0        0      343 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/radio-on_lo.png
+-rw-rw-rw-   0        0        0      395 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/record.png
+-rw-rw-rw-   0        0        0      394 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/record_hi.png
+-rw-rw-rw-   0        0        0      425 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/record_lo.png
+-rw-rw-rw-   0        0        0      408 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/recording.png
+-rw-rw-rw-   0        0        0      435 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/recording_hi.png
+-rw-rw-rw-   0        0        0      532 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/recording_lo.png
+-rw-rw-rw-   0        0        0      454 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/rewind.png
+-rw-rw-rw-   0        0        0      250 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/rewind_hi.png
+-rw-rw-rw-   0        0        0      457 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/rewind_lo.png
+-rw-rw-rw-   0        0        0      187 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_left.png
+-rw-rw-rw-   0        0        0      183 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_left_hi.png
+-rw-rw-rw-   0        0        0      189 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_left_lo.png
+-rw-rw-rw-   0        0        0      162 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_up.png
+-rw-rw-rw-   0        0        0      160 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_up_hi.png
+-rw-rw-rw-   0        0        0      161 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/small_arrow_up_lo.png
+-rw-rw-rw-   0        0        0    19236 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/gui/resources/spinner.gif
+-rw-rw-rw-   0        0        0      158 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/stop.png
+-rw-rw-rw-   0        0        0      140 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/stop_hi.png
+-rw-rw-rw-   0        0        0      151 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/stop_lo.png
+-rw-rw-rw-   0        0        0      143 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/unchecked.png
+-rw-rw-rw-   0        0        0      142 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/unchecked_hi.png
+-rw-rw-rw-   0        0        0      143 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/gui/resources/unchecked_lo.png
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.341396 onvif-gui-1.2.3/modules/
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.345379 onvif-gui-1.2.3/modules/audio/
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/modules/audio/__init__.py
+-rw-rw-rw-   0        0        0     3492 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/modules/audio/sample.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.370296 onvif-gui-1.2.3/modules/video/
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/modules/video/__init__.py
+-rw-rw-rw-   0        0        0     8911 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/modules/video/keypoint.py
+-rw-rw-rw-   0        0        0     6297 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/modules/video/retinanet.py
+-rw-rw-rw-   0        0        0     3244 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/modules/video/sample.py
+-rw-rw-rw-   0        0        0     9442 2023-06-04 20:08:40.000000 onvif-gui-1.2.3/modules/video/segment.py
+-rw-rw-rw-   0        0        0    16288 2023-06-05 18:24:56.000000 onvif-gui-1.2.3/modules/video/yolov7.py
+-rw-rw-rw-   0        0        0    15675 2023-06-05 18:24:50.000000 onvif-gui-1.2.3/modules/video/yolov8.py
+-rw-rw-rw-   0        0        0    17631 2023-06-05 14:49:36.000000 onvif-gui-1.2.3/modules/video/yolox.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.387239 onvif-gui-1.2.3/onvif_gui.egg-info/
+-rw-rw-rw-   0        0        0     9056 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8475 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-06-06 16:18:03.000000 onvif-gui-1.2.3/onvif_gui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1688 2023-06-06 16:00:30.000000 onvif-gui-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:18:04.531755 onvif-gui-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2023-06-06 16:00:23.000000 onvif-gui-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.408169 onvif-gui-1.2.3/tracker/
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/basetrack.py
+-rw-rw-rw-   0        0        0    12632 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/byte_tracker.py
+-rw-rw-rw-   0        0        0     9816 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/kalman_filter.py
+-rw-rw-rw-   0        0        0     6304 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/tracker/matching.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.408169 onvif-gui-1.2.3/yolov7/
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.430096 onvif-gui-1.2.3/yolov7/models/
+-rw-rw-rw-   0        0        0        6 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/models/__init__.py
+-rw-rw-rw-   0        0        0    86435 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/models/common.py
+-rw-rw-rw-   0        0        0    11177 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/models/experimental.py
+-rw-rw-rw-   0        0        0    40895 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/models/yolo.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.484912 onvif-gui-1.2.3/yolov7/utils/
+-rw-rw-rw-   0        0        0        6 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/__init__.py
+-rw-rw-rw-   0        0        0     2320 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/activations.py
+-rw-rw-rw-   0        0        0     5771 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/add_nms.py
+-rw-rw-rw-   0        0        0     7321 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/autoanchor.py
+-rw-rw-rw-   0        0        0    57559 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/datasets.py
+-rw-rw-rw-   0        0        0    37789 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/general.py
+-rw-rw-rw-   0        0        0     4996 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/google_utils.py
+-rw-rw-rw-   0        0        0    76741 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/loss.py
+-rw-rw-rw-   0        0        0     9537 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/metrics.py
+-rw-rw-rw-   0        0        0    21424 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/plots.py
+-rw-rw-rw-   0        0        0    15840 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolov7/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.485909 onvif-gui-1.2.3/yolox/
+-rw-rw-rw-   0        0        0        0 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.523782 onvif-gui-1.2.3/yolox/models/
+-rw-rw-rw-   0        0        0      961 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/__init__.py
+-rw-rw-rw-   0        0        0     5019 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/build.py
+-rw-rw-rw-   0        0        0     6840 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/darknet.py
+-rw-rw-rw-   0        0        0     2372 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/losses.py
+-rw-rw-rw-   0        0        0     6944 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/network_blocks.py
+-rw-rw-rw-   0        0        0     3202 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/yolo_fpn.py
+-rw-rw-rw-   0        0        0    26204 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/yolo_head.py
+-rw-rw-rw-   0        0        0     4288 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/yolo_pafpn.py
+-rw-rw-rw-   0        0        0     2054 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/models/yolox.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:18:04.530759 onvif-gui-1.2.3/yolox/utils/
+-rw-rw-rw-   0        0        0      130 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/utils/__init__.py
+-rw-rw-rw-   0        0        0     1628 2023-05-25 20:20:34.000000 onvif-gui-1.2.3/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.2.2/LICENSE` & `onvif-gui-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/README.md` & `onvif-gui-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.2.3/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/checkpoint/catalog.py` & `onvif-gui-1.2.3/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.2.3/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/config/__init__.py` & `onvif-gui-1.2.3/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/config/compat.py` & `onvif-gui-1.2.3/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/config/config.py` & `onvif-gui-1.2.3/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/config/defaults.py` & `onvif-gui-1.2.3/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/config/instantiate.py` & `onvif-gui-1.2.3/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/config/lazy.py` & `onvif-gui-1.2.3/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/configs/Base-RCNN-FPN.yaml` & `onvif-gui-1.2.3/detectron2/configs/Base-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml` & `onvif-gui-1.2.3/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/__init__.py` & `onvif-gui-1.2.3/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/benchmark.py` & `onvif-gui-1.2.3/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/build.py` & `onvif-gui-1.2.3/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/catalog.py` & `onvif-gui-1.2.3/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/common.py` & `onvif-gui-1.2.3/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/dataset_mapper.py` & `onvif-gui-1.2.3/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/__init__.py` & `onvif-gui-1.2.3/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/builtin.py` & `onvif-gui-1.2.3/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.2.3/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.2.3/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.2.3/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/coco.py` & `onvif-gui-1.2.3/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.2.3/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/lvis.py` & `onvif-gui-1.2.3/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.2.3/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.2.3/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.2.3/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.2.3/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/detection_utils.py` & `onvif-gui-1.2.3/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.2.3/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.2.3/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.2.3/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.2.3/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/data/transforms/transform.py` & `onvif-gui-1.2.3/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/__init__.py` & `onvif-gui-1.2.3/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/aspp.py` & `onvif-gui-1.2.3/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/batch_norm.py` & `onvif-gui-1.2.3/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/blocks.py` & `onvif-gui-1.2.3/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/deform_conv.py` & `onvif-gui-1.2.3/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/losses.py` & `onvif-gui-1.2.3/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/mask_ops.py` & `onvif-gui-1.2.3/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/nms.py` & `onvif-gui-1.2.3/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/roi_align.py` & `onvif-gui-1.2.3/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.2.3/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.2.3/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/shape_spec.py` & `onvif-gui-1.2.3/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/layers/wrappers.py` & `onvif-gui-1.2.3/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/__init__.py` & `onvif-gui-1.2.3/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.2.3/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/build.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.2.3/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/box_regression.py` & `onvif-gui-1.2.3/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/matcher.py` & `onvif-gui-1.2.3/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/meta_arch/__init__.py` & `onvif-gui-1.2.3/detectron2/modeling/meta_arch/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.2.3/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.2.3/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.2.3/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.2.3/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.2.3/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.2.3/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.2.3/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.2.3/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/poolers.py` & `onvif-gui-1.2.3/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/postprocessing.py` & `onvif-gui-1.2.3/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.2.3/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.2.3/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.2.3/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.2.3/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.2.3/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.2.3/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.2.3/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.2.3/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.2.3/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.2.3/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.2.3/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.2.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/sampling.py` & `onvif-gui-1.2.3/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.2.3/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/predictor.py` & `onvif-gui-1.2.3/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/structures/__init__.py` & `onvif-gui-1.2.3/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/structures/boxes.py` & `onvif-gui-1.2.3/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/structures/image_list.py` & `onvif-gui-1.2.3/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/structures/instances.py` & `onvif-gui-1.2.3/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/structures/keypoints.py` & `onvif-gui-1.2.3/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/structures/masks.py` & `onvif-gui-1.2.3/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.2.3/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/tracker.py` & `onvif-gui-1.2.3/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/analysis.py` & `onvif-gui-1.2.3/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/collect_env.py` & `onvif-gui-1.2.3/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/colormap.py` & `onvif-gui-1.2.3/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/comm.py` & `onvif-gui-1.2.3/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/develop.py` & `onvif-gui-1.2.3/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/env.py` & `onvif-gui-1.2.3/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/events.py` & `onvif-gui-1.2.3/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/file_io.py` & `onvif-gui-1.2.3/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/logger.py` & `onvif-gui-1.2.3/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/memory.py` & `onvif-gui-1.2.3/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/registry.py` & `onvif-gui-1.2.3/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/serialize.py` & `onvif-gui-1.2.3/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/testing.py` & `onvif-gui-1.2.3/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/video_visualizer.py` & `onvif-gui-1.2.3/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/detectron2/utils/visualizer.py` & `onvif-gui-1.2.3/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/components/comboselector.py` & `onvif-gui-1.2.3/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/components/directoryselector.py` & `onvif-gui-1.2.3/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/components/fileselector.py` & `onvif-gui-1.2.3/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/components/labelselector.py` & `onvif-gui-1.2.3/gui/onvif/videotab.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,113 @@
-#*******************************************************************************
-# onvif-gui/gui/components/labelselector.py
+#/********************************************************************
+# onvif-gui/gui/onvif/videotab.py 
 #
-# Copyright (c) 2023 Stephen Rhodes 
+# Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-#******************************************************************************/
+#*********************************************************************/
 
-from PyQt6.QtWidgets import QPushButton, QColorDialog, \
-QGridLayout, QWidget, QCheckBox, QLabel, QComboBox
+from PyQt6.QtWidgets import QComboBox, QLineEdit, QSpinBox, \
+QGridLayout, QWidget, QLabel
 from PyQt6.QtCore import Qt
-from PyQt6.QtGui import QColor
 
-class LabelSelector(QWidget):
-    def __init__(self, mw, name, index, labels=None):
+class SpinBox(QSpinBox):
+    def __init__(self, qle):
         super().__init__()
+        self.setLineEdit(qle)
 
-        self.labels = [ "person", "bicycle", "car", "motorcycle", "airplane", "bus", "train", "truck", 
-                        "boat", "traffic light", "fire hydrant", "stop sign", "parking meter", "bench",
-                        "bird", "cat", "dog", "horse", "sheep", "cow", "elephant", "bear",  "zebra",
-                        "giraffe", "backpack", "umbrella", "handbag", "tie", "suitcase", "frisbee", "skis",
-                        "snowboard", "sports ball", "kite", "baseball bat", "baseball glove", "skateboard",
-                        "surfboard", "tennis racket", "bottle", "wine glass", "cup", "fork", "knife",
-                        "spoon", "bowl", "banana", "apple", "sandwich", "orange", "broccoli", "carrot",
-                        "hot dog", "pizza", "donut", "cake", "chair", "couch", "potted plant", "bed",
-                        "dining table", "toilet", "tv", "laptop", "mouse", "remote", "keyboard",
-                        "cell phone", "microwave", "oven", "toaster", "sink", "refrigerator", "book",
-                        "clock", "vase", "scissors", "teddy bear", "hair drier", "toothbrush" ]
-        if labels is not None:
-            self.labels = labels
-        
-        self.mw = mw
-        self.index = index
-        self.colorKey = "Module/" + name + "/color" + str(index)
-        self.enabledKey = "Module/" + name + "/enabled" + str(index)
-        self.labelKey = "Module/" + name + "/label" + str(index)
-        self.idleColor = QColor("#3B3B3B")
-        self.m_color = QColor(self.mw.settings.value(self.colorKey, self.idleColor.name()))
-        
-        self.cmbLabel = QComboBox()
-        self.cmbLabel.addItems(self.labels)
-        self.cmbLabel.setCurrentText(self.mw.settings.value(self.labelKey))
-        self.cmbLabel.currentTextChanged.connect(self.cmbLabelChanged)
-
-        self.chkBox = QCheckBox()
-        self.chkBox.setChecked(int(self.mw.settings.value(self.enabledKey, 0)))
-        self.chkBox.stateChanged.connect(self.chkBoxClicked)
-
-        self.btnColor = QPushButton("...")
-        self.btnColor.setToolTip("Set Box Color")
-        self.btnColor.setToolTipDuration(2000)
-        self.btnColor.setMaximumWidth(36)
-        self.btnColor.setStyleSheet("QPushButton {background-color: " + self.m_color.name() + "; color: white;}")
-        self.btnColor.clicked.connect(self.btnColorClicked)
-
-        self.lblCount = QLabel()
-        self.lblCount.setMinimumWidth(30)
-        self.lblCount.setAlignment(Qt.AlignmentFlag.AlignRight)
-
-        lytLabel = QGridLayout(self)
-        lytLabel.addWidget(self.chkBox,   0, 0, 1, 1)
-        lytLabel.addWidget(self.cmbLabel, 0, 1, 1, 1)
-        lytLabel.addWidget(self.btnColor, 0, 2, 1, 1)
-        lytLabel.addWidget(self.lblCount, 0, 3, 1, 1)
-        lytLabel.setColumnStretch(1, 10)
-        lytLabel.setContentsMargins(0, 0, 0, 0)
-
-        self.setEnabled(self.chkBox.isChecked())
-
-    def btnColorClicked(self):
-        color = QColorDialog.getColor(self.m_color)
-        if color.isValid():
-            self.m_color = color
-            self.btnColor.setStyleSheet("QPushButton {background-color: " + self.m_color.name() + "; color: white;}")
-            self.mw.settings.setValue(self.colorKey, self.m_color.name())
-            print("label selector color", color.red(), color.green(), color.blue(), color.name())
-
-    def chkBoxClicked(self, state):
-        self.setEnabled(state)
-        self.mw.settings.setValue(self.enabledKey, state)
-        self.lblCount.setText("")
-
-    def cmbLabelChanged(self, label):
-        self.mw.settings.setValue(self.labelKey, label)
-
-    def setEnabled(self, enabled):
-        self.chkBox.setChecked(enabled)
-        self.cmbLabel.setEnabled(enabled)
-        self.btnColor.setEnabled(enabled)
-        if enabled:
-            self.btnColor.setStyleSheet("QPushButton {background-color: " + self.m_color.name() + "; color: white;}")
-        else:
-            self.btnColor.setStyleSheet("QPushButton {background-color: " + self.idleColor.name() + "; color: white;}")
-
-    def setCount(self, count):
-        self.lblCount.setText(str(count))
-
-    def label(self):
-        return self.cmbLabel.currentIndex()
-    
-    def color(self):
-        return [self.m_color.red(), self.m_color.green(), self.m_color.blue()]
-    
-    def isChecked(self):
-        return self.chkBox.isChecked()
+class VideoTab(QWidget):
+    def __init__(self, cp):
+        super().__init__()
+        self.cp = cp
+
+        self.cmbResolutions = QComboBox()
+        self.cmbResolutions.currentTextChanged.connect(self.cp.onEdit)
+        self.lblResolutions = QLabel("Resolution")
+
+        txtFrameRate = QLineEdit()
+        self.spnFrameRate = SpinBox(txtFrameRate)
+        self.spnFrameRate.textChanged.connect(self.cp.onEdit)
+        self.lblFrameRate = QLabel("Frame Rate")
+
+        txtGovLength = QLineEdit()
+        self.spnGovLength = SpinBox(txtGovLength)
+        self.spnGovLength.textChanged.connect(self.cp.onEdit)
+        self.lblGovLength = QLabel("GOP Length")
+
+        txtBitrate = QLineEdit()
+        self.spnBitrate = SpinBox(txtBitrate)
+        self.spnBitrate.textChanged.connect(self.cp.onEdit)
+        self.lblBitrate = QLabel("Bitrate")
+
+        lytMain = QGridLayout(self)
+        lytMain.addWidget(self.lblResolutions, 1, 0, 1, 1)
+        lytMain.addWidget(self.cmbResolutions, 1, 1, 1, 1)
+        lytMain.addWidget(self.lblFrameRate,   2, 0, 1, 1)
+        lytMain.addWidget(self.spnFrameRate,   2, 1, 1, 1)
+        lytMain.addWidget(self.lblGovLength,   3, 0, 1, 1)
+        lytMain.addWidget(self.spnGovLength,   3, 1, 1, 1)
+        lytMain.addWidget(self.lblBitrate,     4, 0, 1, 1)
+        lytMain.addWidget(self.spnBitrate,     4, 1, 1, 1)
+
+    def fill(self, onvif_data):
+        self.cmbResolutions.clear()
+        i = 0
+        while len(onvif_data.resolutions_buf(i)) > 0 and i < 16:
+            self.cmbResolutions.addItem(onvif_data.resolutions_buf(i))
+            i += 1
+
+        current_resolution = str(onvif_data.width()) + " x " + str(onvif_data.height())
+        self.cmbResolutions.setCurrentText(current_resolution)
+
+        self.spnFrameRate.setMaximum(onvif_data.frame_rate_max())
+        self.spnFrameRate.setMinimum(onvif_data.frame_rate_min())
+        self.spnFrameRate.setValue(onvif_data.frame_rate())
+
+        self.spnGovLength.setMaximum(onvif_data.gov_length_max())
+        self.spnGovLength.setMinimum(onvif_data.gov_length_min())
+        self.spnGovLength.setValue(onvif_data.gov_length())
+
+        self.spnBitrate.setMaximum(onvif_data.bitrate_max())
+        self.spnBitrate.setMinimum(onvif_data.bitrate_min())
+        self.spnBitrate.setValue(onvif_data.bitrate())
+
+        self.setEnabled(onvif_data.width())
+        self.cp.onEdit()
+
+    def edited(self, onvif_data):
+        result = False
+        if self.isEnabled():
+            current_resolution = str(onvif_data.width()) + " x " + str(onvif_data.height())
+            if not current_resolution == self.cmbResolutions.currentText():
+                result = True
+            if not onvif_data.frame_rate() == self.spnFrameRate.value():
+                result = True
+            if not onvif_data.gov_length() == self.spnGovLength.value():
+                result = True
+            if not onvif_data.bitrate() == self.spnBitrate.value():
+                result = True
+
+        return result
+
+    def update(self, onvif_data):
+        if self.edited(onvif_data):
+            self.setEnabled(False)
+            onvif_data.setFrameRate(self.spnFrameRate.value())
+            onvif_data.setGovLength(self.spnGovLength.value())
+            onvif_data.setBitrate(self.spnBitrate.value())
+            dims = self.cmbResolutions.currentText().split('x')
+            onvif_data.setWidth(int(dims[0]))
+            onvif_data.setHeight(int(dims[1]))
+            self.cp.boss.onvif_data = onvif_data
+            self.cp.boss.startUpdateVideo()
```

### Comparing `onvif-gui-1.2.2/gui/components/progress.py` & `onvif-gui-1.2.3/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/components/thresholdslider.py` & `onvif-gui-1.2.3/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/components/waitdialog.py` & `onvif-gui-1.2.3/gui/components/waitdialog.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from PyQt6.QtWidgets import QDialog, QLabel, QGridLayout
-from PyQt6.QtGui import QMovie
-from PyQt6.QtCore import Qt, QSize
-
-class WaitDialog(QDialog):
-    def __init__(self, p):
-        super().__init__(p)
-        self.lblMessage = QLabel("Please wait for operations to be completed")
-        self.lblProgress = QLabel()
-        self.movie = QMovie("image:spinner.gif")
-        self.movie.setScaledSize(QSize(50, 50))
-        self.lblProgress.setMovie(self.movie)
-        self.setWindowTitle("onvif-gui")
-
-        lytMain = QGridLayout(self)
-        lytMain.addWidget(self.lblMessage,  0, 1, 1, 1, Qt.AlignmentFlag.AlignCenter)
-        lytMain.addWidget(self.lblProgress, 1, 1, 1, 1, Qt.AlignmentFlag.AlignCenter)
-
-        self.movie.start()
-        self.setModal(True)
-
-    def sizeHint(self):
-        return QSize(300, 100)
-    
+from PyQt6.QtWidgets import QDialog, QLabel, QGridLayout
+from PyQt6.QtGui import QMovie
+from PyQt6.QtCore import Qt, QSize
+
+class WaitDialog(QDialog):
+    def __init__(self, p):
+        super().__init__(p)
+        self.lblMessage = QLabel("Please wait for operations to be completed")
+        self.lblProgress = QLabel()
+        self.movie = QMovie("image:spinner.gif")
+        self.movie.setScaledSize(QSize(50, 50))
+        self.lblProgress.setMovie(self.movie)
+        self.setWindowTitle("onvif-gui")
+
+        lytMain = QGridLayout(self)
+        lytMain.addWidget(self.lblMessage,  0, 1, 1, 1, Qt.AlignmentFlag.AlignCenter)
+        lytMain.addWidget(self.lblProgress, 1, 1, 1, 1, Qt.AlignmentFlag.AlignCenter)
+
+        self.movie.start()
+        self.setModal(True)
+
+    def sizeHint(self):
+        return QSize(300, 100)
+
```

### Comparing `onvif-gui-1.2.2/gui/glwidget.py` & `onvif-gui-1.2.3/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/main.py` & `onvif-gui-1.2.3/gui/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 import os
 import sys
+from loguru import logger
+if sys.platform == "win32":
+    filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
+else:
+    filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
+logger.add(filename, retention="1 days")
+
 import time
+from datetime import datetime
 import importlib.util
 from pathlib import Path
 from PyQt6.QtWidgets import QApplication, QMainWindow, QLabel, QSplitter, \
     QTabWidget, QMessageBox
-from PyQt6.QtCore import pyqtSignal, QObject, QSettings, QDir, QSize
+from PyQt6.QtCore import pyqtSignal, QObject, QSettings, QDir, QSize, QTimer
 from PyQt6.QtGui import QIcon
 from gui.panels import CameraPanel, FilePanel, SettingsPanel, VideoPanel, AudioPanel
 from gui.glwidget import GLWidget
 from gui.components import WaitDialog
 from collections import deque
 
 import avio
@@ -51,26 +59,30 @@
 class MainWindow(QMainWindow):
     def __init__(self, clear_settings=False):
         super().__init__()
         os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = "ON"
         QDir.addSearchPath("image", self.getLocation() + "/gui/resources/")
         self.style()
 
-        self.program_name = "onvif gui version 1.2.2"
+        self.program_name = "onvif gui version 1.2.3"
         self.setWindowTitle(self.program_name)
         self.setWindowIcon(QIcon('image:onvif-gui.png'))
         self.settings = QSettings("onvif", "gui")
         if clear_settings:
             self.settings.clear()
         self.volumeKey = "MainWindow/volume"
         self.muteKey = "MainWindow/mute"
         self.geometryKey = "MainWindow/geometry"
         self.tabIndexKey = "MainWindow/tabIndex"
         self.splitKey = "MainWindow/split"
 
+        self.uri = ""
+        self.reconnectTimer = QTimer()
+        self.reconnectTimer.setSingleShot(True)
+        self.reconnectTimer.timeout.connect(self.reconnect)
         self.player = None
         self.playing = False
         self.connecting = False
         self.volume = self.settings.value(self.volumeKey, 80)
 
         if self.settings.value(self.muteKey, 0) == 0:
             self.mute = False
@@ -235,14 +247,15 @@
         else:
             self.audioPanel.lblElapsed.setText("")
         return F
 
     def playMedia(self, uri):
         self.stopMedia()
         self.player = avio.Player()
+        self.uri = uri
         self.player.uri = uri
         self.player.width = lambda : self.glWidget.width()
         self.player.height = lambda : self.glWidget.height()
         if not self.settingsPanel.chkLowLatency.isChecked():
             self.player.vpq_size = 100
             self.player.apq_size = 100
         self.player.progressCallback = lambda f : self.mediaProgress(f)
@@ -334,30 +347,60 @@
     def infoCallback(self, msg):
         print(msg)
 
     def errorCallback(self, msg):
         self.signals.error.emit(msg)
 
     def onError(self, msg):
-        msgBox = QMessageBox(self)
-        msgBox.setText(msg)
-        msgBox.setWindowTitle(self.program_name)
-        msgBox.setIcon(QMessageBox.Icon.Warning)
-        msgBox.exec()
-        self.cameraPanel.setBtnRecord()
-        self.filePanel.control.setBtnRecord()
-        self.cameraPanel.setEnabled(True)
+        logger.debug("Error processing stream: " + self.uri + " - " + msg)
+        if self.settingsPanel.chkAutoReconnect.isChecked():
+            self.reconnectTimer.start(10000)
+            self.signals.showWait.emit()
+        else:
+            msgBox = QMessageBox(self)
+            msgBox.setText(msg)
+            msgBox.setWindowTitle(self.program_name)
+            msgBox.setIcon(QMessageBox.Icon.Warning)
+            msgBox.exec()
+            self.cameraPanel.setBtnRecord()
+            self.filePanel.control.setBtnRecord()
+            self.cameraPanel.setEnabled(True)
+
+    def reconnect(self):
+        self.signals.hideWait.emit()
+        logger.debug("Attempting to re-connnect")
+        self.playMedia(self.uri)
 
     def splitterMoved(self, pos, index):
         self.settings.setValue(self.splitKey, self.split.saveState())
 
     def getLocation(self):
         path = Path(os.path.dirname(__file__))
         return str(path.parent.absolute())
     
+    def getVideoFrameRate(self):
+        result = 0
+        if self.player is not None:
+            result = self.player.getVideoFrameRate()
+        return result
+    
+    def get_log_filename(self):
+        source = self.windowTitle()
+        source = source.replace(".", "_")
+        source = source.replace(" ", "_")
+        datestamp = datetime.now().strftime("%Y%m%d")
+        timestamp = datetime.now().strftime("%H%M%S")
+        log_dir = ""
+        if sys.platform == "win32":
+            log_dir = os.environ["HOMEPATH"]
+        else:
+            log_dir = os.environ["HOME"]
+        log_dir += os.path.sep + "logs" + os.path.sep + "onvif-gui" + os.path.sep + datestamp
+        return log_dir + os.path.sep + source + "_" + timestamp + ".csv"
+    
     def style(self):
         blDefault = "#5B5B5B"
         bmDefault = "#4B4B4B"
         bdDefault = "#3B3B3B"
         flDefault = "#C6D9F2"
         fmDefault = "#9DADC2"
         fdDefault = "#808D9E"
```

### Comparing `onvif-gui-1.2.2/gui/onvif/admintab.py` & `onvif-gui-1.2.3/gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/onvif/imagetab.py` & `onvif-gui-1.2.3/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/onvif/logindialog.py` & `onvif-gui-1.2.3/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/onvif/networktab.py` & `onvif-gui-1.2.3/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/onvif/ptztab.py` & `onvif-gui-1.2.3/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/panels/audiopanel.py` & `onvif-gui-1.2.3/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/panels/camerapanel.py` & `onvif-gui-1.2.3/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/panels/filepanel.py` & `onvif-gui-1.2.3/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/panels/settingspanel.py` & `onvif-gui-1.2.3/gui/panels/settingspanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self.hardwareEncodeKey = "settings/hardwareEncode"
         self.processPauseKey = "settings/processPause"
         self.processFrameKey = "settings/processFrame"
         self.cacheSizeKey = "settings/cacheSize"
         self.interfaceKey = "settings/interface"
         self.videoFilterKey = "settings/videoFilter"
         self.audioFilterKey = "settings/audioFilter"
+        self.autoReconnectKey = "settings/autoReconnect"
 
         decoders = ["NONE", "CUDA", "VAAPI", "VDPAU", "DXVA2", "D3D11VA"]
 
         self.chkAutoDiscover = QCheckBox("Enable Auto Discovery")
         self.chkAutoDiscover.setChecked(int(mw.settings.value(self.autoDiscoverKey, 0)))
         self.chkAutoDiscover.stateChanged.connect(self.autoDiscoverChecked)
         
@@ -116,24 +117,29 @@
         self.chkProcessPause.setChecked(int(mw.settings.value(self.processPauseKey, 0)))
         self.chkProcessPause.stateChanged.connect(self.processPauseChecked)
 
         self.chkLowLatency = QCheckBox("Low Latency")
         self.chkLowLatency.setChecked(int(mw.settings.value(self.latencyKey, 0)))
         self.chkLowLatency.stateChanged.connect(self.lowLatencyChecked)
 
+        self.chkAutoReconnect = QCheckBox("Auto Reconnect")
+        self.chkAutoReconnect.setChecked(int(mw.settings.value(self.autoReconnectKey, 0)))
+        self.chkAutoReconnect.stateChanged.connect(self.autoReconnectChecked)
+
         pnlChecks = QWidget()
         lytChecks = QGridLayout(pnlChecks)
         lytChecks.addWidget(self.chkDirectRender,   0, 0, 1, 1)
         lytChecks.addWidget(self.chkConvert2RGB,    0, 1, 1, 1)
         lytChecks.addWidget(self.chkDisableAudio,   1, 0, 1, 1)
         lytChecks.addWidget(self.chkDisableVideo,   1, 1, 1, 1)
         lytChecks.addWidget(self.chkPostEncode,     2, 0, 1, 1)
         lytChecks.addWidget(self.chkHardwareEncode, 2, 1, 1, 1)
         lytChecks.addWidget(self.chkProcessPause,   3, 0, 1, 1)
         lytChecks.addWidget(self.chkLowLatency,     3, 1, 1, 1)
+        lytChecks.addWidget(self.chkAutoReconnect,  4, 0, 1, 1)
 
         self.spnCacheSize = QSpinBox()
         self.spnCacheSize.setMinimum(1)
         self.spnCacheSize.setMaximum(10)
         self.spnCacheSize.setMaximumWidth(80)
         self.spnCacheSize.setValue(int(self.mw.settings.value(self.cacheSizeKey, 1)))
         self.spnCacheSize.valueChanged.connect(self.spnCacheSizeChanged)
@@ -258,14 +264,17 @@
 
     def processPauseChecked(self, state):
         self.mw.settings.setValue(self.processPauseKey, state)
 
     def lowLatencyChecked(self, state):
         self.mw.settings.setValue(self.latencyKey, state)
 
+    def autoReconnectChecked(self, state):
+        self.mw.settings.setValue(self.autoReconnectKey, state)
+
     def radioFilenameChecked(self):
         if self.radGenerateFilename.isChecked():
             self.mw.settings.setValue(self.generateKey, 1)
         else:
             self.mw.settings.setValue(self.generateKey, 0)
 
     def spnCacheSizeChanged(self, i):
```

### Comparing `onvif-gui-1.2.2/gui/panels/videopanel.py` & `onvif-gui-1.2.3/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/LICENSE` & `onvif-gui-1.2.3/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/audio.png` & `onvif-gui-1.2.3/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/audio_hi.png` & `onvif-gui-1.2.3/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/audio_lo.png` & `onvif-gui-1.2.3/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/darkstyle.qss` & `onvif-gui-1.2.3/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/discover.png` & `onvif-gui-1.2.3/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/discover_hi.png` & `onvif-gui-1.2.3/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/discover_lo.png` & `onvif-gui-1.2.3/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/mute.png` & `onvif-gui-1.2.3/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/mute_lo.png` & `onvif-gui-1.2.3/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/onvif-gui.png` & `onvif-gui-1.2.3/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/recording_lo.png` & `onvif-gui-1.2.3/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/gui/resources/spinner.gif` & `onvif-gui-1.2.3/gui/resources/spinner.gif`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/modules/audio/sample.py` & `onvif-gui-1.2.3/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/modules/video/keypoint.py` & `onvif-gui-1.2.3/modules/video/keypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 IMPORT_ERROR = ""
 try:
-    import numpy as np
-    import cv2
-    import math
     import os
     import sys
     from loguru import logger
-    logger.add("onvif-gui-errors.txt", retention="1 days")
+    if sys.platform == "win32":
+        filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
+    else:
+        filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
+    logger.add(filename, retention="1 days")
+
+    import numpy as np
+    import cv2
+    import math
     from pathlib import Path
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
     from gui.components import ThresholdSlider
 
     import torch
     from detectron2.config import get_cfg
     from detectron2.predictor import Predictor
```

### Comparing `onvif-gui-1.2.2/modules/video/retinanet.py` & `onvif-gui-1.2.3/modules/video/retinanet.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,23 @@
 #
 #*********************************************************************/
 
 IMPORT_ERROR = ""
 try:
     import os
     import sys
+    from loguru import logger
+    if sys.platform == "win32":
+        filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
+    else:
+        filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
+    logger.add(filename, retention="1 days")
+
     import cv2
     import numpy as np
-    from loguru import logger
-    logger.add("onvif-gui-errors.txt", retention="1 days")
     from contextlib import redirect_stderr
     from PyQt6.QtWidgets import QGridLayout, QWidget, QLabel, QMessageBox
     from PyQt6.QtCore import Qt
     from gui.components.thresholdslider import ThresholdSlider
     from gui.components.labelselector import LabelSelector
 
     import torch
```

### Comparing `onvif-gui-1.2.2/modules/video/sample.py` & `onvif-gui-1.2.3/modules/video/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/modules/video/segment.py` & `onvif-gui-1.2.3/modules/video/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 IMPORT_ERROR = ""
 try:
-    import numpy as np
     import os
-    import cv2
     import sys
     from loguru import logger
-    logger.add("onvif-gui-errors.txt", retention="1 days")
+    if sys.platform == "win32":
+        filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
+    else:
+        filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
+    logger.add(filename, retention="1 days")
+
+    import cv2
+    import numpy as np
     from pathlib import Path
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
     from PyQt6.QtCore import Qt
     from gui.components import ThresholdSlider, LabelSelector
 
     import torch
     from detectron2.config import get_cfg
```

### Comparing `onvif-gui-1.2.2/modules/video/yolov7.py` & `onvif-gui-1.2.3/modules/video/yolov8.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# onvif-gui/modules/video/yolov7.py 
+# onvif-gui/modules/video/yolov8.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -15,270 +15,336 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 IMPORT_ERROR = ""
 try:
-    import cv2
     import os
     import sys
-    import gc
-    import numpy as np
-    from pathlib import Path
     from loguru import logger
-    logger.add("onvif-gui-errors.txt", retention="1 days")
+    if sys.platform == "win32":
+        filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
+    else:
+        filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
+    logger.add(filename, retention="1 days")
 
+    import cv2
+    import numpy as np
+    from datetime import datetime
+    from pathlib import Path
     from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
-    from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox
-    from PyQt6.QtCore import Qt
+    from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox, QLineEdit
+    from PyQt6.QtCore import Qt, QRegularExpression
+    from PyQt6.QtGui import QRegularExpressionValidator
 
-    import cv2
     import torch
+    from ultralytics import YOLO
     from tracker.byte_tracker import BYTETracker
 
-    sys.path.append("yolov7")
-    for path in sys.path:
-        tmp = os.path.join(path, "yolov7")
-        if os.path.isdir(tmp):
-            sys.path.append(tmp)
-
-    from models.experimental import attempt_load
-    from utils.datasets import letterbox
-    from utils.general import non_max_suppression, scale_coords
-    from utils.torch_utils import select_device
-
 except ModuleNotFoundError as ex:
     IMPORT_ERROR = str(ex)
     logger.debug("Import Error has occurred, missing modules need to be installed, please consult documentation: " + IMPORT_ERROR)
 
 os.environ['KMP_DUPLICATE_LIB_OK']='True'
-MODULE_NAME = "yolov7"
+MODULE_NAME = "yolov8"
 
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
             self.name = MODULE_NAME
+            self.last_ex = ""
             self.autoKey = "Module/" + MODULE_NAME + "/autoDownload"
             self.trackKey = "Module/" + MODULE_NAME + "/track"
             self.showIDKey = "Module/" + MODULE_NAME + "/showID"
+            self.logCountKey = "Module/" + MODULE_NAME + "/logCount"
+            self.countIntervalKey = "Module/" + MODULE_NAME + "/countInterval"
+
+            self.mw.signals.started.connect(self.onMediaStarted)
+            
+            self.model_names = {"nano" : "yolov8n.pt", "small" : "yolov8s.pt", "medium" : "yolov8m.pt", "large" : "yolov8l.pt", "XL" : "yolov8x.pt"}
 
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
 
-            self.txtFilename = FileSelector(mw, MODULE_NAME)
-            self.txtFilename.setEnabled(not self.chkAuto.isChecked())
+            self.cmbModel = ComboSelector(mw, "Model Name", self.model_names.keys(), "nano", MODULE_NAME)
+            self.cmbModel.setEnabled(self.chkAuto.isChecked())
+
+            self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280", "1440"), "320", MODULE_NAME)
 
-            self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280"), "640", MODULE_NAME)
-            self.cmbType = ComboSelector(mw, "Model Name", ("yolov7", "yolov7x"), "yolov7", MODULE_NAME)
+            self.txtModelFile = FileSelector(mw, MODULE_NAME)
+            self.txtModelFile.setEnabled(not self.chkAuto.isChecked())
+
+            self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
 
             self.chkTrack = QCheckBox("Track Objects")
             self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
             self.chkTrack.stateChanged.connect(self.chkTrackClicked)
 
             self.chkShowID = QCheckBox("Show Object ID")
             self.chkShowID.setChecked(int(self.mw.settings.value(self.showIDKey, 1)))
             self.chkShowID.stateChanged.connect(self.chkShowIDClicked)
 
             if not self.chkTrack.isChecked():
                 self.chkShowID.setVisible(False)
 
-            self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
+            pnlCount = QWidget()
+            lblCount = QLabel("Count Interval (seconds)")
+            self.txtCountInterval = QLineEdit()
+            self.txtCountInterval.setText(self.mw.settings.value(self.countIntervalKey, ""))
+            self.txtCountInterval.textChanged.connect(self.countIntervalChanged)
+            numRegex = QRegularExpression("[0-9]*")
+            numValidator = QRegularExpressionValidator(numRegex, self)
+            self.txtCountInterval.setValidator(numValidator)        
+            self.chkLogCount = QCheckBox("Log Counts")
+            self.chkLogCount.setChecked(int(self.mw.settings.value(self.logCountKey, 0)))
+            self.chkLogCount.stateChanged.connect(self.chkLogCountClicked)
+            lytCount = QGridLayout(pnlCount)
+            lytCount.addWidget(lblCount,              0, 0, 1, 1)
+            lytCount.addWidget(self.txtCountInterval, 0, 1, 1, 1)
+            lytCount.addWidget(self.chkLogCount,      0, 2, 1, 1)
+            lytCount.setContentsMargins(0, 0, 0, 0)
 
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
                 self.labels.append(LabelSelector(mw, MODULE_NAME, i+1))
             pnlLabels = QWidget()
             lytLabels = QGridLayout(pnlLabels)
-            lblPanel = QLabel("Select classes to be identified")
+            lblPanel = QLabel("Select classes to be identified and counted")
             lblPanel.setAlignment(Qt.AlignmentFlag.AlignCenter)
             lytLabels.addWidget(lblPanel,        0, 0, 1, 1)
             for i in range(number_of_labels):
                 lytLabels.addWidget(self.labels[i], i+1, 0, 1, 1)
             lytLabels.setContentsMargins(0, 0, 0, 0)
 
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.chkAuto,      0, 0, 1, 2)
-            lytMain.addWidget(self.cmbType,      1, 0, 1, 2)
-            lytMain.addWidget(self.txtFilename,  2, 0, 1, 2)
+            lytMain.addWidget(self.cmbModel,     1, 0, 1, 2)
+            lytMain.addWidget(self.txtModelFile, 2, 0, 1, 2)
             lytMain.addWidget(self.cmbRes,       3, 0, 1, 2)
             lytMain.addWidget(self.sldConfThre,  4, 0, 1, 2)
-            lytMain.addWidget(self.chkTrack,     6, 0, 1, 1)
-            lytMain.addWidget(self.chkShowID,    6, 1, 1, 1)
+            lytMain.addWidget(self.chkTrack,     5, 0, 1, 1)
+            lytMain.addWidget(self.chkShowID,    5, 1, 1, 1)
+            lytMain.addWidget(pnlCount,          6, 0, 1, 2)
             lytMain.addWidget(pnlLabels,         7, 0, 1, 2)
             lytMain.addWidget(QLabel(),          8, 0, 1, 2)
             lytMain.setRowStretch(8, 10)
 
+            self.first_pass = True
+
             if len(IMPORT_ERROR) > 0:
                 QMessageBox.critical(None, MODULE_NAME + " Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
 
         except:
             logger.exception(MODULE_NAME + " configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
-        self.txtFilename.setEnabled(not self.chkAuto.isChecked())
+        self.cmbModel.setEnabled(self.chkAuto.isChecked())
+        self.txtModelFile.setEnabled(not self.chkAuto.isChecked())
 
     def chkTrackClicked(self, state):
         self.mw.settings.setValue(self.trackKey, state)
         self.chkShowID.setVisible(state)
 
     def chkShowIDClicked(self, state):
         self.mw.settings.setValue(self.showIDKey, state)
 
-    def getLabel(self, cls):
+    def chkLogCountClicked(self, state):
+        self.mw.settings.setValue(self.logCountKey, state)
+
+    def countIntervalChanged(self, txt):
+        self.mw.settings.setValue(self.countIntervalKey, txt)
+
+    def getCountInterval(self):
+        result = 0
+        if len(self.txtCountInterval.text()) > 0:
+            result = int(self.txtCountInterval.text())
+        return result
+
+    def onMediaStarted(self, n):
+        self.first_pass = True
+
+    def getModelName(self):
+        if self.chkAuto.isChecked():
+            return self.model_names[self.cmbModel.currentText()]
+        else:
+            return self.txtModelFile.text()
+        
+    def getLabel(self, class_id):
         for lbl in self.labels:
-            if lbl.label() == cls:
+            if lbl.label() == class_id:
                 return lbl
-
+            
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
             if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
                 return
             
             self.mw.signals.showWait.emit()
 
             self.ckpt_file = None
             if self.mw.configure.chkAuto.isChecked():
                 self.ckpt_file = self.get_auto_ckpt_filename()
-                print("cpkt_file:", self.ckpt_file)
                 cache = Path(self.ckpt_file)
 
                 if not cache.is_file():
                     cache.parent.mkdir(parents=True, exist_ok=True)
-                    model_name = self.mw.configure.cmbType.currentText()
-                    link = "https://github.com/WongKinYiu/yolov7/releases/download/v0.1/" + model_name + ".pt"
+                    model_name = self.mw.configure.getModelName()
+                    link = "https://github.com/ultralytics/assets/releases/download/v0.0.0/" + model_name
                     if os.path.split(sys.executable)[1] == "pythonw.exe":
                         torch.hub.download_url_to_file(link, self.ckpt_file, progress=False)
                     else:
                         torch.hub.download_url_to_file(link, self.ckpt_file)
             else:
-                self.ckpt_file = self.mw.configure.txtFilename.text()
-
-            weights = self.ckpt_file
-            res = int(self.mw.configure.cmbRes.currentText())
-            self.iou_thres = 0.45
-
-            self.device = select_device('')
-            self.half = self.device.type != 'cpu'
+                self.ckpt_file = self.configure.txtFilename.text()
 
-            self.model = None
-            gc.collect()
-            with torch.no_grad():
-                torch.cuda.empty_cache()
-
-            self.model = attempt_load(weights, map_location=self.device)
-            self.stride = int(self.model.stride.max())
-            if self.half:
-                self.model.half()
-            self.names = self.model.module.names if hasattr(self.model, 'module') else self.model.names
-
-            with torch.no_grad():
-                self.model(torch.zeros(1, 3, res, res).to(self.device).type_as(next(self.model.parameters())))
+            self.model_name = self.mw.configure.getModelName()
+            self.model = YOLO(Path(self.ckpt_file))
+            self.model.predict(np.zeros([1280, 720, 3], dtype=np.uint8), stream=True, verbose=False)
 
             self.track_thresh = self.mw.configure.sldConfThre.value()
             self.track_buffer = 30
             self.match_thresh = 0.8
-
-            self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
+            framerate = self.mw.getVideoFrameRate()
+            if framerate == 0: framerate = 30
+            self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh, frame_rate=framerate)
+
+            self.count_interval_start = 0
+            self.rts = 0
+            self.log_filename = ""
 
             self.mw.signals.hideWait.emit()
 
         except:
             logger.exception(MODULE_NAME + " initialization failure")
             self.mw.signals.hideWait.emit()
             self.mw.signals.error.emit(MODULE_NAME + " initialization failure, please check logs for details")
 
     def __call__(self, F):
         try:
-            original_img = np.array(F, copy=False)
+            img = np.array(F, copy=False)
+            self.rts = F.m_rts
 
             if self.mw.configure.name != MODULE_NAME:
                 return
             
-            res = int(self.mw.configure.cmbRes.currentText())
-            img = letterbox(original_img, res, stride=self.stride)[0]
-            img = img[:, :, ::-1].transpose(2, 0, 1)
-            img = np.ascontiguousarray(img)
-            img = torch.from_numpy(img).to(self.device)
-            img = img.half() if self.half else img.float()
-            img /= 255.0
-            if img.ndimension() == 3:
-                img = img.unsqueeze(0)
-
-            with torch.no_grad():
-                pred = self.model(img, augment=False)[0]
-
-            conf_thres = self.mw.configure.sldConfThre.value()
-            if self.mw.configure.chkTrack.isChecked():
-                conf_thres = 0.001
+            if self.mw.configure.first_pass:
+                self.count_interval_start = self.rts
+                self.mw.configure.first_pass = False
+                self.log_filename = ""
 
             label_counts = {}
             label_filter = []
             for lbl in self.mw.configure.labels:
                 if lbl.chkBox.isChecked():
                     label_filter.append(lbl.label())
                     label_counts[lbl.label()] = 0
 
-            pred = non_max_suppression(pred, conf_thres, self.iou_thres, classes=label_filter, agnostic=False)
+            confthre = self.mw.configure.sldConfThre.value()
+            if self.mw.configure.chkTrack.isChecked():
+                confthre = 0.001
+
+            if self.model_name != self.mw.configure.getModelName():
+                self.model_name = self.mw.configure.getModelName()
+                with torch.no_grad():
+                    torch.cuda.empty_cache()
+                self.__init__(self.mw)
 
-            boxes = pred[0]
-            if len(boxes):
-                boxes[:, :4] = scale_coords(img.shape[2:], boxes[:, :4], original_img.shape).round()
-                boxes = boxes.cpu().numpy()
+            res = int(self.mw.configure.cmbRes.currentText())
+                
+            results = self.model.predict(img, stream=True, verbose=False, 
+                                         classes=label_filter,
+                                         conf=confthre, 
+                                         imgsz=res)
+
+            interval = self.mw.configure.getCountInterval()
+            q_size = self.mw.getVideoFrameRate() * interval
 
+            for result in results:
                 if self.mw.configure.chkTrack.isChecked():
-                    w = original_img.shape[0]
-                    h = original_img.shape[1]
+
+                    output = result.boxes.xyxy
+                    scores = result.boxes.conf.reshape(-1, 1)
+                    labels = result.boxes.cls.reshape(-1, 1)
+                    output = torch.hstack((output, scores))
+                    output = torch.hstack((output, labels))
+                    output = output.cpu().numpy()
+
                     if self.track_thresh != self.mw.configure.sldConfThre.value():
                         self.track_thresh = self.mw.configure.sldConfThre.value()
-                        self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
+                        framerate = self.mw.getVideoFrameRate()
+                        if framerate == 0: framerate = 30
+                        self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh, frame_rate=framerate)
+
+                    online_targets = self.tracker.update(output, [img.shape[0] * res / img.shape[1], res], (res, res))
 
-                    online_targets = self.tracker.update(boxes, [w * res / h, res], (res, res))
                     for t in online_targets:
                         label_counts[t.label] += 1
+
                         track_id = int(t.track_id)
                         id_text = '{}'.format(int(track_id)).zfill(5)
                         box_color = ((37 * track_id) % 255, (17 * track_id) % 255, (29 * track_id) % 255)
 
                         x, y, w, h = t.tlwh.astype(int)
-                        cv2.rectangle(original_img, (x, y), (x+w, y+h), box_color, 2)
+                        cv2.rectangle(img, (x, y), (x+w, y+h), box_color, 2)
                         if self.mw.configure.chkShowID.isChecked():
                             label_color = self.mw.configure.getLabel(t.label).color()
-                            cv2.putText(original_img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_color, 2)
-
+                            cv2.putText(img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_color, 2)
                 else:
+                    boxes = result.boxes.cpu().numpy()
                     for box in boxes:
-                        x1, y1, x2, y2 = box[:4].astype(int)
-                        cls = box[5].astype(int)
-                        label_counts[cls] += 1
-                        color = self.mw.configure.getLabel(cls).color()
-                        cv2.rectangle(original_img, (x1, y1), (x2, y2), color, 2)
+                        r = box.xyxy[0].astype(int)
+                        class_id = int(box.cls[0])
+                        color = self.mw.configure.getLabel(class_id).color()
+                        label_counts[class_id] += 1
+                        cv2.rectangle(img, r[:2], r[2:], color, 2)
 
-            for lbl in label_filter:
-                self.mw.configure.getLabel(lbl).setCount(label_counts[lbl])
+            for lbl in self.mw.configure.labels:
+                if lbl.isChecked():
+                    if self.mw.configure.getCountInterval() > 0:
+                        lbl.avgCount(label_counts[lbl.label()], q_size)
+                    else:
+                        lbl.setCount(label_counts[lbl.label()])
 
-            tmp = None
-            if self.mw.configure.chkAuto.isChecked():
-                tmp = self.get_auto_ckpt_filename()
-            else:
-                tmp = self.mw.configure.txtFilename.text()
-            if self.ckpt_file != tmp:
-                self.__init__(self.mw)
+            if  self.rts - self.count_interval_start >= interval * 1000:
+                self.count_interval_start = self.rts
+                if self.mw.configure.chkLogCount.isChecked():
+                    self.writeLog()
+                else:
+                    self.log_filename = ""
 
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
 
+    def writeLog(self):
+        if len(self.log_filename) == 0:
+            self.log_filename = self.mw.get_log_filename()
+            dir = os.path.dirname(self.log_filename)
+            if not os.path.exists(dir):
+                os.makedirs(dir)
+            if not os.path.exists(self.log_filename):
+                with open(self.log_filename, "a") as f:
+                    f.write("milliseconds, timestamp, class, count\n")
+        for lbl in self.mw.configure.labels:
+            if lbl.chkBox.isChecked():
+                if self.mw.configure.chkLogCount.isChecked():
+                    msg = str(self.rts) + " , "
+                    msg += datetime.now().strftime("%m/%d/%Y %H:%M:%S") + " , "
+                    msg += lbl.cmbLabel.currentText() + " , "
+                    msg += lbl.lblCount.text() + "\n"
+                    with open(self.log_filename, "a") as f: 
+                        f.write(msg)
+
     def get_auto_ckpt_filename(self):
-        return torch.hub.get_dir() +  "/checkpoints/" + self.mw.configure.cmbType.currentText() + ".pt"
+        return torch.hub.get_dir() +  "/checkpoints/" + self.mw.configure.getModelName()
 
-
```

### Comparing `onvif-gui-1.2.2/modules/video/yolox.py` & `onvif-gui-1.2.3/modules/video/yolox.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,25 +15,31 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 IMPORT_ERROR = ""
 try:
-    import cv2
     import os
     import sys
-    import numpy as np
-    from pathlib import Path
     from loguru import logger
-    logger.add("onvif-gui-errors.txt", retention="1 days")
+    if sys.platform == "win32":
+        filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/errors.txt"
+    else:
+        filename = os.environ['HOME'] + "/.cache/onvif-gui/errors.txt"
+    logger.add(filename, retention="1 days")
 
+    import cv2
+    import numpy as np
+    from pathlib import Path
+    from datetime import datetime
     from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
-    from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox
-    from PyQt6.QtCore import Qt
+    from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox, QLineEdit
+    from PyQt6.QtCore import Qt, QRegularExpression
+    from PyQt6.QtGui import QRegularExpressionValidator
 
     import torch
     from torchvision.transforms import functional
     import torch.nn as nn
     
     from yolox.models import YOLOX, YOLOPAFPN, YOLOXHead
     from yolox.utils import postprocess
@@ -51,15 +57,19 @@
         try:
             super().__init__()
             self.mw = mw
             self.name = MODULE_NAME
             self.autoKey = "Module/" + MODULE_NAME + "/autoDownload"
             self.trackKey = "Module/" + MODULE_NAME + "/track"
             self.showIDKey = "Module/" + MODULE_NAME + "/showID"
+            self.logCountKey = "Module/" + MODULE_NAME + "/logCount"
+            self.countIntervalKey = "Module/" + MODULE_NAME + "/countInterval"
 
+            self.mw.signals.started.connect(self.onMediaStarted)
+            
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
 
             self.txtFilename = FileSelector(mw, MODULE_NAME)
             self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
@@ -72,55 +82,93 @@
 
             self.chkShowID = QCheckBox("Show Object ID")
             self.chkShowID.setChecked(int(self.mw.settings.value(self.showIDKey, 1)))
             self.chkShowID.stateChanged.connect(self.chkShowIDClicked)
 
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
 
+            self.chkShowID.setVisible(self.chkTrack.isChecked())
+
+            pnlCount = QWidget()
+            lblCount = QLabel("Count Interval (seconds)")
+            self.txtCountInterval = QLineEdit()
+            self.txtCountInterval.setText(self.mw.settings.value(self.countIntervalKey, ""))
+            self.txtCountInterval.textChanged.connect(self.countIntervalChanged)
+            numRegex = QRegularExpression("[0-9]*")
+            numValidator = QRegularExpressionValidator(numRegex, self)
+            self.txtCountInterval.setValidator(numValidator)        
+            self.chkLogCount = QCheckBox("Log Counts")
+            self.chkLogCount.setChecked(int(self.mw.settings.value(self.logCountKey, 0)))
+            self.chkLogCount.stateChanged.connect(self.chkLogCountClicked)
+            lytCount = QGridLayout(pnlCount)
+            lytCount.addWidget(lblCount,              0, 0, 1, 1)
+            lytCount.addWidget(self.txtCountInterval, 0, 1, 1, 1)
+            lytCount.addWidget(self.chkLogCount,      0, 2, 1, 1)
+            lytCount.setContentsMargins(0, 0, 0, 0)
+
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
                 self.labels.append(LabelSelector(mw, MODULE_NAME, i+1))
             pnlLabels = QWidget()
             lytLabels = QGridLayout(pnlLabels)
-            lblPanel = QLabel("Select classes to be identified")
+            lblPanel = QLabel("Select classes to be identified and counted")
             lblPanel.setAlignment(Qt.AlignmentFlag.AlignCenter)
             lytLabels.addWidget(lblPanel,        0, 0, 1, 1)
             for i in range(number_of_labels):
                 lytLabels.addWidget(self.labels[i], i+1, 0, 1, 1)
             lytLabels.setContentsMargins(0, 0, 0, 0)
 
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.chkAuto,      0, 0, 1, 2)
             lytMain.addWidget(self.cmbType,      1, 0, 1, 2)
             lytMain.addWidget(self.txtFilename,  2, 0, 1, 2)
             lytMain.addWidget(self.cmbRes,       3, 0, 1, 2)
             lytMain.addWidget(self.sldConfThre,  4, 0, 1, 2)
             lytMain.addWidget(self.chkTrack,     6, 0, 1, 1)
             lytMain.addWidget(self.chkShowID,    6, 1, 1, 1)
-            lytMain.addWidget(pnlLabels,         7, 0, 1, 2)
-            lytMain.addWidget(QLabel(),          8, 0, 1, 2)
-            lytMain.setRowStretch(8, 10)
+            lytMain.addWidget(pnlCount,          7, 0, 1, 2)
+            lytMain.addWidget(pnlLabels,         8, 0, 1, 2)
+            lytMain.addWidget(QLabel(),          9, 0, 1, 2)
+            lytMain.setRowStretch(9, 10)
+
+            self.first_pass = True
 
             if len(IMPORT_ERROR) > 0:
                 QMessageBox.critical(None, MODULE_NAME + " Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
 
         except:
             logger.exception(MODULE_NAME + " configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
     def chkTrackClicked(self, state):
         self.mw.settings.setValue(self.trackKey, state)
+        self.chkShowID.setVisible(state)
 
     def chkShowIDClicked(self, state):
         self.mw.settings.setValue(self.showIDKey, state)
 
+    def chkLogCountClicked(self, state):
+        self.mw.settings.setValue(self.logCountKey, state)
+
+    def countIntervalChanged(self, txt):
+        self.mw.settings.setValue(self.countIntervalKey, txt)
+
+    def getCountInterval(self):
+        result = 0
+        if len(self.txtCountInterval.text()) > 0:
+            result = int(self.txtCountInterval.text())
+        return result
+
+    def onMediaStarted(self, n):
+        self.first_pass = True
+
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
 
             if self.mw.configure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
@@ -163,39 +211,52 @@
 
             res = int(self.mw.configure.cmbRes.currentText())
             self.model(torch.zeros(1, 3, res, res).to(self.device))
 
             self.track_thresh = self.mw.configure.sldConfThre.value()
             self.track_buffer = 30
             self.match_thresh = 0.8
-            self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
+            framerate = self.mw.getVideoFrameRate()
+            if framerate == 0: framerate = 30
+            self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh, frame_rate=framerate)
+
+            self.count_interval_start = 0
+            self.rts = 0
+            self.log_filename = ""
 
             self.mw.signals.hideWait.emit()
 
         except:
             logger.exception(MODULE_NAME + " initialization failure")
             self.mw.signals.hideWait.emit()
             self.mw.signals.error.emit(MODULE_NAME + " initialization failure, please check logs for details")
 
     def __call__(self, F):
         try:
             img = np.array(F, copy=False)
+            self.rts = F.m_rts
 
             if self.mw.configure.name != MODULE_NAME:
                 return
             
+            if self.mw.configure.first_pass:
+                self.count_interval_start = self.rts
+                self.mw.configure.first_pass = False
+                self.log_filename = ""
+
             res = int(self.mw.configure.cmbRes.currentText())
             test_size = (res, res)
             ratio = min(test_size[0] / img.shape[0], test_size[1] / img.shape[1])
             inf_shape = (int(img.shape[0] * ratio), int(img.shape[1] * ratio))
             bottom = test_size[0] - inf_shape[0]
             side = test_size[1] - inf_shape[1]
             pad = (0, 0, side, bottom)
 
-            timg = functional.to_tensor(img.copy()).to(self.device)
+            #timg = functional.to_tensor(img.copy()).to(self.device)
+            timg = functional.to_tensor(img).to(self.device)
             timg *= 255
             timg = functional.resize(timg, inf_shape)
             timg = functional.pad(timg, pad, 114)
             timg = timg.unsqueeze(0)
 
             if self.mw.configure.chkTrack.isChecked():
                 confthre = 0.001
@@ -219,15 +280,17 @@
                     labels = output[:, 6].numpy().astype(int)
                     mask = np.in1d(labels, label_filter)
                     output = output[mask]
                     output = output.cpu().numpy()
                     
                     if self.track_thresh != self.mw.configure.sldConfThre.value():
                         self.track_thresh = self.mw.configure.sldConfThre.value()
-                        self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
+                        framerate = self.mw.getVideoFrameRate()
+                        if framerate == 0: framerate = 30
+                        self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh, frame_rate=framerate)
 
                     online_targets = self.tracker.update(output, [img.shape[0], img.shape[1]], test_size)
                     self.draw_track_boxes(img, online_targets)
                 else:
                     self.draw_plain_boxes(img, output, ratio)
 
             tmp = None
@@ -240,25 +303,40 @@
 
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
 
     def draw_plain_boxes(self, img, output, ratio):
+        interval = self.mw.configure.getCountInterval()
+        q_size = self.mw.getVideoFrameRate() * interval
+
         boxes = output[:, 0:4] / ratio
         labels = output[:, 6].numpy().astype(int)
+
         for lbl in self.mw.configure.labels:
             if lbl.chkBox.isChecked():
                 lbl_boxes = boxes[labels == lbl.label()].numpy().astype(int)
-                lbl.setCount(lbl_boxes.shape[0])
-
                 for box in lbl_boxes:
                     cv2.rectangle(img, (box[0], box[1]), (box[2], box[3]), lbl.color(), 2)
+                if self.mw.configure.getCountInterval() > 0:
+                    lbl.avgCount(lbl_boxes.shape[0], q_size)
+                else:
+                    lbl.setCount(lbl_boxes.shape[0])
+
+        if  self.rts - self.count_interval_start >= interval * 1000:
+            self.count_interval_start = self.rts
+            if self.mw.configure.chkLogCount.isChecked():
+                self.writeLog()
+            else:
+                self.log_filename = ""
 
     def draw_track_boxes(self, img, online_targets):
+        interval = self.mw.configure.getCountInterval()
+        q_size = self.mw.getVideoFrameRate() * interval
         label_colors = {}
         count = {}
 
         for lbl in self.mw.configure.labels:
             if lbl.chkBox.isChecked():
                 label_colors[lbl.label()] = lbl.color()
                 count[lbl.label()] = 0
@@ -274,15 +352,44 @@
             x, y, w, h = tlwh.astype(int)
             cv2.rectangle(img, (x, y), (x+w, y+h), color, 2)
             if self.mw.configure.chkShowID.isChecked():
                 cv2.putText(img, id_text, (x, y), cv2.FONT_HERSHEY_PLAIN, 2, label_colors[t.label], 2)
 
         for lbl in self.mw.configure.labels:
             if lbl.chkBox.isChecked():
-                lbl.setCount(count[lbl.label()])
+                if self.mw.configure.getCountInterval() > 0:
+                    lbl.avgCount(count[lbl.label()], q_size)
+                else:
+                    lbl.setCount(count[lbl.label()])
+
+        if  self.rts - self.count_interval_start >= interval * 1000:
+            self.count_interval_start = self.rts
+            if self.mw.configure.chkLogCount.isChecked():
+                self.writeLog()
+            else:
+                self.log_filename = ""
+
+    def writeLog(self):
+        if len(self.log_filename) == 0:
+            self.log_filename = self.mw.get_log_filename()
+            dir = os.path.dirname(self.log_filename)
+            if not os.path.exists(dir):
+                os.makedirs(dir)
+            if not os.path.exists(self.log_filename):
+                with open(self.log_filename, "a") as f:
+                    f.write("milliseconds, timestamp, class, count\n")
+        for lbl in self.mw.configure.labels:
+            if lbl.chkBox.isChecked():
+                if self.mw.configure.chkLogCount.isChecked():
+                    msg = str(self.rts) + " , "
+                    msg += datetime.now().strftime("%m/%d/%Y %H:%M:%S") + " , "
+                    msg += lbl.cmbLabel.currentText() + " , "
+                    msg += lbl.lblCount.text() + "\n"
+                    with open(self.log_filename, "a") as f: 
+                        f.write(msg)
 
     def get_auto_ckpt_filename(self):
         return torch.hub.get_dir() + "/checkpoints/" + self.mw.configure.cmbType.currentText() + ".pth"
 
     def get_model(self, num_classes, depth, width, act):
         def init_yolo(M):
             for m in M.modules():
@@ -293,8 +400,8 @@
         in_channels = [256, 512, 1024]
         backbone = YOLOPAFPN(depth, width, in_channels=in_channels)
         head = YOLOXHead(num_classes, width, in_channels=in_channels)
         model = YOLOX(backbone, head)
 
         model.apply(init_yolo)
         model.head.initialize_biases(1e-2)
-        return model
+        return model
```

### Comparing `onvif-gui-1.2.2/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.2.3/onvif_gui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 gui/resources/fast-forward_lo.png
 gui/resources/mute.png
 gui/resources/mute_hi.png
 gui/resources/mute_lo.png
 gui/resources/next.png
 gui/resources/next_hi.png
 gui/resources/next_lo.png
+gui/resources/onvif-gui.ico
 gui/resources/onvif-gui.png
 gui/resources/pause.png
 gui/resources/pause_hi.png
 gui/resources/pause_lo.png
 gui/resources/play.png
 gui/resources/play_hi.png
 gui/resources/play_lo.png
```

### Comparing `onvif-gui-1.2.2/pyproject.toml` & `onvif-gui-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.2.2"  
+version = "1.2.3"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
```

### Comparing `onvif-gui-1.2.2/setup.py` & `onvif-gui-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.2.2",
+    version="1.2.3",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.2.2/tracker/basetrack.py` & `onvif-gui-1.2.3/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/tracker/byte_tracker.py` & `onvif-gui-1.2.3/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/tracker/kalman_filter.py` & `onvif-gui-1.2.3/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/tracker/matching.py` & `onvif-gui-1.2.3/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/models/common.py` & `onvif-gui-1.2.3/yolov7/models/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/models/experimental.py` & `onvif-gui-1.2.3/yolov7/models/experimental.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/models/yolo.py` & `onvif-gui-1.2.3/yolov7/models/yolo.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/activations.py` & `onvif-gui-1.2.3/yolov7/utils/activations.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/add_nms.py` & `onvif-gui-1.2.3/yolov7/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/autoanchor.py` & `onvif-gui-1.2.3/yolov7/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/datasets.py` & `onvif-gui-1.2.3/yolov7/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/general.py` & `onvif-gui-1.2.3/yolov7/utils/general.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/google_utils.py` & `onvif-gui-1.2.3/yolov7/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/loss.py` & `onvif-gui-1.2.3/yolov7/utils/loss.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/metrics.py` & `onvif-gui-1.2.3/yolov7/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/plots.py` & `onvif-gui-1.2.3/yolov7/utils/plots.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolov7/utils/torch_utils.py` & `onvif-gui-1.2.3/yolov7/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/__init__.py` & `onvif-gui-1.2.3/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/build.py` & `onvif-gui-1.2.3/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/darknet.py` & `onvif-gui-1.2.3/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/losses.py` & `onvif-gui-1.2.3/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/network_blocks.py` & `onvif-gui-1.2.3/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/yolo_fpn.py` & `onvif-gui-1.2.3/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/yolo_head.py` & `onvif-gui-1.2.3/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/yolo_pafpn.py` & `onvif-gui-1.2.3/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/models/yolox.py` & `onvif-gui-1.2.3/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.2/yolox/utils/utils.py` & `onvif-gui-1.2.3/yolox/utils/utils.py`

 * *Files identical despite different names*

