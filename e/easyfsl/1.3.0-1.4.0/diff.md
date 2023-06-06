# Comparing `tmp/easyfsl-1.3.0.tar.gz` & `tmp/easyfsl-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfsl-1.3.0.tar", last modified: Tue May 16 09:13:30 2023, max compression
+gzip compressed data, was "easyfsl-1.4.0.tar", last modified: Tue Jun  6 08:42:34 2023, max compression
```

## Comparing `easyfsl-1.3.0.tar` & `easyfsl-1.4.0.tar`

### file list

```diff
@@ -1,70 +1,78 @@
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.518336 easyfsl-1.3.0/
--rw-r--r--   0 etienne    (501) staff       (20)     1063 2022-09-05 12:06:43.000000 easyfsl-1.3.0/LICENSE
--rw-r--r--   0 etienne    (501) staff       (20)    10774 2023-05-16 09:13:30.518155 easyfsl-1.3.0/PKG-INFO
--rw-r--r--   0 etienne    (501) staff       (20)     9991 2023-05-16 08:17:50.000000 easyfsl-1.3.0/README.md
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.509929 easyfsl-1.3.0/easyfsl/
--rw-r--r--   0 etienne    (501) staff       (20)      169 2023-05-16 09:04:23.000000 easyfsl-1.3.0/easyfsl/__init__.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.512839 easyfsl-1.3.0/easyfsl/datasets/
--rw-r--r--   0 etienne    (501) staff       (20)      367 2023-05-16 08:17:50.000000 easyfsl-1.3.0/easyfsl/datasets/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)      735 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/cub.py
--rw-r--r--   0 etienne    (501) staff       (20)     2820 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/danish_fungi.py
--rw-r--r--   0 etienne    (501) staff       (20)     2943 2023-03-30 08:04:18.000000 easyfsl-1.3.0/easyfsl/datasets/default_configs.py
--rw-r--r--   0 etienne    (501) staff       (20)     6023 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/datasets/easy_set.py
--rw-r--r--   0 etienne    (501) staff       (20)     3998 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/datasets/features_dataset.py
--rw-r--r--   0 etienne    (501) staff       (20)     1137 2023-03-29 10:01:49.000000 easyfsl-1.3.0/easyfsl/datasets/few_shot_dataset.py
--rw-r--r--   0 etienne    (501) staff       (20)     6105 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/mini_imagenet.py
--rw-r--r--   0 etienne    (501) staff       (20)     2722 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/support_set_folder.py
--rw-r--r--   0 etienne    (501) staff       (20)      861 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/tiered_imagenet.py
--rw-r--r--   0 etienne    (501) staff       (20)     2555 2023-05-16 08:17:50.000000 easyfsl-1.3.0/easyfsl/datasets/wrap_few_shot_dataset.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.514428 easyfsl-1.3.0/easyfsl/methods/
--rw-r--r--   0 etienne    (501) staff       (20)      343 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/methods/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     2964 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/bd_cspn.py
--rw-r--r--   0 etienne    (501) staff       (20)     4779 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/few_shot_classifier.py
--rw-r--r--   0 etienne    (501) staff       (20)     2615 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/finetune.py
--rw-r--r--   0 etienne    (501) staff       (20)     7885 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/matching_networks.py
--rw-r--r--   0 etienne    (501) staff       (20)     2079 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/prototypical_networks.py
--rw-r--r--   0 etienne    (501) staff       (20)     5732 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/relation_networks.py
--rw-r--r--   0 etienne    (501) staff       (20)     4416 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/tim.py
--rw-r--r--   0 etienne    (501) staff       (20)     2984 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/transductive_finetuning.py
--rw-r--r--   0 etienne    (501) staff       (20)     1146 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/methods/utils.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.514890 easyfsl-1.3.0/easyfsl/modules/
--rw-r--r--   0 etienne    (501) staff       (20)       76 2023-03-30 08:04:18.000000 easyfsl-1.3.0/easyfsl/modules/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     3379 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/modules/predesigned_modules.py
--rw-r--r--   0 etienne    (501) staff       (20)     5782 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/modules/resnet.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.515213 easyfsl-1.3.0/easyfsl/samplers/
--rw-r--r--   0 etienne    (501) staff       (20)       38 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/samplers/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     7874 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/samplers/task_sampler.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.515402 easyfsl-1.3.0/easyfsl/tests/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/__init__.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.516159 easyfsl-1.3.0/easyfsl/tests/datasets/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/datasets/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     4584 2023-03-30 08:04:18.000000 easyfsl-1.3.0/easyfsl/tests/datasets/easy_set_test.py
--rw-r--r--   0 etienne    (501) staff       (20)    13495 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/tests/datasets/features_dataset_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     1433 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/datasets/support_set_folder_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     3458 2023-05-16 08:17:50.000000 easyfsl-1.3.0/easyfsl/tests/datasets/wrap_few_shot_dataset_test.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.517095 easyfsl-1.3.0/easyfsl/tests/methods/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/methods/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     1374 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/methods/conftest.py
--rw-r--r--   0 etienne    (501) staff       (20)      587 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/methods/few_shot_classifier_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     6957 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/tests/methods/finetuning_methods_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     2875 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/methods/matching_networks_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     3262 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/methods/prototypical_networks_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     3640 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/methods/relation_networks_test.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.517668 easyfsl-1.3.0/easyfsl/tests/modules/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/modules/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)      774 2023-03-30 08:04:18.000000 easyfsl-1.3.0/easyfsl/tests/modules/predesigned_modules_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     1243 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/modules/resnet_test.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.517977 easyfsl-1.3.0/easyfsl/tests/samplers/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/samplers/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)    12547 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/tests/samplers/task_sampler_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     7564 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/utils_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     5105 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/utils.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.510589 easyfsl-1.3.0/easyfsl.egg-info/
--rw-r--r--   0 etienne    (501) staff       (20)    10774 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/PKG-INFO
--rw-r--r--   0 etienne    (501) staff       (20)     1886 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/SOURCES.txt
--rw-r--r--   0 etienne    (501) staff       (20)        1 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/dependency_links.txt
--rw-r--r--   0 etienne    (501) staff       (20)       76 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/requires.txt
--rw-r--r--   0 etienne    (501) staff       (20)        8 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/top_level.txt
--rw-r--r--   0 etienne    (501) staff       (20)      799 2023-05-16 08:42:43.000000 easyfsl-1.3.0/pyproject.toml
--rw-r--r--   0 etienne    (501) staff       (20)       38 2023-05-16 09:13:30.518368 easyfsl-1.3.0/setup.cfg
--rw-r--r--   0 etienne    (501) staff       (20)     1172 2023-05-16 09:04:23.000000 easyfsl-1.3.0/setup.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.897517 easyfsl-1.4.0/
+-rw-r--r--   0 etienne    (501) staff       (20)     1063 2022-09-05 12:06:43.000000 easyfsl-1.4.0/LICENSE
+-rw-r--r--   0 etienne    (501) staff       (20)    16048 2023-06-06 08:42:34.897322 easyfsl-1.4.0/PKG-INFO
+-rw-r--r--   0 etienne    (501) staff       (20)    15265 2023-06-05 14:28:04.000000 easyfsl-1.4.0/README.md
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.887650 easyfsl-1.4.0/easyfsl/
+-rw-r--r--   0 etienne    (501) staff       (20)      169 2023-06-06 08:34:29.000000 easyfsl-1.4.0/easyfsl/__init__.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.890670 easyfsl-1.4.0/easyfsl/datasets/
+-rw-r--r--   0 etienne    (501) staff       (20)      367 2023-05-16 08:17:50.000000 easyfsl-1.4.0/easyfsl/datasets/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)      749 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/datasets/cub.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3349 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/datasets/danish_fungi.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2943 2023-03-30 08:04:18.000000 easyfsl-1.4.0/easyfsl/datasets/default_configs.py
+-rw-r--r--   0 etienne    (501) staff       (20)     6023 2023-05-12 13:53:16.000000 easyfsl-1.4.0/easyfsl/datasets/easy_set.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3998 2023-05-12 13:53:16.000000 easyfsl-1.4.0/easyfsl/datasets/features_dataset.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1137 2023-03-29 10:01:49.000000 easyfsl-1.4.0/easyfsl/datasets/few_shot_dataset.py
+-rw-r--r--   0 etienne    (501) staff       (20)     6105 2023-04-26 14:40:51.000000 easyfsl-1.4.0/easyfsl/datasets/mini_imagenet.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2722 2023-04-26 14:40:51.000000 easyfsl-1.4.0/easyfsl/datasets/support_set_folder.py
+-rw-r--r--   0 etienne    (501) staff       (20)      830 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/datasets/tiered_imagenet.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2555 2023-05-16 08:17:50.000000 easyfsl-1.4.0/easyfsl/datasets/wrap_few_shot_dataset.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.893092 easyfsl-1.4.0/easyfsl/methods/
+-rw-r--r--   0 etienne    (501) staff       (20)      470 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2964 2023-05-31 09:06:31.000000 easyfsl-1.4.0/easyfsl/methods/bd_cspn.py
+-rw-r--r--   0 etienne    (501) staff       (20)     4991 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/feat.py
+-rw-r--r--   0 etienne    (501) staff       (20)     4873 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/few_shot_classifier.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2952 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/finetune.py
+-rw-r--r--   0 etienne    (501) staff       (20)     5060 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/laplacian_shot.py
+-rw-r--r--   0 etienne    (501) staff       (20)     7885 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/methods/matching_networks.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1994 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/prototypical_networks.py
+-rw-r--r--   0 etienne    (501) staff       (20)     4704 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/pt_map.py
+-rw-r--r--   0 etienne    (501) staff       (20)     5732 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/methods/relation_networks.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1052 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/simple_shot.py
+-rw-r--r--   0 etienne    (501) staff       (20)     4821 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/tim.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3306 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/transductive_finetuning.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2823 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/methods/utils.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.893968 easyfsl-1.4.0/easyfsl/modules/
+-rw-r--r--   0 etienne    (501) staff       (20)      167 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/modules/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3047 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/modules/attention_modules.py
+-rw-r--r--   0 etienne    (501) staff       (20)      649 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/modules/build_from_checkpoint.py
+-rw-r--r--   0 etienne    (501) staff       (20)     5168 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/modules/feat_resnet12.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3379 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/modules/predesigned_modules.py
+-rw-r--r--   0 etienne    (501) staff       (20)     5782 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/modules/resnet.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.894417 easyfsl-1.4.0/easyfsl/samplers/
+-rw-r--r--   0 etienne    (501) staff       (20)       38 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/samplers/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     7874 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/samplers/task_sampler.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.894625 easyfsl-1.4.0/easyfsl/tests/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/tests/__init__.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.895434 easyfsl-1.4.0/easyfsl/tests/datasets/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/tests/datasets/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     4584 2023-03-30 08:04:18.000000 easyfsl-1.4.0/easyfsl/tests/datasets/easy_set_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)    13495 2023-05-12 13:53:16.000000 easyfsl-1.4.0/easyfsl/tests/datasets/features_dataset_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1433 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/tests/datasets/support_set_folder_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3458 2023-05-16 08:17:50.000000 easyfsl-1.4.0/easyfsl/tests/datasets/wrap_few_shot_dataset_test.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.896487 easyfsl-1.4.0/easyfsl/tests/methods/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/tests/methods/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1374 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/tests/methods/conftest.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3070 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/tests/methods/feat_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)      587 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/tests/methods/few_shot_classifier_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     6975 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/tests/methods/finetuning_methods_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2875 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/tests/methods/matching_networks_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3262 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/tests/methods/prototypical_networks_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3640 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/tests/methods/relation_networks_test.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.896847 easyfsl-1.4.0/easyfsl/tests/modules/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/tests/modules/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)      774 2023-03-30 08:04:18.000000 easyfsl-1.4.0/easyfsl/tests/modules/predesigned_modules_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1243 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/tests/modules/resnet_test.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.897131 easyfsl-1.4.0/easyfsl/tests/samplers/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.4.0/easyfsl/tests/samplers/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)    12547 2023-04-26 14:40:51.000000 easyfsl-1.4.0/easyfsl/tests/samplers/task_sampler_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     7564 2023-05-16 08:54:13.000000 easyfsl-1.4.0/easyfsl/tests/utils_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     5236 2023-06-05 14:28:04.000000 easyfsl-1.4.0/easyfsl/utils.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-06-06 08:42:34.888439 easyfsl-1.4.0/easyfsl.egg-info/
+-rw-r--r--   0 etienne    (501) staff       (20)    16048 2023-06-06 08:42:34.000000 easyfsl-1.4.0/easyfsl.egg-info/PKG-INFO
+-rw-r--r--   0 etienne    (501) staff       (20)     2147 2023-06-06 08:42:34.000000 easyfsl-1.4.0/easyfsl.egg-info/SOURCES.txt
+-rw-r--r--   0 etienne    (501) staff       (20)        1 2023-06-06 08:42:34.000000 easyfsl-1.4.0/easyfsl.egg-info/dependency_links.txt
+-rw-r--r--   0 etienne    (501) staff       (20)       76 2023-06-06 08:42:34.000000 easyfsl-1.4.0/easyfsl.egg-info/requires.txt
+-rw-r--r--   0 etienne    (501) staff       (20)        8 2023-06-06 08:42:34.000000 easyfsl-1.4.0/easyfsl.egg-info/top_level.txt
+-rw-r--r--   0 etienne    (501) staff       (20)      799 2023-05-16 08:42:43.000000 easyfsl-1.4.0/pyproject.toml
+-rw-r--r--   0 etienne    (501) staff       (20)       38 2023-06-06 08:42:34.897551 easyfsl-1.4.0/setup.cfg
+-rw-r--r--   0 etienne    (501) staff       (20)     1172 2023-06-06 08:34:29.000000 easyfsl-1.4.0/setup.py
```

### Comparing `easyfsl-1.3.0/LICENSE` & `easyfsl-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/PKG-INFO` & `easyfsl-1.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: easyfsl
-Version: 1.3.0
-Summary: Ready-to-use PyTorch code to boost your way into few-shot image classification
-Home-page: https://github.com/sicara/easy-few-shot-learning
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Easy Few-Shot Learning
 ![Python Versions](https://img.shields.io/pypi/pyversions/easyfsl?logo=python&logoColor=white&style=for-the-badge)
 ![License: MIT](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)
 ![CircleCI](https://img.shields.io/circleci/build/github/sicara/easy-few-shot-learning?logo=circleci&style=for-the-badge)
 ![PyPi Downloads](https://img.shields.io/pypi/dm/easyfsl?logo=pypi&logoColor=white&style=for-the-badge)
 ![Last Release](https://img.shields.io/github/release-date/sicara/easy-few-shot-learning?label=Last%20Release&logo=pypi&logoColor=white&style=for-the-badge)
 ![Github Issues](https://img.shields.io/github/issues-closed/sicara/easy-few-shot-learning?color=green&logo=github&style=for-the-badge)
@@ -46,39 +26,50 @@
 | [Example of classical training](notebooks/classical_training.ipynb)                            | Use it as a starting point if you want to design a script for classical training using EasyFSL.                                                                                              | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/classical_training.ipynb)                |
 | [Test with pre-extracted embeddings](notebooks/inference_with_extracted_embeddings.ipynb)      | Most few-shot methods use a frozen backbone at test-time. With EasyFSL, you can extract all embeddings for your dataset once and for all, and then perform inference directly on embeddings. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/inference_with_extracted_embeddings.ipynb) |
 
 ### Code that you can use and understand
 
 **State-Of-The-Art Few-Shot Learning methods:**
 
-- [FewShotClassifier](easyfsl/methods/few_shot_classifier.py): an abstract class with methods that can be used for 
-  any few-shot classification algorithm
+With 11 built-in methods, EasyFSL is the most comprehensive open-source Few-Shot Learning library!
+
 - [Prototypical Networks](easyfsl/methods/prototypical_networks.py)
+- [SimpleShot](easyfsl/methods/simple_shot.py)
 - [Matching Networks](easyfsl/methods/matching_networks.py)
 - [Relation Networks](easyfsl/methods/relation_networks.py)
+- [FEAT](easyfsl/methods/feat.py)
 - [Fine-Tune](easyfsl/methods/finetune.py)
 - [BD-CSPN](easyfsl/methods/bd_cspn.py)
-- [Transductive Fine-Tuning](easyfsl/methods/transductive_finetuning.py)
+- [LaplacianShot](easyfsl/methods/laplacian_shot.py)
 - [Transductive Information Maximization](easyfsl/methods/tim.py)
+- [PT-MAP](easyfsl/methods/pt_map.py)
+- [Transductive Fine-Tuning](easyfsl/methods/transductive_finetuning.py)
+
+We also provide a [FewShotClassifier](easyfsl/methods/few_shot_classifier.py) class to quickstart your implementation 
+of any few-shot classification algorithm, as well as [commonly used architectures](easyfsl/modules).
 
-To reproduce their results, you can use the [standard network architectures](easyfsl/modules/predesigned_modules.py) 
-used in Few-Shot Learning research. They're also a feature of EasyFSL!
+See the benchmarks section below for more details on the methods.
 
 **Tools for data loading:**
 
 Data loading in FSL is a bit different from standard classification because we sample batches of
 instances in the shape of few-shot classification tasks. No sweat! In EasyFSL you have:
 
 - [TaskSampler](easyfsl/samplers/task_sampler.py): an extension of the standard PyTorch Sampler object, to sample batches in the shape of few-shot classification tasks
 - [FewShotDataset](easyfsl/datasets/few_shot_dataset.py): an abstract class to standardize the interface of any dataset you'd like to use
 - [EasySet](easyfsl/datasets/easy_set.py): a ready-to-use FewShotDataset object to handle datasets of images with a class-wise directory split
 - [WrapFewShotDataset](easyfsl/datasets/wrap_few_shot_dataset.py): a wrapper to transform any dataset into a FewShotDataset object
 - [FeaturesDataset](easyfsl/datasets/features_dataset.py): a dataset to handle pre-extracted features
 - [SupportSetFolder](easyfsl/datasets/support_set_folder.py): a dataset to handle support sets stored in a directory
 
+**Scripts to reproduce our benchmarks:**
+
+- `scripts/predict_embeddings.py` to extract all embeddings from a dataset with a given pre-trained backbone
+- `scripts/benchmark_methods.py` to evaluate a method on a test dataset using pre-extracted embeddings.
+
 **And also:** [some utilities](easyfsl/utils.py) that I felt I often used in my research, so I'm sharing with you.
 
 ### Datasets to test your model
 
 There are enough datasets used in Few-Shot Learning for anyone to get lost in them. They're all here, 
 explicited, downloadable and easy-to-use, in EasyFSL. 
 
@@ -166,9 +157,59 @@
 ## Contribute
 This project is very open to contributions! You can help in various ways:
 - raise issues
 - resolve issues already opened
 - tackle new features from the roadmap
 - fix typos, improve code quality
 
+## Benchmarks
+
+We used EasyFSL to benchmark a dozen methods. 
+Inference times are computed over 1000 tasks using pre-extracted features. They are only indicative.
+Note that the inference time for fine-tuning methods highly depends on the number of fine-tuning steps.
+
+All methods hyper-parameters are defined in [this JSON file](scripts/backbones_configs.json). 
+They were selected on miniImageNet validation set. 
+The procedure can be reproduced from [this other project](https://github.com/ebennequin/few-shot-open-set).
+We decided to use miniImageNet's hyperparameters for all benchmarks in order to highlight the adaptability of
+the different methods.
+
+### miniImageNet & tieredImageNet
+
+All methods use the same backbone: [a custom ResNet12](easyfsl/modules/feat_resnet12.py) using the trained parameters
+provided by the authors from [FEAT](https://github.com/Sha-Lab/FEAT) 
+(download: [miniImageNet](https://drive.google.com/file/d/1ixqw1l9XVxl3lh1m5VXkctw6JssahGbQ/view),
+[tieredImageNet](https://drive.google.com/file/d/1M93jdOjAn8IihICPKJg8Mb4B-eYDSZfE/view)).
+
+| Method                                                                    | Ind / Trans  | *mini*Imagenet<br/>1-shot | *mini*Imagenet<br/>5-shot | *tiered*Imagenet<br/>1-shot | *tiered*Imagenet<br/>5-shot | Time    |
+|---------------------------------------------------------------------------|--------------|---------------------------|---------------------------|-----------------------------|-----------------------------|---------|
+| **[ProtoNet](easyfsl/methods/prototypical_networks.py)**                  | Inductive    | 61.5                      | 79.3                      | 56.4                        | 76.5                        | 10s     |
+| **[SimpleShot](easyfsl/methods/simple_shot.py)**                          | Inductive    | 65.5                      | 80.3                      | 60.2                        | 77.3                        | 9s      |
+| **[MatchingNet](easyfsl/methods/matching_networks.py)**                   | Inductive    | -                         | -                         | -                           | -                           | -       |
+| **[RelationNet](easyfsl/methods/relation_networks.py)**                   | Inductive    | -                         | -                         | -                           | -                           | -       |
+| **[Finetune](easyfsl/methods/finetune.py)**                               | Inductive    | 63.4                      | 80.38                     | 60.1                        | 77.4                        | 3mn03s  |
+| **[FEAT](easyfsl/methods/feat.py)**                                       | Inductive    | 64.7                      | 80.13                     | 61.3                        | 76.2                        | 3s      |
+| **[BD-CSPN](easyfsl/methods/bd_cspn.py)**                                 | Transductive | 71.7                      | 82.17                     | 66.1                        | 79.1                        | 10s     |
+| **[LaplacianShot](easyfsl/methods/laplacian_shot.py)**                    | Transductive | 69.6                      | 81.9                      | 66.0                        | 78.9                        | 12s     |
+| **[PT-MAP](easyfsl/methods/pt_map.py)**                                   | Transductive | -                         | -                         | -                           | -                           | 22mn50s |
+| **[TIM](easyfsl/methods/tim.py)**                                         | Transductive | 64.0                      | 80.4                      | 60.4                        | 77.4                        | 2mn48s  |
+| **[Transductive Finetuning](easyfsl/methods/transductive_finetuning.py)** | Transductive | -                         | -                         | -                           | -                           | -       |
+
+To reproduce:
+
+1. Download the [*mini*ImageNet](https://drive.google.com/file/d/1ixqw1l9XVxl3lh1m5VXkctw6JssahGbQ/view) 
+   and [tieredImageNet](https://drive.google.com/file/d/1M93jdOjAn8IihICPKJg8Mb4B-eYDSZfE/view) weights for ResNet12 
+   and save them under `data/models/feat_resnet12_mini_imagenet.pth` (resp. `tiered`).
+2. Extract all embeddings from the test sets of all datasets with `make extract-all-features-with-resnet12`.
+3. Run the evaluation script with `make benchmark-mini-imagenet`.
+
+
+### Next steps (01/06/2023): 
+
+1. Complete benchmark with Matching and Relation Nets, PT-MAP, Transductive Finetuning (est. July 23)
+2. Add explicit hyperparameter selection (est. July 23)
+3. Add feature normalization as it's been proven to have a huge impact on the results (est. July 23)
+4. Add cross-domain benchmarks (CUB, Fungi) and using other backbones (est. September 23)
+
+
```

### Comparing `easyfsl-1.3.0/easyfsl/datasets/cub.py` & `easyfsl-1.4.0/easyfsl/datasets/cub.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from pathlib import Path
 
 from .easy_set import EasySet
 
 CUB_SPECS_DIR = Path("data/CUB")
 
 
-def CUB(split: str, **kwargs) -> EasySet:  # pylint: disable=invalid-name
-    """
-    Build the CUB dataset for the specific split.
-    Args:
-        split: one of the available split (typically train, val, test).
-
-    Returns:
-        the constructed dataset using EasySet
-
-    Raises:
-        ValueError: if the specified split cannot be associated with a JSON spec file
-            from CUB's specs directory
-    """
-    specs_file = CUB_SPECS_DIR / f"{split}.json"
-    if specs_file.is_file():
-        return EasySet(specs_file=specs_file, **kwargs)
-
-    raise ValueError(f"Could not find specs file {specs_file.name} in {CUB_SPECS_DIR}")
+class CUB(EasySet):
+    def __init__(self, split: str, **kwargs):
+        """
+        Build the CUB dataset for the specific split.
+        Args:
+            split: one of the available split (typically train, val, test).
+        Raises:
+            ValueError: if the specified split cannot be associated with a JSON spec file
+                from CUB's specs directory
+        """
+        specs_file = CUB_SPECS_DIR / f"{split}.json"
+        if not specs_file.is_file():
+            raise ValueError(
+                f"Could not find specs file {specs_file.name} in {CUB_SPECS_DIR}"
+            )
+        super().__init__(specs_file=specs_file, **kwargs)
```

### Comparing `easyfsl-1.3.0/easyfsl/datasets/danish_fungi.py` & `easyfsl-1.4.0/easyfsl/datasets/danish_fungi.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,59 +16,68 @@
     def __init__(
         self,
         root: Union[Path, str],
         specs_file: Union[Path, str] = WHOLE_DANISH_FUNGI_SPECS_FILE,
         image_size: int = 84,
         transform: Optional[Callable] = None,
         training: bool = False,
+        image_file_extension: str = ".JPG",
     ):
         """
         Args:
             root: directory where all the images are
             specs_file: path to the CSV file
             image_size: images returned by the dataset will be square images of the given size
             transform: torchvision transforms to be applied to images. If none is provided,
                 we use some standard transformations including ImageNet normalization.
                 These default transformations depend on the "training" argument.
             training: preprocessing is slightly different for a training set, adding a random
                 cropping and a random horizontal flip. Only used if transforms = None.
+            image_file_extension: the metadata csv file and the complete dataset user ".JPG" image file extension,
+                but the version of the dataset with 300px images uses ".jpg" extensions. If using the small dataset,
+                set this to ".jpg".
         """
         self.root = Path(root)
+        self.image_file_extension = image_file_extension
         self.data = self.load_specs(Path(specs_file))
 
         self.class_names = list(self.data.drop_duplicates("label").scientific_name)
 
         self.transform = (
             transform if transform else default_transform(image_size, training=training)
         )
 
-    @staticmethod
-    def load_specs(specs_file: Path) -> DataFrame:
+    def load_specs(self, specs_file: Path) -> DataFrame:
         """
         Load specs from a CSV file.
         Args:
             specs_file: path to the CSV file
         Returns:
             curated data contained in the CSV file
         """
         data = pd.read_csv(specs_file)
 
         class_names = list(data.scientific_name.unique())
         label_mapping = {name: class_names.index(name) for name in class_names}
 
+        if self.image_file_extension != ".JPG":
+            data.image_path = data.image_path.str.replace(
+                ".JPG", self.image_file_extension
+            )
+
         return data.assign(label=lambda df: df.scientific_name.map(label_mapping))
 
     def __getitem__(self, item: int) -> Tuple[Tensor, int]:
         """
         Get a data sample from its integer id.
         Args:
             item: sample's integer id
         Returns:
             data sample in the form of a tuple (image, label), where label is an integer.
-            The type of the image object depends of the output type of self.transform.
+            The type of the image object depends on the output type of self.transform.
         """
         img = self.transform(
             Image.open(self.root / self.data.image_path[item]).convert("RGB")
         )
         label = self.data.label[item]
 
         return img, label
```

### Comparing `easyfsl-1.3.0/easyfsl/datasets/default_configs.py` & `easyfsl-1.4.0/easyfsl/datasets/default_configs.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/datasets/easy_set.py` & `easyfsl-1.4.0/easyfsl/datasets/easy_set.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/datasets/features_dataset.py` & `easyfsl-1.4.0/easyfsl/datasets/features_dataset.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/datasets/few_shot_dataset.py` & `easyfsl-1.4.0/easyfsl/datasets/few_shot_dataset.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/datasets/mini_imagenet.py` & `easyfsl-1.4.0/easyfsl/datasets/mini_imagenet.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/datasets/support_set_folder.py` & `easyfsl-1.4.0/easyfsl/datasets/support_set_folder.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/datasets/tiered_imagenet.py` & `easyfsl-1.4.0/easyfsl/datasets/tiered_imagenet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from pathlib import Path
 
 from .easy_set import EasySet
 
 TIERED_IMAGENET_SPECS_DIR = Path("data/tiered_imagenet")
 
 
-# pylint: disable=invalid-name
-def TieredImageNet(split: str, **kwargs) -> EasySet:
-    """
-    Build the tieredImageNet dataset for the specific split.
-    Args:
-        split: one of the available split (typically train, val, test).
-
-    Returns:
-        the constructed dataset using EasySet
-
-    Raises:
-        ValueError: if the specified split cannot be associated with a JSON spec file
-            from tieredImageNet's specs directory
-    """
-    specs_file = TIERED_IMAGENET_SPECS_DIR / f"{split}.json"
-    if specs_file.is_file():
-        return EasySet(specs_file=specs_file, **kwargs)
-
-    raise ValueError(
-        f"Could not find specs file {specs_file.name} in {TIERED_IMAGENET_SPECS_DIR}"
-    )
-
-
-# pylint: enable=invalid-name
+class TieredImageNet(EasySet):
+    def __init__(self, split: str, **kwargs):
+        """
+        Build the tieredImageNet dataset for the specific split.
+        Args:
+            split: one of the available split (typically train, val, test).
+        Raises:
+            ValueError: if the specified split cannot be associated with a JSON spec file
+                from tieredImageNet's specs directory
+        """
+        specs_file = TIERED_IMAGENET_SPECS_DIR / f"{split}.json"
+        if not specs_file.is_file():
+            raise ValueError(
+                f"Could not find specs file {specs_file.name} in {TIERED_IMAGENET_SPECS_DIR}"
+            )
+        super().__init__(specs_file=specs_file, **kwargs)
```

### Comparing `easyfsl-1.3.0/easyfsl/datasets/wrap_few_shot_dataset.py` & `easyfsl-1.4.0/easyfsl/datasets/wrap_few_shot_dataset.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/methods/bd_cspn.py` & `easyfsl-1.4.0/easyfsl/methods/bd_cspn.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/methods/few_shot_classifier.py` & `easyfsl-1.4.0/easyfsl/methods/few_shot_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,24 +64,25 @@
 
     @staticmethod
     def is_transductive() -> bool:
         raise NotImplementedError(
             "All few-shot algorithms must implement a is_transductive method."
         )
 
-    def softmax_if_specified(self, output: Tensor) -> Tensor:
+    def softmax_if_specified(self, output: Tensor, temperature: float = 1.0) -> Tensor:
         """
         If the option is chosen when the classifier is initialized, we perform a softmax on the
         output in order to return soft probabilities.
         Args:
             output: output of the forward method of shape (n_query, n_classes)
+            temperature: temperature of the softmax
         Returns:
             output as it was, or output as soft probabilities, of shape (n_query, n_classes)
         """
-        return output.softmax(-1) if self.use_softmax else output
+        return (temperature * output).softmax(-1) if self.use_softmax else output
 
     def l2_distance_to_prototypes(self, samples: Tensor) -> Tensor:
         """
         Compute prediction logits from their euclidean distance to support set prototypes.
         Args:
             samples: features of the items to classify of shape (n_samples, feature_dimension)
         Returns:
```

### Comparing `easyfsl-1.3.0/easyfsl/methods/finetune.py` & `easyfsl-1.4.0/easyfsl/methods/finetune.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,31 +17,35 @@
 
     This is an inductive method.
     """
 
     def __init__(
         self,
         *args,
-        fine_tuning_steps: int = 10,
-        fine_tuning_lr: float = 1e-3,
+        fine_tuning_steps: int = 200,
+        fine_tuning_lr: float = 1e-4,
+        temperature: float = 1.0,
         **kwargs,
     ):
         """
         Args:
             fine_tuning_steps: number of fine-tuning steps
             fine_tuning_lr: learning rate for fine-tuning
+            temperature: temperature applied to the logits before computing
+                softmax or cross-entropy. Higher temperature means softer predictions.
         """
         super().__init__(*args, **kwargs)
 
         # Since we fine-tune the prototypes we need to make them leaf variables
         # i.e. we need to freeze the backbone.
         self.backbone.requires_grad_(False)
 
         self.fine_tuning_steps = fine_tuning_steps
         self.fine_tuning_lr = fine_tuning_lr
+        self.temperature = temperature
 
     def process_support_set(
         self,
         support_images: torch.Tensor,
         support_labels: torch.Tensor,
     ):
         """
@@ -63,19 +67,22 @@
         with torch.enable_grad():
             self.prototypes.requires_grad_()
             optimizer = torch.optim.Adam([self.prototypes], lr=self.fine_tuning_lr)
             for _ in range(self.fine_tuning_steps):
                 support_logits = self.cosine_distance_to_prototypes(
                     self.support_features
                 )
-                loss = nn.functional.cross_entropy(support_logits, self.support_labels)
+                loss = nn.functional.cross_entropy(
+                    self.temperature * support_logits, self.support_labels
+                )
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
 
         return self.softmax_if_specified(
-            self.cosine_distance_to_prototypes(query_features)
+            self.cosine_distance_to_prototypes(query_features),
+            temperature=self.temperature,
         ).detach()
 
     @staticmethod
     def is_transductive() -> bool:
         return False
```

### Comparing `easyfsl-1.3.0/easyfsl/methods/matching_networks.py` & `easyfsl-1.4.0/easyfsl/methods/matching_networks.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/methods/prototypical_networks.py` & `easyfsl-1.4.0/easyfsl/methods/prototypical_networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 See original implementation (quite far from this one)
 at https://github.com/jakesnell/prototypical-networks
 """
 
-import torch
 from torch import Tensor
 
 from .few_shot_classifier import FewShotClassifier
 from .utils import compute_prototypes
 
 
 class PrototypicalNetworks(FewShotClassifier):
@@ -45,17 +44,14 @@
         Classification scores are the negative of euclidean distances.
         """
         # Extract the features of query images
         query_features = self.backbone.forward(query_images)
         self._raise_error_if_features_are_multi_dimensional(query_features)
 
         # Compute the euclidean distance from queries to prototypes
-        dists = torch.cdist(query_features, self.prototypes)
-
-        # Use it to compute classification scores
-        scores = -dists
+        scores = self.l2_distance_to_prototypes(query_features)
 
         return self.softmax_if_specified(scores)
 
     @staticmethod
     def is_transductive() -> bool:
         return False
```

### Comparing `easyfsl-1.3.0/easyfsl/methods/relation_networks.py` & `easyfsl-1.4.0/easyfsl/methods/relation_networks.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/methods/tim.py` & `easyfsl-1.4.0/easyfsl/methods/tim.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,40 +19,44 @@
 
     TIM is a transductive method.
     """
 
     def __init__(
         self,
         *args,
-        fine_tuning_steps: int = 100,
-        fine_tuning_lr: float = 1e-3,
+        fine_tuning_steps: int = 50,
+        fine_tuning_lr: float = 1e-4,
         cross_entropy_weight: float = 1.0,
         marginal_entropy_weight: float = 1.0,
         conditional_entropy_weight: float = 0.1,
+        temperature: float = 10.0,
         **kwargs,
     ):
         """
         Args:
             fine_tuning_steps: number of fine-tuning steps
             fine_tuning_lr: learning rate for fine-tuning
             cross_entropy_weight: weight given to the cross-entropy term of the loss
             marginal_entropy_weight: weight given to the marginal entropy term of the loss
             conditional_entropy_weight: weight given to the conditional entropy term of the loss
+            temperature: temperature applied to the logits before computing
+                softmax or cross-entropy. Higher temperature means softer predictions.
         """
         super().__init__(*args, **kwargs)
 
         # Since we fine-tune the prototypes we need to make them leaf variables
         # i.e. we need to freeze the backbone.
         self.backbone.requires_grad_(False)
 
         self.fine_tuning_steps = fine_tuning_steps
         self.fine_tuning_lr = fine_tuning_lr
         self.cross_entropy_weight = cross_entropy_weight
         self.marginal_entropy_weight = marginal_entropy_weight
         self.conditional_entropy_weight = conditional_entropy_weight
+        self.temperature = temperature
 
     def process_support_set(
         self,
         support_images: torch.Tensor,
         support_labels: torch.Tensor,
     ):
         """
@@ -76,16 +80,20 @@
         support_labels_one_hot = nn.functional.one_hot(self.support_labels, num_classes)
 
         with torch.enable_grad():
             self.prototypes.requires_grad_()
             optimizer = torch.optim.Adam([self.prototypes], lr=self.fine_tuning_lr)
 
             for _ in range(self.fine_tuning_steps):
-                support_logits = self.l2_distance_to_prototypes(self.support_features)
-                query_logits = self.l2_distance_to_prototypes(query_features)
+                support_logits = self.temperature * self.cosine_distance_to_prototypes(
+                    self.support_features
+                )
+                query_logits = self.temperature * self.cosine_distance_to_prototypes(
+                    query_features
+                )
 
                 support_cross_entropy = (
                     -(support_labels_one_hot * support_logits.log_softmax(1))
                     .sum(1)
                     .mean(0)
                 )
 
@@ -107,13 +115,14 @@
                 )
 
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
 
         return self.softmax_if_specified(
-            self.l2_distance_to_prototypes(query_features)
+            self.cosine_distance_to_prototypes(query_features),
+            temperature=self.temperature,
         ).detach()
 
     @staticmethod
     def is_transductive() -> bool:
         return True
```

### Comparing `easyfsl-1.3.0/easyfsl/modules/predesigned_modules.py` & `easyfsl-1.4.0/easyfsl/modules/predesigned_modules.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/modules/resnet.py` & `easyfsl-1.4.0/easyfsl/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/samplers/task_sampler.py` & `easyfsl-1.4.0/easyfsl/samplers/task_sampler.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/datasets/easy_set_test.py` & `easyfsl-1.4.0/easyfsl/tests/datasets/easy_set_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/datasets/features_dataset_test.py` & `easyfsl-1.4.0/easyfsl/tests/datasets/features_dataset_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/datasets/support_set_folder_test.py` & `easyfsl-1.4.0/easyfsl/tests/datasets/support_set_folder_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/datasets/wrap_few_shot_dataset_test.py` & `easyfsl-1.4.0/easyfsl/tests/datasets/wrap_few_shot_dataset_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/methods/conftest.py` & `easyfsl-1.4.0/easyfsl/tests/methods/conftest.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/methods/few_shot_classifier_test.py` & `easyfsl-1.4.0/easyfsl/tests/methods/few_shot_classifier_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/methods/finetuning_methods_test.py` & `easyfsl-1.4.0/easyfsl/tests/methods/finetuning_methods_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from itertools import product
 
 import pytest
 import torch
 from torch import nn
 
 from easyfsl.datasets import SupportSetFolder
-from easyfsl.methods import TIM, Finetune, TransductiveFinetuning
+from easyfsl.methods import PTMAP, TIM, Finetune, TransductiveFinetuning
 
 ALL_FINETUNING_METHODS = [
     Finetune,
     TIM,
     TransductiveFinetuning,
+    PTMAP,
 ]
 
 
 class TestFinetuningMethodsRun:
     @staticmethod
     @pytest.mark.parametrize("method", ALL_FINETUNING_METHODS)
     def test_methods_run_in_ordinary_context(
```

### Comparing `easyfsl-1.3.0/easyfsl/tests/methods/matching_networks_test.py` & `easyfsl-1.4.0/easyfsl/tests/methods/matching_networks_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/methods/prototypical_networks_test.py` & `easyfsl-1.4.0/easyfsl/tests/methods/prototypical_networks_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/methods/relation_networks_test.py` & `easyfsl-1.4.0/easyfsl/tests/methods/relation_networks_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/modules/predesigned_modules_test.py` & `easyfsl-1.4.0/easyfsl/tests/modules/predesigned_modules_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/modules/resnet_test.py` & `easyfsl-1.4.0/easyfsl/tests/modules/resnet_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/samplers/task_sampler_test.py` & `easyfsl-1.4.0/easyfsl/tests/samplers/task_sampler_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/tests/utils_test.py` & `easyfsl-1.4.0/easyfsl/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/easyfsl/utils.py` & `easyfsl-1.4.0/easyfsl/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     all_class_names = []
     with torch.no_grad():
         for images, class_names in tqdm(
             dataloader, unit="batch", desc="Predicting embeddings"
         ):
             if device is not None:
                 images = images.to(device)
-            all_embeddings.append(model(images).cpu())
+            all_embeddings.append(model(images).detach().cpu())
             if isinstance(class_names, torch.Tensor):
                 all_class_names += class_names.tolist()
             else:
                 all_class_names += class_names
 
     concatenated_embeddings = torch.cat(all_embeddings)
 
@@ -93,21 +93,19 @@
     query_labels: Tensor,
 ) -> Tuple[int, int]:
     """
     Returns the number of correct predictions of query labels, and the total number of
     predictions.
     """
     model.process_support_set(support_images, support_labels)
-    return (
-        torch.max(
-            model(query_images).detach().data,
-            1,
-        )[1]
-        == query_labels
-    ).sum().item(), len(query_labels)
+    predictions = model(query_images).detach().data
+    number_of_correct_predictions = (
+        (torch.max(predictions, 1)[1] == query_labels).sum().item()
+    )
+    return number_of_correct_predictions, len(query_labels)
 
 
 def evaluate(
     model: FewShotClassifier,
     data_loader: DataLoader,
     device: str = "cuda",
     use_tqdm: bool = True,
@@ -129,14 +127,15 @@
     total_predictions = 0
     correct_predictions = 0
 
     # eval mode affects the behaviour of some layers (such as batch normalization or dropout)
     # no_grad() tells torch not to keep in memory the whole computational graph
     model.eval()
     with torch.no_grad():
+        # We use a tqdm context to show a progress bar in the logs
         with tqdm(
             enumerate(data_loader),
             total=len(data_loader),
             disable=not use_tqdm,
             desc=tqdm_prefix,
         ) as tqdm_eval:
             for _, (
```

### Comparing `easyfsl-1.3.0/easyfsl.egg-info/SOURCES.txt` & `easyfsl-1.4.0/easyfsl.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,36 +18,44 @@
 easyfsl/datasets/few_shot_dataset.py
 easyfsl/datasets/mini_imagenet.py
 easyfsl/datasets/support_set_folder.py
 easyfsl/datasets/tiered_imagenet.py
 easyfsl/datasets/wrap_few_shot_dataset.py
 easyfsl/methods/__init__.py
 easyfsl/methods/bd_cspn.py
+easyfsl/methods/feat.py
 easyfsl/methods/few_shot_classifier.py
 easyfsl/methods/finetune.py
+easyfsl/methods/laplacian_shot.py
 easyfsl/methods/matching_networks.py
 easyfsl/methods/prototypical_networks.py
+easyfsl/methods/pt_map.py
 easyfsl/methods/relation_networks.py
+easyfsl/methods/simple_shot.py
 easyfsl/methods/tim.py
 easyfsl/methods/transductive_finetuning.py
 easyfsl/methods/utils.py
 easyfsl/modules/__init__.py
+easyfsl/modules/attention_modules.py
+easyfsl/modules/build_from_checkpoint.py
+easyfsl/modules/feat_resnet12.py
 easyfsl/modules/predesigned_modules.py
 easyfsl/modules/resnet.py
 easyfsl/samplers/__init__.py
 easyfsl/samplers/task_sampler.py
 easyfsl/tests/__init__.py
 easyfsl/tests/utils_test.py
 easyfsl/tests/datasets/__init__.py
 easyfsl/tests/datasets/easy_set_test.py
 easyfsl/tests/datasets/features_dataset_test.py
 easyfsl/tests/datasets/support_set_folder_test.py
 easyfsl/tests/datasets/wrap_few_shot_dataset_test.py
 easyfsl/tests/methods/__init__.py
 easyfsl/tests/methods/conftest.py
+easyfsl/tests/methods/feat_test.py
 easyfsl/tests/methods/few_shot_classifier_test.py
 easyfsl/tests/methods/finetuning_methods_test.py
 easyfsl/tests/methods/matching_networks_test.py
 easyfsl/tests/methods/prototypical_networks_test.py
 easyfsl/tests/methods/relation_networks_test.py
 easyfsl/tests/modules/__init__.py
 easyfsl/tests/modules/predesigned_modules_test.py
```

### Comparing `easyfsl-1.3.0/pyproject.toml` & `easyfsl-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyfsl-1.3.0/setup.py` & `easyfsl-1.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="easyfsl",
-    version="1.3.0",
+    version="1.4.0",
     description="Ready-to-use PyTorch code to boost your way into few-shot image classification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sicara/easy-few-shot-learning",
     license="MIT",
     install_requires=[
         "matplotlib>=3.0.0",
-        "pandas>=1.3.0",
+        "pandas>=1.4.0",
         "torch>=1.4.0",
         "torchvision>=0.7.0",
         "tqdm>=4.1.0",
     ],
     packages=find_packages(),
     python_requires=">=3.6",
     entry_points={},
```

