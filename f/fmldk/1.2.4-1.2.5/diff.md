# Comparing `tmp/fmldk-1.2.4.tar.gz` & `tmp/fmldk-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmldk-1.2.4.tar", last modified: Wed May 17 16:49:43 2023, max compression
+gzip compressed data, was "fmldk-1.2.5.tar", last modified: Tue Jun  6 06:08:55 2023, max compression
```

## Comparing `fmldk-1.2.4.tar` & `fmldk-1.2.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.485812 fmldk-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-17 16:49:43.485812 fmldk-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-05-17 16:49:32.000000 fmldk-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.473812 fmldk-1.2.4/ctfr/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_models_v0.1.29.py
--rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.473812 fmldk-1.2.4/ctfrv2/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/ctfrv2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/ctfrv2_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/ctfrv2_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/ctfrv2_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.473812 fmldk-1.2.4/ctfrv2_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36588 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2_gpu/ctfrv2_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2_gpu/ctfrv2_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    78757 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2_gpu/ctfrv2_model_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.473812 fmldk-1.2.4/eda/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/eda_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/eda_lib_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/eda_lib_v0.1.19.py
--rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/eda_lib_v0.1.37.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.477812 fmldk-1.2.4/fmldk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.477812 fmldk-1.2.4/sage/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46655 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_global_scaled_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_losses_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    86777 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_model_old.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.477812 fmldk-1.2.4/sage_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36569 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/sage_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/sage_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    90885 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/sage_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    87795 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/sage_model_gpu_v1.2.3.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:49:43.485812 fmldk-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-17 16:49:32.000000 fmldk-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.477812 fmldk-1.2.4/stctn/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/stctn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/stctn_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/stctn_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/stctn_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.481812 fmldk-1.2.4/tfr/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.14.py
--rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.15.py
--rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.16.py
--rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.21.py
--rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_local_block_sparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_local_block_sparse_attention_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_local_block_sparse_attention_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models_v0.1.23.py
--rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.485812 fmldk-1.2.4/tft/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46653 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_data_v1.1.3.py
--rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_data_v1.1.7.py
--rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    84122 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_model_v0.1.26.py
--rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_model_v0.1.31.py
--rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_model_v1.1.3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.485812 fmldk-1.2.4/tft_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36585 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft_gpu/tft_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft_gpu/tft_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    78604 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft_gpu/tft_model_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.406413 fmldk-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-06-06 06:08:55.406413 fmldk-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-06-06 06:08:42.000000 fmldk-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.390412 fmldk-1.2.5/ctfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfr/ctfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfr/ctfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfr/ctfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfr/ctfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfr/ctfr_models_v0.1.29.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfr/ctfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.390412 fmldk-1.2.5/ctfrv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2/ctfrv2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2/ctfrv2_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2/ctfrv2_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2/ctfrv2_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.390412 fmldk-1.2.5/ctfrv2_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36588 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2_gpu/ctfrv2_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2_gpu/ctfrv2_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82828 2023-06-06 06:08:42.000000 fmldk-1.2.5/ctfrv2_gpu/ctfrv2_model_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.394412 fmldk-1.2.5/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 06:08:42.000000 fmldk-1.2.5/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-06-06 06:08:42.000000 fmldk-1.2.5/eda/eda_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-06-06 06:08:42.000000 fmldk-1.2.5/eda/eda_lib_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-06-06 06:08:42.000000 fmldk-1.2.5/eda/eda_lib_v0.1.19.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-06-06 06:08:42.000000 fmldk-1.2.5/eda/eda_lib_v0.1.37.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.394412 fmldk-1.2.5/fmldk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-06-06 06:08:55.000000 fmldk-1.2.5/fmldk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-06 06:08:55.000000 fmldk-1.2.5/fmldk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:08:55.000000 fmldk-1.2.5/fmldk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 06:08:55.000000 fmldk-1.2.5/fmldk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 06:08:55.000000 fmldk-1.2.5/fmldk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.394412 fmldk-1.2.5/sage/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46655 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage/sage_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage/sage_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage/sage_global_scaled_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage/sage_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage/sage_losses_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97638 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage/sage_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83682 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage/sage_model_old.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.394412 fmldk-1.2.5/sage_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36569 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage_gpu/sage_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage_gpu/sage_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96543 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage_gpu/sage_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87795 2023-06-06 06:08:42.000000 fmldk-1.2.5/sage_gpu/sage_model_gpu_v1.2.3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 06:08:55.406413 fmldk-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-06 06:08:42.000000 fmldk-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.398412 fmldk-1.2.5/stctn/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-06 06:08:42.000000 fmldk-1.2.5/stctn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-06-06 06:08:42.000000 fmldk-1.2.5/stctn/stctn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-06-06 06:08:42.000000 fmldk-1.2.5/stctn/stctn_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-06-06 06:08:42.000000 fmldk-1.2.5/stctn/stctn_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-06-06 06:08:42.000000 fmldk-1.2.5/stctn/stctn_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.402413 fmldk-1.2.5/tfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_data_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_data_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_data_v0.1.14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_data_v0.1.15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_data_v0.1.16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_data_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_data_v0.1.21.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_local_block_sparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_local_block_sparse_attention_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_local_block_sparse_attention_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_models_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_models_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_models_v0.1.23.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-06-06 06:08:42.000000 fmldk-1.2.5/tfr/tfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.406413 fmldk-1.2.5/tft/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46653 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_data_v1.1.3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_data_v1.1.7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88381 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_model_v0.1.26.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_model_v0.1.31.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft/tft_model_v1.1.3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:08:55.406413 fmldk-1.2.5/tft_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36585 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft_gpu/tft_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft_gpu/tft_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82884 2023-06-06 06:08:42.000000 fmldk-1.2.5/tft_gpu/tft_model_gpu.py
```

### Comparing `fmldk-1.2.4/PKG-INFO` & `fmldk-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.2.4
+Version: 1.2.5
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
```

### Comparing `fmldk-1.2.4/README.md` & `fmldk-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfr/ctfr_data.py` & `fmldk-1.2.5/ctfr/ctfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfr/ctfr_losses.py` & `fmldk-1.2.5/ctfr/ctfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfr/ctfr_losses_bkp.py` & `fmldk-1.2.5/ctfr/ctfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfr/ctfr_models.py` & `fmldk-1.2.5/ctfr/ctfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfr/ctfr_models_v0.1.29.py` & `fmldk-1.2.5/ctfr/ctfr_models_v0.1.29.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfr/ctfr_models_v0.1.31.py` & `fmldk-1.2.5/ctfr/ctfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfrv2/ctfrv2_data.py` & `fmldk-1.2.5/ctfrv2/ctfrv2_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfrv2/ctfrv2_global_scaled_data.py` & `fmldk-1.2.5/ctfrv2/ctfrv2_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfrv2/ctfrv2_losses.py` & `fmldk-1.2.5/ctfrv2/ctfrv2_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfrv2/ctfrv2_models.py` & `fmldk-1.2.5/ctfrv2/ctfrv2_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfrv2_gpu/ctfrv2_data_gpu.py` & `fmldk-1.2.5/ctfrv2_gpu/ctfrv2_data_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfrv2_gpu/ctfrv2_losses_gpu.py` & `fmldk-1.2.5/ctfrv2_gpu/ctfrv2_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/ctfrv2_gpu/ctfrv2_model_gpu.py` & `fmldk-1.2.5/tft_gpu/tft_model_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,63 @@
     return tf.reduce_mean(dist.sample(sample_shape=n_samples), axis=0)
 
 # Gumbel
 def GumbelSample(a, b, n_samples=1):
     dist = tfd.Gumbel(loc=a, scale=b)
     return tf.reduce_mean(tf.stop_gradient(dist.sample(sample_shape=n_samples)), axis=0)
 
+# Quantile Risk Metric (MSE & MAE Metrics are available out of the box in tf)
+class q_risk(tf.keras.metrics.Metric):
+    def __init__(self, name='q_risk', q=[0.5], **kwargs):
+        super(q_risk, self).__init__(name=name, **kwargs)
+        self.q = q
+        self.qrisk = self.add_weight(name='qrisk_' + str(q), initializer='zeros')
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+
+        n_quantiles = y_pred.shape.as_list()[-1]
+        assert len(self.q) == n_quantiles
+
+        qr = 0
+        for q, qr_quantile in zip(range(n_quantiles), self.q):
+            qr += self.q_risk_function(y_true, y_pred[:, :, q:q + 1], qr_quantile)
+
+        if sample_weight is not None:
+            raise ValueError("Weighted q-risk not implemented.")
+            #sample_weight = tf.cast(sample_weight, self.dtype)
+            #sample_weight = tf.broadcast_to(sample_weight, values.shape)
+            #values = tf.multiply(values, sample_weight)
+
+        self.qrisk.assign_add(tf.reduce_mean(qr))
+
+    def q_risk_function(self, y_true, y_pred, qr_quantile):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+        qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+            tf.cast(0, tf.float32), (y_pred - y_true))
+        qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+        return qr_scaled
+
+    def result(self):
+        return self.qrisk
+
+
+def q_risk_function(y_true, y_pred, qr_quantile):
+    y_true = tf.cast(y_true, tf.float32)
+    y_pred = tf.cast(y_pred, tf.float32)
+
+    qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+        tf.cast(0, tf.float32), (y_pred - y_true))
+    qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+    return qr_scaled
+
 
 # Self-Attention
 def ScaledDotProductAttention(q, k, v, causal_mask, padding_mask):
     matmul_qk = tf.matmul(q, k, transpose_b=True)  # (..., seq_len_q, seq_len_k)
     dk = tf.cast(tf.shape(k)[-1], tf.float32)
     scaled_attention_logits = matmul_qk / tf.math.sqrt(dk)
     
@@ -1213,39 +1262,89 @@
             if weighted_training:                               
                 loss = loss_function(y_test, [o, wts])
             else:
                 loss = loss_function(y_test, o)                                   
         else:
             raise ValueError("Invalid loss_type specified!")        
         return loss, o
-       
+
+    def rescale_io(y_true, y_pred, scale):
+
+        out_len = y_true.shape.as_list()[1]
+        s_dim = scale.shape.as_list()[-1]
+
+        if loss_type in ['Point', 'Tweedie', 'Poisson']:
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred * scale[:, -out_len:, :]
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                y_pred_rescaled = y_pred * s_std + s_mean
+
+        elif loss_type in ['Quantile']:
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred * scale[:, -out_len:, :]
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                # rescale each quantile
+                n_quantiles = y_pred.shape.as_list()[-1]
+                y_list = []
+                for q in range(n_quantiles):
+                    y = y_pred[:, :, q:q + 1] * s_std + s_mean
+                    y_list.append(y)
+                y_pred_rescaled = tf.concat(y_list, axis=-1)
+
+        elif loss_type in ['Normal', 'Negbin']:
+            # predictions are already rescaled
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                y_pred_rescaled = y_pred
+
+        return y_true_rescaled, y_pred_rescaled
+
+
     # training specific vars
     if opt is None:
         optimizer = tf.keras.optimizers.Nadam(learning_rate=learning_rate)
     else:
         optimizer = opt
         optimizer.learning_rate=learning_rate
     
     if clipnorm is None:
         pass
     else:
-        optimizer.global_clipnorm = clipnorm
+        optimizer.clipnorm = clipnorm
        
     print("lr: ",optimizer.learning_rate.numpy())
     
     # model loss & metric
     train_loss_avg = tf.keras.metrics.Mean('train_loss', dtype=tf.float32)
     test_loss_avg = tf.keras.metrics.Mean('test_loss', dtype=tf.float32)
 
     if metric == 'MAE':  
         train_metric = tf.keras.metrics.MeanAbsoluteError('train_mae')
         test_metric = tf.keras.metrics.MeanAbsoluteError('test_mae')
+
     elif metric == 'MSE':
         train_metric = tf.keras.metrics.MeanSquaredError('train_mse')
         test_metric = tf.keras.metrics.MeanSquaredError('test_mse')
+
+    elif isinstance(metric, list):
+        train_metric = q_risk(name='train_qrisk', q=metric)
+        test_metric = q_risk(name='test_qrisk', q=metric)
     else:
         raise ValueError("{}: Not a Supported Metric".format(metric))
             
     #logging
     train_log_dir = str(logdir).rstrip('/') +'/train'
     test_log_dir = str(logdir).rstrip('/')+'/test'
     train_summary_writer = tf.summary.create_file_writer(train_log_dir)
@@ -1326,48 +1425,58 @@
         test_wts = tf.concat(test_wts, axis=0)
         print("Test Samples Gathered: ", x_test.shape[0])
 
         # chained tf.data.pipeline
         trainset = tf.data.Dataset.from_tensor_slices((x_train, y_train, train_scale, train_wts))
         trainset = trainset.shuffle(buffer_size=int(x_train.shape[0]), reshuffle_each_iteration=shuffle)
         trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
-        trainset = trainset.prefetch(buffer_size = tf.data.AUTOTUNE)
+        trainset = trainset.prefetch(buffer_size=tf.data.AUTOTUNE)
         
         testset = tf.data.Dataset.from_tensor_slices((x_test, y_test, test_scale, test_wts))
-        testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=False)
+        testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=shuffle)
         testset = testset.batch(batch_size=test_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
-        testset = testset.prefetch(buffer_size = tf.data.AUTOTUNE)
+        testset = testset.prefetch(buffer_size=tf.data.AUTOTUNE)
         
         for epoch in range(max_epochs):
             print("Epoch {}/{}".format(epoch, max_epochs))
            
             for i, (x_batch, y_batch, scale, wts) in enumerate(trainset):
                 train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
-                out_len = tf.shape(train_out)[1]
                 train_loss_avg.update_state(train_loss)
-                if loss_type in ['Normal', 'Negbin']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out)
-                elif loss_type in ['Point', 'Poisson', 'Tweedie']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
-                elif loss_type in ['Quantile']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
+                # rescale io & update metric
+                y_true, y_pred = rescale_io(y_batch, train_out, scale)
+                train_metric.update_state(y_true, y_pred)
+
+                #if loss_type in ['Normal', 'Negbin']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out)
+                #elif loss_type in ['Point', 'Poisson', 'Tweedie']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
+                #elif loss_type in ['Quantile']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
                 with train_summary_writer.as_default():
                     tf.summary.scalar('loss', train_loss_avg.result(), step=(i+1)*(epoch+1))
                     tf.summary.scalar('accuracy', train_metric.result(), step=(i+1)*(epoch+1))
 
             for i, (x_batch, y_batch, scale, wts) in enumerate(testset):
-                test_loss, test_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=False)
-                out_len = tf.shape(test_out)[1]
+                test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
                 test_loss_avg.update_state(test_loss)
-                if loss_type in ['Normal', 'Negbin']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out)
-                elif loss_type in ['Point', 'Tweedie', 'Poisson']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
-                elif loss_type in ['Quantile']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
+                # rescale io
+                y_true, y_pred = rescale_io(y_batch, test_out, scale)
+                test_metric.update_state(y_true, y_pred)
+
+                #if loss_type in ['Normal', 'Negbin']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out)
+                #elif loss_type in ['Point', 'Tweedie', 'Poisson']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
+                #elif loss_type in ['Quantile']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
                 with test_summary_writer.as_default():
                     tf.summary.scalar('loss', test_loss_avg.result(), step=(i+1)*(epoch+1))
                     tf.summary.scalar('accuracy', test_metric.result(), step=(i+1)*(epoch+1))
 
             print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
                                                                                                        train_loss_avg.result().numpy(),
                                                                                                        test_loss_avg.result().numpy(),
@@ -1395,21 +1504,25 @@
             else:
                 prev_min_loss = np.min(test_loss_results[:-1])
             current_min_loss = np.min(test_loss_results)
             delta = current_min_loss - prev_min_loss
 
             print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
             # track & save best model
