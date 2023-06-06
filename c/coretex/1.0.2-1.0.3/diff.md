# Comparing `tmp/coretex-1.0.2.tar.gz` & `tmp/coretex-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coretex-1.0.2.tar", last modified: Wed May 31 07:58:38 2023, max compression
+gzip compressed data, was "coretex-1.0.3.tar", last modified: Tue Jun  6 11:51:09 2023, max compression
```

## Comparing `coretex-1.0.2.tar` & `coretex-1.0.3.tar`

### file list

```diff
@@ -1,180 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.370583 coretex-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-05-31 07:58:21.000000 coretex-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-31 07:58:38.366583 coretex-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-31 07:58:21.000000 coretex-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-31 07:58:21.000000 coretex-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:58:38.370583 coretex-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.330583 coretex-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.334583 coretex-1.0.2/src/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.338583 coretex-1.0.2/src/coretex/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/cache/cache_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.338583 coretex-1.0.2/src/coretex/codable/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/codable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/codable/codable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/codable/descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.338583 coretex-1.0.2/src/coretex/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.338583 coretex-1.0.2/src/coretex/coretex/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.338583 coretex-1.0.2/src/coretex/coretex/annotation/image/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/annotation/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/annotation/image/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/annotation/image/classes_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/annotation/image/coretex_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.342583 coretex-1.0.2/src/coretex/coretex/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converter_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.342583 coretex-1.0.2/src/coretex/coretex/conversion/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/city_scape_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/coco_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/create_ml_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/human_segmentation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/label_me_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.342583 coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/voc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/conversion/converters/yolo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.346583 coretex-1.0.2/src/coretex/coretex/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.346583 coretex-1.0.2/src/coretex/coretex/dataset/computer_vision_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.346583 coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.346583 coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.350583 coretex-1.0.2/src/coretex/coretex/dataset/image_segmentation_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/local_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/network_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.350583 coretex-1.0.2/src/coretex/coretex/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/executing_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.350583 coretex-1.0.2/src/coretex/coretex/experiment/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/metric_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.354583 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/experiment/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.354583 coretex-1.0.2/src/coretex/coretex/model/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.354583 coretex-1.0.2/src/coretex/coretex/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/any_local_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.354583 coretex-1.0.2/src/coretex/coretex/sample/computer_vision_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/computer_vision_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.358583 coretex-1.0.2/src/coretex/coretex/sample/custom_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/custom_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/custom_sample/custom_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/custom_sample/custom_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/custom_sample/local_custom_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.358583 coretex-1.0.2/src/coretex/coretex/sample/image_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/image_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/image_sample/image_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/image_sample/image_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/image_sample/image_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/image_sample/local_image_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.358583 coretex-1.0.2/src/coretex/coretex/sample/image_segmentation_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/image_segmentation_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/local_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/network_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/sample/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.358583 coretex-1.0.2/src/coretex/coretex/space/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/space/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/space/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/space/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/coretex/space/space_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.362583 coretex-1.0.2/src/coretex/folder_management/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/folder_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/folder_management/folder_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.362583 coretex-1.0.2/src/coretex/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/logging/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/logging/log_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.362583 coretex-1.0.2/src/coretex/networking/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/chunk_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/network_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/network_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/network_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/requests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/networking/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.366583 coretex-1.0.2/src/coretex/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/nlp/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/nlp/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/nlp/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.366583 coretex-1.0.2/src/coretex/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/project/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/project/calculate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/project/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/project/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/project/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.366583 coretex-1.0.2/src/coretex/qiime2/
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/qiime2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/qiime2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.366583 coretex-1.0.2/src/coretex/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/threading/threaded_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.366583 coretex-1.0.2/src/coretex/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/utils/console_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-31 07:58:21.000000 coretex-1.0.2/src/coretex/utils/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.338583 coretex-1.0.2/src/coretex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-31 07:58:38.000000 coretex-1.0.2/src/coretex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-31 07:58:38.000000 coretex-1.0.2/src/coretex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:58:38.000000 coretex-1.0.2/src/coretex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 07:58:38.000000 coretex-1.0.2/src/coretex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 07:58:38.000000 coretex-1.0.2/src/coretex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.166153 coretex-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-06-06 11:50:57.000000 coretex-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-06 11:51:09.166153 coretex-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-06 11:50:57.000000 coretex-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-06 11:50:57.000000 coretex-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:51:09.166153 coretex-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.142153 coretex-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.146153 coretex-1.0.3/src/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.150153 coretex-1.0.3/src/coretex/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/cache/cache_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.150153 coretex-1.0.3/src/coretex/codable/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/codable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/codable/codable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/codable/descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.150153 coretex-1.0.3/src/coretex/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.150153 coretex-1.0.3/src/coretex/coretex/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.150153 coretex-1.0.3/src/coretex/coretex/annotation/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/annotation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/annotation/image/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/annotation/image/classes_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/annotation/image/coretex_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.150153 coretex-1.0.3/src/coretex/coretex/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converter_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.154153 coretex-1.0.3/src/coretex/coretex/conversion/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/city_scape_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/create_ml_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/human_segmentation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/label_me_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.154153 coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/voc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/conversion/converters/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.154153 coretex-1.0.3/src/coretex/coretex/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.154153 coretex-1.0.3/src/coretex/coretex/dataset/computer_vision_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.154153 coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.154153 coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.158153 coretex-1.0.3/src/coretex/coretex/dataset/image_segmentation_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/network_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.158153 coretex-1.0.3/src/coretex/coretex/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/executing_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.158153 coretex-1.0.3/src/coretex/coretex/experiment/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/metric_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.158153 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/experiment/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.158153 coretex-1.0.3/src/coretex/coretex/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.162153 coretex-1.0.3/src/coretex/coretex/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/any_local_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.162153 coretex-1.0.3/src/coretex/coretex/sample/computer_vision_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/computer_vision_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.162153 coretex-1.0.3/src/coretex/coretex/sample/custom_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/custom_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/custom_sample/custom_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/custom_sample/custom_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/custom_sample/local_custom_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.162153 coretex-1.0.3/src/coretex/coretex/sample/image_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/image_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/image_sample/image_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/image_sample/image_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/image_sample/image_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/image_sample/local_image_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.162153 coretex-1.0.3/src/coretex/coretex/sample/image_segmentation_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/image_segmentation_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/local_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/network_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/sample/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.162153 coretex-1.0.3/src/coretex/coretex/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/space/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/space/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/coretex/space/space_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.162153 coretex-1.0.3/src/coretex/folder_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/folder_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/folder_management/folder_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.162153 coretex-1.0.3/src/coretex/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/logging/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/logging/log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.166153 coretex-1.0.3/src/coretex/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/chunk_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/network_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/network_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/network_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/requests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/networking/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.166153 coretex-1.0.3/src/coretex/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/nlp/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/nlp/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/nlp/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.166153 coretex-1.0.3/src/coretex/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/project/calculate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/project/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/project/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/project/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.166153 coretex-1.0.3/src/coretex/qiime2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/qiime2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/qiime2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.166153 coretex-1.0.3/src/coretex/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/threading/threaded_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.166153 coretex-1.0.3/src/coretex/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/utils/console_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-06 11:50:57.000000 coretex-1.0.3/src/coretex/utils/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:51:09.150153 coretex-1.0.3/src/coretex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-06 11:51:09.000000 coretex-1.0.3/src/coretex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-06 11:51:09.000000 coretex-1.0.3/src/coretex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:51:09.000000 coretex-1.0.3/src/coretex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 11:51:09.000000 coretex-1.0.3/src/coretex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 11:51:09.000000 coretex-1.0.3/src/coretex.egg-info/top_level.txt
```

### Comparing `coretex-1.0.2/LICENSE` & `coretex-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/PKG-INFO` & `coretex-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
-Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>, Igor Perić <igor@coretex.ai>
+Maintainer-email: Igor Perić <igor@coretex.ai>, Duško Mirković <dmirkovic@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Linter code check](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml/badge.svg?branch=develop)](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml)
```

### Comparing `coretex-1.0.2/README.md` & `coretex-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/pyproject.toml` & `coretex-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coretex"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
 ]
 maintainers = [
+  { name="Igor Perić", email="igor@coretex.ai" },
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
   { name="Jovica Zarić", email="jzaric@coretex.ai" },
   { name="Darko Zarić", email="dzaric@coretex.ai" },
   { name="Bogdan Tintor", email="btintor@coretex.ai" },
   { name="Alex Maslennikov", email="alex@coretex.ai" },
-  { name="Igor Perić", email="igor@coretex.ai" },
 ]
 description = "A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "requests",
   "inflection",
   "pillow",
   "numpy",
