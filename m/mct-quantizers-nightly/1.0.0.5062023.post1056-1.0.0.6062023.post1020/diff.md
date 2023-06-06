# Comparing `tmp/mct-quantizers-nightly-1.0.0.5062023.post1056.tar.gz` & `tmp/mct-quantizers-nightly-1.0.0.6062023.post1020.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.0.0.5062023.post1056.tar", last modified: Mon Jun  5 00:10:59 2023, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.0.0.6062023.post1020.tar", last modified: Tue Jun  6 00:10:22 2023, max compression
```

## Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056.tar` & `mct-quantizers-nightly-1.0.0.6062023.post1020.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.394463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.394463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.394463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.394463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.394463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-05 00:10:31.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-05 00:10:58.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-05 00:10:59.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:10:58.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 00:10:58.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 00:10:58.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 00:10:59.398463 mct-quantizers-nightly-1.0.0.5062023.post1056/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-05 00:10:56.000000 mct-quantizers-nightly-1.0.0.5062023.post1056/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.217260 mct-quantizers-nightly-1.0.0.6062023.post1020/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-06 00:10:22.221260 mct-quantizers-nightly-1.0.0.6062023.post1020/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.213260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.213260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.213260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.213260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.213260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.213260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.213260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.217260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.217260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.217260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-06 00:10:07.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:10:22.217260 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-06 00:10:21.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-06 00:10:22.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 00:10:21.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 00:10:21.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 00:10:21.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-06 00:10:22.221260 mct-quantizers-nightly-1.0.0.6062023.post1020/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-06 00:10:20.000000 mct-quantizers-nightly-1.0.0.6062023.post1020/setup.py
```

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/LICENSE.md` & `mct-quantizers-nightly-1.0.0.6062023.post1020/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/PKG-INFO` & `mct-quantizers-nightly-1.0.0.6062023.post1020/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.0.0.5062023.post1056
+Version: 1.0.0.6062023.post1020
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Tollkit (MCT) Quantizers
         
         This is an open-source library that provides tools that enable to easily represent a quantized neural network, both in Keras and in PyTorch.
         It provides researchers, developers, and engineers a set of useful quantizers and, in addition, a simple interface for implementing new custom quantizers.
```

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/README.md` & `mct-quantizers-nightly-1.0.0.6062023.post1020/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.0.0.5062023.post1056
+Version: 1.0.0.6062023.post1020
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Tollkit (MCT) Quantizers
         
         This is an open-source library that provides tools that enable to easily represent a quantized neural network, both in Keras and in PyTorch.
         It provides researchers, developers, and engineers a set of useful quantizers and, in addition, a simple interface for implementing new custom quantizers.
```

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.0.0.6062023.post1020/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.5062023.post1056/setup.py` & `mct-quantizers-nightly-1.0.0.6062023.post1020/setup.py`

 * *Files identical despite different names*