-            if ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
+            if ((test_loss_results[-1] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
                 best_model = model_path
                 tf.keras.models.save_model(model, model_path)
                 # reset time_since_improvement
                 time_since_improvement = 0
             else:
                 time_since_improvement += 1
+                train_loss_results.pop()
+                test_loss_results.pop()
+                train_metric_results.pop()
+                test_metric_results.pop()
 
             model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
             print("Best Model: ", best_model)
 
             # remove older models
             if len(model_list) > patience:
                 for m in model_list[:-patience]:
@@ -1549,43 +1662,41 @@
     #decoder_wts_df = pd.concat([pd.DataFrame(id_arr.reshape(-1,1)), decoder_wts_df], axis=1)
 
     print(stat_wts_df.shape, encoder_wts_df.shape, decoder_wts_df.shape)
         
     return forecast_df, stat_wts_df, encoder_wts_df, decoder_wts_df
 
 
-class Feature_Weighted_ConvTransformer:
+class Temporal_Fusion_Transformer:
     def __init__(self, 
                  col_index_dict,
                  vocab_dict,
                  num_layers,
                  num_heads,
-                 kernel_sizes,
                  d_model,
                  forecast_horizon,
                  max_inp_len,
                  loss_type,
                  num_quantiles=1,
-                 decoder_lags=1,
+                 decoder_start_tokens=1,
                  dropout_rate=0.1,
                  seed=None,
                  deterministic_ops=False):
         
         self.col_index_dict = col_index_dict
         self.vocab_dict = vocab_dict
         self.num_layers = num_layers
         self.num_heads = num_heads
-        self.kernel_sizes = kernel_sizes  #not used -- using lstm instead
         self.d_model = d_model
         self.forecast_horizon = forecast_horizon
         self.max_inp_len = max_inp_len
         self.loss_type = loss_type
         self.num_quantiles = num_quantiles
         self.dropout_rate = dropout_rate
-        self.decoder_start_tokens = decoder_lags
+        self.decoder_start_tokens = decoder_start_tokens
         self.target_col_name, self.target_index = self.col_index_dict.get('target_index')
         self.seed = seed
         self.allow_deterministic_ops = deterministic_ops
 
     def set_seed(self):
         tf.keras.utils.set_random_seed(self.seed)
         if self.allow_deterministic_ops:
@@ -1625,15 +1736,15 @@
               train_dataset, 
               test_dataset,
               loss_function, 
               metric='MSE',
               learning_rate=0.0001,
               max_epochs=100,
               min_epochs=10,
-              prefill_buffers=False,
+              prefill_buffers=True,
               num_train_samples=200000,
               num_test_samples=50000,
               train_batch_size=64,
               test_batch_size=128,
               train_steps_per_epoch=200,
               test_steps_per_epoch=100,
               patience=10,
@@ -1687,13 +1798,12 @@
                                self.allow_deterministic_ops)
         return best_model
     
     def load(self, model_path):
         tf.keras.backend.clear_session()
         self.model = tf.keras.models.load_model(model_path)
         
-    def infer(self, inputs, recursive_decode=True):
-        # recursive decode not used
+    def infer(self, inputs):
         forecast, stat_wts_df, encoder_wts_df, decoder_wts_df = TFT_Infer(self.model, inputs, self.loss_type, self.max_inp_len, self.forecast_horizon, self.target_index, self.num_quantiles)
         
         return forecast, [stat_wts_df, encoder_wts_df, decoder_wts_df]
```

### Comparing `fmldk-1.2.4/eda/eda_lib.py` & `fmldk-1.2.5/eda/eda_lib.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/eda/eda_lib_v0.1.18.py` & `fmldk-1.2.5/eda/eda_lib_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/eda/eda_lib_v0.1.19.py` & `fmldk-1.2.5/eda/eda_lib_v0.1.19.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/eda/eda_lib_v0.1.37.py` & `fmldk-1.2.5/eda/eda_lib_v0.1.37.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/fmldk.egg-info/PKG-INFO` & `fmldk-1.2.5/fmldk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.2.4
+Version: 1.2.5
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
```

### Comparing `fmldk-1.2.4/fmldk.egg-info/SOURCES.txt` & `fmldk-1.2.5/fmldk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/sage/sage_data.py` & `fmldk-1.2.5/sage/sage_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/sage/sage_data_old.py` & `fmldk-1.2.5/sage/sage_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/sage/sage_global_scaled_data_old.py` & `fmldk-1.2.5/sage/sage_global_scaled_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/sage/sage_losses.py` & `fmldk-1.2.5/sage/sage_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/sage/sage_losses_old.py` & `fmldk-1.2.5/sage/sage_losses_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/sage/sage_model.py` & `fmldk-1.2.5/sage_gpu/sage_model_gpu_v1.2.3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-
+# Databricks notebook source
 import numpy as np
 import math as m
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import shutil
 import pickle
 import absl.logging
 absl.logging.set_verbosity(absl.logging.ERROR)
 import pandas as pd
 import gc
+from sys import platform
 import os
 
 # Distribution Sampling functions
 
 # negbin
 def negbin_sample(mu, alpha, n_samples=1):
     tol = 1e-5
@@ -856,16 +854,15 @@
        
         if self.loss_fn in ['Point','Quantile','Tweedie','Poisson']:
             return out, scale, static_weights, decoder_weights
         else:
             return out, parameters, static_weights, decoder_weights
 
 
-
-# SAGE Wrapper
+# SageTransformer Wrapper
 
 class SageTransformer_Model(tf.keras.Model):
     def __init__(self,
                  col_index_dict,
                  vocab_dict,
                  num_layers,
                  num_heads,
@@ -1118,18 +1115,19 @@
                       test_batch_size,
                       train_steps_per_epoch,
                       test_steps_per_epoch,
                       patience,
                       weighted_training,
                       model_prefix,
                       logdir,
-                      opt=None,
-                      clipnorm=None,
-                      min_delta=0.0001,
-                      shuffle=True):
+                      opt,
+                      clipnorm,
+                      min_delta,
+                      shuffle,
+                      deterministic):
     """
      train_dataset, test_dataset: tf.data.Dataset iterator for train & test datasets 
      loss_type: One of ['Point','Quantile','Normal','Poisson','Negbin']
      loss_function: One of the supported loss functions in loss library
      metric: 'MAE' or 'MSE' 
      max_epochs: Max. training epochs
      min_epochs: Min. Training epochs
@@ -1263,15 +1261,15 @@
        
     # training specific vars
     if opt is None:
         optimizer = tf.keras.optimizers.Nadam(learning_rate=learning_rate)
     else:
         optimizer = opt
         optimizer.learning_rate=learning_rate
-    
+        
     if clipnorm is None:
         pass
     else:
         optimizer.global_clipnorm = clipnorm
        
     print("lr: ",optimizer.learning_rate.numpy())
     
@@ -1341,100 +1339,95 @@
       seed = np.random.randint(0, 2**(32 - 1) - 1) if set_seed < 0 else set_seed
       for arr in arrays:
         rstate = np.random.RandomState(seed)
         rstate.shuffle(arr)
     
     if prefill_buffers:
       print("prefetching training samples ... ")
-      # get batch size
-      batch_size = 0
-      for x,y,s,w in train_dataset.take(1):
-        batch_size = int(x.shape[0])
-
+      
       x_train = []
       y_train = []
       train_scale = []
       train_wts = []
-      #num_train_batches = 0
+   
       for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
         x_train.append(x_batch)
         y_train.append(y_batch)
         train_scale.append(scale)
         train_wts.append(wts)
-        #num_train_batches = num_train_batches + m.floor(batch_size/train_batch_size)
-        if (step+1)*batch_size >= num_train_samples:
-          break
        
       # concat
       x_train = tf.concat(x_train, axis=0)
       y_train = tf.concat(y_train, axis=0)
       train_scale = tf.concat(train_scale, axis=0)
       train_wts = tf.concat(train_wts, axis=0)
       print("Training Samples Gathered: ", x_train.shape[0])
       
       print("prefetching test samples ... ")
       x_test = []
       y_test = []
       test_scale = []
       test_wts = []
-      #num_test_batches = 0
+
       for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
         x_test.append(x_batch)
         y_test.append(y_batch)
         test_scale.append(scale)
         test_wts.append(wts)
-        #num_test_batches = num_test_batches + m.floor(batch_size/train_batch_size)
-        if (step+1)*batch_size >= num_test_samples:
-          break
 
       # concat
       x_test = tf.concat(x_test, axis=0)
       y_test = tf.concat(y_test, axis=0)
       test_scale = tf.concat(test_scale, axis=0)
       test_wts = tf.concat(test_wts, axis=0)
       print("Test Samples Gathered: ", x_test.shape[0])
         
-      num_train_batches = int(x_train.shape[0]//train_batch_size)
-      num_test_batches = int(x_test.shape[0]//test_batch_size)
-
+      #num_train_batches = int(x_train.shape[0]//train_batch_size)
+      #num_test_batches = int(x_test.shape[0]//test_batch_size)
+       
+      # chained tf.data.pipeline
+      trainset = tf.data.Dataset.from_tensor_slices((x_train, y_train, train_scale, train_wts))
+      trainset = trainset.shuffle(buffer_size=int(x_train.shape[0]), reshuffle_each_iteration=shuffle)
+      trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
+      trainset = trainset.prefetch(buffer_size = tf.data.AUTOTUNE)
+        
+      testset = tf.data.Dataset.from_tensor_slices((x_test, y_test, test_scale, test_wts))
+      testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=False)
+      testset = testset.batch(batch_size=test_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
+      testset = testset.prefetch(buffer_size = tf.data.AUTOTUNE)
+        
       for epoch in range(max_epochs):
           print("Epoch {}/{}". format(epoch, max_epochs))
           # shuffle Training data only,if shuffle=True
-          if shuffle:
-            #shuffle_arrays([x_train, y_train, train_scale, train_wts])
-            indices = tf.range(start=0, limit=tf.shape(x_train)[0], dtype=tf.int32)
-            shuffled_indices = tf.random.shuffle(indices)
-            x_train = tf.gather(x_train, shuffled_indices)
-            y_train = tf.gather(y_train, shuffled_indices)
-            train_scale = tf.gather(train_scale, shuffled_indices)
-            train_wts = tf.gather(train_wts, shuffled_indices)
-
-          for i in range(num_train_batches):
-            x_batch = x_train[i*train_batch_size:(i+1)*train_batch_size]
-            y_batch = y_train[i*train_batch_size:(i+1)*train_batch_size]
-            scale = train_scale[i*train_batch_size:(i+1)*train_batch_size]
-            wts = train_wts[i*train_batch_size:(i+1)*train_batch_size]
+          #if shuffle:
+          #  #shuffle_arrays([x_train, y_train, train_scale, train_wts])
+          #  indices = tf.range(start=0, limit=tf.shape(x_train)[0], dtype=tf.int32)
+          #  shuffled_indices = tf.random.shuffle(indices)
+          #  x_train = tf.gather(x_train, shuffled_indices)
+          #  y_train = tf.gather(y_train, shuffled_indices)
+          #  train_scale = tf.gather(train_scale, shuffled_indices)
+          #  train_wts = tf.gather(train_wts, shuffled_indices)
+          #  print("epoch {} first record {}".format(epoch, x_train[0,-1,:]))
+          #  print("epoch {} last record {}".format(epoch, x_train[-1,-1,:]))
+        
+          for i, (x_batch, y_batch, scale, wts) in enumerate(trainset):
             train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
             out_len = tf.shape(train_out)[1]
             train_loss_avg.update_state(train_loss)
             if loss_type in ['Normal','Negbin']:
               train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
             elif loss_type in ['Point','Tweedie','Poisson']:
               train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out*scale[:,-out_len:,:])
             elif loss_type in ['Quantile']:
               train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
             with train_summary_writer.as_default():
               tf.summary.scalar('loss', train_loss_avg.result(), step=(i+1)*(epoch+1))
               tf.summary.scalar('accuracy', train_metric.result(), step=(i+1)*(epoch+1))
-
-          for i in range(num_test_batches):
-            x_batch = x_test[i*train_batch_size:(i+1)*train_batch_size]
-            y_batch = y_test[i*train_batch_size:(i+1)*train_batch_size]
-            scale = test_scale[i*train_batch_size:(i+1)*train_batch_size]
-            wts = test_wts[i*train_batch_size:(i+1)*train_batch_size]
+                
+          for i, (x_batch, y_batch, scale, wts) in enumerate(testset):
             test_loss, test_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=False)
             out_len = tf.shape(test_out)[1]
             test_loss_avg.update_state(test_loss)
             if loss_type in ['Normal','Negbin']:
               test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
             elif loss_type in ['Point','Tweedie','Poisson']:
               test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out*scale[:,-out_len:,:])
@@ -1481,15 +1474,19 @@
               # reset time_since_improvement
               time_since_improvement = 0
           else:
               time_since_improvement += 1
 
           model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
           print("Best Model: ", best_model)
-
+          
+          # model avg. use ema after each epoch
+          #if use_ema:
+          #      optimizer.finalize_variable_values(model.trainable_variables)
+            
           # remove older models
           if len(model_list)>patience:
               for m in model_list[:-patience]:
                   if m != best_model:
                       try:
                           shutil.rmtree(m)
                       except:
@@ -1568,24 +1565,28 @@
           else:
             prev_min_loss = np.min(test_loss_results[:-1])
           current_min_loss = np.min(test_loss_results)
           delta = current_min_loss - prev_min_loss
          
           print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
           # track & save best model
-          if ((test_loss_results[epoch]==np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
+          if ((test_loss_results[epoch]==np.min(test_loss_results)) and (-delta > min_delta)) or  (epoch == 0):
               best_model = model_path
               tf.keras.models.save_model(model, model_path)
               # reset time_since_improvement
               time_since_improvement = 0
           else:
               time_since_improvement += 1
 
           model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
           print("Best Model: ", best_model)
+            
+          # model avg. use ema after each epoch
+          #if use_ema:
+          #  optimizer.finalize_variable_values(model.trainable_variables)
 
           # remove older models
           if len(model_list)>patience:
               for m in model_list[:-patience]:
                   if m != best_model:
                       try:
                           shutil.rmtree(m)
@@ -1598,16 +1599,15 @@
               break
 
           # write after each epoch
           model_tracker_file.flush()
         
     return best_model
         
- 
-        
+
 def SageTransformer_InferRecursive(model, inputs, loss_type, hist_len, f_len, target_index, num_quantiles):
     infer_tensor, scale, id_arr, date_arr = inputs
     s_dim = scale.shape[-1]
     
     if s_dim == 1:
         scale = scale[:,-1:,-1]
     else:
@@ -1664,14 +1664,15 @@
         
     # rescale if necessary
     if loss_type in ['Normal','Negbin']:
         output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr), axis=1))
         output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
         output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
     elif loss_type in ['Point','Tweedie','Poisson']:
+        # 
         if s_dim == 1:
             output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr[:,:,0]*scale.reshape(-1,1)), axis=1))
         else:
             output_arr = output_arr[:,:,0]*scale_std.reshape(-1,1) + scale_mean.reshape(-1,1)
             output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1), output_arr), axis=1))
         output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
         output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
@@ -1710,16 +1711,14 @@
     decoder_wts_df = pd.concat([fid_df, decoder_wts_df], axis=1) 
     
     print(stat_wts_df.shape, decoder_wts_df.shape)
         
     return forecast_df, stat_wts_df, decoder_wts_df
 
 
-
-
 class SageModel:
     def __init__(self, 
                  col_index_dict,
                  vocab_dict,
                  num_layers,
                  num_heads,
                  kernel_sizes,
@@ -1742,21 +1741,29 @@
         self.max_inp_len = max_inp_len
         self.loss_type = loss_type
         self.num_quantiles = num_quantiles
         self.dropout_rate = dropout_rate
         self.target_col_name, self.target_index = self.col_index_dict.get('target_index')
         self.seed = seed
         self.allow_deterministic_ops = deterministic_ops
-    
+        
     def set_seed(self):
         tf.keras.utils.set_random_seed(self.seed)
         if self.allow_deterministic_ops:
             print("Deterministic Ops enabled.")
-            os.environ["TF_DETERMINISTIC_OPS"] = "True"
-            os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
+            if platform == "linux" or platform == "linux2":
+              print("GPU/CPU Determinism enabled for Linux")
+              os.environ["TF_DETERMINISTIC_OPS"] = "True"
+            else:
+              print("GPU/CPU Determinism partially enabled for Windows & Others")
+              os.environ["TF_DETERMINISTIC_OPS"] = "True"
+              os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
+        else:
+            print("Deterministic Ops disabled.")
+            os.environ["TF_DETERMINISTIC_OPS"] = "False"
         
     def build(self):
         tf.keras.backend.clear_session()
         if self.seed is None:
             print("No seed set for deterministic weights initialization")
         else:
             print("Using seed {} for weights initialization".format(self.seed))
@@ -1798,19 +1805,21 @@
               clipnorm=None,
               min_delta=0.0001,
               shuffle=True):
         
         if load_model is None:
             # Initialize Weights
             for x,y,s,w in train_dataset.take(1):
-                self.model(x, training=False)
+                self.model(x[0:2], training=False)
+                #print(x[0:2,-1:,:])
+                #print(self.model.layers[0].get_weights())
         else:
             # Initialize Weights
             for x,y,s,w in train_dataset.take(1):
-                self.model(x, training=False)
+                self.model(x[0:2], training=False)
             saved_model = tf.keras.models.load_model(load_model)
             self.model.set_weights(saved_model.get_weights())
             del saved_model
             gc.collect()
             print("Saved model: {} loaded. Continuing training ...".format(load_model))
         
         best_model = SageTransformer_Train(self.model,
@@ -1833,21 +1842,21 @@
                                           patience,
                                           weighted_training,
                                           model_prefix,
                                           logdir,
                                           opt,
                                           clipnorm,
                                           min_delta,
-                                          shuffle)
+                                          shuffle,
+                                          self.allow_deterministic_ops)
         return best_model
     
     def load(self, model_path):
         tf.keras.backend.clear_session()
         self.model = tf.keras.models.load_model(model_path)
         
     def infer(self, inputs):
         forecast, stat_wts_df, decoder_wts_df = SageTransformer_InferRecursive(self.model, inputs, self.loss_type, self.max_inp_len, self.forecast_horizon, self.target_index, self.num_quantiles)
         
         return forecast, [stat_wts_df, decoder_wts_df]
     
     
-
```

### Comparing `fmldk-1.2.4/sage/sage_model_old.py` & `fmldk-1.2.5/sage/sage_model_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -1331,31 +1331,29 @@
       assert all(len(arr) == len(arrays[0]) for arr in arrays)
       seed = np.random.randint(0, 2**(32 - 1) - 1) if set_seed < 0 else set_seed
       for arr in arrays:
         rstate = np.random.RandomState(seed)
         rstate.shuffle(arr)
     
     if prefill_buffers:
-      print("prefetching training samples ... ")
       # get batch size
       batch_size = 0
       for x,y,s,w in train_dataset.take(1):
         batch_size = int(x.shape[0])
 
+      print("prefetching training samples ... ")
       x_train = []
       y_train = []
       train_scale = []
       train_wts = []
-      #num_train_batches = 0
       for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
         x_train.append(x_batch)
         y_train.append(y_batch)
         train_scale.append(scale)
         train_wts.append(wts)
-        #num_train_batches = num_train_batches + m.floor(batch_size/train_batch_size)
         if (step+1)*batch_size >= num_train_samples:
           break
        
       # concat
       x_train = tf.concat(x_train, axis=0)
       y_train = tf.concat(y_train, axis=0)
       train_scale = tf.concat(train_scale, axis=0)
@@ -1363,21 +1361,19 @@
       print("Training Samples Gathered: ", x_train.shape[0])
       
       print("prefetching test samples ... ")
       x_test = []
       y_test = []
       test_scale = []
       test_wts = []
-      #num_test_batches = 0
       for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
         x_test.append(x_batch)
         y_test.append(y_batch)
         test_scale.append(scale)
         test_wts.append(wts)
-        #num_test_batches = num_test_batches + m.floor(batch_size/train_batch_size)
         if (step+1)*batch_size >= num_test_samples:
           break
 
       # concat
       x_test = tf.concat(x_test, axis=0)
       y_test = tf.concat(y_test, axis=0)
       test_scale = tf.concat(test_scale, axis=0)
```

### Comparing `fmldk-1.2.4/sage_gpu/sage_data_gpu.py` & `fmldk-1.2.5/sage_gpu/sage_data_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/sage_gpu/sage_losses_gpu.py` & `fmldk-1.2.5/sage_gpu/sage_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/sage_gpu/sage_model_gpu.py` & `fmldk-1.2.5/sage_gpu/sage_model_gpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,63 @@
 def GumbelSample(a, b, n_samples=1):
     dist = tfd.Gumbel(loc=a, scale=b)
     return tf.reduce_mean(tf.stop_gradient(dist.sample(sample_shape=n_samples)), axis=0)
 
 def min_power_of_2(x):
     return m.ceil(m.log2(x))
 
+# Quantile Risk Metric (MSE & MAE Metrics are available out of the box in tf)
+class q_risk(tf.keras.metrics.Metric):
+    def __init__(self, name='q_risk', q=[0.5], **kwargs):
+        super(q_risk, self).__init__(name=name, **kwargs)
+        self.q = q
+        self.qrisk = self.add_weight(name='qrisk_' + str(q), initializer='zeros')
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+
+        n_quantiles = y_pred.shape.as_list()[-1]
+        assert len(self.q) == n_quantiles
+
+        qr = 0
+        for q, qr_quantile in zip(range(n_quantiles), self.q):
+            qr += self.q_risk_function(y_true, y_pred[:, :, q:q + 1], qr_quantile)
+
+        if sample_weight is not None:
+            raise ValueError("Weighted q-risk not implemented.")
+            #sample_weight = tf.cast(sample_weight, self.dtype)
+            #sample_weight = tf.broadcast_to(sample_weight, values.shape)
+            #values = tf.multiply(values, sample_weight)
+
+        self.qrisk.assign_add(tf.reduce_mean(qr))
+
+    def q_risk_function(self, y_true, y_pred, qr_quantile):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+        qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+            tf.cast(0, tf.float32), (y_pred - y_true))
+        qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+        return qr_scaled
+
+    def result(self):
+        return self.qrisk
+
+
+def q_risk_function(y_true, y_pred, qr_quantile):
+    y_true = tf.cast(y_true, tf.float32)
+    y_pred = tf.cast(y_pred, tf.float32)
+
+    qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+        tf.cast(0, tf.float32), (y_pred - y_true))
+    qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+    return qr_scaled
+
 
 # Model Class - Dense Transformer w/ Variable Selection
 
 # Positional Encoding
 
 def get_angles(pos, i, d_model):
     angle_rates = 1 / np.power(10000, (2 * (i//2)) / np.float32(d_model))
@@ -1120,15 +1169,17 @@
                       model_prefix,
                       logdir,
                       opt,
                       clipnorm,
                       min_delta,
                       shuffle,
                       deterministic,
-                      use_metric_for_convergence):
+                      use_metric_for_convergence,
+                      val_fraction,
+                      val_batch_size):
     """
      train_dataset, test_dataset: tf.data.Dataset iterator for train & test datasets 
      loss_type: One of ['Point','Quantile','Normal','Poisson','Negbin']
      loss_function: One of the supported loss functions in loss library
      metric: 'MAE' or 'MSE' 
      max_epochs: Max. training epochs
      min_epochs: Min. Training epochs
@@ -1181,17 +1232,67 @@
                     loss = loss_function(y_train, [o, wts])
                 else:
                     loss = loss_function(y_train, o)                                   
             else:
                 raise ValueError("Invalid loss_type specified!")
         grads = tape.gradient(loss, model.trainable_variables)
         optimizer.apply_gradients((grad, var) for (grad, var) in zip(grads, model.trainable_variables) if grad is not None)
+
         return loss, o
 
+    @tf.function
     def teststep(model, x_test, y_test, scale, wts, training):
+
+        o, s, f = model(x_test, training=training)
+        out_len = tf.shape(s)[1]
+        s_dim = tf.shape(scale)[-1]
+
+        if loss_type in ['Normal', 'Negbin']:
+            if s_dim == 1:
+                if weighted_training:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], [s, wts])
+                else:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], s)
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                if weighted_training:
+                    loss = loss_function(y_test * s_std + s_mean, [s, wts])
+                else:
+                    loss = loss_function(y_test * s_std + s_mean, s)
+        elif loss_type in ['Tweedie', 'Poisson']:
+            if s_dim == 1:
+                if weighted_training:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], [o * scale[:, -out_len:, :], wts])
+                else:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], o * scale[:, -out_len:, :])
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                if weighted_training:
+                    loss = loss_function(y_test * s_std + s_mean, [o * s_std + s_mean, wts])
+                else:
+                    loss = loss_function(y_test * s_std + s_mean, o * s_std + s_mean)
+        elif loss_type in ['Point']:
+            if weighted_training:
+                loss = loss_function(y_test, [o, wts])
+            else:
+                loss = loss_function(y_test, o)
+        elif loss_type in ['Quantile']:
+            if weighted_training:
+                loss = loss_function(y_test, [o, wts])
+            else:
+                loss = loss_function(y_test, o)
+        else:
+            raise ValueError("Invalid loss_type specified!")
+
+        return loss, o
+
+
+    def valstep(model, x_test, y_test, scale, wts, training):
         out_len = y_test.shape.as_list()[1]
         s_dim = scale.shape.as_list()[-1]
         hist_len = x_test.shape.as_list()[1] - out_len
         
         if s_dim == 1:
             scale_mean = scale[:,-1:,-1]
         else:
@@ -1299,54 +1400,99 @@
             else:
                 s_mean = scale[:, -out_len:, 0:1]
                 s_std = scale[:, -out_len:, 1:2]
                 y_true_rescaled = y_true * s_std + s_mean
                 y_pred_rescaled = y_pred
 
         return y_true_rescaled, y_pred_rescaled