```

### Comparing `coretex-1.0.2/src/coretex/__init__.py` & `coretex-1.0.3/src/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/_configuration.py` & `coretex-1.0.3/src/coretex/_configuration.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/_logger.py` & `coretex-1.0.3/src/coretex/_logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/cache/__init__.py` & `coretex-1.0.3/src/coretex/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/cache/cache_module.py` & `coretex-1.0.3/src/coretex/cache/cache_module.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/codable/__init__.py` & `coretex-1.0.3/src/coretex/codable/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/codable/codable.py` & `coretex-1.0.3/src/coretex/codable/codable.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/codable/descriptor.py` & `coretex-1.0.3/src/coretex/codable/descriptor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/__init__.py` & `coretex-1.0.3/src/coretex/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/annotation/__init__.py` & `coretex-1.0.3/src/coretex/coretex/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/annotation/image/__init__.py` & `coretex-1.0.3/src/coretex/coretex/annotation/image/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/annotation/image/bbox.py` & `coretex-1.0.3/src/coretex/coretex/annotation/image/bbox.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/annotation/image/classes_format.py` & `coretex-1.0.3/src/coretex/coretex/annotation/image/classes_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/annotation/image/coretex_format.py` & `coretex-1.0.3/src/coretex/coretex/annotation/image/coretex_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/__init__.py` & `coretex-1.0.3/src/coretex/coretex/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/base_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/base_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converter_processor_factory.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converter_processor_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/__init__.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/city_scape_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/city_scape_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/coco_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/coco_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/create_ml_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/create_ml_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/human_segmentation_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/human_segmentation_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/label_me_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/label_me_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/__init__.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/pascal/shared.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/pascal/shared.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/voc_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/voc_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/conversion/converters/yolo_converter.py` & `coretex-1.0.3/src/coretex/coretex/conversion/converters/yolo_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/__init__.py` & `coretex-1.0.3/src/coretex/coretex/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py` & `coretex-1.0.3/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/__init__.py` & `coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/base.py` & `coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/__init__.py` & `coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/base.py` & `coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/image_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py` & `coretex-1.0.3/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py` & `coretex-1.0.3/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/local_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/local_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/network_dataset.py` & `coretex-1.0.3/src/coretex/coretex/dataset/network_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/dataset/utils.py` & `coretex-1.0.3/src/coretex/coretex/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/__init__.py` & `coretex-1.0.3/src/coretex/coretex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/artifact.py` & `coretex-1.0.3/src/coretex/coretex/experiment/artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -20,15 +20,15 @@
 from enum import IntEnum
 from typing import Optional, Dict, List
 from pathlib import Path
 
 import os
 
 from ...codable import Codable, KeyDescriptor
-from ...networking import networkManager, RequestType
+from ...networking import networkManager, RequestType, FileData
 from ...folder_management import FolderManager
 from ...utils import guessMimeType
 
 
 class ArtifactType(IntEnum):
 
     """
@@ -136,15 +136,15 @@
             # If guessing fails, fallback to binary type
             try:
                 mimeType = guessMimeType(localFilePath)
             except:
                 mimeType = "application/octet-stream"
 
         files = [
-            ("file", ("file", open(localFilePath, "rb"), mimeType))
+            FileData.createFromPath("file", localFilePath, mimeType = mimeType)
         ]
 
         parameters = {
             "model_queue_id": experimentId,
             "path": remoteFilePath
         }
```

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/executing_experiment.py` & `coretex-1.0.3/src/coretex/coretex/experiment/executing_experiment.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/experiment.py` & `coretex-1.0.3/src/coretex/coretex/experiment/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,16 +386,14 @@
         parameters: Optional[List[Dict[str, Any]]] = None
     ) -> Self:
         """
             Starts an Experiment on Coretex.ai with the provided parameters
 
             Parameters
             ----------