+
+    @tf.function
+    def validation_metric(y_true_rescaled, y_pred_rescaled):
+
+        val_loss = 0
+
+        if metric == 'MAE':
+            if loss_type in ['Quantile']:
+                n_quantiles = y_pred_rescaled.shape.as_list()[-1]
+                for q in range(n_quantiles):
+                    val_loss += tf.reduce_mean(tf.abs(tf.subtract(y_true_rescaled, y_pred_rescaled[:, :, q:q + 1])))
+            else:
+                val_loss = tf.reduce_mean(tf.abs(tf.subtract(y_true_rescaled, y_pred_rescaled)))
+
+        elif metric == 'MSE':
+            if loss_type in ['Quantile']:
+                n_quantiles = y_pred_rescaled.shape.as_list()[-1]
+                for q in range(n_quantiles):
+                    val_loss += tf.reduce_mean(tf.square(tf.subtract(y_true_rescaled, y_pred_rescaled[:, :, q:q + 1])))
+            else:
+                val_loss = tf.reduce_mean(tf.squared(tf.subtract(y_true_rescaled, y_pred_rescaled)))
+
+        elif isinstance(metric, list):
+            if loss_type in ['Quantile']:
+                n_quantiles = y_pred_rescaled.shape.as_list()[-1]
+                assert len(metric) == n_quantiles
+                for q, qr_quantile in zip(range(n_quantiles), metric):
+                    val_loss += q_risk_function(y_true_rescaled, y_pred_rescaled[:, :, q:q + 1], qr_quantile)
+            else:
+                raise ValueError(" q-risk metric not defined for non-quantile loss functions")
+
+        return val_loss
        
     # training specific vars
     if opt is None:
         optimizer = tf.keras.optimizers.Nadam(learning_rate=learning_rate)
     else:
         optimizer = opt
         optimizer.learning_rate=learning_rate
         
     if clipnorm is None:
         pass
     else:
-        optimizer.global_clipnorm = clipnorm
+        optimizer.clipnorm = clipnorm
+        #optimizer.global_clipnorm = clipnorm
        
     print("lr: ",optimizer.learning_rate.numpy())
     
     # model loss & metric
     train_loss_avg = tf.keras.metrics.Mean('train_loss', dtype=tf.float32)
     test_loss_avg = tf.keras.metrics.Mean('test_loss', dtype=tf.float32)
+    val_loss_avg = tf.keras.metrics.Mean('val_loss', dtype=tf.float32)
 
     if metric == 'MAE':  
         train_metric = tf.keras.metrics.MeanAbsoluteError('train_mae')
         test_metric = tf.keras.metrics.MeanAbsoluteError('test_mae')
+        val_metric = tf.keras.metrics.MeanAbsoluteError('val_mae')
+
     elif metric == 'MSE':
         train_metric = tf.keras.metrics.MeanSquaredError('train_mse')
         test_metric = tf.keras.metrics.MeanSquaredError('test_mse')
+        val_metric = tf.keras.metrics.MeanSquaredError('val_mse')
+
+    elif isinstance(metric, list):
+        train_metric = q_risk(name='train_qrisk', q=metric)
+        test_metric = q_risk(name='test_qrisk', q=metric)
+        val_metric = q_risk(name='val_qrisk', q=metric)
+
     else:
         raise ValueError("{}: Not a Supported Metric".format(metric))
             
     #logging
     train_log_dir = str(logdir).rstrip('/') +'/train'
     test_log_dir = str(logdir).rstrip('/')+'/test'
     train_summary_writer = tf.summary.create_file_writer(train_log_dir)
     test_summary_writer = tf.summary.create_file_writer(test_log_dir)
         
     # hold results
     train_loss_results = []
     train_metric_results = []
     test_loss_results = []
     test_metric_results = []
-        
+    val_loss_results = []
+    val_metric_results = []
+
     # initialize model tracking vars
     
     columns_dict_file = model_prefix + '_col_index_dict.pkl'
     with open(columns_dict_file, 'wb') as f:
         pickle.dump(model.col_index_dict, f)
 
     vocab_dict_file = model_prefix + '_vocab_dict.pkl'
@@ -1402,14 +1548,15 @@
        
       # concat
       x_train = tf.concat(x_train, axis=0)
       y_train = tf.concat(y_train, axis=0)
       train_scale = tf.concat(train_scale, axis=0)
       train_wts = tf.concat(train_wts, axis=0)
       print("Training Samples Gathered: ", x_train.shape[0])
+      print("Unique Ids in Trainset: ", len(np.unique(x_train[:, -1, 0])))
       
       print("prefetching test samples ... ")
       x_test = []
       y_test = []
       test_scale = []
       test_wts = []
 
@@ -1421,128 +1568,144 @@
 
       # concat
       x_test = tf.concat(x_test, axis=0)
       y_test = tf.concat(y_test, axis=0)
       test_scale = tf.concat(test_scale, axis=0)
       test_wts = tf.concat(test_wts, axis=0)
       print("Test Samples Gathered: ", x_test.shape[0])
+      print("Unique Ids in Trainset: ", len(np.unique(x_test[:, -1, 0])))
+
+      # sample for oos test -- 10% of test
+      val_samples = int(x_test.shape.as_list()[0] * val_fraction)
+      val_indices = tf.range(start=0, limit=tf.shape(x_test)[0], dtype=tf.int32)
+      val_shuffled_indices = tf.random.shuffle(val_indices)[:val_samples]
+      x_val = tf.gather(x_test, val_shuffled_indices)
+      y_val = tf.gather(y_test, val_shuffled_indices)
+      val_scale = tf.gather(test_scale, val_shuffled_indices)
+      val_wts = tf.gather(test_wts, val_shuffled_indices)
+      print("OOS Samples Gathered: ", x_val.shape[0])
+      print("Unique Ids in OOS set: ", len(np.unique(x_val[:, -1, 0])))
         
-      #num_train_batches = int(x_train.shape[0]//train_batch_size)
-      #num_test_batches = int(x_test.shape[0]//test_batch_size)
-       
+
       # chained tf.data.pipeline
       trainset = tf.data.Dataset.from_tensor_slices((x_train, y_train, train_scale, train_wts))
       trainset = trainset.shuffle(buffer_size=int(x_train.shape[0]), reshuffle_each_iteration=shuffle)
-      trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
-      trainset = trainset.prefetch(buffer_size = tf.data.AUTOTUNE)
+      trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=True, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
+      trainset = trainset.prefetch(buffer_size=tf.data.AUTOTUNE)
         
       testset = tf.data.Dataset.from_tensor_slices((x_test, y_test, test_scale, test_wts))
-      testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=False)
+      testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=shuffle)
       testset = testset.batch(batch_size=test_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
-      testset = testset.prefetch(buffer_size = tf.data.AUTOTUNE)
+      testset = testset.prefetch(buffer_size=tf.data.AUTOTUNE)
+
+      valset = tf.data.Dataset.from_tensor_slices((x_val, y_val, val_scale, val_wts))
+      valset = valset.batch(batch_size=int(val_batch_size), drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
+      valset = valset.prefetch(buffer_size=tf.data.AUTOTUNE)
         
       for epoch in range(max_epochs):
           print("Epoch {}/{}". format(epoch, max_epochs))
-          # shuffle Training data only,if shuffle=True
-          #if shuffle:
-          #  #shuffle_arrays([x_train, y_train, train_scale, train_wts])
-          #  indices = tf.range(start=0, limit=tf.shape(x_train)[0], dtype=tf.int32)
-          #  shuffled_indices = tf.random.shuffle(indices)
-          #  x_train = tf.gather(x_train, shuffled_indices)
-          #  y_train = tf.gather(y_train, shuffled_indices)
-          #  train_scale = tf.gather(train_scale, shuffled_indices)
-          #  train_wts = tf.gather(train_wts, shuffled_indices)
-          #  print("epoch {} first record {}".format(epoch, x_train[0,-1,:]))
-          #  print("epoch {} last record {}".format(epoch, x_train[-1,-1,:]))
-        
+
           for i, (x_batch, y_batch, scale, wts) in enumerate(trainset):
             train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
-            out_len = tf.shape(train_out)[1]
             train_loss_avg.update_state(train_loss)
 
             # rescale io & update metric
             y_true, y_pred = rescale_io(y_batch, train_out, scale)
             train_metric.update_state(y_true, y_pred)
 
-            #if loss_type in ['Normal','Negbin']:
-            #  train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
-            #elif loss_type in ['Point','Tweedie','Poisson']:
-            #  train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out*scale[:,-out_len:,:])
-            #elif loss_type in ['Quantile']:
-            #  train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
-
             with train_summary_writer.as_default():
               tf.summary.scalar('loss', train_loss_avg.result(), step=(i+1)*(epoch+1))
               tf.summary.scalar('accuracy', train_metric.result(), step=(i+1)*(epoch+1))
                 
           for i, (x_batch, y_batch, scale, wts) in enumerate(testset):
-            test_loss, test_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=False)
-            out_len = tf.shape(test_out)[1]
+            test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
             test_loss_avg.update_state(test_loss)
 
             # rescale io
             y_true, y_pred = rescale_io(y_batch, test_out, scale)
             test_metric.update_state(y_true, y_pred)
 
-            #if loss_type in ['Normal','Negbin']:
-            #  test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
-            #elif loss_type in ['Point','Tweedie','Poisson']:
-            #  test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out*scale[:,-out_len:,:])
-            #elif loss_type in ['Quantile']:
-            #  test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
-
             with test_summary_writer.as_default():
               tf.summary.scalar('loss', test_loss_avg.result(), step=(i+1)*(epoch+1))
               tf.summary.scalar('accuracy', test_metric.result(), step=(i+1)*(epoch+1))
 
-          print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch, 
-                                                                                                      train_loss_avg.result().numpy(),
-                                                                                                      test_loss_avg.result().numpy(),
-                                                                                                      train_metric.result().numpy(),
-                                                                                                      test_metric.result().numpy()))
+
+          for i, (x_batch, y_batch, scale, wts) in enumerate(valset):
+            val_loss, val_out = valstep(model, x_batch, y_batch, scale, wts, training=False)
+            val_loss_avg.update_state(val_loss)
+
+            # rescale io
+            y_true, y_pred = rescale_io(y_batch, val_out, scale)
+            val_metric.update_state(y_true, y_pred)
+
+          print("Epoch: {}, train_loss: {}, test_loss: {}, val_loss: {}, train_metric: {}, test_metric: {}, val_metric: {}".format(
+                  epoch,
+                  train_loss_avg.result().numpy(),
+                  test_loss_avg.result().numpy(),
+                  val_loss_avg.result().numpy(),
+                  train_metric.result().numpy(),
+                  test_metric.result().numpy(),
+                  val_metric.result().numpy()))
 
           # record losses & metric in lists
           train_loss_results.append(train_loss_avg.result().numpy())
           train_metric_results.append(train_metric.result().numpy())
           test_loss_results.append(test_loss_avg.result().numpy())
           test_metric_results.append(test_metric.result().numpy())
+          val_loss_results.append(val_loss_avg.result().numpy())
+          val_metric_results.append(val_metric.result().numpy())
 
           # reset states
           train_loss_avg.reset_states()
           train_metric.reset_states()
           test_loss_avg.reset_states()
           test_metric.reset_states()
+          val_loss_avg.reset_states()
+          val_metric.reset_states()
 
           # Save Model
           model_path = model_prefix + '_' + str(epoch) 
           model_list.append(model_path)
-          
+
           if epoch == 0:
-            prev_min_loss = np.min(test_loss_results)
+              prev_min_loss = np.min(test_loss_results)
+              prev_val_loss = np.min(val_loss_results)
           else:
-            prev_min_loss = np.min(test_loss_results[:-1])
+              prev_min_loss = np.min(test_loss_results[:-1])
+              prev_val_loss = np.min(val_loss_results[:-1])
+
           current_min_loss = np.min(test_loss_results)
           delta = current_min_loss - prev_min_loss
 
+          current_min_val_loss = np.min(val_loss_results)
+          val_delta = current_min_val_loss - prev_val_loss
+
           if use_metric_for_convergence:
               # decide on convergence on the basis of both loss & metric
-              save_condition = ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta) and (test_metric_results[epoch] == np.min(test_metric_results))) or (epoch == 0)
+              save_condition = ((test_loss_results[-1] == np.min(test_loss_results)) and (val_loss_results[-1] == np.min(val_loss_results)) and (-delta > min_delta) and (val_metric_results[-1] == np.min(val_metric_results))) or (epoch == 0)
           else:
               # decide on convergence on the basis of loss only
-              save_condition = ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0)
+              save_condition = ((test_loss_results[-1] == np.min(test_loss_results)) and (val_loss_results[-1] == np.min(val_loss_results)) and (-delta > min_delta)) or (epoch == 0)
 
           print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
+
           # track & save best model
           if save_condition:
               best_model = model_path
               tf.keras.models.save_model(model, model_path)
               # reset time_since_improvement
               time_since_improvement = 0
           else:
               time_since_improvement += 1
+              train_loss_results.pop()
+              test_loss_results.pop()
+              val_loss_results.pop()
+              train_metric_results.pop()
+              test_metric_results.pop()
+              val_metric_results.pop()
 
           model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
           print("Best Model: ", best_model)
           
           # model avg. use ema after each epoch
           #if use_ema:
           #      optimizer.finalize_variable_values(model.trainable_variables)
@@ -1561,64 +1724,54 @@
               model_tracker_file.close()
               break
 
           # write after each epoch
           model_tracker_file.flush()
     
     else:
+
       # Use random, dynamic samples from generator 
       for epoch in range(max_epochs):
-          print("Epoch {}/{}". format(epoch, max_epochs)) 
+
+          print("Epoch {}/{}". format(epoch, max_epochs))
           for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
               if step > train_steps_per_epoch:
                   break
               else:
                   train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
-                  out_len = tf.shape(train_out)[1]
                   train_loss_avg.update_state(train_loss)
 
                   # rescale io & update metric
                   y_true, y_pred = rescale_io(y_batch, train_out, scale)
                   train_metric.update_state(y_true, y_pred)
 
-                  #if loss_type in ['Normal','Negbin']:
-                  #    train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
-                  #elif loss_type in ['Point','Tweedie','Poisson']:
-                  #    train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out*scale[:,-out_len:,:])
-                  #elif loss_type in ['Quantile']:
-                  #    train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
-
                   with train_summary_writer.as_default():
                       tf.summary.scalar('loss', train_loss_avg.result(), step=(step+1)*(epoch+1))
                       tf.summary.scalar('accuracy', train_metric.result(), step=(step+1)*(epoch+1))
 
           for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
               if step > test_steps_per_epoch:
                   break
               else:
                   test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
-                  out_len = tf.shape(test_out)[1]
                   test_loss_avg.update_state(test_loss)
 
                   # rescale io
                   y_true, y_pred = rescale_io(y_batch, test_out, scale)
                   test_metric.update_state(y_true, y_pred)
 
-                  #if loss_type in ['Normal','Negbin']:
-                  #    test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
-                  #elif loss_type in ['Point','Tweedie','Poisson']:
-                  #    test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out*scale[:,-out_len:,:])
-                  #elif loss_type in ['Quantile']:
-                  #    test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
-
                   with test_summary_writer.as_default():
                       tf.summary.scalar('loss', test_loss_avg.result(), step=(step+1)*(epoch+1))
                       tf.summary.scalar('accuracy', test_metric.result(), step=(step+1)*(epoch+1))
 
-          print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch, train_loss_avg.result().numpy(), test_loss_avg.result().numpy(), train_metric.result().numpy(), test_metric.result().numpy()))
+          print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
+                                                                                                     train_loss_avg.result().numpy(),
+                                                                                                     test_loss_avg.result().numpy(),
+                                                                                                     train_metric.result().numpy(),
+                                                                                                     test_metric.result().numpy()))
 
           # record losses & metric in lists
           train_loss_results.append(train_loss_avg.result().numpy())
           train_metric_results.append(train_metric.result().numpy())
           test_loss_results.append(test_loss_avg.result().numpy())
           test_metric_results.append(test_metric.result().numpy())
 
@@ -1637,28 +1790,32 @@
           else:
             prev_min_loss = np.min(test_loss_results[:-1])
           current_min_loss = np.min(test_loss_results)
           delta = current_min_loss - prev_min_loss
 
           if use_metric_for_convergence:
               # decide on convergence on the basis of both loss & metric
-              save_condition = ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta) and (test_metric_results[epoch] == np.min(test_metric_results))) or (epoch == 0)
+              save_condition = ((test_loss_results[-1] == np.min(test_loss_results)) and (-delta > min_delta) and (test_metric_results[-1] == np.min(test_metric_results))) or (epoch == 0)
           else:
               # decide on convergence on the basis of loss only
-              save_condition = ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0)
+              save_condition = ((test_loss_results[-1] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0)
 
           print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
           # track & save best model
           if save_condition:
               best_model = model_path
               tf.keras.models.save_model(model, model_path)
               # reset time_since_improvement
               time_since_improvement = 0
           else:
               time_since_improvement += 1
+              train_loss_results.pop()
+              test_loss_results.pop()
+              train_metric_results.pop()
+              test_metric_results.pop()
 
           model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
           print("Best Model: ", best_model)
             
           # model avg. use ema after each epoch
           #if use_ema:
           #  optimizer.finalize_variable_values(model.trainable_variables)
@@ -1860,35 +2017,37 @@
                                   self.num_quantiles,
                                   self.dropout_rate)
         
     def train(self, 
               train_dataset, 
               test_dataset,
               loss_function, 
-              metric, 
-              learning_rate,
-              max_epochs, 
-              min_epochs,
-              prefill_buffers,
-              num_train_samples,
-              num_test_samples,
-              train_batch_size,
-              test_batch_size,
-              train_steps_per_epoch,
-              test_steps_per_epoch,
-              patience,
-              weighted_training,
-              model_prefix,
-              logdir,
+              metric='MSE',
+              learning_rate=0.0001,
+              max_epochs=100,
+              min_epochs=10,
+              prefill_buffers=True,
+              num_train_samples=500000,
+              num_test_samples=50000,
+              train_batch_size=64,
+              test_batch_size=128,
+              train_steps_per_epoch=200,
+              test_steps_per_epoch=100,
+              patience=5,
+              weighted_training=False,
+              model_prefix='./sage_model',
+              logdir='/tmp/sage_logs',
               load_model=None,
               opt=None,
               clipnorm=None,
               min_delta=0.0001,
               shuffle=True,
-              use_metric_for_convergence=False):
+              use_metric_for_convergence=False,
+              val_fraction=0.2,
+              val_batch_size=2048):
         
         if load_model is None:
             # Initialize Weights
             for x,y,s,w in train_dataset.take(1):
                 self.model(x[0:2], training=False)
                 #print(x[0:2,-1:,:])
                 #print(self.model.layers[0].get_weights())
@@ -1924,15 +2083,17 @@
                                           model_prefix,
                                           logdir,
                                           opt,
                                           clipnorm,
                                           min_delta,
                                           shuffle,
                                           self.allow_deterministic_ops,
-                                          use_metric_for_convergence )
+                                          use_metric_for_convergence,
+                                          val_fraction,
+                                          val_batch_size)
         return best_model
     
     def load(self, model_path):
         tf.keras.backend.clear_session()
         self.model = tf.keras.models.load_model(model_path)
         
     def infer(self, inputs):
```

### Comparing `fmldk-1.2.4/sage_gpu/sage_model_gpu_v1.2.3.py` & `fmldk-1.2.5/sage/sage_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# Databricks notebook source
+#!/usr/bin/env python
+# coding: utf-8
+
+
 import numpy as np
 import math as m
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import shutil
 import pickle
@@ -58,14 +61,63 @@
 def GumbelSample(a, b, n_samples=1):
     dist = tfd.Gumbel(loc=a, scale=b)
     return tf.reduce_mean(tf.stop_gradient(dist.sample(sample_shape=n_samples)), axis=0)
 
 def min_power_of_2(x):
     return m.ceil(m.log2(x))
 