-            datasetId : int
-                id of dataset that is being used for starting custom Experiment
             projectId : int
                 id of project that is being used for starting custom Experiment
             nodeId : Union[int, str]
                 id of node that is being used for starting custom Experiment
             name : Optional[str]
                 name of Experiment
             description : Optional[str]
```

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/__init__.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/metric.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/metric_factory.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/metric_type.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/metrics/utils.py` & `coretex-1.0.3/src/coretex/coretex/experiment/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/parameters.py` & `coretex-1.0.3/src/coretex/coretex/experiment/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -158,14 +158,20 @@
                 return False
 
             return all(
                 isinstance(element, self.dataType.listType)
                 for element in self.value
             )
 
+        # Dataset parameter is an integer under the hood, and in python bool is a subclass
+        # of integer. To avoid assinging boolean values to dataset parameters we have to explicitly
+        # check if the value which was passed in for dataset is a bool.
+        if self.dataType == ExperimentParameterType.dataset and isinstance(self.value, bool):
+            return False
+
         return any(isinstance(self.value, dataType) for dataType in self.dataType.types)
 
     def generateTypeDescription(self) -> str:
         if not self.dataType.isList or self.value is None:
             return type(self.value).__name__
 
         elementTypes = ", ".join({type(value).__name__ for value in self.value})
```

### Comparing `coretex-1.0.2/src/coretex/coretex/experiment/status.py` & `coretex-1.0.3/src/coretex/coretex/experiment/status.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/model/__init__.py` & `coretex-1.0.3/src/coretex/coretex/model/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/model/model.py` & `coretex-1.0.3/src/coretex/coretex/model/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Any, Dict
+from typing import Any, Dict, Union
 from typing_extensions import Self
 from datetime import datetime
 from zipfile import ZipFile
+from pathlib import Path
 
 import os
-import shutil
 import json
 import logging
 
-from ...networking import networkManager, NetworkObject
+from ...networking import networkManager, NetworkObject, FileData
 from ...folder_management import FolderManager
 from ...codable import KeyDescriptor
 
 
 class Model(NetworkObject):
 
     """
@@ -196,26 +196,25 @@
             endpoint=f"model/download?id={self.id}",
             destination=modelZipDestination
         )
 
         if response.hasFailed():
             logging.getLogger("coretexpylib").info(">> [Coretex] Failed to download the model")
 
-        zipFile = ZipFile(modelZipDestination)
-        zipFile.extractall(modelFolderDestination)
-        zipFile.close()
+        with ZipFile(modelZipDestination) as zipFile:
+            zipFile.extractall(modelFolderDestination)
 
-    def upload(self, path: str) -> bool:
+    def upload(self, path: Union[Path, str]) -> bool:
         """
-            Uploads the model zip file to Coretex.ai
+            Uploads the provided model folder as zip file to Coretex.ai
 
             Parameters
             ----------
-            path : str
-                Path to the saved model dir
+            path : Union[Path, str]
+                Path to the saved model directory
 
             Returns
             -------
             bool -> True if model data uploaded successfully, False if model data upload has failed
 
 
             Example
@@ -232,21 +231,30 @@
             >>> if not model.upload("path/to/model-dir"):
                     print("Failed to upload model")
         """
 
         if self.isDeleted:
             return False
 
-        logging.getLogger("coretexpylib").info(">> [Coretex] Uploading model file...")
+        if isinstance(path, str):
+            path = Path(path)
 
-        shutil.make_archive(path, "zip", path)
+        if not path.is_dir():
+            raise ValueError(">> [Coretex] \"path\" must be a directory")
 
-        files = {
-            ("file", open(f"{path}.zip", "rb"))
-        }
+        logging.getLogger("coretexpylib").info(">> [Coretex] Uploading model file...")
+
+        zipPath = path.with_suffix(".zip")
+        with ZipFile(zipPath, "w") as zipFile:
+            for value in path.iterdir():
+                zipFile.write(value, value.name)
+
+        files = [
+            FileData.createFromPath("file", zipPath)
+        ]
 
         parameters = {
             "id": self.id
         }
 
         response = networkManager.genericUpload("model/upload", files, parameters)
         if response.hasFailed():
```

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/__init__.py` & `coretex-1.0.3/src/coretex/coretex/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/any_local_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/any_local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/computer_vision_sample/__init__.py` & `coretex-1.0.3/src/coretex/coretex/sample/computer_vision_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/custom_sample/__init__.py` & `coretex-1.0.3/src/coretex/coretex/sample/custom_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/custom_sample/custom_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/custom_sample/custom_sample.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -19,14 +19,15 @@
 from typing_extensions import Self
 from pathlib import Path
 
 from .custom_sample_data import CustomSampleData
 from .local_custom_sample import LocalCustomSample
 from ..network_sample import NetworkSample
 from ....networking import networkManager, ChunkUploadSession, MAX_CHUNK_SIZE
+from ....utils.file import isArchive
 
 
 class CustomSample(NetworkSample[CustomSampleData], LocalCustomSample):
 
     """
         Represents the custom Sample object from Coretex.ai\n
         Custom samples are used when working with Other Task\n
@@ -37,31 +38,28 @@
         NetworkSample.__init__(self)
 
     @classmethod
     def createCustomSample(
         cls,
         name: str,
         datasetId: int,
-        filePath: Union[Path, str],
-        mimeType: Optional[str] = None
+        filePath: Union[Path, str]
     ) -> Optional[Self]:
         """
             Creates a new custom sample with specified properties\n
             For creating custom sample, sample must be an archive
 
             Parameters
             ----------
             name : str
                 sample name
             datasetId : int
                 id of dataset to which the sample will be added
-            filePath : str
+            filePath : Union[Path, str]
                 path to the sample
-            mimeType : Optional[str]
-                mime type of the file, if None mime type guessing will be performed
 
             Returns
             -------
             Optional[Self] -> The created sample object or None if creation failed
 
             Raises
             ------
@@ -73,23 +71,27 @@
             >>> from coretex import CustomSample
             \b
             >>> sample = CustomSample.createCustomSample("name", 1023, "path/to/file")
             >>> if sample is None:
                     print("Failed to create custom sample")
         """
 
-        uploadSession = ChunkUploadSession(MAX_CHUNK_SIZE, filePath, mimeType)
+        if isinstance(filePath, str):
+            filePath = Path(filePath)
+
+        if not isArchive(filePath):
+            raise ValueError(">> [Coretex] File must be an archive [.zip, .tar, .tar.gz]")
+
+        uploadSession = ChunkUploadSession(MAX_CHUNK_SIZE, filePath)
         uploadId = uploadSession.run()
 
-        parameters = [
-            ("name",       (None, name)),
-            ("dataset_id", (None, datasetId)),
-            ("file_id",    (None, uploadId))
-        ]
-
-        # files parameter can accept parameters that are not files, this way we can
-        # send form-data requests without actual files
-        response = networkManager.genericUpload("session/import", files = parameters)
+        parameters = {
+            "name": name,
+            "dataset_id": datasetId,
+            "file_id": uploadId
+        }
+
+        response = networkManager.genericFormData("session/import", parameters)
         if response.hasFailed():
             return None
 
         return cls.decode(response.json)
```

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/custom_sample/custom_sample_data.py` & `coretex-1.0.3/src/coretex/coretex/sample/custom_sample/custom_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/custom_sample/local_custom_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/custom_sample/local_custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/image_sample/__init__.py` & `coretex-1.0.3/src/coretex/coretex/sample/image_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/image_sample/image_format.py` & `coretex-1.0.3/src/coretex/coretex/sample/image_sample/image_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/image_sample/image_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/image_sample/image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/image_sample/image_sample_data.py` & `coretex-1.0.3/src/coretex/coretex/sample/image_sample/image_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/image_sample/local_image_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/image_sample/local_image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/image_segmentation_sample/__init__.py` & `coretex-1.0.3/src/coretex/coretex/sample/image_segmentation_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/local_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/network_sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/network_sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -20,15 +20,15 @@
 from pathlib import Path
 
 import os
 
 from .sample import Sample
 from ..space import SpaceTask
 from ...codable import KeyDescriptor
-from ...networking import NetworkObject, networkManager
+from ...networking import NetworkObject, networkManager, FileData
 from ...folder_management import FolderManager
 from ...utils import guessMimeType
 
 
 SampleDataType = TypeVar("SampleDataType")
 
 
@@ -85,41 +85,37 @@
 
             Parametrs
             ---------
             endpoint : str
                 API endpoint
             parameters : Dict[str, Any]
                 parameters which will be sent as request body
-            filePath : str
+            filePath : Union[Path, str]
                 path to sample
             mimeType : Optional[str]
                 mimeType (not required)
 
             Returns
             -------
             Optional[Self] -> created sample object if request
             was successful, None otherwise
         """
 
         if isinstance(filePath, str):
             filePath = Path(filePath)
 
-        if mimeType is None:
-            mimeType = guessMimeType(str(filePath))
+        files = [
+            FileData.createFromPath("file", filePath, mimeType = mimeType)
+        ]
+
+        response = networkManager.genericUpload("session/import", files, parameters)
+        if response.hasFailed():
+            return None
 
-        with filePath.open("rb") as sampleFile:
-            files = [
-                ("file", (filePath.stem, sampleFile, mimeType))
-            ]
-
-            response = networkManager.genericUpload("session/import", files, parameters)
-            if response.hasFailed():
-                return None
-
-            return cls.decode(response.json)
+        return cls.decode(response.json)
 
     def download(self, ignoreCache: bool = False) -> bool:
         """
             Downloads sample from Coretex.ai
 
             Returns
             -------
```

### Comparing `coretex-1.0.2/src/coretex/coretex/sample/sample.py` & `coretex-1.0.3/src/coretex/coretex/sample/sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/space/__init__.py` & `coretex-1.0.3/src/coretex/coretex/space/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/space/base.py` & `coretex-1.0.3/src/coretex/coretex/space/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/space/project.py` & `coretex-1.0.3/src/coretex/coretex/space/project.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/space/space.py` & `coretex-1.0.3/src/coretex/coretex/space/space.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/coretex/space/space_task.py` & `coretex-1.0.3/src/coretex/coretex/space/space_task.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/folder_management/__init__.py` & `coretex-1.0.3/src/coretex/folder_management/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/folder_management/folder_manager.py` & `coretex-1.0.3/src/coretex/folder_management/folder_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/logging/__init__.py` & `coretex-1.0.3/src/coretex/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/logging/log.py` & `coretex-1.0.3/src/coretex/logging/log.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/logging/log_severity.py` & `coretex-1.0.3/src/coretex/logging/log_severity.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/logging/logger.py` & `coretex-1.0.3/src/coretex/logging/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -20,15 +20,14 @@
 from typing import Optional, Any, List
 from threading import Lock, Thread
 from logging import LogRecord, StreamHandler
 
 import time
 import sys
 import logging
-import copy
 
 from .log import Log
 from .log_severity import LogSeverity
 from ..networking import networkManager, RequestType, RequestFailedError
 
 
 # Logs from library that is being used for making api requests is causing project to freeze because
@@ -106,82 +105,80 @@
                     cls.__instance = LogHandler(sys.stdout)
 
         return cls.__instance
 
     def __init__(self, stream: Any) -> None:
         super().__init__(stream)
 
+        # Locks appending and flushing of the pending logs,
+        # reset will not be locked to avoid waiting on flush
+        # if the request for uploading logs will timeout
+        self.__pendingLogsLock = Lock()
         self.__pendingLogs: List[Log] = []
+
         self.__uploadWorker = _LoggerUploadWorker()
 
         self.currentExperimentId: Optional[int] = None
         self.severity = LogSeverity.info
 
         self.__uploadWorker.start()
 
     def __restartUploadWorker(self) -> None:
         if self.__uploadWorker.is_alive():
             raise RuntimeError(">> [Coretex] Upload worker is already running")
 
         self.__uploadWorker = _LoggerUploadWorker()
         self.__uploadWorker.start()
 