+# q-risk metric
+class q_risk(tf.keras.metrics.Metric):
+    def __init__(self, name='q_risk', q=[0.5], **kwargs):
+        super(q_risk, self).__init__(name=name, **kwargs)
+        self.q = q
+        self.qrisk = self.add_weight(name='qrisk_' + str(q), initializer='zeros')
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+
+        n_quantiles = y_pred.shape.as_list()[-1]
+        assert len(self.q) == n_quantiles
+
+        qr = 0
+        for q, qr_quantile in zip(range(n_quantiles), self.q):
+            qr += self.q_risk_function(y_true, y_pred[:, :, q:q + 1], qr_quantile)
+
+        if sample_weight is not None:
+            raise ValueError("sample weighted q-risk not implemented")
+            #sample_weight = tf.cast(sample_weight, self.dtype)
+            #sample_weight = tf.broadcast_to(sample_weight, values.shape)
+            #values = tf.multiply(values, sample_weight)
+
+        self.qrisk.assign_add(tf.reduce_mean(qr))
+
+    def q_risk_function(self, y_true, y_pred, qr_quantile):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+        qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+            tf.cast(0, tf.float32), (y_pred - y_true))
+        qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+        return qr_scaled
+
+    def result(self):
+        return self.qrisk
+
+
+def q_risk_function(y_true, y_pred, qr_quantile):
+    y_true = tf.cast(y_true, tf.float32)
+    y_pred = tf.cast(y_pred, tf.float32)
+
+    qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+        tf.cast(0, tf.float32), (y_pred - y_true))
+    qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+    return qr_scaled
+
 
 # Model Class - Dense Transformer w/ Variable Selection
 
 # Positional Encoding
 
 def get_angles(pos, i, d_model):
     angle_rates = 1 / np.power(10000, (2 * (i//2)) / np.float32(d_model))
@@ -854,15 +906,16 @@
        
         if self.loss_fn in ['Point','Quantile','Tweedie','Poisson']:
             return out, scale, static_weights, decoder_weights
         else:
             return out, parameters, static_weights, decoder_weights
 
 
-# SageTransformer Wrapper
+
+# SAGE Wrapper
 
 class SageTransformer_Model(tf.keras.Model):
     def __init__(self,
                  col_index_dict,
                  vocab_dict,
                  num_layers,
                  num_heads,
@@ -1092,226 +1145,370 @@
             o, s, s_wts, f_wts = self.model([decoder_vars_list, mask, scale], training=training)
 
         # Retain period-wise importance
         bs = tf.shape(f_wts)[0]
         f_wts = tf.reshape(f_wts, [bs*(self.f_len), -1])
               
         return o, s, ([stat_cols_ordered_list,future_cols_ordered_list], [s_wts, f_wts])
-    
-    
+
+
 def SageTransformer_Train(model,
-                      target_index,
-                      train_dataset, 
-                      test_dataset, 
-                      loss_type,
-                      loss_function, 
-                      metric, 
-                      learning_rate,
-                      max_epochs, 
-                      min_epochs,
-                      prefill_buffers,
-                      num_train_samples,
-                      num_test_samples,
-                      train_batch_size,
-                      test_batch_size,
-                      train_steps_per_epoch,
-                      test_steps_per_epoch,
-                      patience,
-                      weighted_training,
-                      model_prefix,
-                      logdir,
-                      opt,
-                      clipnorm,
-                      min_delta,
-                      shuffle,
-                      deterministic):
+                          target_index,
+                          train_dataset,
+                          test_dataset,
+                          loss_type,
+                          loss_function,
+                          metric,
+                          learning_rate,
+                          max_epochs,
+                          min_epochs,
+                          prefill_buffers,
+                          num_train_samples,
+                          num_test_samples,
+                          train_batch_size,
+                          test_batch_size,
+                          train_steps_per_epoch,
+                          test_steps_per_epoch,
+                          patience,
+                          weighted_training,
+                          model_prefix,
+                          logdir,
+                          opt,
+                          clipnorm,
+                          min_delta,
+                          shuffle,
+                          deterministic,
+                          use_metric_for_convergence,
+                          val_fraction,
+                          val_batch_size):
     """
-     train_dataset, test_dataset: tf.data.Dataset iterator for train & test datasets 
+     train_dataset, test_dataset: tf.data.Dataset iterator for train & test datasets
      loss_type: One of ['Point','Quantile','Normal','Poisson','Negbin']
      loss_function: One of the supported loss functions in loss library
-     metric: 'MAE' or 'MSE' 
+     metric: 'MAE' or 'MSE'
      max_epochs: Max. training epochs
      min_epochs: Min. Training epochs
-     *_steps_per_epoch: batches per epoch 
+     *_steps_per_epoch: batches per epoch
      weighted_training: True/False
      model_prefix: relative or absolute model path with a prefix for a model name
      logdir: tensorflow training logs for tensorboard
-        
+
     """
-   
+
     @tf.function
     def trainstep(model, optimizer, x_train, y_train, scale, wts, training):
         with tf.GradientTape() as tape:
             o, s, f = model(x_train, training=training)
             out_len = tf.shape(s)[1]
             s_dim = tf.shape(scale)[-1]
-            if loss_type in ['Normal','Negbin']:
+            if loss_type in ['Normal', 'Negbin']:
                 if s_dim == 1:
                     if weighted_training:
-                        loss = loss_function(y_train*scale[:,-out_len:,:], [s, wts])
+                        loss = loss_function(y_train * scale[:, -out_len:, :], [s, wts])
                     else:
-                        loss = loss_function(y_train*scale[:,-out_len:,:], s)
+                        loss = loss_function(y_train * scale[:, -out_len:, :], s)
                 else:
-                    s_mean = scale[:,-out_len:,0:1]
-                    s_std = scale[:,-out_len:,1:2]
+                    s_mean = scale[:, -out_len:, 0:1]
+                    s_std = scale[:, -out_len:, 1:2]
                     if weighted_training:
-                        loss = loss_function(y_train*s_std + s_mean, [s, wts])
+                        loss = loss_function(y_train * s_std + s_mean, [s, wts])
                     else:
-                        loss = loss_function(y_train*s_std + s_mean, s)
-            elif loss_type in ['Tweedie','Poisson']:
+                        loss = loss_function(y_train * s_std + s_mean, s)
+            elif loss_type in ['Tweedie', 'Poisson']:
                 if s_dim == 1:
-                    if weighted_training:                               
-                        loss = loss_function(y_train*scale[:,-out_len:,:], [o*scale[:,-out_len:,:], wts])
+                    if weighted_training:
+                        loss = loss_function(y_train * scale[:, -out_len:, :], [o * scale[:, -out_len:, :], wts])
                     else:
-                        loss = loss_function(y_train*scale[:,-out_len:,:], o*scale[:,-out_len:,:])
+                        loss = loss_function(y_train * scale[:, -out_len:, :], o * scale[:, -out_len:, :])
                 else:
-                    s_mean = scale[:,-out_len:,0:1]
-                    s_std = scale[:,-out_len:,1:2]
+                    s_mean = scale[:, -out_len:, 0:1]
+                    s_std = scale[:, -out_len:, 1:2]
                     if weighted_training:
-                        loss = loss_function(y_train*s_std + s_mean, [o*s_std + s_mean, wts])
+                        loss = loss_function(y_train * s_std + s_mean, [o * s_std + s_mean, wts])
                     else:
-                        loss = loss_function(y_train*s_std + s_mean, o*s_std + s_mean)
+                        loss = loss_function(y_train * s_std + s_mean, o * s_std + s_mean)
             elif loss_type in ['Point']:
-                    if weighted_training:                               
-                        loss = loss_function(y_train, [o, wts])
-                    else:
-                        loss = loss_function(y_train, o)
+                if weighted_training:
+                    loss = loss_function(y_train, [o, wts])
+                else:
+                    loss = loss_function(y_train, o)
             elif loss_type in ['Quantile']:
-                if weighted_training:                               
+                if weighted_training:
                     loss = loss_function(y_train, [o, wts])
                 else:
-                    loss = loss_function(y_train, o)                                   
+                    loss = loss_function(y_train, o)
             else:
                 raise ValueError("Invalid loss_type specified!")
         grads = tape.gradient(loss, model.trainable_variables)
-        optimizer.apply_gradients((grad, var) for (grad, var) in zip(grads, model.trainable_variables) if grad is not None)
+        optimizer.apply_gradients(
+            (grad, var) for (grad, var) in zip(grads, model.trainable_variables) if grad is not None)
+
         return loss, o
 
+    @tf.function
     def teststep(model, x_test, y_test, scale, wts, training):
+
+        o, s, f = model(x_test, training=training)
+        out_len = tf.shape(s)[1]
+        s_dim = tf.shape(scale)[-1]
+
+        if loss_type in ['Normal', 'Negbin']:
+            if s_dim == 1:
+                if weighted_training:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], [s, wts])
+                else:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], s)
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                if weighted_training:
+                    loss = loss_function(y_test * s_std + s_mean, [s, wts])
+                else:
+                    loss = loss_function(y_test * s_std + s_mean, s)
+        elif loss_type in ['Tweedie', 'Poisson']:
+            if s_dim == 1:
+                if weighted_training:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], [o * scale[:, -out_len:, :], wts])
+                else:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], o * scale[:, -out_len:, :])
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                if weighted_training:
+                    loss = loss_function(y_test * s_std + s_mean, [o * s_std + s_mean, wts])
+                else:
+                    loss = loss_function(y_test * s_std + s_mean, o * s_std + s_mean)
+        elif loss_type in ['Point']:
+            if weighted_training:
+                loss = loss_function(y_test, [o, wts])
+            else:
+                loss = loss_function(y_test, o)
+        elif loss_type in ['Quantile']:
+            if weighted_training:
+                loss = loss_function(y_test, [o, wts])
+            else:
+                loss = loss_function(y_test, o)
+        else:
+            raise ValueError("Invalid loss_type specified!")
+
+        return loss, o
+
+    def valstep(model, x_test, y_test, scale, wts, training):
         out_len = y_test.shape.as_list()[1]
         s_dim = scale.shape.as_list()[-1]
         hist_len = x_test.shape.as_list()[1] - out_len
-        
+
         if s_dim == 1:
-            scale_mean = scale[:,-1:,-1]
+            scale_mean = scale[:, -1:, -1]
         else:
-            scale_mean = scale[:,-1:,0]
-            scale_std = scale[:,-1:,1]
-            
+            scale_mean = scale[:, -1:, 0]
+            scale_std = scale[:, -1:, 1]
+
         # recursive predict
         output = []
-        
+
         for i in range(out_len):
             o, s, f = model(x_test, training=training)
             infer_arr = x_test.numpy()
             # update target
-            if loss_type in ['Normal','Negbin']:
-                output.append(s[:,i:i+1,:])
+            if loss_type in ['Normal', 'Negbin']:
+                output.append(s[:, i:i + 1, :])
                 if s_dim == 1:
-                    infer_arr[:,hist_len+i:hist_len+i+1,target_index] = o[:,i:i+1,0]/scale_mean
+                    infer_arr[:, hist_len + i:hist_len + i + 1, target_index] = o[:, i:i + 1, 0] / scale_mean
                 else:
-                    infer_arr[:,hist_len+i:hist_len+i+1,target_index] = np.nan_to_num((o[:,i:i+1,0] - scale_mean)/scale_std)
+                    infer_arr[:, hist_len + i:hist_len + i + 1, target_index] = np.nan_to_num(
+                        (o[:, i:i + 1, 0] - scale_mean) / scale_std)
 
-            elif loss_type in ['Point','Quantile','Tweedie','Poisson']:
-                output.append(o[:,i:i+1,:])
-                infer_arr[:,hist_len+i:hist_len+i+1,target_index] = o[:,i:i+1,0] # append q=0.5 value assuming it's the first in sequence
+            elif loss_type in ['Point', 'Quantile', 'Tweedie', 'Poisson']:
+                output.append(o[:, i:i + 1, :])
+                infer_arr[:, hist_len + i:hist_len + i + 1, target_index] = o[:, i:i + 1,
+                                                                            0]  # append q=0.5 value assuming it's the first in sequence
 
             # feedback updated hist + fh tensor
-            x_test = tf.convert_to_tensor(np.char.decode(infer_arr.astype(np.bytes_), 'UTF-8'), dtype=tf.string) 
-        
+            x_test = tf.convert_to_tensor(np.char.decode(infer_arr.astype(np.bytes_), 'UTF-8'), dtype=tf.string)
+
         o = tf.concat(output, axis=1)
-        if loss_type in ['Normal','Negbin']:
+        if loss_type in ['Normal', 'Negbin']:
             if s_dim == 1:
                 if weighted_training:
-                    loss = loss_function(y_test*scale[:,-out_len:,:], [s, wts])
+                    loss = loss_function(y_test * scale[:, -out_len:, :], [s, wts])
                 else:
-                    loss = loss_function(y_test*scale[:,-out_len:,:], s)
+                    loss = loss_function(y_test * scale[:, -out_len:, :], s)
             else:
-                s_mean = scale[:,-out_len:,0:1]
-                s_std = scale[:,-out_len:,1:2]
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
                 if weighted_training:
-                    loss = loss_function(y_test*s_std + s_mean, [s, wts])
+                    loss = loss_function(y_test * s_std + s_mean, [s, wts])
                 else:
-                    loss = loss_function(y_test*s_std + s_mean, s)
-        elif loss_type in ['Tweedie','Poisson']:
+                    loss = loss_function(y_test * s_std + s_mean, s)
+        elif loss_type in ['Tweedie', 'Poisson']:
             if s_dim == 1:
-                if weighted_training:                               
-                    loss = loss_function(y_test*scale[:,-out_len:,:], [o*scale[:,-out_len:,:], wts])
+                if weighted_training:
+                    loss = loss_function(y_test * scale[:, -out_len:, :], [o * scale[:, -out_len:, :], wts])
                 else:
-                    loss = loss_function(y_test*scale[:,-out_len:,:], o*scale[:,-out_len:,:])
+                    loss = loss_function(y_test * scale[:, -out_len:, :], o * scale[:, -out_len:, :])
             else:
-                s_mean = scale[:,-out_len:,0:1]
-                s_std = scale[:,-out_len:,1:2]
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
                 if weighted_training:
-                    loss = loss_function(y_test*s_std + s_mean, [o*s_std + s_mean, wts])
+                    loss = loss_function(y_test * s_std + s_mean, [o * s_std + s_mean, wts])
                 else:
-                    loss = loss_function(y_test*s_std + s_mean, o*s_std + s_mean)
+                    loss = loss_function(y_test * s_std + s_mean, o * s_std + s_mean)
         elif loss_type in ['Point']:
-            if weighted_training:                               
+            if weighted_training:
                 loss = loss_function(y_test, [o, wts])
             else:
                 loss = loss_function(y_test, o)
         elif loss_type in ['Quantile']:
-            if weighted_training:                               
+            if weighted_training:
                 loss = loss_function(y_test, [o, wts])
             else:
-                loss = loss_function(y_test, o)                                   
+                loss = loss_function(y_test, o)
         else:
-            raise ValueError("Invalid loss_type specified!")        
+            raise ValueError("Invalid loss_type specified!")
         return loss, o
-       
+
+    def rescale_io(y_true, y_pred, scale):
+
+        out_len = y_true.shape.as_list()[1]
+        s_dim = scale.shape.as_list()[-1]
+
+        if loss_type in ['Point', 'Tweedie', 'Poisson']:
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred * scale[:, -out_len:, :]
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                y_pred_rescaled = y_pred * s_std + s_mean
+
+        elif loss_type in ['Quantile']:
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred * scale[:, -out_len:, :]
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                # rescale each quantile
+                n_quantiles = y_pred.shape.as_list()[-1]
+                y_list = []
+                for q in range(n_quantiles):
+                    y = y_pred[:, :, q:q + 1] * s_std + s_mean
+                    y_list.append(y)
+                y_pred_rescaled = tf.concat(y_list, axis=-1)
+
+        elif loss_type in ['Normal', 'Negbin']:
+            # predictions are already rescaled
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                y_pred_rescaled = y_pred
+
+        return y_true_rescaled, y_pred_rescaled
+
+    @tf.function
+    def validation_metric(y_true_rescaled, y_pred_rescaled):
+
+        val_loss = 0
+
+        if metric == 'MAE':
+            if loss_type in ['Quantile']:
+                n_quantiles = y_pred_rescaled.shape.as_list()[-1]
+                for q in range(n_quantiles):
+                    val_loss += tf.reduce_mean(tf.abs(tf.subtract(y_true_rescaled, y_pred_rescaled[:, :, q:q + 1])))
+            else:
+                val_loss = tf.reduce_mean(tf.abs(tf.subtract(y_true_rescaled, y_pred_rescaled)))
+
+        elif metric == 'MSE':
+            if loss_type in ['Quantile']:
+                n_quantiles = y_pred_rescaled.shape.as_list()[-1]
+                for q in range(n_quantiles):
+                    val_loss += tf.reduce_mean(tf.square(tf.subtract(y_true_rescaled, y_pred_rescaled[:, :, q:q + 1])))
+            else:
+                val_loss = tf.reduce_mean(tf.squared(tf.subtract(y_true_rescaled, y_pred_rescaled)))
+
+        elif isinstance(metric, list):
+            if loss_type in ['Quantile']:
+                n_quantiles = y_pred_rescaled.shape.as_list()[-1]
+                assert len(metric) == n_quantiles
+                for q, qr_quantile in zip(range(n_quantiles), metric):
+                    val_loss += q_risk_function(y_true_rescaled, y_pred_rescaled[:, :, q:q + 1], qr_quantile)
+            else:
+                raise ValueError(" q-risk metric not defined for non-quantile loss functions")
+
+        return val_loss
+
     # training specific vars
     if opt is None:
         optimizer = tf.keras.optimizers.Nadam(learning_rate=learning_rate)
     else:
         optimizer = opt
-        optimizer.learning_rate=learning_rate
-        
+        optimizer.learning_rate = learning_rate
+
     if clipnorm is None:
         pass
     else:
-        optimizer.global_clipnorm = clipnorm
-       
-    print("lr: ",optimizer.learning_rate.numpy())
-    
+        optimizer.clipnorm = clipnorm
+        # optimizer.global_clipnorm = clipnorm
+
+    print("lr: ", optimizer.learning_rate.numpy())
+
     # model loss & metric
     train_loss_avg = tf.keras.metrics.Mean('train_loss', dtype=tf.float32)
     test_loss_avg = tf.keras.metrics.Mean('test_loss', dtype=tf.float32)
+    val_loss_avg = tf.keras.metrics.Mean('val_loss', dtype=tf.float32)
 
-    if metric == 'MAE':  
+    if metric == 'MAE':
         train_metric = tf.keras.metrics.MeanAbsoluteError('train_mae')
         test_metric = tf.keras.metrics.MeanAbsoluteError('test_mae')
+        val_metric = tf.keras.metrics.MeanAbsoluteError('val_mae')
+
     elif metric == 'MSE':
         train_metric = tf.keras.metrics.MeanSquaredError('train_mse')
         test_metric = tf.keras.metrics.MeanSquaredError('test_mse')
+        val_metric = tf.keras.metrics.MeanSquaredError('val_mse')
+
+    elif isinstance(metric, list):
+        train_metric = q_risk(name='train_qrisk', q=metric)
+        test_metric = q_risk(name='test_qrisk', q=metric)
+        val_metric = q_risk(name='val_qrisk', q=metric)
+
     else:
         raise ValueError("{}: Not a Supported Metric".format(metric))
-            
-    #logging
-    train_log_dir = str(logdir).rstrip('/') +'/train'
-    test_log_dir = str(logdir).rstrip('/')+'/test'
+
+    # logging
+    train_log_dir = str(logdir).rstrip('/') + '/train'
+    test_log_dir = str(logdir).rstrip('/') + '/test'
     train_summary_writer = tf.summary.create_file_writer(train_log_dir)
     test_summary_writer = tf.summary.create_file_writer(test_log_dir)
-        
+
     # hold results
     train_loss_results = []
     train_metric_results = []
     test_loss_results = []
     test_metric_results = []
-        
+    val_loss_results = []
+    val_metric_results = []
+
     # initialize model tracking vars
-    
+
     columns_dict_file = model_prefix + '_col_index_dict.pkl'
     with open(columns_dict_file, 'wb') as f:
         pickle.dump(model.col_index_dict, f)
 
     vocab_dict_file = model_prefix + '_vocab_dict.pkl'
     with open(vocab_dict_file, 'wb') as f:
         pickle.dump(model.vocab_dict, f)
-    
+
     model_tracker_file = open(model_prefix + '_tracker.txt', mode='w', encoding='utf-8')
 
     model_tracker_file.write('Feature Weighted ConvTransformer Training started with following Model Parameters ... \n')
     model_tracker_file.write('----------------------------------------\n')
     model_tracker_file.write('num_layers ' + str(model.num_layers) + '\n')
     model_tracker_file.write('num_heads ' + str(model.num_heads) + '\n')
     model_tracker_file.write('d_model ' + str(model.d_model) + '\n')
@@ -1319,294 +1516,352 @@
     model_tracker_file.write('max_inp_len ' + str(model.max_inp_len) + '\n')
     model_tracker_file.write('dropout_rate ' + str(model.dropout_rate) + '\n')
     model_tracker_file.write('col_index_dict path ' + str(columns_dict_file) + '\n')
     model_tracker_file.write('vocab_dict path ' + str(vocab_dict_file) + '\n')
     model_tracker_file.write('----------------------------------------\n')
     model_tracker_file.write('\n')
     model_tracker_file.flush()
-    
+
     model_list = []
     best_model = None
     time_since_improvement = 0
-    
+
     ######################################################### train loop -- pre-filled tensor buffers
-    
+
     def shuffle_arrays(arrays, set_seed=-1):
-      """Shuffles arrays in-place, in the same order, along axis=0
-      arrays : List of NumPy arrays.
-      set_seed : Seed value if int >= 0, else seed is random.
-      """
-      assert all(len(arr) == len(arrays[0]) for arr in arrays)
-      seed = np.random.randint(0, 2**(32 - 1) - 1) if set_seed < 0 else set_seed
-      for arr in arrays:
-        rstate = np.random.RandomState(seed)
-        rstate.shuffle(arr)
-    
+        """Shuffles arrays in-place, in the same order, along axis=0
+        arrays : List of NumPy arrays.
+        set_seed : Seed value if int >= 0, else seed is random.
+        """
+        assert all(len(arr) == len(arrays[0]) for arr in arrays)
+        seed = np.random.randint(0, 2 ** (32 - 1) - 1) if set_seed < 0 else set_seed
+        for arr in arrays:
+            rstate = np.random.RandomState(seed)
+            rstate.shuffle(arr)
+
     if prefill_buffers:
-      print("prefetching training samples ... ")
-      
-      x_train = []
-      y_train = []
-      train_scale = []
-      train_wts = []
-   
-      for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
-        x_train.append(x_batch)
-        y_train.append(y_batch)
-        train_scale.append(scale)
-        train_wts.append(wts)
-       
-      # concat
-      x_train = tf.concat(x_train, axis=0)
-      y_train = tf.concat(y_train, axis=0)
-      train_scale = tf.concat(train_scale, axis=0)
-      train_wts = tf.concat(train_wts, axis=0)
-      print("Training Samples Gathered: ", x_train.shape[0])
-      
-      print("prefetching test samples ... ")
-      x_test = []
-      y_test = []
-      test_scale = []
-      test_wts = []
-
-      for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
-        x_test.append(x_batch)
-        y_test.append(y_batch)
-        test_scale.append(scale)
-        test_wts.append(wts)
-
-      # concat
-      x_test = tf.concat(x_test, axis=0)
-      y_test = tf.concat(y_test, axis=0)
-      test_scale = tf.concat(test_scale, axis=0)
-      test_wts = tf.concat(test_wts, axis=0)
-      print("Test Samples Gathered: ", x_test.shape[0])
-        
-      #num_train_batches = int(x_train.shape[0]//train_batch_size)
-      #num_test_batches = int(x_test.shape[0]//test_batch_size)
-       
-      # chained tf.data.pipeline
-      trainset = tf.data.Dataset.from_tensor_slices((x_train, y_train, train_scale, train_wts))
-      trainset = trainset.shuffle(buffer_size=int(x_train.shape[0]), reshuffle_each_iteration=shuffle)
-      trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
-      trainset = trainset.prefetch(buffer_size = tf.data.AUTOTUNE)
-        
-      testset = tf.data.Dataset.from_tensor_slices((x_test, y_test, test_scale, test_wts))
-      testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=False)
-      testset = testset.batch(batch_size=test_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
-      testset = testset.prefetch(buffer_size = tf.data.AUTOTUNE)
-        
-      for epoch in range(max_epochs):
-          print("Epoch {}/{}". format(epoch, max_epochs))
-          # shuffle Training data only,if shuffle=True
-          #if shuffle:
-          #  #shuffle_arrays([x_train, y_train, train_scale, train_wts])
-          #  indices = tf.range(start=0, limit=tf.shape(x_train)[0], dtype=tf.int32)
-          #  shuffled_indices = tf.random.shuffle(indices)
-          #  x_train = tf.gather(x_train, shuffled_indices)
-          #  y_train = tf.gather(y_train, shuffled_indices)
-          #  train_scale = tf.gather(train_scale, shuffled_indices)
-          #  train_wts = tf.gather(train_wts, shuffled_indices)
-          #  print("epoch {} first record {}".format(epoch, x_train[0,-1,:]))
-          #  print("epoch {} last record {}".format(epoch, x_train[-1,-1,:]))
-        
-          for i, (x_batch, y_batch, scale, wts) in enumerate(trainset):
-            train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
-            out_len = tf.shape(train_out)[1]
-            train_loss_avg.update_state(train_loss)
-            if loss_type in ['Normal','Negbin']:
-              train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
-            elif loss_type in ['Point','Tweedie','Poisson']:
-              train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out*scale[:,-out_len:,:])
-            elif loss_type in ['Quantile']:
-              train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
-            with train_summary_writer.as_default():
-              tf.summary.scalar('loss', train_loss_avg.result(), step=(i+1)*(epoch+1))
-              tf.summary.scalar('accuracy', train_metric.result(), step=(i+1)*(epoch+1))
-                
-          for i, (x_batch, y_batch, scale, wts) in enumerate(testset):
-            test_loss, test_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=False)
-            out_len = tf.shape(test_out)[1]
-            test_loss_avg.update_state(test_loss)
-            if loss_type in ['Normal','Negbin']:
-              test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
-            elif loss_type in ['Point','Tweedie','Poisson']:
-              test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out*scale[:,-out_len:,:])
-            elif loss_type in ['Quantile']:
-              test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
-            with test_summary_writer.as_default():
-              tf.summary.scalar('loss', test_loss_avg.result(), step=(i+1)*(epoch+1))
-              tf.summary.scalar('accuracy', test_metric.result(), step=(i+1)*(epoch+1))
-
-          print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch, 
-                                                                                                      train_loss_avg.result().numpy(),
-                                                                                                      test_loss_avg.result().numpy(),
-                                                                                                      train_metric.result().numpy(),
-                                                                                                      test_metric.result().numpy()))
-
-          # record losses & metric in lists
-          train_loss_results.append(train_loss_avg.result().numpy())
-          train_metric_results.append(train_metric.result().numpy())
-          test_loss_results.append(test_loss_avg.result().numpy())
-          test_metric_results.append(test_metric.result().numpy())
-
-          # reset states
-          train_loss_avg.reset_states()
-          train_metric.reset_states()
-          test_loss_avg.reset_states()
-          test_metric.reset_states()
-
-          # Save Model
-          model_path = model_prefix + '_' + str(epoch) 
-          model_list.append(model_path)
-          
-          if epoch == 0:
-            prev_min_loss = np.min(test_loss_results)
-          else:
-            prev_min_loss = np.min(test_loss_results[:-1])
-          current_min_loss = np.min(test_loss_results)
-          delta = current_min_loss - prev_min_loss
-
-          print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
-          # track & save best model
-          if ((test_loss_results[epoch]==np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
-              best_model = model_path
-              tf.keras.models.save_model(model, model_path)
-              # reset time_since_improvement
-              time_since_improvement = 0
-          else:
-              time_since_improvement += 1
+        print("prefetching training samples ... ")
 
-          model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
-          print("Best Model: ", best_model)
-          
-          # model avg. use ema after each epoch
-          #if use_ema:
-          #      optimizer.finalize_variable_values(model.trainable_variables)
-            
-          # remove older models
-          if len(model_list)>patience:
-              for m in model_list[:-patience]:
-                  if m != best_model:
-                      try:
-                          shutil.rmtree(m)
-                      except:
-                          pass
-
-          if (time_since_improvement > patience) and (epoch > min_epochs):
-              print("Terminating Training. Best Model path: {}".format(best_model))
-              model_tracker_file.close()
-              break
+        # get batch size
+        batch_size = 0
+        for x, y, s, w in train_dataset.take(1):
+            batch_size = int(x.shape[0])
+
+        x_train = []
+        y_train = []
+        train_scale = []
+        train_wts = []
+
+        for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
+            x_train.append(x_batch)
+            y_train.append(y_batch)
+            train_scale.append(scale)
+            train_wts.append(wts)
+            if (step + 1) * batch_size >= num_train_samples:
+                break
+
+        # concat
+        x_train = tf.concat(x_train, axis=0)
+        y_train = tf.concat(y_train, axis=0)
+        train_scale = tf.concat(train_scale, axis=0)
+        train_wts = tf.concat(train_wts, axis=0)
+        print("Training Samples Gathered: ", x_train.shape[0])
+        print("Unique Ids in Trainset: ", len(np.unique(x_train[:, -1, 0])))
+
+        print("prefetching test samples ... ")
+        x_test = []
+        y_test = []
+        test_scale = []
+        test_wts = []
+
+        for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
+            x_test.append(x_batch)
+            y_test.append(y_batch)
+            test_scale.append(scale)
+            test_wts.append(wts)
+            if (step + 1) * batch_size >= num_test_samples:
+                break
+
+        # concat
+        x_test = tf.concat(x_test, axis=0)
+        y_test = tf.concat(y_test, axis=0)
+        test_scale = tf.concat(test_scale, axis=0)
+        test_wts = tf.concat(test_wts, axis=0)
+        print("Test Samples Gathered: ", x_test.shape[0])
+        print("Unique Ids in Trainset: ", len(np.unique(x_test[:, -1, 0])))
+
+        # sample for oos test -- 10% of test
+        val_samples = int(x_test.shape.as_list()[0] * val_fraction)
+        val_indices = tf.range(start=0, limit=tf.shape(x_test)[0], dtype=tf.int32)
+        val_shuffled_indices = tf.random.shuffle(val_indices)[:val_samples]
+        x_val = tf.gather(x_test, val_shuffled_indices)
+        y_val = tf.gather(y_test, val_shuffled_indices)
+        val_scale = tf.gather(test_scale, val_shuffled_indices)
+        val_wts = tf.gather(test_wts, val_shuffled_indices)
+        print("OOS Samples Gathered: ", x_val.shape[0])
+        print("Unique Ids in OOS set: ", len(np.unique(x_val[:, -1, 0])))
+
+        # chained tf.data.pipeline
+        trainset = tf.data.Dataset.from_tensor_slices((x_train, y_train, train_scale, train_wts))
+        trainset = trainset.shuffle(buffer_size=int(x_train.shape[0]), reshuffle_each_iteration=shuffle)
+        trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=True, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
+        trainset = trainset.prefetch(buffer_size=tf.data.AUTOTUNE)
+
+        testset = tf.data.Dataset.from_tensor_slices((x_test, y_test, test_scale, test_wts))
+        testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=shuffle)
+        testset = testset.batch(batch_size=test_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
+        testset = testset.prefetch(buffer_size=tf.data.AUTOTUNE)
+
+        valset = tf.data.Dataset.from_tensor_slices((x_val, y_val, val_scale, val_wts))
+        valset = valset.batch(batch_size=int(val_batch_size), drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
+        valset = valset.prefetch(buffer_size=tf.data.AUTOTUNE)
+
+        for epoch in range(max_epochs):
+            print("Epoch {}/{}".format(epoch, max_epochs))
+
+            for i, (x_batch, y_batch, scale, wts) in enumerate(trainset):
+                train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
+                train_loss_avg.update_state(train_loss)
+
+                # rescale io & update metric
+                y_true, y_pred = rescale_io(y_batch, train_out, scale)
+                train_metric.update_state(y_true, y_pred)
+
+                with train_summary_writer.as_default():
+                    tf.summary.scalar('loss', train_loss_avg.result(), step=(i + 1) * (epoch + 1))
+                    tf.summary.scalar('accuracy', train_metric.result(), step=(i + 1) * (epoch + 1))
+
+            for i, (x_batch, y_batch, scale, wts) in enumerate(testset):
+                test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
+                test_loss_avg.update_state(test_loss)
+
+                # rescale io
+                y_true, y_pred = rescale_io(y_batch, test_out, scale)
+                test_metric.update_state(y_true, y_pred)
+
+                with test_summary_writer.as_default():
+                    tf.summary.scalar('loss', test_loss_avg.result(), step=(i + 1) * (epoch + 1))
+                    tf.summary.scalar('accuracy', test_metric.result(), step=(i + 1) * (epoch + 1))
+
+            for i, (x_batch, y_batch, scale, wts) in enumerate(valset):
+                val_loss, val_out = valstep(model, x_batch, y_batch, scale, wts, training=False)
+                val_loss_avg.update_state(val_loss)
+
+                # rescale io
+                y_true, y_pred = rescale_io(y_batch, val_out, scale)
+                val_metric.update_state(y_true, y_pred)
+
+            print(
+                "Epoch: {}, train_loss: {}, test_loss: {}, val_loss: {}, train_metric: {}, test_metric: {}, val_metric: {}".format(
+                    epoch,
+                    train_loss_avg.result().numpy(),
+                    test_loss_avg.result().numpy(),
+                    val_loss_avg.result().numpy(),
+                    train_metric.result().numpy(),
+                    test_metric.result().numpy(),
+                    val_metric.result().numpy()))
+
+            # record losses & metric in lists
+            train_loss_results.append(train_loss_avg.result().numpy())
+            train_metric_results.append(train_metric.result().numpy())
+            test_loss_results.append(test_loss_avg.result().numpy())
+            test_metric_results.append(test_metric.result().numpy())
+            val_loss_results.append(val_loss_avg.result().numpy())
+            val_metric_results.append(val_metric.result().numpy())
+
+            # reset states
+            train_loss_avg.reset_states()
+            train_metric.reset_states()
+            test_loss_avg.reset_states()
+            test_metric.reset_states()
+            val_loss_avg.reset_states()
+            val_metric.reset_states()
+
+            # Save Model
+            model_path = model_prefix + '_' + str(epoch)
+            model_list.append(model_path)
+
+            if epoch == 0:
+                prev_min_loss = np.min(test_loss_results)
+                prev_val_loss = np.min(val_loss_results)
+            else:
+                prev_min_loss = np.min(test_loss_results[:-1])
+                prev_val_loss = np.min(val_loss_results[:-1])
+
+            current_min_loss = np.min(test_loss_results)
+            delta = current_min_loss - prev_min_loss
+
+            current_min_val_loss = np.min(val_loss_results)
+            val_delta = current_min_val_loss - prev_val_loss
+
+            if use_metric_for_convergence:
+                # decide on convergence on the basis of both loss & metric
+                save_condition = ((test_loss_results[-1] == np.min(test_loss_results)) and (
+                            val_loss_results[-1] == np.min(val_loss_results)) and (-delta > min_delta) and (
+                                              val_metric_results[-1] == np.min(val_metric_results))) or (epoch == 0)
+            else:
+                # decide on convergence on the basis of loss only
+                save_condition = ((test_loss_results[-1] == np.min(test_loss_results)) and (
+                            val_loss_results[-1] == np.min(val_loss_results)) and (-delta > min_delta)) or (epoch == 0)
+
+            print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
+
+            # track & save best model
+            if save_condition:
+                best_model = model_path
+                tf.keras.models.save_model(model, model_path)
+                # reset time_since_improvement
+                time_since_improvement = 0
+            else:
+                time_since_improvement += 1
+                train_loss_results.pop()
+                test_loss_results.pop()
+                val_loss_results.pop()
+                train_metric_results.pop()
+                test_metric_results.pop()
+                val_metric_results.pop()
+
+            model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
+            print("Best Model: ", best_model)
+
+            # model avg. use ema after each epoch
+            # if use_ema:
+            #      optimizer.finalize_variable_values(model.trainable_variables)
+
+            # remove older models
+            if len(model_list) > patience:
+                for m in model_list[:-patience]:
+                    if m != best_model:
+                        try:
+                            shutil.rmtree(m)
+                        except:
+                            pass
+
+            if (time_since_improvement > patience) and (epoch > min_epochs):
+                print("Terminating Training. Best Model path: {}".format(best_model))
+                model_tracker_file.close()
+                break
+
+            # write after each epoch
+            model_tracker_file.flush()
 
-          # write after each epoch
-          model_tracker_file.flush()
-    
     else:
-      # Use random, dynamic samples from generator 
-      for epoch in range(max_epochs):
-          print("Epoch {}/{}". format(epoch, max_epochs)) 
-          for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
-              if step > train_steps_per_epoch:
-                  break
-              else:
-                  train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
-                  out_len = tf.shape(train_out)[1]
-                  train_loss_avg.update_state(train_loss)
-                  if loss_type in ['Normal','Negbin']:
-                      train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
-                  elif loss_type in ['Point','Tweedie','Poisson']:
-                      train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out*scale[:,-out_len:,:])
-                  elif loss_type in ['Quantile']:
-                      train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
-                  with train_summary_writer.as_default():
-                      tf.summary.scalar('loss', train_loss_avg.result(), step=(step+1)*(epoch+1))
-                      tf.summary.scalar('accuracy', train_metric.result(), step=(step+1)*(epoch+1))
-
-          for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
-              if step > test_steps_per_epoch:
-                  break
-              else:
-                  test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
-                  out_len = tf.shape(test_out)[1]
-                  test_loss_avg.update_state(test_loss)
-                  if loss_type in ['Normal','Negbin']:
-                      test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
-                  elif loss_type in ['Point','Tweedie','Poisson']:
-                      test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out*scale[:,-out_len:,:])
-                  elif loss_type in ['Quantile']:
-                      test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
-                  with test_summary_writer.as_default():
-                      tf.summary.scalar('loss', test_loss_avg.result(), step=(step+1)*(epoch+1))
-                      tf.summary.scalar('accuracy', test_metric.result(), step=(step+1)*(epoch+1))
-
-          print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch, 
-                                                                                                      train_loss_avg.result().numpy(),
-                                                                                                      test_loss_avg.result().numpy(),
-                                                                                                      train_metric.result().numpy(),
-                                                                                                      test_metric.result().numpy()))
-
-          # record losses & metric in lists
-          train_loss_results.append(train_loss_avg.result().numpy())
-          train_metric_results.append(train_metric.result().numpy())
-          test_loss_results.append(test_loss_avg.result().numpy())
-          test_metric_results.append(test_metric.result().numpy())
-
-          # reset states
-          train_loss_avg.reset_states()
-          train_metric.reset_states()
-          test_loss_avg.reset_states()
-          test_metric.reset_states()
-
-          # Save Model
-          model_path = model_prefix + '_' + str(epoch) 
-          model_list.append(model_path)
-          
-          if epoch == 0:
-            prev_min_loss = np.min(test_loss_results)
-          else:
-            prev_min_loss = np.min(test_loss_results[:-1])
-          current_min_loss = np.min(test_loss_results)
-          delta = current_min_loss - prev_min_loss
-         
-          print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
-          # track & save best model
-          if ((test_loss_results[epoch]==np.min(test_loss_results)) and (-delta > min_delta)) or  (epoch == 0):
-              best_model = model_path
-              tf.keras.models.save_model(model, model_path)
-              # reset time_since_improvement
-              time_since_improvement = 0
-          else:
-              time_since_improvement += 1
 
-          model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
-          print("Best Model: ", best_model)
-            
-          # model avg. use ema after each epoch
-          #if use_ema:
-          #  optimizer.finalize_variable_values(model.trainable_variables)
-
-          # remove older models
-          if len(model_list)>patience:
-              for m in model_list[:-patience]:
-                  if m != best_model:
-                      try:
-                          shutil.rmtree(m)
-                      except:
-                          pass
-
-          if (time_since_improvement > patience) and (epoch > min_epochs):
-              print("Terminating Training. Best Model path: {}".format(best_model))
-              model_tracker_file.close()
-              break
+        # Use random, dynamic samples from generator
+        for epoch in range(max_epochs):
+
+            print("Epoch {}/{}".format(epoch, max_epochs))
+            for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
+                if step > train_steps_per_epoch:
+                    break
+                else:
+                    train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
+                    train_loss_avg.update_state(train_loss)
+
+                    # rescale io & update metric
+                    y_true, y_pred = rescale_io(y_batch, train_out, scale)
+                    train_metric.update_state(y_true, y_pred)
+
+                    with train_summary_writer.as_default():
+                        tf.summary.scalar('loss', train_loss_avg.result(), step=(step + 1) * (epoch + 1))
+                        tf.summary.scalar('accuracy', train_metric.result(), step=(step + 1) * (epoch + 1))
+
+            for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
+                if step > test_steps_per_epoch:
+                    break
+                else:
+                    test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
+                    test_loss_avg.update_state(test_loss)
+
+                    # rescale io
+                    y_true, y_pred = rescale_io(y_batch, test_out, scale)
+                    test_metric.update_state(y_true, y_pred)
+
+                    with test_summary_writer.as_default():
+                        tf.summary.scalar('loss', test_loss_avg.result(), step=(step + 1) * (epoch + 1))
+                        tf.summary.scalar('accuracy', test_metric.result(), step=(step + 1) * (epoch + 1))
+
+            print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
+                                                                                                       train_loss_avg.result().numpy(),
+                                                                                                       test_loss_avg.result().numpy(),
+                                                                                                       train_metric.result().numpy(),
+                                                                                                       test_metric.result().numpy()))
+
+            # record losses & metric in lists
+            train_loss_results.append(train_loss_avg.result().numpy())
+            train_metric_results.append(train_metric.result().numpy())
+            test_loss_results.append(test_loss_avg.result().numpy())
+            test_metric_results.append(test_metric.result().numpy())
+
+            # reset states
+            train_loss_avg.reset_states()
+            train_metric.reset_states()
+            test_loss_avg.reset_states()
+            test_metric.reset_states()
+
+            # Save Model
+            model_path = model_prefix + '_' + str(epoch)
+            model_list.append(model_path)
+
+            if epoch == 0:
+                prev_min_loss = np.min(test_loss_results)
+            else:
+                prev_min_loss = np.min(test_loss_results[:-1])
+            current_min_loss = np.min(test_loss_results)
+            delta = current_min_loss - prev_min_loss
+
+            if use_metric_for_convergence:
+                # decide on convergence on the basis of both loss & metric
+                save_condition = ((test_loss_results[-1] == np.min(test_loss_results)) and (-delta > min_delta) and (
+                            test_metric_results[-1] == np.min(test_metric_results))) or (epoch == 0)
+            else:
+                # decide on convergence on the basis of loss only
+                save_condition = ((test_loss_results[-1] == np.min(test_loss_results)) and (-delta > min_delta)) or (
+                            epoch == 0)
+
+            print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
+            # track & save best model
+            if save_condition:
+                best_model = model_path
+                tf.keras.models.save_model(model, model_path)
+                # reset time_since_improvement
+                time_since_improvement = 0
+            else:
+                time_since_improvement += 1
+                train_loss_results.pop()
+                test_loss_results.pop()
+                train_metric_results.pop()
+                test_metric_results.pop()
+
+            model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
+            print("Best Model: ", best_model)
+
+            # model avg. use ema after each epoch
+            # if use_ema:
+            #  optimizer.finalize_variable_values(model.trainable_variables)
+
+            # remove older models
+            if len(model_list) > patience:
+                for m in model_list[:-patience]:
+                    if m != best_model:
+                        try:
+                            shutil.rmtree(m)
+                        except:
+                            pass
+
+            if (time_since_improvement > patience) and (epoch > min_epochs):
+                print("Terminating Training. Best Model path: {}".format(best_model))
+                model_tracker_file.close()
+                break
+
+            # write after each epoch
+            model_tracker_file.flush()
 
-          # write after each epoch
-          model_tracker_file.flush()
-        
     return best_model
-        
+
 
 def SageTransformer_InferRecursive(model, inputs, loss_type, hist_len, f_len, target_index, num_quantiles):
     infer_tensor, scale, id_arr, date_arr = inputs
     s_dim = scale.shape[-1]
     
     if s_dim == 1:
         scale = scale[:,-1:,-1]
@@ -1664,15 +1919,14 @@
         
     # rescale if necessary
     if loss_type in ['Normal','Negbin']:
         output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr), axis=1))
         output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
         output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
     elif loss_type in ['Point','Tweedie','Poisson']:
-        # 
         if s_dim == 1:
             output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr[:,:,0]*scale.reshape(-1,1)), axis=1))
         else:
             output_arr = output_arr[:,:,0]*scale_std.reshape(-1,1) + scale_mean.reshape(-1,1)
             output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1), output_arr), axis=1))
         output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
         output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
@@ -1712,151 +1966,160 @@
     
     print(stat_wts_df.shape, decoder_wts_df.shape)
         
     return forecast_df, stat_wts_df, decoder_wts_df
 
 
 class SageModel:
-    def __init__(self, 
+    def __init__(self,
                  col_index_dict,
                  vocab_dict,
                  num_layers,
                  num_heads,
                  kernel_sizes,
                  d_model,
                  forecast_horizon,
                  max_inp_len,
                  loss_type,
                  num_quantiles,
                  dropout_rate=0.1,
                  seed=None,
                  deterministic_ops=False):
-        
+
         self.col_index_dict = col_index_dict
         self.vocab_dict = vocab_dict
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.kernel_sizes = kernel_sizes
         self.d_model = d_model
         self.forecast_horizon = forecast_horizon
         self.max_inp_len = max_inp_len
         self.loss_type = loss_type
         self.num_quantiles = num_quantiles
         self.dropout_rate = dropout_rate
         self.target_col_name, self.target_index = self.col_index_dict.get('target_index')
         self.seed = seed
         self.allow_deterministic_ops = deterministic_ops
-        
+
     def set_seed(self):
         tf.keras.utils.set_random_seed(self.seed)
         if self.allow_deterministic_ops:
             print("Deterministic Ops enabled.")
             if platform == "linux" or platform == "linux2":
-              print("GPU/CPU Determinism enabled for Linux")
-              os.environ["TF_DETERMINISTIC_OPS"] = "True"
+                print("GPU/CPU Determinism enabled for Linux")
+                os.environ["TF_DETERMINISTIC_OPS"] = "True"
             else:
-              print("GPU/CPU Determinism partially enabled for Windows & Others")
-              os.environ["TF_DETERMINISTIC_OPS"] = "True"
-              os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
+                print("GPU/CPU Determinism partially enabled for Windows & Others")
+                os.environ["TF_DETERMINISTIC_OPS"] = "True"
+                os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
         else:
             print("Deterministic Ops disabled.")
             os.environ["TF_DETERMINISTIC_OPS"] = "False"
-        
+
     def build(self):
         tf.keras.backend.clear_session()
         if self.seed is None:
             print("No seed set for deterministic weights initialization")
         else:
             print("Using seed {} for weights initialization".format(self.seed))
             self.set_seed()
-            
+
         self.model = SageTransformer_Model(self.col_index_dict,
-                                  self.vocab_dict,
-                                  self.num_layers,
-                                  self.num_heads,
-                                  self.kernel_sizes,
-                                  self.d_model,
-                                  self.forecast_horizon,
-                                  self.max_inp_len,
-                                  self.loss_type,
-                                  self.num_quantiles,
-                                  self.dropout_rate)
-        
-    def train(self, 
-              train_dataset, 
+                                           self.vocab_dict,
+                                           self.num_layers,
+                                           self.num_heads,
+                                           self.kernel_sizes,
+                                           self.d_model,
+                                           self.forecast_horizon,
+                                           self.max_inp_len,
+                                           self.loss_type,
+                                           self.num_quantiles,
+                                           self.dropout_rate)
+
+    def train(self,
+              train_dataset,
               test_dataset,
-              loss_function, 
-              metric, 
-              learning_rate,
-              max_epochs, 
-              min_epochs,
-              prefill_buffers,
-              num_train_samples,
-              num_test_samples,
-              train_batch_size,
-              test_batch_size,
-              train_steps_per_epoch,
-              test_steps_per_epoch,
-              patience,
-              weighted_training,
-              model_prefix,
-              logdir,
+              loss_function,
+              metric='MSE',
+              learning_rate=0.0001,
+              max_epochs=100,
+              min_epochs=10,
+              prefill_buffers=True,
+              num_train_samples=500000,
+              num_test_samples=50000,
+              train_batch_size=64,
+              test_batch_size=128,
+              train_steps_per_epoch=200,
+              test_steps_per_epoch=100,
+              patience=5,
+              weighted_training=False,
+              model_prefix='./sage_model',
+              logdir='/tmp/sage_logs',
               load_model=None,
               opt=None,
               clipnorm=None,
               min_delta=0.0001,
-              shuffle=True):
-        
+              shuffle=True,
+              use_metric_for_convergence=False,
+              val_fraction=0.2,
+              val_batch_size=2048):
+
         if load_model is None:
             # Initialize Weights
-            for x,y,s,w in train_dataset.take(1):
+            for x, y, s, w in train_dataset.take(1):
                 self.model(x[0:2], training=False)
-                #print(x[0:2,-1:,:])
-                #print(self.model.layers[0].get_weights())
+                # print(x[0:2,-1:,:])
+                # print(self.model.layers[0].get_weights())
         else:
             # Initialize Weights
-            for x,y,s,w in train_dataset.take(1):
+            for x, y, s, w in train_dataset.take(1):
                 self.model(x[0:2], training=False)
             saved_model = tf.keras.models.load_model(load_model)
             self.model.set_weights(saved_model.get_weights())
             del saved_model
             gc.collect()
             print("Saved model: {} loaded. Continuing training ...".format(load_model))
-        
+
         best_model = SageTransformer_Train(self.model,
-                                          self.target_index,    
-                                          train_dataset, 
-                                          test_dataset, 
-                                          self.loss_type,
-                                          loss_function, 
-                                          metric, 
-                                          learning_rate,
-                                          max_epochs, 
-                                          min_epochs,
-                                          prefill_buffers,
-                                          num_train_samples,
-                                          num_test_samples,
-                                          train_batch_size,
-                                          test_batch_size,
-                                          train_steps_per_epoch,
-                                          test_steps_per_epoch,
-                                          patience,
-                                          weighted_training,
-                                          model_prefix,
-                                          logdir,
-                                          opt,
-                                          clipnorm,
-                                          min_delta,
-                                          shuffle,
-                                          self.allow_deterministic_ops)
+                                           self.target_index,
+                                           train_dataset,
+                                           test_dataset,
+                                           self.loss_type,
+                                           loss_function,
+                                           metric,
+                                           learning_rate,
+                                           max_epochs,
+                                           min_epochs,
+                                           prefill_buffers,
+                                           num_train_samples,
+                                           num_test_samples,
+                                           train_batch_size,
+                                           test_batch_size,
+                                           train_steps_per_epoch,
+                                           test_steps_per_epoch,
+                                           patience,
+                                           weighted_training,
+                                           model_prefix,
+                                           logdir,
+                                           opt,
+                                           clipnorm,
+                                           min_delta,
+                                           shuffle,
+                                           self.allow_deterministic_ops,
+                                           use_metric_for_convergence,
+                                           val_fraction,
+                                           val_batch_size)
         return best_model
-    
+
     def load(self, model_path):
         tf.keras.backend.clear_session()
         self.model = tf.keras.models.load_model(model_path)
-        
+
     def infer(self, inputs):
-        forecast, stat_wts_df, decoder_wts_df = SageTransformer_InferRecursive(self.model, inputs, self.loss_type, self.max_inp_len, self.forecast_horizon, self.target_index, self.num_quantiles)
-        
+        forecast, stat_wts_df, decoder_wts_df = SageTransformer_InferRecursive(self.model, inputs, self.loss_type,
+                                                                               self.max_inp_len, self.forecast_horizon,
+                                                                               self.target_index, self.num_quantiles)
+
         return forecast, [stat_wts_df, decoder_wts_df]
     
     
+
```

### Comparing `fmldk-1.2.4/setup.py` & `fmldk-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The directory containing this file
 this_directory = Path(__file__).parent
 long_description  = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="fmldk",
-    version="1.2.4",
+    version="1.2.5",
     description="Forecast ML library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rahul Sinha",
     author_email="rahul.sinha@unilever.com",
     packages=["sage","sage_gpu","tfr","tft","tft_gpu","stctn","ctfr","ctfrv2","ctfrv2_gpu","eda"],
     include_package_data=True,
```

### Comparing `fmldk-1.2.4/stctn/stctn_data.py` & `fmldk-1.2.5/stctn/stctn_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/stctn/stctn_losses.py` & `fmldk-1.2.5/stctn/stctn_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/stctn/stctn_losses_bkp.py` & `fmldk-1.2.5/stctn/stctn_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/stctn/stctn_models.py` & `fmldk-1.2.5/stctn/stctn_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_data.py` & `fmldk-1.2.5/tfr/tfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_data_v0.1.11.py` & `fmldk-1.2.5/tfr/tfr_data_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_data_v0.1.12.py` & `fmldk-1.2.5/tfr/tfr_data_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_data_v0.1.14.py` & `fmldk-1.2.5/tfr/tfr_data_v0.1.14.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_data_v0.1.15.py` & `fmldk-1.2.5/tfr/tfr_data_v0.1.15.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_data_v0.1.16.py` & `fmldk-1.2.5/tfr/tfr_data_v0.1.16.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_data_v0.1.18.py` & `fmldk-1.2.5/tfr/tfr_data_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_data_v0.1.21.py` & `fmldk-1.2.5/tfr/tfr_data_v0.1.21.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_local_block_sparse_attention.py` & `fmldk-1.2.5/tfr/tfr_local_block_sparse_attention.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_local_block_sparse_attention_v0.1.10.py` & `fmldk-1.2.5/tfr/tfr_local_block_sparse_attention_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_local_block_sparse_attention_v0.1.12.py` & `fmldk-1.2.5/tfr/tfr_local_block_sparse_attention_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_losses.py` & `fmldk-1.2.5/tfr/tfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_losses_bkp.py` & `fmldk-1.2.5/tfr/tfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_models.py` & `fmldk-1.2.5/tfr/tfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_models_v0.1.10.py` & `fmldk-1.2.5/tfr/tfr_models_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_models_v0.1.11.py` & `fmldk-1.2.5/tfr/tfr_models_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_models_v0.1.23.py` & `fmldk-1.2.5/tfr/tfr_models_v0.1.23.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tfr/tfr_models_v0.1.31.py` & `fmldk-1.2.5/tfr/tfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_data.py` & `fmldk-1.2.5/tft/tft_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_data_old.py` & `fmldk-1.2.5/tft/tft_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_data_v1.1.3.py` & `fmldk-1.2.5/tft/tft_data_v1.1.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_data_v1.1.7.py` & `fmldk-1.2.5/tft/tft_data_v1.1.7.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_global_scaled_data.py` & `fmldk-1.2.5/tft/tft_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_losses.py` & `fmldk-1.2.5/tft/tft_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_model.py` & `fmldk-1.2.5/ctfrv2_gpu/ctfrv2_model_gpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[1]:
-
 
 import numpy as np
 import math as m
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import shutil
 import pickle
 import absl.logging
 absl.logging.set_verbosity(absl.logging.ERROR)
 import pandas as pd
 import gc
 import os
+from sys import platform
+
 
 # Distribution Sampling functions
 
 # negbin
 def negbin_sample(mu, alpha, n_samples=1):
     tol = 1e-5
     r = 1.0 / alpha
@@ -59,16 +59,62 @@
     return tf.reduce_mean(dist.sample(sample_shape=n_samples), axis=0)
 
 # Gumbel
 def GumbelSample(a, b, n_samples=1):
     dist = tfd.Gumbel(loc=a, scale=b)
     return tf.reduce_mean(tf.stop_gradient(dist.sample(sample_shape=n_samples)), axis=0)
 
+# Quantile Risk Metric (MSE & MAE Metrics are available out of the box in tf)
+class q_risk(tf.keras.metrics.Metric):
+    def __init__(self, name='q_risk', q=[0.5], **kwargs):
+        super(q_risk, self).__init__(name=name, **kwargs)
+        self.q = q
+        self.qrisk = self.add_weight(name='qrisk_' + str(q), initializer='zeros')
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+
+        n_quantiles = y_pred.shape.as_list()[-1]
+        assert len(self.q) == n_quantiles
+
+        qr = 0
+        for q, qr_quantile in zip(range(n_quantiles), self.q):
+            qr += self.q_risk_function(y_true, y_pred[:, :, q:q + 1], qr_quantile)
+
+        if sample_weight is not None:
+            raise ValueError("Weighted q-risk not implemented.")
+            #sample_weight = tf.cast(sample_weight, self.dtype)
+            #sample_weight = tf.broadcast_to(sample_weight, values.shape)
+            #values = tf.multiply(values, sample_weight)
+
+        self.qrisk.assign_add(tf.reduce_mean(qr))
+
+    def q_risk_function(self, y_true, y_pred, qr_quantile):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+        qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+            tf.cast(0, tf.float32), (y_pred - y_true))
+        qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+        return qr_scaled
+
+    def result(self):
+        return self.qrisk
+
+
+def q_risk_function(y_true, y_pred, qr_quantile):
+    y_true = tf.cast(y_true, tf.float32)
+    y_pred = tf.cast(y_pred, tf.float32)
+
+    qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+        tf.cast(0, tf.float32), (y_pred - y_true))
+    qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
 
-# In[3]:
+    return qr_scaled
 
 
 # Self-Attention
 def ScaledDotProductAttention(q, k, v, causal_mask, padding_mask):
     matmul_qk = tf.matmul(q, k, transpose_b=True)  # (..., seq_len_q, seq_len_k)
     dk = tf.cast(tf.shape(k)[-1], tf.float32)
     scaled_attention_logits = matmul_qk / tf.math.sqrt(dk)
@@ -1081,59 +1127,61 @@
 
         # Retain period-wise importance
         bs = tf.shape(p_wts)[0]
         p_wts = tf.reshape(p_wts, [bs * self.hist_len, -1])
         f_wts = tf.reshape(f_wts, [bs * self.f_len, -1])
         
         return o, s, ([stat_cols_ordered_list,past_cols_ordered_list,future_cols_ordered_list], [s_wts, p_wts, f_wts])
-    
-    
-def TFT_Train(model, 
-              train_dataset, 
-              test_dataset, 
+
+
+def TFT_Train(model,
+              train_dataset,
+              test_dataset,
               loss_type,
-              loss_function, 
-              metric, 
+              loss_function,
+              metric,
               learning_rate,
-              max_epochs, 
+              max_epochs,
               min_epochs,
               prefill_buffers,
               num_train_samples,
               num_test_samples,
               train_batch_size,
               test_batch_size,
               train_steps_per_epoch,
               test_steps_per_epoch,
               patience,
               weighted_training,
               model_prefix,
               logdir,
-              opt=None,
-              clipnorm=None,
-              min_delta=0.0001,
-              shuffle=True):
+              opt,
+              clipnorm,
+              min_delta,
+              shuffle,
+              deterministic):
     """
      train_dataset, test_dataset: tf.data.Dataset iterator for train & test datasets 
      loss_type: One of ['Point','Quantile','Normal','Poisson','Negbin']
      loss_function: One of the supported loss functions in loss library
      metric: 'MAE' or 'MSE' 
      max_epochs: Max. training epochs
      min_epochs: Min. Training epochs
      *_steps_per_epoch: batches per epoch 
      weighted_training: True/False
      model_prefix: relative or absolute model path with a prefix for a model name
      logdir: tensorflow training logs for tensorboard
-        
+
     """
+
     @tf.function
     def trainstep(model, optimizer, x_train, y_train, scale, wts, training):
         with tf.GradientTape() as tape:
             o, s, f = model(x_train, training=training)
-            out_len = s.shape.as_list()[1]  # tf.shape(s)[1]
-            s_dim = scale.shape.as_list()[-1]  # tf.shape(scale)[-1]
+            out_len = tf.shape(s)[1]
+            s_dim = tf.shape(scale)[-1]
             if loss_type in ['Normal', 'Negbin']:
                 if s_dim == 1:
                     if weighted_training:
                         loss = loss_function(y_train * scale[:, -out_len:, :], [s, wts])
                     else:
                         loss = loss_function(y_train * scale[:, -out_len:, :], s)
                 else:
@@ -1142,40 +1190,41 @@
                     if weighted_training:
                         loss = loss_function(y_train * s_std + s_mean, [s, wts])
                     else:
                         loss = loss_function(y_train * s_std + s_mean, s)
             elif loss_type in ['Tweedie', 'Poisson']:
                 if s_dim == 1:
                     if weighted_training:
-                        loss = loss_function(y_train*scale[:, -out_len:, :], [o*scale[:, -out_len:, :], wts])
+                        loss = loss_function(y_train * scale[:, -out_len:, :], [o * scale[:, -out_len:, :], wts])
                     else:
-                        loss = loss_function(y_train*scale[:, -out_len:, :], o*scale[:, -out_len:, :])
+                        loss = loss_function(y_train * scale[:, -out_len:, :], o * scale[:, -out_len:, :])
                 else:
                     s_mean = scale[:, -out_len:, 0:1]
                     s_std = scale[:, -out_len:, 1:2]
                     if weighted_training:
-                        loss = loss_function(y_train*s_std + s_mean, [o*s_std + s_mean, wts])
+                        loss = loss_function(y_train * s_std + s_mean, [o * s_std + s_mean, wts])
                     else:
-                        loss = loss_function(y_train*s_std + s_mean, o*s_std + s_mean)
+                        loss = loss_function(y_train * s_std + s_mean, o * s_std + s_mean)
             elif loss_type in ['Point', 'Binary']:
-                if weighted_training:                               
+                if weighted_training:
                     loss = loss_function(y_train, [o, wts])
                 else:
                     loss = loss_function(y_train, o)
             elif loss_type in ['Quantile']:
-                if weighted_training:                               
+                if weighted_training:
                     loss = loss_function(y_train, [o, wts])
                 else:
-                    loss = loss_function(y_train, o)                                   
+                    loss = loss_function(y_train, o)
             else:
                 raise ValueError("Invalid loss_type specified!")
         grads = tape.gradient(loss, model.trainable_variables)
-        optimizer.apply_gradients((grad, var) for (grad, var) in zip(grads, model.trainable_variables) if grad is not None)
+        optimizer.apply_gradients(
+            (grad, var) for (grad, var) in zip(grads, model.trainable_variables) if grad is not None)
         return loss, o
-    
+
     @tf.function
     def teststep(model, x_test, y_test, scale, wts, training):
         o, s, f = model(x_test, training=training)
         out_len = s.shape.as_list()[1]  # tf.shape(s)[1]
         s_dim = scale.shape.as_list()[-1]  # tf.shape(scale)[-1]
         if loss_type in ['Normal', 'Negbin']:
             if s_dim == 1:
@@ -1190,89 +1239,138 @@
                     loss = loss_function(y_test * s_std + s_mean, [s, wts])
                 else:
                     loss = loss_function(y_test * s_std + s_mean, s)
 
         elif loss_type in ['Tweedie', 'Poisson']:
             if s_dim == 1:
                 if weighted_training:
-                    loss = loss_function(y_test*scale[:, -out_len:, :], [o*scale[:, -out_len:, :], wts])
+                    loss = loss_function(y_test * scale[:, -out_len:, :], [o * scale[:, -out_len:, :], wts])
                 else:
-                    loss = loss_function(y_test*scale[:, -out_len:, :], o*scale[:, -out_len:, :])
+                    loss = loss_function(y_test * scale[:, -out_len:, :], o * scale[:, -out_len:, :])
             else:
                 s_mean = scale[:, -out_len:, 0:1]
                 s_std = scale[:, -out_len:, 1:2]
                 if weighted_training:
-                    loss = loss_function(y_test*s_std + s_mean, [o*s_std + s_mean, wts])
+                    loss = loss_function(y_test * s_std + s_mean, [o * s_std + s_mean, wts])
                 else:
-                    loss = loss_function(y_test*s_std + s_mean, o*s_std + s_mean)
+                    loss = loss_function(y_test * s_std + s_mean, o * s_std + s_mean)
 
         elif loss_type in ['Point', 'Binary']:
-            if weighted_training:                               
+            if weighted_training:
                 loss = loss_function(y_test, [o, wts])
             else:
                 loss = loss_function(y_test, o)
 
         elif loss_type in ['Quantile']:
-            if weighted_training:                               
+            if weighted_training:
                 loss = loss_function(y_test, [o, wts])
             else:
-                loss = loss_function(y_test, o)                                   
+                loss = loss_function(y_test, o)
         else:
-            raise ValueError("Invalid loss_type specified!")        
+            raise ValueError("Invalid loss_type specified!")
         return loss, o
-       
+
+    def rescale_io(y_true, y_pred, scale):
+
+        out_len = y_true.shape.as_list()[1]
+        s_dim = scale.shape.as_list()[-1]
+
+        if loss_type in ['Point', 'Tweedie', 'Poisson']:
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred * scale[:, -out_len:, :]
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                y_pred_rescaled = y_pred * s_std + s_mean
+
+        elif loss_type in ['Quantile']:
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred * scale[:, -out_len:, :]
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                # rescale each quantile
+                n_quantiles = y_pred.shape.as_list()[-1]
+                y_list = []
+                for q in range(n_quantiles):
+                    y = y_pred[:, :, q:q + 1] * s_std + s_mean
+                    y_list.append(y)
+                y_pred_rescaled = tf.concat(y_list, axis=-1)
+
+        elif loss_type in ['Normal', 'Negbin']:
+            # predictions are already rescaled
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                y_pred_rescaled = y_pred
+
+        return y_true_rescaled, y_pred_rescaled
+
     # training specific vars
     if opt is None:
         optimizer = tf.keras.optimizers.Nadam(learning_rate=learning_rate)
     else:
         optimizer = opt
-        optimizer.learning_rate=learning_rate
-    
+        optimizer.learning_rate = learning_rate
+
     if clipnorm is None:
         pass
     else:
-        optimizer.global_clipnorm = clipnorm
-       
-    print("lr: ",optimizer.learning_rate.numpy())
-    
+        optimizer.clipnorm = clipnorm
+
+    print("lr: ", optimizer.learning_rate.numpy())
+
     # model loss & metric
     train_loss_avg = tf.keras.metrics.Mean('train_loss', dtype=tf.float32)
     test_loss_avg = tf.keras.metrics.Mean('test_loss', dtype=tf.float32)
 
-    if metric == 'MAE':  
+    if metric == 'MAE':
         train_metric = tf.keras.metrics.MeanAbsoluteError('train_mae')
         test_metric = tf.keras.metrics.MeanAbsoluteError('test_mae')
+
     elif metric == 'MSE':
         train_metric = tf.keras.metrics.MeanSquaredError('train_mse')
         test_metric = tf.keras.metrics.MeanSquaredError('test_mse')
+
+    elif isinstance(metric, list):
+        train_metric = q_risk(name='train_qrisk', q=metric)
+        test_metric = q_risk(name='test_qrisk', q=metric)
     else:
         raise ValueError("{}: Not a Supported Metric".format(metric))
-            
-    #logging
-    train_log_dir = str(logdir).rstrip('/') +'/train'
-    test_log_dir = str(logdir).rstrip('/')+'/test'
+
+    # logging
+    train_log_dir = str(logdir).rstrip('/') + '/train'
+    test_log_dir = str(logdir).rstrip('/') + '/test'
     train_summary_writer = tf.summary.create_file_writer(train_log_dir)
     test_summary_writer = tf.summary.create_file_writer(test_log_dir)
-        
+
     # hold results
     train_loss_results = []
     train_metric_results = []
     test_loss_results = []
     test_metric_results = []
-        
+
     # initialize model tracking vars
-    
+
     columns_dict_file = model_prefix + '_col_index_dict.pkl'
     with open(columns_dict_file, 'wb') as f:
         pickle.dump(model.col_index_dict, f)
 
     vocab_dict_file = model_prefix + '_vocab_dict.pkl'
     with open(vocab_dict_file, 'wb') as f:
         pickle.dump(model.vocab_dict, f)
-    
+
     model_tracker_file = open(model_prefix + '_tracker.txt', mode='w', encoding='utf-8')
 
     model_tracker_file.write('Feature Weighted Transformer Training started with following Model Parameters ... \n')
     model_tracker_file.write('----------------------------------------\n')
     model_tracker_file.write('num_layers ' + str(model.num_layers) + '\n')
     model_tracker_file.write('num_heads ' + str(model.num_heads) + '\n')
     model_tracker_file.write('d_model ' + str(model.d_model) + '\n')
@@ -1280,38 +1378,32 @@
     model_tracker_file.write('max_inp_len ' + str(model.max_inp_len) + '\n')
     model_tracker_file.write('dropout_rate ' + str(model.dropout_rate) + '\n')
     model_tracker_file.write('col_index_dict path ' + str(columns_dict_file) + '\n')
     model_tracker_file.write('vocab_dict path ' + str(vocab_dict_file) + '\n')
     model_tracker_file.write('----------------------------------------\n')
     model_tracker_file.write('\n')
     model_tracker_file.flush()
-    
+
     model_list = []
     best_model = None
     time_since_improvement = 0
     #####################################################################
 
     if prefill_buffers:
         print("prefetching training samples ... ")
-        # get batch size
-        batch_size = 0
-        for x, y, s, w in train_dataset.take(1):
-            batch_size = int(x.shape[0])
 
         x_train = []
         y_train = []
         train_scale = []
         train_wts = []
         for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
             x_train.append(x_batch)
             y_train.append(y_batch)
             train_scale.append(scale)
             train_wts.append(wts)
-            if (step + 1) * batch_size >= num_train_samples:
-                break
 
         # concat
         x_train = tf.concat(x_train, axis=0)
         y_train = tf.concat(y_train, axis=0)
         train_scale = tf.concat(train_scale, axis=0)
         train_wts = tf.concat(train_wts, axis=0)
         print("Training Samples Gathered: ", x_train.shape[0])
@@ -1322,74 +1414,75 @@
         test_scale = []
         test_wts = []
         for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
             x_test.append(x_batch)
             y_test.append(y_batch)
             test_scale.append(scale)
             test_wts.append(wts)
-            if (step + 1) * batch_size >= num_test_samples:
-                break
 
         # concat
         x_test = tf.concat(x_test, axis=0)
         y_test = tf.concat(y_test, axis=0)
         test_scale = tf.concat(test_scale, axis=0)
         test_wts = tf.concat(test_wts, axis=0)
         print("Test Samples Gathered: ", x_test.shape[0])
 
-        num_train_batches = int(x_train.shape[0] // train_batch_size)
-        num_test_batches = int(x_test.shape[0] // test_batch_size)
+        # chained tf.data.pipeline
+        trainset = tf.data.Dataset.from_tensor_slices((x_train, y_train, train_scale, train_wts))
+        trainset = trainset.shuffle(buffer_size=int(x_train.shape[0]), reshuffle_each_iteration=shuffle)
+        trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=False,
+                                  num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
+        trainset = trainset.prefetch(buffer_size=tf.data.AUTOTUNE)
+
+        testset = tf.data.Dataset.from_tensor_slices((x_test, y_test, test_scale, test_wts))
+        testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=shuffle)
+        testset = testset.batch(batch_size=test_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE,
+                                deterministic=deterministic)
+        testset = testset.prefetch(buffer_size=tf.data.AUTOTUNE)
 
         for epoch in range(max_epochs):
             print("Epoch {}/{}".format(epoch, max_epochs))
-            # shuffle Training data only,if shuffle=True
-            if shuffle:
-                # shuffle_arrays([x_train, y_train, train_scale, train_wts])
-                indices = tf.range(start=0, limit=tf.shape(x_train)[0], dtype=tf.int32)
-                shuffled_indices = tf.random.shuffle(indices)
-                x_train = tf.gather(x_train, shuffled_indices)
-                y_train = tf.gather(y_train, shuffled_indices)
-                train_scale = tf.gather(train_scale, shuffled_indices)
-                train_wts = tf.gather(train_wts, shuffled_indices)
-
-            for i in range(num_train_batches):
-                x_batch = x_train[i * train_batch_size:(i + 1) * train_batch_size]
-                y_batch = y_train[i * train_batch_size:(i + 1) * train_batch_size]
-                scale = train_scale[i * train_batch_size:(i + 1) * train_batch_size]
-                wts = train_wts[i * train_batch_size:(i + 1) * train_batch_size]
+
+            for i, (x_batch, y_batch, scale, wts) in enumerate(trainset):
                 train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
-                out_len = tf.shape(train_out)[1]
                 train_loss_avg.update_state(train_loss)
-                if loss_type in ['Normal', 'Negbin']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out)
-                elif loss_type in ['Point', 'Poisson', 'Tweedie']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
-                elif loss_type in ['Quantile']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
+                # rescale io & update metric
+                y_true, y_pred = rescale_io(y_batch, train_out, scale)
+                train_metric.update_state(y_true, y_pred)
+
+                # if loss_type in ['Normal', 'Negbin']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out)
+                # elif loss_type in ['Point', 'Poisson', 'Tweedie']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
+                # elif loss_type in ['Quantile']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
                 with train_summary_writer.as_default():
-                    tf.summary.scalar('loss', train_loss_avg.result(), step=epoch)
-                    tf.summary.scalar('accuracy', train_metric.result(), step=epoch)
+                    tf.summary.scalar('loss', train_loss_avg.result(), step=(i + 1) * (epoch + 1))
+                    tf.summary.scalar('accuracy', train_metric.result(), step=(i + 1) * (epoch + 1))
 
-            for i in range(num_test_batches):
-                x_batch = x_test[i * train_batch_size:(i + 1) * train_batch_size]
-                y_batch = y_test[i * train_batch_size:(i + 1) * train_batch_size]
-                scale = test_scale[i * train_batch_size:(i + 1) * train_batch_size]
-                wts = test_wts[i * train_batch_size:(i + 1) * train_batch_size]
-                test_loss, test_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=False)
-                out_len = tf.shape(test_out)[1]
+            for i, (x_batch, y_batch, scale, wts) in enumerate(testset):
+                test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
                 test_loss_avg.update_state(test_loss)
-                if loss_type in ['Normal', 'Negbin']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out)
-                elif loss_type in ['Point', 'Tweedie', 'Poisson']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
-                elif loss_type in ['Quantile']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
+                # rescale io
+                y_true, y_pred = rescale_io(y_batch, test_out, scale)
+                test_metric.update_state(y_true, y_pred)
+
+                # if loss_type in ['Normal', 'Negbin']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out)
+                # elif loss_type in ['Point', 'Tweedie', 'Poisson']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
+                # elif loss_type in ['Quantile']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
                 with test_summary_writer.as_default():
-                    tf.summary.scalar('loss', test_loss_avg.result(), step=epoch)
-                    tf.summary.scalar('accuracy', test_metric.result(), step=epoch)
+                    tf.summary.scalar('loss', test_loss_avg.result(), step=(i + 1) * (epoch + 1))
+                    tf.summary.scalar('accuracy', test_metric.result(), step=(i + 1) * (epoch + 1))
 
             print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
                                                                                                        train_loss_avg.result().numpy(),
                                                                                                        test_loss_avg.result().numpy(),
                                                                                                        train_metric.result().numpy(),
                                                                                                        test_metric.result().numpy()))
 
@@ -1414,21 +1507,25 @@
             else:
                 prev_min_loss = np.min(test_loss_results[:-1])
             current_min_loss = np.min(test_loss_results)
             delta = current_min_loss - prev_min_loss
 
             print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
             # track & save best model
-            if ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
+            if ((test_loss_results[-1] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
                 best_model = model_path
                 tf.keras.models.save_model(model, model_path)
                 # reset time_since_improvement
                 time_since_improvement = 0
             else:
                 time_since_improvement += 1
+                train_loss_results.pop()
+                test_loss_results.pop()
+                train_metric_results.pop()
+                test_metric_results.pop()
 
             model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
             print("Best Model: ", best_model)
 
             # remove older models
             if len(model_list) > patience:
                 for m in model_list[:-patience]:
@@ -1442,112 +1539,19 @@
                 print("Terminating Training. Best Model path: {}".format(best_model))
                 model_tracker_file.close()
                 break
 
             # write after each epoch
             model_tracker_file.flush()
     else:
-        # train loop
-        for epoch in range(max_epochs):
-            print("Epoch {}/{}". format(epoch, max_epochs))
-            for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
-                if step > train_steps_per_epoch:
-                    break
-                else:
-                    train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
-                    out_len = tf.shape(train_out)[1]
-                    train_loss_avg.update_state(train_loss)
-                    if loss_type in ['Normal', 'Negbin']:
-                        train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
-                    elif loss_type in ['Point', 'Tweedie', 'Poisson']:
-                        train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
-                    elif loss_type in ['Quantile']:
-                        train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
-                    with train_summary_writer.as_default():
-                        tf.summary.scalar('loss', train_loss_avg.result(), step=epoch)
-                        tf.summary.scalar('accuracy', train_metric.result(), step=epoch)
-
-            for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
-                if step > train_steps_per_epoch:
-                    break
-                else:
-                    test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
-                    out_len = tf.shape(test_out)[1]
-                    test_loss_avg.update_state(test_loss)
-                    if loss_type in ['Normal', 'Negbin']:
-                        test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
-                    elif loss_type in ['Point', 'Tweedie', 'Poisson']:
-                        test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
-                    elif loss_type in ['Quantile']:
-                        test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
-                    with test_summary_writer.as_default():
-                        tf.summary.scalar('loss', test_loss_avg.result(), step=epoch)
-                        tf.summary.scalar('accuracy', test_metric.result(), step=epoch)
-
-            print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
-                                                                                                        train_loss_avg.result().numpy(),
-                                                                                                        test_loss_avg.result().numpy(),
-                                                                                                        train_metric.result().numpy(),
-                                                                                                        test_metric.result().numpy()))
-
-            # record losses & metric in lists
-            train_loss_results.append(train_loss_avg.result().numpy())
-            train_metric_results.append(train_metric.result().numpy())
-            test_loss_results.append(test_loss_avg.result().numpy())
-            test_metric_results.append(test_metric.result().numpy())
-
-            # reset states
-            train_loss_avg.reset_states()
-            train_metric.reset_states()
-            test_loss_avg.reset_states()
-            test_metric.reset_states()
-
-            # Save Model
-            model_path = model_prefix + '_' + str(epoch)
-            model_list.append(model_path)
-
-            if epoch == 0:
-                prev_min_loss = np.min(test_loss_results)
-            else:
-                prev_min_loss = np.min(test_loss_results[:-1])
-            current_min_loss = np.min(test_loss_results)
-            delta = current_min_loss - prev_min_loss
+        print("Only static dataset supported. Use prefill_buffers=True")
 
-            print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
-            # track & save best model
-            if ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
-                best_model = model_path
-                tf.keras.models.save_model(model, model_path)
-                # reset time_since_improvement
-                time_since_improvement = 0
-            else:
-                time_since_improvement += 1
-
-            model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
-            print("Best Model: ", best_model)
-
-            # remove older models
-            if len(model_list)>patience:
-                for m in model_list[:-patience]:
-                    if m != best_model:
-                        try:
-                            shutil.rmtree(m)
-                        except:
-                            pass
-
-            if (time_since_improvement > patience) and (epoch > min_epochs):
-                print("Terminating Training. Best Model path: {}".format(best_model))
-                model_tracker_file.close()
-                break
+    return best_model
 
-            # write after each epoch
-            model_tracker_file.flush()
 
-    return best_model
-        
 def TFT_Infer(model, inputs, loss_type, hist_len, f_len, target_index, num_quantiles):
     infer_tensor, scale, id_arr, date_arr = inputs
 
     s_dim = scale.shape[-1]
 
     if s_dim == 1:
         scale = scale[:, -1:, -1]
@@ -1661,51 +1665,61 @@
     #decoder_wts_df = pd.concat([pd.DataFrame(id_arr.reshape(-1,1)), decoder_wts_df], axis=1)
 
     print(stat_wts_df.shape, encoder_wts_df.shape, decoder_wts_df.shape)
         
     return forecast_df, stat_wts_df, encoder_wts_df, decoder_wts_df
 
 
-class Temporal_Fusion_Transformer:
+class Feature_Weighted_ConvTransformer:
     def __init__(self, 
                  col_index_dict,
                  vocab_dict,
                  num_layers,
                  num_heads,
+                 kernel_sizes,
                  d_model,
                  forecast_horizon,
                  max_inp_len,
                  loss_type,
                  num_quantiles=1,
-                 decoder_start_tokens=1,
+                 decoder_lags=1,
                  dropout_rate=0.1,
                  seed=None,
                  deterministic_ops=False):
         
         self.col_index_dict = col_index_dict
         self.vocab_dict = vocab_dict
         self.num_layers = num_layers
         self.num_heads = num_heads
+        self.kernel_sizes = kernel_sizes  #not used -- using lstm instead
         self.d_model = d_model
         self.forecast_horizon = forecast_horizon
         self.max_inp_len = max_inp_len
         self.loss_type = loss_type
         self.num_quantiles = num_quantiles
         self.dropout_rate = dropout_rate
-        self.decoder_start_tokens = decoder_start_tokens
+        self.decoder_start_tokens = decoder_lags
         self.target_col_name, self.target_index = self.col_index_dict.get('target_index')
         self.seed = seed
         self.allow_deterministic_ops = deterministic_ops
 
     def set_seed(self):
         tf.keras.utils.set_random_seed(self.seed)
         if self.allow_deterministic_ops:
             print("Deterministic Ops enabled.")
-            os.environ["TF_DETERMINISTIC_OPS"] = "True"
-            os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
+            if platform == "linux" or platform == "linux2":
+              print("GPU/CPU Determinism enabled for Linux")
+              os.environ["TF_DETERMINISTIC_OPS"] = "True"
+            else:
+              print("GPU/CPU Determinism partially enabled for Windows & Others")
+              os.environ["TF_DETERMINISTIC_OPS"] = "True"
+              os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
+        else:
+            print("Deterministic Ops disabled.")
+            os.environ["TF_DETERMINISTIC_OPS"] = "False"
 
     def build(self):
         tf.keras.backend.clear_session()
         if self.seed is None:
             print("No seed set for deterministic weights initialization")
         else:
             print("Using seed {} for weights initialization".format(self.seed))
@@ -1727,15 +1741,15 @@
               train_dataset, 
               test_dataset,
               loss_function, 
               metric='MSE',
               learning_rate=0.0001,
               max_epochs=100,
               min_epochs=10,
-              prefill_buffers=False,
+              prefill_buffers=True,
               num_train_samples=200000,
               num_test_samples=50000,
               train_batch_size=64,
               test_batch_size=128,
               train_steps_per_epoch=200,
               test_steps_per_epoch=100,
               patience=10,
@@ -1747,19 +1761,19 @@
               clipnorm=None,
               min_delta=0.0001,
               shuffle=True):
 
         if load_model is None:
             # Initialize Weights
             for x,y,s,w in train_dataset.take(1):
-                self.model(x, training=False)
+                self.model(x[0:2], training=False)
         else:
             # Initialize Weights
             for x, y, s, w in train_dataset.take(1):
-                self.model(x, training=False)
+                self.model(x[0:2], training=False)
             saved_model = tf.keras.models.load_model(load_model)
             self.model.set_weights(saved_model.get_weights())
             del saved_model
             gc.collect()
             print("Saved model: {} loaded. Continuing training ...".format(load_model))
 
         best_model = TFT_Train(self.model, 
@@ -1781,19 +1795,21 @@
                                patience,
                                weighted_training,
                                model_prefix,
                                logdir,
                                opt,
                                clipnorm,
                                min_delta,
-                               shuffle)
+                               shuffle,
+                               self.allow_deterministic_ops)
         return best_model
     
     def load(self, model_path):
         tf.keras.backend.clear_session()
         self.model = tf.keras.models.load_model(model_path)
         
-    def infer(self, inputs):
+    def infer(self, inputs, recursive_decode=True):
+        # recursive decode not used
         forecast, stat_wts_df, encoder_wts_df, decoder_wts_df = TFT_Infer(self.model, inputs, self.loss_type, self.max_inp_len, self.forecast_horizon, self.target_index, self.num_quantiles)
         
         return forecast, [stat_wts_df, encoder_wts_df, decoder_wts_df]