-    def __clearLogs(self, snapshot: List[Log]) -> None:
-        for log in snapshot:
-            try:
-                self.__pendingLogs.remove(log)
-            except ValueError:
-                continue
-
     def emit(self, record: LogRecord) -> None:
         super().emit(record)
 
-        if record.name in IGNORED_LOGGERS:
-            return
+        with self.__pendingLogsLock:
+            if record.name in IGNORED_LOGGERS:
+                return
 
-        if not self.__uploadWorker.is_alive():
-            self.__restartUploadWorker()
+            if not self.__uploadWorker.is_alive():
+                self.__restartUploadWorker()
 
-        severity = LogSeverity.fromStd(record.levelno)
-        log = Log.create(record.message, severity)
+            severity = LogSeverity.fromStd(record.levelno)
+            log = Log.create(record.message, severity)
 
-        self.__pendingLogs.append(log)
+            self.__pendingLogs.append(log)
 
     def flushLogs(self) -> bool:
         """
             Uploads all currently stored logs to Coretex backend
 
             Returns
             -------
             bool -> True if the upload is successful, False otherwise
         """
 
-        if len(self.__pendingLogs) == 0:
-            return True
-
-        if self.currentExperimentId is None:
-            self.__pendingLogs.clear()
-            return True
-
-        snapshot = copy.copy(self.__pendingLogs)
-
-        response = networkManager.genericJSONRequest(
-            endpoint = "model-queue/add-console-log",
-            requestType = RequestType.post,
-            parameters = {
-                "model_queue_id": self.currentExperimentId,
-                "logs": [log.encode() for log in snapshot]
-            }
-        )
-
-        # Only clear logs if they were successfully uploaded to coretex
-        if not response.hasFailed():
-            self.__clearLogs(snapshot)
+        with self.__pendingLogsLock:
+            if len(self.__pendingLogs) == 0:
+                return True
+
+            if self.currentExperimentId is None:
+                self.__pendingLogs.clear()
+                return True
+
+            response = networkManager.genericJSONRequest(
+                endpoint = "model-queue/add-console-log",
+                requestType = RequestType.post,
+                parameters = {
+                    "model_queue_id": self.currentExperimentId,
+                    "logs": [log.encode() for log in self.__pendingLogs]
+                }
+            )
+
+            # Only clear logs if they were successfully uploaded to coretex
+            if not response.hasFailed():
+                self.__pendingLogs.clear()
 
-        return not response.hasFailed()
+            return not response.hasFailed()
 
     def reset(self) -> None:
         """
             Resets the internal state of the LogHandler
             Clears all pending logs
             Resets the upload worker thread
         """
```

### Comparing `coretex-1.0.2/src/coretex/networking/__init__.py` & `coretex-1.0.3/src/coretex/networking/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from .network_manager_base import NetworkManagerBase
+from .network_manager_base import NetworkManagerBase, FileData
 from .network_manager import networkManager
 from .network_object import NetworkObject, DEFAULT_PAGE_SIZE
 from .network_response import NetworkResponse, NetworkRequestError
 from .request_type import RequestType
 from .requests_manager import RequestFailedError
 from .chunk_upload_session import ChunkUploadSession, MAX_CHUNK_SIZE
```

### Comparing `coretex-1.0.2/src/coretex/networking/chunk_upload_session.py` & `coretex-1.0.3/src/coretex/networking/chunk_upload_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Union, Optional
+from typing import Union
 from pathlib import Path
 
 import logging
 
+from .network_manager_base import FileData
 from .network_manager import networkManager
 from .network_response import NetworkRequestError
 from .request_type import RequestType
-from ..utils import guessMimeType
 
 
 MAX_CHUNK_SIZE = 128 * 1024 * 1024  # 128 MiB
 
 
 def _loadChunk(filePath: Path, start: int, chunkSize: int) -> bytes:
     with filePath.open("rb") as file:
@@ -50,33 +50,26 @@
         chunkSize : int
             size of chunks into which the file will be split
             maximum value is 128 MiB, while the minimum value is 1
         filePath : Union[Path, str]
             path to the file which will be uploaded
         fileSize : int
             size of the file which will be uploaded
-        mimeType : str
-            mime type of the file - if None is passed, guess will
-            be performed, if guess fails Exception will be raised
     """
 
-    def __init__(self, chunkSize: int, filePath: Union[Path, str], mimeType: Optional[str] = None) -> None:
+    def __init__(self, chunkSize: int, filePath: Union[Path, str]) -> None:
         if chunkSize <= 0 or chunkSize > MAX_CHUNK_SIZE:
             raise ValueError(f">> [Coretex] Invalid \"chunkSize\" value \"{chunkSize}\". Value must be in range 0-{MAX_CHUNK_SIZE}")
 
         if isinstance(filePath, str):
             filePath = Path(filePath)
 
-        if mimeType is None:
-            mimeType = guessMimeType(str(filePath))
-
         self.chunkSize = chunkSize
         self.filePath = filePath
         self.fileSize = filePath.lstat().st_size
-        self.mimeType = mimeType
 
     def __start(self) -> str:
         parameters = {
             "size": self.fileSize
         }
 
         response = networkManager.genericJSONRequest("upload/start", RequestType.post, parameters)
@@ -88,17 +81,17 @@
         if not isinstance(uploadId, str):
             raise ValueError(f">> [Coretex] Invalid API response, invalid value \"{uploadId}\" for field \"id\"")
 
         return uploadId
 
     def __uploadChunk(self, uploadId: str, start: int, end: int) -> None:
         chunk = _loadChunk(self.filePath, start, self.chunkSize)
-        files = {
-            "file": (self.filePath.name, chunk, self.mimeType)
-        }
+        files = [
+            FileData.createFromBytes("file", chunk, self.filePath.name)
+        ]
 
         parameters = {
             "id": uploadId,
             "start": start,
             "end": end - 1  # API expects start/end to be inclusive
         }
```

### Comparing `coretex-1.0.2/src/coretex/networking/network_manager.py` & `coretex-1.0.3/src/coretex/networking/network_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/networking/network_manager_base.py` & `coretex-1.0.3/src/coretex/networking/network_manager_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+from typing import Optional, Any, Dict, List
 from pathlib import Path
-from typing import Optional, Any, Dict
 from abc import ABC, abstractmethod
 from importlib.metadata import version as getLibraryVersion
 
 import json
 import logging
 import os
 import platform
 
 from .requests_manager import RequestsManager
 from .request_type import RequestType
 from .network_response import HttpCode, NetworkResponse
+from .file_data import FileData
 
 
 class NetworkManagerBase(ABC):
 
     MAX_RETRY_COUNT = 3
 
     def __init__(self) -> None:
@@ -196,15 +197,16 @@
             endpoint : str
                 API endpoint
             destination : str
                 path to save file
             parameters : Optional[dict[str, Any]]
                 request parameters (not required)
             retryCount : int
-                number of function calls if request has failed
+                number of function calls if request has failed, used
+                for internal retry mechanism
 
             Returns
             -------
             NetworkResponse as response content to request
 
             Example
             -------
@@ -243,65 +245,123 @@
                 downloadedFile.write(response.raw.content)
 
         return response
 
     def genericUpload(
         self,
         endpoint: str,
-        files: Any,
+        files: List[FileData],
         parameters: Optional[Dict[str, Any]] = None,
         retryCount: int = 0
     ) -> NetworkResponse:
+
         """
-            Uploads files to Cortex.ai
+            Sends a multipart form data request to Coretex.ai
+            with files
 
             Parameters
             ----------
             endpoint : str
                 API endpoint
-            files : Any
-                files
-            parameters : Optional[dict[str, Any]]
-                request parameters (not required)
+            files : List[FileData]
+                List of "FileData" objects which describe how
+                should the files be uploaded to Coretex.ai
+            parameters : dict[str, Any]
+                request parameters - must be ordered to match
+                expected values on Coretex.ai
             retryCount : int
-                number of function calls if request has failed
+                number of function calls if request has failed, used
+                for internal retry mechanism
 
             Returns
             -------
             NetworkResponse -> NetworkResponse object containing the full response info
 
             Example
             -------
-            >>> from coretex import networkManager
+            >>> from coretex import networkManager, FileData
+            \b
+            >>> with open("path/to/file_2.ext", "rb") as file:
+                    fileBytes = file.read()
             \b
-            >>> localFilePath = "path/to/file/filename.ext"
-            >>> with open(localFilePath, "rb") as file:
-                    files = [
-                        ("file", ("filename.ext", file, "application/zip"))
-                    ]
+            >>> files = [
+                    FileData.createFromPath("file_1", "path/to/file_1.ext"),
+                    FileData.createFromBytes("file_2", fileBytes, fileName = "file_2")
+                ]
+            \b
+            >>> response = networkManager.genericFormData(
+                    endpoint = "dummy/form-data",
+                    files = files,
+                    parameters = {
+                        "first": "first_value",
+                        "second": "second_value"
+                    }
+                )
+            >>> if response.hasFailed():
+                    print("Failed to upload the provided files")
+        """
+
+        networkResponse = self._requestManager.upload(endpoint, self._requestHeader(), files, parameters)
+
+        if self.shouldRetry(retryCount, networkResponse):
+            return self.genericUpload(endpoint, files, parameters, retryCount + 1)
+
+        return networkResponse
+
+    def genericFormData(self, endpoint: str, parameters: Dict[str, Any], retryCount: int = 0) -> NetworkResponse:
+        """
+            Sends a form data request to Cortex.ai
+
+            Parameters
+            ----------
+            endpoint : str
+                API endpoint
+            parameters : dict[str, Any]
+                request parameters - must be ordered to match
+                expected values on Coretex.ai
+            retryCount : int
+                number of function calls if request has failed, used
+                for internal retry mechanism
+
+            Returns
+            -------
+            NetworkResponse -> NetworkResponse object containing the full response info
+
+            Example
+            -------
+            >>> from coretex import networkManager
             \b
-                    response = networkManager.genericUpload(
-                        endpoint = "dummy/upload",
-                        files = files,
-                    )
+            >>> response = networkManager.genericFormData(
+                    endpoint = "dummy/form-data",
+                    parameters = {
+                        "first": "first_value",
+                        "second": "second_value"
+                    }
+                )
             >>> if response.hasFailed():
-                    print("Failed to upload the file")
+                    print("Failed to execute form data request")
         """
 
         headers = self._requestHeader()
         del headers['Content-Type']
 
-        if parameters is None:
-            parameters = {}
+        # Map to correct form data parameter format
+        formDataParameters = {
+            key: (None, value)
+            for key, value in parameters.items()
+        }
 
-        networkResponse = self._requestManager.genericRequest(RequestType.post, endpoint, headers, parameters, files)
+        # RequestsManager.genericRequest files parameter can
+        # accept parameters that are not files, this way we can
+        # send form-data requests without actual files
+        networkResponse = self._requestManager.genericRequest(RequestType.post, endpoint, headers, files = formDataParameters)
 
         if self.shouldRetry(retryCount, networkResponse):
             print(">> [Coretex] Retry count: {0}".format(retryCount))
-            return self.genericUpload(endpoint, files, parameters, retryCount + 1)
+            return self.genericFormData(endpoint, parameters, retryCount + 1)
 
         return networkResponse
 
     def genericDelete(
         self,
         endpoint: str
     ) -> NetworkResponse:
@@ -348,15 +408,16 @@
             requestType : RequestType
                 request type
             parameters : Optional[dict[str, Any]]
                 request parameters (not required)
             headers : Optional[dict[str, str]]
                 headers (not required)
             retryCount : int
-                number of function calls if request has failed
+                number of function calls if request has failed, used
+                for internal retry mechanism
 
             Returns
             -------
             NetworkResponse -> NetworkResponse object containing the full response info
 
             Example
             -------
```

### Comparing `coretex-1.0.2/src/coretex/networking/network_object.py` & `coretex-1.0.3/src/coretex/networking/network_object.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/networking/network_response.py` & `coretex-1.0.3/src/coretex/networking/network_response.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/networking/request_type.py` & `coretex-1.0.3/src/coretex/networking/request_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/networking/requests_manager.py` & `coretex-1.0.3/src/coretex/networking/requests_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Final, Any, Optional, Dict
+from typing import Final, Any, Optional, Dict, List
+from contextlib import ExitStack
 
 import logging
 
 from requests import Session
 
 from .network_response import NetworkResponse
 from .request_type import RequestType
+from .file_data import FileData
 
 
 class RequestFailedError(RuntimeError):
 
     def __init__(self) -> None:
         super().__init__(">> [Coretex] Failed to execute request after retrying")
 
@@ -73,15 +75,16 @@
             headers : Optional[Dict[str, str]]
                 headers (not required)
             data : Any
                 (not required)
             files : Any
                 (not required)
             retryCount : int
-                number of function calls if request has failed
+                number of function calls if request has failed, used
+                for internal retry mechanism
 
             Returns
             -------
             NetworkResponse -> NetworkResponse object as response content to request
         """
 
         logging.getLogger("coretexpylib").debug(f"Sending request {requestType}, {endpoint}, HEADERS: {headers}, DATA: {data}")