```

### Comparing `fmldk-1.2.4/tft/tft_model_v0.1.26.py` & `fmldk-1.2.5/tft/tft_model_v0.1.26.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_model_v0.1.31.py` & `fmldk-1.2.5/tft/tft_model_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft/tft_model_v1.1.3.py` & `fmldk-1.2.5/tft/tft_model_v1.1.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft_gpu/tft_data_gpu.py` & `fmldk-1.2.5/tft_gpu/tft_data_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft_gpu/tft_losses_gpu.py` & `fmldk-1.2.5/tft_gpu/tft_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.4/tft_gpu/tft_model_gpu.py` & `fmldk-1.2.5/tft/tft_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-
 import numpy as np
 import math as m
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import shutil
 import pickle
 import absl.logging
 absl.logging.set_verbosity(absl.logging.ERROR)
 import pandas as pd
 import gc
 import os
-from sys import platform
-
 
 # Distribution Sampling functions
 
 # negbin
 def negbin_sample(mu, alpha, n_samples=1):
     tol = 1e-5
     r = 1.0 / alpha
@@ -59,14 +56,63 @@
     return tf.reduce_mean(dist.sample(sample_shape=n_samples), axis=0)
 
 # Gumbel
 def GumbelSample(a, b, n_samples=1):
     dist = tfd.Gumbel(loc=a, scale=b)
     return tf.reduce_mean(tf.stop_gradient(dist.sample(sample_shape=n_samples)), axis=0)
 
+# Quantile Risk Metric (MSE & MAE Metrics are available out of the box in tf)
+class q_risk(tf.keras.metrics.Metric):
+    def __init__(self, name='q_risk', q=[0.5], **kwargs):
+        super(q_risk, self).__init__(name=name, **kwargs)
+        self.q = q
+        self.qrisk = self.add_weight(name='qrisk_' + str(q), initializer='zeros')
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+
+        n_quantiles = y_pred.shape.as_list()[-1]
+        assert len(self.q) == n_quantiles
+
+        qr = 0
+        for q, qr_quantile in zip(range(n_quantiles), self.q):
+            qr += self.q_risk_function(y_true, y_pred[:, :, q:q + 1], qr_quantile)
+
+        if sample_weight is not None:
+            raise ValueError("Weighted q-risk not implemented.")
+            #sample_weight = tf.cast(sample_weight, self.dtype)
+            #sample_weight = tf.broadcast_to(sample_weight, values.shape)
+            #values = tf.multiply(values, sample_weight)
+
+        self.qrisk.assign_add(tf.reduce_mean(qr))
+
+    def q_risk_function(self, y_true, y_pred, qr_quantile):
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+        qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+            tf.cast(0, tf.float32), (y_pred - y_true))
+        qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+        return qr_scaled
+
+    def result(self):
+        return self.qrisk
+
+
+def q_risk_function(y_true, y_pred, qr_quantile):
+    y_true = tf.cast(y_true, tf.float32)
+    y_pred = tf.cast(y_pred, tf.float32)
+
+    qr = qr_quantile * tf.maximum(tf.cast(0, tf.float32), (y_true - y_pred)) + (1 - qr_quantile) * tf.maximum(
+        tf.cast(0, tf.float32), (y_pred - y_true))
+    qr_scaled = 2 * tf.reduce_mean(qr) / tf.reduce_mean(tf.abs(y_true))
+
+    return qr_scaled
+
 
 # Self-Attention
 def ScaledDotProductAttention(q, k, v, causal_mask, padding_mask):
     matmul_qk = tf.matmul(q, k, transpose_b=True)  # (..., seq_len_q, seq_len_k)
     dk = tf.cast(tf.shape(k)[-1], tf.float32)
     scaled_attention_logits = matmul_qk / tf.math.sqrt(dk)
     
@@ -1100,19 +1146,18 @@
               test_batch_size,
               train_steps_per_epoch,
               test_steps_per_epoch,
               patience,
               weighted_training,
               model_prefix,
               logdir,
-              opt,
-              clipnorm,
-              min_delta,
-              shuffle,
-              deterministic):
+              opt=None,
+              clipnorm=None,
+              min_delta=0.0001,
+              shuffle=True):
     """
      train_dataset, test_dataset: tf.data.Dataset iterator for train & test datasets 
      loss_type: One of ['Point','Quantile','Normal','Poisson','Negbin']
      loss_function: One of the supported loss functions in loss library
      metric: 'MAE' or 'MSE' 
      max_epochs: Max. training epochs
      min_epochs: Min. Training epochs
@@ -1122,16 +1167,16 @@
      logdir: tensorflow training logs for tensorboard
         
     """
     @tf.function
     def trainstep(model, optimizer, x_train, y_train, scale, wts, training):
         with tf.GradientTape() as tape:
             o, s, f = model(x_train, training=training)
-            out_len = tf.shape(s)[1]
-            s_dim = tf.shape(scale)[-1]
+            out_len = s.shape.as_list()[1]  # tf.shape(s)[1]
+            s_dim = scale.shape.as_list()[-1]  # tf.shape(scale)[-1]
             if loss_type in ['Normal', 'Negbin']:
                 if s_dim == 1:
                     if weighted_training:
                         loss = loss_function(y_train * scale[:, -out_len:, :], [s, wts])
                     else:
                         loss = loss_function(y_train * scale[:, -out_len:, :], s)
                 else:
@@ -1213,39 +1258,89 @@
             if weighted_training:                               
                 loss = loss_function(y_test, [o, wts])
             else:
                 loss = loss_function(y_test, o)                                   
         else:
             raise ValueError("Invalid loss_type specified!")        
         return loss, o
+
+    def rescale_io(y_true, y_pred, scale):
+
+        out_len = y_true.shape.as_list()[1]
+        s_dim = scale.shape.as_list()[-1]
+
+        if loss_type in ['Point', 'Tweedie', 'Poisson']:
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred * scale[:, -out_len:, :]
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                y_pred_rescaled = y_pred * s_std + s_mean
+
+        elif loss_type in ['Quantile']:
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred * scale[:, -out_len:, :]
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                # rescale each quantile
+                n_quantiles = y_pred.shape.as_list()[-1]
+                y_list = []
+                for q in range(n_quantiles):
+                    y = y_pred[:, :, q:q + 1] * s_std + s_mean
+                    y_list.append(y)
+                y_pred_rescaled = tf.concat(y_list, axis=-1)
+
+        elif loss_type in ['Normal', 'Negbin']:
+            # predictions are already rescaled
+            if s_dim == 1:
+                y_true_rescaled = y_true * scale[:, -out_len:, :]
+                y_pred_rescaled = y_pred
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                y_true_rescaled = y_true * s_std + s_mean
+                y_pred_rescaled = y_pred
+
+        return y_true_rescaled, y_pred_rescaled
        
     # training specific vars
     if opt is None:
         optimizer = tf.keras.optimizers.Nadam(learning_rate=learning_rate)
     else:
         optimizer = opt
         optimizer.learning_rate=learning_rate
     
     if clipnorm is None:
         pass
     else:
-        optimizer.global_clipnorm = clipnorm
+        optimizer.clipnorm = clipnorm
        
     print("lr: ",optimizer.learning_rate.numpy())
     
     # model loss & metric
     train_loss_avg = tf.keras.metrics.Mean('train_loss', dtype=tf.float32)
     test_loss_avg = tf.keras.metrics.Mean('test_loss', dtype=tf.float32)
 
     if metric == 'MAE':  
         train_metric = tf.keras.metrics.MeanAbsoluteError('train_mae')
         test_metric = tf.keras.metrics.MeanAbsoluteError('test_mae')
+
     elif metric == 'MSE':
         train_metric = tf.keras.metrics.MeanSquaredError('train_mse')
         test_metric = tf.keras.metrics.MeanSquaredError('test_mse')
+
+    elif isinstance(metric, list):
+        train_metric = q_risk(name='train_qrisk', q=metric)
+        test_metric = q_risk(name='test_qrisk', q=metric)
+
     else:
         raise ValueError("{}: Not a Supported Metric".format(metric))
             
     #logging
     train_log_dir = str(logdir).rstrip('/') +'/train'
     test_log_dir = str(logdir).rstrip('/')+'/test'
     train_summary_writer = tf.summary.create_file_writer(train_log_dir)
@@ -1286,25 +1381,31 @@
     model_list = []
     best_model = None
     time_since_improvement = 0
     #####################################################################
 
     if prefill_buffers:
         print("prefetching training samples ... ")
-       
+        # get batch size
+        batch_size = 0
+        for x, y, s, w in train_dataset.take(1):
+            batch_size = int(x.shape[0])
+
         x_train = []
         y_train = []
         train_scale = []
         train_wts = []
         for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
             x_train.append(x_batch)
             y_train.append(y_batch)
             train_scale.append(scale)
             train_wts.append(wts)
-           
+            if (step + 1) * batch_size >= num_train_samples:
+                break
+
         # concat
         x_train = tf.concat(x_train, axis=0)
         y_train = tf.concat(y_train, axis=0)
         train_scale = tf.concat(train_scale, axis=0)
         train_wts = tf.concat(train_wts, axis=0)
         print("Training Samples Gathered: ", x_train.shape[0])
 
@@ -1314,63 +1415,75 @@
         test_scale = []
         test_wts = []
         for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
             x_test.append(x_batch)
             y_test.append(y_batch)
             test_scale.append(scale)
             test_wts.append(wts)
-           
+            if (step + 1) * batch_size >= num_test_samples:
+                break
+
         # concat
         x_test = tf.concat(x_test, axis=0)
         y_test = tf.concat(y_test, axis=0)
         test_scale = tf.concat(test_scale, axis=0)
         test_wts = tf.concat(test_wts, axis=0)
         print("Test Samples Gathered: ", x_test.shape[0])
 
         # chained tf.data.pipeline
         trainset = tf.data.Dataset.from_tensor_slices((x_train, y_train, train_scale, train_wts))
         trainset = trainset.shuffle(buffer_size=int(x_train.shape[0]), reshuffle_each_iteration=shuffle)
-        trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
-        trainset = trainset.prefetch(buffer_size = tf.data.AUTOTUNE)
-        
+        trainset = trainset.batch(batch_size=train_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE)
+        trainset = trainset.prefetch(buffer_size=tf.data.AUTOTUNE)
+
         testset = tf.data.Dataset.from_tensor_slices((x_test, y_test, test_scale, test_wts))
-        testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=False)
-        testset = testset.batch(batch_size=test_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE, deterministic=deterministic)
-        testset = testset.prefetch(buffer_size = tf.data.AUTOTUNE)
-        
+        testset = testset.shuffle(buffer_size=int(x_test.shape[0]), reshuffle_each_iteration=shuffle)
+        testset = testset.batch(batch_size=test_batch_size, drop_remainder=False, num_parallel_calls=tf.data.AUTOTUNE)
+        testset = testset.prefetch(buffer_size=tf.data.AUTOTUNE)
+
         for epoch in range(max_epochs):
             print("Epoch {}/{}".format(epoch, max_epochs))
-           
+
             for i, (x_batch, y_batch, scale, wts) in enumerate(trainset):
                 train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
-                out_len = tf.shape(train_out)[1]
                 train_loss_avg.update_state(train_loss)
-                if loss_type in ['Normal', 'Negbin']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out)
-                elif loss_type in ['Point', 'Poisson', 'Tweedie']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
-                elif loss_type in ['Quantile']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
+                # rescale io & update metric
+                y_true, y_pred = rescale_io(y_batch, train_out, scale)
+                train_metric.update_state(y_true, y_pred)
+
+                # if loss_type in ['Normal', 'Negbin']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out)
+                # elif loss_type in ['Point', 'Poisson', 'Tweedie']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
+                # elif loss_type in ['Quantile']:
+                #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
                 with train_summary_writer.as_default():
-                    tf.summary.scalar('loss', train_loss_avg.result(), step=(i+1)*(epoch+1))
-                    tf.summary.scalar('accuracy', train_metric.result(), step=(i+1)*(epoch+1))
+                    tf.summary.scalar('loss', train_loss_avg.result(), step=(i + 1) * (epoch + 1))
+                    tf.summary.scalar('accuracy', train_metric.result(), step=(i + 1) * (epoch + 1))
 
             for i, (x_batch, y_batch, scale, wts) in enumerate(testset):
-                test_loss, test_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=False)
-                out_len = tf.shape(test_out)[1]
+                test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
                 test_loss_avg.update_state(test_loss)
-                if loss_type in ['Normal', 'Negbin']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out)
-                elif loss_type in ['Point', 'Tweedie', 'Poisson']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
-                elif loss_type in ['Quantile']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
+                # rescale io
+                y_true, y_pred = rescale_io(y_batch, test_out, scale)
+                test_metric.update_state(y_true, y_pred)
+
+                # if loss_type in ['Normal', 'Negbin']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out)
+                # elif loss_type in ['Point', 'Tweedie', 'Poisson']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
+                # elif loss_type in ['Quantile']:
+                #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
                 with test_summary_writer.as_default():
-                    tf.summary.scalar('loss', test_loss_avg.result(), step=(i+1)*(epoch+1))
-                    tf.summary.scalar('accuracy', test_metric.result(), step=(i+1)*(epoch+1))
+                    tf.summary.scalar('loss', test_loss_avg.result(), step=(i + 1) * (epoch + 1))
+                    tf.summary.scalar('accuracy', test_metric.result(), step=(i + 1) * (epoch + 1))
 
             print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
                                                                                                        train_loss_avg.result().numpy(),
                                                                                                        test_loss_avg.result().numpy(),
                                                                                                        train_metric.result().numpy(),
                                                                                                        test_metric.result().numpy()))
 
@@ -1395,21 +1508,25 @@
             else:
                 prev_min_loss = np.min(test_loss_results[:-1])
             current_min_loss = np.min(test_loss_results)
             delta = current_min_loss - prev_min_loss
 
             print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
             # track & save best model
-            if ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
+            if ((test_loss_results[-1] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
                 best_model = model_path
                 tf.keras.models.save_model(model, model_path)
                 # reset time_since_improvement
                 time_since_improvement = 0
             else:
                 time_since_improvement += 1
+                train_loss_results.pop()
+                test_loss_results.pop()
+                train_metric_results.pop()
+                test_metric_results.pop()
 
             model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
             print("Best Model: ", best_model)
 
             # remove older models
             if len(model_list) > patience:
                 for m in model_list[:-patience]:
@@ -1423,19 +1540,126 @@
                 print("Terminating Training. Best Model path: {}".format(best_model))
                 model_tracker_file.close()
                 break
 
             # write after each epoch
             model_tracker_file.flush()
     else:
-        print("Only static dataset supported. Use prefill_buffers=True")
-    
+        # train loop
+        for epoch in range(max_epochs):
+            print("Epoch {}/{}". format(epoch, max_epochs))
+            for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
+                if step > train_steps_per_epoch:
+                    break
+                else:
+                    train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
+                    train_loss_avg.update_state(train_loss)
+
+                    # rescale io & update metric
+                    y_true, y_pred = rescale_io(y_batch, train_out, scale)
+                    train_metric.update_state(y_true, y_pred)
+
+                    #if loss_type in ['Normal', 'Negbin']:
+                    #    train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
+                    #elif loss_type in ['Point', 'Tweedie', 'Poisson']:
+                    #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
+                    #elif loss_type in ['Quantile']:
+                    #    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
+                    with train_summary_writer.as_default():
+                        tf.summary.scalar('loss', train_loss_avg.result(), step=epoch)
+                        tf.summary.scalar('accuracy', train_metric.result(), step=epoch)
+
+            for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
+                if step > train_steps_per_epoch:
+                    break
+                else:
+                    test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
+                    test_loss_avg.update_state(test_loss)
+
+                    # rescale io
+                    y_true, y_pred = rescale_io(y_batch, test_out, scale)
+                    test_metric.update_state(y_true, y_pred)
+
+                    #if loss_type in ['Normal', 'Negbin']:
+                    #    test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
+                    #elif loss_type in ['Point', 'Tweedie', 'Poisson']:
+                    #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
+                    #elif loss_type in ['Quantile']:
+                    #    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
+
+                    with test_summary_writer.as_default():
+                        tf.summary.scalar('loss', test_loss_avg.result(), step=epoch)
+                        tf.summary.scalar('accuracy', test_metric.result(), step=epoch)
+
+            print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
+                                                                                                        train_loss_avg.result().numpy(),
+                                                                                                        test_loss_avg.result().numpy(),
+                                                                                                        train_metric.result().numpy(),
+                                                                                                        test_metric.result().numpy()))
+
+            # record losses & metric in lists
+            train_loss_results.append(train_loss_avg.result().numpy())
+            train_metric_results.append(train_metric.result().numpy())
+            test_loss_results.append(test_loss_avg.result().numpy())
+            test_metric_results.append(test_metric.result().numpy())
+
+            # reset states
+            train_loss_avg.reset_states()
+            train_metric.reset_states()
+            test_loss_avg.reset_states()
+            test_metric.reset_states()
+
+            # Save Model
+            model_path = model_prefix + '_' + str(epoch)
+            model_list.append(model_path)
+
+            if epoch == 0:
+                prev_min_loss = np.min(test_loss_results)
+            else:
+                prev_min_loss = np.min(test_loss_results[:-1])
+            current_min_loss = np.min(test_loss_results)
+            delta = current_min_loss - prev_min_loss
+
+            print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
+            # track & save best model
+            if ((test_loss_results[-1] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
+                best_model = model_path
+                tf.keras.models.save_model(model, model_path)
+                # reset time_since_improvement
+                time_since_improvement = 0
+            else:
+                time_since_improvement += 1
+                train_loss_results.pop()
+                test_loss_results.pop()
+                train_metric_results.pop()
+                test_metric_results.pop()
+
+            model_tracker_file.write('best_model path after epochs ' + str(epoch) + ': ' + best_model + '\n')
+            print("Best Model: ", best_model)
+
+            # remove older models
+            if len(model_list)>patience:
+                for m in model_list[:-patience]:
+                    if m != best_model:
+                        try:
+                            shutil.rmtree(m)
+                        except:
+                            pass
+
+            if (time_since_improvement > patience) and (epoch > min_epochs):
+                print("Terminating Training. Best Model path: {}".format(best_model))
+                model_tracker_file.close()
+                break
+
+            # write after each epoch
+            model_tracker_file.flush()
+
     return best_model
         
-    
 def TFT_Infer(model, inputs, loss_type, hist_len, f_len, target_index, num_quantiles):
     infer_tensor, scale, id_arr, date_arr = inputs
 
     s_dim = scale.shape[-1]
 
     if s_dim == 1:
         scale = scale[:, -1:, -1]
@@ -1584,24 +1808,16 @@
         self.seed = seed
         self.allow_deterministic_ops = deterministic_ops
 
     def set_seed(self):
         tf.keras.utils.set_random_seed(self.seed)
         if self.allow_deterministic_ops:
             print("Deterministic Ops enabled.")
-            if platform == "linux" or platform == "linux2":
-              print("GPU/CPU Determinism enabled for Linux")
-              os.environ["TF_DETERMINISTIC_OPS"] = "True"
-            else:
-              print("GPU/CPU Determinism partially enabled for Windows & Others")
-              os.environ["TF_DETERMINISTIC_OPS"] = "True"
-              os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
-        else:
-            print("Deterministic Ops disabled.")
-            os.environ["TF_DETERMINISTIC_OPS"] = "False"
+            os.environ["TF_DETERMINISTIC_OPS"] = "True"
+            os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
 
     def build(self):
         tf.keras.backend.clear_session()
         if self.seed is None:
             print("No seed set for deterministic weights initialization")
         else:
             print("Using seed {} for weights initialization".format(self.seed))
@@ -1623,15 +1839,15 @@
               train_dataset, 
               test_dataset,
               loss_function, 
               metric='MSE',
               learning_rate=0.0001,
               max_epochs=100,
               min_epochs=10,
-              prefill_buffers=False,
+              prefill_buffers=True,
               num_train_samples=200000,
               num_test_samples=50000,
               train_batch_size=64,
               test_batch_size=128,
               train_steps_per_epoch=200,
               test_steps_per_epoch=100,
               patience=10,
@@ -1643,19 +1859,19 @@
               clipnorm=None,
               min_delta=0.0001,
               shuffle=True):
 
         if load_model is None:
             # Initialize Weights
             for x,y,s,w in train_dataset.take(1):
-                self.model(x[0:2], training=False)
+                self.model(x, training=False)
         else:
             # Initialize Weights
             for x, y, s, w in train_dataset.take(1):
-                self.model(x[0:2], training=False)
+                self.model(x, training=False)
             saved_model = tf.keras.models.load_model(load_model)
             self.model.set_weights(saved_model.get_weights())
             del saved_model
             gc.collect()
             print("Saved model: {} loaded. Continuing training ...".format(load_model))
 
         best_model = TFT_Train(self.model, 
@@ -1677,16 +1893,15 @@
                                patience,
                                weighted_training,
                                model_prefix,
                                logdir,
                                opt,
                                clipnorm,
                                min_delta,
-                               shuffle,
-                               self.allow_deterministic_ops)
+                               shuffle)
         return best_model
     
     def load(self, model_path):
         tf.keras.backend.clear_session()
         self.model = tf.keras.models.load_model(model_path)
         
     def infer(self, inputs):
```