@@ -93,17 +96,17 @@
                 headers = headers,
                 data = data,
                 files = files
                 # timeout = (self.__connectionTimeout, self.__readTimeout)
             )
 
             return NetworkResponse(requestsResponse, endpoint)
-        except Exception as ex:
+        except:
             if retryCount < RequestsManager.MAX_RETRY_COUNT:
-                RequestsManager.__logRetry(requestType, endpoint, retryCount, ex)
+                RequestsManager.__logRetry(requestType, endpoint, retryCount)
                 return self.genericRequest(requestType, endpoint, headers, data, files, retryCount = retryCount + 1)
 
             raise RequestFailedError
 
     def get(
         self,
         endpoint: str,
@@ -122,15 +125,16 @@
             headers : Optional[Dict[str, str]]
                 headers (not required)
             data : Any
                 (not required)
             jsonObject : Any
                 (not required)
             retryCount : int
-                number of function calls if request has failed
+                number of function calls if request has failed, used
+                for internal retry mechanism
 
             Returns
             -------
             NetworkResponse -> NetworkResponse object as response content to request
         """
 
         logging.getLogger("coretexpylib").debug(f"Sending request {endpoint}, HEADERS: {headers}, DATA: {data}, JSON_OBJECT: {jsonObject}")
@@ -141,17 +145,17 @@
                 headers = headers,
                 data = data,
                 json = jsonObject
                 # timeout = (self.__connectionTimeout, self.__readTimeout)
             )
 
             return NetworkResponse(requestsResponse, endpoint)
-        except Exception as ex:
+        except:
             if retryCount < RequestsManager.MAX_RETRY_COUNT:
-                RequestsManager.__logRetry(RequestType.get, endpoint, retryCount, ex)
+                RequestsManager.__logRetry(RequestType.get, endpoint, retryCount)
                 return self.get(endpoint, headers, data, jsonObject, retryCount = retryCount + 1)
 
             raise RequestFailedError
 
     def post(
         self,
         endpoint: str,
@@ -170,15 +174,16 @@
             headers : Optional[Dict[str, str]]
                 headers (not required)
             data : Any
                 (not required)
             jsonObject : Any
                 (not required)
             retryCount : int
-                number of function calls if request has failed
+                number of function calls if request has failed, used
+                for internal retry mechanism
 
             Returns
             -------
             NetworkResponse -> NetworkResponse object as response content to request
         """
 
         logging.getLogger("coretexpylib").debug(f"Sending request {endpoint}, HEADERS: {headers}, DATA: {data}, JSON_OBJECT: {jsonObject}")
@@ -189,29 +194,87 @@
                 headers = headers,
                 data = data,
                 json = jsonObject
                 # timeout = (self.__connectionTimeout, self.__readTimeout)
             )
 
             return NetworkResponse(requestsResponse, endpoint)
-        except Exception as ex:
+        except:
             if retryCount < RequestsManager.MAX_RETRY_COUNT:
-                RequestsManager.__logRetry(RequestType.post, endpoint, retryCount, ex)
+                RequestsManager.__logRetry(RequestType.post, endpoint, retryCount)
                 return self.post(endpoint, headers, data, jsonObject, retryCount = retryCount + 1)
 
             raise RequestFailedError
 
+    def upload(
+        self,
+        endpoint: str,
+        headers: Dict[str, str],
+        files: List[FileData],
+        parameters: Optional[Dict[str, Any]] = None,
+        retryCount: int = 0
+    ) -> NetworkResponse:
+        """
+            Sends generic HTTP request
+
+            Parameters
+            ----------
+            endpoint : str
+                API endpoint
+            headers : Dict[str, str]
+                request headers
+            files : List[FileData]
+                files which will be uploaded and their metadata
+            parameters : Optional[Dict[str, Any]]
+                request parameters (not required)
+            retryCount : int
+                number of function calls if request has failed, used
+                for internal retry mechanism
+
+            Returns
+            -------
+            NetworkResponse -> NetworkResponse object as response content to request
+        """
+
+        if "Content-Type" in headers:
+            del headers['Content-Type']
+
+        logging.getLogger("coretexpylib").debug(f"Sending upload request {endpoint}, HEADERS: {headers}, FILES: {files}, PARAMETERS: {parameters}")
+
+        try:
+            # ExitStack lets us combine multiple contexts when opening files
+            # and if anything failes then the ExitStack will properly close
+            # all open file handles
+            with ExitStack() as stack:
+                requestsResponse = self.__session.request(
+                    method = RequestType.post.value,
+                    url = self.__url(endpoint),
+                    headers = headers,
+                    data = parameters,
+                    files = [file.prepareForUpload(stack) for file in files]
+                    # timeout = (self.__connectionTimeout, self.__readTimeout)
+                )
+
+            return NetworkResponse(requestsResponse, endpoint)
+        except:
+            if retryCount < RequestsManager.MAX_RETRY_COUNT:
+                RequestsManager.__logRetry(RequestType.post, endpoint, retryCount)
+                return self.upload(endpoint, headers, files, parameters, retryCount + 1)
+
+            raise RequestFailedError
+
     def setAuth(self, username: str, password: str) -> None:
         self.__session.auth = (username, password)
 
     @staticmethod
-    def __logRetry(requestType: RequestType, endpoint: str, retryCount: int, exception: Exception) -> None:
+    def __logRetry(requestType: RequestType, endpoint: str, retryCount: int) -> None:
         """
             Logs the information about request retry
         """
 
         logging.getLogger("coretexpylib").debug(
-            f">> [Coretex] Retry {retryCount + 1} for ({requestType.name} -> {endpoint}), exception: {exception.__class__.__name__}"
+            f">> [Coretex] Retry {retryCount + 1} for ({requestType.name} -> {endpoint})",
+            exc_info = True
         )
 
     def reset(self) -> None:
         self.__session.auth = None
```

### Comparing `coretex-1.0.2/src/coretex/networking/user_data.py` & `coretex-1.0.3/src/coretex/networking/user_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/nlp/__init__.py` & `coretex-1.0.3/src/coretex/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/nlp/text.py` & `coretex-1.0.3/src/coretex/nlp/text.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/nlp/token.py` & `coretex-1.0.3/src/coretex/nlp/token.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/nlp/transcriber.py` & `coretex-1.0.3/src/coretex/nlp/transcriber.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/nlp/transcription.py` & `coretex-1.0.3/src/coretex/nlp/transcription.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/nlp/utils.py` & `coretex-1.0.3/src/coretex/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/project/__init__.py` & `coretex-1.0.3/src/coretex/project/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/project/base.py` & `coretex-1.0.3/src/coretex/project/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
```

### Comparing `coretex-1.0.2/src/coretex/project/calculate_metrics.py` & `coretex-1.0.3/src/coretex/project/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/project/heartbeat.py` & `coretex-1.0.3/src/coretex/project/heartbeat.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/project/local.py` & `coretex-1.0.3/src/coretex/project/local.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/project/remote.py` & `coretex-1.0.3/src/coretex/project/remote.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/qiime2/__init__.py` & `coretex-1.0.3/src/coretex/qiime2/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/qiime2/utils.py` & `coretex-1.0.3/src/coretex/qiime2/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Optional, List
+from typing import List
 from pathlib import Path
 
 import logging
 import gzip
 
 from ..coretex import Experiment, CustomSample, CustomDataset
 
 
 def createSample(name: str, datasetId: int, path: Path, experiment: Experiment, stepName: str, retryCount: int = 0) -> CustomSample:
-    mimeType: Optional[str] = None
-    if path.suffix in [".qza", ".qzv"]:
-        mimeType = "application/zip"
-
-    sample = CustomSample.createCustomSample(name, datasetId, str(path), mimeType)
+    sample = CustomSample.createCustomSample(name, datasetId, str(path))
     if sample is None:
         if retryCount < 3:
             logging.info(f">> [Workspace] Retry count: {retryCount}")
             return createSample(name, datasetId, path, experiment, stepName, retryCount + 1)
 
         raise ValueError(">> [Workspace] Failed to create sample")
```

### Comparing `coretex-1.0.2/src/coretex/threading/__init__.py` & `coretex-1.0.3/src/coretex/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/threading/threaded_data_processor.py` & `coretex-1.0.3/src/coretex/threading/threaded_data_processor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/utils/__init__.py` & `coretex-1.0.3/src/coretex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/utils/console_progress_bar.py` & `coretex-1.0.3/src/coretex/utils/console_progress_bar.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/utils/date.py` & `coretex-1.0.3/src/coretex/utils/date.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex/utils/file.py` & `coretex-1.0.3/src/coretex/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Generator, Optional
+from typing import Generator, Optional, Union
 from pathlib import Path
 from zipfile import ZipFile
 
 import mimetypes
 import zipfile
 import tarfile
 import gzip
@@ -32,22 +32,22 @@
     """
         Exception raised if file extension is unkown or invalid
     """
 
     pass
 
 
-def guessMimeType(filePath: str) -> str:
+def guessMimeType(filePath: Union[Path, str]) -> str:
     """
         Tries to guess mime type of the file
 
         Parameters
         ----------
-        filePath : str
-            file to be guessed
+        filePath : Union[Path, str]
+            file whose mime type will be guessed
 
         Returns
         -------
         str -> guessed mime type
 
         Raises
         ------
@@ -145,16 +145,16 @@
 
         Returns
         -------
         Generator[Path, None, None] -> generator which contains all
         subdirectories and subfiles
     """
 
-    for p in Path(path).iterdir(): 
-        if p.is_dir(): 
+    for p in Path(path).iterdir():
+        if p.is_dir():
             yield from walk(p)
             continue
 
         yield p.resolve()
 
 
 def recursiveUnzip(entryPoint: Path, destination: Optional[Path] = None, remove: bool = False) -> None:
```

### Comparing `coretex-1.0.2/src/coretex/utils/number.py` & `coretex-1.0.3/src/coretex/utils/number.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.2/src/coretex.egg-info/PKG-INFO` & `coretex-1.0.3/src/coretex.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
-Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>, Igor Perić <igor@coretex.ai>
+Maintainer-email: Igor Perić <igor@coretex.ai>, Duško Mirković <dmirkovic@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Linter code check](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml/badge.svg?branch=develop)](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml)
```

### Comparing `coretex-1.0.2/src/coretex.egg-info/SOURCES.txt` & `coretex-1.0.3/src/coretex.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 src/coretex/folder_management/folder_manager.py
 src/coretex/logging/__init__.py
 src/coretex/logging/log.py
 src/coretex/logging/log_severity.py
 src/coretex/logging/logger.py
 src/coretex/networking/__init__.py
 src/coretex/networking/chunk_upload_session.py
+src/coretex/networking/file_data.py
 src/coretex/networking/network_manager.py
 src/coretex/networking/network_manager_base.py
 src/coretex/networking/network_object.py
 src/coretex/networking/network_response.py
 src/coretex/networking/request_type.py
 src/coretex/networking/requests_manager.py
 src/coretex/networking/user_data.py
```

